# Comparing `tmp/pychoreographer-0.0.6.tar.gz` & `tmp/pychoreographer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychoreographer-0.0.6.tar", last modified: Sat Mar 16 22:45:05 2024, max compression
+gzip compressed data, was "pychoreographer-0.0.8.tar", last modified: Tue Apr 30 21:12:15 2024, max compression
```

## Comparing `pychoreographer-0.0.6.tar` & `pychoreographer-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 22:45:05.825767 pychoreographer-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-16 22:44:54.000000 pychoreographer-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-16 22:45:05.825767 pychoreographer-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-03-16 22:44:54.000000 pychoreographer-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 22:45:05.825767 pychoreographer-0.0.6/pychoreographer/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-16 22:44:54.000000 pychoreographer-0.0.6/pychoreographer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-03-16 22:44:54.000000 pychoreographer-0.0.6/pychoreographer/files_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-03-16 22:44:54.000000 pychoreographer-0.0.6/pychoreographer/pychoreographer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 22:45:05.825767 pychoreographer-0.0.6/pychoreographer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-16 22:45:05.000000 pychoreographer-0.0.6/pychoreographer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-16 22:45:05.000000 pychoreographer-0.0.6/pychoreographer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 22:45:05.000000 pychoreographer-0.0.6/pychoreographer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-16 22:45:05.000000 pychoreographer-0.0.6/pychoreographer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-16 22:44:54.000000 pychoreographer-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 22:45:05.825767 pychoreographer-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-16 22:44:54.000000 pychoreographer-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:12:15.214751 pychoreographer-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-30 21:12:05.000000 pychoreographer-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-30 21:12:15.214751 pychoreographer-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-30 21:12:05.000000 pychoreographer-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:12:15.210751 pychoreographer-0.0.8/pychoreographer/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-30 21:12:05.000000 pychoreographer-0.0.8/pychoreographer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:12:15.214751 pychoreographer-0.0.8/pychoreographer/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 21:12:05.000000 pychoreographer-0.0.8/pychoreographer/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-30 21:12:05.000000 pychoreographer-0.0.8/pychoreographer/files/files_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-30 21:12:05.000000 pychoreographer-0.0.8/pychoreographer/pychoreographer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:12:15.210751 pychoreographer-0.0.8/pychoreographer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-30 21:12:15.000000 pychoreographer-0.0.8/pychoreographer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-30 21:12:15.000000 pychoreographer-0.0.8/pychoreographer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:12:15.000000 pychoreographer-0.0.8/pychoreographer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 21:12:15.000000 pychoreographer-0.0.8/pychoreographer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-30 21:12:05.000000 pychoreographer-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 21:12:15.214751 pychoreographer-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 21:12:05.000000 pychoreographer-0.0.8/setup.py
```

### Comparing `pychoreographer-0.0.6/LICENSE` & `pychoreographer-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pychoreographer-0.0.6/PKG-INFO` & `pychoreographer-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychoreographer
-Version: 0.0.6
+Version: 0.0.8
 Summary: Python library for automating file ops, system monitoring
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pychoreographer-0.0.6/README.md` & `pychoreographer-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pychoreographer-0.0.6/pychoreographer/files_operations.py` & `pychoreographer-0.0.8/pychoreographer/files/files_operations.py`

 * *Files identical despite different names*

### Comparing `pychoreographer-0.0.6/pychoreographer/pychoreographer.py` & `pychoreographer-0.0.8/pychoreographer/pychoreographer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Console script for pychoreo."""
 import os
 import sys
 import subprocess
 import json
 import click
-from files_operations import delete_empty_folders, delete_old_files, organize_files_extensions
+from files.files_operations import delete_empty_folders, delete_old_files, organize_files_extensions
 
 
 @click.group()
 def cli():
     """A customizable Python library for automating file operations, system monitoring, and routine tasks"""  # noqa
     pass
```

### Comparing `pychoreographer-0.0.6/pychoreographer.egg-info/PKG-INFO` & `pychoreographer-0.0.8/pychoreographer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychoreographer
-Version: 0.0.6
+Version: 0.0.8
 Summary: Python library for automating file ops, system monitoring
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pychoreographer-0.0.6/pyproject.toml` & `pychoreographer-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]  # Dependencies for building your package
 build-backend = "setuptools.build_meta" 
 
 
 [project]
 name = "Pychoreographer"
-version = "0.0.6"
+version = "0.0.8"
 authors = [
   { name="Rajaa Lebchiri", email="rajaa.lebchiri@gmail.com" },
 ]
 description = "A customizable Python library for automating file operations, system monitoring, and routine tasks."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

