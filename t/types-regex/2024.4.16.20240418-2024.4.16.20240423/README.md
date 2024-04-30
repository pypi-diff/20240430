# Comparing `tmp/types-regex-2024.4.16.20240418.tar.gz` & `tmp/types-regex-2024.4.16.20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-regex-2024.4.16.20240418.tar", last modified: Thu Apr 18 02:16:43 2024, max compression
+gzip compressed data, was "types-regex-2024.4.16.20240423.tar", last modified: Tue Apr 23 02:19:20 2024, max compression
```

## Comparing `types-regex-2024.4.16.20240418.tar` & `types-regex-2024.4.16.20240423.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:16:43.086822 types-regex-2024.4.16.20240418/
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-18 02:16:41.000000 types-regex-2024.4.16.20240418/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 02:16:41.000000 types-regex-2024.4.16.20240418/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-18 02:16:43.082822 types-regex-2024.4.16.20240418/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:16:43.082822 types-regex-2024.4.16.20240418/regex-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 02:16:41.000000 types-regex-2024.4.16.20240418/regex-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 02:16:27.000000 types-regex-2024.4.16.20240418/regex-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-18 02:16:27.000000 types-regex-2024.4.16.20240418/regex-stubs/_regex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-18 02:16:27.000000 types-regex-2024.4.16.20240418/regex-stubs/_regex_core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:16:41.000000 types-regex-2024.4.16.20240418/regex-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19266 2024-04-18 02:16:27.000000 types-regex-2024.4.16.20240418/regex-stubs/regex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 02:16:43.086822 types-regex-2024.4.16.20240418/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-18 02:16:41.000000 types-regex-2024.4.16.20240418/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:16:43.082822 types-regex-2024.4.16.20240418/types_regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-18 02:16:43.000000 types-regex-2024.4.16.20240418/types_regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-18 02:16:43.000000 types-regex-2024.4.16.20240418/types_regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 02:16:43.000000 types-regex-2024.4.16.20240418/types_regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 02:16:43.000000 types-regex-2024.4.16.20240418/types_regex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:20.264456 types-regex-2024.4.16.20240423/
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-23 02:19:19.000000 types-regex-2024.4.16.20240423/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 02:19:19.000000 types-regex-2024.4.16.20240423/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-23 02:19:20.264456 types-regex-2024.4.16.20240423/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:20.264456 types-regex-2024.4.16.20240423/regex-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 02:19:19.000000 types-regex-2024.4.16.20240423/regex-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 02:18:48.000000 types-regex-2024.4.16.20240423/regex-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-23 02:18:48.000000 types-regex-2024.4.16.20240423/regex-stubs/_regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-23 02:18:48.000000 types-regex-2024.4.16.20240423/regex-stubs/_regex_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:19.000000 types-regex-2024.4.16.20240423/regex-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19266 2024-04-23 02:18:48.000000 types-regex-2024.4.16.20240423/regex-stubs/regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:19:20.264456 types-regex-2024.4.16.20240423/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-23 02:19:19.000000 types-regex-2024.4.16.20240423/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:20.264456 types-regex-2024.4.16.20240423/types_regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-23 02:19:20.000000 types-regex-2024.4.16.20240423/types_regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-23 02:19:20.000000 types-regex-2024.4.16.20240423/types_regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:19:20.000000 types-regex-2024.4.16.20240423/types_regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 02:19:20.000000 types-regex-2024.4.16.20240423/types_regex.egg-info/top_level.txt
```

### Comparing `types-regex-2024.4.16.20240418/CHANGELOG.md` & `types-regex-2024.4.16.20240423/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 2024.4.16.20240423 (2024-04-23)
+
+Add precise values for enum members where possible (#11299)
+
+Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
+Co-authored-by: Alex Waygood <alex.waygood@gmail.com>
+
 ## 2024.4.16.20240418 (2024-04-18)
 
 [stubsabot] Bump regex to 2024.4.16 (#11773)
 
 ## 2023.12.25.20240311 (2024-03-11)
 
 Use PEP 570 syntax in third party stubs (#11554)
```

### Comparing `types-regex-2024.4.16.20240418/PKG-INFO` & `types-regex-2024.4.16.20240423/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2024.4.16.20240418
+Version: 2024.4.16.20240423
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-regex` aims to provide accurate annotations
 for `regex==2024.4.16`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `12b9e48324df292379db3eca4e3c54175e5f374e` and was tested
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

### Comparing `types-regex-2024.4.16.20240418/regex-stubs/_regex.pyi` & `types-regex-2024.4.16.20240423/regex-stubs/_regex.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2024.4.16.20240418/regex-stubs/_regex_core.pyi` & `types-regex-2024.4.16.20240423/regex-stubs/_regex_core.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -5,48 +5,48 @@
 
 from .regex import Pattern
 
 class error(Exception):
     def __init__(self, message: str, pattern: AnyStr | None = None, pos: int | None = None) -> None: ...
 
 class RegexFlag(enum.IntFlag):
-    A: int
-    ASCII: int
-    B: int
-    BESTMATCH: int
-    D: int
-    DEBUG: int
-    E: int
-    ENHANCEMATCH: int
-    F: int
-    FULLCASE: int
-    I: int
-    IGNORECASE: int
-    L: int
-    LOCALE: int
-    M: int
-    MULTILINE: int
-    P: int
-    POSIX: int
-    R: int
-    REVERSE: int
-    T: int
-    TEMPLATE: int
-    S: int
-    DOTALL: int
-    U: int
-    UNICODE: int
-    V0: int
-    VERSION0: int
-    V1: int
-    VERSION1: int
-    W: int
-    WORD: int
-    X: int
-    VERBOSE: int
+    A = 0x80
+    ASCII = A
+    B = 0x1000
+    BESTMATCH = B
+    D = 0x200
+    DEBUG = D
+    E = 0x8000
+    ENHANCEMATCH = E
+    F = 0x4000
+    FULLCASE = F
+    I = 0x2
+    IGNORECASE = I
+    L = 0x4
+    LOCALE = L
+    M = 0x8
+    MULTILINE = M
+    P = 0x10000
+    POSIX = P
+    R = 0x400
+    REVERSE = R
+    T = 0x1
+    TEMPLATE = T
+    S = 0x10
+    DOTALL = S
+    U = 0x20
+    UNICODE = U
+    V0 = 0x2000
+    VERSION0 = V0
+    V1 = 0x100
+    VERSION1 = V1
+    W = 0x800
+    WORD = W
+    X = 0x40
+    VERBOSE = X
 
 A: int
 ASCII: int
 B: int
 BESTMATCH: int
 D: int
 DEBUG: int
```

### Comparing `types-regex-2024.4.16.20240418/regex-stubs/regex.pyi` & `types-regex-2024.4.16.20240423/regex-stubs/regex.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2024.4.16.20240418/setup.py` & `types-regex-2024.4.16.20240423/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-regex` aims to provide accurate annotations
 for `regex==2024.4.16`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `12b9e48324df292379db3eca4e3c54175e5f374e` and was tested
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2024.4.16.20240418",
+      version="2024.4.16.20240423",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md",
```

### Comparing `types-regex-2024.4.16.20240418/types_regex.egg-info/PKG-INFO` & `types-regex-2024.4.16.20240423/types_regex.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2024.4.16.20240418
+Version: 2024.4.16.20240423
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-regex` aims to provide accurate annotations
 for `regex==2024.4.16`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `12b9e48324df292379db3eca4e3c54175e5f374e` and was tested
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

