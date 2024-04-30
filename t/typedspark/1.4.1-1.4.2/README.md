# Comparing `tmp/typedspark-1.4.1.tar.gz` & `tmp/typedspark-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedspark-1.4.1.tar", last modified: Sat Apr 13 08:03:22 2024, max compression
+gzip compressed data, was "typedspark-1.4.2.tar", last modified: Tue Apr 30 13:20:13 2024, max compression
```

## Comparing `typedspark-1.4.1.tar` & `typedspark-1.4.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:03:22.543548 typedspark-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-13 08:03:12.000000 typedspark-1.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-13 08:03:22.543548 typedspark-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-13 08:03:12.000000 typedspark-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-13 08:03:12.000000 typedspark-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 08:03:22.543548 typedspark-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-13 08:03:12.000000 typedspark-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:03:22.535548 typedspark-1.4.1/typedspark/
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:03:22.539548 typedspark-1.4.1/typedspark/_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_core/column.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_core/column_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_core/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_core/literaltype.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_core/validate_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:03:22.539548 typedspark-1.4.1/typedspark/_schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_schema/dlt_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_schema/get_schema_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_schema/get_schema_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_schema/structfield.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:03:22.539548 typedspark-1.4.1/typedspark/_transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_transforms/rename_duplicate_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_transforms/structtype_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_transforms/transform_to_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_transforms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:03:22.543548 typedspark-1.4.1/typedspark/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_utils/camelcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_utils/create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_utils/create_dataset_from_structtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_utils/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_utils/load_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/_utils/register_schema_to_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 08:03:12.000000 typedspark-1.4.1/typedspark/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:03:22.543548 typedspark-1.4.1/typedspark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-13 08:03:22.000000 typedspark-1.4.1/typedspark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-13 08:03:22.000000 typedspark-1.4.1/typedspark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 08:03:22.000000 typedspark-1.4.1/typedspark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-13 08:03:22.000000 typedspark-1.4.1/typedspark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-13 08:03:22.000000 typedspark-1.4.1/typedspark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:13.011392 typedspark-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 13:20:00.000000 typedspark-1.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-30 13:20:13.011392 typedspark-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-30 13:20:00.000000 typedspark-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-30 13:20:00.000000 typedspark-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:20:13.011392 typedspark-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-30 13:20:00.000000 typedspark-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:13.007393 typedspark-1.4.2/typedspark/
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:13.007393 typedspark-1.4.2/typedspark/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_core/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_core/column_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12728 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_core/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_core/literaltype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_core/validate_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:13.011392 typedspark-1.4.2/typedspark/_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_schema/dlt_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_schema/get_schema_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_schema/get_schema_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_schema/structfield.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:13.011392 typedspark-1.4.2/typedspark/_transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_transforms/rename_duplicate_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_transforms/structtype_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_transforms/transform_to_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_transforms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:13.011392 typedspark-1.4.2/typedspark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_utils/camelcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_utils/create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_utils/create_dataset_from_structtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_utils/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_utils/load_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/_utils/register_schema_to_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:00.000000 typedspark-1.4.2/typedspark/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:13.011392 typedspark-1.4.2/typedspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-30 13:20:12.000000 typedspark-1.4.2/typedspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-30 13:20:12.000000 typedspark-1.4.2/typedspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:20:12.000000 typedspark-1.4.2/typedspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 13:20:12.000000 typedspark-1.4.2/typedspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 13:20:12.000000 typedspark-1.4.2/typedspark.egg-info/top_level.txt
```

### Comparing `typedspark-1.4.1/LICENSE.txt` & `typedspark-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/PKG-INFO` & `typedspark-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.4.1
+Version: 1.4.2
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
```

### Comparing `typedspark-1.4.1/README.md` & `typedspark-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/pyproject.toml` & `typedspark-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/setup.py` & `typedspark-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/__init__.py` & `typedspark-1.4.2/typedspark/__init__.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_core/column.py` & `typedspark-1.4.2/typedspark/_core/column.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_core/column_meta.py` & `typedspark-1.4.2/typedspark/_core/column_meta.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_core/dataset.py` & `typedspark-1.4.2/typedspark/_core/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module containing classes and functions related to TypedSpark DataSets."""
 
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import Callable, Generic, List, Literal, Optional, Type, TypeVar, Union, cast, overload
 
+from pyspark import StorageLevel
 from pyspark.sql import Column as SparkColumn
 from pyspark.sql import DataFrame
 from typing_extensions import Concatenate, ParamSpec
 
 from typedspark._core.validate_schema import validate_schema
 from typedspark._schema.schema import Schema
 
@@ -56,14 +57,26 @@
     """The following functions are equivalent to their parents in ``DataFrame``, but since they
     don't affect the ``Schema``, we can add type annotations here. We're omitting docstrings,
     such that the docstring from the parent will appear."""
 
     def alias(self, alias: str) -> DataSet[_Implementation]:
         return DataSet[self._schema_annotations](super().alias(alias))  # type: ignore
 
+    def cache(self) -> DataSet[_Implementation]:  # pylint: disable=C0116
+        return DataSet[self._schema_annotations](super().cache())  # type: ignore
+
+    def persist(
+        self,
+        storageLevel: StorageLevel = (StorageLevel.MEMORY_AND_DISK_DESER),
+    ) -> DataSet[_Implementation]:
+        return DataSet[self._schema_annotations](super().persist(storageLevel))  # type: ignore
+
+    def unpersist(self, blocking: bool = False) -> DataSet[_Implementation]:
+        return DataSet[self._schema_annotations](super().unpersist(blocking))  # type: ignore
+
     def distinct(self) -> DataSet[_Implementation]:  # pylint: disable=C0116
         return DataSet[self._schema_annotations](super().distinct())  # type: ignore
 
     def filter(self, condition) -> DataSet[_Implementation]:  # pylint: disable=C0116
         return DataSet[self._schema_annotations](super().filter(condition))  # type: ignore
 
     @overload
@@ -216,14 +229,26 @@
     """The following functions are equivalent to their parents in ``DataSetImplements``. However,
     to support functions like ``functools.reduce(DataSet.unionByName, datasets)``, we also add them
     here. Unfortunately, this leads to some code redundancy, but we'll take that for granted."""
 
     def alias(self, alias: str) -> DataSet[_Schema]:
         return DataSet[self._schema_annotations](super().alias(alias))  # type: ignore
 
+    def cache(self) -> DataSet[_Schema]:  # pylint: disable=C0116
+        return DataSet[self._schema_annotations](super().cache())  # type: ignore
+
+    def persist(
+        self,
+        storageLevel: StorageLevel = (StorageLevel.MEMORY_AND_DISK_DESER),
+    ) -> DataSet[_Schema]:  # pylint: disable=C0116
+        return DataSet[self._schema_annotations](super().persist(storageLevel))  # type: ignore
+
+    def unpersist(self, blocking: bool = False) -> DataSet[_Schema]:  # pylint: disable=C0116
+        return DataSet[self._schema_annotations](super().unpersist(blocking))  # type: ignore
+
     def distinct(self) -> DataSet[_Schema]:  # pylint: disable=C0116
         return DataSet[self._schema_annotations](super().distinct())  # type: ignore
 
     def filter(self, condition) -> DataSet[_Schema]:  # pylint: disable=C0116
         return DataSet[self._schema_annotations](super().filter(condition))  # type: ignore
 
     @overload
```

### Comparing `typedspark-1.4.1/typedspark/_core/datatypes.py` & `typedspark-1.4.2/typedspark/_core/datatypes.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_core/literaltype.py` & `typedspark-1.4.2/typedspark/_core/literaltype.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_core/validate_schema.py` & `typedspark-1.4.2/typedspark/_core/validate_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_schema/get_schema_definition.py` & `typedspark-1.4.2/typedspark/_schema/get_schema_definition.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_schema/get_schema_imports.py` & `typedspark-1.4.2/typedspark/_schema/get_schema_imports.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_schema/schema.py` & `typedspark-1.4.2/typedspark/_schema/schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_schema/structfield.py` & `typedspark-1.4.2/typedspark/_schema/structfield.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_transforms/rename_duplicate_columns.py` & `typedspark-1.4.2/typedspark/_transforms/rename_duplicate_columns.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_transforms/structtype_column.py` & `typedspark-1.4.2/typedspark/_transforms/structtype_column.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_transforms/transform_to_schema.py` & `typedspark-1.4.2/typedspark/_transforms/transform_to_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_transforms/utils.py` & `typedspark-1.4.2/typedspark/_transforms/utils.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_utils/create_dataset.py` & `typedspark-1.4.2/typedspark/_utils/create_dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_utils/create_dataset_from_structtype.py` & `typedspark-1.4.2/typedspark/_utils/create_dataset_from_structtype.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_utils/databases.py` & `typedspark-1.4.2/typedspark/_utils/databases.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_utils/load_table.py` & `typedspark-1.4.2/typedspark/_utils/load_table.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark/_utils/register_schema_to_dataset.py` & `typedspark-1.4.2/typedspark/_utils/register_schema_to_dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.4.1/typedspark.egg-info/PKG-INFO` & `typedspark-1.4.2/typedspark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.4.1
+Version: 1.4.2
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
```

### Comparing `typedspark-1.4.1/typedspark.egg-info/SOURCES.txt` & `typedspark-1.4.2/typedspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

