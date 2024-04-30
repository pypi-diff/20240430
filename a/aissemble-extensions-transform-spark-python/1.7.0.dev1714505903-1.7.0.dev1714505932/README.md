# Comparing `tmp/aissemble_extensions_transform_spark_python-1.7.0.dev1714505903.tar.gz` & `tmp/aissemble_extensions_transform_spark_python-1.7.0.dev1714505932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_extensions_transform_spark_python-1.7.0.dev1714505903.tar", max compression
+gzip compressed data, was "aissemble_extensions_transform_spark_python-1.7.0.dev1714505932.tar", max compression
```

## Comparing `aissemble_extensions_transform_spark_python-1.7.0.dev1714505903.tar` & `aissemble_extensions_transform_spark_python-1.7.0.dev1714505932.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     9580 2024-04-30 19:37:18.046814 aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/LICENSE
--rw-r--r--   0        0        0        0 2024-04-30 19:23:29.265274 aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/README.md
--rw-r--r--   0        0        0      982 2024-04-30 19:38:24.048862 aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/pyproject.toml
--rw-r--r--   0        0        0      248 2024-04-30 19:23:29.265274 aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/src/data_transform_spark/__init__.py
--rw-r--r--   0        0        0     2975 2024-04-30 19:23:29.265274 aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/src/data_transform_spark/data_transformer.py
--rw-r--r--   0        0        0      307 2024-04-30 19:23:29.265274 aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/src/data_transform_spark/mediator/__init__.py
--rw-r--r--   0        0        0     1580 2024-04-30 19:23:29.265274 aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/src/data_transform_spark/mediator/abstract_dataset_mediator.py
--rw-r--r--   0        0        0     1050 2024-04-30 19:23:29.265274 aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/src/data_transform_spark/mediator/dataset_logger.py
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-04-30 19:37:48.725374 aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-30 19:23:29.227569 aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/README.md
+-rw-r--r--   0        0        0      982 2024-04-30 19:38:52.613728 aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/pyproject.toml
+-rw-r--r--   0        0        0      248 2024-04-30 19:23:29.227569 aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/src/data_transform_spark/__init__.py
+-rw-r--r--   0        0        0     2975 2024-04-30 19:23:29.227569 aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/src/data_transform_spark/data_transformer.py
+-rw-r--r--   0        0        0      307 2024-04-30 19:23:29.227569 aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/src/data_transform_spark/mediator/__init__.py
+-rw-r--r--   0        0        0     1580 2024-04-30 19:23:29.227569 aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/src/data_transform_spark/mediator/abstract_dataset_mediator.py
+-rw-r--r--   0        0        0     1050 2024-04-30 19:23:29.227569 aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/src/data_transform_spark/mediator/dataset_logger.py
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/PKG-INFO
```

### Comparing `aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/LICENSE` & `aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/pyproject.toml` & `aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-extensions-transform-spark-python"
-version = "1.7.0.dev1714505903"
+version = "1.7.0.dev1714505932"
 description = "Contains the core Python implementation of data transform for Spark"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "data_transform_spark", from="src"}
 ]
```

### Comparing `aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/src/data_transform_spark/data_transformer.py` & `aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/src/data_transform_spark/data_transformer.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/src/data_transform_spark/mediator/abstract_dataset_mediator.py` & `aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/src/data_transform_spark/mediator/abstract_dataset_mediator.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/src/data_transform_spark/mediator/dataset_logger.py` & `aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/src/data_transform_spark/mediator/dataset_logger.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_transform_spark_python-1.7.0.dev1714505903/PKG-INFO` & `aissemble_extensions_transform_spark_python-1.7.0.dev1714505932/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-extensions-transform-spark-python
-Version: 1.7.0.dev1714505903
+Version: 1.7.0.dev1714505932
 Summary: Contains the core Python implementation of data transform for Spark
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aissemble-foundation-core-python (==1.7.0.*)
```

