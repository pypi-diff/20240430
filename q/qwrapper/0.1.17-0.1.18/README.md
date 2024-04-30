# Comparing `tmp/qwrapper-0.1.17.tar.gz` & `tmp/qwrapper-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwrapper-0.1.17.tar", last modified: Wed Apr 24 19:44:01 2024, max compression
+gzip compressed data, was "qwrapper-0.1.18.tar", last modified: Tue Apr 30 20:37:32 2024, max compression
```

## Comparing `qwrapper-0.1.17.tar` & `qwrapper-0.1.18.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:01.474137 qwrapper-0.1.17/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-04-24 19:43:56.000000 qwrapper-0.1.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-24 19:44:01.474137 qwrapper-0.1.17/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-04-24 19:43:56.000000 qwrapper-0.1.17/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      626 2024-04-24 19:43:56.000000 qwrapper-0.1.17/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:01.470137 qwrapper-0.1.17/qwrapper/
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/qemumachine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:01.474137 qwrapper-0.1.17/qwrapper/x86/
--rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:01.474137 qwrapper-0.1.17/qwrapper/x86/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/utils/debugging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1041 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/utils/machinestate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1147 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/utils/memory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2432 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/utils/registers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4116 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/x86machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:01.474137 qwrapper-0.1.17/qwrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-24 19:44:01.000000 qwrapper-0.1.17/qwrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-24 19:44:01.000000 qwrapper-0.1.17/qwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:44:01.000000 qwrapper-0.1.17/qwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 19:44:01.000000 qwrapper-0.1.17/qwrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 19:44:01.000000 qwrapper-0.1.17/qwrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:44:01.474137 qwrapper-0.1.17/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:01.474137 qwrapper-0.1.17/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 19:43:56.000000 qwrapper-0.1.17/tests/test_qwrapper_x86.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:37:32.808591 qwrapper-0.1.18/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-04-30 20:37:28.000000 qwrapper-0.1.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-30 20:37:32.808591 qwrapper-0.1.18/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1160 2024-04-30 20:37:28.000000 qwrapper-0.1.18/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      626 2024-04-30 20:37:28.000000 qwrapper-0.1.18/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:37:32.808591 qwrapper-0.1.18/qwrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-30 20:37:28.000000 qwrapper-0.1.18/qwrapper/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-04-30 20:37:28.000000 qwrapper-0.1.18/qwrapper/qemumachine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:37:32.808591 qwrapper-0.1.18/qwrapper/x86/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-04-30 20:37:28.000000 qwrapper-0.1.18/qwrapper/x86/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:37:32.808591 qwrapper-0.1.18/qwrapper/x86/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:37:28.000000 qwrapper-0.1.18/qwrapper/x86/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-04-30 20:37:28.000000 qwrapper-0.1.18/qwrapper/x86/utils/debugging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1041 2024-04-30 20:37:28.000000 qwrapper-0.1.18/qwrapper/x86/utils/machinestate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1147 2024-04-30 20:37:28.000000 qwrapper-0.1.18/qwrapper/x86/utils/memory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2432 2024-04-30 20:37:28.000000 qwrapper-0.1.18/qwrapper/x86/utils/registers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4116 2024-04-30 20:37:28.000000 qwrapper-0.1.18/qwrapper/x86/x86machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:37:32.808591 qwrapper-0.1.18/qwrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-30 20:37:32.000000 qwrapper-0.1.18/qwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-30 20:37:32.000000 qwrapper-0.1.18/qwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:37:32.000000 qwrapper-0.1.18/qwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 20:37:32.000000 qwrapper-0.1.18/qwrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 20:37:32.000000 qwrapper-0.1.18/qwrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:37:32.808591 qwrapper-0.1.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:37:32.808591 qwrapper-0.1.18/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 20:37:28.000000 qwrapper-0.1.18/tests/test_qwrapper_x86.py
```

### Comparing `qwrapper-0.1.17/LICENSE` & `qwrapper-0.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.17/PKG-INFO` & `qwrapper-0.1.18/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwrapper
-Version: 0.1.17
+Version: 0.1.18
 Summary: A QEMU wrapper for Python
 Author-email: Daniel Dybing <danieldy@uia.no>, Ali Sirvanovitsj Ismailov <alisi18@uia.no>, Sirén Elise Lund Lohre <selohre@uia.no>
 License: MIT License
         
         Copyright (c) 2024 Ali Ismailov, Daniel Dybing, Sirén Elise Lund Lohre
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygdbmi
 Requires-Dist: qemu.qmp
 
-# QWrapper
+<p align="center">
+  <img src="logo.png" />
+</p>
+
+
+
+
+
+
 
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/ddybing/qwrapper/pypi-publish.yml)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qwrapper)
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/qwrapper)
```

### Comparing `qwrapper-0.1.17/README.md` & `qwrapper-0.1.18/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,16 @@
-# QWrapper
+<p align="center">
+  <img src="logo.png" />
+</p>
+
+
+
+
+
+
 
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/ddybing/qwrapper/pypi-publish.yml)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qwrapper)
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/qwrapper)
```

### Comparing `qwrapper-0.1.17/pyproject.toml` & `qwrapper-0.1.18/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 [project]
 license = { file = "LICENSE" }
 name = "qwrapper"
-version = "0.1.17"
+version = "0.1.18"
 description = "A QEMU wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [{ name = "Daniel Dybing", email = "danieldy@uia.no" },
            { name = "Ali Sirvanovitsj Ismailov", email = "alisi18@uia.no"},
            { name = "Sirén Elise Lund Lohre", email = "selohre@uia.no"}]
 classifiers = [
```

### Comparing `qwrapper-0.1.17/qwrapper/qemumachine.py` & `qwrapper-0.1.18/qwrapper/qemumachine.py`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.17/qwrapper/x86/utils/machinestate.py` & `qwrapper-0.1.18/qwrapper/x86/utils/machinestate.py`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.17/qwrapper/x86/utils/memory.py` & `qwrapper-0.1.18/qwrapper/x86/utils/memory.py`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.17/qwrapper/x86/utils/registers.py` & `qwrapper-0.1.18/qwrapper/x86/utils/registers.py`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.17/qwrapper/x86/x86machine.py` & `qwrapper-0.1.18/qwrapper/x86/x86machine.py`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.17/qwrapper.egg-info/PKG-INFO` & `qwrapper-0.1.18/qwrapper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwrapper
-Version: 0.1.17
+Version: 0.1.18
 Summary: A QEMU wrapper for Python
 Author-email: Daniel Dybing <danieldy@uia.no>, Ali Sirvanovitsj Ismailov <alisi18@uia.no>, Sirén Elise Lund Lohre <selohre@uia.no>
 License: MIT License
         
         Copyright (c) 2024 Ali Ismailov, Daniel Dybing, Sirén Elise Lund Lohre
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygdbmi
 Requires-Dist: qemu.qmp
 
-# QWrapper
+<p align="center">
+  <img src="logo.png" />
+</p>
+
+
+
+
+
+
 
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/ddybing/qwrapper/pypi-publish.yml)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qwrapper)
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/qwrapper)
```

