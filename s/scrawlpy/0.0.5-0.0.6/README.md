# Comparing `tmp/scrawlpy-0.0.5.tar.gz` & `tmp/scrawlpy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrawlpy-0.0.5.tar", last modified: Tue Apr 30 08:34:00 2024, max compression
+gzip compressed data, was "scrawlpy-0.0.6.tar", last modified: Tue Apr 30 08:41:14 2024, max compression
```

## Comparing `scrawlpy-0.0.5.tar` & `scrawlpy-0.0.6.tar`

### file list

```diff
@@ -1,49 +1,69 @@
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.347743 scrawlpy-0.0.5/
--rw-r--r--   0 wu         (501) staff       (20)      906 2024-04-30 08:34:00.347487 scrawlpy-0.0.5/PKG-INFO
--rw-r--r--   0 wu         (501) staff       (20)       66 2024-04-30 03:52:44.000000 scrawlpy-0.0.5/README.md
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.337457 scrawlpy-0.0.5/scrawlpy/
--rw-r--r--   0 wu         (501) staff       (20)      135 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/__init__.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.340320 scrawlpy-0.0.5/scrawlpy/commands/
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     3824 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/cmdline.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.343603 scrawlpy-0.0.5/scrawlpy/commands/create/
--rw-r--r--   0 wu         (501) staff       (20)      543 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      975 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_cookies.py
--rw-r--r--   0 wu         (501) staff       (20)      670 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_init.py
--rw-r--r--   0 wu         (501) staff       (20)     6004 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_item.py
--rw-r--r--   0 wu         (501) staff       (20)     1366 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_json.py
--rw-r--r--   0 wu         (501) staff       (20)     1106 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_params.py
--rw-r--r--   0 wu         (501) staff       (20)     1360 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_project.py
--rw-r--r--   0 wu         (501) staff       (20)      693 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_setting.py
--rw-r--r--   0 wu         (501) staff       (20)     3648 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_spider.py
--rw-r--r--   0 wu         (501) staff       (20)     4288 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/create/create_table.py
--rw-r--r--   0 wu         (501) staff       (20)     3986 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/commands/create_builder.py
--rw-r--r--   0 wu         (501) staff       (20)     1356 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/commands/retry.py
--rw-r--r--   0 wu         (501) staff       (20)     5514 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/shell.py
--rw-r--r--   0 wu         (501) staff       (20)     2572 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/commands/zip.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.344299 scrawlpy-0.0.5/scrawlpy/core/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:29:09.000000 scrawlpy-0.0.5/scrawlpy/core/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      705 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/core/base_spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.344777 scrawlpy-0.0.5/scrawlpy/core/spiders/
--rw-r--r--   0 wu         (501) staff       (20)      125 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/core/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      306 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/core/spiders/spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.345407 scrawlpy-0.0.5/scrawlpy/http/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-29 15:39:00.000000 scrawlpy-0.0.5/scrawlpy/http/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     7206 2024-04-28 08:57:54.000000 scrawlpy-0.0.5/scrawlpy/http/request.py
--rw-r--r--   0 wu         (501) staff       (20)    11219 2024-04-28 08:11:46.000000 scrawlpy-0.0.5/scrawlpy/setting.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.345750 scrawlpy-0.0.5/scrawlpy/test/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.5/scrawlpy/test/__init__.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.346286 scrawlpy-0.0.5/scrawlpy/test/spiders/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.5/scrawlpy/test/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      326 2024-04-30 03:46:59.000000 scrawlpy-0.0.5/scrawlpy/test/spiders/spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.338813 scrawlpy-0.0.5/scrawlpy.egg-info/
--rw-r--r--   0 wu         (501) staff       (20)      906 2024-04-30 08:34:00.000000 scrawlpy-0.0.5/scrawlpy.egg-info/PKG-INFO
--rw-r--r--   0 wu         (501) staff       (20)     1122 2024-04-30 08:34:00.000000 scrawlpy-0.0.5/scrawlpy.egg-info/SOURCES.txt
--rw-r--r--   0 wu         (501) staff       (20)        1 2024-04-30 08:34:00.000000 scrawlpy-0.0.5/scrawlpy.egg-info/dependency_links.txt
--rw-r--r--   0 wu         (501) staff       (20)       63 2024-04-30 08:34:00.000000 scrawlpy-0.0.5/scrawlpy.egg-info/entry_points.txt
--rw-r--r--   0 wu         (501) staff       (20)      214 2024-04-30 08:34:00.000000 scrawlpy-0.0.5/scrawlpy.egg-info/requires.txt
--rw-r--r--   0 wu         (501) staff       (20)       17 2024-04-30 08:34:00.000000 scrawlpy-0.0.5/scrawlpy.egg-info/top_level.txt
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:34:00.346486 scrawlpy-0.0.5/scripts/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:23:17.000000 scrawlpy-0.0.5/scripts/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)       38 2024-04-30 08:34:00.347800 scrawlpy-0.0.5/setup.cfg
--rw-r--r--   0 wu         (501) staff       (20)     1732 2024-04-30 08:33:59.000000 scrawlpy-0.0.5/setup.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.249121 scrawlpy-0.0.6/
+-rw-r--r--   0 wu         (501) staff       (20)     1102 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/LICENSE
+-rw-r--r--   0 wu         (501) staff       (20)      235 2024-04-30 08:40:25.000000 scrawlpy-0.0.6/MANIFEST.in
+-rw-r--r--   0 wu         (501) staff       (20)      928 2024-04-30 08:41:14.248839 scrawlpy-0.0.6/PKG-INFO
+-rw-r--r--   0 wu         (501) staff       (20)       66 2024-04-30 03:52:44.000000 scrawlpy-0.0.6/README.md
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.237231 scrawlpy-0.0.6/scrawlpy/
+-rw-r--r--   0 wu         (501) staff       (20)        5 2024-04-30 08:41:12.000000 scrawlpy-0.0.6/scrawlpy/VERSION
+-rw-r--r--   0 wu         (501) staff       (20)      135 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/scrawlpy/__init__.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.239877 scrawlpy-0.0.6/scrawlpy/commands/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     3824 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/cmdline.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.242538 scrawlpy-0.0.6/scrawlpy/commands/create/
+-rw-r--r--   0 wu         (501) staff       (20)      543 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      975 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_cookies.py
+-rw-r--r--   0 wu         (501) staff       (20)      670 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_init.py
+-rw-r--r--   0 wu         (501) staff       (20)     6004 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_item.py
+-rw-r--r--   0 wu         (501) staff       (20)     1366 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_json.py
+-rw-r--r--   0 wu         (501) staff       (20)     1106 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_params.py
+-rw-r--r--   0 wu         (501) staff       (20)     1360 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_project.py
+-rw-r--r--   0 wu         (501) staff       (20)      693 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_setting.py
+-rw-r--r--   0 wu         (501) staff       (20)     3648 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_spider.py
+-rw-r--r--   0 wu         (501) staff       (20)     4288 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_table.py
+-rw-r--r--   0 wu         (501) staff       (20)     3986 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/scrawlpy/commands/create_builder.py
+-rw-r--r--   0 wu         (501) staff       (20)     1356 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/scrawlpy/commands/retry.py
+-rw-r--r--   0 wu         (501) staff       (20)     5514 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/shell.py
+-rw-r--r--   0 wu         (501) staff       (20)     2572 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/zip.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.243084 scrawlpy-0.0.6/scrawlpy/core/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:29:09.000000 scrawlpy-0.0.6/scrawlpy/core/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      705 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/scrawlpy/core/base_spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.243420 scrawlpy-0.0.6/scrawlpy/core/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)      125 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/scrawlpy/core/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      306 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/scrawlpy/core/spiders/spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.243839 scrawlpy-0.0.6/scrawlpy/http/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-29 15:39:00.000000 scrawlpy-0.0.6/scrawlpy/http/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     7206 2024-04-28 08:57:54.000000 scrawlpy-0.0.6/scrawlpy/http/request.py
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-30 08:37:28.000000 scrawlpy-0.0.6/scrawlpy/requirements.txt
+-rw-r--r--   0 wu         (501) staff       (20)    11219 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/setting.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.245542 scrawlpy-0.0.6/scrawlpy/templates/
+-rw-r--r--   0 wu         (501) staff       (20)      592 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/air_spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)     2083 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/batch_spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)      353 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/item_template.tmpl
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.246206 scrawlpy-0.0.6/scrawlpy/templates/project_template/
+-rw-r--r--   0 wu         (501) staff       (20)     1574 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/project_template/CHECK_DATA.md
+-rw-r--r--   0 wu         (501) staff       (20)       81 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/project_template/README.md
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.246513 scrawlpy-0.0.6/scrawlpy/templates/project_template/items/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/project_template/items/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     2089 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/project_template/main.py
+-rw-r--r--   0 wu         (501) staff       (20)     9207 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/project_template/setting.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.246613 scrawlpy-0.0.6/scrawlpy/templates/project_template/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/project_template/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      805 2024-04-28 08:40:08.000000 scrawlpy-0.0.6/scrawlpy/templates/spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)     2336 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/task_spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)      365 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/update_item_template.tmpl
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.238393 scrawlpy-0.0.6/scrawlpy.egg-info/
+-rw-r--r--   0 wu         (501) staff       (20)      928 2024-04-30 08:41:14.000000 scrawlpy-0.0.6/scrawlpy.egg-info/PKG-INFO
+-rw-r--r--   0 wu         (501) staff       (20)     1713 2024-04-30 08:41:14.000000 scrawlpy-0.0.6/scrawlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 wu         (501) staff       (20)        1 2024-04-30 08:41:14.000000 scrawlpy-0.0.6/scrawlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 wu         (501) staff       (20)       63 2024-04-30 08:41:14.000000 scrawlpy-0.0.6/scrawlpy.egg-info/entry_points.txt
+-rw-r--r--   0 wu         (501) staff       (20)      214 2024-04-30 08:41:14.000000 scrawlpy-0.0.6/scrawlpy.egg-info/requires.txt
+-rw-r--r--   0 wu         (501) staff       (20)       22 2024-04-30 08:41:14.000000 scrawlpy-0.0.6/scrawlpy.egg-info/top_level.txt
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.246709 scrawlpy-0.0.6/scripts/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:23:17.000000 scrawlpy-0.0.6/scripts/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)       38 2024-04-30 08:41:14.249173 scrawlpy-0.0.6/setup.cfg
+-rw-r--r--   0 wu         (501) staff       (20)     1732 2024-04-30 08:41:12.000000 scrawlpy-0.0.6/setup.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.247082 scrawlpy-0.0.6/test/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.6/test/__init__.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.247658 scrawlpy-0.0.6/test/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.6/test/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      326 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/test/spiders/spider.py
```

### Comparing `scrawlpy-0.0.5/PKG-INFO` & `scrawlpy-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: scrawlpy
-Version: 0.0.5
+Version: 0.0.6
 Summary: scrawlpy是一款python爬虫框架
 Author: Jayden
 Author-email: jayden@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests>=2.22.0
 Provides-Extra: all
 Requires-Dist: bitarray>=1.5.3; extra == "all"
 Requires-Dist: PyExecJS>=1.5.1; extra == "all"
 Requires-Dist: pymongo>=3.10.1; extra == "all"
 Requires-Dist: redis-py-cluster>=2.1.0; extra == "all"
 Requires-Dist: webdriver-manager>=4.0.0; extra == "all"
```

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/cmdline.py` & `scrawlpy-0.0.6/scrawlpy/commands/cmdline.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/create/__init__.py` & `scrawlpy-0.0.6/scrawlpy/commands/create/__init__.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/create/create_cookies.py` & `scrawlpy-0.0.6/scrawlpy/commands/create/create_cookies.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/create/create_init.py` & `scrawlpy-0.0.6/scrawlpy/commands/create/create_init.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/create/create_item.py` & `scrawlpy-0.0.6/scrawlpy/commands/create/create_item.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/create/create_json.py` & `scrawlpy-0.0.6/scrawlpy/commands/create/create_json.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/create/create_params.py` & `scrawlpy-0.0.6/scrawlpy/commands/create/create_params.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/create/create_project.py` & `scrawlpy-0.0.6/scrawlpy/commands/create/create_project.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/create/create_setting.py` & `scrawlpy-0.0.6/scrawlpy/commands/create/create_setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/create/create_spider.py` & `scrawlpy-0.0.6/scrawlpy/commands/create/create_spider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/create/create_table.py` & `scrawlpy-0.0.6/scrawlpy/commands/create/create_table.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/create_builder.py` & `scrawlpy-0.0.6/scrawlpy/commands/create_builder.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/retry.py` & `scrawlpy-0.0.6/scrawlpy/commands/retry.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/shell.py` & `scrawlpy-0.0.6/scrawlpy/commands/shell.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/commands/zip.py` & `scrawlpy-0.0.6/scrawlpy/commands/zip.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/core/base_spider.py` & `scrawlpy-0.0.6/scrawlpy/core/base_spider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/http/request.py` & `scrawlpy-0.0.6/scrawlpy/http/request.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy/setting.py` & `scrawlpy-0.0.6/scrawlpy/setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.5/scrawlpy.egg-info/PKG-INFO` & `scrawlpy-0.0.6/scrawlpy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: scrawlpy
-Version: 0.0.5
+Version: 0.0.6
 Summary: scrawlpy是一款python爬虫框架
 Author: Jayden
 Author-email: jayden@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests>=2.22.0
 Provides-Extra: all
 Requires-Dist: bitarray>=1.5.3; extra == "all"
 Requires-Dist: PyExecJS>=1.5.1; extra == "all"
 Requires-Dist: pymongo>=3.10.1; extra == "all"
 Requires-Dist: redis-py-cluster>=2.1.0; extra == "all"
 Requires-Dist: webdriver-manager>=4.0.0; extra == "all"
```

### Comparing `scrawlpy-0.0.5/setup.py` & `scrawlpy-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     "PyExecJS>=1.5.1",
     "pymongo>=3.10.1",
     "redis-py-cluster>=2.1.0",
 ] + render_requires
 
 setuptools.setup(
     name="scrawlpy",
-    version="0.0.5",
+    version=version,
     author="Jayden",
     license="MIT",
     author_email="jayden@qq.com",
     python_requires=">=3.6",
     description="scrawlpy是一款python爬虫框架",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

