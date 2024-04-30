# Comparing `tmp/yedextended-1.0.1.tar.gz` & `tmp/yedextended-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yedextended-1.0.1.tar", last modified: Tue Apr 30 09:21:54 2024, max compression
+gzip compressed data, was "yedextended-1.0.2.tar", last modified: Tue Apr 30 09:36:06 2024, max compression
```

## Comparing `yedextended-1.0.1.tar` & `yedextended-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:21:54.756913 yedextended-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-30 09:21:46.000000 yedextended-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-30 09:21:54.756913 yedextended-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-30 09:21:46.000000 yedextended-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-30 09:21:46.000000 yedextended-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:21:54.756913 yedextended-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:21:54.756913 yedextended-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:21:54.756913 yedextended-1.0.1/src/yedextended/
--rw-r--r--   0 runner    (1001) docker     (127)    73127 2024-04-30 09:21:46.000000 yedextended-1.0.1/src/yedextended/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:21:54.756913 yedextended-1.0.1/src/yedextended.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-30 09:21:54.000000 yedextended-1.0.1/src/yedextended.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-30 09:21:54.000000 yedextended-1.0.1/src/yedextended.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:21:54.000000 yedextended-1.0.1/src/yedextended.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 09:21:54.000000 yedextended-1.0.1/src/yedextended.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 09:21:54.000000 yedextended-1.0.1/src/yedextended.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:21:54.756913 yedextended-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-30 09:21:46.000000 yedextended-1.0.1/tests/test_yedextended.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:36:06.847379 yedextended-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-30 09:36:02.000000 yedextended-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-30 09:36:06.847379 yedextended-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-30 09:36:02.000000 yedextended-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-30 09:36:02.000000 yedextended-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:36:06.847379 yedextended-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:36:06.847379 yedextended-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:36:06.847379 yedextended-1.0.2/src/yedextended/
+-rw-r--r--   0 runner    (1001) docker     (127)    73127 2024-04-30 09:36:02.000000 yedextended-1.0.2/src/yedextended/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:36:06.847379 yedextended-1.0.2/src/yedextended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-30 09:36:06.000000 yedextended-1.0.2/src/yedextended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-30 09:36:06.000000 yedextended-1.0.2/src/yedextended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:36:06.000000 yedextended-1.0.2/src/yedextended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 09:36:06.000000 yedextended-1.0.2/src/yedextended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 09:36:06.000000 yedextended-1.0.2/src/yedextended.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:36:06.847379 yedextended-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-30 09:36:02.000000 yedextended-1.0.2/tests/test_yedextended.py
```

### Comparing `yedextended-1.0.1/LICENSE` & `yedextended-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.1/PKG-INFO` & `yedextended-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yedextended
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python library extending yEd functionality through programmatic interface to graphs.
 Author-email: Cole St John <info@colestjohn.com>
 Project-URL: Homepage, https://github.com/cole-st-john/yedextended
 Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 - [x] reading graphs
 - [x] bulk data addition or management (MS excel-based)
 - [x] management of the yEd application (starting, killing, maximizing)
 - [ ] enforcing rules on graphs
 - [ ] addition of standard sorting methods
 - [ ] graph comparison tools
 
-![image](images/graph.gif)
+![yEd Graph](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph.gif)
 
 
 # Basic Usage
 
 Below are some basic usages of yEdExtended in interfacing with yEd and GraphML files:
 
 
@@ -149,27 +149,27 @@
 
 # Manage data in excel (add/remove/modify relations)
 graph1.manage_graph_data_in_excel(type="relations")
 ```
 
 ### Adding Objects / Groups per Excel:
 
-![Excel Object Entry](images/excel_obj_entry.gif)
+![Excel Object Entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/excel_obj_entry.gif)
 
 ### Result:
 
-![Graph result of excel data entry](images/graph_from_excel_obj.gif)
+![Graph result of excel data entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph_from_excel_obj.gif)
 
 ### Adding Relationships per Excel:
 
-![Excel Relation Entry](images/excel_rel_entry.gif)
+![Excel Relation Entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/excel_rel_entry.gif)
 
 ### Result:
 
-![Graph result of excel relation entry](images/graph_from_excel_rel.gif)
+![Graph result of excel relation entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph_from_excel_rel.gif)
 
 
 ## Possible outputs of Graph
 
 ```python
 # Demonstrate stringified GraphML version of structure
 print(graph1.stringify_graph())
```

### Comparing `yedextended-1.0.1/README.md` & `yedextended-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - [x] reading graphs
 - [x] bulk data addition or management (MS excel-based)
 - [x] management of the yEd application (starting, killing, maximizing)
 - [ ] enforcing rules on graphs
 - [ ] addition of standard sorting methods
 - [ ] graph comparison tools
 
-![image](images/graph.gif)
+![yEd Graph](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph.gif)
 
 
 # Basic Usage
 
 Below are some basic usages of yEdExtended in interfacing with yEd and GraphML files:
 
 
@@ -132,27 +132,27 @@
 
 # Manage data in excel (add/remove/modify relations)
 graph1.manage_graph_data_in_excel(type="relations")
 ```
 
 ### Adding Objects / Groups per Excel:
 
-![Excel Object Entry](images/excel_obj_entry.gif)
+![Excel Object Entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/excel_obj_entry.gif)
 
 ### Result:
 
-![Graph result of excel data entry](images/graph_from_excel_obj.gif)
+![Graph result of excel data entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph_from_excel_obj.gif)
 
 ### Adding Relationships per Excel:
 
-![Excel Relation Entry](images/excel_rel_entry.gif)
+![Excel Relation Entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/excel_rel_entry.gif)
 
 ### Result:
 
-![Graph result of excel relation entry](images/graph_from_excel_rel.gif)
+![Graph result of excel relation entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph_from_excel_rel.gif)
 
 
 ## Possible outputs of Graph
 
 ```python
 # Demonstrate stringified GraphML version of structure
 print(graph1.stringify_graph())
```

### Comparing `yedextended-1.0.1/pyproject.toml` & `yedextended-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "yedextended"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{ name = "Cole St John", email = "info@colestjohn.com" }]
 description = "Python library extending yEd functionality through programmatic interface to graphs."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = ["psutil", "pygetwindow", "openpyxl"]
 classifiers = [
 	"Programming Language :: Python :: 3",
```

### Comparing `yedextended-1.0.1/src/yedextended/__init__.py` & `yedextended-1.0.2/src/yedextended/__init__.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.1/src/yedextended.egg-info/PKG-INFO` & `yedextended-1.0.2/src/yedextended.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yedextended
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python library extending yEd functionality through programmatic interface to graphs.
 Author-email: Cole St John <info@colestjohn.com>
 Project-URL: Homepage, https://github.com/cole-st-john/yedextended
 Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 - [x] reading graphs
 - [x] bulk data addition or management (MS excel-based)
 - [x] management of the yEd application (starting, killing, maximizing)
 - [ ] enforcing rules on graphs
 - [ ] addition of standard sorting methods
 - [ ] graph comparison tools
 
-![image](images/graph.gif)
+![yEd Graph](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph.gif)
 
 
 # Basic Usage
 
 Below are some basic usages of yEdExtended in interfacing with yEd and GraphML files:
 
 
@@ -149,27 +149,27 @@
 
 # Manage data in excel (add/remove/modify relations)
 graph1.manage_graph_data_in_excel(type="relations")
 ```
 
 ### Adding Objects / Groups per Excel:
 
-![Excel Object Entry](images/excel_obj_entry.gif)
+![Excel Object Entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/excel_obj_entry.gif)
 
 ### Result:
 
-![Graph result of excel data entry](images/graph_from_excel_obj.gif)
+![Graph result of excel data entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph_from_excel_obj.gif)
 
 ### Adding Relationships per Excel:
 
-![Excel Relation Entry](images/excel_rel_entry.gif)
+![Excel Relation Entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/excel_rel_entry.gif)
 
 ### Result:
 
-![Graph result of excel relation entry](images/graph_from_excel_rel.gif)
+![Graph result of excel relation entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph_from_excel_rel.gif)
 
 
 ## Possible outputs of Graph
 
 ```python
 # Demonstrate stringified GraphML version of structure
 print(graph1.stringify_graph())
```

### Comparing `yedextended-1.0.1/tests/test_yedextended.py` & `yedextended-1.0.2/tests/test_yedextended.py`

 * *Files identical despite different names*

