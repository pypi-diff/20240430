# Comparing `tmp/yedextended-1.0.2.tar.gz` & `tmp/yedextended-1.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yedextended-1.0.2.tar", last modified: Tue Apr 30 09:36:06 2024, max compression
+gzip compressed data, was "yedextended-1.0.4a1.tar", last modified: Tue Apr 30 10:31:46 2024, max compression
```

## Comparing `yedextended-1.0.2.tar` & `yedextended-1.0.4a1.tar`

### file list

```diff
@@ -1,17 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:36:06.847379 yedextended-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-30 09:36:02.000000 yedextended-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-30 09:36:06.847379 yedextended-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-30 09:36:02.000000 yedextended-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-30 09:36:02.000000 yedextended-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:36:06.847379 yedextended-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:36:06.847379 yedextended-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:36:06.847379 yedextended-1.0.2/src/yedextended/
--rw-r--r--   0 runner    (1001) docker     (127)    73127 2024-04-30 09:36:02.000000 yedextended-1.0.2/src/yedextended/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:36:06.847379 yedextended-1.0.2/src/yedextended.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-30 09:36:06.000000 yedextended-1.0.2/src/yedextended.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-30 09:36:06.000000 yedextended-1.0.2/src/yedextended.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:36:06.000000 yedextended-1.0.2/src/yedextended.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 09:36:06.000000 yedextended-1.0.2/src/yedextended.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 09:36:06.000000 yedextended-1.0.2/src/yedextended.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:36:06.847379 yedextended-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-30 09:36:02.000000 yedextended-1.0.2/tests/test_yedextended.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:31:46.120331 yedextended-1.0.4a1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:31:46.108331 yedextended-1.0.4a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:31:46.112331 yedextended-1.0.4a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-30 10:31:46.116331 yedextended-1.0.4a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:31:46.116331 yedextended-1.0.4a1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/demo-basic-create-and-open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/demo-basic-formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/demo-basic_bulk_manage1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/demo-basic_bulk_manage2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/demo-custom-properties-nodes-edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/demo-multilabels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/demo-round-robin_read_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/demo-uml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/demo-url-description-groups-nodes-edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/readme-1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/readme-2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/readme-3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/test.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/yed_created_edges.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/examples/yed_modified_app_created.graphml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:31:46.116331 yedextended-1.0.4a1/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/images/demo_multilabel.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/images/example-UML.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/images/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/images/excel_obj_entry.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/images/excel_rel_entry.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/images/graph.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/images/graph_from_excel_obj.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/images/graph_from_excel_rel.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 10:31:46.120331 yedextended-1.0.4a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:31:46.108331 yedextended-1.0.4a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:31:46.116331 yedextended-1.0.4a1/src/yedextended/
+-rw-r--r--   0 runner    (1001) docker     (127)    73127 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/src/yedextended/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:31:46.116331 yedextended-1.0.4a1/src/yedextended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-30 10:31:46.000000 yedextended-1.0.4a1/src/yedextended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-30 10:31:46.000000 yedextended-1.0.4a1/src/yedextended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:31:46.000000 yedextended-1.0.4a1/src/yedextended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 10:31:46.000000 yedextended-1.0.4a1/src/yedextended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 10:31:46.000000 yedextended-1.0.4a1/src/yedextended.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:31:46.116331 yedextended-1.0.4a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-30 10:31:40.000000 yedextended-1.0.4a1/tests/test_yedextended.py
```

### Comparing `yedextended-1.0.2/LICENSE` & `yedextended-1.0.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.2/PKG-INFO` & `yedextended-1.0.4a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 Metadata-Version: 2.1
 Name: yedextended
-Version: 1.0.2
+Version: 1.0.4a1
 Summary: Python library extending yEd functionality through programmatic interface to graphs.
 Author-email: Cole St John <info@colestjohn.com>
 Project-URL: Homepage, https://github.com/cole-st-john/yedextended
 Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil
 Requires-Dist: pygetwindow
 Requires-Dist: openpyxl
 
+
+
+
 # Extended Python Support for yEd 
+[![CI](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml/badge.svg)](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/cole-st-john/yedextended)
+<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended?labelColor=2334D058) -->
 
 This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
 
 - [x] creating graphs
 - [x] formatting graphs
 - [x] reading graphs
 - [x] bulk data addition or management (MS excel-based)
```

### Comparing `yedextended-1.0.2/README.md` & `yedextended-1.0.4a1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,15 @@
+
+
+
 # Extended Python Support for yEd 
+[![CI](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml/badge.svg)](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/cole-st-john/yedextended)
+<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended?labelColor=2334D058) -->
 
 This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
 
 - [x] creating graphs
 - [x] formatting graphs
 - [x] reading graphs
 - [x] bulk data addition or management (MS excel-based)
```

### Comparing `yedextended-1.0.2/pyproject.toml` & `yedextended-1.0.4a1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 [project]
 name = "yedextended"
-version = "1.0.2"
+dynamic = ["version"]
 authors = [{ name = "Cole St John", email = "info@colestjohn.com" }]
 description = "Python library extending yEd functionality through programmatic interface to graphs."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = ["psutil", "pygetwindow", "openpyxl"]
 classifiers = [
-	"Programming Language :: Python :: 3",
+	"Programming Language :: Python :: 3 :: Only",
+	"Programming Language :: Python :: 3.10",
+	"Programming Language :: Python :: 3.11",
+	"Programming Language :: Python :: 3.12",
 	"License :: OSI Approved :: BSD License",
 	"Operating System :: OS Independent",
 ]
 
 
 [project.urls]
 Homepage = "https://github.com/cole-st-john/yedextended"
 Issues = "https://github.com/cole-st-john/yedextended/issues"
 
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools_scm]
+
 [tool.ruff]
 # Exclude a variety of commonly ignored directories.
 exclude = [
 	".bzr",
 	".direnv",
 	".eggs",
 	".git",
```

### Comparing `yedextended-1.0.2/src/yedextended/__init__.py` & `yedextended-1.0.4a1/src/yedextended/__init__.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.2/src/yedextended.egg-info/PKG-INFO` & `yedextended-1.0.4a1/src/yedextended.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 Metadata-Version: 2.1
 Name: yedextended
-Version: 1.0.2
+Version: 1.0.4a1
 Summary: Python library extending yEd functionality through programmatic interface to graphs.
 Author-email: Cole St John <info@colestjohn.com>
 Project-URL: Homepage, https://github.com/cole-st-john/yedextended
 Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil
 Requires-Dist: pygetwindow
 Requires-Dist: openpyxl
 
+
+
+
 # Extended Python Support for yEd 
+[![CI](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml/badge.svg)](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/cole-st-john/yedextended)
+<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended?labelColor=2334D058) -->
 
 This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
 
 - [x] creating graphs
 - [x] formatting graphs
 - [x] reading graphs
 - [x] bulk data addition or management (MS excel-based)
```

### Comparing `yedextended-1.0.2/tests/test_yedextended.py` & `yedextended-1.0.4a1/tests/test_yedextended.py`

 * *Files identical despite different names*

