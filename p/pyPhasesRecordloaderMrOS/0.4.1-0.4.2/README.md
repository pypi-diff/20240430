# Comparing `tmp/pyPhasesRecordloaderMrOS-0.4.1.tar.gz` & `tmp/pyPhasesRecordloaderMrOS-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesRecordloaderMrOS-0.4.1.tar", last modified: Fri Feb 16 11:04:06 2024, max compression
+gzip compressed data, was "pyPhasesRecordloaderMrOS-0.4.2.tar", last modified: Tue Apr 30 06:57:17 2024, max compression
```

## Comparing `pyPhasesRecordloaderMrOS-0.4.1.tar` & `pyPhasesRecordloaderMrOS-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:04:06.942631 pyPhasesRecordloaderMrOS-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     1116 2024-02-16 11:03:48.000000 pyPhasesRecordloaderMrOS-0.4.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1086 2024-02-16 11:03:48.000000 pyPhasesRecordloaderMrOS-0.4.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-02-16 11:03:48.000000 pyPhasesRecordloaderMrOS-0.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1439 2024-02-16 11:04:06.942631 pyPhasesRecordloaderMrOS-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      950 2024-02-16 11:03:48.000000 pyPhasesRecordloaderMrOS-0.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:04:06.941631 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS/
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-02-16 11:03:48.000000 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2024-02-16 11:03:48.000000 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5559 2024-02-16 11:03:48.000000 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:04:06.942631 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS/recordLoaders/
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-02-16 11:03:48.000000 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS/recordLoaders/MrOSAnnotationLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     3387 2024-02-16 11:03:48.000000 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS/recordLoaders/RecordLoaderMrOS.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-16 11:03:48.000000 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS/recordLoaders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:04:06.942631 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1439 2024-02-16 11:04:06.000000 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      615 2024-02-16 11:04:06.000000 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-16 11:04:06.000000 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-02-16 11:04:06.000000 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-02-16 11:04:06.000000 pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-16 11:04:06.943631 pyPhasesRecordloaderMrOS-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      871 2024-02-16 11:03:49.000000 pyPhasesRecordloaderMrOS-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:57:17.360912 pyPhasesRecordloaderMrOS-0.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2024-04-30 06:56:57.000000 pyPhasesRecordloaderMrOS-0.4.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-04-30 06:56:57.000000 pyPhasesRecordloaderMrOS-0.4.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-30 06:56:57.000000 pyPhasesRecordloaderMrOS-0.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-04-30 06:57:17.360912 pyPhasesRecordloaderMrOS-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      950 2024-04-30 06:56:57.000000 pyPhasesRecordloaderMrOS-0.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:57:17.358912 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS/
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-04-30 06:56:57.000000 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-30 06:56:57.000000 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5582 2024-04-30 06:56:57.000000 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:57:17.360912 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS/recordLoaders/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-30 06:56:57.000000 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS/recordLoaders/MrOSAnnotationLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3387 2024-04-30 06:56:57.000000 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS/recordLoaders/RecordLoaderMrOS.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 06:56:57.000000 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS/recordLoaders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:57:17.359912 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-04-30 06:57:17.000000 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      615 2024-04-30 06:57:17.000000 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 06:57:17.000000 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-30 06:57:17.000000 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-30 06:57:17.000000 pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 06:57:17.360912 pyPhasesRecordloaderMrOS-0.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      871 2024-04-30 06:56:59.000000 pyPhasesRecordloaderMrOS-0.4.2/setup.py
```

### Comparing `pyPhasesRecordloaderMrOS-0.4.1/.gitlab-ci.yml` & `pyPhasesRecordloaderMrOS-0.4.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderMrOS-0.4.1/LICENSE` & `pyPhasesRecordloaderMrOS-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderMrOS-0.4.1/PKG-INFO` & `pyPhasesRecordloaderMrOS-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesRecordloaderMrOS
-Version: 0.4.1
+Version: 0.4.2
 Summary: Adds a record loaders to the pyPhases package
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesRecordloaderMrOS-0.4.1/README.md` & `pyPhasesRecordloaderMrOS-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS/Plugin.py` & `pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS/config.yaml` & `pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
   mros: &mros
     dataBase: mros
     dataBaseVersion: 1.0.0 # needs to be raised every time new data is added
 
     filePath: ./datasets/mros
     copyRawDataToLocal: True
+    dataIsFinal: True
 
     dataset:
       loaderName: RecordLoaderMrOS
       fromFiles: True # if the records are read from files or sql-database
       downloader:
         type: nsrr
         listFilter: null
```

### Comparing `pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS/recordLoaders/RecordLoaderMrOS.py` & `pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS/recordLoaders/RecordLoaderMrOS.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS.egg-info/PKG-INFO` & `pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesRecordloaderMrOS
-Version: 0.4.1
+Version: 0.4.2
 Summary: Adds a record loaders to the pyPhases package
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesRecordloaderMrOS-0.4.1/pyPhasesRecordloaderMrOS.egg-info/SOURCES.txt` & `pyPhasesRecordloaderMrOS-0.4.2/pyPhasesRecordloaderMrOS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderMrOS-0.4.1/setup.py` & `pyPhasesRecordloaderMrOS-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesRecordloaderMrOS",
-    version="v0.4.1"[1:],
+    version="v0.4.2"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="Adds a record loaders to the pyPhases package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/",
     packages=setuptools.find_packages(),
```

