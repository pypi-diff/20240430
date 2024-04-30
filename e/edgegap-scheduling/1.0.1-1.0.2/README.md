# Comparing `tmp/edgegap_scheduling-1.0.1.tar.gz` & `tmp/edgegap_scheduling-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_scheduling-1.0.1.tar", max compression
+gzip compressed data, was "edgegap_scheduling-1.0.2.tar", max compression
```

## Comparing `edgegap_scheduling-1.0.1.tar` & `edgegap_scheduling-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1993 2024-04-29 18:21:35.343371 edgegap_scheduling-1.0.1/LICENSE
--rw-r--r--   0        0        0     2164 2024-04-29 18:21:35.343371 edgegap_scheduling-1.0.1/README.md
--rw-r--r--   0        0        0      280 2024-04-29 18:21:35.343371 edgegap_scheduling-1.0.1/edgegap_scheduling/__init__.py
--rw-r--r--   0        0        0      128 2024-04-29 18:21:35.343371 edgegap_scheduling-1.0.1/edgegap_scheduling/_depends.py
--rw-r--r--   0        0        0     3389 2024-04-29 18:21:35.343371 edgegap_scheduling-1.0.1/edgegap_scheduling/_runner.py
--rw-r--r--   0        0        0     3855 2024-04-29 18:21:35.343371 edgegap_scheduling-1.0.1/edgegap_scheduling/_scheduler.py
--rw-r--r--   0        0        0     1025 2024-04-29 18:21:35.343371 edgegap_scheduling-1.0.1/edgegap_scheduling/_signature.py
--rw-r--r--   0        0        0      482 2024-04-29 18:21:35.343371 edgegap_scheduling-1.0.1/edgegap_scheduling/_singleton.py
--rw-r--r--   0        0        0     1233 2024-04-29 18:21:35.343371 edgegap_scheduling-1.0.1/edgegap_scheduling/_sleep.py
--rw-r--r--   0        0        0      188 2024-04-29 18:21:35.343371 edgegap_scheduling-1.0.1/edgegap_scheduling/_state.py
--rw-r--r--   0        0        0     2780 2024-04-29 18:21:35.343371 edgegap_scheduling-1.0.1/edgegap_scheduling/_task.py
--rw-r--r--   0        0        0      132 2024-04-29 18:21:35.343371 edgegap_scheduling-1.0.1/edgegap_scheduling/errors/__init__.py
--rw-r--r--   0        0        0      103 2024-04-29 18:21:35.343371 edgegap_scheduling-1.0.1/edgegap_scheduling/errors/_errors.py
--rw-r--r--   0        0        0      501 2024-04-29 18:21:53.767516 edgegap_scheduling-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 edgegap_scheduling-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 18:23:33.441036 edgegap_scheduling-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2164 2024-04-29 18:23:33.441036 edgegap_scheduling-1.0.2/README.md
+-rw-r--r--   0        0        0      280 2024-04-29 18:23:33.441036 edgegap_scheduling-1.0.2/edgegap_scheduling/__init__.py
+-rw-r--r--   0        0        0      128 2024-04-29 18:23:33.441036 edgegap_scheduling-1.0.2/edgegap_scheduling/_depends.py
+-rw-r--r--   0        0        0     3389 2024-04-29 18:23:33.441036 edgegap_scheduling-1.0.2/edgegap_scheduling/_runner.py
+-rw-r--r--   0        0        0     3855 2024-04-29 18:23:33.441036 edgegap_scheduling-1.0.2/edgegap_scheduling/_scheduler.py
+-rw-r--r--   0        0        0     1025 2024-04-29 18:23:33.441036 edgegap_scheduling-1.0.2/edgegap_scheduling/_signature.py
+-rw-r--r--   0        0        0      482 2024-04-29 18:23:33.441036 edgegap_scheduling-1.0.2/edgegap_scheduling/_singleton.py
+-rw-r--r--   0        0        0     1233 2024-04-29 18:23:33.441036 edgegap_scheduling-1.0.2/edgegap_scheduling/_sleep.py
+-rw-r--r--   0        0        0      188 2024-04-29 18:23:33.441036 edgegap_scheduling-1.0.2/edgegap_scheduling/_state.py
+-rw-r--r--   0        0        0     2780 2024-04-29 18:23:33.441036 edgegap_scheduling-1.0.2/edgegap_scheduling/_task.py
+-rw-r--r--   0        0        0      132 2024-04-29 18:23:33.441036 edgegap_scheduling-1.0.2/edgegap_scheduling/errors/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-29 18:23:33.441036 edgegap_scheduling-1.0.2/edgegap_scheduling/errors/_errors.py
+-rw-r--r--   0        0        0      501 2024-04-29 18:24:03.389178 edgegap_scheduling-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 edgegap_scheduling-1.0.2/PKG-INFO
```

### Comparing `edgegap_scheduling-1.0.1/LICENSE` & `edgegap_scheduling-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.0.1/README.md` & `edgegap_scheduling-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.0.1/edgegap_scheduling/_runner.py` & `edgegap_scheduling-1.0.2/edgegap_scheduling/_runner.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.0.1/edgegap_scheduling/_scheduler.py` & `edgegap_scheduling-1.0.2/edgegap_scheduling/_scheduler.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.0.1/edgegap_scheduling/_signature.py` & `edgegap_scheduling-1.0.2/edgegap_scheduling/_signature.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.0.1/edgegap_scheduling/_sleep.py` & `edgegap_scheduling-1.0.2/edgegap_scheduling/_sleep.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.0.1/edgegap_scheduling/_task.py` & `edgegap_scheduling-1.0.2/edgegap_scheduling/_task.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.0.1/PKG-INFO` & `edgegap_scheduling-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: edgegap-scheduling
-Version: 1.0.1
+Version: 1.0.2
 Summary: The Edgegap Scheduling library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: edgegap-logging (>=0.1.2,<0.2.0)
+Requires-Dist: edgegap-logging (>=1.0.0,<2.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pytimeparse (>=1.1.8,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Edgegap Scheduling Library
 
 This is the README for the Edgegap Scheduling Helper, which is part of the Edgegap suite of helpers.
```

