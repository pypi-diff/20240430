# Comparing `tmp/scrawlpy-0.0.4.tar.gz` & `tmp/scrawlpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrawlpy-0.0.4.tar", last modified: Tue Apr 30 08:32:28 2024, max compression
+gzip compressed data, was "scrawlpy-0.0.5.tar", last modified: Tue Apr 30 08:34:00 2024, max compression
```

## Comparing `scrawlpy-0.0.4.tar` & `scrawlpy-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:32:28.403879 scrawlpy-0.0.4/
--rw-r--r--   0 wu         (501) staff       (20)      906 2024-04-30 08:32:28.403610 scrawlpy-0.0.4/PKG-INFO
--rw-r--r--   0 wu         (501) staff       (20)       66 2024-04-30 03:52:44.000000 scrawlpy-0.0.4/README.md
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:32:28.394165 scrawlpy-0.0.4/scrawlpy/
--rw-r--r--   0 wu         (501) staff       (20)      135 2024-04-30 03:46:59.000000 scrawlpy-0.0.4/scrawlpy/__init__.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:32:28.396969 scrawlpy-0.0.4/scrawlpy/commands/
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     3824 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/cmdline.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:32:28.399822 scrawlpy-0.0.4/scrawlpy/commands/create/
--rw-r--r--   0 wu         (501) staff       (20)      543 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/create/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      975 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/create/create_cookies.py
--rw-r--r--   0 wu         (501) staff       (20)      670 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/create/create_init.py
--rw-r--r--   0 wu         (501) staff       (20)     6004 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/create/create_item.py
--rw-r--r--   0 wu         (501) staff       (20)     1366 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/create/create_json.py
--rw-r--r--   0 wu         (501) staff       (20)     1106 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/create/create_params.py
--rw-r--r--   0 wu         (501) staff       (20)     1360 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/create/create_project.py
--rw-r--r--   0 wu         (501) staff       (20)      693 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/create/create_setting.py
--rw-r--r--   0 wu         (501) staff       (20)     3648 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/create/create_spider.py
--rw-r--r--   0 wu         (501) staff       (20)     4288 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/create/create_table.py
--rw-r--r--   0 wu         (501) staff       (20)     3986 2024-04-30 03:46:59.000000 scrawlpy-0.0.4/scrawlpy/commands/create_builder.py
--rw-r--r--   0 wu         (501) staff       (20)     1356 2024-04-30 03:46:59.000000 scrawlpy-0.0.4/scrawlpy/commands/retry.py
--rw-r--r--   0 wu         (501) staff       (20)     5514 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/shell.py
--rw-r--r--   0 wu         (501) staff       (20)     2572 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/commands/zip.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:32:28.400569 scrawlpy-0.0.4/scrawlpy/core/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:29:09.000000 scrawlpy-0.0.4/scrawlpy/core/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      705 2024-04-30 03:46:59.000000 scrawlpy-0.0.4/scrawlpy/core/base_spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:32:28.401095 scrawlpy-0.0.4/scrawlpy/core/spiders/
--rw-r--r--   0 wu         (501) staff       (20)      125 2024-04-30 03:46:59.000000 scrawlpy-0.0.4/scrawlpy/core/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      306 2024-04-30 03:46:59.000000 scrawlpy-0.0.4/scrawlpy/core/spiders/spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:32:28.401673 scrawlpy-0.0.4/scrawlpy/http/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-29 15:39:00.000000 scrawlpy-0.0.4/scrawlpy/http/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     7206 2024-04-28 08:57:54.000000 scrawlpy-0.0.4/scrawlpy/http/request.py
--rw-r--r--   0 wu         (501) staff       (20)    11219 2024-04-28 08:11:46.000000 scrawlpy-0.0.4/scrawlpy/setting.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:32:28.402027 scrawlpy-0.0.4/scrawlpy/test/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.4/scrawlpy/test/__init__.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:32:28.402526 scrawlpy-0.0.4/scrawlpy/test/spiders/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.4/scrawlpy/test/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      326 2024-04-30 03:46:59.000000 scrawlpy-0.0.4/scrawlpy/test/spiders/spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:32:28.395410 scrawlpy-0.0.4/scrawlpy.egg-info/
--rw-r--r--   0 wu         (501) staff       (20)      906 2024-04-30 08:32:28.000000 scrawlpy-0.0.4/scrawlpy.egg-info/PKG-INFO
--rw-r--r--   0 wu         (501) staff       (20)     1122 2024-04-30 08:32:28.000000 scrawlpy-0.0.4/scrawlpy.egg-info/SOURCES.txt
--rw-r--r--   0 wu         (501) staff       (20)        1 2024-04-30 08:32:28.000000 scrawlpy-0.0.4/scrawlpy.egg-info/dependency_links.txt
--rw-r--r--   0 wu         (501) staff       (20)       63 2024-04-30 08:32:28.000000 scrawlpy-0.0.4/scrawlpy.egg-info/entry_points.txt
--rw-r--r--   0 wu         (501) staff       (20)      214 2024-04-30 08:32:28.000000 scrawlpy-0.0.4/scrawlpy.egg-info/requires.txt
--rw-r--r--   0 wu         (501) staff       (20)       17 2024-04-30 08:32:28.000000 scrawlpy-0.0.4/scrawlpy.egg-info/top_level.txt
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:32:28.402679 scrawlpy-0.0.4/scripts/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:23:17.000000 scrawlpy-0.0.4/scripts/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)       38 2024-04-30 08:32:28.403933 scrawlpy-0.0.4/setup.cfg
--rw-r--r--   0 wu         (501) staff       (20)     1736 2024-04-30 08:32:26.000000 scrawlpy-0.0.4/setup.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.347743 scrawlpy-0.0.5/
+-rw-r--r--   0 wu         (501) staff       (20)      906 2024-04-30 08:34:00.347487 scrawlpy-0.0.5/PKG-INFO
+-rw-r--r--   0 wu         (501) staff       (20)       66 2024-04-30 03:52:44.000000 scrawlpy-0.0.5/README.md
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.337457 scrawlpy-0.0.5/scrawlpy/
+-rw-r--r--   0 wu         (501) staff       (20)      135 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/__init__.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.340320 scrawlpy-0.0.5/scrawlpy/commands/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     3824 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/cmdline.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.343603 scrawlpy-0.0.5/scrawlpy/commands/create/
+-rw-r--r--   0 wu         (501) staff       (20)      543 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      975 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_cookies.py
+-rw-r--r--   0 wu         (501) staff       (20)      670 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_init.py
+-rw-r--r--   0 wu         (501) staff       (20)     6004 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_item.py
+-rw-r--r--   0 wu         (501) staff       (20)     1366 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_json.py
+-rw-r--r--   0 wu         (501) staff       (20)     1106 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_params.py
+-rw-r--r--   0 wu         (501) staff       (20)     1360 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_project.py
+-rw-r--r--   0 wu         (501) staff       (20)      693 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_setting.py
+-rw-r--r--   0 wu         (501) staff       (20)     3648 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_spider.py
+-rw-r--r--   0 wu         (501) staff       (20)     4288 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_table.py
+-rw-r--r--   0 wu         (501) staff       (20)     3986 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/commands/create_builder.py
+-rw-r--r--   0 wu         (501) staff       (20)     1356 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/commands/retry.py
+-rw-r--r--   0 wu         (501) staff       (20)     5514 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/shell.py
+-rw-r--r--   0 wu         (501) staff       (20)     2572 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/zip.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.344299 scrawlpy-0.0.5/scrawlpy/core/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:29:09.000000 scrawlpy-0.0.5/scrawlpy/core/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      705 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/core/base_spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.344777 scrawlpy-0.0.5/scrawlpy/core/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)      125 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/core/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      306 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/core/spiders/spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.345407 scrawlpy-0.0.5/scrawlpy/http/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-29 15:39:00.000000 scrawlpy-0.0.5/scrawlpy/http/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     7206 2024-04-28 08:57:54.000000 scrawlpy-0.0.5/scrawlpy/http/request.py
+-rw-r--r--   0 wu         (501) staff       (20)    11219 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/setting.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.345750 scrawlpy-0.0.5/scrawlpy/test/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.5/scrawlpy/test/__init__.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.346286 scrawlpy-0.0.5/scrawlpy/test/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.5/scrawlpy/test/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      326 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/test/spiders/spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.338813 scrawlpy-0.0.5/scrawlpy.egg-info/
+-rw-r--r--   0 wu         (501) staff       (20)      906 2024-04-30 08:34:00.000000 scrawlpy-0.0.5/scrawlpy.egg-info/PKG-INFO
+-rw-r--r--   0 wu         (501) staff       (20)     1122 2024-04-30 08:34:00.000000 scrawlpy-0.0.5/scrawlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 wu         (501) staff       (20)        1 2024-04-30 08:34:00.000000 scrawlpy-0.0.5/scrawlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 wu         (501) staff       (20)       63 2024-04-30 08:34:00.000000 scrawlpy-0.0.5/scrawlpy.egg-info/entry_points.txt
+-rw-r--r--   0 wu         (501) staff       (20)      214 2024-04-30 08:34:00.000000 scrawlpy-0.0.5/scrawlpy.egg-info/requires.txt
+-rw-r--r--   0 wu         (501) staff       (20)       17 2024-04-30 08:34:00.000000 scrawlpy-0.0.5/scrawlpy.egg-info/top_level.txt
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.346486 scrawlpy-0.0.5/scripts/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:23:17.000000 scrawlpy-0.0.5/scripts/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)       38 2024-04-30 08:34:00.347800 scrawlpy-0.0.5/setup.cfg
+-rw-r--r--   0 wu         (501) staff       (20)     1732 2024-04-30 08:33:59.000000 scrawlpy-0.0.5/setup.py
```

### Comparing `scrawlpy-0.0.4/PKG-INFO` & `scrawlpy-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrawlpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: scrawlpy是一款python爬虫框架
 Author: Jayden
 Author-email: jayden@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/cmdline.py` & `scrawlpy-0.0.5/scrawlpy/commands/cmdline.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/create/__init__.py` & `scrawlpy-0.0.5/scrawlpy/commands/create/__init__.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/create/create_cookies.py` & `scrawlpy-0.0.5/scrawlpy/commands/create/create_cookies.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/create/create_init.py` & `scrawlpy-0.0.5/scrawlpy/commands/create/create_init.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/create/create_item.py` & `scrawlpy-0.0.5/scrawlpy/commands/create/create_item.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/create/create_json.py` & `scrawlpy-0.0.5/scrawlpy/commands/create/create_json.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/create/create_params.py` & `scrawlpy-0.0.5/scrawlpy/commands/create/create_params.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/create/create_project.py` & `scrawlpy-0.0.5/scrawlpy/commands/create/create_project.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/create/create_setting.py` & `scrawlpy-0.0.5/scrawlpy/commands/create/create_setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/create/create_spider.py` & `scrawlpy-0.0.5/scrawlpy/commands/create/create_spider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/create/create_table.py` & `scrawlpy-0.0.5/scrawlpy/commands/create/create_table.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/create_builder.py` & `scrawlpy-0.0.5/scrawlpy/commands/create_builder.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/retry.py` & `scrawlpy-0.0.5/scrawlpy/commands/retry.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/shell.py` & `scrawlpy-0.0.5/scrawlpy/commands/shell.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/commands/zip.py` & `scrawlpy-0.0.5/scrawlpy/commands/zip.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/core/base_spider.py` & `scrawlpy-0.0.5/scrawlpy/core/base_spider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/http/request.py` & `scrawlpy-0.0.5/scrawlpy/http/request.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy/setting.py` & `scrawlpy-0.0.5/scrawlpy/setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/scrawlpy.egg-info/PKG-INFO` & `scrawlpy-0.0.5/scrawlpy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrawlpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: scrawlpy是一款python爬虫框架
 Author: Jayden
 Author-email: jayden@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scrawlpy-0.0.4/scrawlpy.egg-info/SOURCES.txt` & `scrawlpy-0.0.5/scrawlpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.4/setup.py` & `scrawlpy-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from sys import version_info
 
 import setuptools
 
 if version_info < (3, 6, 0):
     raise SystemExit("Sorry! scrawlpy requires python 3.6.0 or later.")
 
-# with open(join(dirname(__file__), "scrawlpy/VERSION"), "r") as fh:
-#     version = fh.read().strip()
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
-    version="0.0.4",
+    version="0.0.5",
     author="Jayden",
     license="MIT",
     author_email="jayden@qq.com",
     python_requires=">=3.6",
     description="scrawlpy是一款python爬虫框架",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

