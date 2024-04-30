# Comparing `tmp/airbyte_source_salesforce-2.5.6.tar.gz` & `tmp/airbyte_source_salesforce-2.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_salesforce-2.5.6.tar", max compression
+gzip compressed data, was "airbyte_source_salesforce-2.5.7.tar", max compression
```

## Comparing `airbyte_source_salesforce-2.5.6.tar` & `airbyte_source_salesforce-2.5.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4568 2024-04-19 20:53:45.000000 airbyte_source_salesforce-2.5.6/README.md
--rw-r--r--   0        0        0      826 2024-04-19 21:41:33.106400 airbyte_source_salesforce-2.5.6/pyproject.toml
--rw-r--r--   0        0        0      131 2024-04-19 20:53:45.000000 airbyte_source_salesforce-2.5.6/source_salesforce/__init__.py
--rw-r--r--   0        0        0    17451 2024-04-19 20:53:45.000000 airbyte_source_salesforce-2.5.6/source_salesforce/api.py
--rw-r--r--   0        0        0     1621 2024-04-19 20:53:45.000000 airbyte_source_salesforce-2.5.6/source_salesforce/availability_strategy.py
--rw-r--r--   0        0        0      808 2024-04-19 20:53:45.000000 airbyte_source_salesforce-2.5.6/source_salesforce/exceptions.py
--rw-r--r--   0        0        0     3946 2024-04-19 20:53:45.000000 airbyte_source_salesforce-2.5.6/source_salesforce/rate_limiting.py
--rw-r--r--   0        0        0     1619 2024-04-19 20:53:45.000000 airbyte_source_salesforce-2.5.6/source_salesforce/run.py
--rw-r--r--   0        0        0     9747 2024-04-19 20:53:45.000000 airbyte_source_salesforce-2.5.6/source_salesforce/schemas/Describe.json
--rw-r--r--   0        0        0    15502 2024-04-19 20:53:45.000000 airbyte_source_salesforce-2.5.6/source_salesforce/source.py
--rw-r--r--   0        0        0     4769 2024-04-19 20:53:45.000000 airbyte_source_salesforce-2.5.6/source_salesforce/spec.yaml
--rw-r--r--   0        0        0    41478 2024-04-19 20:53:45.000000 airbyte_source_salesforce-2.5.6/source_salesforce/streams.py
--rw-r--r--   0        0        0     1024 2024-04-19 20:53:45.000000 airbyte_source_salesforce-2.5.6/source_salesforce/utils.py
--rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.5.6/PKG-INFO
+-rw-r--r--   0        0        0     4568 2024-04-30 15:30:43.076023 airbyte_source_salesforce-2.5.7/README.md
+-rw-r--r--   0        0        0      830 2024-04-30 15:35:03.996412 airbyte_source_salesforce-2.5.7/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-04-30 15:30:43.076023 airbyte_source_salesforce-2.5.7/source_salesforce/__init__.py
+-rw-r--r--   0        0        0    17451 2024-04-30 15:30:43.076023 airbyte_source_salesforce-2.5.7/source_salesforce/api.py
+-rw-r--r--   0        0        0     1621 2024-04-30 15:30:43.076023 airbyte_source_salesforce-2.5.7/source_salesforce/availability_strategy.py
+-rw-r--r--   0        0        0      808 2024-04-30 15:30:43.076023 airbyte_source_salesforce-2.5.7/source_salesforce/exceptions.py
+-rw-r--r--   0        0        0     3946 2024-04-30 15:30:43.076023 airbyte_source_salesforce-2.5.7/source_salesforce/rate_limiting.py
+-rw-r--r--   0        0        0     1619 2024-04-30 15:30:43.076023 airbyte_source_salesforce-2.5.7/source_salesforce/run.py
+-rw-r--r--   0        0        0    17796 2024-04-30 15:30:43.076023 airbyte_source_salesforce-2.5.7/source_salesforce/schemas/Describe.json
+-rw-r--r--   0        0        0    15502 2024-04-30 15:30:43.076023 airbyte_source_salesforce-2.5.7/source_salesforce/source.py
+-rw-r--r--   0        0        0     4769 2024-04-30 15:30:43.076023 airbyte_source_salesforce-2.5.7/source_salesforce/spec.yaml
+-rw-r--r--   0        0        0    41478 2024-04-30 15:30:43.076023 airbyte_source_salesforce-2.5.7/source_salesforce/streams.py
+-rw-r--r--   0        0        0     1024 2024-04-30 15:30:43.076023 airbyte_source_salesforce-2.5.7/source_salesforce/utils.py
+-rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.5.7/PKG-INFO
```

### Comparing `airbyte_source_salesforce-2.5.6/README.md` & `airbyte_source_salesforce-2.5.7/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.6/pyproject.toml` & `airbyte_source_salesforce-2.5.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.5.6"
+version = "2.5.7"
 name = "airbyte-source-salesforce"
 description = "Source implementation for Salesforce."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
@@ -19,15 +19,15 @@
 packages = [
     { include = "source_salesforce" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 pandas = "2.2.1"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.83.1"
 
 [tool.poetry.scripts]
 source-salesforce = "source_salesforce.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest-mock = "^3.6"
 pytest = "^6.1"
```

### Comparing `airbyte_source_salesforce-2.5.6/source_salesforce/api.py` & `airbyte_source_salesforce-2.5.7/source_salesforce/api.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.6/source_salesforce/availability_strategy.py` & `airbyte_source_salesforce-2.5.7/source_salesforce/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.6/source_salesforce/exceptions.py` & `airbyte_source_salesforce-2.5.7/source_salesforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.6/source_salesforce/rate_limiting.py` & `airbyte_source_salesforce-2.5.7/source_salesforce/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.6/source_salesforce/run.py` & `airbyte_source_salesforce-2.5.7/source_salesforce/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.6/source_salesforce/source.py` & `airbyte_source_salesforce-2.5.7/source_salesforce/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.6/source_salesforce/spec.yaml` & `airbyte_source_salesforce-2.5.7/source_salesforce/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.6/source_salesforce/streams.py` & `airbyte_source_salesforce-2.5.7/source_salesforce/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.6/source_salesforce/utils.py` & `airbyte_source_salesforce-2.5.7/source_salesforce/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.6/PKG-INFO` & `airbyte_source_salesforce-2.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-salesforce
-Version: 2.5.6
+Version: 2.5.7
 Summary: Source implementation for Salesforce.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.83.1)
 Requires-Dist: pandas (==2.2.1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/salesforce
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Salesforce source connector
```

