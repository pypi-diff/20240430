# Comparing `tmp/textual_pandas-0.2.1.tar.gz` & `tmp/textual_pandas-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_pandas-0.2.1.tar", max compression
+gzip compressed data, was "textual_pandas-0.2.2.tar", max compression
```

## Comparing `textual_pandas-0.2.1.tar` & `textual_pandas-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-05-06 00:59:39.338531 textual_pandas-0.2.1/LICENSE
--rw-r--r--   0        0        0     2696 2023-05-06 01:49:48.722528 textual_pandas-0.2.1/README.md
--rw-r--r--   0        0        0      501 2023-05-06 01:53:44.612362 textual_pandas-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       80 2023-05-06 00:59:39.339155 textual_pandas-0.2.1/textual_pandas/__init__.py
--rw-r--r--   0        0        0     1117 2023-05-06 00:59:39.339259 textual_pandas-0.2.1/textual_pandas/widgets.py
--rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 textual_pandas-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-30 00:21:18.590736 textual_pandas-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2696 2024-04-30 00:21:18.590864 textual_pandas-0.2.2/README.md
+-rw-r--r--   0        0        0      519 2024-04-30 00:41:15.600029 textual_pandas-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-04-30 00:21:18.591815 textual_pandas-0.2.2/textual_pandas/__init__.py
+-rw-r--r--   0        0        0     1149 2024-04-30 00:21:18.591926 textual_pandas-0.2.2/textual_pandas/widgets.py
+-rw-r--r--   0        0        0     3460 1970-01-01 00:00:00.000000 textual_pandas-0.2.2/PKG-INFO
```

### Comparing `textual_pandas-0.2.1/LICENSE` & `textual_pandas-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_pandas-0.2.1/README.md` & `textual_pandas-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `textual_pandas-0.2.1/textual_pandas/widgets.py` & `textual_pandas-0.2.2/textual_pandas/widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from textual.widgets import DataTable
 import pandas as pd
 
 
 class DataFrameTable(DataTable):
     """Display Pandas dataframe in DataTable widget."""
 
-    def __init__(self):
-        super().__init__()
 
+    DEFAULT_CSS = """
+    DataFrameTable {
+        height: 1fr
+    }
+    """
+
+    
     def add_df(self, df: pd.DataFrame):
         """Add DataFrame data to DataTable."""
         self.df = df
         self.add_columns(*self._add_df_columns())
         self.add_rows(self._add_df_rows()[0:])
         return self
```

### Comparing `textual_pandas-0.2.1/PKG-INFO` & `textual_pandas-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: textual-pandas
-Version: 0.2.1
+Version: 0.2.2
 Summary: A module to build Textual widgets that represent data from the Pandas library
 Home-page: https://github.com/dannywade/textual-pandas
 License: MIT
 Author: Dan Wade
 Author-email: danny.wade35@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: textual (>=0.23.0,<0.24.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pandas (<=2.2.2)
+Requires-Dist: textual (>=0.23.0,<=0.58.0)
 Description-Content-Type: text/markdown
 
 # textual-pandas
 
 A module to display Pandas DataFrames in Textual's DataTable widget.
 
 ## Background
```

