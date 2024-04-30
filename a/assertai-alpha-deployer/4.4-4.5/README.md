# Comparing `tmp/assertai_alpha_deployer-4.4.tar.gz` & `tmp/assertai_alpha_deployer-4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assertai_alpha_deployer-4.4.tar", last modified: Tue Apr 30 20:49:18 2024, max compression
+gzip compressed data, was "assertai_alpha_deployer-4.5.tar", last modified: Tue Apr 30 20:52:23 2024, max compression
```

## Comparing `assertai_alpha_deployer-4.4.tar` & `assertai_alpha_deployer-4.5.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:49:18.124056 assertai_alpha_deployer-4.4/
--rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:49:18.124056 assertai_alpha_deployer-4.4/PKG-INFO
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:49:18.120056 assertai_alpha_deployer-4.4/assertai_alpha_deployer/
--rw-rw-r--   0 devl      (1000) devl      (1000)        0 2024-04-30 08:56:14.000000 assertai_alpha_deployer-4.4/assertai_alpha_deployer/__init__.py
--rw-rw-r--   0 devl      (1000) devl      (1000)       72 2024-04-30 19:45:43.000000 assertai_alpha_deployer-4.4/assertai_alpha_deployer/__main__.py
--rw-rw-r--   0 devl      (1000) devl      (1000)     6486 2024-04-30 20:40:18.000000 assertai_alpha_deployer-4.4/assertai_alpha_deployer/script_manager.py
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:49:18.124056 assertai_alpha_deployer-4.4/assertai_alpha_deployer.egg-info/
--rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:49:18.000000 assertai_alpha_deployer-4.4/assertai_alpha_deployer.egg-info/PKG-INFO
--rw-rw-r--   0 devl      (1000) devl      (1000)      406 2024-04-30 20:49:18.000000 assertai_alpha_deployer-4.4/assertai_alpha_deployer.egg-info/SOURCES.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)        1 2024-04-30 20:49:18.000000 assertai_alpha_deployer-4.4/assertai_alpha_deployer.egg-info/dependency_links.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       82 2024-04-30 20:49:18.000000 assertai_alpha_deployer-4.4/assertai_alpha_deployer.egg-info/entry_points.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)        7 2024-04-30 20:49:18.000000 assertai_alpha_deployer-4.4/assertai_alpha_deployer.egg-info/requires.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       24 2024-04-30 20:49:18.000000 assertai_alpha_deployer-4.4/assertai_alpha_deployer.egg-info/top_level.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       38 2024-04-30 20:49:18.124056 assertai_alpha_deployer-4.4/setup.cfg
--rw-rw-r--   0 devl      (1000) devl      (1000)     1147 2024-04-30 20:48:57.000000 assertai_alpha_deployer-4.4/setup.py
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:52:23.722282 assertai_alpha_deployer-4.5/
+-rw-rw-r--   0 devl      (1000) devl      (1000)       85 2024-04-30 20:51:30.000000 assertai_alpha_deployer-4.5/MANIFEST.in
+-rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:52:23.722282 assertai_alpha_deployer-4.5/PKG-INFO
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:52:23.722282 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/
+-rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:52:23.000000 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/PKG-INFO
+-rw-rw-r--   0 devl      (1000) devl      (1000)      304 2024-04-30 20:52:23.000000 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/SOURCES.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)        1 2024-04-30 20:52:23.000000 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/dependency_links.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       82 2024-04-30 20:52:23.000000 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/entry_points.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)        7 2024-04-30 20:52:23.000000 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/requires.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       24 2024-04-30 20:52:23.000000 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/top_level.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       38 2024-04-30 20:52:23.722282 assertai_alpha_deployer-4.5/setup.cfg
+-rw-rw-r--   0 devl      (1000) devl      (1000)     1040 2024-04-30 20:51:58.000000 assertai_alpha_deployer-4.5/setup.py
```

### Comparing `assertai_alpha_deployer-4.4/PKG-INFO` & `assertai_alpha_deployer-4.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assertai_alpha_deployer
-Version: 4.4
+Version: 4.5
 Summary: A package to deploy python codes on bare-metal
 Home-page: https://www.linkedin.com/in/rajeshroy402
 Author: Rajesh Roy
 Author-email: rajeshroy402@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assertai_alpha_deployer-4.4/assertai_alpha_deployer.egg-info/PKG-INFO` & `assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assertai_alpha_deployer
-Version: 4.4
+Version: 4.5
 Summary: A package to deploy python codes on bare-metal
 Home-page: https://www.linkedin.com/in/rajeshroy402
 Author: Rajesh Roy
 Author-email: rajeshroy402@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assertai_alpha_deployer-4.4/setup.py` & `assertai_alpha_deployer-4.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='assertai_alpha_deployer',
-    version='4.4',
-    packages=find_packages(exclude=['assertai_alpha_deployer.script_manager']),
-    package_data={'assertai_alpha_deployer': ['*.pyc']},
+    version='4.5',
+    packages=find_packages(),
     install_requires=[
         'psutil',
     ],
     entry_points={
         'console_scripts': [
             'assertai-alpha-deployer=assertai_alpha_deployer.__main__:main',
         ],
```

