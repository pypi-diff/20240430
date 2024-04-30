# Comparing `tmp/netsuite_connector-0.3.0.tar.gz` & `tmp/netsuite_connector-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_connector-0.3.0.tar", last modified: Fri Apr 19 00:41:41 2024, max compression
+gzip compressed data, was "netsuite_connector-0.3.1.tar", last modified: Tue Apr 30 14:47:56 2024, max compression
```

## Comparing `netsuite_connector-0.3.0.tar` & `netsuite_connector-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-19 00:41:41.539584 netsuite_connector-0.3.0/
--rw-r--r--   0 marcos     (501) staff       (20)     1069 2024-04-18 21:33:03.000000 netsuite_connector-0.3.0/LICENSE
--rw-r--r--   0 marcos     (501) staff       (20)     4440 2024-04-19 00:41:41.539176 netsuite_connector-0.3.0/PKG-INFO
--rw-r--r--   0 marcos     (501) staff       (20)     2661 2024-04-18 23:56:48.000000 netsuite_connector-0.3.0/README.md
--rw-r--r--   0 marcos     (501) staff       (20)      713 2024-04-18 23:05:56.000000 netsuite_connector-0.3.0/pyproject.toml
--rw-r--r--   0 marcos     (501) staff       (20)       38 2024-04-19 00:41:41.539648 netsuite_connector-0.3.0/setup.cfg
-drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-19 00:41:41.531896 netsuite_connector-0.3.0/src/
-drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-19 00:41:41.533578 netsuite_connector-0.3.0/src/NetSuite_Connector/
--rw-r--r--   0 marcos     (501) staff       (20)     5585 2024-04-18 23:53:43.000000 netsuite_connector-0.3.0/src/NetSuite_Connector/NetSuite.py
--rw-r--r--   0 marcos     (501) staff       (20)     1612 2024-04-19 00:01:26.000000 netsuite_connector-0.3.0/src/NetSuite_Connector/ODBC.py
--rw-------   0 marcos     (501) staff       (20)        0 2022-10-25 21:58:40.000000 netsuite_connector-0.3.0/src/NetSuite_Connector/__init__.py
-drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-19 00:41:41.538701 netsuite_connector-0.3.0/src/NetSuite_Connector.egg-info/
--rw-r--r--   0 marcos     (501) staff       (20)     4440 2024-04-19 00:41:41.000000 netsuite_connector-0.3.0/src/NetSuite_Connector.egg-info/PKG-INFO
--rw-r--r--   0 marcos     (501) staff       (20)      359 2024-04-19 00:41:41.000000 netsuite_connector-0.3.0/src/NetSuite_Connector.egg-info/SOURCES.txt
--rw-r--r--   0 marcos     (501) staff       (20)        1 2024-04-19 00:41:41.000000 netsuite_connector-0.3.0/src/NetSuite_Connector.egg-info/dependency_links.txt
--rw-r--r--   0 marcos     (501) staff       (20)       19 2024-04-19 00:41:41.000000 netsuite_connector-0.3.0/src/NetSuite_Connector.egg-info/top_level.txt
-drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-19 00:41:41.538259 netsuite_connector-0.3.0/tests/
--rw-r--r--   0 marcos     (501) staff       (20)    12133 2024-04-18 23:59:11.000000 netsuite_connector-0.3.0/tests/test_netsuite.py
--rw-r--r--   0 marcos     (501) staff       (20)     7682 2024-04-18 21:33:57.000000 netsuite_connector-0.3.0/tests/test_odbc.py
+drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-30 14:47:56.089307 netsuite_connector-0.3.1/
+-rw-r--r--   0 marcos     (501) staff       (20)     1069 2024-04-18 21:33:03.000000 netsuite_connector-0.3.1/LICENSE
+-rw-r--r--   0 marcos     (501) staff       (20)     4440 2024-04-30 14:47:56.088909 netsuite_connector-0.3.1/PKG-INFO
+-rw-r--r--   0 marcos     (501) staff       (20)     2661 2024-04-18 23:56:48.000000 netsuite_connector-0.3.1/README.md
+-rw-r--r--   0 marcos     (501) staff       (20)      713 2024-04-29 22:19:20.000000 netsuite_connector-0.3.1/pyproject.toml
+-rw-r--r--   0 marcos     (501) staff       (20)       38 2024-04-30 14:47:56.089365 netsuite_connector-0.3.1/setup.cfg
+drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-30 14:47:56.078497 netsuite_connector-0.3.1/src/
+drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-30 14:47:56.083240 netsuite_connector-0.3.1/src/NetSuite_Connector/
+-rw-r--r--   0 marcos     (501) staff       (20)     8379 2024-04-29 22:44:47.000000 netsuite_connector-0.3.1/src/NetSuite_Connector/NetSuite.py
+-rw-r--r--   0 marcos     (501) staff       (20)     1613 2024-04-29 22:17:05.000000 netsuite_connector-0.3.1/src/NetSuite_Connector/ODBC.py
+-rw-------   0 marcos     (501) staff       (20)        0 2022-10-25 21:58:40.000000 netsuite_connector-0.3.1/src/NetSuite_Connector/__init__.py
+drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-30 14:47:56.088530 netsuite_connector-0.3.1/src/NetSuite_Connector.egg-info/
+-rw-r--r--   0 marcos     (501) staff       (20)     4440 2024-04-30 14:47:56.000000 netsuite_connector-0.3.1/src/NetSuite_Connector.egg-info/PKG-INFO
+-rw-r--r--   0 marcos     (501) staff       (20)      359 2024-04-30 14:47:56.000000 netsuite_connector-0.3.1/src/NetSuite_Connector.egg-info/SOURCES.txt
+-rw-r--r--   0 marcos     (501) staff       (20)        1 2024-04-30 14:47:56.000000 netsuite_connector-0.3.1/src/NetSuite_Connector.egg-info/dependency_links.txt
+-rw-r--r--   0 marcos     (501) staff       (20)       19 2024-04-30 14:47:56.000000 netsuite_connector-0.3.1/src/NetSuite_Connector.egg-info/top_level.txt
+drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-30 14:47:56.087719 netsuite_connector-0.3.1/tests/
+-rw-r--r--   0 marcos     (501) staff       (20)    12133 2024-04-30 14:45:57.000000 netsuite_connector-0.3.1/tests/test_netsuite.py
+-rw-r--r--   0 marcos     (501) staff       (20)     7682 2024-04-18 21:33:57.000000 netsuite_connector-0.3.1/tests/test_odbc.py
```

### Comparing `netsuite_connector-0.3.0/LICENSE` & `netsuite_connector-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netsuite_connector-0.3.0/PKG-INFO` & `netsuite_connector-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetSuite-Connector
-Version: 0.3.0
+Version: 0.3.1
 Summary: NetSuite Connector
 Author-email: Marcos Lopez <merick16@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Marcos Lopez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `netsuite_connector-0.3.0/README.md` & `netsuite_connector-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `netsuite_connector-0.3.0/pyproject.toml` & `netsuite_connector-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.27.1","requests-oauthlib>=1.3.1","pyodbc>=4.0.34","pandas>=1.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NetSuite-Connector"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Marcos Lopez", email="merick16@gmail.com" },
 ]
 description = "NetSuite Connector"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `netsuite_connector-0.3.0/src/NetSuite_Connector/ODBC.py` & `netsuite_connector-0.3.1/src/NetSuite_Connector/ODBC.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .NetSuite import NetSuite, NetsuiteObject
 
 
 class ODBC(NetSuite):
 
     def __init__(self, account_id: Any, consumer_keys: dict, token_keys: dict) -> None:
         super().__init__(account_id, consumer_keys, token_keys)
-        self.suiteql_endpoint = f'https://{account_id.lower().replace("-", "")}.suitetalk.api.netsuite.com/services/rest/query/v1/suiteql'
+        self.suiteql_endpoint = f'https://{account_id.lower().replace("_", "-")}.suitetalk.api.netsuite.com/services/rest/query/v1/suiteql'
 
     def query(self, query: str) -> NetsuiteObject:
         """
         Perfom a query to ODBC driver
         query: fully qualified sql query
         >>> from NetSuite_Connector.ODBC import ODBC
```

### Comparing `netsuite_connector-0.3.0/src/NetSuite_Connector.egg-info/PKG-INFO` & `netsuite_connector-0.3.1/src/NetSuite_Connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetSuite-Connector
-Version: 0.3.0
+Version: 0.3.1
 Summary: NetSuite Connector
 Author-email: Marcos Lopez <merick16@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Marcos Lopez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `netsuite_connector-0.3.0/tests/test_netsuite.py` & `netsuite_connector-0.3.1/tests/test_netsuite.py`

 * *Files identical despite different names*

### Comparing `netsuite_connector-0.3.0/tests/test_odbc.py` & `netsuite_connector-0.3.1/tests/test_odbc.py`

 * *Files identical despite different names*

