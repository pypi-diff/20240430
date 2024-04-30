# Comparing `tmp/openimis-be-im_export-1.1.0.tar.gz` & `tmp/openimis_be_im_export-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-im_export-1.1.0.tar", last modified: Sat Dec 16 01:00:22 2023, max compression
+gzip compressed data, was "openimis_be_im_export-1.2.0.tar", last modified: Tue Apr 30 09:07:27 2024, max compression
```

## Comparing `openimis-be-im_export-1.1.0.tar` & `openimis_be_im_export-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:00:22.885264 openimis-be-im_export-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-12-16 01:00:22.885264 openimis-be-im_export-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:00:22.885264 openimis-be-im_export-1.1.0/im_export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/im_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/im_export/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/im_export/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    10111 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/im_export/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/im_export/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:00:22.885264 openimis-be-im_export-1.1.0/im_export/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/im_export/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/im_export/tests/import_example.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9590 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/im_export/tests/import_example.json
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/im_export/tests/test_insuree.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/im_export/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-12-16 01:00:15.000000 openimis-be-im_export-1.1.0/im_export/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:00:22.885264 openimis-be-im_export-1.1.0/openimis_be_im_export.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-12-16 01:00:22.000000 openimis-be-im_export-1.1.0/openimis_be_im_export.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-12-16 01:00:22.000000 openimis-be-im_export-1.1.0/openimis_be_im_export.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 01:00:22.000000 openimis-be-im_export-1.1.0/openimis_be_im_export.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-16 01:00:22.000000 openimis-be-im_export-1.1.0/openimis_be_im_export.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-16 01:00:22.000000 openimis-be-im_export-1.1.0/openimis_be_im_export.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 01:00:22.885264 openimis-be-im_export-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-12-16 01:00:22.000000 openimis-be-im_export-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:27.185722 openimis_be_im_export-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-30 09:07:27.185722 openimis_be_im_export-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:27.185722 openimis_be_im_export-1.2.0/im_export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/im_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/im_export/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/im_export/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10111 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/im_export/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/im_export/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:27.185722 openimis_be_im_export-1.2.0/im_export/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/im_export/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/im_export/tests/import_example.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9590 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/im_export/tests/import_example.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/im_export/tests/test_insuree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/im_export/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-30 09:07:17.000000 openimis_be_im_export-1.2.0/im_export/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:27.185722 openimis_be_im_export-1.2.0/openimis_be_im_export.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-30 09:07:27.000000 openimis_be_im_export-1.2.0/openimis_be_im_export.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-30 09:07:27.000000 openimis_be_im_export-1.2.0/openimis_be_im_export.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:07:27.000000 openimis_be_im_export-1.2.0/openimis_be_im_export.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 09:07:27.000000 openimis_be_im_export-1.2.0/openimis_be_im_export.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 09:07:27.000000 openimis_be_im_export-1.2.0/openimis_be_im_export.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:07:27.185722 openimis_be_im_export-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-30 09:07:26.000000 openimis_be_im_export-1.2.0/setup.py
```

### Comparing `openimis-be-im_export-1.1.0/LICENSE` & `openimis_be_im_export-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openimis-be-im_export-1.1.0/PKG-INFO` & `openimis_be_im_export-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-im_export
-Version: 1.1.0
+Version: 1.2.0
 Summary: The openIMIS Backend import-export reference module based on django-import-export.
 Home-page: https://openimis.org/
 Author: Patrick Delcroix
 Author-email: patrick.delcroix@swisstph.ch
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-im_export-1.1.0/README.md` & `openimis_be_im_export-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-im_export-1.1.0/im_export/apps.py` & `openimis_be_im_export-1.2.0/im_export/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-im_export-1.1.0/im_export/resources.py` & `openimis_be_im_export-1.2.0/im_export/resources.py`

 * *Files identical despite different names*

### Comparing `openimis-be-im_export-1.1.0/im_export/services.py` & `openimis_be_im_export-1.2.0/im_export/services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-im_export-1.1.0/im_export/tests/import_example.csv` & `openimis_be_im_export-1.2.0/im_export/tests/import_example.csv`

 * *Files identical despite different names*

### Comparing `openimis-be-im_export-1.1.0/im_export/tests/import_example.json` & `openimis_be_im_export-1.2.0/im_export/tests/import_example.json`

 * *Files identical despite different names*

### Comparing `openimis-be-im_export-1.1.0/im_export/tests/test_insuree.py` & `openimis_be_im_export-1.2.0/im_export/tests/test_insuree.py`

 * *Files identical despite different names*

### Comparing `openimis-be-im_export-1.1.0/im_export/views.py` & `openimis_be_im_export-1.2.0/im_export/views.py`

 * *Files identical despite different names*

### Comparing `openimis-be-im_export-1.1.0/openimis_be_im_export.egg-info/PKG-INFO` & `openimis_be_im_export-1.2.0/openimis_be_im_export.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-im-export
-Version: 1.1.0
+Name: openimis-be-im_export
+Version: 1.2.0
 Summary: The openIMIS Backend import-export reference module based on django-import-export.
 Home-page: https://openimis.org/
 Author: Patrick Delcroix
 Author-email: patrick.delcroix@swisstph.ch
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-im_export-1.1.0/openimis_be_im_export.egg-info/SOURCES.txt` & `openimis_be_im_export-1.2.0/openimis_be_im_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-im_export-1.1.0/setup.py` & `openimis_be_im_export-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-im_export',
-    version='v1.1.0',
+    version='v1.2.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend import-export reference module based on django-import-export.',
     # long_description=README,
     url='https://openimis.org/',
     author='Patrick Delcroix',
```

