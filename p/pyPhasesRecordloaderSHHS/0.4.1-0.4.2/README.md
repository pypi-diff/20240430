# Comparing `tmp/pyPhasesRecordloaderSHHS-0.4.1.tar.gz` & `tmp/pyPhasesRecordloaderSHHS-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesRecordloaderSHHS-0.4.1.tar", last modified: Sat Sep 16 09:19:59 2023, max compression
+gzip compressed data, was "pyPhasesRecordloaderSHHS-0.4.2.tar", last modified: Tue Apr 30 06:58:00 2024, max compression
```

## Comparing `pyPhasesRecordloaderSHHS-0.4.1.tar` & `pyPhasesRecordloaderSHHS-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-16 09:19:59.195584 pyPhasesRecordloaderSHHS-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     1116 2023-09-16 09:19:41.000000 pyPhasesRecordloaderSHHS-0.4.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-09-16 09:19:41.000000 pyPhasesRecordloaderSHHS-0.4.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-09-16 09:19:41.000000 pyPhasesRecordloaderSHHS-0.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1487 2023-09-16 09:19:59.194584 pyPhasesRecordloaderSHHS-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-09-16 09:19:41.000000 pyPhasesRecordloaderSHHS-0.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-16 09:19:59.193584 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/
--rw-rw-rw-   0 root         (0) root         (0)     1491 2023-09-16 09:19:41.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     5080 2023-09-16 09:19:41.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/RecordManager.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-09-16 09:19:41.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2023-09-16 09:19:41.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-16 09:19:59.192584 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/configs/
--rw-rw-rw-   0 root         (0) root         (0)     3314 2023-09-16 09:19:41.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/configs/shhs.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3524 2023-09-16 09:19:41.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/configs/shhs2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-16 09:19:59.194584 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/recordLoaders/
--rw-rw-rw-   0 root         (0) root         (0)     4070 2023-09-16 09:19:41.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/recordLoaders/RecordLoaderSHHS.py
--rw-rw-rw-   0 root         (0) root         (0)     5185 2023-09-16 09:19:41.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/recordLoaders/SHHSAnnotationLoader.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-16 09:19:41.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/recordLoaders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-16 09:19:59.194584 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1487 2023-09-16 09:19:59.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      835 2023-09-16 09:19:59.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-16 09:19:59.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-09-16 09:19:59.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-09-16 09:19:59.000000 pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-16 09:19:59.195584 pyPhasesRecordloaderSHHS-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      898 2023-09-16 09:19:42.000000 pyPhasesRecordloaderSHHS-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:58:00.789741 pyPhasesRecordloaderSHHS-0.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2024-04-30 06:57:41.000000 pyPhasesRecordloaderSHHS-0.4.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-04-30 06:57:41.000000 pyPhasesRecordloaderSHHS-0.4.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-30 06:57:41.000000 pyPhasesRecordloaderSHHS-0.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-04-30 06:58:00.788741 pyPhasesRecordloaderSHHS-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      998 2024-04-30 06:57:41.000000 pyPhasesRecordloaderSHHS-0.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:58:00.787741 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2024-04-30 06:57:41.000000 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-30 06:57:41.000000 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2024-04-30 06:57:41.000000 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:58:00.786741 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/configs/
+-rw-rw-rw-   0 root         (0) root         (0)     3337 2024-04-30 06:57:41.000000 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/configs/shhs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3547 2024-04-30 06:57:41.000000 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/configs/shhs2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:58:00.788741 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/recordLoaders/
+-rw-rw-rw-   0 root         (0) root         (0)     4070 2024-04-30 06:57:41.000000 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/recordLoaders/RecordLoaderSHHS.py
+-rw-rw-rw-   0 root         (0) root         (0)     5185 2024-04-30 06:57:41.000000 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/recordLoaders/SHHSAnnotationLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 06:57:41.000000 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/recordLoaders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:58:00.788741 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-04-30 06:58:00.000000 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      793 2024-04-30 06:58:00.000000 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 06:58:00.000000 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-30 06:58:00.000000 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-30 06:58:00.000000 pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 06:58:00.789741 pyPhasesRecordloaderSHHS-0.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      898 2024-04-30 06:57:42.000000 pyPhasesRecordloaderSHHS-0.4.2/setup.py
```

### Comparing `pyPhasesRecordloaderSHHS-0.4.1/.gitlab-ci.yml` & `pyPhasesRecordloaderSHHS-0.4.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderSHHS-0.4.1/LICENSE` & `pyPhasesRecordloaderSHHS-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderSHHS-0.4.1/PKG-INFO` & `pyPhasesRecordloaderSHHS-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesRecordloaderSHHS
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

### Comparing `pyPhasesRecordloaderSHHS-0.4.1/README.md` & `pyPhasesRecordloaderSHHS-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/Plugin.py` & `pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/configs/shhs.yaml` & `pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/configs/shhs.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 loader:
   shhs:
     dataBase: SHHS1
     dataBaseVersion: 1.0.0 # needs to be raised every time new data is added
 
     filePath: ./datasets/SHHS1
     copyRawDataToLocal: True
+    dataIsFinal: True
 
     dataset:
       loaderName: RecordLoaderSHHS
       fromFiles: True # if the records are read from files or sql-database
       downloader:
         type: nsrr
         listFilter: null
```

### Comparing `pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/configs/shhs2.yaml` & `pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/configs/shhs2.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 loader:
   shhs2:
     dataBase: SHHS2
     dataBaseVersion: 1.0.0 # needs to be raised every time new data is added
 
     filePath: ./datasets/SHHS2
     copyRawDataToLocal: True
+    dataIsFinal: True
 
     dataset:
       loaderName: RecordLoaderSHHS
       fromFiles: True # if the records are read from files or sql-database
       downloader:
         type: nsrr
         listFilter: null
```

### Comparing `pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/recordLoaders/RecordLoaderSHHS.py` & `pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/recordLoaders/RecordLoaderSHHS.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS/recordLoaders/SHHSAnnotationLoader.py` & `pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS/recordLoaders/SHHSAnnotationLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS.egg-info/PKG-INFO` & `pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesRecordloaderSHHS
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

### Comparing `pyPhasesRecordloaderSHHS-0.4.1/pyPhasesRecordloaderSHHS.egg-info/SOURCES.txt` & `pyPhasesRecordloaderSHHS-0.4.2/pyPhasesRecordloaderSHHS.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.md
 setup.py
 ./.gitlab-ci.yml
 ./pyPhasesRecordloaderSHHS/config.yaml
 ./pyPhasesRecordloaderSHHS/configs/shhs.yaml
 ./pyPhasesRecordloaderSHHS/configs/shhs2.yaml
 pyPhasesRecordloaderSHHS/Plugin.py
-pyPhasesRecordloaderSHHS/RecordManager.py
 pyPhasesRecordloaderSHHS/__init__.py
 pyPhasesRecordloaderSHHS/config.yaml
 pyPhasesRecordloaderSHHS.egg-info/PKG-INFO
 pyPhasesRecordloaderSHHS.egg-info/SOURCES.txt
 pyPhasesRecordloaderSHHS.egg-info/dependency_links.txt
 pyPhasesRecordloaderSHHS.egg-info/requires.txt
 pyPhasesRecordloaderSHHS.egg-info/top_level.txt
```

### Comparing `pyPhasesRecordloaderSHHS-0.4.1/setup.py` & `pyPhasesRecordloaderSHHS-0.4.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesRecordloaderSHHS",
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

