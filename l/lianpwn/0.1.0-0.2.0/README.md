# Comparing `tmp/lianpwn-0.1.0.tar.gz` & `tmp/lianpwn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lianpwn-0.1.0.tar", last modified: Mon Apr 29 13:11:22 2024, max compression
+gzip compressed data, was "lianpwn-0.2.0.tar", last modified: Tue Apr 30 10:48:59 2024, max compression
```

## Comparing `lianpwn-0.1.0.tar` & `lianpwn-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxr-x   0 eastxuelian  (1000) eastxuelian  (1000)        0 2024-04-29 13:11:22.576766 lianpwn-0.1.0/
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)     2400 2024-04-29 13:07:59.000000 lianpwn-0.1.0/LICENSE
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      400 2024-04-29 13:11:22.576766 lianpwn-0.1.0/PKG-INFO
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)       10 2024-04-29 13:07:59.000000 lianpwn-0.1.0/README.md
-drwxrwxr-x   0 eastxuelian  (1000) eastxuelian  (1000)        0 2024-04-29 13:11:22.572766 lianpwn-0.1.0/lianpwn/
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)     2873 2024-04-29 13:07:59.000000 lianpwn-0.1.0/lianpwn/__init__.py
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      754 2024-04-29 13:07:59.000000 lianpwn-0.1.0/lianpwn/nocli.py
-drwxrwxr-x   0 eastxuelian  (1000) eastxuelian  (1000)        0 2024-04-29 13:11:22.576766 lianpwn-0.1.0/lianpwn.egg-info/
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      400 2024-04-29 13:11:22.000000 lianpwn-0.1.0/lianpwn.egg-info/PKG-INFO
--rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)      187 2024-04-29 13:11:22.000000 lianpwn-0.1.0/lianpwn.egg-info/SOURCES.txt
--rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)        1 2024-04-29 13:11:22.000000 lianpwn-0.1.0/lianpwn.egg-info/dependency_links.txt
--rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)        8 2024-04-29 13:11:22.000000 lianpwn-0.1.0/lianpwn.egg-info/top_level.txt
--rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)       38 2024-04-29 13:11:22.576766 lianpwn-0.1.0/setup.cfg
--rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      629 2024-04-29 13:10:05.000000 lianpwn-0.1.0/setup.py
+drwxrwxr-x   0 eastxuelian  (1000) eastxuelian  (1000)        0 2024-04-30 10:48:59.839923 lianpwn-0.2.0/
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)     2400 2024-04-29 13:07:59.000000 lianpwn-0.2.0/LICENSE
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)      400 2024-04-30 10:48:59.839923 lianpwn-0.2.0/PKG-INFO
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)       10 2024-04-29 13:07:59.000000 lianpwn-0.2.0/README.md
+drwxrwxr-x   0 eastxuelian  (1000) eastxuelian  (1000)        0 2024-04-30 10:48:59.839923 lianpwn-0.2.0/lianpwn/
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)     2873 2024-04-29 13:07:59.000000 lianpwn-0.2.0/lianpwn/__init__.py
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      241 2024-04-30 10:45:08.000000 lianpwn-0.2.0/lianpwn/cli.py
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      754 2024-04-29 13:07:59.000000 lianpwn-0.2.0/lianpwn/nocli.py
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)      751 2024-04-30 10:41:05.000000 lianpwn-0.2.0/lianpwn/template_gen.py
+drwxrwxr-x   0 eastxuelian  (1000) eastxuelian  (1000)        0 2024-04-30 10:48:59.839923 lianpwn-0.2.0/lianpwn.egg-info/
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      400 2024-04-30 10:48:59.000000 lianpwn-0.2.0/lianpwn.egg-info/PKG-INFO
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)      290 2024-04-30 10:48:59.000000 lianpwn-0.2.0/lianpwn.egg-info/SOURCES.txt
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)        1 2024-04-30 10:48:59.000000 lianpwn-0.2.0/lianpwn.egg-info/dependency_links.txt
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)       44 2024-04-30 10:48:59.000000 lianpwn-0.2.0/lianpwn.egg-info/entry_points.txt
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)       22 2024-04-30 10:48:59.000000 lianpwn-0.2.0/lianpwn.egg-info/requires.txt
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)        8 2024-04-30 10:48:59.000000 lianpwn-0.2.0/lianpwn.egg-info/top_level.txt
+-rw-rw-r--   0 eastxuelian  (1000) eastxuelian  (1000)       38 2024-04-30 10:48:59.839923 lianpwn-0.2.0/setup.cfg
+-rw-r--r--   0 eastxuelian  (1000) eastxuelian  (1000)      756 2024-04-30 10:48:18.000000 lianpwn-0.2.0/setup.py
```

### Comparing `lianpwn-0.1.0/LICENSE` & `lianpwn-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lianpwn-0.1.0/lianpwn/__init__.py` & `lianpwn-0.2.0/lianpwn/__init__.py`

 * *Files identical despite different names*

### Comparing `lianpwn-0.1.0/lianpwn/nocli.py` & `lianpwn-0.2.0/lianpwn/nocli.py`

 * *Files identical despite different names*

### Comparing `lianpwn-0.1.0/setup.py` & `lianpwn-0.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="lianpwn",
-    version="0.1.0",
+    version="0.2.0",
     author="eastXueLian",
     author_email="eastxuelian@gmail.com",
     description="lianpwn based on pwncli",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://eastxuelian.nebuu.la/",
     packages=find_packages(),
+    include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=[],
+    install_requires=["click", "pwntools", "pwncli"],
+    entry_points={"console_scripts": ["lianpwn=lianpwn.cli:cli"]},
 )
```

