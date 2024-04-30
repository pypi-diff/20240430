# Comparing `tmp/assertai_alpha_deployer-4.2.tar.gz` & `tmp/assertai_alpha_deployer-4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assertai_alpha_deployer-4.2.tar", last modified: Tue Apr 30 20:34:28 2024, max compression
+gzip compressed data, was "assertai_alpha_deployer-4.3.tar", last modified: Tue Apr 30 20:46:24 2024, max compression
```

## Comparing `assertai_alpha_deployer-4.2.tar` & `assertai_alpha_deployer-4.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:34:28.510695 assertai_alpha_deployer-4.2/
--rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:34:28.510695 assertai_alpha_deployer-4.2/PKG-INFO
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:34:28.510695 assertai_alpha_deployer-4.2/assertai_alpha_deployer/
--rw-rw-r--   0 devl      (1000) devl      (1000)        0 2024-04-30 08:56:14.000000 assertai_alpha_deployer-4.2/assertai_alpha_deployer/__init__.py
--rw-rw-r--   0 devl      (1000) devl      (1000)       72 2024-04-30 19:45:43.000000 assertai_alpha_deployer-4.2/assertai_alpha_deployer/__main__.py
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:34:28.510695 assertai_alpha_deployer-4.2/assertai_alpha_deployer.egg-info/
--rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:34:28.000000 assertai_alpha_deployer-4.2/assertai_alpha_deployer.egg-info/PKG-INFO
--rw-rw-r--   0 devl      (1000) devl      (1000)      364 2024-04-30 20:34:28.000000 assertai_alpha_deployer-4.2/assertai_alpha_deployer.egg-info/SOURCES.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)        1 2024-04-30 20:34:28.000000 assertai_alpha_deployer-4.2/assertai_alpha_deployer.egg-info/dependency_links.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       82 2024-04-30 20:34:28.000000 assertai_alpha_deployer-4.2/assertai_alpha_deployer.egg-info/entry_points.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)        7 2024-04-30 20:34:28.000000 assertai_alpha_deployer-4.2/assertai_alpha_deployer.egg-info/requires.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       24 2024-04-30 20:34:28.000000 assertai_alpha_deployer-4.2/assertai_alpha_deployer.egg-info/top_level.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       38 2024-04-30 20:34:28.510695 assertai_alpha_deployer-4.2/setup.cfg
--rw-rw-r--   0 devl      (1000) devl      (1000)     1138 2024-04-30 20:32:41.000000 assertai_alpha_deployer-4.2/setup.py
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:46:24.582401 assertai_alpha_deployer-4.3/
+-rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:46:24.578400 assertai_alpha_deployer-4.3/PKG-INFO
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:46:24.578400 assertai_alpha_deployer-4.3/assertai_alpha_deployer/
+-rw-rw-r--   0 devl      (1000) devl      (1000)        0 2024-04-30 08:56:14.000000 assertai_alpha_deployer-4.3/assertai_alpha_deployer/__init__.py
+-rw-rw-r--   0 devl      (1000) devl      (1000)       72 2024-04-30 19:45:43.000000 assertai_alpha_deployer-4.3/assertai_alpha_deployer/__main__.py
+-rw-rw-r--   0 devl      (1000) devl      (1000)     6486 2024-04-30 20:40:18.000000 assertai_alpha_deployer-4.3/assertai_alpha_deployer/script_manager.py
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:46:24.578400 assertai_alpha_deployer-4.3/assertai_alpha_deployer.egg-info/
+-rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:46:24.000000 assertai_alpha_deployer-4.3/assertai_alpha_deployer.egg-info/PKG-INFO
+-rw-rw-r--   0 devl      (1000) devl      (1000)      406 2024-04-30 20:46:24.000000 assertai_alpha_deployer-4.3/assertai_alpha_deployer.egg-info/SOURCES.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)        1 2024-04-30 20:46:24.000000 assertai_alpha_deployer-4.3/assertai_alpha_deployer.egg-info/dependency_links.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       82 2024-04-30 20:46:24.000000 assertai_alpha_deployer-4.3/assertai_alpha_deployer.egg-info/entry_points.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)        7 2024-04-30 20:46:24.000000 assertai_alpha_deployer-4.3/assertai_alpha_deployer.egg-info/requires.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       24 2024-04-30 20:46:24.000000 assertai_alpha_deployer-4.3/assertai_alpha_deployer.egg-info/top_level.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       38 2024-04-30 20:46:24.582401 assertai_alpha_deployer-4.3/setup.cfg
+-rw-rw-r--   0 devl      (1000) devl      (1000)     1135 2024-04-30 20:44:14.000000 assertai_alpha_deployer-4.3/setup.py
```

### Comparing `assertai_alpha_deployer-4.2/PKG-INFO` & `assertai_alpha_deployer-4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assertai_alpha_deployer
-Version: 4.2
+Version: 4.3
 Summary: A package to deploy python codes on bare-metal
 Home-page: https://www.linkedin.com/in/rajeshroy402
 Author: Rajesh Roy
 Author-email: rajeshroy402@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assertai_alpha_deployer-4.2/assertai_alpha_deployer.egg-info/PKG-INFO` & `assertai_alpha_deployer-4.3/assertai_alpha_deployer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assertai_alpha_deployer
-Version: 4.2
+Version: 4.3
 Summary: A package to deploy python codes on bare-metal
 Home-page: https://www.linkedin.com/in/rajeshroy402
 Author: Rajesh Roy
 Author-email: rajeshroy402@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assertai_alpha_deployer-4.2/setup.py` & `assertai_alpha_deployer-4.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 setup(
     name='assertai_alpha_deployer',
-    version='4.2',
-    packages=find_packages(),
+    version='4.3',
+    packages=['assertai_alpha_deployer'],
     package_data={'assertai_alpha_deployer': ['*.pyc']},
     exclude_package_data={'': ['*.py']},
     install_requires=[
         'psutil',
     ],
     entry_points={
         'console_scripts': [
```

