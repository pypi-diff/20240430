# Comparing `tmp/ExcelFormulaParser-1.0.0.tar.gz` & `tmp/ExcelFormulaParser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExcelFormulaParser-1.0.0.tar", last modified: Mon Apr 29 23:11:11 2024, max compression
+gzip compressed data, was "ExcelFormulaParser-1.0.1.tar", last modified: Mon Apr 29 23:33:59 2024, max compression
```

## Comparing `ExcelFormulaParser-1.0.0.tar` & `ExcelFormulaParser-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 23:11:11.269301 ExcelFormulaParser-1.0.0/
--rw-rw-rw-   0        0        0     1089 2024-04-14 04:33:18.000000 ExcelFormulaParser-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3319 2024-04-29 23:11:11.268296 ExcelFormulaParser-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2790 2024-04-29 02:03:05.000000 ExcelFormulaParser-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 23:11:11.269301 ExcelFormulaParser-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      897 2024-04-29 17:46:22.000000 ExcelFormulaParser-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 23:11:11.171269 ExcelFormulaParser-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 23:11:11.216321 ExcelFormulaParser-1.0.0/src/ExcelFormulaParser.egg-info/
--rw-rw-rw-   0        0        0     3319 2024-04-29 23:11:11.000000 ExcelFormulaParser-1.0.0/src/ExcelFormulaParser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      644 2024-04-29 23:11:11.000000 ExcelFormulaParser-1.0.0/src/ExcelFormulaParser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 23:11:11.000000 ExcelFormulaParser-1.0.0/src/ExcelFormulaParser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 23:11:11.000000 ExcelFormulaParser-1.0.0/src/ExcelFormulaParser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 23:11:11.000000 ExcelFormulaParser-1.0.0/src/ExcelFormulaParser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 23:11:11.243530 ExcelFormulaParser-1.0.0/src/Models/
--rw-rw-rw-   0        0        0       25 2024-04-29 17:36:59.000000 ExcelFormulaParser-1.0.0/src/Models/__init__.py
--rw-rw-rw-   0        0        0     1069 2024-04-29 02:03:00.000000 ExcelFormulaParser-1.0.0/src/Models/constant.py
--rw-rw-rw-   0        0        0     6093 2024-04-29 18:37:40.000000 ExcelFormulaParser-1.0.0/src/Models/expression.py
--rw-rw-rw-   0        0        0     2642 2024-04-29 18:15:15.000000 ExcelFormulaParser-1.0.0/src/Models/formula.py
--rw-rw-rw-   0        0        0     5904 2024-04-29 18:37:40.000000 ExcelFormulaParser-1.0.0/src/Models/function.py
--rw-rw-rw-   0        0        0     1001 2024-04-29 22:19:08.000000 ExcelFormulaParser-1.0.0/src/Models/model_types.py
--rw-rw-rw-   0        0        0    11128 2024-04-29 05:29:01.000000 ExcelFormulaParser-1.0.0/src/Models/parser.py
--rw-rw-rw-   0        0        0     5385 2024-04-29 22:55:51.000000 ExcelFormulaParser-1.0.0/src/Models/range.py
--rw-rw-rw-   0        0        0     5430 2024-04-29 02:03:00.000000 ExcelFormulaParser-1.0.0/src/Models/reference.py
-drwxrwxrwx   0        0        0        0 2024-04-29 23:11:11.265788 ExcelFormulaParser-1.0.0/src/Tests/
--rw-rw-rw-   0        0        0        0 2024-04-15 00:32:35.000000 ExcelFormulaParser-1.0.0/src/Tests/__init__.py
--rw-rw-rw-   0        0        0     1360 2024-04-29 02:03:00.000000 ExcelFormulaParser-1.0.0/src/Tests/test_constant.py
--rw-rw-rw-   0        0        0     3315 2024-04-29 02:03:00.000000 ExcelFormulaParser-1.0.0/src/Tests/test_expression.py
--rw-rw-rw-   0        0        0     3525 2024-04-29 02:03:00.000000 ExcelFormulaParser-1.0.0/src/Tests/test_function.py
--rw-rw-rw-   0        0        0     5944 2024-04-29 02:03:00.000000 ExcelFormulaParser-1.0.0/src/Tests/test_parser.py
--rw-rw-rw-   0        0        0     4268 2024-04-29 22:55:17.000000 ExcelFormulaParser-1.0.0/src/Tests/test_range.py
--rw-rw-rw-   0        0        0     2459 2024-04-29 02:03:00.000000 ExcelFormulaParser-1.0.0/src/Tests/test_reference.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:33:59.775613 ExcelFormulaParser-1.0.1/
+-rw-rw-rw-   0        0        0     1089 2024-04-14 04:33:18.000000 ExcelFormulaParser-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3360 2024-04-29 23:33:59.775613 ExcelFormulaParser-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2790 2024-04-29 02:03:05.000000 ExcelFormulaParser-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 23:33:59.775613 ExcelFormulaParser-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      958 2024-04-29 23:33:54.000000 ExcelFormulaParser-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:33:59.707470 ExcelFormulaParser-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 23:33:59.737354 ExcelFormulaParser-1.0.1/src/ExcelFormulaParser.egg-info/
+-rw-rw-rw-   0        0        0     3360 2024-04-29 23:33:59.000000 ExcelFormulaParser-1.0.1/src/ExcelFormulaParser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2024-04-29 23:33:59.000000 ExcelFormulaParser-1.0.1/src/ExcelFormulaParser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 23:33:59.000000 ExcelFormulaParser-1.0.1/src/ExcelFormulaParser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 23:33:59.000000 ExcelFormulaParser-1.0.1/src/ExcelFormulaParser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-29 23:33:59.000000 ExcelFormulaParser-1.0.1/src/ExcelFormulaParser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 23:33:59.757495 ExcelFormulaParser-1.0.1/src/Models/
+-rw-rw-rw-   0        0        0       25 2024-04-29 23:22:34.000000 ExcelFormulaParser-1.0.1/src/Models/__init__.py
+-rw-rw-rw-   0        0        0     1069 2024-04-29 23:22:05.000000 ExcelFormulaParser-1.0.1/src/Models/constant.py
+-rw-rw-rw-   0        0        0     6093 2024-04-29 23:22:05.000000 ExcelFormulaParser-1.0.1/src/Models/expression.py
+-rw-rw-rw-   0        0        0     2642 2024-04-29 23:22:34.000000 ExcelFormulaParser-1.0.1/src/Models/formula.py
+-rw-rw-rw-   0        0        0     5904 2024-04-29 23:22:05.000000 ExcelFormulaParser-1.0.1/src/Models/function.py
+-rw-rw-rw-   0        0        0     1001 2024-04-29 23:22:05.000000 ExcelFormulaParser-1.0.1/src/Models/model_types.py
+-rw-rw-rw-   0        0        0    11128 2024-04-29 23:22:35.000000 ExcelFormulaParser-1.0.1/src/Models/parser.py
+-rw-rw-rw-   0        0        0     5385 2024-04-29 23:22:05.000000 ExcelFormulaParser-1.0.1/src/Models/range.py
+-rw-rw-rw-   0        0        0     5430 2024-04-29 23:22:05.000000 ExcelFormulaParser-1.0.1/src/Models/reference.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:33:59.772611 ExcelFormulaParser-1.0.1/src/Tests/
+-rw-rw-rw-   0        0        0        0 2024-04-15 00:32:35.000000 ExcelFormulaParser-1.0.1/src/Tests/__init__.py
+-rw-rw-rw-   0        0        0     1360 2024-04-29 23:22:05.000000 ExcelFormulaParser-1.0.1/src/Tests/test_constant.py
+-rw-rw-rw-   0        0        0     3315 2024-04-29 23:22:05.000000 ExcelFormulaParser-1.0.1/src/Tests/test_expression.py
+-rw-rw-rw-   0        0        0     3525 2024-04-29 23:22:05.000000 ExcelFormulaParser-1.0.1/src/Tests/test_function.py
+-rw-rw-rw-   0        0        0     5944 2024-04-29 23:22:35.000000 ExcelFormulaParser-1.0.1/src/Tests/test_parser.py
+-rw-rw-rw-   0        0        0     4268 2024-04-29 23:22:05.000000 ExcelFormulaParser-1.0.1/src/Tests/test_range.py
+-rw-rw-rw-   0        0        0     2459 2024-04-29 23:22:05.000000 ExcelFormulaParser-1.0.1/src/Tests/test_reference.py
```

### Comparing `ExcelFormulaParser-1.0.0/LICENSE` & `ExcelFormulaParser-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/PKG-INFO` & `ExcelFormulaParser-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ExcelFormulaParser
-Version: 1.0.0
+Version: 1.0.1
 Summary: A framework to break down Excel Formula strings into a parsable and modifiable JSON data structure.
-Home-page: UNKNOWN
+Home-page: https://github.com/Voltaic314/ExcelFormulaParser
 Author: Voltaic314
 Author-email: logan@stax.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ExcelFormulaParser-1.0.0/README.md` & `ExcelFormulaParser-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/setup.py` & `ExcelFormulaParser-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ExcelFormulaParser",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(where="src"),  # Tells setuptools to package any Python packages found in src
     package_dir={"": "src"},  # Tells setuptools that the packages are under src directory
     author="Voltaic314",
     author_email="logan@stax.ai",
     description="A framework to break down Excel Formula strings into a parsable and modifiable JSON data structure.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
+    url='https://github.com/Voltaic314/ExcelFormulaParser',
     install_requires=[
         'openpyxl',  # List your dependencies here
         'pandas',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ExcelFormulaParser-1.0.0/src/ExcelFormulaParser.egg-info/PKG-INFO` & `ExcelFormulaParser-1.0.1/src/ExcelFormulaParser.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ExcelFormulaParser
-Version: 1.0.0
+Version: 1.0.1
 Summary: A framework to break down Excel Formula strings into a parsable and modifiable JSON data structure.
-Home-page: UNKNOWN
+Home-page: https://github.com/Voltaic314/ExcelFormulaParser
 Author: Voltaic314
 Author-email: logan@stax.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ExcelFormulaParser-1.0.0/src/ExcelFormulaParser.egg-info/SOURCES.txt` & `ExcelFormulaParser-1.0.1/src/ExcelFormulaParser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Models/constant.py` & `ExcelFormulaParser-1.0.1/src/Models/constant.py`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Models/expression.py` & `ExcelFormulaParser-1.0.1/src/Models/expression.py`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Models/formula.py` & `ExcelFormulaParser-1.0.1/src/Models/formula.py`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Models/function.py` & `ExcelFormulaParser-1.0.1/src/Models/function.py`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Models/model_types.py` & `ExcelFormulaParser-1.0.1/src/Models/model_types.py`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Models/parser.py` & `ExcelFormulaParser-1.0.1/src/Models/parser.py`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Models/range.py` & `ExcelFormulaParser-1.0.1/src/Models/range.py`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Models/reference.py` & `ExcelFormulaParser-1.0.1/src/Models/reference.py`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Tests/test_constant.py` & `ExcelFormulaParser-1.0.1/src/Tests/test_constant.py`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Tests/test_expression.py` & `ExcelFormulaParser-1.0.1/src/Tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Tests/test_function.py` & `ExcelFormulaParser-1.0.1/src/Tests/test_function.py`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Tests/test_parser.py` & `ExcelFormulaParser-1.0.1/src/Tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Tests/test_range.py` & `ExcelFormulaParser-1.0.1/src/Tests/test_range.py`

 * *Files identical despite different names*

### Comparing `ExcelFormulaParser-1.0.0/src/Tests/test_reference.py` & `ExcelFormulaParser-1.0.1/src/Tests/test_reference.py`

 * *Files identical despite different names*

