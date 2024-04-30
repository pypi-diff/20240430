# Comparing `tmp/retriever_search-0.0.2.tar.gz` & `tmp/retriever_search-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retriever_search-0.0.2.tar", last modified: Tue Apr 30 04:43:54 2024, max compression
+gzip compressed data, was "retriever_search-0.0.6.tar", last modified: Tue Apr 30 05:07:14 2024, max compression
```

## Comparing `retriever_search-0.0.2.tar` & `retriever_search-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 04:43:54.569067 retriever_search-0.0.2/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.0.2/LICENSE
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1170 2024-04-30 04:43:54.568729 retriever_search-0.0.2/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      534 2024-04-30 04:43:33.000000 retriever_search-0.0.2/README.md
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 04:43:54.566881 retriever_search-0.0.2/retriever_search/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6434 2024-04-24 08:53:52.000000 retriever_search-0.0.2/retriever_search/DocumentIngestion.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.0.2/retriever_search/QueryPipeline.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       85 2024-04-30 04:43:45.000000 retriever_search-0.0.2/retriever_search/__init__.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3617 2024-04-24 08:53:52.000000 retriever_search-0.0.2/retriever_search/frontend_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1424 2024-04-25 03:47:47.000000 retriever_search-0.0.2/retriever_search/search_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3381 2024-04-25 03:47:48.000000 retriever_search-0.0.2/retriever_search/search_server.py
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 04:43:54.568326 retriever_search-0.0.2/retriever_search.egg-info/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1170 2024-04-30 04:43:54.000000 retriever_search-0.0.2/retriever_search.egg-info/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      424 2024-04-30 04:43:54.000000 retriever_search-0.0.2/retriever_search.egg-info/SOURCES.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-30 04:43:54.000000 retriever_search-0.0.2/retriever_search.egg-info/dependency_links.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      191 2024-04-30 04:43:54.000000 retriever_search-0.0.2/retriever_search.egg-info/requires.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-04-30 04:43:54.000000 retriever_search-0.0.2/retriever_search.egg-info/top_level.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-04-30 04:43:54.569143 retriever_search-0.0.2/setup.cfg
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      834 2024-04-30 04:41:43.000000 retriever_search-0.0.2/setup.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 05:07:14.939724 retriever_search-0.0.6/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.0.6/LICENSE
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1841 2024-04-30 05:07:14.939390 retriever_search-0.0.6/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1205 2024-04-30 05:04:29.000000 retriever_search-0.0.6/README.md
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 05:07:14.937301 retriever_search-0.0.6/retriever_search/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6434 2024-04-24 08:53:52.000000 retriever_search-0.0.6/retriever_search/DocumentIngestion.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.0.6/retriever_search/QueryPipeline.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       85 2024-04-30 05:07:08.000000 retriever_search-0.0.6/retriever_search/__init__.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3617 2024-04-24 08:53:52.000000 retriever_search-0.0.6/retriever_search/frontend_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1424 2024-04-25 03:47:47.000000 retriever_search-0.0.6/retriever_search/search_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3381 2024-04-25 03:47:48.000000 retriever_search-0.0.6/retriever_search/search_server.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 05:07:14.938963 retriever_search-0.0.6/retriever_search.egg-info/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1841 2024-04-30 05:07:14.000000 retriever_search-0.0.6/retriever_search.egg-info/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      424 2024-04-30 05:07:14.000000 retriever_search-0.0.6/retriever_search.egg-info/SOURCES.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-30 05:07:14.000000 retriever_search-0.0.6/retriever_search.egg-info/dependency_links.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      191 2024-04-30 05:07:14.000000 retriever_search-0.0.6/retriever_search.egg-info/requires.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-04-30 05:07:14.000000 retriever_search-0.0.6/retriever_search.egg-info/top_level.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-04-30 05:07:14.939798 retriever_search-0.0.6/setup.cfg
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      834 2024-04-30 04:41:43.000000 retriever_search-0.0.6/setup.py
```

### Comparing `retriever_search-0.0.2/LICENSE` & `retriever_search-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.2/retriever_search/DocumentIngestion.py` & `retriever_search-0.0.6/retriever_search/DocumentIngestion.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.2/retriever_search/QueryPipeline.py` & `retriever_search-0.0.6/retriever_search/QueryPipeline.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.2/retriever_search/frontend_app.py` & `retriever_search-0.0.6/retriever_search/frontend_app.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.2/retriever_search/search_app.py` & `retriever_search-0.0.6/retriever_search/search_app.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.2/retriever_search/search_server.py` & `retriever_search-0.0.6/retriever_search/search_server.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.2/setup.py` & `retriever_search-0.0.6/setup.py`

 * *Files identical despite different names*

