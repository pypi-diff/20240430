# Comparing `tmp/scrawlpy-0.0.2.tar.gz` & `tmp/scrawlpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrawlpy-0.0.2.tar", last modified: Tue Apr 30 04:03:24 2024, max compression
+gzip compressed data, was "scrawlpy-0.0.3.tar", last modified: Tue Apr 30 08:31:14 2024, max compression
```

## Comparing `scrawlpy-0.0.2.tar` & `scrawlpy-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 04:03:24.941641 scrawlpy-0.0.2/
--rw-r--r--   0 wu         (501) staff       (20)      906 2024-04-30 04:03:24.941426 scrawlpy-0.0.2/PKG-INFO
--rw-r--r--   0 wu         (501) staff       (20)       66 2024-04-30 03:52:44.000000 scrawlpy-0.0.2/README.md
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 04:03:24.935861 scrawlpy-0.0.2/scrawlpy/
--rw-r--r--   0 wu         (501) staff       (20)      135 2024-04-30 03:46:59.000000 scrawlpy-0.0.2/scrawlpy/__init__.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 04:03:24.937539 scrawlpy-0.0.2/scrawlpy/commands/
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     3824 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/cmdline.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 04:03:24.939257 scrawlpy-0.0.2/scrawlpy/commands/create/
--rw-r--r--   0 wu         (501) staff       (20)      543 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/create/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      975 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/create/create_cookies.py
--rw-r--r--   0 wu         (501) staff       (20)      670 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/create/create_init.py
--rw-r--r--   0 wu         (501) staff       (20)     6004 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/create/create_item.py
--rw-r--r--   0 wu         (501) staff       (20)     1366 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/create/create_json.py
--rw-r--r--   0 wu         (501) staff       (20)     1106 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/create/create_params.py
--rw-r--r--   0 wu         (501) staff       (20)     1360 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/create/create_project.py
--rw-r--r--   0 wu         (501) staff       (20)      693 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/create/create_setting.py
--rw-r--r--   0 wu         (501) staff       (20)     3648 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/create/create_spider.py
--rw-r--r--   0 wu         (501) staff       (20)     4288 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/create/create_table.py
--rw-r--r--   0 wu         (501) staff       (20)     3986 2024-04-30 03:46:59.000000 scrawlpy-0.0.2/scrawlpy/commands/create_builder.py
--rw-r--r--   0 wu         (501) staff       (20)     1356 2024-04-30 03:46:59.000000 scrawlpy-0.0.2/scrawlpy/commands/retry.py
--rw-r--r--   0 wu         (501) staff       (20)     5514 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/shell.py
--rw-r--r--   0 wu         (501) staff       (20)     2572 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/commands/zip.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 04:03:24.939571 scrawlpy-0.0.2/scrawlpy/core/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:29:09.000000 scrawlpy-0.0.2/scrawlpy/core/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      705 2024-04-30 03:46:59.000000 scrawlpy-0.0.2/scrawlpy/core/base_spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 04:03:24.939837 scrawlpy-0.0.2/scrawlpy/core/spiders/
--rw-r--r--   0 wu         (501) staff       (20)      125 2024-04-30 03:46:59.000000 scrawlpy-0.0.2/scrawlpy/core/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      306 2024-04-30 03:46:59.000000 scrawlpy-0.0.2/scrawlpy/core/spiders/spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 04:03:24.940106 scrawlpy-0.0.2/scrawlpy/http/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-29 15:39:00.000000 scrawlpy-0.0.2/scrawlpy/http/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     7206 2024-04-28 08:57:54.000000 scrawlpy-0.0.2/scrawlpy/http/request.py
--rw-r--r--   0 wu         (501) staff       (20)    11219 2024-04-28 08:11:46.000000 scrawlpy-0.0.2/scrawlpy/setting.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 04:03:24.940270 scrawlpy-0.0.2/scrawlpy/test/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.2/scrawlpy/test/__init__.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 04:03:24.940559 scrawlpy-0.0.2/scrawlpy/test/spiders/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.2/scrawlpy/test/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      326 2024-04-30 03:46:59.000000 scrawlpy-0.0.2/scrawlpy/test/spiders/spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 04:03:24.936737 scrawlpy-0.0.2/scrawlpy.egg-info/
--rw-r--r--   0 wu         (501) staff       (20)      906 2024-04-30 04:03:24.000000 scrawlpy-0.0.2/scrawlpy.egg-info/PKG-INFO
--rw-r--r--   0 wu         (501) staff       (20)     1122 2024-04-30 04:03:24.000000 scrawlpy-0.0.2/scrawlpy.egg-info/SOURCES.txt
--rw-r--r--   0 wu         (501) staff       (20)        1 2024-04-30 04:03:24.000000 scrawlpy-0.0.2/scrawlpy.egg-info/dependency_links.txt
--rw-r--r--   0 wu         (501) staff       (20)       63 2024-04-30 04:03:24.000000 scrawlpy-0.0.2/scrawlpy.egg-info/entry_points.txt
--rw-r--r--   0 wu         (501) staff       (20)      214 2024-04-30 04:03:24.000000 scrawlpy-0.0.2/scrawlpy.egg-info/requires.txt
--rw-r--r--   0 wu         (501) staff       (20)       17 2024-04-30 04:03:24.000000 scrawlpy-0.0.2/scrawlpy.egg-info/top_level.txt
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 04:03:24.940693 scrawlpy-0.0.2/scripts/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:23:17.000000 scrawlpy-0.0.2/scripts/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)       38 2024-04-30 04:03:24.941691 scrawlpy-0.0.2/setup.cfg
--rw-r--r--   0 wu         (501) staff       (20)     1748 2024-04-30 04:03:22.000000 scrawlpy-0.0.2/setup.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:31:14.421020 scrawlpy-0.0.3/
+-rw-r--r--   0 wu         (501) staff       (20)      906 2024-04-30 08:31:14.420725 scrawlpy-0.0.3/PKG-INFO
+-rw-r--r--   0 wu         (501) staff       (20)       66 2024-04-30 03:52:44.000000 scrawlpy-0.0.3/README.md
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:31:14.411514 scrawlpy-0.0.3/scrawlpy/
+-rw-r--r--   0 wu         (501) staff       (20)      135 2024-04-30 03:46:59.000000 scrawlpy-0.0.3/scrawlpy/__init__.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:31:14.414202 scrawlpy-0.0.3/scrawlpy/commands/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     3824 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/cmdline.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:31:14.417130 scrawlpy-0.0.3/scrawlpy/commands/create/
+-rw-r--r--   0 wu         (501) staff       (20)      543 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/create/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      975 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/create/create_cookies.py
+-rw-r--r--   0 wu         (501) staff       (20)      670 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/create/create_init.py
+-rw-r--r--   0 wu         (501) staff       (20)     6004 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/create/create_item.py
+-rw-r--r--   0 wu         (501) staff       (20)     1366 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/create/create_json.py
+-rw-r--r--   0 wu         (501) staff       (20)     1106 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/create/create_params.py
+-rw-r--r--   0 wu         (501) staff       (20)     1360 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/create/create_project.py
+-rw-r--r--   0 wu         (501) staff       (20)      693 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/create/create_setting.py
+-rw-r--r--   0 wu         (501) staff       (20)     3648 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/create/create_spider.py
+-rw-r--r--   0 wu         (501) staff       (20)     4288 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/create/create_table.py
+-rw-r--r--   0 wu         (501) staff       (20)     3986 2024-04-30 03:46:59.000000 scrawlpy-0.0.3/scrawlpy/commands/create_builder.py
+-rw-r--r--   0 wu         (501) staff       (20)     1356 2024-04-30 03:46:59.000000 scrawlpy-0.0.3/scrawlpy/commands/retry.py
+-rw-r--r--   0 wu         (501) staff       (20)     5514 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/shell.py
+-rw-r--r--   0 wu         (501) staff       (20)     2572 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/commands/zip.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:31:14.417811 scrawlpy-0.0.3/scrawlpy/core/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:29:09.000000 scrawlpy-0.0.3/scrawlpy/core/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      705 2024-04-30 03:46:59.000000 scrawlpy-0.0.3/scrawlpy/core/base_spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:31:14.418227 scrawlpy-0.0.3/scrawlpy/core/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)      125 2024-04-30 03:46:59.000000 scrawlpy-0.0.3/scrawlpy/core/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      306 2024-04-30 03:46:59.000000 scrawlpy-0.0.3/scrawlpy/core/spiders/spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:31:14.418700 scrawlpy-0.0.3/scrawlpy/http/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-29 15:39:00.000000 scrawlpy-0.0.3/scrawlpy/http/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     7206 2024-04-28 08:57:54.000000 scrawlpy-0.0.3/scrawlpy/http/request.py
+-rw-r--r--   0 wu         (501) staff       (20)    11219 2024-04-28 08:11:46.000000 scrawlpy-0.0.3/scrawlpy/setting.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:31:14.419094 scrawlpy-0.0.3/scrawlpy/test/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.3/scrawlpy/test/__init__.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:31:14.419614 scrawlpy-0.0.3/scrawlpy/test/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.3/scrawlpy/test/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      326 2024-04-30 03:46:59.000000 scrawlpy-0.0.3/scrawlpy/test/spiders/spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:31:14.412594 scrawlpy-0.0.3/scrawlpy.egg-info/
+-rw-r--r--   0 wu         (501) staff       (20)      906 2024-04-30 08:31:14.000000 scrawlpy-0.0.3/scrawlpy.egg-info/PKG-INFO
+-rw-r--r--   0 wu         (501) staff       (20)     1122 2024-04-30 08:31:14.000000 scrawlpy-0.0.3/scrawlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 wu         (501) staff       (20)        1 2024-04-30 08:31:14.000000 scrawlpy-0.0.3/scrawlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 wu         (501) staff       (20)       63 2024-04-30 08:31:14.000000 scrawlpy-0.0.3/scrawlpy.egg-info/entry_points.txt
+-rw-r--r--   0 wu         (501) staff       (20)      214 2024-04-30 08:31:14.000000 scrawlpy-0.0.3/scrawlpy.egg-info/requires.txt
+-rw-r--r--   0 wu         (501) staff       (20)       17 2024-04-30 08:31:14.000000 scrawlpy-0.0.3/scrawlpy.egg-info/top_level.txt
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:31:14.419787 scrawlpy-0.0.3/scripts/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:23:17.000000 scrawlpy-0.0.3/scripts/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)       38 2024-04-30 08:31:14.421094 scrawlpy-0.0.3/setup.cfg
+-rw-r--r--   0 wu         (501) staff       (20)     1732 2024-04-30 08:30:08.000000 scrawlpy-0.0.3/setup.py
```

### Comparing `scrawlpy-0.0.2/PKG-INFO` & `scrawlpy-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrawlpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: scrawlpy是一款python爬虫框架
 Author: Jayden
 Author-email: jayden@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/cmdline.py` & `scrawlpy-0.0.3/scrawlpy/commands/cmdline.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/create/__init__.py` & `scrawlpy-0.0.3/scrawlpy/commands/create/__init__.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/create/create_cookies.py` & `scrawlpy-0.0.3/scrawlpy/commands/create/create_cookies.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/create/create_init.py` & `scrawlpy-0.0.3/scrawlpy/commands/create/create_init.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/create/create_item.py` & `scrawlpy-0.0.3/scrawlpy/commands/create/create_item.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/create/create_json.py` & `scrawlpy-0.0.3/scrawlpy/commands/create/create_json.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/create/create_params.py` & `scrawlpy-0.0.3/scrawlpy/commands/create/create_params.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/create/create_project.py` & `scrawlpy-0.0.3/scrawlpy/commands/create/create_project.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/create/create_setting.py` & `scrawlpy-0.0.3/scrawlpy/commands/create/create_setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/create/create_spider.py` & `scrawlpy-0.0.3/scrawlpy/commands/create/create_spider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/create/create_table.py` & `scrawlpy-0.0.3/scrawlpy/commands/create/create_table.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/create_builder.py` & `scrawlpy-0.0.3/scrawlpy/commands/create_builder.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/retry.py` & `scrawlpy-0.0.3/scrawlpy/commands/retry.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/shell.py` & `scrawlpy-0.0.3/scrawlpy/commands/shell.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/commands/zip.py` & `scrawlpy-0.0.3/scrawlpy/commands/zip.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/core/base_spider.py` & `scrawlpy-0.0.3/scrawlpy/core/base_spider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/http/request.py` & `scrawlpy-0.0.3/scrawlpy/http/request.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy/setting.py` & `scrawlpy-0.0.3/scrawlpy/setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/scrawlpy.egg-info/PKG-INFO` & `scrawlpy-0.0.3/scrawlpy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrawlpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: scrawlpy是一款python爬虫框架
 Author: Jayden
 Author-email: jayden@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scrawlpy-0.0.2/scrawlpy.egg-info/SOURCES.txt` & `scrawlpy-0.0.3/scrawlpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.2/setup.py` & `scrawlpy-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 from os.path import dirname, join
 from sys import version_info
 
 import setuptools
 
 if version_info < (3, 6, 0):
-    raise SystemExit("Sorry! feapder requires python 3.6.0 or later.")
+    raise SystemExit("Sorry! scrawlpy requires python 3.6.0 or later.")
 
-with open(join(dirname(__file__), "scrawlpy/VERSION"), "rb") as fh:
-    version = fh.read().decode("ascii").strip()
+with open(join(dirname(__file__), "scrawlpy/VERSION"), "r") as fh:
+    version = fh.read().strip()
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 packages = setuptools.find_packages()
 packages.extend(
     [
@@ -48,15 +48,15 @@
     "PyExecJS>=1.5.1",
     "pymongo>=3.10.1",
     "redis-py-cluster>=2.1.0",
 ] + render_requires
 
 setuptools.setup(
     name="scrawlpy",
-    version="0.0.2",
+    version=version,
     author="Jayden",
     license="MIT",
     author_email="jayden@qq.com",
     python_requires=">=3.6",
     description="scrawlpy是一款python爬虫框架",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

