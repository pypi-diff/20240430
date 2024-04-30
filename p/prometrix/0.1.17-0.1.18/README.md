# Comparing `tmp/prometrix-0.1.17.tar.gz` & `tmp/prometrix-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometrix-0.1.17.tar", max compression
+gzip compressed data, was "prometrix-0.1.18.tar", max compression
```

## Comparing `prometrix-0.1.17.tar` & `prometrix-0.1.18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-07-31 10:33:26.887864 prometrix-0.1.17/LICENSE.md
--rw-r--r--   0        0        0     5985 2024-03-17 11:02:19.154214 prometrix-0.1.17/README.md
--rw-r--r--   0        0        0      963 2023-08-01 11:27:45.325158 prometrix-0.1.17/prometrix/__init__.py
--rw-r--r--   0        0        0     3053 2023-08-01 11:27:45.322610 prometrix-0.1.17/prometrix/auth.py
--rw-r--r--   0        0        0     5466 2023-08-01 11:28:09.811185 prometrix-0.1.17/prometrix/connect/__pycache__/aws_connect.cpython-39.pyc
--rw-r--r--   0        0        0     5510 2023-08-01 11:28:09.824570 prometrix-0.1.17/prometrix/connect/__pycache__/custom_connect.cpython-39.pyc
--rw-r--r--   0        0        0     6428 2024-03-17 11:02:19.153414 prometrix-0.1.17/prometrix/connect/aws_connect.py
--rw-r--r--   0        0        0     8496 2024-03-17 11:02:19.153488 prometrix-0.1.17/prometrix/connect/custom_connect.py
--rw-r--r--   0        0        0      660 2023-07-31 08:10:29.276369 prometrix-0.1.17/prometrix/exceptions.py
--rw-r--r--   0        0        0     2386 2023-08-01 11:28:09.803615 prometrix-0.1.17/prometrix/models/__pycache__/prometheus_config.cpython-39.pyc
--rw-r--r--   0        0        0     4024 2023-07-31 08:32:22.473137 prometrix-0.1.17/prometrix/models/__pycache__/prometheus_result.cpython-39.pyc
--rw-r--r--   0        0        0     1982 2023-08-01 11:27:45.200857 prometrix-0.1.17/prometrix/models/prometheus_config.py
--rw-r--r--   0        0        0     4356 2023-10-02 10:28:53.355097 prometrix-0.1.17/prometrix/models/prometheus_result.py
--rw-r--r--   0        0        0     1730 2024-03-17 11:02:19.154756 prometrix-0.1.17/prometrix/utils.py
--rw-r--r--   0        0        0      826 2024-04-08 11:08:56.244103 prometrix-0.1.17/pyproject.toml
--rw-r--r--   0        0        0     6780 1970-01-01 00:00:00.000000 prometrix-0.1.17/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-31 10:33:26.887864 prometrix-0.1.18/LICENSE.md
+-rw-r--r--   0        0        0     5985 2024-03-17 11:02:19.154214 prometrix-0.1.18/README.md
+-rw-r--r--   0        0        0      963 2023-08-01 11:27:45.325158 prometrix-0.1.18/prometrix/__init__.py
+-rw-r--r--   0        0        0     3053 2023-08-01 11:27:45.322610 prometrix-0.1.18/prometrix/auth.py
+-rw-r--r--   0        0        0     5466 2023-08-01 11:28:09.811185 prometrix-0.1.18/prometrix/connect/__pycache__/aws_connect.cpython-39.pyc
+-rw-r--r--   0        0        0     5510 2023-08-01 11:28:09.824570 prometrix-0.1.18/prometrix/connect/__pycache__/custom_connect.cpython-39.pyc
+-rw-r--r--   0        0        0     6428 2024-03-17 11:02:19.153414 prometrix-0.1.18/prometrix/connect/aws_connect.py
+-rw-r--r--   0        0        0     8496 2024-03-17 11:02:19.153488 prometrix-0.1.18/prometrix/connect/custom_connect.py
+-rw-r--r--   0        0        0      660 2023-07-31 08:10:29.276369 prometrix-0.1.18/prometrix/exceptions.py
+-rw-r--r--   0        0        0     2386 2023-08-01 11:28:09.803615 prometrix-0.1.18/prometrix/models/__pycache__/prometheus_config.cpython-39.pyc
+-rw-r--r--   0        0        0     4024 2023-07-31 08:32:22.473137 prometrix-0.1.18/prometrix/models/__pycache__/prometheus_result.cpython-39.pyc
+-rw-r--r--   0        0        0     2024 2024-04-30 06:29:23.600575 prometrix-0.1.18/prometrix/models/prometheus_config.py
+-rw-r--r--   0        0        0     4384 2024-04-30 06:29:23.600759 prometrix-0.1.18/prometrix/models/prometheus_result.py
+-rw-r--r--   0        0        0     1730 2024-03-17 11:02:19.154756 prometrix-0.1.18/prometrix/utils.py
+-rw-r--r--   0        0        0      826 2024-04-30 06:29:30.920378 prometrix-0.1.18/pyproject.toml
+-rw-r--r--   0        0        0     6831 1970-01-01 00:00:00.000000 prometrix-0.1.18/PKG-INFO
```

### Comparing `prometrix-0.1.17/LICENSE.md` & `prometrix-0.1.18/LICENSE.md`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.17/README.md` & `prometrix-0.1.18/README.md`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.17/prometrix/__init__.py` & `prometrix-0.1.18/prometrix/__init__.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.17/prometrix/auth.py` & `prometrix-0.1.18/prometrix/auth.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.17/prometrix/connect/__pycache__/aws_connect.cpython-39.pyc` & `prometrix-0.1.18/prometrix/connect/__pycache__/aws_connect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.17/prometrix/connect/__pycache__/custom_connect.cpython-39.pyc` & `prometrix-0.1.18/prometrix/connect/__pycache__/custom_connect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.17/prometrix/connect/aws_connect.py` & `prometrix-0.1.18/prometrix/connect/aws_connect.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.17/prometrix/connect/custom_connect.py` & `prometrix-0.1.18/prometrix/connect/custom_connect.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.17/prometrix/exceptions.py` & `prometrix-0.1.18/prometrix/exceptions.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.17/prometrix/models/__pycache__/prometheus_config.cpython-39.pyc` & `prometrix-0.1.18/prometrix/models/__pycache__/prometheus_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.17/prometrix/models/__pycache__/prometheus_result.cpython-39.pyc` & `prometrix-0.1.18/prometrix/models/__pycache__/prometheus_result.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.17/prometrix/models/prometheus_config.py` & `prometrix-0.1.18/prometrix/models/prometheus_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 
 class PrometheusConfig(BaseModel):
     url: str
     disable_ssl: bool = False
     headers: Dict[str, str] = {}
     prometheus_auth: Optional[SecretStr] = None
-    prometheus_url_query_string: Optional[str]
-    additional_labels: Optional[Dict[str, str]]
+    prometheus_url_query_string: Optional[str] = None
+    additional_labels: Optional[Dict[str, str]] = None
     supported_apis: List[PrometheusApis] = [
         PrometheusApis.QUERY,
         PrometheusApis.QUERY_RANGE,
         PrometheusApis.LABELS,
         PrometheusApis.FLAGS,
     ]
 
@@ -59,15 +59,15 @@
 
 # Does not support labels according to the docs, See below for apis
 # https://learn.microsoft.com/en-us/azure/azure-monitor/essentials/prometheus-api-promql#supported-apis
 class AzurePrometheusConfig(PrometheusConfig):
     azure_resource: str
     azure_metadata_endpoint: str
     azure_token_endpoint: str
-    azure_use_managed_id: Optional[str]
-    azure_client_id: Optional[str]
-    azure_tenant_id: Optional[str]
-    azure_client_secret: Optional[str]
+    azure_use_managed_id: Optional[str] = None
+    azure_client_id: Optional[str] = None
+    azure_tenant_id: Optional[str] = None
+    azure_client_secret: Optional[str] = None
     supported_apis: List[PrometheusApis] = [
         PrometheusApis.QUERY,
         PrometheusApis.QUERY_RANGE,
     ]
```

### Comparing `prometrix-0.1.17/prometrix/models/prometheus_result.py` & `prometrix-0.1.18/prometrix/models/prometheus_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,18 +66,18 @@
     :var string_result:  a string of the query result, if the var result_type is "string"
 
     :raises:
         (Exception) Raises an Exception in the case that there is an issue with the resultType and result not matching
     """
 
     result_type: str
-    vector_result: Optional[List[PrometheusVector]]
-    series_list_result: Optional[List[PrometheusSeries]]
-    scalar_result: Optional[PrometheusScalarValue]
-    string_result: Optional[str]
+    vector_result: Optional[List[PrometheusVector]] = None
+    series_list_result: Optional[List[PrometheusSeries]] = None
+    scalar_result: Optional[PrometheusScalarValue] = None
+    string_result: Optional[str] = None
 
     def __init__(self, data):
         result = data.get("result", None)
         result_type = data.get("resultType", None)
         vector_result = None
         series_list_result = None
         scalar_result = None
```

### Comparing `prometrix-0.1.17/prometrix/utils.py` & `prometrix-0.1.18/prometrix/utils.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.17/pyproject.toml` & `prometrix-0.1.18/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "prometrix"
-version = "0.1.17"
+version = "0.1.18"
 authors = ["Avi Kotlicky <avi@robusta.dev>"]
 readme = "README.md"
 packages = [{include = "prometrix"}]
 description = "A Python Prometheus client for all Prometheus instances."
 
 [project.urls]
 "Homepage" = "https://github.com/robusta-dev/prometrix"
 "Bug Tracker" = "https://github.com/robusta-dev/prometrix/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = "^1.28.15"
 botocore = "^1.31.15"
-pydantic = "^1.8.1"
+pydantic = "^2.7.0"
 prometheus-api-client = "^0.5.3"
 pillow = "^10.3.0" # added to Pin transitive dependency, not needed directly
 fonttools = "^4.43.0" # added to Pin transitive dependency, not needed directly
 urllib3 = "^1.26.18" # added to Pin transitive dependency, not needed directly
 
 
 [build-system]
```

### Comparing `prometrix-0.1.17/PKG-INFO` & `prometrix-0.1.18/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: prometrix
-Version: 0.1.17
+Version: 0.1.18
 Summary: A Python Prometheus client for all Prometheus instances.
 Author: Avi Kotlicky
 Author-email: avi@robusta.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.28.15,<2.0.0)
 Requires-Dist: botocore (>=1.31.15,<2.0.0)
 Requires-Dist: fonttools (>=4.43.0,<5.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: prometheus-api-client (>=0.5.3,<0.6.0)
-Requires-Dist: pydantic (>=1.8.1,<2.0.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.18,<2.0.0)
 Description-Content-Type: text/markdown
 
 Prometrix - Unified Prometheus Client
 ======================================================
 
 Overview
```

