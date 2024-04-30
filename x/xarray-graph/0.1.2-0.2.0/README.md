# Comparing `tmp/xarray_graph-0.1.2.tar.gz` & `tmp/xarray_graph-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_graph-0.1.2.tar", last modified: Thu Jan 11 16:24:58 2024, max compression
+gzip compressed data, was "xarray_graph-0.2.0.tar", last modified: Tue Apr 30 21:47:35 2024, max compression
```

## Comparing `xarray_graph-0.1.2.tar` & `xarray_graph-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-01-11 15:44:26.780358 xarray_graph-0.1.2/LICENSE
--rw-r--r--   0        0        0      134 2024-01-11 15:44:26.780526 xarray_graph-0.1.2/README.md
--rw-r--r--   0        0        0     1326 2024-01-11 16:24:58.851204 xarray_graph-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    82077 2024-01-11 16:16:39.067738 xarray_graph-0.1.2/src/xarray_graph/XarrayGraph.py
--rw-r--r--   0        0        0       48 2024-01-11 15:44:26.782449 xarray_graph-0.1.2/src/xarray_graph/__init__.py
--rw-r--r--   0        0        0      239 2024-01-11 16:04:58.520462 xarray_graph-0.1.2/src/xarray_graph/xarray-graph.code-workspace
--rw-r--r--   0        0        0        0 2024-01-11 15:44:26.782628 xarray_graph-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 xarray_graph-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-11 15:44:26.780358 xarray_graph-0.2.0/LICENSE
+-rw-r--r--   0        0        0      205 2024-01-22 15:50:52.988118 xarray_graph-0.2.0/README.md
+-rw-r--r--   0        0        0     1380 2024-04-30 21:47:35.865609 xarray_graph-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1841 2024-04-30 14:22:30.897258 xarray_graph-0.2.0/src/xarray_graph/RegionsManager.py
+-rw-r--r--   0        0        0   100581 2024-04-30 16:07:54.427853 xarray_graph-0.2.0/src/xarray_graph/XarrayGraph.py
+-rw-r--r--   0        0        0       48 2024-01-11 15:44:26.782449 xarray_graph-0.2.0/src/xarray_graph/__init__.py
+-rw-r--r--   0        0        0      265 2024-01-22 15:50:52.989812 xarray_graph-0.2.0/src/xarray_graph/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-11 15:44:26.782628 xarray_graph-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1451 1970-01-01 00:00:00.000000 xarray_graph-0.2.0/PKG-INFO
```

### Comparing `xarray_graph-0.1.2/LICENSE` & `xarray_graph-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray_graph-0.1.2/pyproject.toml` & `xarray_graph-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -31,23 +31,26 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-version = "0.1.2"
+version = "0.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/marcel-goldschen-ohm/xarray-graph"
 repository = "https://github.com/marcel-goldschen-ohm/xarray-graph"
 
+[project.scripts]
+xrg = "xarray_graph.__main__:main"
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
```

### Comparing `xarray_graph-0.1.2/PKG-INFO` & `xarray_graph-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xarray-graph
-Version: 0.1.2
+Version: 0.2.0
 Summary: PyQt/PySide UI for graphing (x,y) slices of Xarray datasets.
-Keywords: PyQt PySide xarray graph
+Keywords: PyQt,PySide,xarray,graph
 Home-page: https://github.com/marcel-goldschen-ohm/xarray-graph
 Author-Email: Marcel Goldschen-Ohm <goldschen-ohm@utexas.edu>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -26,14 +26,19 @@
 Requires-Dist: pyqt-ext>=1.1.0
 Requires-Dist: pyqtgraph-ext>=1.0.0
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: lmfit>=1.2.2
 Description-Content-Type: text/markdown
 
 # xarray-graph
-PyQt/PySide UI for graphing (x,y) slices of xarray datasets.
+PyQt/PySide UI for graphing (x,y) slices of Xarray datasets.
+
+# Install
+Should work with PySide6, PyQt6, or PyQt5.
+```shell
+pip install PySide6 xarray-graph
+```
 
 # TODO
-- named regions
-- measurements
-- curve fits
 - i/o
+- tests
+- docs
```

