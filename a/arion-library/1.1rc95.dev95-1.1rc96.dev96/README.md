# Comparing `tmp/arion_library-1.1rc95.dev95.tar.gz` & `tmp/arion_library-1.1rc96.dev96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc95.dev95.tar", last modified: Tue Apr 30 14:44:51 2024, max compression
+gzip compressed data, was "arion_library-1.1rc96.dev96.tar", last modified: Tue Apr 30 15:25:56 2024, max compression
```

## Comparing `arion_library-1.1rc95.dev95.tar` & `arion_library-1.1rc96.dev96.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:44:51.556731 arion_library-1.1rc95.dev95/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-30 14:44:51.556731 arion_library-1.1rc95.dev95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:44:02.000000 arion_library-1.1rc95.dev95/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:44:51.556731 arion_library-1.1rc95.dev95/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-30 14:44:51.000000 arion_library-1.1rc95.dev95/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-30 14:44:51.000000 arion_library-1.1rc95.dev95/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:44:51.000000 arion_library-1.1rc95.dev95/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-30 14:44:51.000000 arion_library-1.1rc95.dev95/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:44:51.000000 arion_library-1.1rc95.dev95/arion_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:44:51.556731 arion_library-1.1rc95.dev95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-30 14:44:50.000000 arion_library-1.1rc95.dev95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:25:56.399384 arion_library-1.1rc96.dev96/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-30 15:25:56.399384 arion_library-1.1rc96.dev96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:24:56.000000 arion_library-1.1rc96.dev96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:25:56.399384 arion_library-1.1rc96.dev96/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-30 15:25:56.000000 arion_library-1.1rc96.dev96/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-30 15:25:56.000000 arion_library-1.1rc96.dev96/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:25:56.000000 arion_library-1.1rc96.dev96/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-30 15:25:56.000000 arion_library-1.1rc96.dev96/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:25:56.000000 arion_library-1.1rc96.dev96/arion_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:25:56.399384 arion_library-1.1rc96.dev96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-30 15:25:54.000000 arion_library-1.1rc96.dev96/setup.py
```

### Comparing `arion_library-1.1rc95.dev95/setup.py` & `arion_library-1.1rc96.dev96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='arion_library',
-    version='1.1rc95.dev95',  
+    version='1.1rc96.dev96',  
     author='Heni Nechi',  
     author_email='h.nechi@arion-tech.com',  
     url='https://github.com/Ariontech/ArionLibrary.git',  
     packages=find_packages(include=['arion.*']),  
     python_requires='>=3.8',  
     install_requires=['pyodbc', 'pytest', 'pysftp==0.2.9', 'ShopifyAPI==12.5.0', 'requests==2.31.0', 'azure-core==1.29.6', 'azure-data-tables==12.5.0', 'azure-storage-blob==12.19.1', 'python-dotenv==1.0.1', 'pytest==8.1.1', 'pandas==2.0.3', 'pytest'],
 )
```

