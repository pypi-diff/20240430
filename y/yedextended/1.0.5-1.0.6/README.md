# Comparing `tmp/yedextended-1.0.5.tar.gz` & `tmp/yedextended-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yedextended-1.0.5.tar", last modified: Tue Apr 30 10:35:33 2024, max compression
+gzip compressed data, was "yedextended-1.0.6.tar", last modified: Tue Apr 30 14:48:33 2024, max compression
```

## Comparing `yedextended-1.0.5.tar` & `yedextended-1.0.6.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:35:33.959515 yedextended-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:35:33.955515 yedextended-1.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:35:33.955515 yedextended-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-30 10:35:28.000000 yedextended-1.0.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-30 10:35:28.000000 yedextended-1.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-30 10:35:28.000000 yedextended-1.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-30 10:35:28.000000 yedextended-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-30 10:35:33.959515 yedextended-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-30 10:35:28.000000 yedextended-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:35:33.959515 yedextended-1.0.5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/demo-basic-create-and-open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/demo-basic-formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/demo-basic_bulk_manage1.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/demo-basic_bulk_manage2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/demo-custom-properties-nodes-edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/demo-multilabels.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/demo-round-robin_read_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/demo-uml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/demo-url-description-groups-nodes-edges.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/readme-1.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/readme-2.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/readme-3.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/test.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/test.graphml
--rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/yed_created_edges.graphml
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-30 10:35:28.000000 yedextended-1.0.5/examples/yed_modified_app_created.graphml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:35:33.959515 yedextended-1.0.5/images/
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-04-30 10:35:28.000000 yedextended-1.0.5/images/demo_multilabel.png
--rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-04-30 10:35:28.000000 yedextended-1.0.5/images/example-UML.png
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-30 10:35:28.000000 yedextended-1.0.5/images/example.png
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-04-30 10:35:28.000000 yedextended-1.0.5/images/excel_obj_entry.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-30 10:35:28.000000 yedextended-1.0.5/images/excel_rel_entry.gif
--rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-04-30 10:35:28.000000 yedextended-1.0.5/images/graph.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-30 10:35:28.000000 yedextended-1.0.5/images/graph_from_excel_obj.gif
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-30 10:35:28.000000 yedextended-1.0.5/images/graph_from_excel_rel.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-30 10:35:28.000000 yedextended-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 10:35:28.000000 yedextended-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 10:35:33.959515 yedextended-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:35:33.955515 yedextended-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:35:33.959515 yedextended-1.0.5/src/yedextended/
--rw-r--r--   0 runner    (1001) docker     (127)    73127 2024-04-30 10:35:28.000000 yedextended-1.0.5/src/yedextended/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:35:33.959515 yedextended-1.0.5/src/yedextended.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-30 10:35:33.000000 yedextended-1.0.5/src/yedextended.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-30 10:35:33.000000 yedextended-1.0.5/src/yedextended.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:35:33.000000 yedextended-1.0.5/src/yedextended.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 10:35:33.000000 yedextended-1.0.5/src/yedextended.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 10:35:33.000000 yedextended-1.0.5/src/yedextended.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:35:33.959515 yedextended-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:35:28.000000 yedextended-1.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-30 10:35:28.000000 yedextended-1.0.5/tests/test_yedextended.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:48:33.485942 yedextended-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 14:48:24.000000 yedextended-1.0.6/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:48:33.477942 yedextended-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:48:33.481942 yedextended-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-30 14:48:24.000000 yedextended-1.0.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-30 14:48:24.000000 yedextended-1.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-30 14:48:24.000000 yedextended-1.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-30 14:48:24.000000 yedextended-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-30 14:48:33.485942 yedextended-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-30 14:48:24.000000 yedextended-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:48:33.481942 yedextended-1.0.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/demo-basic-create-and-open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/demo-basic-formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/demo-basic_bulk_manage1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/demo-basic_bulk_manage2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/demo-custom-properties-nodes-edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/demo-multilabels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/demo-round-robin_read_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/demo-uml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/demo-url-description-groups-nodes-edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/readme-1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/readme-2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/readme-3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/test.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/yed_created_edges.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-30 14:48:24.000000 yedextended-1.0.6/examples/yed_modified_app_created.graphml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:48:33.481942 yedextended-1.0.6/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-04-30 14:48:24.000000 yedextended-1.0.6/images/demo_multilabel.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-04-30 14:48:24.000000 yedextended-1.0.6/images/example-UML.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-30 14:48:24.000000 yedextended-1.0.6/images/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-04-30 14:48:24.000000 yedextended-1.0.6/images/excel_obj_entry.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-30 14:48:24.000000 yedextended-1.0.6/images/excel_rel_entry.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-04-30 14:48:24.000000 yedextended-1.0.6/images/graph.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-30 14:48:24.000000 yedextended-1.0.6/images/graph_from_excel_obj.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-30 14:48:24.000000 yedextended-1.0.6/images/graph_from_excel_rel.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-30 14:48:24.000000 yedextended-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 14:48:24.000000 yedextended-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:48:33.485942 yedextended-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:48:33.477942 yedextended-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:48:33.485942 yedextended-1.0.6/src/yedextended/
+-rw-r--r--   0 runner    (1001) docker     (127)    73127 2024-04-30 14:48:24.000000 yedextended-1.0.6/src/yedextended/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:48:33.485942 yedextended-1.0.6/src/yedextended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-30 14:48:33.000000 yedextended-1.0.6/src/yedextended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-30 14:48:33.000000 yedextended-1.0.6/src/yedextended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:48:33.000000 yedextended-1.0.6/src/yedextended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 14:48:33.000000 yedextended-1.0.6/src/yedextended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 14:48:33.000000 yedextended-1.0.6/src/yedextended.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-30 14:48:24.000000 yedextended-1.0.6/test_coverage.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:48:33.485942 yedextended-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:48:24.000000 yedextended-1.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-30 14:48:24.000000 yedextended-1.0.6/tests/test_yedextended.py
```

### Comparing `yedextended-1.0.5/.github/workflows/python-publish.yml` & `yedextended-1.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/.gitignore` & `yedextended-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/LICENSE` & `yedextended-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/PKG-INFO` & `yedextended-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yedextended
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python library extending yEd functionality through programmatic interface to graphs.
 Author-email: Cole St John <info@colestjohn.com>
 Project-URL: Homepage, https://github.com/cole-st-john/yedextended
 Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,14 +19,15 @@
 Requires-Dist: openpyxl
 
 
 
 
 # Extended Python Support for yEd 
 [![CI](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml/badge.svg)](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml)
+![Test Coverage](https://raw.githubusercontent.com/cole-st-john/yedextended/master/test_coverage.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/cole-st-john/yedextended)
 <!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended?labelColor=2334D058) -->
 
 This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
 
 - [x] creating graphs
@@ -196,14 +197,16 @@
 graph_file = graph1.persist_graph("pretty_example.graphml", pretty_print=True)  #  tool specific with formatting
 
 ```
 
 
 ## Opening files in yEd Application *(assumes yEd installed and on PATH)*
 
+First install yEd application from [here](https://www.yworks.com/products/yed/download#download).
+
 ```python
 # From existing handle
 graph_file.open_with_yed(force=True)
 
 # From file path
 yed.open_yed_file("examples/test.graphml")
 ```
```

### Comparing `yedextended-1.0.5/README.md` & `yedextended-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 
 
 # Extended Python Support for yEd 
 [![CI](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml/badge.svg)](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml)
+![Test Coverage](https://raw.githubusercontent.com/cole-st-john/yedextended/master/test_coverage.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/cole-st-john/yedextended)
 <!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended?labelColor=2334D058) -->
 
 This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
 
 - [x] creating graphs
@@ -176,14 +177,16 @@
 graph_file = graph1.persist_graph("pretty_example.graphml", pretty_print=True)  #  tool specific with formatting
 
 ```
 
 
 ## Opening files in yEd Application *(assumes yEd installed and on PATH)*
 
+First install yEd application from [here](https://www.yworks.com/products/yed/download#download).
+
 ```python
 # From existing handle
 graph_file.open_with_yed(force=True)
 
 # From file path
 yed.open_yed_file("examples/test.graphml")
 ```
```

### Comparing `yedextended-1.0.5/examples/demo-basic-create-and-open.py` & `yedextended-1.0.6/examples/demo-basic-create-and-open.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/examples/demo-basic-formatting.py` & `yedextended-1.0.6/examples/demo-basic-formatting.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/examples/demo-custom-properties-nodes-edges.py` & `yedextended-1.0.6/examples/demo-custom-properties-nodes-edges.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/examples/demo-multilabels.py` & `yedextended-1.0.6/examples/demo-multilabels.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/examples/demo-uml.py` & `yedextended-1.0.6/examples/demo-uml.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/examples/demo-url-description-groups-nodes-edges.py` & `yedextended-1.0.6/examples/demo-url-description-groups-nodes-edges.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/examples/readme-3.py` & `yedextended-1.0.6/examples/readme-3.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/examples/test.graphml` & `yedextended-1.0.6/examples/test.graphml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/examples/yed_created_edges.graphml` & `yedextended-1.0.6/examples/yed_created_edges.graphml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/examples/yed_modified_app_created.graphml` & `yedextended-1.0.6/examples/yed_modified_app_created.graphml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/images/demo_multilabel.png` & `yedextended-1.0.6/images/demo_multilabel.png`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/images/example-UML.png` & `yedextended-1.0.6/images/example-UML.png`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/images/example.png` & `yedextended-1.0.6/images/example.png`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/images/excel_obj_entry.gif` & `yedextended-1.0.6/images/excel_obj_entry.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/images/excel_rel_entry.gif` & `yedextended-1.0.6/images/excel_rel_entry.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/images/graph.gif` & `yedextended-1.0.6/images/graph.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/images/graph_from_excel_obj.gif` & `yedextended-1.0.6/images/graph_from_excel_obj.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/images/graph_from_excel_rel.gif` & `yedextended-1.0.6/images/graph_from_excel_rel.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/pyproject.toml` & `yedextended-1.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -87,7 +87,44 @@
 skip-magic-trailing-comma = false
 line-ending = "auto"
 docstring-code-format = true
 docstring-code-line-length = "dynamic"
 
 [tool.ruff.lint.isort]
 case-sensitive = false
+
+
+# Performing test coverage statistics - primarily for README.md
+[tool.coverage]
+
+[tool.coverage.run]
+branch = true
+relative_files = true
+
+[tool.coverage.report]
+# Regexes for lines to exclude from consideration
+exclude_also = [
+	# Don't complain about missing debug-only code:
+	"def __repr__",
+	"if self\\.debug",
+
+	# Don't complain if tests don't hit defensive assertion code:
+	"raise AssertionError",
+	"raise NotImplementedError",
+
+	# Don't complain if non-runnable code isn't run:
+	"if 0:",
+	"if __name__ == .__main__.:",
+
+	# Don't complain about abstract methods, they aren't run:
+	"@(abc\\.)?abstractmethod",
+]
+
+ignore_errors = true
+
+
+[tool.coverage.paths]
+source = ["src/"]
+
+
+[tool.coverage.html]
+directory = "coverage_html_report"
```

### Comparing `yedextended-1.0.5/src/yedextended/__init__.py` & `yedextended-1.0.6/src/yedextended/__init__.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.5/src/yedextended.egg-info/PKG-INFO` & `yedextended-1.0.6/src/yedextended.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yedextended
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python library extending yEd functionality through programmatic interface to graphs.
 Author-email: Cole St John <info@colestjohn.com>
 Project-URL: Homepage, https://github.com/cole-st-john/yedextended
 Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,14 +19,15 @@
 Requires-Dist: openpyxl
 
 
 
 
 # Extended Python Support for yEd 
 [![CI](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml/badge.svg)](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml)
+![Test Coverage](https://raw.githubusercontent.com/cole-st-john/yedextended/master/test_coverage.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/cole-st-john/yedextended)
 <!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended?labelColor=2334D058) -->
 
 This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
 
 - [x] creating graphs
@@ -196,14 +197,16 @@
 graph_file = graph1.persist_graph("pretty_example.graphml", pretty_print=True)  #  tool specific with formatting
 
 ```
 
 
 ## Opening files in yEd Application *(assumes yEd installed and on PATH)*
 
+First install yEd application from [here](https://www.yworks.com/products/yed/download#download).
+
 ```python
 # From existing handle
 graph_file.open_with_yed(force=True)
 
 # From file path
 yed.open_yed_file("examples/test.graphml")
 ```
```

### Comparing `yedextended-1.0.5/src/yedextended.egg-info/SOURCES.txt` & `yedextended-1.0.6/src/yedextended.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+.deepsource.toml
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
+test_coverage.svg
 .github/workflows/ci.yml
 .github/workflows/python-publish.yml
 examples/demo-basic-create-and-open.py
 examples/demo-basic-formatting.py
 examples/demo-basic_bulk_manage1.py
 examples/demo-basic_bulk_manage2.py
 examples/demo-custom-properties-nodes-edges.py
```

### Comparing `yedextended-1.0.5/tests/test_yedextended.py` & `yedextended-1.0.6/tests/test_yedextended.py`

 * *Files identical despite different names*

