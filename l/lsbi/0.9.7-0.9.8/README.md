# Comparing `tmp/lsbi-0.9.7.tar.gz` & `tmp/lsbi-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsbi-0.9.7.tar", last modified: Sat Nov 25 15:15:37 2023, max compression
+gzip compressed data, was "lsbi-0.9.8.tar", last modified: Sat Nov 25 15:24:48 2023, max compression
```

## Comparing `lsbi-0.9.7.tar` & `lsbi-0.9.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 15:15:37.475186 lsbi-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-11-25 15:15:29.000000 lsbi-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2023-11-25 15:15:37.475186 lsbi-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2023-11-25 15:15:29.000000 lsbi-0.9.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 15:15:37.475186 lsbi-0.9.7/lsbi/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-11-25 15:15:29.000000 lsbi-0.9.7/lsbi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-25 15:15:29.000000 lsbi-0.9.7/lsbi/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    20447 2023-11-25 15:15:29.000000 lsbi-0.9.7/lsbi/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2023-11-25 15:15:29.000000 lsbi-0.9.7/lsbi/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2023-11-25 15:15:29.000000 lsbi-0.9.7/lsbi/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2023-11-25 15:15:29.000000 lsbi-0.9.7/lsbi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 15:15:37.475186 lsbi-0.9.7/lsbi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2023-11-25 15:15:37.000000 lsbi-0.9.7/lsbi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-11-25 15:15:37.000000 lsbi-0.9.7/lsbi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-25 15:15:37.000000 lsbi-0.9.7/lsbi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-25 15:15:37.000000 lsbi-0.9.7/lsbi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-25 15:15:37.000000 lsbi-0.9.7/lsbi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2023-11-25 15:15:29.000000 lsbi-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-25 15:15:37.475186 lsbi-0.9.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 15:15:37.475186 lsbi-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    24796 2023-11-25 15:15:29.000000 lsbi-0.9.7/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2023-11-25 15:15:29.000000 lsbi-0.9.7/tests/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-11-25 15:15:29.000000 lsbi-0.9.7/tests/test_scaffolding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2023-11-25 15:15:29.000000 lsbi-0.9.7/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-11-25 15:15:29.000000 lsbi-0.9.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 15:24:48.541195 lsbi-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-11-25 15:24:38.000000 lsbi-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2023-11-25 15:24:48.541195 lsbi-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2023-11-25 15:24:38.000000 lsbi-0.9.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 15:24:48.537196 lsbi-0.9.8/lsbi/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2023-11-25 15:24:38.000000 lsbi-0.9.8/lsbi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-25 15:24:38.000000 lsbi-0.9.8/lsbi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20447 2023-11-25 15:24:38.000000 lsbi-0.9.8/lsbi/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2023-11-25 15:24:38.000000 lsbi-0.9.8/lsbi/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2023-11-25 15:24:38.000000 lsbi-0.9.8/lsbi/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2023-11-25 15:24:38.000000 lsbi-0.9.8/lsbi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 15:24:48.541195 lsbi-0.9.8/lsbi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2023-11-25 15:24:48.000000 lsbi-0.9.8/lsbi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2023-11-25 15:24:48.000000 lsbi-0.9.8/lsbi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-25 15:24:48.000000 lsbi-0.9.8/lsbi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-25 15:24:48.000000 lsbi-0.9.8/lsbi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-25 15:24:48.000000 lsbi-0.9.8/lsbi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2023-11-25 15:24:38.000000 lsbi-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-25 15:24:48.541195 lsbi-0.9.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 15:24:48.541195 lsbi-0.9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    24796 2023-11-25 15:24:38.000000 lsbi-0.9.8/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2023-11-25 15:24:38.000000 lsbi-0.9.8/tests/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-11-25 15:24:38.000000 lsbi-0.9.8/tests/test_scaffolding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2023-11-25 15:24:38.000000 lsbi-0.9.8/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2023-11-25 15:24:38.000000 lsbi-0.9.8/tests/test_utils.py
```

### Comparing `lsbi-0.9.7/LICENSE` & `lsbi-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lsbi-0.9.7/PKG-INFO` & `lsbi-0.9.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsbi
-Version: 0.9.7
+Version: 0.9.8
 Summary: Linear Simulation Based Inference
 Author-email: Will Handley <williamjameshandley@gmail.com>, David Yallup <david.yallup@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Will Handley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,21 +61,24 @@
 Requires-Dist: pre-commit; extra == "test"
 
 =======================================
 lsbi: Linear Simulation Based Inference
 =======================================
 :lsbi: Linear Simulation Based Inference
 :Author: Will Handley & David Yallup
-:Version: 0.9.7
+:Version: 0.9.8
 :Homepage: https://github.com/handley-lab/lsbi
 :Documentation: http://lsbi.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/lsbi/actions/workflows/unittests.yaml/badge.svg?branch=master
    :target: https://github.com/handley-lab/lsbi/actions/workflows/unittests.yaml?query=branch%3Amaster
-   :alt: Build Status
+   :alt: Unit test status
+.. image:: https://github.com/handley-lab/lsbi/actions/workflows/build.yaml/badge.svg?branch=master
+   :target: https://github.com/handley-lab/lsbi/actions/workflows/build.yaml?query=branch%3Amaster
+   :alt: Build status
 .. image:: https://codecov.io/gh/handley-lab/lsbi/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/handley-lab/lsbi
    :alt: Test Coverage Status
 .. image:: https://readthedocs.org/projects/lsbi/badge/?version=latest
    :target: https://lsbi.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: https://badge.fury.io/py/lsbi.svg
```

### Comparing `lsbi-0.9.7/README.rst` & `lsbi-0.9.8/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 =======================================
 lsbi: Linear Simulation Based Inference
 =======================================
 :lsbi: Linear Simulation Based Inference
 :Author: Will Handley & David Yallup
-:Version: 0.9.7
+:Version: 0.9.8
 :Homepage: https://github.com/handley-lab/lsbi
 :Documentation: http://lsbi.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/lsbi/actions/workflows/unittests.yaml/badge.svg?branch=master
    :target: https://github.com/handley-lab/lsbi/actions/workflows/unittests.yaml?query=branch%3Amaster
-   :alt: Build Status
+   :alt: Unit test status
+.. image:: https://github.com/handley-lab/lsbi/actions/workflows/build.yaml/badge.svg?branch=master
+   :target: https://github.com/handley-lab/lsbi/actions/workflows/build.yaml?query=branch%3Amaster
+   :alt: Build status
 .. image:: https://codecov.io/gh/handley-lab/lsbi/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/handley-lab/lsbi
    :alt: Test Coverage Status
 .. image:: https://readthedocs.org/projects/lsbi/badge/?version=latest
    :target: https://lsbi.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: https://badge.fury.io/py/lsbi.svg
```

### Comparing `lsbi-0.9.7/lsbi/model.py` & `lsbi-0.9.8/lsbi/model.py`

 * *Files identical despite different names*

### Comparing `lsbi-0.9.7/lsbi/network.py` & `lsbi-0.9.8/lsbi/network.py`

 * *Files identical despite different names*

### Comparing `lsbi-0.9.7/lsbi/stats.py` & `lsbi-0.9.8/lsbi/stats.py`

 * *Files identical despite different names*

### Comparing `lsbi-0.9.7/lsbi/utils.py` & `lsbi-0.9.8/lsbi/utils.py`

 * *Files identical despite different names*

### Comparing `lsbi-0.9.7/lsbi.egg-info/PKG-INFO` & `lsbi-0.9.8/lsbi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsbi
-Version: 0.9.7
+Version: 0.9.8
 Summary: Linear Simulation Based Inference
 Author-email: Will Handley <williamjameshandley@gmail.com>, David Yallup <david.yallup@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Will Handley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,21 +61,24 @@
 Requires-Dist: pre-commit; extra == "test"
 
 =======================================
 lsbi: Linear Simulation Based Inference
 =======================================
 :lsbi: Linear Simulation Based Inference
 :Author: Will Handley & David Yallup
-:Version: 0.9.7
+:Version: 0.9.8
 :Homepage: https://github.com/handley-lab/lsbi
 :Documentation: http://lsbi.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/lsbi/actions/workflows/unittests.yaml/badge.svg?branch=master
    :target: https://github.com/handley-lab/lsbi/actions/workflows/unittests.yaml?query=branch%3Amaster
-   :alt: Build Status
+   :alt: Unit test status
+.. image:: https://github.com/handley-lab/lsbi/actions/workflows/build.yaml/badge.svg?branch=master
+   :target: https://github.com/handley-lab/lsbi/actions/workflows/build.yaml?query=branch%3Amaster
+   :alt: Build status
 .. image:: https://codecov.io/gh/handley-lab/lsbi/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/handley-lab/lsbi
    :alt: Test Coverage Status
 .. image:: https://readthedocs.org/projects/lsbi/badge/?version=latest
    :target: https://lsbi.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: https://badge.fury.io/py/lsbi.svg
```

### Comparing `lsbi-0.9.7/pyproject.toml` & `lsbi-0.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsbi-0.9.7/tests/test_model.py` & `lsbi-0.9.8/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lsbi-0.9.7/tests/test_networks.py` & `lsbi-0.9.8/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `lsbi-0.9.7/tests/test_stats.py` & `lsbi-0.9.8/tests/test_stats.py`

 * *Files identical despite different names*

