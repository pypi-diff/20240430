# Comparing `tmp/saltstack_age-0.1.1-py3-none-any.whl.zip` & `tmp/saltstack_age-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5521 bytes, number of entries: 11
+Zip file size: 6133 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 saltstack_age/__init__.py
--rw-r--r--  2.0 unx     4672 b- defN 20-Feb-02 00:00 saltstack_age/cli.py
--rw-r--r--  2.0 unx      309 b- defN 20-Feb-02 00:00 saltstack_age/identities.py
+-rw-r--r--  2.0 unx     6101 b- defN 20-Feb-02 00:00 saltstack_age/cli.py
+-rw-r--r--  2.0 unx      752 b- defN 20-Feb-02 00:00 saltstack_age/identities.py
 -rw-r--r--  2.0 unx      109 b- defN 20-Feb-02 00:00 saltstack_age/passphrase.py
--rw-r--r--  2.0 unx     1561 b- defN 20-Feb-02 00:00 saltstack_age/secure_value.py
+-rw-r--r--  2.0 unx     1279 b- defN 20-Feb-02 00:00 saltstack_age/secure_value.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 saltstack_age/renderers/__init__.py
--rw-r--r--  2.0 unx     1672 b- defN 20-Feb-02 00:00 saltstack_age/renderers/age.py
-?rw-r--r--  2.0 unx      345 b- defN 20-Feb-02 00:00 saltstack_age-0.1.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 saltstack_age-0.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx      102 b- defN 20-Feb-02 00:00 saltstack_age-0.1.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      909 b- defN 20-Feb-02 00:00 saltstack_age-0.1.1.dist-info/RECORD
-11 files, 9766 bytes uncompressed, 3967 bytes compressed:  59.4%
+-rw-r--r--  2.0 unx     2355 b- defN 20-Feb-02 00:00 saltstack_age/renderers/age.py
+?rw-r--r--  2.0 unx      345 b- defN 20-Feb-02 00:00 saltstack_age-0.2.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 saltstack_age-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      102 b- defN 20-Feb-02 00:00 saltstack_age-0.2.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      909 b- defN 20-Feb-02 00:00 saltstack_age-0.2.0.dist-info/RECORD
+11 files, 12039 bytes uncompressed, 4579 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: saltstack_age/renderers/__init__.py
 Comment: 
 
 Filename: saltstack_age/renderers/age.py
 Comment: 
 
-Filename: saltstack_age-0.1.1.dist-info/METADATA
+Filename: saltstack_age-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: saltstack_age-0.1.1.dist-info/WHEEL
+Filename: saltstack_age-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: saltstack_age-0.1.1.dist-info/entry_points.txt
+Filename: saltstack_age-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: saltstack_age-0.1.1.dist-info/RECORD
+Filename: saltstack_age-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## saltstack_age/cli.py

```diff
@@ -1,42 +1,43 @@
 import logging
 import sys
 from argparse import ArgumentParser, ArgumentTypeError, Namespace
 from base64 import b64encode
 from collections.abc import Sequence
 from getpass import getpass
 from pathlib import Path
+from typing import Literal
 
 import pyrage
 
-from saltstack_age.identities import read_identity_file
+from saltstack_age.identities import get_identity_from_environment, read_identity_file
 from saltstack_age.passphrase import get_passphrase_from_environment
 from saltstack_age.secure_value import (
     IdentitySecureValue,
     parse_secure_value,
 )
 
 LOGGER = logging.getLogger(__name__)
 
 
-def normalize_identity(identity: str) -> Path:
+def normalize_identity(identity: str) -> pyrage.x25519.Identity:
     path = Path(identity)
 
     if path.is_file():
-        return path
+        return read_identity_file(path)
 
     raise ArgumentTypeError(f"Identity file does not exist: {identity}")
 
 
 def parse_cli_arguments(args: Sequence[str] | None = None) -> Namespace:
     parser = ArgumentParser(
         description="Encrypt or decrypt secrets for use with saltstack-age renderer.",
-        epilog="When no passphrase or identity is provided, the tool defaults to "
-        "passphrase-based encryption and attempts to retrieve the passphrase from "
-        "the AGE_PASSPHRASE environment variable.",
+        epilog="When no passphrase or identity is provided, the tool tries to "
+        "retrieve a passphrase from the AGE_PASSPHRASE environment variable, "
+        "or an identity using the AGE_IDENTITY_FILE variable.",
     )
 
     type_parameters = parser.add_mutually_exclusive_group()
     _ = type_parameters.add_argument(
         "-i",
         "--identity",
         type=normalize_identity,
@@ -96,47 +97,85 @@
     if passphrase is None:
         LOGGER.critical("No age passphrase provided")
         raise SystemExit(-1)
 
     return passphrase
 
 
+def get_identities(arguments: Namespace) -> list[pyrage.x25519.Identity]:
+    identities: list[pyrage.x25519.Identity] = arguments.identities or []
+
+    # When no identity is provided on the CLI, try to get one from the environment
+    if not identities:
+        identity_from_environment = get_identity_from_environment()
+        if identity_from_environment:
+            LOGGER.debug("Found identity file in environment")
+            identities.append(identity_from_environment)
+
+    return identities
+
+
 def get_value(arguments: Namespace) -> str:
     return arguments.value or sys.stdin.read()
 
 
+def determine_encryption_type(
+    arguments: Namespace,
+) -> Literal["identity", "passphrase"]:
+    if arguments.passphrase or arguments.passphrase_from_stdin:
+        return "passphrase"
+    if arguments.identities:
+        return "identity"
+
+    # We want the tool to be easy to use, so there is a lot of guesswork.
+    # But we also want to avoid inconsistent behaviors.
+    # So in case no passphrase or identity is passed to CLI,
+    # but both are configured in the environment, we raise an error.
+    identities = get_identities(arguments)
+    passphrase = get_passphrase(arguments)
+    if identities and passphrase:
+        LOGGER.critical("Error: Found both passphrase and identity file in environment")
+        raise SystemExit(-1)
+
+    if identities:
+        return "identity"
+
+    return "passphrase"
+
+
 def encrypt(arguments: Namespace) -> None:
     value = get_value(arguments).encode()
 
-    if arguments.identities:
-        recipients = [
-            read_identity_file(identity).to_public()
-            for identity in arguments.identities
-        ]
+    if determine_encryption_type(arguments) == "identity":
+        recipients = [identity.to_public() for identity in get_identities(arguments)]
         ciphertext = pyrage.encrypt(value, recipients)
         LOGGER.info("ENC[age-identity,%s]", b64encode(ciphertext).decode())
 
     else:
         ciphertext = pyrage.passphrase.encrypt(value, get_passphrase(arguments))
         LOGGER.info("ENC[age-passphrase,%s]", b64encode(ciphertext).decode())
 
 
 def decrypt(arguments: Namespace) -> None:
     secure_value = parse_secure_value(get_value(arguments))
 
     if isinstance(secure_value, IdentitySecureValue):
-        if arguments.identities is None:
+        identities = get_identities(arguments)
+
+        if not identities:
             LOGGER.critical("An identity is required to decrypt this value")
             raise SystemExit(-1)
-        if len(arguments.identities) != 1:
+
+        if len(identities) != 1:
             LOGGER.critical(
                 "A single identity must be passed to decrypt this value (got %d)",
                 len(arguments.identities),
             )
             raise SystemExit(-1)
+
         LOGGER.info("%s", secure_value.decrypt(arguments.identities[0]))
 
     else:  # isinstance(secure_value, PassphraseSecureValue)
         LOGGER.info("%s", secure_value.decrypt(get_passphrase(arguments)))
 
 
 def main(cli_args: Sequence[str] | None = None) -> None:
```

## saltstack_age/identities.py

```diff
@@ -1,14 +1,34 @@
+import os
 import re
 from pathlib import Path
 
 import pyrage
 
 
-def read_identity_file(path: Path) -> pyrage.x25519.Identity:
+def read_identity_file(path: Path | str) -> pyrage.x25519.Identity:
+    if isinstance(path, str):
+        path = Path(path)
+
+    # Remove comments
     identity_string = re.sub(
         r"^#.*\n?",
         "",
         path.read_text(),
         flags=re.MULTILINE,
     ).rstrip("\n")
+
     return pyrage.x25519.Identity.from_str(identity_string)
+
+
+def get_identity_from_environment() -> pyrage.x25519.Identity | None:
+    path_string = os.environ.get("AGE_IDENTITY_FILE")
+
+    if path_string is None:
+        return None
+
+    path = Path(path_string)
+
+    if not path.is_file():
+        raise FileNotFoundError(f"AGE_IDENTITY_FILE does not exist: {path}")
+
+    return read_identity_file(path)
```

## saltstack_age/secure_value.py

```diff
@@ -1,16 +1,13 @@
 import re
 from base64 import b64decode
 from dataclasses import dataclass
-from pathlib import Path
 
 import pyrage
 
-from saltstack_age.identities import read_identity_file
-
 RE_SECURE_VALUE = re.compile(
     r"""
 ENC\[
 age-(?P<type>passphrase|identity)
 ,
 (?P<base64CipherText>
     (?:[A-Za-z0-9+/]{4})*
@@ -38,20 +35,16 @@
 
 class PassphraseSecureValue(SecureValue):
     def decrypt(self, passphrase: str) -> str:
         return pyrage.passphrase.decrypt(self.ciphertext, passphrase).decode()
 
 
 class IdentitySecureValue(SecureValue):
-    def decrypt(self, identity: Path | str) -> str:
-        if isinstance(identity, str):
-            identity = Path(identity)
-        if not identity.is_file():
-            raise FileNotFoundError(f"Identity file does not exist: {identity}")
-        return pyrage.decrypt(self.ciphertext, [read_identity_file(identity)]).decode()
+    def decrypt(self, identity: pyrage.x25519.Identity) -> str:
+        return pyrage.decrypt(self.ciphertext, [identity]).decode()
 
 
 def parse_secure_value(string: str) -> PassphraseSecureValue | IdentitySecureValue:
     match = RE_SECURE_VALUE.match(string)
 
     if not match:
         raise ValueError(f"Invalid secure value: {string}")
```

## saltstack_age/renderers/age.py

```diff
@@ -1,13 +1,16 @@
 from collections import OrderedDict
 from importlib import import_module
+from pathlib import Path
 from typing import Any
 
+import pyrage
 from salt.exceptions import SaltRenderError
 
+from saltstack_age.identities import get_identity_from_environment, read_identity_file
 from saltstack_age.passphrase import get_passphrase_from_environment
 from saltstack_age.secure_value import (
     IdentitySecureValue,
     is_secure_value,
     parse_secure_value,
 )
 
@@ -25,34 +28,53 @@
         _ = import_module("pyrage")
     except ModuleNotFoundError:
         return (False, "pyrage is not installed")
 
     return __virtualname__
 
 
-def _decrypt(string: str) -> str:
-    secure_value = parse_secure_value(string)
+def _get_identity() -> pyrage.x25519.Identity:
+    # 1. Try to get identity file from Salt configuration
+    identity_file_string: str | None = __salt__["config.get"]("age_identity_file")
+    if identity_file_string:
+        identity_file_path = Path(identity_file_string)
 
-    if isinstance(secure_value, IdentitySecureValue):
-        identity_file: str | None = __salt__["config.get"]("age_identity_file")
+        if not identity_file_path.is_file():
+            raise SaltRenderError(
+                f"age_identity file does not exist: {identity_file_string}"
+            )
 
-        if not identity_file:
-            raise SaltRenderError("age_identity_file is not defined")
+        return read_identity_file(identity_file_path)
 
-        return secure_value.decrypt(identity_file)
+    # 2. Try to get identity from the environment
+    identity = get_identity_from_environment()
+    if identity:
+        return identity
 
-    # secure_value is a PassphraseSecureValue
+    raise SaltRenderError("No age identity file found in config or environment")
+
+
+def _get_passphrase() -> str:
     passphrase: str | None = (
         __salt__["config.get"]("age_passphrase") or get_passphrase_from_environment()
     )
 
     if passphrase is None:
         raise SaltRenderError("No age passphrase found in config or environment")
 
-    return secure_value.decrypt(passphrase)
+    return passphrase
+
+
+def _decrypt(string: str) -> str:
+    secure_value = parse_secure_value(string)
+
+    if isinstance(secure_value, IdentitySecureValue):
+        return secure_value.decrypt(_get_identity())
+
+    return secure_value.decrypt(_get_passphrase())
 
 
 def render(
     data: Data,
     _saltenv: str = "base",
     _sls: str = "",
     **_kwargs: None,
```

## Comparing `saltstack_age-0.1.1.dist-info/RECORD` & `saltstack_age-0.2.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 saltstack_age/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-saltstack_age/cli.py,sha256=LNPgS0Me-FeBF1E6pZ4bMA5bcdUZIT_2fEHb-wglKNw,4672
-saltstack_age/identities.py,sha256=aBBja0zYHwnq2ia472FqMoYTSMSCOhM8OhrE-IKcVOw,309
+saltstack_age/cli.py,sha256=m3KsLULzEmiZ0r5IedtghwZCC-KEQ-AAeBKECAPe_uA,6101
+saltstack_age/identities.py,sha256=5RicnFmDsKtYVqjRlI2wl9qFNtTkcm9jHKrPJ_9bXj4,752
 saltstack_age/passphrase.py,sha256=GdV9TmaAsIL5b043x6w0IUN0iN273tXjq2eW9SOU6XY,109
-saltstack_age/secure_value.py,sha256=0xLrGp3tXklr3xWYPji03z8BrLIvDqEkmJZcyOMehuU,1561
+saltstack_age/secure_value.py,sha256=kxPLJAg_gv7DRn-C6Le2x6sqiLKJrB89vK8VcoiOFyU,1279
 saltstack_age/renderers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-saltstack_age/renderers/age.py,sha256=vityfXrEojd5QU7sC-YfyYFxJRpCnbO2KP1pezfV-9w,1672
-saltstack_age-0.1.1.dist-info/METADATA,sha256=7BCe8mxeUrI41QpRVUHJkQcyX-B2_jn2r101udf30cg,345
-saltstack_age-0.1.1.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-saltstack_age-0.1.1.dist-info/entry_points.txt,sha256=AI6n3Tyjmxxz9FzJFJHJhhhv-hHZGhSrHFFjgbV2zH0,102
-saltstack_age-0.1.1.dist-info/RECORD,,
+saltstack_age/renderers/age.py,sha256=S7J3DPq1Rtykg4T2Q-S6C46vRi1WEZVLG5rSXOmwF1Q,2355
+saltstack_age-0.2.0.dist-info/METADATA,sha256=6jtH1nR-qCxZFDR5XYGQs8sNJmlksi_18PETrpl7lqw,345
+saltstack_age-0.2.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+saltstack_age-0.2.0.dist-info/entry_points.txt,sha256=AI6n3Tyjmxxz9FzJFJHJhhhv-hHZGhSrHFFjgbV2zH0,102
+saltstack_age-0.2.0.dist-info/RECORD,,
```

