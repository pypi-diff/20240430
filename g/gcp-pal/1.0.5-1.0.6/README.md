# Comparing `tmp/gcp_pal-1.0.5.tar.gz` & `tmp/gcp_pal-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_pal-1.0.5.tar", max compression
+gzip compressed data, was "gcp_pal-1.0.6.tar", max compression
```

## Comparing `gcp_pal-1.0.5.tar` & `gcp_pal-1.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    25169 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/README.md
--rw-r--r--   0        0        0      810 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/__init__.py
--rw-r--r--   0        0        0    31402 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/bigquery.py
--rw-r--r--   0        0        0    13156 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/cloudfunctions.py
--rw-r--r--   0        0        0    13855 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/cloudrun.py
--rw-r--r--   0        0        0     7754 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/cloudscheduler.py
--rw-r--r--   0        0        0       42 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/config/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/config/vars.py
--rw-r--r--   0        0        0    12490 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/firestore.py
--rw-r--r--   0        0        0     3170 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/project.py
--rw-r--r--   0        0        0     1674 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/pubsub.py
--rw-r--r--   0        0        0     3873 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/pydocker.py
--rw-r--r--   0        0        0     6975 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/pylogging.py
--rw-r--r--   0        0        0     4737 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/request.py
--rw-r--r--   0        0        0    23631 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/schema.py
--rw-r--r--   0        0        0     6332 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/secretmanager.py
--rw-r--r--   0        0        0       88 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/storage/__init__.py
--rw-r--r--   0        0        0     8735 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/storage/parquet.py
--rw-r--r--   0        0        0    17133 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/storage/storage.py
--rw-r--r--   0        0        0       82 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/utils/__init__.py
--rw-r--r--   0        0        0      935 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/utils/lazy_loader.py
--rw-r--r--   0        0        0    11431 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/utils/utils.py
--rw-r--r--   0        0        0      958 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    25559 1970-01-01 00:00:00.000000 gcp_pal-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    25269 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/README.md
+-rw-r--r--   0        0        0      810 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/gcp_pal/__init__.py
+-rw-r--r--   0        0        0    31402 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/gcp_pal/bigquery.py
+-rw-r--r--   0        0        0    13156 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/gcp_pal/cloudfunctions.py
+-rw-r--r--   0        0        0    13855 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/gcp_pal/cloudrun.py
+-rw-r--r--   0        0        0     7754 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/gcp_pal/cloudscheduler.py
+-rw-r--r--   0        0        0       42 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/gcp_pal/config/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/config/vars.py
+-rw-r--r--   0        0        0    12490 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/firestore.py
+-rw-r--r--   0        0        0     3170 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/project.py
+-rw-r--r--   0        0        0     1674 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/pubsub.py
+-rw-r--r--   0        0        0     3873 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/pydocker.py
+-rw-r--r--   0        0        0     6975 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/pylogging.py
+-rw-r--r--   0        0        0     4737 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/request.py
+-rw-r--r--   0        0        0    23631 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/schema.py
+-rw-r--r--   0        0        0     6332 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/secretmanager.py
+-rw-r--r--   0        0        0       88 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/storage/__init__.py
+-rw-r--r--   0        0        0     8735 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/storage/parquet.py
+-rw-r--r--   0        0        0    17133 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/storage/storage.py
+-rw-r--r--   0        0        0       82 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/utils/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/utils/lazy_loader.py
+-rw-r--r--   0        0        0    11431 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/utils/utils.py
+-rw-r--r--   0        0        0     1017 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    25718 1970-01-01 00:00:00.000000 gcp_pal-1.0.6/PKG-INFO
```

### Comparing `gcp_pal-1.0.5/README.md` & `gcp_pal-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 # GCP Pal Library
 
 The `gcp-pal` library provides a set of utilities for interacting with Google Cloud Platform (GCP) services, streamlining the process of implementing GCP functionalities within your Python applications.
 
 The utilities are designed to work with the `google-cloud` Python libraries, providing a more user-friendly and intuitive interface for common tasks.
 
+Source code: **https://github.com/VitaminB16/gcp-pal**
+PyPI: **https://pypi.org/project/gcp-pal/**
+
 ---
 
 ## Installation
 
 The package is available on PyPI as `gcp-pal`. To install with `pip`:
 
 ```bash
```

### Comparing `gcp_pal-1.0.5/gcp_pal/__init__.py` & `gcp_pal-1.0.6/gcp_pal/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/bigquery.py` & `gcp_pal-1.0.6/gcp_pal/bigquery.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/cloudfunctions.py` & `gcp_pal-1.0.6/gcp_pal/cloudfunctions.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/cloudrun.py` & `gcp_pal-1.0.6/gcp_pal/cloudrun.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/cloudscheduler.py` & `gcp_pal-1.0.6/gcp_pal/cloudscheduler.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/config/vars.py` & `gcp_pal-1.0.6/gcp_pal/config/vars.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/firestore.py` & `gcp_pal-1.0.6/gcp_pal/firestore.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/project.py` & `gcp_pal-1.0.6/gcp_pal/project.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/pubsub.py` & `gcp_pal-1.0.6/gcp_pal/pubsub.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/pydocker.py` & `gcp_pal-1.0.6/gcp_pal/pydocker.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/pylogging.py` & `gcp_pal-1.0.6/gcp_pal/pylogging.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/request.py` & `gcp_pal-1.0.6/gcp_pal/request.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/schema.py` & `gcp_pal-1.0.6/gcp_pal/schema.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/secretmanager.py` & `gcp_pal-1.0.6/gcp_pal/secretmanager.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/storage/parquet.py` & `gcp_pal-1.0.6/gcp_pal/storage/parquet.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/storage/storage.py` & `gcp_pal-1.0.6/gcp_pal/storage/storage.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/utils/lazy_loader.py` & `gcp_pal-1.0.6/gcp_pal/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/gcp_pal/utils/utils.py` & `gcp_pal-1.0.6/gcp_pal/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.5/pyproject.toml` & `gcp_pal-1.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "gcp-pal"
-version = "1.0.5"
-description = ""
+version = "1.0.6"
+description = "Set of utilities for interacting with Google Cloud Platform"
 authors = ["VitaminB16 <artemiy.nosov@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gcp_pal-1.0.5/PKG-INFO` & `gcp_pal-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gcp-pal
-Version: 1.0.5
-Summary: 
+Version: 1.0.6
+Summary: Set of utilities for interacting with Google Cloud Platform
 Author: VitaminB16
 Author-email: artemiy.nosov@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -35,14 +35,17 @@
 
 # GCP Pal Library
 
 The `gcp-pal` library provides a set of utilities for interacting with Google Cloud Platform (GCP) services, streamlining the process of implementing GCP functionalities within your Python applications.
 
 The utilities are designed to work with the `google-cloud` Python libraries, providing a more user-friendly and intuitive interface for common tasks.
 
+Source code: **https://github.com/VitaminB16/gcp-pal**
+PyPI: **https://pypi.org/project/gcp-pal/**
+
 ---
 
 ## Installation
 
 The package is available on PyPI as `gcp-pal`. To install with `pip`:
 
 ```bash
```

