# Comparing `tmp/diambra-engine-2.2.3.tar.gz` & `tmp/diambra-engine-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diambra-engine-2.2.3.tar", last modified: Sun Apr 28 15:30:46 2024, max compression
+gzip compressed data, was "diambra-engine-2.2.4.tar", last modified: Tue Apr 30 19:10:57 2024, max compression
```

## Comparing `diambra-engine-2.2.3.tar` & `diambra-engine-2.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:30:46.820932 diambra-engine-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-28 15:30:46.820932 diambra-engine-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-28 15:30:36.000000 diambra-engine-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:30:46.816932 diambra-engine-2.2.3/diambra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 15:30:36.000000 diambra-engine-2.2.3/diambra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:30:46.816932 diambra-engine-2.2.3/diambra/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-28 15:30:36.000000 diambra-engine-2.2.3/diambra/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28742 2024-04-28 15:30:45.000000 diambra-engine-2.2.3/diambra/engine/interface_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8969 2024-04-28 15:30:45.000000 diambra-engine-2.2.3/diambra/engine/interface_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:30:46.816932 diambra-engine-2.2.3/diambra_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-28 15:30:46.000000 diambra-engine-2.2.3/diambra_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-28 15:30:46.000000 diambra-engine-2.2.3/diambra_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:30:46.000000 diambra-engine-2.2.3/diambra_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-28 15:30:46.000000 diambra-engine-2.2.3/diambra_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 15:30:46.000000 diambra-engine-2.2.3/diambra_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:30:46.820932 diambra-engine-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-28 15:30:36.000000 diambra-engine-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:10:57.560346 diambra-engine-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-30 19:10:57.560346 diambra-engine-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-30 19:10:45.000000 diambra-engine-2.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:10:57.556346 diambra-engine-2.2.4/diambra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:10:45.000000 diambra-engine-2.2.4/diambra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:10:57.556346 diambra-engine-2.2.4/diambra/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-30 19:10:45.000000 diambra-engine-2.2.4/diambra/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28742 2024-04-30 19:10:56.000000 diambra-engine-2.2.4/diambra/engine/interface_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8969 2024-04-30 19:10:56.000000 diambra-engine-2.2.4/diambra/engine/interface_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:10:57.560346 diambra-engine-2.2.4/diambra_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-30 19:10:57.000000 diambra-engine-2.2.4/diambra_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-30 19:10:57.000000 diambra-engine-2.2.4/diambra_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:10:57.000000 diambra-engine-2.2.4/diambra_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 19:10:57.000000 diambra-engine-2.2.4/diambra_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 19:10:57.000000 diambra-engine-2.2.4/diambra_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:10:57.560346 diambra-engine-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-30 19:10:45.000000 diambra-engine-2.2.4/setup.py
```

### Comparing `diambra-engine-2.2.3/PKG-INFO` & `diambra-engine-2.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-engine
-Version: 2.2.3
+Version: 2.2.4
 Summary: DIAMBRA™ Arena Engine API Client
 Home-page: https://diambra.ai
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

### Comparing `diambra-engine-2.2.3/diambra/engine/__init__.py` & `diambra-engine-2.2.4/diambra/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `diambra-engine-2.2.3/diambra/engine/interface_pb2.py` & `diambra-engine-2.2.4/diambra/engine/interface_pb2.py`

 * *Files identical despite different names*

### Comparing `diambra-engine-2.2.3/diambra/engine/interface_pb2_grpc.py` & `diambra-engine-2.2.4/diambra/engine/interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `diambra-engine-2.2.3/diambra_engine.egg-info/PKG-INFO` & `diambra-engine-2.2.4/diambra_engine.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-engine
-Version: 2.2.3
+Version: 2.2.4
 Summary: DIAMBRA™ Arena Engine API Client
 Home-page: https://diambra.ai
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

### Comparing `diambra-engine-2.2.3/setup.py` & `diambra-engine-2.2.4/setup.py`

 * *Files identical despite different names*

