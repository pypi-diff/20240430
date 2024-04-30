# Comparing `tmp/assertai_alpha_deployer-4.5.tar.gz` & `tmp/assertai_alpha_deployer-4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assertai_alpha_deployer-4.5.tar", last modified: Tue Apr 30 20:52:23 2024, max compression
+gzip compressed data, was "assertai_alpha_deployer-4.6.tar", last modified: Tue Apr 30 20:54:39 2024, max compression
```

## Comparing `assertai_alpha_deployer-4.5.tar` & `assertai_alpha_deployer-4.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:52:23.722282 assertai_alpha_deployer-4.5/
--rw-rw-r--   0 devl      (1000) devl      (1000)       85 2024-04-30 20:51:30.000000 assertai_alpha_deployer-4.5/MANIFEST.in
--rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:52:23.722282 assertai_alpha_deployer-4.5/PKG-INFO
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:52:23.722282 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/
--rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:52:23.000000 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/PKG-INFO
--rw-rw-r--   0 devl      (1000) devl      (1000)      304 2024-04-30 20:52:23.000000 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/SOURCES.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)        1 2024-04-30 20:52:23.000000 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/dependency_links.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       82 2024-04-30 20:52:23.000000 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/entry_points.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)        7 2024-04-30 20:52:23.000000 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/requires.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       24 2024-04-30 20:52:23.000000 assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/top_level.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       38 2024-04-30 20:52:23.722282 assertai_alpha_deployer-4.5/setup.cfg
--rw-rw-r--   0 devl      (1000) devl      (1000)     1040 2024-04-30 20:51:58.000000 assertai_alpha_deployer-4.5/setup.py
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:54:39.670926 assertai_alpha_deployer-4.6/
+-rw-rw-r--   0 devl      (1000) devl      (1000)       85 2024-04-30 20:51:30.000000 assertai_alpha_deployer-4.6/MANIFEST.in
+-rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:54:39.670926 assertai_alpha_deployer-4.6/PKG-INFO
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:54:39.670926 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/
+-rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:54:39.000000 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/PKG-INFO
+-rw-rw-r--   0 devl      (1000) devl      (1000)      304 2024-04-30 20:54:39.000000 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/SOURCES.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)        1 2024-04-30 20:54:39.000000 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/dependency_links.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       82 2024-04-30 20:54:39.000000 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/entry_points.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)        7 2024-04-30 20:54:39.000000 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/requires.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       24 2024-04-30 20:54:39.000000 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/top_level.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       38 2024-04-30 20:54:39.670926 assertai_alpha_deployer-4.6/setup.cfg
+-rw-rw-r--   0 devl      (1000) devl      (1000)     1117 2024-04-30 20:54:20.000000 assertai_alpha_deployer-4.6/setup.py
```

### Comparing `assertai_alpha_deployer-4.5/PKG-INFO` & `assertai_alpha_deployer-4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assertai_alpha_deployer
-Version: 4.5
+Version: 4.6
 Summary: A package to deploy python codes on bare-metal
 Home-page: https://www.linkedin.com/in/rajeshroy402
 Author: Rajesh Roy
 Author-email: rajeshroy402@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assertai_alpha_deployer-4.5/assertai_alpha_deployer.egg-info/PKG-INFO` & `assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assertai_alpha_deployer
-Version: 4.5
+Version: 4.6
 Summary: A package to deploy python codes on bare-metal
 Home-page: https://www.linkedin.com/in/rajeshroy402
 Author: Rajesh Roy
 Author-email: rajeshroy402@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assertai_alpha_deployer-4.5/setup.py` & `assertai_alpha_deployer-4.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='assertai_alpha_deployer',
-    version='4.5',
+    version='4.6',
     packages=find_packages(),
+    package_data={
+        'assertai_alpha_deployer': ['*', '!*.py'],
+    },
     install_requires=[
         'psutil',
     ],
     entry_points={
         'console_scripts': [
             'assertai-alpha-deployer=assertai_alpha_deployer.__main__:main',
         ],
```

