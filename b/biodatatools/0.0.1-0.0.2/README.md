# Comparing `tmp/biodatatools-0.0.1.tar.gz` & `tmp/biodatatools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biodatatools-0.0.1.tar", last modified: Tue Apr 30 02:58:25 2024, max compression
+gzip compressed data, was "biodatatools-0.0.2.tar", last modified: Tue Apr 30 03:10:45 2024, max compression
```

## Comparing `biodatatools-0.0.1.tar` & `biodatatools-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 02:58:25.640177 biodatatools-0.0.1/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      785 2024-04-30 02:58:25.639177 biodatatools-0.0.1/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      177 2024-04-24 07:09:47.000000 biodatatools-0.0.1/README.md
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 02:58:25.638177 biodatatools-0.0.1/biodatatools/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)    11004 2024-04-30 02:53:35.000000 biodatatools-0.0.1/biodatatools/__init__.py
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 02:58:25.639177 biodatatools-0.0.1/biodatatools.egg-info/
--rw-r--r--   0 kl945     (5298) hy299_0001 (80905)      785 2024-04-30 02:58:25.000000 biodatatools-0.0.1/biodatatools.egg-info/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      261 2024-04-30 02:58:25.000000 biodatatools-0.0.1/biodatatools.egg-info/SOURCES.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2024-04-30 02:58:25.000000 biodatatools-0.0.1/biodatatools.egg-info/dependency_links.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       51 2024-04-30 02:58:25.000000 biodatatools-0.0.1/biodatatools.egg-info/entry_points.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      118 2024-04-30 02:58:25.000000 biodatatools-0.0.1/biodatatools.egg-info/requires.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       13 2024-04-30 02:58:25.000000 biodatatools-0.0.1/biodatatools.egg-info/top_level.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2024-04-30 02:58:25.640177 biodatatools-0.0.1/setup.cfg
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     1078 2024-04-30 02:57:22.000000 biodatatools-0.0.1/setup.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 03:10:45.207139 biodatatools-0.0.2/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      785 2024-04-30 03:10:45.206139 biodatatools-0.0.2/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      177 2024-04-24 07:09:47.000000 biodatatools-0.0.2/README.md
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 03:10:45.204139 biodatatools-0.0.2/biodatatools/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)    11004 2024-04-30 03:09:35.000000 biodatatools-0.0.2/biodatatools/__init__.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 03:10:45.206139 biodatatools-0.0.2/biodatatools.egg-info/
+-rw-r--r--   0 kl945     (5298) hy299_0001 (80905)      785 2024-04-30 03:10:45.000000 biodatatools-0.0.2/biodatatools.egg-info/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      261 2024-04-30 03:10:45.000000 biodatatools-0.0.2/biodatatools.egg-info/SOURCES.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2024-04-30 03:10:45.000000 biodatatools-0.0.2/biodatatools.egg-info/dependency_links.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       51 2024-04-30 03:10:45.000000 biodatatools-0.0.2/biodatatools.egg-info/entry_points.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      132 2024-04-30 03:10:45.000000 biodatatools-0.0.2/biodatatools.egg-info/requires.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       13 2024-04-30 03:10:45.000000 biodatatools-0.0.2/biodatatools.egg-info/top_level.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2024-04-30 03:10:45.207139 biodatatools-0.0.2/setup.cfg
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     1095 2024-04-30 03:09:21.000000 biodatatools-0.0.2/setup.py
```

### Comparing `biodatatools-0.0.1/PKG-INFO` & `biodatatools-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biodatatools
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package with useful biological data processing methods
 Home-page: https://github.com/aldenleung/biodatatools/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biodatatools-0.0.1/biodatatools/__init__.py` & `biodatatools-0.0.2/biodatatools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 import simplevc
-simplevc.register(sys.modules[__name__], "0.0.1")
+simplevc.register(sys.modules[__name__], "0.0.2")
 
 import tempfile
 import os
 import subprocess
 import shutil
 
 import pysam
```

### Comparing `biodatatools-0.0.1/biodatatools.egg-info/PKG-INFO` & `biodatatools-0.0.2/biodatatools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biodatatools
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package with useful biological data processing methods
 Home-page: https://github.com/aldenleung/biodatatools/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biodatatools-0.0.1/setup.py` & `biodatatools-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as readme_file:
 	readme = readme_file.read()
 
-requirements = ["genomictools>=0.0.7", "biodata>=0.0.6", "pysam>=0.22.1", "pyBigWig>=0.3.22", "simplevc>=0.0.2", "commonhelper>=0.0.1", "mphelper>=0.0.1"]
+requirements = ["genomictools>=0.0.7", "biodata>=0.0.6", "pysam>=0.22.1", "pyBigWig>=0.3.22", "simplevc>=0.0.2", "commonhelper>=0.0.1", "mphelper>=0.0.1", "numpy>=1.26.4"]
 
 setup(
 	name="biodatatools",
-	version="0.0.1",
+	version="0.0.2",
 	author="Alden Leung",
 	author_email="alden.leung@gmail.com",
 	description="A python package with useful biological data processing methods",
 	long_description=readme,
 	long_description_content_type="text/markdown",
 	url="https://github.com/aldenleung/biodatatools/",
 	packages=find_packages(),
```

