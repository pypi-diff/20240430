# Comparing `tmp/prophetverse-0.0.3a0.tar.gz` & `tmp/prophetverse-0.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophetverse-0.0.3a0.tar", max compression
+gzip compressed data, was "prophetverse-0.0.3rc1.tar", max compression
```

## Comparing `prophetverse-0.0.3a0.tar` & `prophetverse-0.0.3rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2024-04-30 12:07:43.248255 prophetverse-0.0.3a0/LICENSE
--rw-r--r--   0        0        0     3328 2024-04-30 12:07:43.248255 prophetverse-0.0.3a0/README.md
--rw-r--r--   0        0        0      671 2024-04-30 12:08:33.056820 prophetverse-0.0.3a0/pyproject.toml
--rw-r--r--   0        0        0       61 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/__init__.py
--rw-r--r--   0        0        0     1797 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/changepoint.py
--rw-r--r--   0        0        0    14517 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/effects.py
--rw-r--r--   0        0        0     6608 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/engine.py
--rw-r--r--   0        0        0       66 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/logger.py
--rw-r--r--   0        0        0      110 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/models/__init__.py
--rw-r--r--   0        0        0       25 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/models/multivariate_model/__init__.py
--rw-r--r--   0        0        0     2528 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/models/multivariate_model/_model.py
--rw-r--r--   0        0        0     1541 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/models/multivariate_model/changepoint.py
--rw-r--r--   0        0        0     4831 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/models/multivariate_model/multiindex.py
--rw-r--r--   0        0        0     1546 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/models/univariate_model.py
--rw-r--r--   0        0        0       77 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/sktime/__init__.py
--rw-r--r--   0        0        0     4364 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/sktime/_expand_column_per_level.py
--rw-r--r--   0        0        0    14328 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/sktime/base.py
--rw-r--r--   0        0        0    25304 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/sktime/multivariate.py
--rw-r--r--   0        0        0     2054 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/sktime/seasonality.py
--rw-r--r--   0        0        0    13915 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/sktime/univariate.py
--rw-r--r--   0        0        0     3813 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/utils/frame_to_array.py
--rw-r--r--   0        0        0     1206 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/utils/logistic.py
--rw-r--r--   0        0        0      756 2024-04-30 12:07:43.268255 prophetverse-0.0.3a0/src/prophetverse/utils/regex.py
--rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 prophetverse-0.0.3a0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-30 13:00:34.998978 prophetverse-0.0.3rc1/LICENSE
+-rw-r--r--   0        0        0     3328 2024-04-30 13:00:34.998978 prophetverse-0.0.3rc1/README.md
+-rw-r--r--   0        0        0      673 2024-04-30 13:01:41.506610 prophetverse-0.0.3rc1/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/__init__.py
+-rw-r--r--   0        0        0     1797 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/changepoint.py
+-rw-r--r--   0        0        0    14517 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/effects.py
+-rw-r--r--   0        0        0     6608 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/engine.py
+-rw-r--r--   0        0        0       66 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/logger.py
+-rw-r--r--   0        0        0      110 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/models/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/models/multivariate_model/__init__.py
+-rw-r--r--   0        0        0     2528 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/models/multivariate_model/_model.py
+-rw-r--r--   0        0        0     1541 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/models/multivariate_model/changepoint.py
+-rw-r--r--   0        0        0     4831 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/models/multivariate_model/multiindex.py
+-rw-r--r--   0        0        0     1546 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/models/univariate_model.py
+-rw-r--r--   0        0        0       77 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/sktime/__init__.py
+-rw-r--r--   0        0        0     4364 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/sktime/_expand_column_per_level.py
+-rw-r--r--   0        0        0    14328 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/sktime/base.py
+-rw-r--r--   0        0        0    25304 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/sktime/multivariate.py
+-rw-r--r--   0        0        0     2054 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/sktime/seasonality.py
+-rw-r--r--   0        0        0    13915 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/sktime/univariate.py
+-rw-r--r--   0        0        0     3813 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/utils/frame_to_array.py
+-rw-r--r--   0        0        0     1206 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/utils/logistic.py
+-rw-r--r--   0        0        0      756 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/utils/regex.py
+-rw-r--r--   0        0        0     3874 1970-01-01 00:00:00.000000 prophetverse-0.0.3rc1/PKG-INFO
```

### Comparing `prophetverse-0.0.3a0/LICENSE` & `prophetverse-0.0.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/README.md` & `prophetverse-0.0.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/pyproject.toml` & `prophetverse-0.0.3rc1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prophetverse"
-version = "0.0.3a0"
+version = "0.0.3-rc1"
 description = ""
 authors = ["Felipe Angelim <felipeangelim@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "prophetverse", from="src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
```

### Comparing `prophetverse-0.0.3a0/src/prophetverse/changepoint.py` & `prophetverse-0.0.3rc1/src/prophetverse/changepoint.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/effects.py` & `prophetverse-0.0.3rc1/src/prophetverse/effects.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/engine.py` & `prophetverse-0.0.3rc1/src/prophetverse/engine.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/models/multivariate_model/_model.py` & `prophetverse-0.0.3rc1/src/prophetverse/models/multivariate_model/_model.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/models/multivariate_model/changepoint.py` & `prophetverse-0.0.3rc1/src/prophetverse/models/multivariate_model/changepoint.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/models/multivariate_model/multiindex.py` & `prophetverse-0.0.3rc1/src/prophetverse/models/multivariate_model/multiindex.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/models/univariate_model.py` & `prophetverse-0.0.3rc1/src/prophetverse/models/univariate_model.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/sktime/_expand_column_per_level.py` & `prophetverse-0.0.3rc1/src/prophetverse/sktime/_expand_column_per_level.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/sktime/base.py` & `prophetverse-0.0.3rc1/src/prophetverse/sktime/base.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/sktime/multivariate.py` & `prophetverse-0.0.3rc1/src/prophetverse/sktime/multivariate.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/sktime/seasonality.py` & `prophetverse-0.0.3rc1/src/prophetverse/sktime/seasonality.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/sktime/univariate.py` & `prophetverse-0.0.3rc1/src/prophetverse/sktime/univariate.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/utils/frame_to_array.py` & `prophetverse-0.0.3rc1/src/prophetverse/utils/frame_to_array.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/utils/logistic.py` & `prophetverse-0.0.3rc1/src/prophetverse/utils/logistic.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/src/prophetverse/utils/regex.py` & `prophetverse-0.0.3rc1/src/prophetverse/utils/regex.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3a0/PKG-INFO` & `prophetverse-0.0.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophetverse
-Version: 0.0.3a0
+Version: 0.0.3rc1
 Summary: 
 Author: Felipe Angelim
 Author-email: felipeangelim@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

