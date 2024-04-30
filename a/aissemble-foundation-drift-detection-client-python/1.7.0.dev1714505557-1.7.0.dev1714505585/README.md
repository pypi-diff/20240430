# Comparing `tmp/aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557.tar.gz` & `tmp/aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557.tar", max compression
+gzip compressed data, was "aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585.tar", max compression
```

## Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557.tar` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     9580 2024-04-30 19:32:23.791559 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/LICENSE
--rw-r--r--   0        0        0        0 2024-04-30 19:23:29.279274 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/README.md
--rw-r--r--   0        0        0      661 2024-04-30 19:32:38.219580 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/pyproject.toml
--rw-r--r--   0        0        0      194 2024-04-30 19:23:29.279274 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/src/config/__init__.py
--rw-r--r--   0        0        0      672 2024-04-30 19:23:29.279274 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/src/config/rest_config.py
--rw-r--r--   0        0        0      194 2024-04-30 19:23:29.280274 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/src/drift/__init__.py
--rw-r--r--   0        0        0      194 2024-04-30 19:23:29.280274 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/src/drift/detection/__init__.py
--rw-r--r--   0        0        0      194 2024-04-30 19:23:29.280274 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/src/drift/detection/rest/__init__.py
--rw-r--r--   0        0        0      194 2024-04-30 19:23:29.280274 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/src/drift/detection/rest/client/__init__.py
--rw-r--r--   0        0        0     1755 2024-04-30 19:23:29.280274 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/src/drift/detection/rest/client/drift_rest_client.py
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-04-30 19:32:50.543074 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-30 19:23:29.247568 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/README.md
+-rw-r--r--   0        0        0      661 2024-04-30 19:33:06.282678 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/pyproject.toml
+-rw-r--r--   0        0        0      194 2024-04-30 19:23:29.247568 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/src/config/__init__.py
+-rw-r--r--   0        0        0      672 2024-04-30 19:23:29.247568 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/src/config/rest_config.py
+-rw-r--r--   0        0        0      194 2024-04-30 19:23:29.247568 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/src/drift/__init__.py
+-rw-r--r--   0        0        0      194 2024-04-30 19:23:29.247568 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/src/drift/detection/__init__.py
+-rw-r--r--   0        0        0      194 2024-04-30 19:23:29.247568 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/src/drift/detection/rest/__init__.py
+-rw-r--r--   0        0        0      194 2024-04-30 19:23:29.247568 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/src/drift/detection/rest/client/__init__.py
+-rw-r--r--   0        0        0     1755 2024-04-30 19:23:29.247568 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/src/drift/detection/rest/client/drift_rest_client.py
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/PKG-INFO
```

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/LICENSE` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/pyproject.toml` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-drift-detection-client-python"
-version = "1.7.0.dev1714505557"
+version = "1.7.0.dev1714505585"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "config", from = "src"},
     {include = "drift", from = "src"}
 ]
```

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/src/config/rest_config.py` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/src/config/rest_config.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/src/drift/detection/rest/client/drift_rest_client.py` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/src/drift/detection/rest/client/drift_rest_client.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505557/PKG-INFO` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714505585/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-drift-detection-client-python
-Version: 1.7.0.dev1714505557
+Version: 1.7.0.dev1714505585
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cryptography (>=42.0.4)
```

