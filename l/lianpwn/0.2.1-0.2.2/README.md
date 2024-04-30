# Comparing `tmp/lianpwn-0.2.1.tar.gz` & `tmp/lianpwn-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lianpwn-0.2.1.tar", last modified: Tue Apr 30 10:52:21 2024, max compression
+gzip compressed data, was "lianpwn-0.2.2.tar", last modified: Tue Apr 30 10:53:36 2024, max compression
```

## Comparing `lianpwn-0.2.1.tar` & `lianpwn-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 eastxuelian  (1000) eastxuelian  (1000)        0 2024-04-30 10:52:21.438606 lianpwn-0.2.1/
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)     2400 2024-04-29 13:07:59.000000 lianpwn-0.2.1/LICENSE
--rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)      400 2024-04-30 10:52:21.438606 lianpwn-0.2.1/PKG-INFO
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)       10 2024-04-29 13:07:59.000000 lianpwn-0.2.1/README.md
-drwxrwxr-x   0 eastxuelian  (1000) eastxuelian  (1000)        0 2024-04-30 10:52:21.438606 lianpwn-0.2.1/lianpwn/
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)     2873 2024-04-29 13:07:59.000000 lianpwn-0.2.1/lianpwn/__init__.py
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      241 2024-04-30 10:45:08.000000 lianpwn-0.2.1/lianpwn/cli.py
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      754 2024-04-29 13:07:59.000000 lianpwn-0.2.1/lianpwn/nocli.py
--rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)      751 2024-04-30 10:51:30.000000 lianpwn-0.2.1/lianpwn/template_gen.py
-drwxrwxr-x   0 eastxuelian  (1000) eastxuelian  (1000)        0 2024-04-30 10:52:21.438606 lianpwn-0.2.1/lianpwn.egg-info/
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      400 2024-04-30 10:52:21.000000 lianpwn-0.2.1/lianpwn.egg-info/PKG-INFO
--rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)      290 2024-04-30 10:52:21.000000 lianpwn-0.2.1/lianpwn.egg-info/SOURCES.txt
--rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)        1 2024-04-30 10:52:21.000000 lianpwn-0.2.1/lianpwn.egg-info/dependency_links.txt
--rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)       44 2024-04-30 10:52:21.000000 lianpwn-0.2.1/lianpwn.egg-info/entry_points.txt
--rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)       22 2024-04-30 10:52:21.000000 lianpwn-0.2.1/lianpwn.egg-info/requires.txt
--rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)        8 2024-04-30 10:52:21.000000 lianpwn-0.2.1/lianpwn.egg-info/top_level.txt
--rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)       38 2024-04-30 10:52:21.438606 lianpwn-0.2.1/setup.cfg
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      756 2024-04-30 10:52:10.000000 lianpwn-0.2.1/setup.py
+drwxrwxr-x   0 eastxuelian  (1000) eastxuelian  (1000)        0 2024-04-30 10:53:36.855625 lianpwn-0.2.2/
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)     2400 2024-04-29 13:07:59.000000 lianpwn-0.2.2/LICENSE
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)      400 2024-04-30 10:53:36.855625 lianpwn-0.2.2/PKG-INFO
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)       10 2024-04-29 13:07:59.000000 lianpwn-0.2.2/README.md
+drwxrwxr-x   0 eastxuelian  (1000) eastxuelian  (1000)        0 2024-04-30 10:53:36.855625 lianpwn-0.2.2/lianpwn/
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)     2873 2024-04-29 13:07:59.000000 lianpwn-0.2.2/lianpwn/__init__.py
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      241 2024-04-30 10:45:08.000000 lianpwn-0.2.2/lianpwn/cli.py
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      754 2024-04-29 13:07:59.000000 lianpwn-0.2.2/lianpwn/nocli.py
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)      759 2024-04-30 10:53:21.000000 lianpwn-0.2.2/lianpwn/template_gen.py
+drwxrwxr-x   0 eastxuelian  (1000) eastxuelian  (1000)        0 2024-04-30 10:53:36.855625 lianpwn-0.2.2/lianpwn.egg-info/
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      400 2024-04-30 10:53:36.000000 lianpwn-0.2.2/lianpwn.egg-info/PKG-INFO
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)      290 2024-04-30 10:53:36.000000 lianpwn-0.2.2/lianpwn.egg-info/SOURCES.txt
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)        1 2024-04-30 10:53:36.000000 lianpwn-0.2.2/lianpwn.egg-info/dependency_links.txt
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)       44 2024-04-30 10:53:36.000000 lianpwn-0.2.2/lianpwn.egg-info/entry_points.txt
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)       22 2024-04-30 10:53:36.000000 lianpwn-0.2.2/lianpwn.egg-info/requires.txt
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)        8 2024-04-30 10:53:36.000000 lianpwn-0.2.2/lianpwn.egg-info/top_level.txt
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)       38 2024-04-30 10:53:36.855625 lianpwn-0.2.2/setup.cfg
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      756 2024-04-30 10:53:26.000000 lianpwn-0.2.2/setup.py
```

### Comparing `lianpwn-0.2.1/LICENSE` & `lianpwn-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lianpwn-0.2.1/lianpwn/__init__.py` & `lianpwn-0.2.2/lianpwn/__init__.py`

 * *Files identical despite different names*

### Comparing `lianpwn-0.2.1/lianpwn/nocli.py` & `lianpwn-0.2.2/lianpwn/nocli.py`

 * *Files identical despite different names*

### Comparing `lianpwn-0.2.1/lianpwn/template_gen.py` & `lianpwn-0.2.2/lianpwn/template_gen.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # template_gen.py
 import os
 from pwncli import *
-from lianpwn import lg_err, lg_suc
+from lianpwn import lg_err, lg_suc, lg_inf
 import subprocess
 
 
 def generate_template():
     if os.path.exists("exp.py"):
         lg_err("File 'exp.py' already exists.")
         subprocess.run(["mv", "exp.py", "exp.py.bak"])
```

### Comparing `lianpwn-0.2.1/setup.py` & `lianpwn-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="lianpwn",
-    version="0.2.1",
+    version="0.2.2",
     author="eastXueLian",
     author_email="eastxuelian@gmail.com",
     description="lianpwn based on pwncli",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://eastxuelian.nebuu.la/",
     packages=find_packages(),
```

