# Comparing `tmp/dicomthings-0.7.0.tar.gz` & `tmp/dicomthings-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicomthings-0.7.0.tar", last modified: Mon Dec 11 12:29:49 2023, max compression
+gzip compressed data, was "dicomthings-0.7.1.tar", last modified: Tue Apr 30 09:47:13 2024, max compression
```

## Comparing `dicomthings-0.7.0.tar` & `dicomthings-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jeroenbertels   (501) staff       (20)        0 2023-12-11 12:29:49.866983 dicomthings-0.7.0/
--rw-r--r--   0 jeroenbertels   (501) staff       (20)    11357 2023-11-03 13:41:14.000000 dicomthings-0.7.0/LICENSE
--rw-r--r--   0 jeroenbertels   (501) staff       (20)      567 2023-12-11 12:29:49.866710 dicomthings-0.7.0/PKG-INFO
--rw-r--r--   0 jeroenbertels   (501) staff       (20)       61 2023-11-06 08:08:03.000000 dicomthings-0.7.0/README.md
-drwxr-xr-x   0 jeroenbertels   (501) staff       (20)        0 2023-12-11 12:29:49.865266 dicomthings-0.7.0/dicomthings/
--rw-r--r--   0 jeroenbertels   (501) staff       (20)        0 2023-11-13 11:07:07.000000 dicomthings-0.7.0/dicomthings/__init__.py
--rw-r--r--   0 jeroenbertels   (501) staff       (20)     8650 2023-12-11 12:28:36.000000 dicomthings-0.7.0/dicomthings/array.py
--rw-r--r--   0 jeroenbertels   (501) staff       (20)    15233 2023-11-14 12:59:40.000000 dicomthings-0.7.0/dicomthings/dicom.py
--rw-r--r--   0 jeroenbertels   (501) staff       (20)     4954 2023-12-11 12:28:36.000000 dicomthings-0.7.0/dicomthings/nifti.py
--rw-r--r--   0 jeroenbertels   (501) staff       (20)     2265 2023-11-22 10:02:41.000000 dicomthings-0.7.0/dicomthings/utils.py
-drwxr-xr-x   0 jeroenbertels   (501) staff       (20)        0 2023-12-11 12:29:49.866418 dicomthings-0.7.0/dicomthings.egg-info/
--rw-r--r--   0 jeroenbertels   (501) staff       (20)      567 2023-12-11 12:29:49.000000 dicomthings-0.7.0/dicomthings.egg-info/PKG-INFO
--rw-r--r--   0 jeroenbertels   (501) staff       (20)      314 2023-12-11 12:29:49.000000 dicomthings-0.7.0/dicomthings.egg-info/SOURCES.txt
--rw-r--r--   0 jeroenbertels   (501) staff       (20)        1 2023-12-11 12:29:49.000000 dicomthings-0.7.0/dicomthings.egg-info/dependency_links.txt
--rw-r--r--   0 jeroenbertels   (501) staff       (20)       12 2023-12-11 12:29:49.000000 dicomthings-0.7.0/dicomthings.egg-info/requires.txt
--rw-r--r--   0 jeroenbertels   (501) staff       (20)       12 2023-12-11 12:29:49.000000 dicomthings-0.7.0/dicomthings.egg-info/top_level.txt
--rw-r--r--   0 jeroenbertels   (501) staff       (20)      665 2023-11-06 08:08:03.000000 dicomthings-0.7.0/pyproject.toml
--rw-r--r--   0 jeroenbertels   (501) staff       (20)       38 2023-12-11 12:29:49.867045 dicomthings-0.7.0/setup.cfg
+drwxr-xr-x   0 jeroenbertels   (501) staff       (20)        0 2024-04-30 09:47:13.424729 dicomthings-0.7.1/
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)    11357 2023-11-03 13:41:14.000000 dicomthings-0.7.1/LICENSE
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)      567 2024-04-30 09:47:13.424547 dicomthings-0.7.1/PKG-INFO
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)       61 2023-11-06 08:08:03.000000 dicomthings-0.7.1/README.md
+drwxr-xr-x   0 jeroenbertels   (501) staff       (20)        0 2024-04-30 09:47:13.423462 dicomthings-0.7.1/dicomthings/
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)        0 2023-11-13 11:07:07.000000 dicomthings-0.7.1/dicomthings/__init__.py
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)     8650 2023-12-11 12:28:36.000000 dicomthings-0.7.1/dicomthings/array.py
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)    15233 2023-11-14 12:59:40.000000 dicomthings-0.7.1/dicomthings/dicom.py
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)     4954 2024-04-30 09:44:56.000000 dicomthings-0.7.1/dicomthings/nifti.py
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)     2265 2023-11-22 10:02:41.000000 dicomthings-0.7.1/dicomthings/utils.py
+drwxr-xr-x   0 jeroenbertels   (501) staff       (20)        0 2024-04-30 09:47:13.424344 dicomthings-0.7.1/dicomthings.egg-info/
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)      567 2024-04-30 09:47:13.000000 dicomthings-0.7.1/dicomthings.egg-info/PKG-INFO
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)      314 2024-04-30 09:47:13.000000 dicomthings-0.7.1/dicomthings.egg-info/SOURCES.txt
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)        1 2024-04-30 09:47:13.000000 dicomthings-0.7.1/dicomthings.egg-info/dependency_links.txt
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)       12 2024-04-30 09:47:13.000000 dicomthings-0.7.1/dicomthings.egg-info/requires.txt
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)       12 2024-04-30 09:47:13.000000 dicomthings-0.7.1/dicomthings.egg-info/top_level.txt
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)      665 2024-04-30 09:45:16.000000 dicomthings-0.7.1/pyproject.toml
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)       38 2024-04-30 09:47:13.424772 dicomthings-0.7.1/setup.cfg
```

### Comparing `dicomthings-0.7.0/LICENSE` & `dicomthings-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dicomthings-0.7.0/PKG-INFO` & `dicomthings-0.7.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dicomthings
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python library for working with DICOM files.
 Author-email: Jeroen Bertels <jeroen.bertels@gmail.com>
 Project-URL: Homepage, https://github.com/JeroenBertels/dicomthings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dicom2nifti
 
 # dicomthings
 A Python library for working with DICOM files.
```

### Comparing `dicomthings-0.7.0/dicomthings/array.py` & `dicomthings-0.7.1/dicomthings/array.py`

 * *Files identical despite different names*

### Comparing `dicomthings-0.7.0/dicomthings/dicom.py` & `dicomthings-0.7.1/dicomthings/dicom.py`

 * *Files identical despite different names*

### Comparing `dicomthings-0.7.0/dicomthings/nifti.py` & `dicomthings-0.7.1/dicomthings/nifti.py`

 * *Files identical despite different names*

### Comparing `dicomthings-0.7.0/dicomthings/utils.py` & `dicomthings-0.7.1/dicomthings/utils.py`

 * *Files identical despite different names*

### Comparing `dicomthings-0.7.0/dicomthings.egg-info/PKG-INFO` & `dicomthings-0.7.1/dicomthings.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dicomthings
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python library for working with DICOM files.
 Author-email: Jeroen Bertels <jeroen.bertels@gmail.com>
 Project-URL: Homepage, https://github.com/JeroenBertels/dicomthings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dicom2nifti
 
 # dicomthings
 A Python library for working with DICOM files.
```

### Comparing `dicomthings-0.7.0/pyproject.toml` & `dicomthings-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [project]
 name = "dicomthings"
 authors = [
   { name="Jeroen Bertels", email="jeroen.bertels@gmail.com" },
 ]
 description = "A Python library for working with DICOM files."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
 ]
 dynamic = ["version"]
 dependencies = [
```

