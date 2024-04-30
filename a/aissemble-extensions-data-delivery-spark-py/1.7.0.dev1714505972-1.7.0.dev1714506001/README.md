# Comparing `tmp/aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972.tar.gz` & `tmp/aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972.tar", max compression
+gzip compressed data, was "aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001.tar", max compression
```

## Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972.tar` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     9580 2024-04-30 19:39:11.984902 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972/LICENSE
--rw-r--r--   0        0        0      118 2024-04-30 19:23:29.231274 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972/README.md
--rw-r--r--   0        0        0      650 2024-04-30 19:39:33.224921 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972/pyproject.toml
--rw-r--r--   0        0        0      205 2024-04-30 19:23:29.231274 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972/src/data_delivery_spark_py/__init__.py
--rw-r--r--   0        0        0      205 2024-04-30 19:23:29.231274 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972/src/data_delivery_spark_py/test_utils/__init__.py
--rw-r--r--   0        0        0     2822 2024-04-30 19:23:29.231274 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972/src/data_delivery_spark_py/test_utils/spark_session_manager.py
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-04-30 19:39:41.322493 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001/LICENSE
+-rw-r--r--   0        0        0      118 2024-04-30 19:23:29.197570 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001/README.md
+-rw-r--r--   0        0        0      650 2024-04-30 19:40:01.991969 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001/pyproject.toml
+-rw-r--r--   0        0        0      205 2024-04-30 19:23:29.197570 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001/src/data_delivery_spark_py/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-30 19:23:29.197570 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001/src/data_delivery_spark_py/test_utils/__init__.py
+-rw-r--r--   0        0        0     2822 2024-04-30 19:23:29.197570 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001/src/data_delivery_spark_py/test_utils/spark_session_manager.py
+-rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001/PKG-INFO
```

### Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972/LICENSE` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972/pyproject.toml` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-extensions-data-delivery-spark-py"
-version = "1.7.0.dev1714505972"
+version = "1.7.0.dev1714506001"
 description = "Contains the core Python functionality of data delivery for Spark"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "data_delivery_spark_py", from="src"},
 ]
```

### Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972/src/data_delivery_spark_py/test_utils/spark_session_manager.py` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001/src/data_delivery_spark_py/test_utils/spark_session_manager.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714505972/PKG-INFO` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714506001/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-extensions-data-delivery-spark-py
-Version: 1.7.0.dev1714505972
+Version: 1.7.0.dev1714506001
 Summary: Contains the core Python functionality of data delivery for Spark
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: krausening (>=19)
```

