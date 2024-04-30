# Comparing `tmp/pyPhasesRecordloaderMESA-0.2.1.tar.gz` & `tmp/pyPhasesRecordloaderMESA-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesRecordloaderMESA-0.2.1.tar", last modified: Tue Apr 30 06:58:24 2024, max compression
+gzip compressed data, was "pyPhasesRecordloaderMESA-0.2.2.tar", last modified: Tue Apr 30 06:58:23 2024, max compression
```

## Comparing `pyPhasesRecordloaderMESA-0.2.1.tar` & `pyPhasesRecordloaderMESA-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:58:24.073875 pyPhasesRecordloaderMESA-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1116 2024-04-30 06:58:03.000000 pyPhasesRecordloaderMESA-0.2.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-04-30 06:58:03.000000 pyPhasesRecordloaderMESA-0.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-30 06:58:03.000000 pyPhasesRecordloaderMESA-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1460 2024-04-30 06:58:24.073875 pyPhasesRecordloaderMESA-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      971 2024-04-30 06:58:03.000000 pyPhasesRecordloaderMESA-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:58:24.071874 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA/
--rw-rw-rw-   0 root         (0) root         (0)      888 2024-04-30 06:58:03.000000 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-30 06:58:03.000000 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2527 2024-04-30 06:58:03.000000 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:58:24.073875 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA/recordLoaders/
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-30 06:58:03.000000 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA/recordLoaders/MESAAnnotationLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     2209 2024-04-30 06:58:03.000000 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA/recordLoaders/RecordLoaderMESA.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 06:58:03.000000 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA/recordLoaders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:58:24.072875 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1460 2024-04-30 06:58:24.000000 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      615 2024-04-30 06:58:24.000000 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 06:58:24.000000 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-30 06:58:24.000000 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-30 06:58:24.000000 pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 06:58:24.073875 pyPhasesRecordloaderMESA-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-04-30 06:58:04.000000 pyPhasesRecordloaderMESA-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:58:23.865235 pyPhasesRecordloaderMESA-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2024-04-30 06:58:04.000000 pyPhasesRecordloaderMESA-0.2.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-04-30 06:58:04.000000 pyPhasesRecordloaderMESA-0.2.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-30 06:58:04.000000 pyPhasesRecordloaderMESA-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1460 2024-04-30 06:58:23.865235 pyPhasesRecordloaderMESA-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      971 2024-04-30 06:58:04.000000 pyPhasesRecordloaderMESA-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:58:23.863405 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA/
+-rw-rw-rw-   0 root         (0) root         (0)      888 2024-04-30 06:58:04.000000 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-30 06:58:04.000000 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2527 2024-04-30 06:58:04.000000 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:58:23.865235 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA/recordLoaders/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-30 06:58:04.000000 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA/recordLoaders/MESAAnnotationLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     2209 2024-04-30 06:58:04.000000 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA/recordLoaders/RecordLoaderMESA.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 06:58:04.000000 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA/recordLoaders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:58:23.864320 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1460 2024-04-30 06:58:23.000000 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      615 2024-04-30 06:58:23.000000 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 06:58:23.000000 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-30 06:58:23.000000 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-30 06:58:23.000000 pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 06:58:23.865235 pyPhasesRecordloaderMESA-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-04-30 06:58:05.000000 pyPhasesRecordloaderMESA-0.2.2/setup.py
```

### Comparing `pyPhasesRecordloaderMESA-0.2.1/.gitlab-ci.yml` & `pyPhasesRecordloaderMESA-0.2.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderMESA-0.2.1/LICENSE` & `pyPhasesRecordloaderMESA-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderMESA-0.2.1/PKG-INFO` & `pyPhasesRecordloaderMESA-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesRecordloaderMESA
-Version: 0.2.1
+Version: 0.2.2
 Summary: Adds a record loaders to the pyPhases package
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesRecordloaderMESA-0.2.1/README.md` & `pyPhasesRecordloaderMESA-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA/Plugin.py` & `pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA/config.yaml` & `pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA/recordLoaders/RecordLoaderMESA.py` & `pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA/recordLoaders/RecordLoaderMESA.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA.egg-info/PKG-INFO` & `pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesRecordloaderMESA
-Version: 0.2.1
+Version: 0.2.2
 Summary: Adds a record loaders to the pyPhases package
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesRecordloaderMESA-0.2.1/pyPhasesRecordloaderMESA.egg-info/SOURCES.txt` & `pyPhasesRecordloaderMESA-0.2.2/pyPhasesRecordloaderMESA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderMESA-0.2.1/setup.py` & `pyPhasesRecordloaderMESA-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesRecordloaderMESA",
-    version="v0.2.1"[1:],
+    version="v0.2.2"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="Adds a record loaders to the pyPhases package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/",
     packages=setuptools.find_packages(),
```

