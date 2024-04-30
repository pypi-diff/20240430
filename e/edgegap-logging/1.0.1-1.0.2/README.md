# Comparing `tmp/edgegap_logging-1.0.1.tar.gz` & `tmp/edgegap_logging-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_logging-1.0.1.tar", max compression
+gzip compressed data, was "edgegap_logging-1.0.2.tar", max compression
```

## Comparing `edgegap_logging-1.0.1.tar` & `edgegap_logging-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1993 2024-04-29 18:21:35.343371 edgegap_logging-1.0.1/LICENSE
--rw-r--r--   0        0        0     2216 2024-04-29 18:21:35.343371 edgegap_logging-1.0.1/README.md
--rw-r--r--   0        0        0      221 2024-04-29 18:21:35.343371 edgegap_logging-1.0.1/edgegap_logging/__init__.py
--rw-r--r--   0        0        0      417 2024-04-29 18:21:35.343371 edgegap_logging-1.0.1/edgegap_logging/_format.py
--rw-r--r--   0        0        0     4077 2024-04-29 18:21:35.343371 edgegap_logging-1.0.1/edgegap_logging/_logging.py
--rw-r--r--   0        0        0      494 2024-04-29 18:21:46.951462 edgegap_logging-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 edgegap_logging-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 18:23:33.441036 edgegap_logging-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2216 2024-04-29 18:23:33.441036 edgegap_logging-1.0.2/README.md
+-rw-r--r--   0        0        0      221 2024-04-29 18:23:33.441036 edgegap_logging-1.0.2/edgegap_logging/__init__.py
+-rw-r--r--   0        0        0      417 2024-04-29 18:23:33.441036 edgegap_logging-1.0.2/edgegap_logging/_format.py
+-rw-r--r--   0        0        0     4077 2024-04-29 18:23:33.441036 edgegap_logging-1.0.2/edgegap_logging/_logging.py
+-rw-r--r--   0        0        0      494 2024-04-29 18:23:41.117072 edgegap_logging-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 edgegap_logging-1.0.2/PKG-INFO
```

### Comparing `edgegap_logging-1.0.1/LICENSE` & `edgegap_logging-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.0.1/README.md` & `edgegap_logging-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.0.1/edgegap_logging/_logging.py` & `edgegap_logging-1.0.2/edgegap_logging/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.0.1/PKG-INFO` & `edgegap_logging-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-logging
-Version: 1.0.1
+Version: 1.0.2
 Summary: The Edgegap Logging library includes various tools and helpers for interacting with Standard Logging Formatter and Colored Logs. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

