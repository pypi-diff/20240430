# Comparing `tmp/synthx-1.0.2.tar.gz` & `tmp/synthx-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthx-1.0.2.tar", max compression
+gzip compressed data, was "synthx-1.1.0.tar", max compression
```

## Comparing `synthx-1.0.2.tar` & `synthx-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7544 2024-04-24 02:57:16.510688 synthx-1.0.2/README.md
--rw-r--r--   0        0        0     1270 2024-04-24 16:13:16.769836 synthx-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-1.0.2/synthx/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-1.0.2/synthx/core/__init__.py
--rw-r--r--   0        0        0     8374 2024-04-23 18:48:20.102367 synthx-1.0.2/synthx/core/dataset.py
--rw-r--r--   0        0        0     6772 2024-04-23 18:48:20.102583 synthx-1.0.2/synthx/core/result.py
--rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-1.0.2/synthx/core/sample.py
--rw-r--r--   0        0        0      818 2024-04-18 01:31:14.755622 synthx-1.0.2/synthx/errors/__init__.py
--rw-r--r--   0        0        0    11221 2024-04-24 16:13:16.770151 synthx-1.0.2/synthx/method.py
--rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-1.0.2/synthx/stats/__init__.py
--rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-1.0.2/synthx/stats/norm.py
--rw-r--r--   0        0        0     1053 2024-04-23 18:47:48.800391 synthx-1.0.2/synthx/stats/p.py
--rw-r--r--   0        0        0     8328 1970-01-01 00:00:00.000000 synthx-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     7544 2024-04-30 07:29:11.374218 synthx-1.1.0/README.md
+-rw-r--r--   0        0        0     1270 2024-04-30 09:13:02.339012 synthx-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-1.1.0/synthx/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-1.1.0/synthx/core/__init__.py
+-rw-r--r--   0        0        0    12286 2024-04-30 09:13:02.339283 synthx-1.1.0/synthx/core/dataset.py
+-rw-r--r--   0        0        0     8907 2024-04-30 09:13:02.339542 synthx-1.1.0/synthx/core/result.py
+-rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-1.1.0/synthx/core/sample.py
+-rw-r--r--   0        0        0      923 2024-04-30 09:13:02.339718 synthx-1.1.0/synthx/errors/__init__.py
+-rw-r--r--   0        0        0    11221 2024-04-24 16:13:54.752232 synthx-1.1.0/synthx/method.py
+-rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-1.1.0/synthx/stats/__init__.py
+-rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-1.1.0/synthx/stats/norm.py
+-rw-r--r--   0        0        0     1053 2024-04-23 18:47:48.800391 synthx-1.1.0/synthx/stats/p.py
+-rw-r--r--   0        0        0     8328 1970-01-01 00:00:00.000000 synthx-1.1.0/PKG-INFO
```

### Comparing `synthx-1.0.2/README.md` & `synthx-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `synthx-1.0.2/pyproject.toml` & `synthx-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synthx"
-version = "1.0.2"
+version = "1.1.0"
 description = "A Python Library for Advanced Synthetic Control Analysis"
 authors = ["kenki931128 <kenki.nkmr@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `synthx-1.0.2/synthx/core/sample.py` & `synthx-1.1.0/synthx/core/sample.py`

 * *Files identical despite different names*

### Comparing `synthx-1.0.2/synthx/errors/__init__.py` & `synthx-1.1.0/synthx/errors/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,7 +23,11 @@
 
 class InconsistentTimestampsError(Exception):
     """Exception raised when timestamp is not inconcistent across units."""
 
 
 class InvalidNormalizationError(Exception):
     """Exception raised when undefined normalization is selected."""
+
+
+class StrictFilteringError(Exception):
+    """Exception raised when no data exists after filtering."""
```

### Comparing `synthx-1.0.2/synthx/method.py` & `synthx-1.1.0/synthx/method.py`

 * *Files identical despite different names*

### Comparing `synthx-1.0.2/synthx/stats/norm.py` & `synthx-1.1.0/synthx/stats/norm.py`

 * *Files identical despite different names*

### Comparing `synthx-1.0.2/synthx/stats/p.py` & `synthx-1.1.0/synthx/stats/p.py`

 * *Files identical despite different names*

### Comparing `synthx-1.0.2/PKG-INFO` & `synthx-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthx
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Python Library for Advanced Synthetic Control Analysis
 License: MIT
 Author: kenki931128
 Author-email: kenki.nkmr@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

