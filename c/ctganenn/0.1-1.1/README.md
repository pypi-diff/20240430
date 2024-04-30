# Comparing `tmp/ctganenn-0.1.tar.gz` & `tmp/ctganenn-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctganenn-0.1.tar", last modified: Tue Apr 30 10:21:03 2024, max compression
+gzip compressed data, was "ctganenn-1.1.tar", last modified: Tue Apr 30 10:53:27 2024, max compression
```

## Comparing `ctganenn-0.1.tar` & `ctganenn-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 10:21:03.645405 ctganenn-0.1/
--rw-rw-rw-   0        0        0      192 2024-04-30 10:21:03.645405 ctganenn-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-30 09:21:44.000000 ctganenn-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 10:21:03.631663 ctganenn-0.1/ctganenn/
--rw-rw-rw-   0        0        0       26 2024-04-30 09:09:12.000000 ctganenn-0.1/ctganenn/__init__.py
--rw-rw-rw-   0        0        0      732 2024-04-30 10:04:43.000000 ctganenn-0.1/ctganenn/main.py
-drwxrwxrwx   0        0        0        0 2024-04-30 10:21:03.645405 ctganenn-0.1/ctganenn.egg-info/
--rw-rw-rw-   0        0        0      192 2024-04-30 10:21:03.000000 ctganenn-0.1/ctganenn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-04-30 10:21:03.000000 ctganenn-0.1/ctganenn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 10:21:03.000000 ctganenn-0.1/ctganenn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-30 10:21:03.000000 ctganenn-0.1/ctganenn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-30 10:21:03.000000 ctganenn-0.1/ctganenn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 10:21:03.645405 ctganenn-0.1/setup.cfg
--rw-rw-rw-   0        0        0      558 2024-04-30 10:20:27.000000 ctganenn-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:53:27.841573 ctganenn-1.1/
+-rw-rw-rw-   0        0        0      192 2024-04-30 10:53:27.840573 ctganenn-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-30 09:21:44.000000 ctganenn-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 10:53:27.818620 ctganenn-1.1/ctganenn/
+-rw-rw-rw-   0        0        0       26 2024-04-30 10:51:54.000000 ctganenn-1.1/ctganenn/__init__.py
+-rw-rw-rw-   0        0        0      732 2024-04-30 10:04:43.000000 ctganenn-1.1/ctganenn/main.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:53:27.839578 ctganenn-1.1/ctganenn.egg-info/
+-rw-rw-rw-   0        0        0      192 2024-04-30 10:53:27.000000 ctganenn-1.1/ctganenn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-04-30 10:53:27.000000 ctganenn-1.1/ctganenn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 10:53:27.000000 ctganenn-1.1/ctganenn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-30 10:53:27.000000 ctganenn-1.1/ctganenn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 10:53:27.000000 ctganenn-1.1/ctganenn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 10:53:27.841573 ctganenn-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      558 2024-04-30 10:52:17.000000 ctganenn-1.1/setup.py
```

### Comparing `ctganenn-0.1/ctganenn/main.py` & `ctganenn-1.1/ctganenn/main.py`

 * *Files identical despite different names*

### Comparing `ctganenn-0.1/setup.py` & `ctganenn-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='ctganenn',
-    version='0.1',
+    version='1.1',
     packages=find_packages(),
     install_requires=[
         'scikit-learn==1.2.2',
         'ctgan==0.9.1',
         'sdv==1.11.0',
         'pandas==2.0.3',
         # Add any dependencies your package needs
```

