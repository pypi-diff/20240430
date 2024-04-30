# Comparing `tmp/assets2036py-0.1.8.tar.gz` & `tmp/assets2036py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assets2036py-0.1.8.tar", last modified: Thu Feb 22 14:31:39 2024, max compression
+gzip compressed data, was "assets2036py-0.1.9.tar", last modified: Thu Feb 22 16:06:46 2024, max compression
```

## Comparing `assets2036py-0.1.8.tar` & `assets2036py-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:31:39.466343 assets2036py-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-02-22 14:31:31.000000 assets2036py-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-22 14:31:31.000000 assets2036py-0.1.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-22 14:31:39.466343 assets2036py-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-22 14:31:31.000000 assets2036py-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:31:39.466343 assets2036py-0.1.8/assets2036py/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-22 14:31:31.000000 assets2036py-0.1.8/assets2036py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-22 14:31:31.000000 assets2036py-0.1.8/assets2036py/assetlogging.py
--rw-r--r--   0 runner    (1001) docker     (127)    11184 2024-02-22 14:31:31.000000 assets2036py-0.1.8/assets2036py/assetmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    22681 2024-02-22 14:31:31.000000 assets2036py-0.1.8/assets2036py/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-02-22 14:31:31.000000 assets2036py-0.1.8/assets2036py/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-22 14:31:31.000000 assets2036py-0.1.8/assets2036py/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 14:31:31.000000 assets2036py-0.1.8/assets2036py/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:31:39.466343 assets2036py-0.1.8/assets2036py/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-02-22 14:31:31.000000 assets2036py-0.1.8/assets2036py/resources/_endpoint.json
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-22 14:31:31.000000 assets2036py-0.1.8/assets2036py/resources/submodel_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-02-22 14:31:31.000000 assets2036py-0.1.8/assets2036py/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:31:39.466343 assets2036py-0.1.8/assets2036py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-22 14:31:39.000000 assets2036py-0.1.8/assets2036py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-22 14:31:39.000000 assets2036py-0.1.8/assets2036py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 14:31:39.000000 assets2036py-0.1.8/assets2036py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-22 14:31:39.000000 assets2036py-0.1.8/assets2036py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-22 14:31:39.000000 assets2036py-0.1.8/assets2036py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 14:31:39.466343 assets2036py-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-22 14:31:31.000000 assets2036py-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:31:39.466343 assets2036py-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    31300 2024-02-22 14:31:31.000000 assets2036py-0.1.8/tests/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-02-22 14:31:31.000000 assets2036py-0.1.8/tests/test_assetmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-02-22 14:31:31.000000 assets2036py-0.1.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:06:46.144720 assets2036py-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-02-22 16:06:35.000000 assets2036py-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-22 16:06:35.000000 assets2036py-0.1.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-22 16:06:46.144720 assets2036py-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-22 16:06:35.000000 assets2036py-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:06:46.140720 assets2036py-0.1.9/assets2036py/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-22 16:06:35.000000 assets2036py-0.1.9/assets2036py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-22 16:06:35.000000 assets2036py-0.1.9/assets2036py/assetlogging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11184 2024-02-22 16:06:35.000000 assets2036py-0.1.9/assets2036py/assetmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22681 2024-02-22 16:06:35.000000 assets2036py-0.1.9/assets2036py/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-02-22 16:06:35.000000 assets2036py-0.1.9/assets2036py/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-22 16:06:35.000000 assets2036py-0.1.9/assets2036py/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 16:06:35.000000 assets2036py-0.1.9/assets2036py/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:06:46.140720 assets2036py-0.1.9/assets2036py/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-02-22 16:06:35.000000 assets2036py-0.1.9/assets2036py/resources/_endpoint.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-22 16:06:35.000000 assets2036py-0.1.9/assets2036py/resources/submodel_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-02-22 16:06:35.000000 assets2036py-0.1.9/assets2036py/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:06:46.144720 assets2036py-0.1.9/assets2036py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-22 16:06:46.000000 assets2036py-0.1.9/assets2036py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-22 16:06:46.000000 assets2036py-0.1.9/assets2036py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 16:06:46.000000 assets2036py-0.1.9/assets2036py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-22 16:06:46.000000 assets2036py-0.1.9/assets2036py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-22 16:06:46.000000 assets2036py-0.1.9/assets2036py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 16:06:46.144720 assets2036py-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-22 16:06:35.000000 assets2036py-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:06:46.144720 assets2036py-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    31300 2024-02-22 16:06:35.000000 assets2036py-0.1.9/tests/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-02-22 16:06:35.000000 assets2036py-0.1.9/tests/test_assetmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-02-22 16:06:35.000000 assets2036py-0.1.9/tests/test_utils.py
```

### Comparing `assets2036py-0.1.8/LICENSE` & `assets2036py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `assets2036py-0.1.8/NOTICE` & `assets2036py-0.1.9/NOTICE`

 * *Files identical despite different names*

### Comparing `assets2036py-0.1.8/PKG-INFO` & `assets2036py-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assets2036py
-Version: 0.1.8
+Version: 0.1.9
 Summary: helper library to easily implement assets2036
 Home-page: https://github.com/boschresearch/assets2036spy
 Author: Daniel Ewert (CR/APT5)
 Author-email: Daniel.Ewert@de.bosch.com
 License: BIOS
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `assets2036py-0.1.8/assets2036py/__init__.py` & `assets2036py-0.1.9/assets2036py/__init__.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.1.8/assets2036py/assetmanager.py` & `assets2036py-0.1.9/assets2036py/assetmanager.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.1.8/assets2036py/assets.py` & `assets2036py-0.1.9/assets2036py/assets.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.1.8/assets2036py/communication.py` & `assets2036py-0.1.9/assets2036py/communication.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.1.8/assets2036py/exceptions.py` & `assets2036py-0.1.9/assets2036py/exceptions.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.1.8/assets2036py/resources/_endpoint.json` & `assets2036py-0.1.9/assets2036py/resources/_endpoint.json`

 * *Files identical despite different names*

### Comparing `assets2036py-0.1.8/assets2036py/resources/submodel_schema.json` & `assets2036py-0.1.9/assets2036py/resources/submodel_schema.json`

 * *Files identical despite different names*

### Comparing `assets2036py-0.1.8/assets2036py/utilities.py` & `assets2036py-0.1.9/assets2036py/utilities.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.1.8/assets2036py.egg-info/PKG-INFO` & `assets2036py-0.1.9/assets2036py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assets2036py
-Version: 0.1.8
+Version: 0.1.9
 Summary: helper library to easily implement assets2036
 Home-page: https://github.com/boschresearch/assets2036spy
 Author: Daniel Ewert (CR/APT5)
 Author-email: Daniel.Ewert@de.bosch.com
 License: BIOS
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `assets2036py-0.1.8/assets2036py.egg-info/SOURCES.txt` & `assets2036py-0.1.9/assets2036py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assets2036py-0.1.8/setup.py` & `assets2036py-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="assets2036py",
-    version="0.1.8",
+    version="0.1.9",
     url="https://github.com/boschresearch/assets2036spy",
     license="BIOS",
     author="Daniel Ewert (CR/APT5)",
     author_email="Daniel.Ewert@de.bosch.com",
     description="helper library to easily implement assets2036",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `assets2036py-0.1.8/tests/test_asset.py` & `assets2036py-0.1.9/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.1.8/tests/test_assetmanager.py` & `assets2036py-0.1.9/tests/test_assetmanager.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.1.8/tests/test_utils.py` & `assets2036py-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

