# Comparing `tmp/assertai_alpha_deployer-2.0.tar.gz` & `tmp/assertai_alpha_deployer-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assertai_alpha_deployer-2.0.tar", last modified: Tue Apr 30 19:59:06 2024, max compression
+gzip compressed data, was "assertai_alpha_deployer-3.0.tar", last modified: Tue Apr 30 20:04:15 2024, max compression
```

## Comparing `assertai_alpha_deployer-2.0.tar` & `assertai_alpha_deployer-3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 19:59:06.435482 assertai_alpha_deployer-2.0/
--rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 19:59:06.435482 assertai_alpha_deployer-2.0/PKG-INFO
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 19:59:06.435482 assertai_alpha_deployer-2.0/assertai_alpha_deployer/
--rw-rw-r--   0 devl      (1000) devl      (1000)        0 2024-04-30 08:56:14.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer/__init__.py
--rw-rw-r--   0 devl      (1000) devl      (1000)       72 2024-04-30 19:45:43.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer/__main__.py
--rw-rw-r--   0 devl      (1000) devl      (1000)     6486 2024-04-29 12:53:32.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer/script_manager.py
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 19:59:06.435482 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/
--rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 19:59:06.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/PKG-INFO
--rw-rw-r--   0 devl      (1000) devl      (1000)      406 2024-04-30 19:59:06.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/SOURCES.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)        1 2024-04-30 19:59:06.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/dependency_links.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       82 2024-04-30 19:59:06.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/entry_points.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)        7 2024-04-30 19:59:06.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/requires.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       24 2024-04-30 19:59:06.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/top_level.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       38 2024-04-30 19:59:06.435482 assertai_alpha_deployer-2.0/setup.cfg
--rw-rw-r--   0 devl      (1000) devl      (1000)     1037 2024-04-30 19:58:40.000000 assertai_alpha_deployer-2.0/setup.py
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:04:15.783115 assertai_alpha_deployer-3.0/
+-rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:04:15.783115 assertai_alpha_deployer-3.0/PKG-INFO
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:04:15.783115 assertai_alpha_deployer-3.0/assertai_alpha_deployer/
+-rw-rw-r--   0 devl      (1000) devl      (1000)        0 2024-04-30 08:56:14.000000 assertai_alpha_deployer-3.0/assertai_alpha_deployer/__init__.py
+-rw-rw-r--   0 devl      (1000) devl      (1000)       72 2024-04-30 19:45:43.000000 assertai_alpha_deployer-3.0/assertai_alpha_deployer/__main__.py
+-rw-rw-r--   0 devl      (1000) devl      (1000)     6486 2024-04-29 12:53:32.000000 assertai_alpha_deployer-3.0/assertai_alpha_deployer/script_manager.py
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:04:15.783115 assertai_alpha_deployer-3.0/assertai_alpha_deployer.egg-info/
+-rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:04:15.000000 assertai_alpha_deployer-3.0/assertai_alpha_deployer.egg-info/PKG-INFO
+-rw-rw-r--   0 devl      (1000) devl      (1000)      406 2024-04-30 20:04:15.000000 assertai_alpha_deployer-3.0/assertai_alpha_deployer.egg-info/SOURCES.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)        1 2024-04-30 20:04:15.000000 assertai_alpha_deployer-3.0/assertai_alpha_deployer.egg-info/dependency_links.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       82 2024-04-30 20:04:15.000000 assertai_alpha_deployer-3.0/assertai_alpha_deployer.egg-info/entry_points.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)        7 2024-04-30 20:04:15.000000 assertai_alpha_deployer-3.0/assertai_alpha_deployer.egg-info/requires.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       24 2024-04-30 20:04:15.000000 assertai_alpha_deployer-3.0/assertai_alpha_deployer.egg-info/top_level.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       38 2024-04-30 20:04:15.783115 assertai_alpha_deployer-3.0/setup.cfg
+-rw-rw-r--   0 devl      (1000) devl      (1000)     1037 2024-04-30 20:03:40.000000 assertai_alpha_deployer-3.0/setup.py
```

### Comparing `assertai_alpha_deployer-2.0/PKG-INFO` & `assertai_alpha_deployer-3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assertai_alpha_deployer
-Version: 2.0
+Version: 3.0
 Summary: A package to deploy python codes on bare-metal
 Home-page: https://www.linkedin.com/in/rajeshroy402
 Author: Rajesh Roy
 Author-email: rajeshroy402@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assertai_alpha_deployer-2.0/assertai_alpha_deployer/script_manager.py` & `assertai_alpha_deployer-3.0/assertai_alpha_deployer/script_manager.py`

 * *Files identical despite different names*

### Comparing `assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/PKG-INFO` & `assertai_alpha_deployer-3.0/assertai_alpha_deployer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assertai_alpha_deployer
-Version: 2.0
+Version: 3.0
 Summary: A package to deploy python codes on bare-metal
 Home-page: https://www.linkedin.com/in/rajeshroy402
 Author: Rajesh Roy
 Author-email: rajeshroy402@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assertai_alpha_deployer-2.0/setup.py` & `assertai_alpha_deployer-3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='assertai_alpha_deployer',
-    version='2.0',
+    version='3.0',
     packages=['assertai_alpha_deployer'],
     install_requires=[
         'psutil',
     ],
     entry_points={
         'console_scripts': [
             'assertai-alpha-deployer=assertai_alpha_deployer.__main__:main',
```

