# Comparing `tmp/saltstack_age-0.1.0-py3-none-any.whl.zip` & `tmp/saltstack_age-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,13 @@
-Zip file size: 2693 bytes, number of entries: 7
+Zip file size: 5521 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 saltstack_age/__init__.py
+-rw-r--r--  2.0 unx     4672 b- defN 20-Feb-02 00:00 saltstack_age/cli.py
+-rw-r--r--  2.0 unx      309 b- defN 20-Feb-02 00:00 saltstack_age/identities.py
+-rw-r--r--  2.0 unx      109 b- defN 20-Feb-02 00:00 saltstack_age/passphrase.py
+-rw-r--r--  2.0 unx     1561 b- defN 20-Feb-02 00:00 saltstack_age/secure_value.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 saltstack_age/renderers/__init__.py
--rw-r--r--  2.0 unx     2408 b- defN 20-Feb-02 00:00 saltstack_age/renderers/age.py
-?rw-r--r--  2.0 unx      345 b- defN 20-Feb-02 00:00 saltstack_age-0.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 saltstack_age-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx       44 b- defN 20-Feb-02 00:00 saltstack_age-0.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      579 b- defN 20-Feb-02 00:00 saltstack_age-0.1.0.dist-info/RECORD
-7 files, 3463 bytes uncompressed, 1649 bytes compressed:  52.4%
+-rw-r--r--  2.0 unx     1672 b- defN 20-Feb-02 00:00 saltstack_age/renderers/age.py
+?rw-r--r--  2.0 unx      345 b- defN 20-Feb-02 00:00 saltstack_age-0.1.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 saltstack_age-0.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      102 b- defN 20-Feb-02 00:00 saltstack_age-0.1.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      909 b- defN 20-Feb-02 00:00 saltstack_age-0.1.1.dist-info/RECORD
+11 files, 9766 bytes uncompressed, 3967 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -1,22 +1,34 @@
 Filename: saltstack_age/__init__.py
 Comment: 
 
+Filename: saltstack_age/cli.py
+Comment: 
+
+Filename: saltstack_age/identities.py
+Comment: 
+
+Filename: saltstack_age/passphrase.py
+Comment: 
+
+Filename: saltstack_age/secure_value.py
+Comment: 
+
 Filename: saltstack_age/renderers/__init__.py
 Comment: 
 
 Filename: saltstack_age/renderers/age.py
 Comment: 
 
-Filename: saltstack_age-0.1.0.dist-info/METADATA
+Filename: saltstack_age-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: saltstack_age-0.1.0.dist-info/WHEEL
+Filename: saltstack_age-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: saltstack_age-0.1.0.dist-info/entry_points.txt
+Filename: saltstack_age-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: saltstack_age-0.1.0.dist-info/RECORD
+Filename: saltstack_age-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## saltstack_age/renderers/age.py

```diff
@@ -1,95 +1,63 @@
-import os
-import re
-from base64 import b64decode
 from collections import OrderedDict
-from pathlib import Path
+from importlib import import_module
 from typing import Any
 
-import pyrage
 from salt.exceptions import SaltRenderError
 
-Data = OrderedDict[str, Any]
-
-
-RE_SECURE_VALUE = re.compile(
-    r"""
-ENC\[
-age-(?P<type>passphrase|identity)
-,
-(?P<base64CipherText>
-    (?:[A-Za-z0-9+/]{4})*
-    (?:
-        [A-Za-z0-9+/]{2}==
-        |
-        [A-Za-z0-9+/]{3}=
-    )?
-)
-\]
-\s*
-""",
-    re.VERBOSE,
+from saltstack_age.passphrase import get_passphrase_from_environment
+from saltstack_age.secure_value import (
+    IdentitySecureValue,
+    is_secure_value,
+    parse_secure_value,
 )
 
+Data = OrderedDict[str, Any]
 
-def _decrypt_with_identity(ciphertext: bytes) -> str:
-    identity_file: str | None = __salt__["config.get"]("age_identity_file")
-
-    if not identity_file:
-        raise SaltRenderError("age_identity_file is not defined")
-
-    identity_path = Path(identity_file)
+__virtualname__ = "age"
 
-    if not identity_path.is_file():
-        raise SaltRenderError(f"age_identity_file not found: {identity_file}")
 
-    identity_string = re.sub(
-        r"^#.*\n?",
-        "",
-        identity_path.read_text(),
-        flags=re.MULTILINE,
-    ).rstrip("\n")
-    identity = pyrage.x25519.Identity.from_str(identity_string)
+def __virtual__() -> str | tuple[bool, str]:  # noqa: N807
+    if "config.get" not in __salt__:
+        # Not sure how/when that happens?
+        return (False, '"config.get" is not available')
 
-    return pyrage.decrypt(ciphertext, [identity]).decode()
+    try:
+        _ = import_module("pyrage")
+    except ModuleNotFoundError:
+        return (False, "pyrage is not installed")
 
+    return __virtualname__
 
-def _decrypt(secure_value: str) -> str:
-    match = RE_SECURE_VALUE.match(secure_value)
 
-    if not match:
-        # Should _never_ happen as we match against the regex in render()
-        raise SaltRenderError(f"Invalid age secure value: {secure_value}")
+def _decrypt(string: str) -> str:
+    secure_value = parse_secure_value(string)
 
-    type_, base64_ciphertext = match.groups()
-    ciphertext = b64decode(base64_ciphertext)
+    if isinstance(secure_value, IdentitySecureValue):
+        identity_file: str | None = __salt__["config.get"]("age_identity_file")
 
-    if type_ == "identity":
-        if "config.get" in __salt__:
-            return _decrypt_with_identity(ciphertext)
+        if not identity_file:
+            raise SaltRenderError("age_identity_file is not defined")
 
-        # Not sure how/when that happens...
-        raise RuntimeError('__salt__["config.get"] is not available')
+        return secure_value.decrypt(identity_file)
 
-    if type_ == "passphrase":
-        if "AGE_PASSPHRASE" in os.environ:
-            return pyrage.passphrase.decrypt(
-                ciphertext,
-                os.environ["AGE_PASSPHRASE"],
-            ).decode()
+    # secure_value is a PassphraseSecureValue
+    passphrase: str | None = (
+        __salt__["config.get"]("age_passphrase") or get_passphrase_from_environment()
+    )
 
-        raise SaltRenderError("The AGE_PASSPHRASE environment variable is not defined")
+    if passphrase is None:
+        raise SaltRenderError("No age passphrase found in config or environment")
 
-    # This can only happen if we change the regex without updating this function
-    raise SaltRenderError(f"Invalid age encryption type: {type_}")
+    return secure_value.decrypt(passphrase)
 
 
 def render(
     data: Data,
     _saltenv: str = "base",
     _sls: str = "",
     **_kwargs: None,
 ) -> Data:
     return OrderedDict(
-        (key, _decrypt(value) if RE_SECURE_VALUE.match(value) else value)
+        (key, _decrypt(value) if is_secure_value(value) else value)
         for key, value in data.items()
     )
```

