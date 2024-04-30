# Comparing `tmp/iterdir-0.0.5.1.tar.gz` & `tmp/iterdir-0.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterdir-0.0.5.1.tar", max compression
+gzip compressed data, was "iterdir-0.0.5.2.tar", max compression
```

## Comparing `iterdir-0.0.5.1.tar` & `iterdir-0.0.5.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.5.1/LICENSE
--rwxr-xr-x   0        0        0     9421 2024-04-30 05:54:47.336601 iterdir-0.0.5.1/iterdir/__init__.py
--rwxr-xr-x   0        0        0    10117 2024-04-30 06:10:28.107257 iterdir-0.0.5.1/iterdir/__main__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 iterdir-0.0.5.1/iterdir/py.typed
--rw-r--r--   0        0        0     1137 2024-04-30 06:10:55.051079 iterdir-0.0.5.1/pyproject.toml
--rw-r--r--   0        0        0     5348 2024-04-30 06:04:55.686039 iterdir-0.0.5.1/readme.md
--rw-r--r--   0        0        0     6467 1970-01-01 00:00:00.000000 iterdir-0.0.5.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.5.2/LICENSE
+-rwxr-xr-x   0        0        0     9420 2024-04-30 09:50:20.128917 iterdir-0.0.5.2/iterdir/__init__.py
+-rwxr-xr-x   0        0        0    10117 2024-04-30 06:10:28.107257 iterdir-0.0.5.2/iterdir/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 iterdir-0.0.5.2/iterdir/py.typed
+-rw-r--r--   0        0        0     1137 2024-04-30 09:51:02.442875 iterdir-0.0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     5348 2024-04-30 06:04:55.686039 iterdir-0.0.5.2/readme.md
+-rw-r--r--   0        0        0     6467 1970-01-01 00:00:00.000000 iterdir-0.0.5.2/PKG-INFO
```

### Comparing `iterdir-0.0.5.1/LICENSE` & `iterdir-0.0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iterdir-0.0.5.1/iterdir/__init__.py` & `iterdir-0.0.5.2/iterdir/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         min_depth -= 1
     elif min_depth <= 0:
         pred = True if predicate is None else predicate(top)
         if pred is None:
             return
         elif pred:
             yield top
-        if not is_dir(top):
+        if not isdir(top):
             return
         min_depth = 1
     if max_depth > 0:
         max_depth -= 1
     try:
         for path in iter_dir(top):
             yield_me = global_yield_me
```

### Comparing `iterdir-0.0.5.1/iterdir/__main__.py` & `iterdir-0.0.5.2/iterdir/__main__.py`

 * *Files identical despite different names*

### Comparing `iterdir-0.0.5.1/pyproject.toml` & `iterdir-0.0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iterdir"
-version = "0.0.5.1"
+version = "0.0.5.2"
 description = "python iterate over path tree."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 keywords = ["iterdir", "traverse"]
```

### Comparing `iterdir-0.0.5.1/readme.md` & `iterdir-0.0.5.2/readme.md`

 * *Files identical despite different names*

### Comparing `iterdir-0.0.5.1/PKG-INFO` & `iterdir-0.0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterdir
-Version: 0.0.5.1
+Version: 0.0.5.2
 Summary: python iterate over path tree.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir
 License: MIT
 Keywords: iterdir,traverse
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

