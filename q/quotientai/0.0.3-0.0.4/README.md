# Comparing `tmp/quotientai-0.0.3.tar.gz` & `tmp/quotientai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quotientai-0.0.3.tar", max compression
+gzip compressed data, was "quotientai-0.0.4.tar", max compression
```

## Comparing `quotientai-0.0.3.tar` & `quotientai-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11345 2024-04-29 14:35:38.397110 quotientai-0.0.3/LICENSE
--rw-r--r--   0        0        0      390 2024-04-29 14:35:38.397110 quotientai-0.0.3/README.md
--rw-r--r--   0        0        0     1011 2024-04-29 14:35:38.397110 quotientai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      288 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/__init__.py
--rw-r--r--   0        0        0       47 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/cli/__init__.py
--rw-r--r--   0        0        0    18956 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/cli/entrypoint.py
--rw-r--r--   0        0        0     7961 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/cli/format.py
--rw-r--r--   0        0        0    41452 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/client.py
--rw-r--r--   0        0        0      181 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/exceptions.py
--rw-r--r--   0        0        0     4280 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/utils.py
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 quotientai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-04-30 18:46:08.552628 quotientai-0.0.4/LICENSE
+-rw-r--r--   0        0        0      390 2024-04-30 18:46:08.552628 quotientai-0.0.4/README.md
+-rw-r--r--   0        0        0     1011 2024-04-30 18:46:08.552628 quotientai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-04-30 18:46:08.552628 quotientai-0.0.4/quotientai/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-30 18:46:08.552628 quotientai-0.0.4/quotientai/cli/__init__.py
+-rw-r--r--   0        0        0    18932 2024-04-30 18:46:08.552628 quotientai-0.0.4/quotientai/cli/entrypoint.py
+-rw-r--r--   0        0        0     7961 2024-04-30 18:46:08.552628 quotientai-0.0.4/quotientai/cli/format.py
+-rw-r--r--   0        0        0    41490 2024-04-30 18:46:08.552628 quotientai-0.0.4/quotientai/client.py
+-rw-r--r--   0        0        0      181 2024-04-30 18:46:08.552628 quotientai-0.0.4/quotientai/exceptions.py
+-rw-r--r--   0        0        0     4280 2024-04-30 18:46:08.552628 quotientai-0.0.4/quotientai/utils.py
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 quotientai-0.0.4/PKG-INFO
```

### Comparing `quotientai-0.0.3/LICENSE` & `quotientai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quotientai-0.0.3/pyproject.toml` & `quotientai-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quotientai"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     "Vic Weiss <vic@quotientai.co>",
     "Freddie Vargus <freddie@quotientai.co>",
     "Allison Kunz <allison@quotient.co>",
 ]
 description = "CLI for evaluating large language models with Quotient"
 readme = "README.md"
```

### Comparing `quotientai-0.0.3/quotientai/cli/entrypoint.py` & `quotientai-0.0.4/quotientai/cli/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,16 +183,16 @@
             config = json.load(file)
 
         # Extract the necessary fields from the JSON configuration
         name = config["name"]
         endpoint = config["request"]["url"]
         description = config["description"]
         method = config["request"]["method"]
-        headers = json.dumps(config["request"]["headers"])
-        payload_template = json.dumps(config["request"]["payloadTemplate"])
+        headers = config["request"]["headers"]
+        payload_template = config["request"]["payloadTemplate"]
         path_to_data = config["responseParsing"]["pathToData"]
         path_to_context = config["responseParsing"].get("pathToContext", None)
 
         # Instantiate your client and call create_model with the extracted fields
         client = QuotientClient()
         client.create_model(
             name=name,
```

### Comparing `quotientai-0.0.3/quotientai/cli/format.py` & `quotientai-0.0.4/quotientai/cli/format.py`

 * *Files identical despite different names*

### Comparing `quotientai-0.0.3/quotientai/client.py` & `quotientai-0.0.4/quotientai/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import mimetypes
 import os
 import time
 from datetime import datetime
 
 import requests
 from postgrest import APIError, SyncPostgrestClient
@@ -303,24 +304,24 @@
     @require_api_key
     def create_model(
         self,
         name: str,
         endpoint: str,
         description: str,
         method: str,
-        headers: str,
-        payload_template: str,
+        headers: dict,
+        payload_template: dict,
         path_to_data: str,
         path_to_context: str,
         model_type: str = "UserHostedModel",
     ) -> dict:
         external_model_config = {
             "method": method,
-            "headers": headers,
-            "payload_template": payload_template,
+            "headers": json.dumps(headers),
+            "payload_template": json.dumps(payload_template),
             "path_to_data": path_to_data,
             "path_to_context": path_to_context,
             "created_at": datetime.utcnow().isoformat(),
         }
 
         model = {
             "name": name,
```

### Comparing `quotientai-0.0.3/quotientai/utils.py` & `quotientai-0.0.4/quotientai/utils.py`

 * *Files identical despite different names*

### Comparing `quotientai-0.0.3/PKG-INFO` & `quotientai-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quotientai
-Version: 0.0.3
+Version: 0.0.4
 Summary: CLI for evaluating large language models with Quotient
 License: Apache-2.0
 Keywords: quotient,evaluation,llms,machine learning,ai
 Author: Vic Weiss
 Author-email: vic@quotientai.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

