# Comparing `tmp/salure_helpers_salesforce-1.4.0.tar.gz` & `tmp/salure_helpers_salesforce-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_salesforce-1.4.0.tar", last modified: Fri Apr  5 07:07:13 2024, max compression
+gzip compressed data, was "dist/salure_helpers_salesforce-1.4.1.tar", last modified: Tue Apr 30 07:27:18 2024, max compression
```

## Comparing `salure_helpers_salesforce-1.4.0.tar` & `salure_helpers_salesforce-1.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/
--rw-r--r--   0 root         (0) root         (0)      274 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers/salesforce/
--rw-rw-rw-   0 root         (0) root         (0)       59 2024-04-05 07:06:55.000000 salure_helpers_salesforce-1.4.0/salure_helpers/salesforce/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15147 2024-04-05 07:06:55.000000 salure_helpers_salesforce-1.4.0/salure_helpers/salesforce/salesforce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/
--rw-r--r--   0 root         (0) root         (0)      274 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      378 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       78 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-04-05 07:06:55.000000 salure_helpers_salesforce-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:27:18.000000 salure_helpers_salesforce-1.4.1/
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-30 07:27:18.000000 salure_helpers_salesforce-1.4.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:27:18.000000 salure_helpers_salesforce-1.4.1/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:27:18.000000 salure_helpers_salesforce-1.4.1/salure_helpers/salesforce/
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-04-30 07:26:59.000000 salure_helpers_salesforce-1.4.1/salure_helpers/salesforce/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15147 2024-04-30 07:26:59.000000 salure_helpers_salesforce-1.4.1/salure_helpers/salesforce/salesforce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:27:18.000000 salure_helpers_salesforce-1.4.1/salure_helpers_salesforce.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-30 07:27:18.000000 salure_helpers_salesforce-1.4.1/salure_helpers_salesforce.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      378 2024-04-30 07:27:18.000000 salure_helpers_salesforce-1.4.1/salure_helpers_salesforce.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 07:27:18.000000 salure_helpers_salesforce-1.4.1/salure_helpers_salesforce.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 07:27:18.000000 salure_helpers_salesforce-1.4.1/salure_helpers_salesforce.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-30 07:27:18.000000 salure_helpers_salesforce-1.4.1/salure_helpers_salesforce.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-30 07:27:18.000000 salure_helpers_salesforce-1.4.1/salure_helpers_salesforce.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 07:27:18.000000 salure_helpers_salesforce-1.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-04-30 07:26:59.000000 salure_helpers_salesforce-1.4.1/setup.py
```

### Comparing `salure_helpers_salesforce-1.4.0/salure_helpers/salesforce/salesforce.py` & `salure_helpers_salesforce-1.4.1/salure_helpers/salesforce/salesforce.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_salesforce-1.4.0/setup.py` & `salure_helpers_salesforce-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_salesforce',
-    version='1.4.0',
+    version='1.4.1',
     description='Salesforce wrapper from Salure',
     long_description='Salesforce wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.salesforce"],
     license='Salure License',
     install_requires=[
         'salure-helpers-salureconnect>=1',
         'requests>=2,<=3',
         'pandas>=1,<3',
-        'pyarrow>=10,<=10'
+        'pyarrow>=10'
     ],
     zip_safe=False,
 )
```

