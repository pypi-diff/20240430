# Comparing `tmp/csulb_mock_dataset-0.1.10.tar.gz` & `tmp/csulb_mock_dataset-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csulb_mock_dataset-0.1.10.tar", last modified: Mon Apr 29 22:06:39 2024, max compression
+gzip compressed data, was "csulb_mock_dataset-0.1.11.tar", last modified: Mon Apr 29 22:15:05 2024, max compression
```

## Comparing `csulb_mock_dataset-0.1.10.tar` & `csulb_mock_dataset-0.1.11.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 guru       (501) staff       (20)        0 2024-04-29 22:06:39.092753 csulb_mock_dataset-0.1.10/
--rw-r--r--   0 guru       (501) staff       (20)      262 2024-04-29 22:06:39.092654 csulb_mock_dataset-0.1.10/PKG-INFO
--rw-r--r--   0 guru       (501) staff       (20)       16 2024-04-29 20:09:04.000000 csulb_mock_dataset-0.1.10/README.md
-drwxr-xr-x   0 guru       (501) staff       (20)        0 2024-04-29 22:06:39.091768 csulb_mock_dataset-0.1.10/csulb_mock_dataset/
--rw-r--r--   0 guru       (501) staff       (20)       28 2024-04-29 21:16:45.000000 csulb_mock_dataset-0.1.10/csulb_mock_dataset/__init__.py
--rw-r--r--   0 guru       (501) staff       (20)      325 2024-04-29 22:03:38.000000 csulb_mock_dataset-0.1.10/csulb_mock_dataset/data.py
-drwxr-xr-x   0 guru       (501) staff       (20)        0 2024-04-29 22:06:39.092505 csulb_mock_dataset-0.1.10/csulb_mock_dataset.egg-info/
--rw-r--r--   0 guru       (501) staff       (20)      262 2024-04-29 22:06:39.000000 csulb_mock_dataset-0.1.10/csulb_mock_dataset.egg-info/PKG-INFO
--rw-r--r--   0 guru       (501) staff       (20)      285 2024-04-29 22:06:39.000000 csulb_mock_dataset-0.1.10/csulb_mock_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 guru       (501) staff       (20)        1 2024-04-29 22:06:39.000000 csulb_mock_dataset-0.1.10/csulb_mock_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 guru       (501) staff       (20)        7 2024-04-29 22:06:39.000000 csulb_mock_dataset-0.1.10/csulb_mock_dataset.egg-info/requires.txt
--rw-r--r--   0 guru       (501) staff       (20)       19 2024-04-29 22:06:39.000000 csulb_mock_dataset-0.1.10/csulb_mock_dataset.egg-info/top_level.txt
--rw-r--r--   0 guru       (501) staff       (20)       38 2024-04-29 22:06:39.092790 csulb_mock_dataset-0.1.10/setup.cfg
--rw-r--r--   0 guru       (501) staff       (20)      588 2024-04-29 22:06:02.000000 csulb_mock_dataset-0.1.10/setup.py
+drwxr-xr-x   0 guru       (501) staff       (20)        0 2024-04-29 22:15:05.570073 csulb_mock_dataset-0.1.11/
+-rw-r--r--   0 guru       (501) staff       (20)      262 2024-04-29 22:15:05.569943 csulb_mock_dataset-0.1.11/PKG-INFO
+-rw-r--r--   0 guru       (501) staff       (20)       16 2024-04-29 20:09:04.000000 csulb_mock_dataset-0.1.11/README.md
+drwxr-xr-x   0 guru       (501) staff       (20)        0 2024-04-29 22:15:05.569081 csulb_mock_dataset-0.1.11/csulb_mock_dataset/
+-rw-r--r--   0 guru       (501) staff       (20)       28 2024-04-29 21:16:45.000000 csulb_mock_dataset-0.1.11/csulb_mock_dataset/__init__.py
+-rw-r--r--   0 guru       (501) staff       (20)  3335723 2024-04-29 20:04:18.000000 csulb_mock_dataset-0.1.11/csulb_mock_dataset/cmp1.csv
+-rw-r--r--   0 guru       (501) staff       (20)      317 2024-04-29 22:13:10.000000 csulb_mock_dataset-0.1.11/csulb_mock_dataset/data.py
+drwxr-xr-x   0 guru       (501) staff       (20)        0 2024-04-29 22:15:05.569794 csulb_mock_dataset-0.1.11/csulb_mock_dataset.egg-info/
+-rw-r--r--   0 guru       (501) staff       (20)      262 2024-04-29 22:15:05.000000 csulb_mock_dataset-0.1.11/csulb_mock_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 guru       (501) staff       (20)      313 2024-04-29 22:15:05.000000 csulb_mock_dataset-0.1.11/csulb_mock_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 guru       (501) staff       (20)        1 2024-04-29 22:15:05.000000 csulb_mock_dataset-0.1.11/csulb_mock_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 guru       (501) staff       (20)        7 2024-04-29 22:15:05.000000 csulb_mock_dataset-0.1.11/csulb_mock_dataset.egg-info/requires.txt
+-rw-r--r--   0 guru       (501) staff       (20)       19 2024-04-29 22:15:05.000000 csulb_mock_dataset-0.1.11/csulb_mock_dataset.egg-info/top_level.txt
+-rw-r--r--   0 guru       (501) staff       (20)       38 2024-04-29 22:15:05.570140 csulb_mock_dataset-0.1.11/setup.cfg
+-rw-r--r--   0 guru       (501) staff       (20)      583 2024-04-29 22:15:00.000000 csulb_mock_dataset-0.1.11/setup.py
```

### Comparing `csulb_mock_dataset-0.1.10/setup.py` & `csulb_mock_dataset-0.1.11/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='csulb_mock_dataset',
-    version='0.1.10',
+    version='0.1.11',
     packages=find_packages(),
     include_package_data=True,
-    package_data={'csulb_mock_dataset': ['data/*.csv']},
+    package_data={'csulb_mock_dataset': ['*.csv']},
     install_requires=[
         'pandas',  # Ensure pandas is installed with your package
     ],
     author='Gurucharan Raju',
     author_email='Gurucharan.Raju-SA@csulb.edu@csulb.edu',
     description='A simple package containing a CSV dataset',
     long_description=open('README.md').read(),
```

