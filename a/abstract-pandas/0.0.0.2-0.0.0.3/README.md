# Comparing `tmp/abstract_pandas-0.0.0.2.tar.gz` & `tmp/abstract_pandas-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_pandas-0.0.0.2.tar", last modified: Mon Apr 29 21:25:29 2024, max compression
+gzip compressed data, was "abstract_pandas-0.0.0.3.tar", last modified: Mon Apr 29 21:38:05 2024, max compression
```

## Comparing `abstract_pandas-0.0.0.2.tar` & `abstract_pandas-0.0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 21:25:29.910421 abstract_pandas-0.0.0.2/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-04-29 21:25:29.910421 abstract_pandas-0.0.0.2/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.2/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-29 21:25:29.910421 abstract_pandas-0.0.0.2/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      979 2024-04-29 21:25:21.000000 abstract_pandas-0.0.0.2/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 21:25:29.910421 abstract_pandas-0.0.0.2/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 21:25:29.910421 abstract_pandas-0.0.0.2/src/abstract_pandas/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      285 2024-04-28 05:06:34.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/class_manager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    20479 2024-04-24 17:55:36.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/excel_gui.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    15784 2024-04-29 21:25:11.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/excel_module.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3227 2024-04-17 09:26:10.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/general_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5664 2024-04-26 19:59:40.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/geo_pandas.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1464 2024-04-26 00:28:54.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/geo_spec.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5426 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/time_module.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 21:25:29.910421 abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-04-29 21:25:29.000000 abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      512 2024-04-29 21:25:29.000000 abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-29 21:25:29.000000 abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-04-29 21:25:29.000000 abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-04-29 21:25:29.000000 abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 21:38:05.211206 abstract_pandas-0.0.0.3/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-04-29 21:38:05.211206 abstract_pandas-0.0.0.3/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.3/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-29 21:38:05.211206 abstract_pandas-0.0.0.3/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      979 2024-04-29 21:37:57.000000 abstract_pandas-0.0.0.3/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 21:38:05.211206 abstract_pandas-0.0.0.3/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 21:38:05.211206 abstract_pandas-0.0.0.3/src/abstract_pandas/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.3/src/abstract_pandas/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      285 2024-04-28 05:06:34.000000 abstract_pandas-0.0.0.3/src/abstract_pandas/class_manager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    20479 2024-04-24 17:55:36.000000 abstract_pandas-0.0.0.3/src/abstract_pandas/excel_gui.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    15773 2024-04-29 21:36:35.000000 abstract_pandas-0.0.0.3/src/abstract_pandas/excel_module.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3227 2024-04-17 09:26:10.000000 abstract_pandas-0.0.0.3/src/abstract_pandas/general_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5664 2024-04-26 19:59:40.000000 abstract_pandas-0.0.0.3/src/abstract_pandas/geo_pandas.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1464 2024-04-26 00:28:54.000000 abstract_pandas-0.0.0.3/src/abstract_pandas/geo_spec.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5426 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.3/src/abstract_pandas/time_module.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 21:38:05.211206 abstract_pandas-0.0.0.3/src/abstract_pandas.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-04-29 21:38:05.000000 abstract_pandas-0.0.0.3/src/abstract_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      512 2024-04-29 21:38:05.000000 abstract_pandas-0.0.0.3/src/abstract_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-29 21:38:05.000000 abstract_pandas-0.0.0.3/src/abstract_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-04-29 21:38:05.000000 abstract_pandas-0.0.0.3/src/abstract_pandas.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-04-29 21:38:05.000000 abstract_pandas-0.0.0.3/src/abstract_pandas.egg-info/top_level.txt
```

### Comparing `abstract_pandas-0.0.0.2/PKG-INFO` & `abstract_pandas-0.0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.2
+Version: 0.0.0.3
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.2/setup.py` & `abstract_pandas-0.0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_pandas',
-    version='0.0.0.2',
+    version='0.0.0.3',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_pandas-0.0.0.2/src/abstract_pandas/excel_gui.py` & `abstract_pandas-0.0.0.3/src/abstract_pandas/excel_gui.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.2/src/abstract_pandas/excel_module.py` & `abstract_pandas-0.0.0.3/src/abstract_pandas/excel_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import pandas as pd
 from pyxlsb import open_workbook
 
 
 
 # Example usage
 
-print(df)
 def read_xlsb_to_dataframe(file_path, sheet_name):
     data = []
     with open_workbook(file_path) as wb:
         with wb.get_sheet(sheet_name) as sheet:
             for row in sheet.rows():
                 data.append([cell.v for cell in row])
     # Create a DataFrame
```

### Comparing `abstract_pandas-0.0.0.2/src/abstract_pandas/general_functions.py` & `abstract_pandas-0.0.0.3/src/abstract_pandas/general_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.2/src/abstract_pandas/geo_pandas.py` & `abstract_pandas-0.0.0.3/src/abstract_pandas/geo_pandas.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.2/src/abstract_pandas/geo_spec.py` & `abstract_pandas-0.0.0.3/src/abstract_pandas/geo_spec.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.2/src/abstract_pandas/time_module.py` & `abstract_pandas-0.0.0.3/src/abstract_pandas/time_module.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/PKG-INFO` & `abstract_pandas-0.0.0.3/src/abstract_pandas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.2
+Version: 0.0.0.3
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/SOURCES.txt` & `abstract_pandas-0.0.0.3/src/abstract_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

