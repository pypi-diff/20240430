# Comparing `tmp/pglib-5.7.1.tar.gz` & `tmp/pglib-5.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pglib-5.7.1.tar", last modified: Thu Jan 25 23:12:39 2024, max compression
+gzip compressed data, was "pglib-5.8.1.tar", last modified: Tue Apr 30 17:38:44 2024, max compression
```

## Comparing `pglib-5.7.1.tar` & `pglib-5.8.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2024-01-25 23:12:39.857029 pglib-5.7.1/
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1075 2021-04-30 17:17:45.000000 pglib-5.7.1/LICENSE
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      101 2021-04-30 17:17:45.000000 pglib-5.7.1/MANIFEST.in
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      753 2024-01-25 23:12:39.857029 pglib-5.7.1/PKG-INFO
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      509 2021-04-30 17:17:45.000000 pglib-5.7.1/README.rst
-drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2024-01-25 23:12:39.853029 pglib-5.7.1/pglib/
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      264 2021-04-30 17:17:45.000000 pglib-5.7.1/pglib/__init__.py
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    16739 2021-04-30 17:17:45.000000 pglib-5.7.1/pglib/_version.py
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     9969 2022-07-23 05:57:37.000000 pglib-5.7.1/pglib/asyncpglib.py
-drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2024-01-25 23:12:39.853029 pglib-5.7.1/pglib.egg-info/
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      753 2024-01-25 23:12:39.000000 pglib-5.7.1/pglib.egg-info/PKG-INFO
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1599 2024-01-25 23:12:39.000000 pglib-5.7.1/pglib.egg-info/SOURCES.txt
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)        1 2024-01-25 23:12:39.000000 pglib-5.7.1/pglib.egg-info/dependency_links.txt
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       13 2024-01-25 23:12:39.000000 pglib-5.7.1/pglib.egg-info/top_level.txt
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       95 2024-01-25 23:12:39.857029 pglib-5.7.1/setup.cfg
--rwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)     5147 2024-01-25 23:10:38.000000 pglib-5.7.1/setup.py
-drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2024-01-25 23:12:39.857029 pglib-5.7.1/src/
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1628 2021-04-30 17:17:45.000000 pglib-5.7.1/src/byteswap.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    44500 2024-01-25 23:00:09.000000 pglib-5.7.1/src/connection.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      764 2022-07-23 04:49:54.000000 pglib-5.7.1/src/connection.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      540 2022-07-23 05:46:16.000000 pglib-5.7.1/src/conninfoopt.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      353 2022-07-23 05:38:59.000000 pglib-5.7.1/src/conninfoopt.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1494 2021-04-30 17:17:45.000000 pglib-5.7.1/src/datatypes.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      452 2021-04-30 17:17:45.000000 pglib-5.7.1/src/datatypes.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      385 2021-04-30 17:17:45.000000 pglib-5.7.1/src/debug.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       93 2021-04-30 17:17:45.000000 pglib-5.7.1/src/debug.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      587 2021-04-30 17:17:45.000000 pglib-5.7.1/src/enums.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       51 2021-04-30 17:17:45.000000 pglib-5.7.1/src/enums.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2867 2022-07-23 04:49:54.000000 pglib-5.7.1/src/errors.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      347 2021-04-30 17:17:45.000000 pglib-5.7.1/src/errors.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    10101 2022-07-23 05:55:49.000000 pglib-5.7.1/src/getdata.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      178 2021-04-30 17:17:45.000000 pglib-5.7.1/src/getdata.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1613 2021-04-30 17:17:45.000000 pglib-5.7.1/src/juliandate.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      239 2021-04-30 17:17:45.000000 pglib-5.7.1/src/juliandate.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    15639 2022-09-24 04:45:37.000000 pglib-5.7.1/src/params.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     3250 2021-04-30 17:17:45.000000 pglib-5.7.1/src/params.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    13847 2021-04-30 17:17:45.000000 pglib-5.7.1/src/pgarrays.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      362 2021-04-30 17:17:45.000000 pglib-5.7.1/src/pgarrays.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     7182 2022-09-24 04:36:59.000000 pglib-5.7.1/src/pglib.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     5541 2022-07-23 04:49:54.000000 pglib-5.7.1/src/pglib.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      196 2021-04-30 17:17:45.000000 pglib-5.7.1/src/pgtypes.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     7895 2024-01-25 22:40:59.000000 pglib-5.7.1/src/resultset.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1033 2021-04-30 17:17:45.000000 pglib-5.7.1/src/resultset.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    12377 2021-04-30 17:17:45.000000 pglib-5.7.1/src/row.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      432 2021-04-30 17:17:45.000000 pglib-5.7.1/src/row.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2421 2021-04-30 17:17:45.000000 pglib-5.7.1/src/runtime.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       58 2021-04-30 17:17:45.000000 pglib-5.7.1/src/runtime.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     4098 2022-07-23 05:00:28.000000 pglib-5.7.1/src/type_hstore.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      387 2022-07-23 05:00:42.000000 pglib-5.7.1/src/type_hstore.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2703 2022-09-24 04:42:40.000000 pglib-5.7.1/src/type_json.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      238 2022-09-24 04:42:23.000000 pglib-5.7.1/src/type_json.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      627 2022-07-23 05:56:05.000000 pglib-5.7.1/src/type_ltree.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      133 2022-07-23 05:50:42.000000 pglib-5.7.1/src/type_ltree.h
-drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2024-01-25 23:12:39.857029 pglib-5.7.1/test/
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     4469 2021-04-30 17:17:45.000000 pglib-5.7.1/test/test_async.py
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    35664 2024-01-25 23:01:51.000000 pglib-5.7.1/test/test_sync.py
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2245 2024-01-25 23:05:52.000000 pglib-5.7.1/test/testutils.py
+drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2024-04-30 17:38:44.584178 pglib-5.8.1/
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1075 2021-04-30 17:17:45.000000 pglib-5.8.1/LICENSE
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      101 2021-04-30 17:17:45.000000 pglib-5.8.1/MANIFEST.in
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      753 2024-04-30 17:38:44.584178 pglib-5.8.1/PKG-INFO
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      509 2021-04-30 17:17:45.000000 pglib-5.8.1/README.rst
+drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2024-04-30 17:38:44.584178 pglib-5.8.1/pglib/
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      264 2021-04-30 17:17:45.000000 pglib-5.8.1/pglib/__init__.py
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    16739 2021-04-30 17:17:45.000000 pglib-5.8.1/pglib/_version.py
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     9969 2022-07-23 05:57:37.000000 pglib-5.8.1/pglib/asyncpglib.py
+drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2024-04-30 17:38:44.584178 pglib-5.8.1/pglib.egg-info/
+-rw-r--r--   0 mkleehammer  (1000) mkleehammer  (1000)      753 2024-04-30 17:38:44.000000 pglib-5.8.1/pglib.egg-info/PKG-INFO
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1599 2024-04-30 17:38:44.000000 pglib-5.8.1/pglib.egg-info/SOURCES.txt
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)        1 2024-04-30 17:38:44.000000 pglib-5.8.1/pglib.egg-info/dependency_links.txt
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       13 2024-04-30 17:38:44.000000 pglib-5.8.1/pglib.egg-info/top_level.txt
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       95 2024-04-30 17:38:44.584178 pglib-5.8.1/setup.cfg
+-rwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)     5147 2024-04-30 17:37:00.000000 pglib-5.8.1/setup.py
+drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2024-04-30 17:38:44.584178 pglib-5.8.1/src/
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1628 2021-04-30 17:17:45.000000 pglib-5.8.1/src/byteswap.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    48712 2024-04-30 16:23:53.000000 pglib-5.8.1/src/connection.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      764 2022-07-23 04:49:54.000000 pglib-5.8.1/src/connection.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      540 2022-07-23 05:46:16.000000 pglib-5.8.1/src/conninfoopt.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      353 2022-07-23 05:38:59.000000 pglib-5.8.1/src/conninfoopt.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1494 2021-04-30 17:17:45.000000 pglib-5.8.1/src/datatypes.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      452 2021-04-30 17:17:45.000000 pglib-5.8.1/src/datatypes.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      385 2021-04-30 17:17:45.000000 pglib-5.8.1/src/debug.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       93 2021-04-30 17:17:45.000000 pglib-5.8.1/src/debug.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      587 2021-04-30 17:17:45.000000 pglib-5.8.1/src/enums.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       51 2021-04-30 17:17:45.000000 pglib-5.8.1/src/enums.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2867 2022-07-23 04:49:54.000000 pglib-5.8.1/src/errors.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      347 2021-04-30 17:17:45.000000 pglib-5.8.1/src/errors.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    10101 2022-07-23 05:55:49.000000 pglib-5.8.1/src/getdata.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      178 2021-04-30 17:17:45.000000 pglib-5.8.1/src/getdata.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1613 2021-04-30 17:17:45.000000 pglib-5.8.1/src/juliandate.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      239 2021-04-30 17:17:45.000000 pglib-5.8.1/src/juliandate.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    15639 2022-09-24 04:45:37.000000 pglib-5.8.1/src/params.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     3250 2021-04-30 17:17:45.000000 pglib-5.8.1/src/params.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    13847 2024-04-30 16:08:38.000000 pglib-5.8.1/src/pgarrays.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      362 2021-04-30 17:17:45.000000 pglib-5.8.1/src/pgarrays.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     7182 2022-09-24 04:36:59.000000 pglib-5.8.1/src/pglib.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     5539 2024-04-30 02:59:08.000000 pglib-5.8.1/src/pglib.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      196 2021-04-30 17:17:45.000000 pglib-5.8.1/src/pgtypes.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     7895 2024-01-25 22:40:59.000000 pglib-5.8.1/src/resultset.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1033 2021-04-30 17:17:45.000000 pglib-5.8.1/src/resultset.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    12377 2021-04-30 17:17:45.000000 pglib-5.8.1/src/row.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      432 2021-04-30 17:17:45.000000 pglib-5.8.1/src/row.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2421 2021-04-30 17:17:45.000000 pglib-5.8.1/src/runtime.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       58 2021-04-30 17:17:45.000000 pglib-5.8.1/src/runtime.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     4098 2022-07-23 05:00:28.000000 pglib-5.8.1/src/type_hstore.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      387 2022-07-23 05:00:42.000000 pglib-5.8.1/src/type_hstore.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2703 2022-09-24 04:42:40.000000 pglib-5.8.1/src/type_json.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      238 2022-09-24 04:42:23.000000 pglib-5.8.1/src/type_json.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      627 2022-07-23 05:56:05.000000 pglib-5.8.1/src/type_ltree.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      133 2022-07-23 05:50:42.000000 pglib-5.8.1/src/type_ltree.h
+drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2024-04-30 17:38:44.584178 pglib-5.8.1/test/
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     4469 2021-04-30 17:17:45.000000 pglib-5.8.1/test/test_async.py
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    37019 2024-04-30 16:26:40.000000 pglib-5.8.1/test/test_sync.py
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2245 2024-01-25 23:05:52.000000 pglib-5.8.1/test/testutils.py
```

### Comparing `pglib-5.7.1/LICENSE` & `pglib-5.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/PKG-INFO` & `pglib-5.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pglib
-Version: 5.7.1
+Version: 5.8.1
 Summary: A PostgreSQL interface
 Home-page: https://gitlab.com/mkleehammer/pglib
 Maintainer: Michael Kleehammer
 Maintainer-email: michael@kleehammer.com
 License: MIT
 Keywords: postgresql postgres
 Platform: UNKNOWN
```

### Comparing `pglib-5.7.1/pglib/_version.py` & `pglib-5.8.1/pglib/_version.py`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/pglib/asyncpglib.py` & `pglib-5.8.1/pglib/asyncpglib.py`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/pglib.egg-info/PKG-INFO` & `pglib-5.8.1/pglib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pglib
-Version: 5.7.1
+Version: 5.8.1
 Summary: A PostgreSQL interface
 Home-page: https://gitlab.com/mkleehammer/pglib
 Maintainer: Michael Kleehammer
 Maintainer-email: michael@kleehammer.com
 License: MIT
 Keywords: postgresql postgres
 Platform: UNKNOWN
```

### Comparing `pglib-5.7.1/pglib.egg-info/SOURCES.txt` & `pglib-5.8.1/pglib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/setup.py` & `pglib-5.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         settings['extra_compile_args'] = ['-Wno-write-strings']
 
     return settings
 
 
 setup(
     name='pglib',
-    version='5.7.1',
+    version='5.8.1',
     description='A PostgreSQL interface',
     long_description=long_description,
     maintainer='Michael Kleehammer',
     maintainer_email='michael@kleehammer.com',
     packages=['pglib'],
     ext_modules=[Extension('_pglib', _get_files(), **_get_settings())],
     keywords='postgresql postgres',
```

### Comparing `pglib-5.7.1/src/byteswap.h` & `pglib-5.8.1/src/byteswap.h`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/connection.cpp` & `pglib-5.8.1/src/connection.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,15 @@
         PyErr_SetString(Error, "Fatal error");
         return 0;
     }
 
     return result;
 }
 
+
 static const char doc_script[] = "Connection.script(sql) --> None\n\n"
     "Executes a script which can contain multiple statements separated by semicolons.";
 
 static PyObject* Connection_script(PyObject* self, PyObject* args)
 {
     Connection* cnxn = CastConnection(self, REQUIRE_OPEN);
     if (!cnxn)
@@ -200,14 +201,15 @@
         return SetResultError(result.Detach());
 
     default:
         Py_RETURN_NONE;
     }
 }
 
+
 const char* doc_copy_from =
     "Connection.copy_from(command, source) --> int\n"
     "\n"
     "Executes the given COPY FROM command and returns the number of records copied.\n"
     "\n"
     "command\n"
     "  The copy command which must be 'from stdin'.\n"
@@ -230,27 +232,27 @@
         return 0;
 
     // If source is a string (Unicode), store the UTF-encoded value in buffer. If a byte
     // object, store directly in buffer.  Otherwise, buffer will be zero and `source` must be
     // an object with a read method (e.g. file).
     const char* buffer = 0;
     Py_ssize_t buffer_size = 0;
-    PyObject* read_method = 0;
+    Object read_method;
 
     if (PyUnicode_Check(source))
     {
         buffer = PyUnicode_AsUTF8AndSize(source, &buffer_size);
         if (buffer == 0)
             return 0;
     }
     else
     {
         if (!PyObject_HasAttrString(source, "read"))
             return PyErr_Format(Error, "CSV source must be a string or file-like object.");
-        read_method = PyObject_GetAttrString(source, "read");
+        read_method.Attach(PyObject_GetAttrString(source, "read"));
     }
 
     Connection* cnxn = CastConnection(self, REQUIRE_OPEN);
     if (!cnxn)
         return 0;
 
     const char* szSQL = PyUnicode_AsUTF8(command);
@@ -350,14 +352,148 @@
     const char* sz = PQcmdTuples(final_result);
     if (sz == 0 || *sz == 0)
       Py_RETURN_NONE;
     return PyLong_FromLong(atoi(sz));
 }
 
 
+const char* doc_copy_to_csv =
+    "Connection.copy_to_csv(table, dest, header=0, delimiter=',', quote='\"')\n"
+    "\n"
+    "Execute a COPY TO command and return the number of records copied.\n"
+    "\n"
+    "table\n"
+    "  The table to copy from.\n"
+    "\n"
+    "dest\n"
+    "  The file-like object to write to.  Strings will be written, not bytes, so\n"
+    "  open in text mode.\n"
+    "\n"
+    "header\n"
+    "  If non-zero, a CSV header will be written.\n";
+
+
+static PyObject* Connection_copy_to_csv(PyObject* self, PyObject* args, PyObject* kwargs)
+{
+    // This is not nearly as efficient as I'd like since newer Python versions no longer give
+    // us access to underlying file objects.  We have to write strings through a write method
+    // since there are io layers involved.
+    //
+    // For maximum performance, we should probably offer an option where we open the file given
+    // a filename.  We can either check the parameter type here or we could make a separate
+    // method with "file" in the name like copy_to_file.
+
+    static const char* kwlist[] = {"table", "dest", "header", "delimiter", "quote", 0};
+
+    PyObject* table;
+    PyObject* dest;
+    int header = 0;
+    char* szDelimiter = 0;
+    char* szQuote = 0;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "UO|pzz", (char**)kwlist, &table, &dest, &header,
+                                     &szDelimiter, &szQuote)) {
+        return 0;
+    }
+
+    Connection* cnxn = CastConnection(self, REQUIRE_OPEN);
+    if (!cnxn)
+        return 0;
+
+    if (!PyObject_HasAttrString(dest, "write"))
+        return PyErr_Format(Error, "CSV destination must be a file-like object.");
+    Object write_method(PyObject_GetAttrString(dest, "write"));
+
+    char header_token[] = "header";
+    if (header == 0) {
+        header_token[0] = 0;
+    }
+
+    const char* pszDelimiter = szDelimiter ? szDelimiter : ",";
+    const char* pszQuote = szQuote ? szQuote : "\"";
+
+    Object sql(PyUnicode_FromFormat("copy %U to stdout with csv %s delimiter '%s' quote '%s'",
+                                    table, header_token, pszDelimiter, pszQuote));
+
+    const char* szSQL = PyUnicode_AsUTF8(sql);
+    ResultHolder result;
+    Py_BEGIN_ALLOW_THREADS
+    result = PQexec(cnxn->pgconn, szSQL);
+    Py_END_ALLOW_THREADS
+
+    if (result == 0)
+        return 0;
+
+    switch (PQresultStatus(result)) {
+    case PGRES_COPY_OUT:
+        // This is what we are expecting.
+        break;
+
+    case PGRES_BAD_RESPONSE:
+    case PGRES_NONFATAL_ERROR:
+    case PGRES_FATAL_ERROR:
+        return SetResultError(result.Detach());
+
+    default:
+        return PyErr_Format(Error, "Result was not PGRES_COPY_IN: %d", (int)PQresultStatus(result));
+    }
+
+
+    for (;;) {
+        int cb = 0;
+        char* buffer;
+        Py_BEGIN_ALLOW_THREADS
+        cb = PQgetCopyData(cnxn->pgconn, &buffer, 0);
+        Py_END_ALLOW_THREADS
+
+        if (cb == -2) {
+            return SetResultError(result.Detach());
+        }
+
+        if (cb == -1) {
+            // The copy is complete.
+            break;
+        }
+
+        // We have a buffer of byte data.  We have the length, but the libpq docs say that the
+        // string is also zero terminated, so we're going to try not calling 'write'.
+
+        int err = PyFile_WriteString(buffer, dest);
+
+        //  while (cb > 0) {
+        //      PyObject* res = PyObject_CallObject(write_method)
+        //  }
+
+        PQfreemem(buffer);
+        if (err) {
+            return 0;
+        }
+    }
+
+    // After a copy, you have to get another result to know if it was successful.
+
+    ResultHolder final_result;
+    ExecStatusType status = PGRES_COMMAND_OK;
+    Py_BEGIN_ALLOW_THREADS
+    final_result = PQgetResult(cnxn->pgconn);
+    status = PQresultStatus(final_result);
+    Py_END_ALLOW_THREADS
+
+    if (status != PGRES_COMMAND_OK) {
+      // SetResultError will take ownership of `result`.
+      return SetResultError(final_result.Detach());
+    }
+
+    const char* sz = PQcmdTuples(final_result);
+    if (sz == 0 || *sz == 0)
+      Py_RETURN_NONE;
+    return PyLong_FromLong(atoi(sz));
+}
+
+
 const char* doc_copy_from_csv =
     "Connection.copy_from_csv(table, source, header=0) --> int\n"
     "\n"
     "Executes a COPY FROM command and returns the number of records copied.\n"
     "\n"
     "table\n"
     "  The table to copy to.  This can also contain the columns to populate.\n"
@@ -386,35 +522,36 @@
 
     char header_token[] = "header";
     if (header == 0)
         header_token[0] = 0;
 
     const char* pszDelimiter = szDelimiter ? szDelimiter : ",";
     const char* pszQuote = szQuote ? szQuote : "\"";
-    PyObject* sql = PyUnicode_FromFormat("copy %U from stdin with csv %s delimiter '%s' quote '%s'",
-                                         table, header_token, pszDelimiter, pszQuote);
+    Object sql(PyUnicode_FromFormat("copy %U from stdin with csv %s delimiter '%s' quote '%s'",
+                                    table, header_token, pszDelimiter, pszQuote));
 
     // If source is a string (Unicode), store the UTF-encoded value in buffer. If a byte
     // object, store directly in buffer.  Otherwise, buffer will be zero and `source` must be
     // an object with a read method (e.g. file).
     const char* buffer = 0;
     Py_ssize_t buffer_size = 0;
-    PyObject* read_method = 0;
+    Object read_method;
+    //  PyObject* read_method = 0;
 
     if (PyUnicode_Check(source))
     {
         buffer = PyUnicode_AsUTF8AndSize(source, &buffer_size);
         if (buffer == 0)
             return 0;
     }
     else
     {
         if (!PyObject_HasAttrString(source, "read"))
             return PyErr_Format(Error, "CSV source must be a string or file-like object.");
-        read_method = PyObject_GetAttrString(source, "read");
+        read_method.Attach(PyObject_GetAttrString(source, "read"));
     }
 
     Connection* cnxn = CastConnection(self, REQUIRE_OPEN);
     if (!cnxn)
         return 0;
 
     const char* szSQL = PyUnicode_AsUTF8(sql);
@@ -1458,14 +1595,15 @@
     { "row",     Connection_row,     METH_VARARGS, 0 },
     { "scalar",  Connection_fetchval,  METH_VARARGS, 0 }, // deprecated
     { "trace",   Connection_trace,   METH_VARARGS, 0 },
     { "reset",   Connection_reset,   METH_NOARGS,  0 },
     { "script",  Connection_script,  METH_VARARGS, doc_script },
     { "copy_from", (PyCFunction) Connection_copy_from, METH_VARARGS | METH_KEYWORDS, doc_copy_from },
     { "copy_from_csv", (PyCFunction) Connection_copy_from_csv, METH_VARARGS | METH_KEYWORDS, doc_copy_from_csv },
+    { "copy_to_csv", (PyCFunction) Connection_copy_to_csv, METH_VARARGS | METH_KEYWORDS, doc_copy_to_csv},
     { "begin",    Connection_begin,   METH_NOARGS, doc_begin },
     { "commit",   Connection_commit,   METH_NOARGS, doc_commit },
     { "rollback", Connection_rollback,   METH_NOARGS, doc_rollback },
     { "close", Connection_close,   METH_NOARGS, doc_close },
     { "_connectPoll", Connection_connectPoll, METH_NOARGS, 0 },
     { "_sendQuery", Connection_sendQuery, METH_VARARGS, 0 },
     { "_sendQueryParams", Connection_sendQueryParams, METH_VARARGS, 0 },
```

### Comparing `pglib-5.7.1/src/connection.h` & `pglib-5.8.1/src/connection.h`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/conninfoopt.cpp` & `pglib-5.8.1/src/conninfoopt.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/datatypes.cpp` & `pglib-5.8.1/src/datatypes.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/enums.cpp` & `pglib-5.8.1/src/enums.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/errors.cpp` & `pglib-5.8.1/src/errors.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/getdata.cpp` & `pglib-5.8.1/src/getdata.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/juliandate.cpp` & `pglib-5.8.1/src/juliandate.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/params.cpp` & `pglib-5.8.1/src/params.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/params.h` & `pglib-5.8.1/src/params.h`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/pgarrays.cpp` & `pglib-5.8.1/src/pgarrays.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/pglib.cpp` & `pglib-5.8.1/src/pglib.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/pglib.h` & `pglib-5.8.1/src/pglib.h`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 // -----------------------------------------------------------------------------------------------
 // C++ wrappers for objects.  No exceptions.
 
 struct Object
 {
     PyObject* p;
 
-    // Borrows the reference (takes ownership without adding a new referencing).
+    // Borrows the reference (takes ownership without adding a new reference).
     Object(PyObject* _p = 0) { p = _p; }
 
     // If it still has the pointer, it dereferences it.
     ~Object() { Py_XDECREF(p); }
 
     operator PyObject*() { return p; }
     PyObject* Get() { return p; }
```

### Comparing `pglib-5.7.1/src/resultset.cpp` & `pglib-5.8.1/src/resultset.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/resultset.h` & `pglib-5.8.1/src/resultset.h`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/row.cpp` & `pglib-5.8.1/src/row.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/runtime.cpp` & `pglib-5.8.1/src/runtime.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/type_hstore.cpp` & `pglib-5.8.1/src/type_hstore.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/type_json.cpp` & `pglib-5.8.1/src/type_json.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/src/type_ltree.cpp` & `pglib-5.8.1/src/type_ltree.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/test/test_async.py` & `pglib-5.8.1/test/test_async.py`

 * *Files identical despite different names*

### Comparing `pglib-5.7.1/test/test_sync.py` & `pglib-5.8.1/test/test_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 # Run with pytest.
 
 # pylint: disable=missing-function-docstring,redefined-outer-name,unidiomatic-typecheck
 
-import sys, threading, gzip, uuid, locale
+import sys, threading, gzip, uuid, locale, tempfile, csv
 from time import sleep
 from os.path import join, dirname, exists
 from decimal import Decimal
-from datetime import date, time, datetime, timedelta, timezone
+from datetime import date, time, datetime, timedelta
 from pathlib import Path
 import pytest
 
 from .import testutils
 testutils.add_to_path()
 
 import pglib
@@ -28,29 +28,29 @@
     # Warning: If I don't manually close the connection, they are not getting deleted.  I don't
     # know if pytest saves them in some test context for each test or what.
 
     # Note that I'm not using "if exists" because that annoyingly prints a notice.
     cnxn = pglib.connect(CONNINFO)
     for i in range(3):
         try:
-            cnxn.execute("drop table t%d" % i)
+            cnxn.execute(f"drop table t{i}")
         except:                 # noqa
             pass
     yield cnxn
     cnxn.close()
 
 
 def _test_strtype(cnxn, sqltype, value, resulttype=None, colsize=None):
     assert colsize is None or isinstance(colsize, int), colsize
     assert colsize is None or (value is None or colsize >= len(value))
 
     if colsize:
-        sql = "create table t1(s %s(%s))" % (sqltype, colsize)
+        sql = f"create table t1(s {sqltype}({colsize}))"
     else:
-        sql = "create table t1(s %s)" % sqltype
+        sql = f"create table t1(s {sqltype})"
 
     if resulttype is None:
         resulttype = type(value)
 
     cnxn.execute(sql)
     cnxn.execute("insert into t1 values($1)", value)
     v = cnxn.fetchval("select * from t1")
@@ -144,57 +144,91 @@
     select 2;
     select 3;
     """
     cnxn.script(sql)
 
 
 #
-# copy
+# copy to
+#
+
+def test_copytocsv(cnxn):
+    # Write a table to a CSV file.
+    #
+    # It isn't as efficient as I'd like since we can no longer get ahold of the file
+    # descriptor.  I think we'll want to make this accept a string filename for a more
+    # efficient write.  For now, make sure the output file is opened in text mode.
+
+    cnxn.execute("create table t1(a text, b text)")
+    cnxn.execute("insert into t1 values ('1', 'one'), ('2', 'two'), ('3', 'three')")
+
+    with tempfile.NamedTemporaryFile(mode='w', encoding='utf8') as tf:
+        print(tf.name)
+        count = cnxn.copy_to_csv('t1', tf, header=1)
+        assert count == 3
+
+        tf.seek(0)
+        with open(tf.name, mode='r', encoding='utf8') as fd:
+            reader = csv.reader(fd)
+            rows = []
+            for row in reader:
+                print('ROW=', row)
+                rows.append(row)
+
+            assert rows == [['a', 'b'], ['1', 'one'], ['2', 'two'], ['3', 'three']]
+
+
+#
+# copy from
 #
 
 def _datapath(filename):
     path = join(dirname(__file__), filename)
     assert exists(path)
     return path
 
 
 def test_copyfromcsv_csv(cnxn):
     cnxn.execute("create table t1(a int, b varchar(20))")
-    count = cnxn.copy_from_csv("t1", open(_datapath('test-noheader.csv')))
+    with open(_datapath('test-noheader.csv')) as fd:
+        count = cnxn.copy_from_csv("t1", fd)
     assert count == 2
     assert cnxn.fetchval("select count(*) from t1") == 2
     row = cnxn.fetchrow("select a,b from t1 where a=2")
     assert row.a == 2
     assert row.b == 'two'
 
 
 def test_copyfromcsv_csv_header(cnxn):
     cnxn.execute("create table t1(a int, b varchar(20))")
-    count = cnxn.copy_from_csv("t1", open(_datapath('test-header.csv')), header=True)
+    with open(_datapath('test-header.csv')) as fd:
+        count = cnxn.copy_from_csv("t1", fd, header=True)
     assert count == 2
     assert cnxn.fetchval("select count(*) from t1") == 2
     row = cnxn.fetchrow("select a,b from t1 where a=2")
     assert row.a == 2
     assert row.b == 'two'
 
 
 def test_copyfromcsv_csv_error(cnxn):
     """
     Ensure an error copying raises a Python error.
     """
     # We'll make the second column too small.
     cnxn.execute("create table t1(a int, b varchar(1) not null)")
     with pytest.raises(pglib.Error):
-        cnxn.copy_from_csv("t1", open(_datapath('test-noheader.csv')))
+        with open(_datapath('test-noheader.csv')) as fd:
+            cnxn.copy_from_csv("t1", fd)
 
 
 def test_copyfromcsv_csv_gzip(cnxn):
     # I don't remember why this test is here.  We're feeding it unzipped data.
     cnxn.execute("create table t1(a int, b varchar(20))")
-    cnxn.copy_from_csv("t1", gzip.open(_datapath('test-header.csv.gz')), header=True)
+    with gzip.open(_datapath('test-header.csv.gz')) as fd:
+        cnxn.copy_from_csv("t1", fd, header=True)
     assert cnxn.fetchval("select count(*) from t1") == 2
     row = cnxn.fetchrow("select a,b from t1 where a=2")
     assert row.a == 2
     assert row.b == 'two'
 
 
 def test_copyfromcsv_csv_string(cnxn):
@@ -1059,24 +1093,36 @@
     with pytest.raises(pglib.Error):
         cnxn.begin()
 
     with pytest.raises(pglib.Error):
         cnxn.rollback()
 
 
-def test_count():
+def test_connection_count():
     before = pglib.connection_count()
     cnxn = pglib.connect(CONNINFO)
     assert pglib.connection_count() == (before + 1)
     cnxn.close()
     assert pglib.connection_count() == before
     cnxn = None
     assert pglib.connection_count() == before
 
 
+def test_count(cnxn):
+    "Ensure delete statements return affected row count."
+    cnxn.execute(
+        """
+        select generate_series(1, 3) as id
+          into t1
+        """)
+
+    count = cnxn.execute("delete from t1 where id in (1, 2, 3)")
+    assert count == 3
+
+
 def test_hstore(cnxn):
     cnxn.execute("create extension if not exists hstore")
     row = cnxn.fetchrow("select oid, typname from pg_type where typname='hstore'")
     pglib.register_type(row.oid, row.typname)
 
     cnxn.execute("create table t1(id serial, fields hstore)")
```

### Comparing `pglib-5.7.1/test/testutils.py` & `pglib-5.8.1/test/testutils.py`

 * *Files identical despite different names*

