# Comparing `tmp/ng_data_pipelines_sdk-0.4.2.tar.gz` & `tmp/ng_data_pipelines_sdk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.4.2.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.5.0.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.4.2.tar` & `ng_data_pipelines_sdk-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/README.md
--rw-r--r--   0        0        0        0 2024-04-27 19:06:03.413718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    26500 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    15377 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     4648 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     1453 2024-04-27 19:06:03.389718 ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      672 2024-04-27 19:06:03.391718 ng_data_pipelines_sdk-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-04-30 20:39:04.002808 ng_data_pipelines_sdk-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 20:39:04.025808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-04-30 20:39:04.003808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-04-30 20:39:04.003808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    26500 2024-04-30 20:39:04.003808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    15420 2024-04-30 20:39:04.003808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     4648 2024-04-30 20:39:04.003808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     1453 2024-04-30 20:39:04.003808 ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      672 2024-04-30 20:39:04.004808 ng_data_pipelines_sdk-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.5.0/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     env: Env
     layer: Optional[Layer] = None
     ng_prefix: str = "ng"
     bucket_name: Optional[str] = None
 
     @model_validator(mode="before")
     def set_bucket_name_if_not_provided(cls, data):
-        layer = data.get("layer").value
+        layer = data.get("layer").value if data.get("layer") is not None else None
         env = data.get("env").value
         ng_prefix = data.get("ng_prefix", "ng")
         bucket_name = data.get("bucket_name")
 
         if bucket_name is None:
             if layer is None:
                 raise ValueError(
```

### Comparing `ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.4.2/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.5.0/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.4.2/pyproject.toml` & `ng_data_pipelines_sdk-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.4.2"
+version = "0.5.0"
 description = "A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-0.4.2/PKG-INFO` & `ng_data_pipelines_sdk-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.4.2
+Version: 0.5.0
 Summary: A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

