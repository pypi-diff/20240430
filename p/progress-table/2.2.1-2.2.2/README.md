# Comparing `tmp/progress-table-2.2.1.tar.gz` & `tmp/progress-table-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress-table-2.2.1.tar", last modified: Mon Apr 29 18:04:41 2024, max compression
+gzip compressed data, was "progress-table-2.2.2.tar", last modified: Mon Apr 29 18:22:13 2024, max compression
```

## Comparing `progress-table-2.2.1.tar` & `progress-table-2.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:04:40.996192 progress-table-2.2.1/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-2.2.1/LICENSE.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4903 2024-04-29 18:04:40.996192 progress-table-2.2.1/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4139 2024-04-28 20:30:22.000000 progress-table-2.2.1/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:04:40.996192 progress-table-2.2.1/progress_table/
--rw-r--r--   0 gaha      (1000) gaha      (1000)      334 2024-04-29 18:02:33.000000 progress-table-2.2.1/progress_table/__init__.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:04:40.996192 progress-table-2.2.1/progress_table/v0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-05 19:18:13.000000 progress-table-2.2.1/progress_table/v0/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    23444 2024-04-05 20:02:34.000000 progress-table-2.2.1/progress_table/v0/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-2.2.1/progress_table/v0/symbols.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:04:40.996192 progress-table-2.2.1/progress_table/v1/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-2.2.1/progress_table/v1/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1500 2024-04-29 17:54:03.000000 progress-table-2.2.1/progress_table/v1/common.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    46305 2024-04-29 17:54:03.000000 progress-table-2.2.1/progress_table/v1/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     7475 2024-04-29 18:02:33.000000 progress-table-2.2.1/progress_table/v1/styles.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:04:40.996192 progress-table-2.2.1/progress_table.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4903 2024-04-29 18:04:40.000000 progress-table-2.2.1/progress_table.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-2.2.1/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
--rw-r--r--   0 gaha      (1000) gaha      (1000)      621 2024-04-29 18:04:40.000000 progress-table-2.2.1/progress_table.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-29 18:04:40.000000 progress-table-2.2.1/progress_table.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-29 18:04:40.000000 progress-table-2.2.1/progress_table.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-29 18:04:40.000000 progress-table-2.2.1/progress_table.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-2.2.1/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-29 18:04:40.996192 progress-table-2.2.1/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1504 2024-04-09 23:00:39.000000 progress-table-2.2.1/setup.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:04:40.996192 progress-table-2.2.1/tests/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1804 2024-04-06 12:00:21.000000 progress-table-2.2.1/tests/test_docs_automated.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1867 2024-04-28 20:30:31.000000 progress-table-2.2.1/tests/test_examples_automated.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:22:13.621395 progress-table-2.2.2/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-2.2.2/LICENSE.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     5159 2024-04-29 18:22:13.621395 progress-table-2.2.2/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4017 2024-04-29 18:22:09.000000 progress-table-2.2.2/README.md
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:22:13.621395 progress-table-2.2.2/progress_table/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      334 2024-04-29 18:22:09.000000 progress-table-2.2.2/progress_table/__init__.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:22:13.621395 progress-table-2.2.2/progress_table/v0/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-05 19:18:13.000000 progress-table-2.2.2/progress_table/v0/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    23444 2024-04-05 20:02:34.000000 progress-table-2.2.2/progress_table/v0/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-2.2.2/progress_table/v0/symbols.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:22:13.621395 progress-table-2.2.2/progress_table/v1/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-2.2.2/progress_table/v1/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1500 2024-04-29 17:54:03.000000 progress-table-2.2.2/progress_table/v1/common.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    46305 2024-04-29 17:54:03.000000 progress-table-2.2.2/progress_table/v1/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     7475 2024-04-29 18:02:33.000000 progress-table-2.2.2/progress_table/v1/styles.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:22:13.621395 progress-table-2.2.2/progress_table.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     5159 2024-04-29 18:22:13.000000 progress-table-2.2.2/progress_table.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-2.2.2/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      621 2024-04-29 18:22:13.000000 progress-table-2.2.2/progress_table.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-29 18:22:13.000000 progress-table-2.2.2/progress_table.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-29 18:22:13.000000 progress-table-2.2.2/progress_table.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-29 18:22:13.000000 progress-table-2.2.2/progress_table.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-2.2.2/pyproject.toml
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-29 18:22:13.621395 progress-table-2.2.2/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1725 2024-04-29 18:22:09.000000 progress-table-2.2.2/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:22:13.621395 progress-table-2.2.2/tests/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1804 2024-04-06 12:00:21.000000 progress-table-2.2.2/tests/test_docs_automated.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1867 2024-04-28 20:30:31.000000 progress-table-2.2.2/tests/test_examples_automated.py
```

### Comparing `progress-table-2.2.1/LICENSE.txt` & `progress-table-2.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.1/PKG-INFO` & `progress-table-2.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 2.2.1
+Version: 2.2.2
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -33,37 +33,37 @@
 * Alternative to TQDM whenever you want to track metrics produced by your process
 * Designed to monitor ML experiments, but works for any metrics-producing process
 * Allows you to see at a glance what's going on with your process
 * Increases readability and simplifies your command line logging
 
 ### Change this:
 
-![example](https://github.com/gahaalt/progress-table/blob/main/images/progress-before3.gif?raw=true)
+![example](https://raw.githubusercontent.com/sjmikler/progress-table/main/images/progress-before3.gif)
 
 ### Into this:
 
-![example](https://github.com/gahaalt/progress-table/blob/main/images/progress-after4.gif?raw=true)
+![example](https://raw.githubusercontent.com/sjmikler/progress-table/main/images/progress-after4.gif)
 
 ## Examples
 
 * Neural network training
 
-![example-training](images/examples-training.gif)
+![example-training](https://raw.githubusercontent.com/sjmikler/progress-table/main/images/examples-training.gif)
 
 * Progress of multi-threaded downloads
 
-![example-download](images/examples-download.gif)
+![example-download](https://raw.githubusercontent.com/sjmikler/progress-table/main/images/examples-download.gif)
 
 * Simulation and interactive display of Brownian motion
 
-![example-brown2d](images/examples-brown2d.gif)
+![example-brown2d](https://raw.githubusercontent.com/sjmikler/progress-table/main/images/examples-brown2d.gif)
 
 * Display of a game board
 
-![example-tictactoe](images/examples-tictactoe.gif)
+![example-tictactoe](https://raw.githubusercontent.com/sjmikler/progress-table/main/images/examples-tictactoe.gif)
 
 ## Quick start code
 
 ```python
 import random
 import time
```

### Comparing `progress-table-2.2.1/README.md` & `progress-table-2.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 * Alternative to TQDM whenever you want to track metrics produced by your process
 * Designed to monitor ML experiments, but works for any metrics-producing process
 * Allows you to see at a glance what's going on with your process
 * Increases readability and simplifies your command line logging
 
 ### Change this:
 
-![example](https://github.com/gahaalt/progress-table/blob/main/images/progress-before3.gif?raw=true)
+![example](images/progress-before3.gif)
 
 ### Into this:
 
-![example](https://github.com/gahaalt/progress-table/blob/main/images/progress-after4.gif?raw=true)
+![example](images/progress-after4.gif)
 
 ## Examples
 
 * Neural network training
 
 ![example-training](images/examples-training.gif)
```

### Comparing `progress-table-2.2.1/progress_table/v0/progress_table.py` & `progress-table-2.2.2/progress_table/v0/progress_table.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.1/progress_table/v0/symbols.py` & `progress-table-2.2.2/progress_table/v0/symbols.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.1/progress_table/v1/common.py` & `progress-table-2.2.2/progress_table/v1/common.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.1/progress_table/v1/progress_table.py` & `progress-table-2.2.2/progress_table/v1/progress_table.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.1/progress_table/v1/styles.py` & `progress-table-2.2.2/progress_table/v1/styles.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.1/progress_table.egg-info/PKG-INFO` & `progress-table-2.2.2/progress_table.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 2.2.1
+Version: 2.2.2
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -33,37 +33,37 @@
 * Alternative to TQDM whenever you want to track metrics produced by your process
 * Designed to monitor ML experiments, but works for any metrics-producing process
 * Allows you to see at a glance what's going on with your process
 * Increases readability and simplifies your command line logging
 
 ### Change this:
 
-![example](https://github.com/gahaalt/progress-table/blob/main/images/progress-before3.gif?raw=true)
+![example](https://raw.githubusercontent.com/sjmikler/progress-table/main/images/progress-before3.gif)
 
 ### Into this:
 
-![example](https://github.com/gahaalt/progress-table/blob/main/images/progress-after4.gif?raw=true)
+![example](https://raw.githubusercontent.com/sjmikler/progress-table/main/images/progress-after4.gif)
 
 ## Examples
 
 * Neural network training
 
-![example-training](images/examples-training.gif)
+![example-training](https://raw.githubusercontent.com/sjmikler/progress-table/main/images/examples-training.gif)
 
 * Progress of multi-threaded downloads
 
-![example-download](images/examples-download.gif)
+![example-download](https://raw.githubusercontent.com/sjmikler/progress-table/main/images/examples-download.gif)
 
 * Simulation and interactive display of Brownian motion
 
-![example-brown2d](images/examples-brown2d.gif)
+![example-brown2d](https://raw.githubusercontent.com/sjmikler/progress-table/main/images/examples-brown2d.gif)
 
 * Display of a game board
 
-![example-tictactoe](images/examples-tictactoe.gif)
+![example-tictactoe](https://raw.githubusercontent.com/sjmikler/progress-table/main/images/examples-tictactoe.gif)
 
 ## Quick start code
 
 ```python
 import random
 import time
```

### Comparing `progress-table-2.2.1/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO` & `progress-table-2.2.2/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.1/progress_table.egg-info/SOURCES.txt` & `progress-table-2.2.2/progress_table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.1/setup.py` & `progress-table-2.2.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,20 @@
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 
 long_description = package_relative_path("README.md").read_text(encoding="UTF-8")
 
+
+def with_direct_github_urls(description):
+    github_link = "https://raw.githubusercontent.com/sjmikler/progress-table/main/images"
+    return description.replace("(images", "(" + github_link)
+
+
 setup(
     name="progress-table",
     version=get_version(),
     url="https://github.com/gahaalt/progress-table.git",
     author="Szymon Mikler",
     author_email="sjmikler@gmail.com",
     license="MIT",
@@ -38,10 +44,10 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     install_requires=["colorama"],
-    long_description=long_description,
+    long_description=with_direct_github_urls(long_description),
     long_description_content_type="text/markdown",
 )
```

### Comparing `progress-table-2.2.1/tests/test_docs_automated.py` & `progress-table-2.2.2/tests/test_docs_automated.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.1/tests/test_examples_automated.py` & `progress-table-2.2.2/tests/test_examples_automated.py`

 * *Files identical despite different names*

