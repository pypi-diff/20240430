# Comparing `tmp/saltstack_age-0.2.3-py3-none-any.whl.zip` & `tmp/saltstack_age-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9097 bytes, number of entries: 11
+Zip file size: 9204 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 saltstack_age/__init__.py
--rw-r--r--  2.0 unx     6101 b- defN 20-Feb-02 00:00 saltstack_age/cli.py
+-rw-r--r--  2.0 unx     6052 b- defN 20-Feb-02 00:00 saltstack_age/cli.py
 -rw-r--r--  2.0 unx      752 b- defN 20-Feb-02 00:00 saltstack_age/identities.py
 -rw-r--r--  2.0 unx      109 b- defN 20-Feb-02 00:00 saltstack_age/passphrase.py
--rw-r--r--  2.0 unx     1279 b- defN 20-Feb-02 00:00 saltstack_age/secure_value.py
+-rw-r--r--  2.0 unx     1353 b- defN 20-Feb-02 00:00 saltstack_age/secure_value.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 saltstack_age/renderers/__init__.py
--rw-r--r--  2.0 unx     2355 b- defN 20-Feb-02 00:00 saltstack_age/renderers/age.py
-?rw-r--r--  2.0 unx     7489 b- defN 20-Feb-02 00:00 saltstack_age-0.2.3.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 saltstack_age-0.2.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx      102 b- defN 20-Feb-02 00:00 saltstack_age-0.2.3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      910 b- defN 20-Feb-02 00:00 saltstack_age-0.2.3.dist-info/RECORD
-11 files, 19184 bytes uncompressed, 7543 bytes compressed:  60.7%
+-rw-r--r--  2.0 unx     2522 b- defN 20-Feb-02 00:00 saltstack_age/renderers/age.py
+?rw-r--r--  2.0 unx     7489 b- defN 20-Feb-02 00:00 saltstack_age-0.3.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 saltstack_age-0.3.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      102 b- defN 20-Feb-02 00:00 saltstack_age-0.3.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      910 b- defN 20-Feb-02 00:00 saltstack_age-0.3.0.dist-info/RECORD
+11 files, 19376 bytes uncompressed, 7650 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: saltstack_age/renderers/__init__.py
 Comment: 
 
 Filename: saltstack_age/renderers/age.py
 Comment: 
 
-Filename: saltstack_age-0.2.3.dist-info/METADATA
+Filename: saltstack_age-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: saltstack_age-0.2.3.dist-info/WHEEL
+Filename: saltstack_age-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: saltstack_age-0.2.3.dist-info/entry_points.txt
+Filename: saltstack_age-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: saltstack_age-0.2.3.dist-info/RECORD
+Filename: saltstack_age-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## saltstack_age/cli.py

```diff
@@ -140,23 +140,23 @@
         return "identity"
 
     return "passphrase"
 
 
 def encrypt(arguments: Namespace) -> None:
     value = get_value(arguments).encode()
+    type_ = determine_encryption_type(arguments)
 
-    if determine_encryption_type(arguments) == "identity":
+    if type_ == "identity":
         recipients = [identity.to_public() for identity in get_identities(arguments)]
         ciphertext = pyrage.encrypt(value, recipients)
-        LOGGER.info("ENC[age-identity,%s]", b64encode(ciphertext).decode())
-
     else:
         ciphertext = pyrage.passphrase.encrypt(value, get_passphrase(arguments))
-        LOGGER.info("ENC[age-passphrase,%s]", b64encode(ciphertext).decode())
+
+    _ = sys.stdout.write(f"ENC[age-{type_},{b64encode(ciphertext).decode()}]\n")
 
 
 def decrypt(arguments: Namespace) -> None:
     secure_value = parse_secure_value(get_value(arguments))
 
     if isinstance(secure_value, IdentitySecureValue):
         identities = get_identities(arguments)
@@ -168,18 +168,18 @@
         if len(identities) != 1:
             LOGGER.critical(
                 "A single identity must be passed to decrypt this value (got %d)",
                 len(arguments.identities),
             )
             raise SystemExit(-1)
 
-        LOGGER.info("%s", secure_value.decrypt(arguments.identities[0]))
+        _ = sys.stdout.write(secure_value.decrypt(arguments.identities[0]))
 
     else:  # isinstance(secure_value, PassphraseSecureValue)
-        LOGGER.info("%s", secure_value.decrypt(get_passphrase(arguments)))
+        _ = sys.stdout.write(secure_value.decrypt(get_passphrase(arguments)))
 
 
 def main(cli_args: Sequence[str] | None = None) -> None:
     arguments = parse_cli_arguments(cli_args)
     configure_logging(debug=arguments.debug)
     LOGGER.debug("CLI arguments: %r", arguments)
     encrypt(arguments) if arguments.mode.startswith("enc") else decrypt(arguments)
```

## saltstack_age/secure_value.py

```diff
@@ -1,10 +1,11 @@
 import re
 from base64 import b64decode
 from dataclasses import dataclass
+from typing import Any
 
 import pyrage
 
 RE_SECURE_VALUE = re.compile(
     r"""
 ENC\[
 age-(?P<type>passphrase|identity)
@@ -20,16 +21,16 @@
 \]
 \s*
 """,
     re.VERBOSE,
 )
 
 
-def is_secure_value(string: str) -> bool:
-    return bool(RE_SECURE_VALUE.match(string))
+def is_secure_value(value: Any) -> bool:  # noqa: ANN401
+    return bool(RE_SECURE_VALUE.match(value)) if isinstance(value, str) else False
 
 
 @dataclass
 class SecureValue:
     ciphertext: bytes
```

## saltstack_age/renderers/age.py

```diff
@@ -1,11 +1,11 @@
 from collections import OrderedDict
 from importlib import import_module
 from pathlib import Path
-from typing import Any
+from typing import Any, cast
 
 import pyrage
 from salt.exceptions import SaltRenderError
 
 from saltstack_age.identities import get_identity_from_environment, read_identity_file
 from saltstack_age.passphrase import get_passphrase_from_environment
 from saltstack_age.secure_value import (
@@ -69,17 +69,22 @@
 
     if isinstance(secure_value, IdentitySecureValue):
         return secure_value.decrypt(_get_identity())
 
     return secure_value.decrypt(_get_passphrase())
 
 
+def _render_value(value: Any) -> Any:  # noqa: ANN401
+    if is_secure_value(value):
+        return _decrypt(value)
+    if isinstance(value, OrderedDict):
+        return render(cast(Data, value))
+    return value
+
+
 def render(
     data: Data,
     _saltenv: str = "base",
     _sls: str = "",
     **_kwargs: None,
 ) -> Data:
-    return OrderedDict(
-        (key, _decrypt(value) if is_secure_value(value) else value)
-        for key, value in data.items()
-    )
+    return OrderedDict((key, _render_value(value)) for key, value in data.items())
```

## Comparing `saltstack_age-0.2.3.dist-info/METADATA` & `saltstack_age-0.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: saltstack-age
-Version: 0.2.3
+Version: 0.3.0
 Summary: age renderer for Saltstack
 Project-URL: Homepage, https://github.com/pmuller/saltstack-age
 Project-URL: Repository, https://github.com/pmuller/saltstack-age.git
 Project-URL: Issues, https://github.com/pmuller/saltstack-age/issues
 Project-URL: Changelog, https://github.com/pmuller/saltstack-age/blob/main/CHANGELOG.md
 Author: Philippe Muller
 License: MIT License
```

## Comparing `saltstack_age-0.2.3.dist-info/RECORD` & `saltstack_age-0.3.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 saltstack_age/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-saltstack_age/cli.py,sha256=m3KsLULzEmiZ0r5IedtghwZCC-KEQ-AAeBKECAPe_uA,6101
+saltstack_age/cli.py,sha256=fFc-Ukt7R5N4VG0t54LuehEsNSrnZkwYM3pmJD3W3JE,6052
 saltstack_age/identities.py,sha256=5RicnFmDsKtYVqjRlI2wl9qFNtTkcm9jHKrPJ_9bXj4,752
 saltstack_age/passphrase.py,sha256=GdV9TmaAsIL5b043x6w0IUN0iN273tXjq2eW9SOU6XY,109
-saltstack_age/secure_value.py,sha256=kxPLJAg_gv7DRn-C6Le2x6sqiLKJrB89vK8VcoiOFyU,1279
+saltstack_age/secure_value.py,sha256=cFfaMPmXd8uBPt13ftwT3ENRl6RIsQxlFysHlRO7ljs,1353
 saltstack_age/renderers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-saltstack_age/renderers/age.py,sha256=S7J3DPq1Rtykg4T2Q-S6C46vRi1WEZVLG5rSXOmwF1Q,2355
-saltstack_age-0.2.3.dist-info/METADATA,sha256=9Y9rm1NDEuiBcBG6XQuOjoyiAD4232C7on93lyCh4_I,7489
-saltstack_age-0.2.3.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-saltstack_age-0.2.3.dist-info/entry_points.txt,sha256=AI6n3Tyjmxxz9FzJFJHJhhhv-hHZGhSrHFFjgbV2zH0,102
-saltstack_age-0.2.3.dist-info/RECORD,,
+saltstack_age/renderers/age.py,sha256=PQzXMdOY2GVdIWnMds64F5L0gUB7pwDf89uA_q1hYjQ,2522
+saltstack_age-0.3.0.dist-info/METADATA,sha256=hQjSgVaLJAEhxvxAaZW4ZFNkYgOSm6husvglfCv9q-0,7489
+saltstack_age-0.3.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+saltstack_age-0.3.0.dist-info/entry_points.txt,sha256=AI6n3Tyjmxxz9FzJFJHJhhhv-hHZGhSrHFFjgbV2zH0,102
+saltstack_age-0.3.0.dist-info/RECORD,,
```

