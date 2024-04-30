# Comparing `tmp/pyany2json-0.1.0.tar.gz` & `tmp/pyany2json-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyany2json-0.1.0.tar", max compression
+gzip compressed data, was "pyany2json-0.1.1.tar", max compression
```

## Comparing `pyany2json-0.1.0.tar` & `pyany2json-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    35149 2024-04-07 14:39:29.855166 pyany2json-0.1.0/LICENSE
--rw-r--r--   0        0        0     2122 2024-04-07 14:44:35.668946 pyany2json-0.1.0/README.md
--rw-r--r--   0        0        0      107 2024-04-06 04:06:45.433805 pyany2json-0.1.0/pyany2json/__init__.py
--rw-r--r--   0        0        0     2243 2024-04-25 03:34:44.734515 pyany2json-0.1.0/pyany2json/document_factory.py
--rw-r--r--   0        0        0      312 2024-04-07 09:29:48.489269 pyany2json-0.1.0/pyany2json/layex_table_parser.py
--rw-r--r--   0        0        0     1085 2024-04-07 09:16:49.923104 pyany2json-0.1.0/pyany2json/model.py
--rw-r--r--   0        0        0       51 2024-04-25 03:46:47.997494 pyany2json-0.1.0/pyany2json/setup.py
--rw-r--r--   0        0        0      658 2024-04-07 09:19:08.905143 pyany2json-0.1.0/pyany2json/types.py
--rw-r--r--   0        0        0      366 2024-04-25 04:09:56.963969 pyany2json-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2540 1970-01-01 00:00:00.000000 pyany2json-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-07 14:39:29.855166 pyany2json-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2139 2024-04-25 04:15:24.414099 pyany2json-0.1.1/README.md
+-rw-r--r--   0        0        0   101192 2024-04-25 08:52:53.877970 pyany2json-0.1.1/libs/xelem-3.1.jar
+-rw-r--r--   0        0        0      107 2024-04-06 04:06:45.433805 pyany2json-0.1.1/pyany2json/__init__.py
+-rw-r--r--   0        0        0     2878 2024-04-30 07:32:28.086864 pyany2json-0.1.1/pyany2json/document_factory.py
+-rw-r--r--   0        0        0      312 2024-04-07 09:29:48.489269 pyany2json-0.1.1/pyany2json/layex_table_parser.py
+-rw-r--r--   0        0        0     1085 2024-04-07 09:16:49.923104 pyany2json-0.1.1/pyany2json/model.py
+-rw-r--r--   0        0        0     1651 2024-04-30 06:04:13.022052 pyany2json-0.1.1/pyany2json/setup.py
+-rw-r--r--   0        0        0      658 2024-04-07 09:19:08.905143 pyany2json-0.1.1/pyany2json/types.py
+-rw-r--r--   0        0        0      427 2024-04-30 07:49:38.004803 pyany2json-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 pyany2json-0.1.1/PKG-INFO
```

### Comparing `pyany2json-0.1.0/LICENSE` & `pyany2json-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyany2json-0.1.0/README.md` & `pyany2json-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 Moreover, by automating the extraction process, it not only saves time but also minimizes errors, particularly beneficial
 for industries dealing with large volumes of such documents. Crucially, this framework integrates with machine learning workflows,
 unlocking new possibilities for data enrichment and predictive modeling. By leveraging determinist algorithms, this framework is perfect
 to prepare your data for training processes in a predictive and reproductible manner. Aligned with the paradigm of data as a service,
 it offers a scalable and efficient means of managing semi-structured data, thereby expanding the toolkit of data services available
 to organizations.
 
-Visit our [full documentation](https://romualdrousseau.github.io/Any2Json-Documents/) and learn more about how it works, try our
+Visit our [full documentation](https://romualdrousseau.github.io/PyAny2Json/) and learn more about how it works, try our
 tutorials and find a full list of plugins and models.
 
 ## Getting Started
 
 ### Dependencies
 
 * Python 3.8.2 or above.
 * Pip 20.0.2 or above.
+* Poetry 1.7.1 or above.
 * Just 1.24.0 or above.
 
 ## Contribute
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

### Comparing `pyany2json-0.1.0/pyany2json/document_factory.py` & `pyany2json-0.1.1/pyany2json/document_factory.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 from .model import *
 
 from com.github.romualdrousseau.any2json import DocumentFactory as DocumentFactory_  # type: ignore
 from com.github.romualdrousseau.any2json import Document as Document_  # type: ignore
+from com.github.romualdrousseau.any2json.base import DataTable as DataTable  # type: ignore
 
 INTELLI_LAYOUT = Document_.Hint.INTELLI_LAYOUT
 INTELLI_TAG = Document_.Hint.INTELLI_TAG
 
 
 class HeaderTag:
     def getValue(self) -> str:
@@ -37,14 +38,41 @@
 class Table:
     def headers(self) -> list[Header]:
         """Toto"""
 
     def rows(self) -> list[Row]:
         """Toto"""
 
+    def getSheet(self) -> Sheet:
+        """Toto"""
+
+    def getNumberOfColumns(self) -> int:
+        """Toto"""
+
+    def getNumberOfRows(self) -> int:
+        """Toto"""
+
+    def getRowAt(self, rowIndex) -> Row:
+        """Toto"""
+
+    def getNumberOfHeaders(self) -> int:
+        """Toto"""
+
+    def getHeaderNames(self) -> list[str]:
+        """Toto"""
+
+    def getHeaderAt(self, i) -> Header:
+        """Toto"""
+
+    def getNumberOfHeaderTags(self) -> int:
+        """Toto"""
+
+    def headerTags(self) -> list[Header]:
+        """Toto"""
+
 
 class OptionalTable:
 
     def isPresent(self) -> bool:
         """Toto"""
 
     def get(self) -> Table:
```

### Comparing `pyany2json-0.1.0/pyany2json/model.py` & `pyany2json-0.1.1/pyany2json/model.py`

 * *Files identical despite different names*

### Comparing `pyany2json-0.1.0/pyany2json/types.py` & `pyany2json-0.1.1/pyany2json/types.py`

 * *Files identical despite different names*

### Comparing `pyany2json-0.1.0/PKG-INFO` & `pyany2json-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyany2json
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python binding to Any2Json
 Author: Romuald Rousseau
 Author-email: romuald.rousseau@servier.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -28,23 +28,24 @@
 Moreover, by automating the extraction process, it not only saves time but also minimizes errors, particularly beneficial
 for industries dealing with large volumes of such documents. Crucially, this framework integrates with machine learning workflows,
 unlocking new possibilities for data enrichment and predictive modeling. By leveraging determinist algorithms, this framework is perfect
 to prepare your data for training processes in a predictive and reproductible manner. Aligned with the paradigm of data as a service,
 it offers a scalable and efficient means of managing semi-structured data, thereby expanding the toolkit of data services available
 to organizations.
 
-Visit our [full documentation](https://romualdrousseau.github.io/Any2Json-Documents/) and learn more about how it works, try our
+Visit our [full documentation](https://romualdrousseau.github.io/PyAny2Json/) and learn more about how it works, try our
 tutorials and find a full list of plugins and models.
 
 ## Getting Started
 
 ### Dependencies
 
 * Python 3.8.2 or above.
 * Pip 20.0.2 or above.
+* Poetry 1.7.1 or above.
 * Just 1.24.0 or above.
 
 ## Contribute
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

