# Comparing `tmp/python_decorator-0.0.1.2.tar.gz` & `tmp/python_decorator-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_decorator-0.0.1.2.tar", max compression
+gzip compressed data, was "python_decorator-0.0.1.3.tar", max compression
```

## Comparing `python_decorator-0.0.1.2.tar` & `python_decorator-0.0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_decorator-0.0.1.2/LICENSE
--rwxr-xr-x   0        0        0     8150 2024-04-24 15:50:19.893394 python_decorator-0.0.1.2/decorator0/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_decorator-0.0.1.2/decorator0/py.typed
--rw-r--r--   0        0        0     1206 2024-04-24 15:55:51.158211 python_decorator-0.0.1.2/pyproject.toml
--rw-r--r--   0        0        0      201 2024-04-24 15:56:16.540240 python_decorator-0.0.1.2/readme.md
--rw-r--r--   0        0        0     1401 1970-01-01 00:00:00.000000 python_decorator-0.0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_decorator-0.0.1.3/LICENSE
+-rwxr-xr-x   0        0        0     8754 2024-04-30 12:32:44.935851 python_decorator-0.0.1.3/decorator0/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_decorator-0.0.1.3/decorator0/py.typed
+-rw-r--r--   0        0        0     1206 2024-04-30 12:33:41.653421 python_decorator-0.0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-04-24 15:56:16.540240 python_decorator-0.0.1.3/readme.md
+-rw-r--r--   0        0        0     1401 1970-01-01 00:00:00.000000 python_decorator-0.0.1.3/PKG-INFO
```

### Comparing `python_decorator-0.0.1.2/LICENSE` & `python_decorator-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_decorator-0.0.1.2/pyproject.toml` & `python_decorator-0.0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-decorator"
-version = "0.0.1.2"
+version = "0.0.1.3"
 description = "Python argument type."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator"
 keywords = ["file", "reverse", "iter"]
```

### Comparing `python_decorator-0.0.1.2/PKG-INFO` & `python_decorator-0.0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-decorator
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Python argument type.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator
 License: MIT
 Keywords: file,reverse,iter
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

