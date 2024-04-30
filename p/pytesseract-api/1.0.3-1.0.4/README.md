# Comparing `tmp/pytesseract_api-1.0.3.tar.gz` & `tmp/pytesseract_api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytesseract_api-1.0.3.tar", last modified: Mon Apr 22 14:03:43 2024, max compression
+gzip compressed data, was "pytesseract_api-1.0.4.tar", last modified: Tue Apr 30 08:17:43 2024, max compression
```

## Comparing `pytesseract_api-1.0.3.tar` & `pytesseract_api-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:03:43.038979 pytesseract_api-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 14:03:38.000000 pytesseract_api-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-22 14:03:38.000000 pytesseract_api-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-22 14:03:43.038979 pytesseract_api-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-22 14:03:38.000000 pytesseract_api-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-22 14:03:38.000000 pytesseract_api-1.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:03:43.034979 pytesseract_api-1.0.3/pytesseract_api/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-22 14:03:38.000000 pytesseract_api-1.0.3/pytesseract_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-22 14:03:38.000000 pytesseract_api-1.0.3/pytesseract_api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-22 14:03:38.000000 pytesseract_api-1.0.3/pytesseract_api/capi_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-22 14:03:38.000000 pytesseract_api-1.0.3/pytesseract_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:03:38.000000 pytesseract_api-1.0.3/pytesseract_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:03:43.038979 pytesseract_api-1.0.3/pytesseract_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-22 14:03:43.000000 pytesseract_api-1.0.3/pytesseract_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-22 14:03:43.000000 pytesseract_api-1.0.3/pytesseract_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 14:03:43.000000 pytesseract_api-1.0.3/pytesseract_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 14:03:43.000000 pytesseract_api-1.0.3/pytesseract_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 14:03:43.038979 pytesseract_api-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-22 14:03:38.000000 pytesseract_api-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:17:43.502632 pytesseract_api-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-30 08:17:35.000000 pytesseract_api-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 08:17:35.000000 pytesseract_api-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-30 08:17:43.502632 pytesseract_api-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-30 08:17:35.000000 pytesseract_api-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-30 08:17:35.000000 pytesseract_api-1.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:17:43.502632 pytesseract_api-1.0.4/pytesseract_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-30 08:17:35.000000 pytesseract_api-1.0.4/pytesseract_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-30 08:17:35.000000 pytesseract_api-1.0.4/pytesseract_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-30 08:17:35.000000 pytesseract_api-1.0.4/pytesseract_api/capi_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-30 08:17:35.000000 pytesseract_api-1.0.4/pytesseract_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:17:35.000000 pytesseract_api-1.0.4/pytesseract_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:17:43.502632 pytesseract_api-1.0.4/pytesseract_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-30 08:17:43.000000 pytesseract_api-1.0.4/pytesseract_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-30 08:17:43.000000 pytesseract_api-1.0.4/pytesseract_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:17:43.000000 pytesseract_api-1.0.4/pytesseract_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 08:17:43.000000 pytesseract_api-1.0.4/pytesseract_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 08:17:43.502632 pytesseract_api-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-30 08:17:35.000000 pytesseract_api-1.0.4/setup.py
```

### Comparing `pytesseract_api-1.0.3/LICENSE` & `pytesseract_api-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytesseract_api-1.0.3/PKG-INFO` & `pytesseract_api-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesseract-api
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tesseract C-API in python, a faster alternative to pytesseract
 Home-page: https://github.com/sandbox-pokhara/pytesseract-api
 Author: Pradish Bijukchhe
 Author-email: pradishbijukchhe@gmail.com
 Project-URL: Bug Tracker, https://github.com/sandbox-pokhara/pytesseract-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytesseract_api-1.0.3/README.md` & `pytesseract_api-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pytesseract_api-1.0.3/pytesseract_api.egg-info/PKG-INFO` & `pytesseract_api-1.0.4/pytesseract_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesseract-api
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tesseract C-API in python, a faster alternative to pytesseract
 Home-page: https://github.com/sandbox-pokhara/pytesseract-api
 Author: Pradish Bijukchhe
 Author-email: pradishbijukchhe@gmail.com
 Project-URL: Bug Tracker, https://github.com/sandbox-pokhara/pytesseract-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytesseract_api-1.0.3/setup.py` & `pytesseract_api-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytesseract-api",
-    version="1.0.3",
+    version="1.0.4",
     author="Pradish Bijukchhe",
     author_email="pradishbijukchhe@gmail.com",
     description=(
         "Tesseract C-API in python, a faster alternative to pytesseract"
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

