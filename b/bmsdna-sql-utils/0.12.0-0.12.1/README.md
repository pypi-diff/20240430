# Comparing `tmp/bmsdna_sql_utils-0.12.0.tar.gz` & `tmp/bmsdna_sql_utils-0.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_sql_utils-0.12.0.tar", max compression
+gzip compressed data, was "bmsdna_sql_utils-0.12.1.tar", max compression
```

## Comparing `bmsdna_sql_utils-0.12.0.tar` & `bmsdna_sql_utils-0.12.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0      255 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/README.md
--rw-r--r--   0        0        0        0 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/__init__.py
--rw-r--r--   0        0        0      382 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/__init__.py
--rw-r--r--   0        0        0     3133 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/async_db_helper.py
--rw-r--r--   0        0        0     1169 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/case_preserving_set.py
--rw-r--r--   0        0        0     3529 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_helper.py
--rw-r--r--   0        0        0        0 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/__init__.py
--rw-r--r--   0        0        0     2113 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/db_logging.py
--rw-r--r--   0        0        0     5382 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/delta_polars_source.py
--rw-r--r--   0        0        0     6060 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/delta_source.py
--rw-r--r--   0        0        0    26081 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/fill_table.py
--rw-r--r--   0        0        0     2116 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/json_insert.py
--rw-r--r--   0        0        0     5178 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/lake_source.py
--rw-r--r--   0        0        0     1754 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/meta_sql_store.py
--rw-r--r--   0        0        0     1481 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/odbc_insert.py
--rw-r--r--   0        0        0     1736 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/source.py
--rw-r--r--   0        0        0      739 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/sql_utils.py
--rw-r--r--   0        0        0    15908 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/sqlschema.py
--rw-r--r--   0        0        0     1258 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/dbapi.py
--rw-r--r--   0        0        0     1332 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/integrity_check.py
--rw-r--r--   0        0        0      199 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/lake/__init__.py
--rw-r--r--   0        0        0     2423 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/lake/lake_meta.py
--rw-r--r--   0        0        0      822 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/lake/type_fromarrow.py
--rw-r--r--   0        0        0      884 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/lake/types.py
--rw-r--r--   0        0        0     5671 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/metadata/__init__.py
--rw-r--r--   0        0        0     4024 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/query.py
--rw-r--r--   0        0        0     2759 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/query_generation.py
--rw-r--r--   0        0        0     2619 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/result.py
--rw-r--r--   0        0        0     4026 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/server_info.py
--rw-r--r--   0        0        0     1078 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/sql_gen.py
--rw-r--r--   0        0        0     1754 2024-04-29 13:57:26.020626 bmsdna_sql_utils-0.12.0/pyproject.toml
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.12.0/PKG-INFO
+-rw-r--r--   0        0        0      255 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/bmsdna/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/__init__.py
+-rw-r--r--   0        0        0     3133 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/async_db_helper.py
+-rw-r--r--   0        0        0     1169 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/case_preserving_set.py
+-rw-r--r--   0        0        0     3529 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_helper.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/__init__.py
+-rw-r--r--   0        0        0     2113 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/db_logging.py
+-rw-r--r--   0        0        0     5382 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/delta_polars_source.py
+-rw-r--r--   0        0        0     6060 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/delta_source.py
+-rw-r--r--   0        0        0    26081 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/fill_table.py
+-rw-r--r--   0        0        0     2116 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/json_insert.py
+-rw-r--r--   0        0        0     5178 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/lake_source.py
+-rw-r--r--   0        0        0     1754 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/meta_sql_store.py
+-rw-r--r--   0        0        0     1481 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/odbc_insert.py
+-rw-r--r--   0        0        0     1736 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/source.py
+-rw-r--r--   0        0        0     3651 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/source_spark.py
+-rw-r--r--   0        0        0      739 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/sql_utils.py
+-rw-r--r--   0        0        0    15908 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/sqlschema.py
+-rw-r--r--   0        0        0     1258 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/dbapi.py
+-rw-r--r--   0        0        0     1332 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/integrity_check.py
+-rw-r--r--   0        0        0      199 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/__init__.py
+-rw-r--r--   0        0        0     2423 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/lake_meta.py
+-rw-r--r--   0        0        0      822 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/type_fromarrow.py
+-rw-r--r--   0        0        0      884 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/types.py
+-rw-r--r--   0        0        0     5671 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/metadata/__init__.py
+-rw-r--r--   0        0        0     4024 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/query.py
+-rw-r--r--   0        0        0     2759 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/query_generation.py
+-rw-r--r--   0        0        0     2619 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/result.py
+-rw-r--r--   0        0        0     4026 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/server_info.py
+-rw-r--r--   0        0        0     1078 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/sql_gen.py
+-rw-r--r--   0        0        0     1774 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/pyproject.toml
+-rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.12.1/PKG-INFO
```

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/async_db_helper.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/async_db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/case_preserving_set.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/case_preserving_set.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_helper.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/db_logging.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/db_logging.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/delta_polars_source.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/delta_polars_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/delta_source.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/delta_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/fill_table.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/fill_table.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/json_insert.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/json_insert.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/lake_source.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/lake_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/meta_sql_store.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/meta_sql_store.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/odbc_insert.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/odbc_insert.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/source.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/sql_utils.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/sql_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/sqlschema.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/sqlschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/dbapi.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/dbapi.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/integrity_check.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/integrity_check.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/lake/lake_meta.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/lake_meta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/lake/type_fromarrow.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/type_fromarrow.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/lake/types.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/metadata/__init__.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/query.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/query.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/query_generation.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/query_generation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/result.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/result.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/server_info.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/server_info.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/sql_gen.py` & `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/sql_gen.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.0/pyproject.toml` & `bmsdna_sql_utils-0.12.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-sql-utils"
-version = "0.12.0"
+version = "0.12.1"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 readme = "README.md"
 packages = [{ include = "bmsdna" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -28,14 +28,15 @@
 pyodbc = { version = ">=4.0.0" }
 aioodbc = { version = "^0.5.0" }
 python-tds = { version = "^1.13.0" }
 pydantic = ">=1.10.0"
 isort = "^5.12.0"
 pycln = "^2.4.0"
 sqlglot = ">=20.0.0"
+pyspark = "^3.5.1"
 
 
 [tool.poetry.group.test.dependencies]
 pytest-asyncio = "^0.23.5"
 pytest = "^7.4.3"
 pytest-order = "^1.2.0"
 docker = "^7.0.0"
```

### Comparing `bmsdna_sql_utils-0.12.0/PKG-INFO` & `bmsdna_sql_utils-0.12.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-sql-utils
-Version: 0.12.0
+Version: 0.12.1
 Summary: 
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

