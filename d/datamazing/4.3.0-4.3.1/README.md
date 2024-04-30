# Comparing `tmp/datamazing-4.3.0.tar.gz` & `tmp/datamazing-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamazing-4.3.0.tar", max compression
+gzip compressed data, was "datamazing-4.3.1.tar", max compression
```

## Comparing `datamazing-4.3.0.tar` & `datamazing-4.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/__init__.py
--rw-r--r--   0        0        0      277 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/_conform.py
--rw-r--r--   0        0        0      645 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pandas/__init__.py
--rw-r--r--   0        0        0      309 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pandas/datacollection/__init__.py
--rw-r--r--   0        0        0     2275 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pandas/io.py
--rw-r--r--   0        0        0      140 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pandas/testing/__init__.py
--rw-r--r--   0        0        0      766 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pandas/testing/assertions.py
--rw-r--r--   0        0        0     2814 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pandas/testing/data.py
--rw-r--r--   0        0        0        0 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pandas/transformations/__init__.py
--rw-r--r--   0        0        0     2384 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pandas/transformations/basic.py
--rw-r--r--   0        0        0     8044 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pandas/transformations/grouping.py
--rw-r--r--   0        0        0     2633 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pandas/transformations/merging.py
--rw-r--r--   0        0        0     2145 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pandas/transformations/reindexing.py
--rw-r--r--   0        0        0     6674 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pandas/transformations/resampling.py
--rw-r--r--   0        0        0      695 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pandas/types.py
--rw-r--r--   0        0        0      184 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pyspark/__init__.py
--rw-r--r--   0        0        0       92 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pyspark/testing/__init__.py
--rw-r--r--   0        0        0      295 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pyspark/testing/assertions.py
--rw-r--r--   0        0        0     2363 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pyspark/testing/data.py
--rw-r--r--   0        0        0        0 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pyspark/transformations/__init__.py
--rw-r--r--   0        0        0     3487 2024-04-22 14:34:19.436646 datamazing-4.3.0/datamazing/pyspark/transformations/grouping.py
--rw-r--r--   0        0        0      734 2024-04-22 14:34:19.436646 datamazing-4.3.0/pyproject.toml
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 datamazing-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/_conform.py
+-rw-r--r--   0        0        0      645 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/datacollection/__init__.py
+-rw-r--r--   0        0        0     2450 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/io.py
+-rw-r--r--   0        0        0      140 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/testing/__init__.py
+-rw-r--r--   0        0        0      766 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/testing/assertions.py
+-rw-r--r--   0        0        0     2814 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/testing/data.py
+-rw-r--r--   0        0        0        0 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/transformations/__init__.py
+-rw-r--r--   0        0        0     2384 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/transformations/basic.py
+-rw-r--r--   0        0        0     8044 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/transformations/grouping.py
+-rw-r--r--   0        0        0     2633 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/transformations/merging.py
+-rw-r--r--   0        0        0     2145 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/transformations/reindexing.py
+-rw-r--r--   0        0        0     6674 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/transformations/resampling.py
+-rw-r--r--   0        0        0      695 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/types.py
+-rw-r--r--   0        0        0      184 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pyspark/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pyspark/testing/__init__.py
+-rw-r--r--   0        0        0      295 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pyspark/testing/assertions.py
+-rw-r--r--   0        0        0     2363 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pyspark/testing/data.py
+-rw-r--r--   0        0        0        0 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pyspark/transformations/__init__.py
+-rw-r--r--   0        0        0     3487 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pyspark/transformations/grouping.py
+-rw-r--r--   0        0        0      734 2024-04-30 12:27:29.490855 datamazing-4.3.1/pyproject.toml
+-rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 datamazing-4.3.1/PKG-INFO
```

### Comparing `datamazing-4.3.0/datamazing/pandas/__init__.py` & `datamazing-4.3.1/datamazing/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.0/datamazing/pandas/io.py` & `datamazing-4.3.1/datamazing/pandas/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from os import PathLike
 
 import pandas as pd
 
 ISO_FORMAT = "%Y-%m-%dT%H:%M:%S%z"
+ISO_FORMAT_MILLISECONDS = "%Y-%m-%dT%H:%M:%S.%f%z"
 
 
 def infer_iso_datetime(values: pd.Series) -> pd.Series:
     try:
-        converted_values = pd.to_datetime(values, format=ISO_FORMAT)
+        converted_values = pd.to_datetime(values, format=ISO_FORMAT_MILLISECONDS)
     except (ValueError, TypeError):
-        # if not possible to parse as datetime, return original values
-        return values
+        try:
+            converted_values = pd.to_datetime(values, format=ISO_FORMAT)
+        except (ValueError, TypeError):
+            # if not possible to parse as datetime, return original values
+            return values
     return converted_values
 
 
 def infer_iso_timedelta(values: pd.Series) -> pd.Series:
     try:
         converted_values = pd.to_timedelta(values)
     except (ValueError, TypeError):
@@ -41,18 +45,15 @@
     Some conversions are invalid and the will cause the reading to fail.
     Example of invalid conversions:
     - converting a string to a float
 
     Args:
         filepath (str): Filepath of the CSV file
     """
-    df = pd.read_csv(
-        filepath,
-        keep_default_na=False,
-    )
+    df = pd.read_csv(filepath, keep_default_na=False)
 
     # Auto cast types based on type hint in column name
     # type hints are on the form <column_name>:<type_hint>
     renames = {}
     for column_name in df.columns:
         if ":" in column_name:
             name, type_hint = column_name.split(":")
```

### Comparing `datamazing-4.3.0/datamazing/pandas/testing/assertions.py` & `datamazing-4.3.1/datamazing/pandas/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.0/datamazing/pandas/testing/data.py` & `datamazing-4.3.1/datamazing/pandas/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.0/datamazing/pandas/transformations/basic.py` & `datamazing-4.3.1/datamazing/pandas/transformations/basic.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.0/datamazing/pandas/transformations/grouping.py` & `datamazing-4.3.1/datamazing/pandas/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.0/datamazing/pandas/transformations/merging.py` & `datamazing-4.3.1/datamazing/pandas/transformations/merging.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.0/datamazing/pandas/transformations/reindexing.py` & `datamazing-4.3.1/datamazing/pandas/transformations/reindexing.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.0/datamazing/pandas/transformations/resampling.py` & `datamazing-4.3.1/datamazing/pandas/transformations/resampling.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.0/datamazing/pandas/types.py` & `datamazing-4.3.1/datamazing/pandas/types.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.0/datamazing/pyspark/testing/data.py` & `datamazing-4.3.1/datamazing/pyspark/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.0/datamazing/pyspark/transformations/grouping.py` & `datamazing-4.3.1/datamazing/pyspark/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.0/pyproject.toml` & `datamazing-4.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datamazing"
-version = "4.3.0"
+version = "4.3.1"
 description = "Package for working with pandas Dataset, but wit specialized functions used for Energinet"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "datamazing" },
 ]
 
 [tool.poetry.dependencies]
```

