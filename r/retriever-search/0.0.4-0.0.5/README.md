# Comparing `tmp/retriever_search-0.0.4.tar.gz` & `tmp/retriever_search-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retriever_search-0.0.4.tar", last modified: Wed Apr 24 08:58:45 2024, max compression
+gzip compressed data, was "retriever_search-0.0.5.tar", last modified: Wed Apr 24 13:25:44 2024, max compression
```

## Comparing `retriever_search-0.0.4.tar` & `retriever_search-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 08:58:45.012519 retriever_search-0.0.4/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.0.4/LICENSE
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      549 2024-04-24 08:58:45.012148 retriever_search-0.0.4/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      409 2024-04-24 08:54:46.000000 retriever_search-0.0.4/README.md
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 08:58:45.011700 retriever_search-0.0.4/retriever_search.egg-info/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      549 2024-04-24 08:58:44.000000 retriever_search-0.0.4/retriever_search.egg-info/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      225 2024-04-24 08:58:44.000000 retriever_search-0.0.4/retriever_search.egg-info/SOURCES.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-24 08:58:44.000000 retriever_search-0.0.4/retriever_search.egg-info/dependency_links.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      191 2024-04-24 08:58:44.000000 retriever_search-0.0.4/retriever_search.egg-info/requires.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-04-24 08:58:44.000000 retriever_search-0.0.4/retriever_search.egg-info/top_level.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-04-24 08:58:45.012602 retriever_search-0.0.4/setup.cfg
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      641 2024-04-24 08:32:32.000000 retriever_search-0.0.4/setup.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 13:25:44.176538 retriever_search-0.0.5/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.0.5/LICENSE
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1000 2024-04-24 13:25:44.176150 retriever_search-0.0.5/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      409 2024-04-24 08:54:46.000000 retriever_search-0.0.5/README.md
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 13:25:44.175638 retriever_search-0.0.5/retriever_search.egg-info/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1000 2024-04-24 13:25:44.000000 retriever_search-0.0.5/retriever_search.egg-info/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      225 2024-04-24 13:25:44.000000 retriever_search-0.0.5/retriever_search.egg-info/SOURCES.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-24 13:25:44.000000 retriever_search-0.0.5/retriever_search.egg-info/dependency_links.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      191 2024-04-24 13:25:44.000000 retriever_search-0.0.5/retriever_search.egg-info/requires.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-04-24 13:25:44.000000 retriever_search-0.0.5/retriever_search.egg-info/top_level.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-04-24 13:25:44.176622 retriever_search-0.0.5/setup.cfg
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      739 2024-04-24 13:25:17.000000 retriever_search-0.0.5/setup.py
```

### Comparing `retriever_search-0.0.4/LICENSE` & `retriever_search-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.4/setup.py` & `retriever_search-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 setup(
     name='retriever_search',
     version=__version__,
 
     url='https://github.com/GovML/retriever.git',
     author='Sidharth Kathpal',
     author_email='kathpal.sid@gmail.com',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     
     py_modules=['retriever_search'],
     install_requires=[
         'haystack-ai==2.0.0',
         'pymupdf==1.22.5',
         'sentence-transformers==2.5.1',
         'umap==0.1.1',
```

