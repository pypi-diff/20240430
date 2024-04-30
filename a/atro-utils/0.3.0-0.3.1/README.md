# Comparing `tmp/atro_utils-0.3.0.tar.gz` & `tmp/atro_utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_utils-0.3.0.tar", max compression
+gzip compressed data, was "atro_utils-0.3.1.tar", max compression
```

## Comparing `atro_utils-0.3.0.tar` & `atro_utils-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2024-04-30 21:28:59.752470 atro_utils-0.3.0/LICENSE
--rw-r--r--   0        0        0       13 2024-04-30 21:28:59.752470 atro_utils-0.3.0/README.md
--rw-r--r--   0        0        0      816 2024-04-30 21:29:20.588550 atro_utils-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       76 2024-04-30 21:28:59.752470 atro_utils-0.3.0/src/atro_utils/__init__.py
--rw-r--r--   0        0        0     2688 2024-04-30 21:28:59.752470 atro_utils-0.3.0/src/atro_utils/atro_dict.py
--rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 atro_utils-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-30 21:48:55.775428 atro_utils-0.3.1/LICENSE
+-rw-r--r--   0        0        0       13 2024-04-30 21:48:55.775428 atro_utils-0.3.1/README.md
+-rw-r--r--   0        0        0      816 2024-04-30 21:49:17.735562 atro_utils-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       76 2024-04-30 21:48:55.779428 atro_utils-0.3.1/src/atro_utils/__init__.py
+-rw-r--r--   0        0        0     2688 2024-04-30 21:48:55.779428 atro_utils-0.3.1/src/atro_utils/atro_dict.py
+-rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 atro_utils-0.3.1/PKG-INFO
```

### Comparing `atro_utils-0.3.0/LICENSE` & `atro_utils-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atro_utils-0.3.0/pyproject.toml` & `atro_utils-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atro-utils"
-version = "0.3.0"
+version = "0.3.1"
 description = "Package containing generic utilities for variety of python usages."
 authors = ["atropos <sv7n@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "atro_utils", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `atro_utils-0.3.0/src/atro_utils/atro_dict.py` & `atro_utils-0.3.1/src/atro_utils/atro_dict.py`

 * *Files identical despite different names*

### Comparing `atro_utils-0.3.0/PKG-INFO` & `atro_utils-0.3.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: Package containing generic utilities for variety of python usages.
 License: MIT
 Author: atropos
 Author-email: sv7n@pm.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

