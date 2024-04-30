# Comparing `tmp/JustDeepIt-0.1.30.tar.gz` & `tmp/justdeepit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JustDeepIt-0.1.30.tar", last modified: Thu Jun  1 07:11:18 2023, max compression
+gzip compressed data, was "justdeepit-0.2.0.tar", last modified: Tue Apr 30 05:49:13 2024, max compression
```

## Comparing `JustDeepIt-0.1.30.tar` & `justdeepit-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.809717 JustDeepIt-0.1.30/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.793717 JustDeepIt-0.1.30/JustDeepIt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:11:18.000000 JustDeepIt-0.1.30/JustDeepIt.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-01 07:11:18.809717 JustDeepIt-0.1.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.793717 JustDeepIt-0.1.30/justdeepit/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.797717 JustDeepIt-0.1.30/justdeepit/models/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13913 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/instance_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/object_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    12243 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/salient_object_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.797717 JustDeepIt-0.1.30/justdeepit/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/utils/detectron2base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/utils/mmdetbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    36052 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/utils/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/models/utils/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.789717 JustDeepIt-0.1.30/justdeepit/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.801717 JustDeepIt-0.1.30/justdeepit/src/font/
--rw-r--r--   0 runner    (1001) docker     (123)   555264 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/src/font/NotoSans-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/src/font/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)    59870 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.805717 JustDeepIt-0.1.30/justdeepit/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29097 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/appbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/appis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/appod.py
--rw-r--r--   0 runner    (1001) docker     (123)    22154 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/appsod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.809717 JustDeepIt-0.1.30/justdeepit/webapp/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/.Rhistory
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/jquery-3.6.0.min.map
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)    58702 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/tree.jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)   174878 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/tree.jquery.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    23347 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/static/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:11:18.809717 JustDeepIt-0.1.30/justdeepit/webapp/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/templates/module.html
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/justdeepit/webapp/templates/shutdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:11:18.809717 JustDeepIt-0.1.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-01 07:09:00.000000 JustDeepIt-0.1.30/setup.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.659912 justdeepit-0.2.0/
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.659415 justdeepit-0.2.0/JustDeepIt.egg-info/
+-rw-r--r--   0 sonk414    (501) staff       (20)     2515 2024-04-30 05:49:13.000000 justdeepit-0.2.0/JustDeepIt.egg-info/PKG-INFO
+-rw-r-----   0 sonk414    (501) staff       (20)     1554 2024-04-30 05:49:13.000000 justdeepit-0.2.0/JustDeepIt.egg-info/SOURCES.txt
+-rw-r-----   0 sonk414    (501) staff       (20)        1 2024-04-30 05:49:13.000000 justdeepit-0.2.0/JustDeepIt.egg-info/dependency_links.txt
+-rw-r-----   0 sonk414    (501) staff       (20)       58 2024-04-30 05:49:13.000000 justdeepit-0.2.0/JustDeepIt.egg-info/entry_points.txt
+-rw-r-----   0 sonk414    (501) staff       (20)      145 2024-04-30 05:49:13.000000 justdeepit-0.2.0/JustDeepIt.egg-info/requires.txt
+-rw-r-----   0 sonk414    (501) staff       (20)       11 2024-04-30 05:49:13.000000 justdeepit-0.2.0/JustDeepIt.egg-info/top_level.txt
+-rw-r-----   0 sonk414    (501) staff       (20)        1 2024-04-30 05:17:09.000000 justdeepit-0.2.0/JustDeepIt.egg-info/zip-safe
+-rw-r--r--   0 sonk414    (501) staff       (20)     1070 2024-04-30 05:17:10.000000 justdeepit-0.2.0/LICENSE
+-rw-r--r--   0 sonk414    (501) staff       (20)      128 2024-04-30 05:17:10.000000 justdeepit-0.2.0/MANIFEST.in
+-rw-r--r--   0 sonk414    (501) staff       (20)     2515 2024-04-30 05:49:13.659702 justdeepit-0.2.0/PKG-INFO
+-rw-r--r--   0 sonk414    (501) staff       (20)     1426 2024-04-30 05:17:10.000000 justdeepit-0.2.0/README.md
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.651816 justdeepit-0.2.0/justdeepit/
+-rw-r--r--   0 sonk414    (501) staff       (20)       95 2024-04-30 05:17:27.000000 justdeepit-0.2.0/justdeepit/__init__.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.652839 justdeepit-0.2.0/justdeepit/app/
+-rw-r--r--   0 sonk414    (501) staff       (20)      162 2024-04-30 05:17:29.000000 justdeepit-0.2.0/justdeepit/app/__init__.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    25983 2024-04-30 05:17:29.000000 justdeepit-0.2.0/justdeepit/app/app.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     5692 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/app/appbase.py
+-rw-r--r--   0 sonk414    (501) staff       (20)      554 2024-04-30 05:17:29.000000 justdeepit-0.2.0/justdeepit/app/appis.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    10048 2024-04-30 05:17:29.000000 justdeepit-0.2.0/justdeepit/app/appod.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    22300 2024-04-30 05:17:29.000000 justdeepit-0.2.0/justdeepit/app/appsod.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.653648 justdeepit-0.2.0/justdeepit/models/
+-rw-r--r--   0 sonk414    (501) staff       (20)      184 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/__init__.py
+-rw-r--r--   0 sonk414    (501) staff       (20)      309 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/abstract.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    12931 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/instance_segment.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    13500 2024-04-30 05:17:27.000000 justdeepit-0.2.0/justdeepit/models/object_detect.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    12227 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/salient_object_detect.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.654558 justdeepit-0.2.0/justdeepit/models/utils/
+-rw-r--r--   0 sonk414    (501) staff       (20)        0 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/utils/__init__.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     6720 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/utils/data.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    11507 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/utils/mmdetbase.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    36052 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/utils/u2net.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    10173 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/utils/unet.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.649685 justdeepit-0.2.0/justdeepit/src/
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.655154 justdeepit-0.2.0/justdeepit/src/font/
+-rw-r--r--   0 sonk414    (501) staff       (20)   555264 2024-04-30 05:17:30.000000 justdeepit-0.2.0/justdeepit/src/font/NotoSans-Medium.ttf
+-rw-r--r--   0 sonk414    (501) staff       (20)     4449 2024-04-30 05:17:30.000000 justdeepit-0.2.0/justdeepit/src/font/OFL.txt
+-rw-r--r--   0 sonk414    (501) staff       (20)    56860 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/utils.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.656295 justdeepit-0.2.0/justdeepit/webapp/
+-rw-r--r--   0 sonk414    (501) staff       (20)      174 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/__init__.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    28329 2024-03-08 01:38:16.000000 justdeepit-0.2.0/justdeepit/webapp/app.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     6844 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/appbase.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     1314 2023-12-26 03:14:25.000000 justdeepit-0.2.0/justdeepit/webapp/appis.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     8356 2023-12-26 03:13:54.000000 justdeepit-0.2.0/justdeepit/webapp/appod.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    22154 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/appsod.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.657363 justdeepit-0.2.0/justdeepit/webapp/static/
+-rw-r--r--   0 sonk414    (501) staff       (20)    89501 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/static/jquery-3.6.0.min.js
+-rw-r--r--   0 sonk414    (501) staff       (20)   137972 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/static/jquery-3.6.0.min.map
+-rw-r--r--   0 sonk414    (501) staff       (20)    14309 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/static/styles.css
+-rw-r--r--   0 sonk414    (501) staff       (20)    58702 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/static/tree.jquery.js
+-rw-r--r--   0 sonk414    (501) staff       (20)   174878 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/static/tree.jquery.js.map
+-rw-r--r--   0 sonk414    (501) staff       (20)    23347 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/static/utils.js
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.657803 justdeepit-0.2.0/justdeepit/webapp/templates/
+-rw-r--r--   0 sonk414    (501) staff       (20)     1198 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/templates/index.html
+-rw-r--r--   0 sonk414    (501) staff       (20)    15402 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/templates/module.html
+-rw-r--r--   0 sonk414    (501) staff       (20)      571 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/templates/shutdown.html
+-rw-r--r--   0 sonk414    (501) staff       (20)      151 2024-04-30 05:17:30.000000 justdeepit-0.2.0/requirements.txt
+-rw-r--r--   0 sonk414    (501) staff       (20)       38 2024-04-30 05:49:13.659956 justdeepit-0.2.0/setup.cfg
+-rw-r--r--   0 sonk414    (501) staff       (20)     1582 2024-04-30 05:47:27.000000 justdeepit-0.2.0/setup.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.658814 justdeepit-0.2.0/tests/
+-rw-r--r--   0 sonk414    (501) staff       (20)     3656 2024-04-30 05:22:19.000000 justdeepit-0.2.0/tests/test_det.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     7845 2023-12-19 06:32:04.000000 justdeepit-0.2.0/tests/test_odmodels.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     4943 2023-12-19 06:32:04.000000 justdeepit-0.2.0/tests/test_osmodels.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     2304 2024-04-30 05:22:19.000000 justdeepit-0.2.0/tests/test_segm.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     3139 2024-04-30 05:22:19.000000 justdeepit-0.2.0/tests/test_sodmodels.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     6933 2024-04-30 05:22:19.000000 justdeepit-0.2.0/tests/test_utils.py
```

### Comparing `JustDeepIt-0.1.30/JustDeepIt.egg-info/PKG-INFO` & `justdeepit-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,32 @@
-Metadata-Version: 2.1
-Name: JustDeepIt
-Version: 0.1.30
-Summary: a GUI tool for object detection and segmentation based on deep learning
-Home-page: https://github.com/biunit/JustDeepIt
-Author: Jianqiang Sun
-Author-email: sun@biunit.dev
-License: MIT
-Keywords: object detection,object segmentation
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: X11 Applications
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-License-File: LICENSE
+# JustDeepIt 
+
+Image analysis based on deep learning is becoming mainstream and increasingly accessible
+for solving various scientific problems in diverse fields including plant science.
+Practical applications in plant science include species classification,
+fruit detection, plant disease and pest detection, weed detection,
+leaf segmentation, and plant segmentation.
+Python programming language and its libraries including PyTorch and MMDetection
+have made deep learning much easier and more accessible to researchers.
+However, deep learning technologies remain challenging for programming beginners
+because they require computer programming skills and a basic familiarity
+with character user interfaces (CUIs).
+JustDeepIt aims to simplify object detection, instance segmentation, and salient object detection
+using deep learning by providing a graphical user interface (GUI).
+In addition, to ensure flexibility and extensibility, JustDeepIt also provides CUI.
+It may be applicable for image analysis in various disciplines beyond plant science.
+
+
+## Documentation
+
+- https://justdeepit.readthedocs.io/en/latest/index.html
+
+
+## Citation
+
+Sun J, Cao W, Yamanaka T.
+JustDeepIt: Software tool with graphical and character user interfaces
+for deep learning-based object detection and segmentation in image analysis.
+Front. Plant Sci., 2022, 13:964058.
+doi: [10.3389/fpls.2022.964058](https://doi.org/10.3389/fpls.2022.964058)
+
 
-Deep learning has been applied to solve various problems, especially in image recognition, across many fields including the life sciences and agriculture. Many studies have reported the use of deep learning to identify plant and insect species, detect flowers and fruits, segment plant individuals from fixed-point observation cameras or drone images, and other applications. Programming languages such as Python and its libraries including PyTorch, MMDetection, and Detectron2 have made deep learning easier and more accessible to researchers. However, it remains difficult for many researchers without advanced programming skills to use deep learning and environments such as the character user interface (CUI) through keyboard input. JustDeepIt aims to support researchers by facilitating the use of deep learning for object detection and segmentation by providing both graphical user interface (GUI) and CUI operations. JustDeepIt can be used for plant detection, pest detection, and a variety of tasks in life sciences, agriculture, and other fields.
```

### Comparing `JustDeepIt-0.1.30/JustDeepIt.egg-info/SOURCES.txt` & `justdeepit-0.2.0/JustDeepIt.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -8,35 +8,46 @@
 JustDeepIt.egg-info/dependency_links.txt
 JustDeepIt.egg-info/entry_points.txt
 JustDeepIt.egg-info/requires.txt
 JustDeepIt.egg-info/top_level.txt
 JustDeepIt.egg-info/zip-safe
 justdeepit/__init__.py
 justdeepit/utils.py
+justdeepit/app/__init__.py
+justdeepit/app/app.py
+justdeepit/app/appbase.py
+justdeepit/app/appis.py
+justdeepit/app/appod.py
+justdeepit/app/appsod.py
 justdeepit/models/__init__.py
 justdeepit/models/abstract.py
 justdeepit/models/instance_segment.py
 justdeepit/models/object_detect.py
 justdeepit/models/salient_object_detect.py
 justdeepit/models/utils/__init__.py
-justdeepit/models/utils/detectron2base.py
+justdeepit/models/utils/data.py
 justdeepit/models/utils/mmdetbase.py
 justdeepit/models/utils/u2net.py
 justdeepit/models/utils/unet.py
 justdeepit/src/font/NotoSans-Medium.ttf
 justdeepit/src/font/OFL.txt
 justdeepit/webapp/__init__.py
 justdeepit/webapp/app.py
 justdeepit/webapp/appbase.py
 justdeepit/webapp/appis.py
 justdeepit/webapp/appod.py
 justdeepit/webapp/appsod.py
-justdeepit/webapp/static/.Rhistory
 justdeepit/webapp/static/jquery-3.6.0.min.js
 justdeepit/webapp/static/jquery-3.6.0.min.map
 justdeepit/webapp/static/styles.css
 justdeepit/webapp/static/tree.jquery.js
 justdeepit/webapp/static/tree.jquery.js.map
 justdeepit/webapp/static/utils.js
 justdeepit/webapp/templates/index.html
 justdeepit/webapp/templates/module.html
-justdeepit/webapp/templates/shutdown.html
+justdeepit/webapp/templates/shutdown.html
+tests/test_det.py
+tests/test_odmodels.py
+tests/test_osmodels.py
+tests/test_segm.py
+tests/test_sodmodels.py
+tests/test_utils.py
```

### Comparing `JustDeepIt-0.1.30/LICENSE` & `justdeepit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/models/instance_segment.py` & `justdeepit-0.2.0/justdeepit/models/salient_object_detect.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,321 +1,290 @@
 import os
 import glob
-import pkg_resources
+from justdeepit.models.utils.u2net import U2Net
 from justdeepit.utils import ImageAnnotation, ImageAnnotations
 
-class IS:
-    """A class to generate model for instance segmentation
-
-    The :class:`IS <justdeepit.models.IS>` class is used for generating
-    deep neural network (DNN) architectures (i.e., models) for instance segmentation
-    by internally calling the MMDetection or Detectron2 library.
-
-    User can specify DNN architectures using the ``model_arch`` or ``model_config``
-    argument. If the ``model_arch`` is specified and ``model_config`` is ``None``,
-    the :class:`IS <justdeepit.models.IS>` class generates a DNN architecture
-    according the ``model_arch`` using the pre-defined configuration.
-    The pre-defined DNN architectures for instance segmentation can be checked with the
-    :func:`available_architectures <justdeepit.models.IS.available_architectures>` method.
-    Alternatively, if the ``model_config`` argument is specified,
-    the :class:`IS <justdeepit.models.IS>` class generates a DNN architecture
-    following the configuration specified with the ``model_config``,
-    regardless of whether the ``model_arch`` is specified.
-
-    The backend for generating DNN architectures can be specified to the MMDetection
-    or Detectron2. Currently, the MMDetection supports more architectures than Detectron2
-    and model training under GPU environments. Detectron2 can train architectures
-    fast and supports CPU and GPU environments.
+class SOD():
+    """Base module to generate salient object detection model
+    
+    The :class:`SOD <justdeepit.models.SOD>` class is used for generating
+    U\ :sup:`2`-Net for salient object detection.
+ 
 
     Args:
-        class_label (str): A path to a file which contains class labels.
-                       The file should be multiple rows with one column,
-                       and string in each row represents a class label.
         model_arch (str): A string to specify model architecture.
-                       If ``model_config`` is given, this option will be ignored.
-        model_config (str): A path to configure file for building models.
-                        If the configure file is not given or does not exist at the specified
-                        path, then load the default configure file according ``model_arch``.
+                          The current version of JustDeepIt only supports U\ :sup:`2`-Net architecture.
         model_weight (str): A path to a model weights. If ``None``, then use the initial
-                        value that randomly generated by the packages.
+                            value that randomly generated by the packages.
         workspace (str): A path to workspace directory. Log information and checkpoints of model
                      training will be stored in this directory.
                      If ``None``, then create temporary directory in the current directory.
-        backend (str): Specify the backend to build instance segmentation mode.
-                   ``detectron2`` or ``mmdetection`` can be speficied.
-    
+ 
     Examples:
-        >>> from justdeepit.models import IS
-        >>> 
-        >>> # initialize Mask RCNN with random weights using MMDetection backend
-        >>> model = IS('./class_label.txt', model_arch='maskrcnn', backend='mmdetection')
-        >>> 
-        >>> # initialize Mask RCNN with randomm weights using Detectron2 backend
-        >>> model = IS('./class_label.txt', model_arch='maskrcnn', backend='detectron2')
-        >>> 
-        >>> # initialize Mask RCNN with trained weights using MMDetection backend
-        >>> model = IS('./class_label.txt', model_arch='maskrcnn', mdoel_weight='trained_weight.pth',
-        >>>            backend='mmdetection')
-        >>> 
-        >>> # initialize Mask RCNN with trained weights using Detectron2 backend
-        >>> model = IS('./class_label.txt', model_arch='maskrcnn', model_weight='trained_weight.pth',
-        >>>            backend='detectron2')
-        >>> 
-    """  
-    
-    
-    def __init__(self, class_label=None, model_arch=None, model_config=None, model_weight=None, workspace=None, backend='mmdetection'):
-        
-        self.module = None
-        self.__architectures = self.__available_architectures()
-        self.__supported_formats = ('COCO', 'VoTT') #, 'RGB mask')
-        self.__image_ext = ['.jpg', '.jpeg', '.png', '.tif', '.tiff']
-        
-        self.backend = backend
-        self.model_arch = model_arch
+            >>> from justdeepit.models import SOD
+            >>> 
+            >>> # initialize U2-Net with random weight
+            >>> model = SOD()
+            >>> 
+            >>> # initialize U2-Net with trained weight (./leaf.u2net.pth)
+            >>> model = SOD(model_weight='./leaf.u2net.pth')
+    
+    """
+    
+    
+    def __init__(self, model_arch='u2net', model_weight=None, workspace=None):
         if workspace is None:
             workspace = os.path.abspath(os.getcwd())
         self.workspace = workspace
-        self.module = self.__init_module(class_label, model_arch, model_config, model_weight, workspace, backend)
-    
-    
-    def __available_architectures(self):
-        return {
-            'mmdetection': [
-                ['Mask R-CNN', 'mask_rcnn_x101_64x4d_fpn_mstrain-poly_3x_coco'],
-                ['Cascade Mask R-CNN', 'cascade_mask_rcnn_x101_64x4d_fpn_mstrain_3x_coco.py'],
-                ['custom',    None]
-            ],
-            'detectron2': [
-                ['Mask R-CNN', 'COCO-InstanceSegmentation/mask_rcnn_R_101_FPN_3x.yaml'],
-                ['custom',    None]
-            ]
-        }
-
+        
+        self.__architectures = ('U2Net',)
+        self.__supported_formats = ('mask', 'COCO')
+        self.__image_ext = ['.jpg', '.jpeg', '.png', '.tif', '.tiff']
+        self.module = self.__init_module(model_arch, model_weight, workspace)
     
     
-    def __init_module(self, class_label, model_arch, model_config, model_weight, workspace, backend):
+    def __init_module(self, model_arch, model_weight, workspace):
         if model_arch is None:
             return None
-        
-        backend_ = self.__norm_backend(backend)
-        
-        if model_config is None:
-            # check model arch
-            model_arch_ = self.__norm_arch(model_arch)
-            if model_arch_ not in [self.__norm_arch(_[0]) for _ in self.__architectures[backend_]]:
-                NotImplementedError('JustDeepIt does not support {} archtecture when {} is specified as a backend.'.format(model_arch, backend))
-
-            # set model_config according to model_arch
-            for available_arch, available_config in self.__architectures[backend_]:
-                if model_arch_ == self.__norm_arch(available_arch):
-                    if model_arch_ == 'custom':
-                        if model_config is None or  model_config == '':
-                            ValueError('The argument `model_config` cannot be none or empty when the user customized architecture is set.')
-                    else:
-                        model_config = available_config
-                    break
-
-        # init module
-        module = None
-        if backend_ == 'mmdetection':
-            from justdeepit.models.utils.mmdetbase import MMDetBase
-            module = MMDetBase(class_label, model_arch, model_config, model_weight, workspace)
-        elif backend_ == 'detectron2':
-            from justdeepit.models.utils.detectron2base import DetectronBase
-            module = DetectronBase(class_label, model_arch, model_config, model_weight, workspace)
-
-        return module
-
-
-
-    def __norm_arch(self, arch):
-        return arch.replace('-', '').replace(' ', '').lower()
-
-
-    def __norm_backend(self, backend):
-        backend_ = backend.lower()
-        if backend in ['mm', 'mmdet', 'mmdetection']:
-            backend_ = 'mmdetection'
-        elif backend_ in ['d2', 'detectron', 'detectron2']:
-            backend_ = 'detectron2'
+            
+        model_arch = model_arch.replace('-', '').replace(' ', '').lower()
+        if model_arch == 'u2net':
+            module = U2Net(model_weight, workspace)
         else:
-            NotImplementedError('JustDeepIt does not support `{}` as a backend.'.format(backend))
-        return backend_
-
+            NotImplementedError('JustDeepIt does not support {}.')
 
+        return module
+        
 
-    def available_architectures(self, backend):
-        """Display the pre-trained architectures for instance segmentation
 
-        This method is used to display the DNN architectures pre-trained
-        in JustDeepIt for instance segmentation.
-        As the different backend supports the
-        different architectures, this method requires user to specify
-        the backend.
+    def available_architectures(self):
+        """Show the available architectures
 
-        Args:
-            backend (str): Specify the backend.
-                           ``detectron2`` or ``mmdetection`` can be speficied.
+        Show the available architectures for salient object detection.
 
         Returns:
             A tuple of the supported architecture.
 
         Examples:
-            >>> from justdeepit.models import IS
+            >>> from justdeepit.models import SOD
             >>>
-            >>> model = IS()
-            >>> model.available_architectures('mmdetection')
+            >>> model = SOD()
+            >>> model.available_architectures()
 
         """
-        return tuple([_[0] for _ in self.__architectures[self.__norm_backend(backend)]])
+        return self.__architectures
 
 
-    
 
     def supported_formats(self):
-        """Display the supported annotation formats for training
-        
-        Display the supported annotation formats for traning instance segmentation architecture.
+        """Show the supported annotation formats
+
+        Show the supported annotation formats for salient object detection.
 
         Returns:
             A tuple of the supported annotation formats.
 
         Examples:
-            >>> from justdeepit.models import IS
+            >>> from justdeepit.models import SOD
             >>>
-            >>> model = IS()
+            >>> model = SOD()
             >>> model.supported_formats()
 
         """
         return self.__supported_formats
 
-
-
+    
     def __norm_format(self, x):
         x = x.replace(' ', '').replace('-', '').lower()
         if ('pascal' in x) or ('xml' in x):
             x = 'voc'
-        if ('rgb' in x) and ('mask' in x):
-            x = 'rgbmask'
         return x
     
-
     
-    def train(self, image_dpath, annotation, annotation_format='COCO',
+
+    def train(self, image_dpath, annotation, annotation_format='mask',
               optimizer=None, scheduler=None,
-              batchsize=8, epoch=100, score_cutoff=0.5, cpu=4, gpu=1):
+              batchsize=8, epoch=100, cpu=4, gpu=1,
+              strategy='resizing', window_size=320):
         """Train model
- 
-        The :func:`train <justdeepit.models.IS.train>` is used for training a model.
-        The training images (``image_dpath``), annotation files (``annotation``),
-        and annotation format (``annotation_format``) must be specified.
-        Note that, the current version of JustDeepIt only supports COCO format.
+        
+        Method :func:`train <justdeepit.models.SOD.train>` is used for
+        training a model using *resizing* or *random cropping* approach.
+        The *resizing* approach scales the original image to 288 x 288 pixels for training,
+        whereas *random cropping* randomly crops small square areas from the original image,
+        and resizes the areas to 288 x 288 pixels for training.
+        The size of the square areas can be specified by the user
+        according to the characteristics of the target task.
+        The default size of the cropped square area is 320 x 320 pixels.
         
         Args:
             image_dpath (str): A path to directory which contains all training images.
-            annotation (str): A file path to COCO format annotation file.
-            annotation_format (str): Annotation format. COCO or VoTT are supported in the current version.
-            optimizer (str): String to specify optimizer/solver supported by MMDetection or Detectron2.
-            scheduler (str): String to specify optimization scheduler.
-            batchsize (int): Batch size for each GPU.
-            epoch (int): Epoch.
-            score_cutoff (float): Cutoff of score for instance segmentation.
-            cpu (int): Number of workers for pre-prociessing images for each GPU.
-            gpu (int): Number of GPUs for model training.
-        
+            annotation (str): A path to a file (when the format is COCO) or folder (when the format is mask).
+            annotation_format (str): Annotation format.
+            optimizer (str): String to specify PyTorch optimizer. The optimizers supported by
+                    PyTorch can be checked from
+                    the `PyTorch website <https://pytorch.org/docs/stable/optim.html>`_.
+            scheduler (str): String to specify PyTorch optimization scheduler. The schedulers supported by
+                    PyTorch can be checked from
+                    the `PyTorch website <https://pytorch.org/docs/stable/optim.html>`_.
+            batchsize (int): Number of batch size.
+                             Note that a large number of batch size may cause out of memory error.
+            epoch (int): Number of epochs.
+            cpu (int): Number of CPUs are used for prerpocessing training images.
+            gpu (int): Number of GPUs are uesd for traininng model.
+            strategy (str): Strategy for model trainig. One of ``resizing`` or ``randomcrop`` can be specified.
+            window_size (int): The width of images should be randomly cropped from the original images
+                                    when ``randomcrop`` srategy was selected.
+
+
         Examples:
-            >>> from justdeepit.models import IS 
+            >>> from justdeepit.models import SOD
+            >>> 
+            >>> model = SOD()
+            >>> 
+            >>> model.train('./train_images', './mask_images', 'mask')
+            >>> 
+            >>> 
+            >>> # set optimizer and scheduler
+            >>> model.train('./train_images', '.mask_images', 'mask',
+            >>>             optimizer='Adam(params, lr=0.001, betas=(0.9, 0.999), eps=1e-08)',
+            >>>             scheduler='ExponentialLR(optimizer, gamma=0.9)')
             >>> 
-            >>> model = IS('./class_label.txt', model_arch='maskrcnn')
-            >>> model.train('./train_images', './annotations.coco.json', 'COCO')
         """
+        
+        images = []
+        masks = []
         annotation_format = self.__norm_format(annotation_format)
-        if annotation_format == 'coco':
-            pass
-        elif annotation_format == 'vott':
-            anns = ImageAnnotations()
-            for fpath in glob.glob(os.path.join(image_dpath, '*')):
-                fname, fext = os.path.splitext(os.path.basename(fpath))
-                if fext.lower() in self.__image_ext:
-                    anns.append(ImageAnnotation(fpath, annotation))
-            if len(anns) > 0:
-                annotation = os.path.join(self.workspace, 'train_image_annotation.coco.json')
-                anns.format('coco', annotation)
+        if annotation_format == 'mask':
+            fdict = {}
+            for f in glob.glob(os.path.join(image_dpath, '*')):
+                fname = os.path.splitext(os.path.basename(f))[0]
+                if os.path.splitext(f)[1].lower() in self.__image_ext:
+                    if fname not in fdict:
+                        fdict[fname] = {'image': None, 'mask': None}
+                    fdict[fname]['image'] = f
+            for f in glob.glob(os.path.join(annotation, '*')):
+                fname = os.path.splitext(os.path.basename(f))[0]
+                if fname not in fdict:
+                    fdict[fname] = {'image': None, 'mask': None}
+                fdict[fname]['mask'] = f
+            for fname, fpath in fdict.items():
+                if fpath['image'] is not None and fpath['mask'] is not None:
+                    images.append(fpath['image'])
+                    masks.append(fpath['mask'])
+           
+        elif annotation_format == 'coco':
+            # generate mask for mdoel training form coco annotation
+            mask_dpath = os.path.join(self.workspace, 'mask')
+            if not os.path.exists(mask_dpath):
+                os.mkdir(mask_dpath)
+            
+            for f in sorted(glob.glob(os.path.join(image_dpath, '*'))):
+                image_fname, image_fext = os.path.splitext(f)
+                if image_fext.lower() in self.__image_ext:
+                    ann = ImageAnnotation(f, annotation, annotation_format)
+                    m = os.path.join(mask_dpath, os.path.splitext(os.path.basename(image_fname))[0] + '.mask.png')
+                    ann.draw('mask', m)
+                    images.append(f)
+                    masks.append(m)
         else:
-            raise NotImplementedError('JustDeepIt does not support {} format for training instance segmentation model.'.format(annotation_format))
+            raise NotImplementedError('JustDeepIt does not support {} format for training salient object detection model.'.format(annotation_format))
+        
+        
+        train_data_fpath = os.path.join(self.workspace, 'train_images.txt')
+        with open(train_data_fpath, 'w') as outfh:
+            for image, mask in zip(images, masks):
+                outfh.write('{}\t{}\n'.format(image, mask))
         
-        self.module.train(image_dpath, annotation,
+        return self.module.train(train_data_fpath,
                           optimizer, scheduler,
-                          batchsize=batchsize, epoch=epoch, score_cutoff=score_cutoff,
-                          cpu=cpu, gpu=gpu)
-    
-    
+                          batchsize, epoch,
+                          cpu, gpu,
+                          strategy, window_size)
+
+
+   
     
-    def save(self, weight_fpath, config_fpath=None):
-        '''Save the trained model
-        
-        Method :func:`save <justdeepit.models.IS.save>`
-        stores the trained model weights and model configuration.
+    def save(self, weight_fpath):
+        """Save weights
         
+        Method to store the current weights.
+
         Args:
-            weight_fpath (str): A path to save the weights.
-            config_fpath (str): A path to save the model configure. If ``None``,
-                                then save the configure to file with same name
-                                of ``weight_fpath`` but different extension.
-        
+            weight_fpath (str): A path to store model weights.
+
         Examples:
-            >>> from justdeepit.models import IS
+            >>> from justdeepit.models import SOD
             >>> 
-            >>> model = IS('./class_label.txt', model_arch='maskrcnn')
-            >>> model.train('./train_images', './annotations.coco.json')
-            >>> odnet.save('./trained_weight.pth')
-        ''' 
-        self.module.save(weight_fpath, config_fpath)
-    
+            >>> model = SOD()
+            >>> model.train('./train_images', './mask_images', 'mask')
+            >>> model.save('trained_weight.pth')
+            >>> 
+
+        """
+        
+        return self.module.save(weight_fpath)
+
+
+
+
+
     
     
-    def inference(self, images, score_cutoff=0.5, batchsize=8, cpu=4, gpu=1):
-        '''Detect objects from images
+    def inference(self, image_path, strategy='resizing', batchsize=8, cpu=4, gpu=1,
+                  window_size=320,
+                  score_cutoff=0.5, image_opening_kernel=0, image_closing_kernel=0):
+        """Object Segmentation
         
-        Method :func:`inference <justdeepit.models.IS.inference>` is used to
-        detect objects from an image or images with a given model (weights).
+        Method :func:`inference <justdeepit.models.SOD.inference>` performs
+        salient object detection through *resizing* or *sliding* approach.
+        The *resizing* approach resizes the original image to 288 x 288 pixels for model training.
+        On the other hand, *sliding* crops adjacent square areas from the original image
+        for input to the model,
+        and the outputs are merged into a single image.
+        The size of the square areas can be specified by the user,
+        but it is recommended to use the value specified by ``window_size`` for training.
         
         Args:
-            images (str): A path to a image file or a path to a directory which contains
-                          multiple images.
-            score_cutoff (float): Cutoff for instance segmentation.
-            batchsize (int): Number of batches.
-            cpu (int): Number of CPUs.
-            gpu (int): Number of GPUs.
-        
+            image_path (str): A path to a image file, a list of image files,
+                              or a path to a directory which contains multiple images.
+            strategy (str): Strategy for model trainig. One of ``resizing`` or ``slide`` can be specified.
+            output_type (str): Output format. 
+            batchsize (int): Number of batch size. Note that a large number of
+                              batch size may cause out of memory error.
+            epoch (int): Number of epochs.
+            cpu (int): Number of CPUs are used for prerpocessing training images.
+            gpu (int): Number of GPUs are used for object segmentation.
+            window_size (int): The width of images should be cropped from the original images
+                                       when ``slide`` srategy was selected.
+            score_cutoff (float): A threshold to cutoff U2Net outputs. Values higher than this threshold
+                              are considering as detected objects.
+            image_opening_kernel (int): The kernel size for image closing
+                                        to remove the noise that detected as object.
+            image_closing_kernel (int): The kernel size for image opening
+                                        to remove the small bubbles in object.
+
         Returns:
-            :class:`ImageAnnotation <justdeepit.utils.ImageAnnotation>` class object
-            or a list of :class:`ImageAnnotation <justdeepit.utils.ImageAnnotation>` class object.
+            array: mask image or mask annotations.
         
         Examples:
             >>> import os
-            >>> from justdeepit.models import IS 
+            >>> from justdeepit.models import SOD
             >>> 
-            >>> model = IS('./class_label.txt', model_arch='maskrcnn', model_weight='./trained_weight.pth')
+            >>> model = SOD(model_weight='trained_weight.pth')
             >>> 
-            >>> # inference single image
+            >>> # single image
             >>> output = model.inference('sample.jpg')
-            >>> output.draw('contour', 'output/sample.png')
+            >>> output.draw('mask', 'sample.predicted_mask.png')
             >>> 
-            >>> # inference multiple images
+            >>> # multiple images
             >>> test_images = ['sample1.jpg', 'sample2.jpg', 'sample3.jpg']
-            >>> outputs = model.inference(sample_images)
+            >>> outputs = model.inference(test_images)
             >>> for test_image, output in zip(test_images, outputs):
-            >>>     bbox_img_fpath = os.path.splitext(test_image)[0] + '.bbox.png'
-            >>>     output.draw('bbox+contour', bbox_img_fpath)
-            >>> 
-        '''
+            >>>     mask_fpath = os.path.splitext(test_image) + '_mask.png'
+            >>>     output.draw('mask', mask_fpath)
+            
+        """
         
-        return self.module.inference(images, score_cutoff=score_cutoff, batchsize=batchsize, cpu=cpu, gpu=gpu)
-    
-    
-
-
-
-
-
+        return self.module.inference(image_path, strategy, batchsize, cpu, gpu,
+                              window_size, score_cutoff,
+                              image_opening_kernel, image_closing_kernel)
```

### Comparing `JustDeepIt-0.1.30/justdeepit/models/utils/detectron2base.py` & `justdeepit-0.2.0/justdeepit/models/utils/mmdetbase.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,291 +1,325 @@
 import os
-import sys
+import shutil
 import json
 import glob
+import math
 import tqdm
-import logging
 import tempfile
-import math
+import logging
+import datetime
 import numpy as np
-import torch
-import PIL.Image
 import skimage
 import skimage.measure
-import cv2
-from justdeepit.models.abstract import ModuleTemplate
-from justdeepit.utils import ImageAnnotation, ImageAnnotations
+import PIL
+import torch
+import torch.multiprocessing
+from justdeepit.models.abstract import ModuleTemplate, JDIError
+from justdeepit.utils import ImageAnnotation, ImageAnnotations, load_images
+from justdeepit.models.utils.data import DataClass, DataPipeline, DataLoader
 
 logger = logging.getLogger(__name__)
 
 try:
-    import detectron2
-    import detectron2.config
-    import detectron2.model_zoo
-    import detectron2.structures
-    import detectron2.engine
-    import detectron2.modeling
-    import detectron2.checkpoint
-    import detectron2.data.transforms
+    import mim
+    import mmcv
+    import mmdet
+    import mmcv.ops
+    import mmdet.utils
+    import mmdet.apis
+    import mmdet.models
+    import mmdet.datasets
+    import mmengine.config
+    import mmengine.registry
+    import mmengine.runner
 except ImportError:
-    msg = 'JustDeepIt requires detectron2 library to build models. Make sure detectron2 has been installed already.'
+    msg = ('JustDeepIt requires the installation of '
+           'the following Python packages:\n'
+           '     - mmcv>=2.0.0\n'
+           '     - mmdet>=3.0.0\n'
+           '     - mmengine>=0.7.3\n'
+           'to build detection/segmentation models. '
+           'Please ensure that these packages are '
+           'already installed with the correct versions.\n')
     logger.error(msg)
-    raise ImportError(msg)
+    raise JDIError(msg)
 
 
 
 
-class DetectronBase(ModuleTemplate):
 
-    def __init__(self, class_labels, model_arch=None, model_config=None, model_weight=None, workspace=None):
-        # model
-        self.model_arch = model_arch
-        self.model = None
-        self.detector = None
+class MMDetBase(ModuleTemplate):
+    
+    
+    def __init__(self,
+                 class_labels=None,
+                 model_arch=None,
+                 model_config=None,
+                 model_weight=None,
+                 model_class=None,
+                 workspace=None,
+                 seed=None):
         
-        # config and weight
-        self.cfg = self.__get_config(model_config, model_weight)
+        # model settings
+        self.model_arch = model_arch
+        self.class_labels = DataClass(class_labels)
+        self.model_class = model_class
+        self.cfg_fpath = model_config
+        self.cfg = self.__set_config(model_config, model_weight, self.class_labels.class_labels)
         
         # workspace
+        self.tempd = None
         if workspace is None:
             self.tempd = tempfile.TemporaryDirectory()
             self.workspace = self.tempd.name
         else:
-            self.tempd = None
             self.workspace = workspace
-        self.cfg.OUTPUT_DIR = os.path.abspath(self.workspace)
-        logger.info('Workspace for Detectron2-based model is set at `{}`.'.format(self.workspace))
-        
-        
-        # class labels
-        self.class_labels = self.__parse_class_labels(class_labels)
-        self.cfg.MODEL.ROI_HEADS.NUM_CLASSES = len(self.class_labels)
-        self.cfg.MODEL.RETINANET.NUM_CLASSES = len(self.class_labels)
-        
-        # default params
-        self.cfg.MODEL.DEVICE = 'cpu'
+        self.cfg.work_dir = os.path.abspath(self.workspace)
+        logger.info(f'The workspace is set to `{self.workspace}`. '
+                    f'Please locate the intermediate and final results '
+                    f'within this workspace.')
+        
+        # random seed
+        if seed is None:
+            seed = int(datetime.datetime.utcnow().timestamp())
+        self.cfg.seed = seed
     
     
+
     def __del__(self):
         try:
             if self.tempd is not None:
                 self.tempd.cleanup()
         except:
-            pass
+            logger.info(f'The temporary directory (`{self.workspace}`) created by JustDeepIt '
+                        f'cannot be removed automatically. Please remove it manually.')
     
     
-    def __get_config(self, model_config, model_weight):
-        if model_config is None or model_config == '':
-            raise ValueError('Configuration file for Detectron2 cannot be empty.')
-        
+
+    def __set_config(self, model_config, model_weight, class_labels):
         cfg = None
+        if model_config is None or model_config == '':
+            raise JDIError(f'JustDeepIt requires a configuration file to build models. '
+                           f'Set up a path to a configuration file or '
+                           f'run `mim search mmcls --valid-config` to set the pre-defined configuration.')
         try:
-            model_config_fpath = model_config
-            if not os.path.exists(model_config_fpath):
-                # if the given path does not exist, set the chkpoint from github as a initial params
-                model_config_fpath = detectron2.model_zoo.get_config_file(model_config_fpath)
-            cfg = detectron2.config.get_cfg()
-            cfg.merge_from_file(model_config_fpath)
-        
+            # if config does not exist, download the config from MMLab.
+            if not os.path.exists(model_config):
+                cache_dpath = os.path.join(os.path.expanduser('~'), '.cache', 'mim')
+                if os.path.splitext(model_config)[1] in ['.py', '.yaml']:
+                    model_config = os.path.splitext(model_config)[0]
+                model_chkpoint = mim.commands.download(package='mmdet',
+                                                       configs=[model_config])[0]
+                model_config = os.path.join(cache_dpath, model_config + '.py')
+                model_chkpoint =  os.path.join(cache_dpath, model_chkpoint)
+            cfg = mmengine.config.Config.fromfile(model_config)
+            
+            # if weights not given, download the weights from MMLab
             if (model_weight is None) or (not os.path.exists(model_weight)):
-                model_weight = detectron2.model_zoo.get_checkpoint_url(model_config)
-            cfg.MODEL.WEIGHTS = model_weight
-        
+                model_weight = model_chkpoint
+            cfg.load_from = model_weight
+            cfg.launcher = 'none'
+            cfg.resume = False
+
+            # update class labels
+            cfg = self.__set_class_labels(cfg, class_labels)
         except:
-            raise FileNotFoundError('The path or name of the configuration file `{}` is incorrect. JustDeepIt cannot find or download.'.format(model_config))
-           
+            raise JDIError('JustDeepIt cannot find or download the configuration file.'
+                           'Please check the file path or the internet connection and try agian.')
+        
+        return  cfg
+        
+    
+
+    def __set_class_labels(self, cfg, class_labels):
+        def __set_cl(cfg, class_labels):
+            for cfg_key in cfg:
+                if isinstance(cfg[cfg_key], dict):
+                    __set_cl(cfg[cfg_key], class_labels)
+                elif isinstance(cfg[cfg_key], (list, tuple)):
+                    if isinstance(cfg[cfg_key][0], dict):
+                        for elem in cfg[cfg_key]: 
+                            __set_cl(elem, class_labels)
+                else:
+                    if cfg_key == 'classes':
+                        cfg[cfg_key] = class_labels
+                    elif cfg_key == 'num_classes' or cfg_key == 'num_things_classes':
+                        cfg[cfg_key] = len(class_labels)
+            return cfg
+        
+        cfg.data_root = ''
+        cfg.merge_from_dict(dict(metainfo = dict(classes=class_labels)))
+        cfg.model = __set_cl(cfg.model, class_labels)
+        # for RetinaNet: ResNet: init_cfg and pretrained cannot be specified at the same time
+        if 'pretrained' in cfg.model:
+            del cfg.model['pretrained']
         return cfg
     
+
+
+    def train(self,
+              train_dataset,
+              valid_dataset=None,
+              test_dataset=None,
+              optimizer=None,
+              scheduler=None,
+              score_cutoff=0.5,
+              batchsize=8,
+              epoch=100,
+              cpu=8,
+              gpu=1):
+        
+        # CPU/GPUs
+        self.__set_device(gpu)
+
+        # training params
+        self.__set_optimizer(optimizer)
+        self.__set_scheduler(scheduler)
+       
+        # datasets
+        if self.model_class == 'od':
+            dataloader = DataLoader(self.cfg,
+                                    train_dataset, valid_dataset, test_dataset,
+                                    batchsize, epoch, cpu,
+                                    with_bbox=True, with_mask=False)
+        elif self.model_class == 'is':
+            dataloader = DataLoader(self.cfg,
+                                    train_dataset, valid_dataset, test_dataset,
+                                    batchsize, epoch, cpu,
+                                    with_bbox=True, with_mask=True)
+        else:
+            raise ValueError('The model class is not supported.')
+        self.cfg.merge_from_dict(dataloader.cfg)
+        self.cfg.default_hooks.checkpoint.interval = 20
+
+        # training
+        runner = mmengine.runner.Runner.from_cfg(self.cfg)
+        runner.train()
+    
     
     
+    def __set_device(self, gpu=0):
+        if gpu != 0 and gpu != 1:
+            raise JDIError('The current JustDeepIt does not support multiple GPUs for trianing. '
+                           'Set `gpu` to 0 or 1.')
+        gpu = gpu if torch.cuda.is_available() else 0
+        gpu = torch.cuda.device_count() if torch.cuda.device_count() < gpu else gpu
+        self.cfg.device = 'cuda:0' if gpu > 0 else 'cpu'
     
-    def __parse_class_labels(self, class_labels):
-        cl = None
-        if class_labels is None:
-            raise ValueError('`class_labels` is required to build model.')
-        else:
-            if isinstance(class_labels, list):
-                cl = class_labels
-            elif isinstance(class_labels, str):
-                cl = []
-                with open(class_labels, 'r') as infh:
-                    for cl_ in infh:
-                        cl.append(cl_.replace('\n', ''))
-            else:
-                raise ValueError('Unsupported data type of `class_labels`. Set a path to a file which contains class labels or set a list of class labels.')
-        return cl
-    
-    
-    def __get_device(self, gpu=1):
-        device = 'cpu'
-        if gpu > 0:
-            if torch.cuda.is_available():
-                device = 'cuda'
-        # device = torch.device(device)
-        return device
-   
-    
-        
-
-    def __dataloader(self, train_data_fpath):
-        data_dict = []
-
-        with open(train_data_fpath, mode='r', encoding='utf-8') as datafh:
-            for imdata in datafh:
-                imdata = imdata.replace('\n', '').split('\t')
-                imann = ImageAnnotation(train_data_fpath[0], train_data_fpath[1], train_data_fpath[2])
-                data_dict.append(imann.format('detectron'))
-
-        return data_dict
-
-
-    
-    def __n_train_images(self, image_dpath):
-        n = 0
-        for fpath in glob.glob(os.path.join(image_dpath, '*')):
-            if os.path.splitext(fpath)[1].lower() in ['.jpg', '.jpeg', '.png', '.tif', '.tiff']:
-                n += 1
-        return n
-    
-    
-    def train(self, image_dpath, annotation,
-              optimizer=None, scheduler=None,
-              batchsize=8, epoch=100, score_cutoff=0.5, cpu=4, gpu=1):
-        lr = 0.001
-        
-        if not torch.cuda.is_available():
-            gpu = 0
-        if torch.cuda.device_count() < gpu:
-            gpu = torch.cuda.device_count()
-        
-        # train settings
-        train_dataset_id = 'ds:{}_train'.format(image_dpath)
-        self.cfg.MODEL.DEVICE =self.__get_device(gpu)
-        self.cfg.MODEL.ROI_HEADS.SCORE_THRESH_TEST = score_cutoff
-        self.cfg.DATALOADER.NUM_WORKERS = cpu
-        self.cfg.SOLVER.IMS_PER_BATCH   = batchsize
-        self.cfg.SOLVER.BASE_LR  = lr
-        self.cfg.SOLVER.MAX_ITER = int(self.__n_train_images(image_dpath) / batchsize * epoch)
-        self.cfg.DATASETS.TRAIN = (train_dataset_id, )
-        self.cfg.DATASETS.TEST = ()
-
-        # datasest settings
-        detectron2.data.DatasetCatalog.clear()
-        detectron2.data.datasets.register_coco_instances(train_dataset_id, {}, annotation, image_dpath)
-        detectron2.data.MetadataCatalog.get(train_dataset_id).set(thing_classes=self.class_labels)
-        
-        # train model
-        trainer = detectron2.engine.DefaultTrainer(self.cfg)
-        trainer.resume_or_load(resume=False)
-        trainer.train()
-        
-        self.model = trainer.model
-
-    
-    def inference(self, image_path, score_cutoff=0.5, batchsize=8, cpu=4, gpu=1):
-        images_fpath = []
-        if isinstance(image_path, list):
-            images_fpath = image_path
-        elif os.path.isfile(image_path):
-            images_fpath = [image_path]
+
+    
+    def __set_optimizer(self, optimizer):
+        if optimizer is not None and optimizer.replace(' ', '') != '':
+            if optimizer[0] != '{' or optimizer[0:4] != 'dict':
+                optimizer = 'dict(' + optimizer + ')'
+            self.cfg.optimizer = eval(optimizer)
+    
+    
+
+    def __set_scheduler(self, scheduler):
+        if scheduler is not None and scheduler.replace(' ', '') != '':
+            if scheduler[0] != '{' or scheduler[0:4] != 'dict':
+                scheduler = 'dict(' + scheduler + ')'
+            self.cfg.scheduler = eval(scheduler)
+    
+
+
+    def save(self, weight_fpath, config_fpath=None):
+        # weight
+        if not weight_fpath.endswith('.pth'):
+            weight_fpath + '.pth'
+        with open(os.path.join(self.cfg.work_dir, 'last_checkpoint')) as chkf:
+            last_chk = chkf.readline().strip()
+            shutil.copy2(last_chk, weight_fpath)
+        # config
+        if config_fpath is None:
+            config_fpath = os.path.splitext(weight_fpath)[0] + '.py'
+        self.cfg.dump(config_fpath)
+
+
+
+    def inference(self,
+                  images,
+                  score_cutoff=0.5,
+                  batchsize=8,
+                  cpu=4,
+                  gpu=1):
+        
+        self.__set_device(gpu)
+        
+        # load images for inference
+        target_images = load_images(images)
+        assert len(target_images) > 0, 'No images found in {}'.format(images)
+        
+        # set params
+        pipeline = DataPipeline()
+        self.cfg.merge_from_dict(
+            dict(test_dataloader=dict(
+                _delete_=True,
+                batch_size=1,
+                num_workers=cpu,
+                persistent_workers=True,
+                drop_last=False,
+                sampler=dict(type='DefaultSampler', shuffle=False),
+                dataset=dict(
+                    type='CocoDataset',
+                    pipeline = pipeline.inference,
+                    metainfo=self.cfg.metainfo))))
+
+
+        # load model
+        model = mmdet.apis.init_detector(self.cfg,
+                                         self.cfg.load_from,
+                                         device=self.cfg.device)
+        
+        # inference
+        outputs = mmdet.apis.inference_detector(model, target_images)
+
+        # format
+        outputs_fmt = []
+        for target_image, output in zip(target_images, outputs):
+            outputs_fmt.append(
+                ImageAnnotation(target_image,
+                                self.__format_annotation(output,
+                                                         score_cutoff)))
+        
+        return ImageAnnotations(outputs_fmt)
+    
+    
+    
+    def __format_annotation(self, output, score_cutoff):
+        if 'bboxes' in output.pred_instances:
+            pred_bboxes = output.pred_instances.bboxes.detach().cpu().numpy().tolist()
+            pred_labels = output.pred_instances.labels.detach().cpu().numpy().tolist()
+            pred_scores = output.pred_instances.scores.detach().cpu().numpy().tolist()
         else:
-            for f in glob.glob(os.path.join(image_path, '*')):
-                if os.path.splitext(f)[1].lower() in ['.jpg', '.png', '.tiff']:
-                    images_fpath.append(f)
-            
-        # build model for inference
-        if self.detector is not None:
-            model = self.detector
+            pred_bboxes = []
+            pred_labels = []
+            pred_scores = []
+        
+        if 'masks' in output.pred_instances:
+            pred_masks = output.pred_instances.masks.detach().cpu().numpy()
         else:
-            self.cfg.MODEL.ROI_HEADS.SCORE_THRESH_TEST = score_cutoff
-            self.cfg.MODEL.DEVICE = self.__get_device(gpu)
-            self.cfg.DATALOADER.NUM_WORKERS = cpu
-            self.cfg.SOLVER.IMS_PER_BATCH = batchsize
-            model = detectron2.modeling.build_model(self.cfg)
-            model.eval()
-            checkpointer = detectron2.checkpoint.DetectionCheckpointer(model)
-            checkpointer.load(self.cfg.MODEL.WEIGHTS)
-            self.detector = model
-        
-        aug = detectron2.data.transforms.ResizeShortestEdge(
-            [self.cfg.INPUT.MIN_SIZE_TEST, self.cfg.INPUT.MIN_SIZE_TEST],
-            self.cfg.INPUT.MAX_SIZE_TEST
-        )
-        # mini-batch inferences
-        outputs = []
-        for batch_id in tqdm.tqdm(range(math.ceil(len(images_fpath) / batchsize)), desc='Processed batches:', leave=True):
-            batch_id_from = batch_id * batchsize
-            batch_id_to = min((batch_id + 1) * batchsize, len(images_fpath))
-            batch_images_fpath = images_fpath[batch_id_from:batch_id_to]
-            inputs = []
-            for image_fpath in batch_images_fpath:
-                pil_im = PIL.Image.open(image_fpath).convert('RGB')
-                original_image = np.array(PIL.ImageOps.exif_transpose(pil_im))
-                original_image = original_image[:, :, ::-1]
-                height, width = original_image.shape[:2]
-                image = aug.get_transform(original_image).apply_image(original_image)
-                image = torch.as_tensor(image.astype('float32').transpose(2, 0, 1))
-                inputs.append({'image': image, 'height': height, 'width': width})
-                pil_im.close()
-        
-            # inference
-            with torch.no_grad():
-                batch_outputs = model(inputs)
-        
-            for image_fpath, output in zip(batch_images_fpath, batch_outputs):
-                output_fmt = None
-                if 'instances' in output:
-                    output['instances'] =  output['instances'].to('cpu')
-                    pred_classes = output['instances'].pred_classes.numpy()
-                    scores = output['instances'].scores.numpy()
-                    pred_boxes = np.array([k.numpy() for k in output['instances'].pred_boxes]).astype(np.int32)
-                    if hasattr(output['instances'], 'pred_masks'):
-                        pred_masks = np.array([k.numpy() for k in output['instances'].pred_masks]).astype(np.uint8)
-                    else:
-                        pred_masks = [None] * len(pred_boxes)
-                
-                    output_fmt = self.__format_annotation(
-                        pred_classes, scores, pred_boxes, pred_masks, score_cutoff, image_fpath
-                    )
-                outputs.append(ImageAnnotation(image_fpath, output_fmt))
+            pred_masks = [None] * len(pred_bboxes)
         
-        return ImageAnnotations(outputs)
-    
-    
-    def __format_annotation(self, pred_classes, scores, pred_boxes, pred_masks, score_cutoff, tmp):
         regions = []
-        for cl, score, bbox, segm  in zip(pred_classes, scores, pred_boxes, pred_masks):
-            if score > score_cutoff:
-                cl = self.class_labels[cl]
-                bb = bbox.tolist()
-                sg = None
-                if (segm is not None) and (np.sum(segm) > 0):
-                    sg = skimage.measure.find_contours(segm.astype(np.uint8), 0.5)
-                
+        for pred_bbox, pred_label, pred_score, pred_mask in zip(
+                pred_bboxes, pred_labels, pred_scores, pred_masks):
+            if pred_score > score_cutoff:
                 region = {
-                    'id'     : len(regions) + 1,
-                    'class'  : cl,
-                    'score'  : score,
-                    'bbox'   : bb,
+                    'id': len(regions) + 1,
+                    'class': self.class_labels[pred_label],
+                    'score': pred_score,
+                    'bbox': pred_bbox #.astype(np.int32)
                 }
-                if sg is not None:
+                if pred_mask is not None:
+                    sg = skimage.measure.find_contours(pred_mask, 0.5)
                     region['contour'] = sg[0][:, [1, 0]]
                 regions.append(region)
-
+        
         return regions
         
     
-    def save(self, weight_fpath, config_fpath=None):
-        if not weight_fpath.endswith('.pth'):
-            weight_fpath + '.pth'
-        
-        # pth file
-        if self.model is not None:
-            torch.save(self.model.to('cpu').state_dict(), weight_fpath)
-        
-        # config file
-        if config_fpath is None:
-            config_fpath = os.path.splitext(weight_fpath)[0] + '.yaml'
-        with open(config_fpath, 'w') as outfh:
-            outfh.write(self.cfg.dump())
+
+
```

### Comparing `JustDeepIt-0.1.30/justdeepit/models/utils/u2net.py` & `justdeepit-0.2.0/justdeepit/models/utils/u2net.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/models/utils/unet.py` & `justdeepit-0.2.0/justdeepit/models/utils/unet.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/src/font/NotoSans-Medium.ttf` & `justdeepit-0.2.0/justdeepit/src/font/NotoSans-Medium.ttf`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/src/font/OFL.txt` & `justdeepit-0.2.0/justdeepit/src/font/OFL.txt`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/utils.py` & `justdeepit-0.2.0/justdeepit/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,26 @@
 import re
 import gzip
 import json
 import base64
 import hashlib
 import random
 import string
+import glob
 import pkg_resources
 import xml.etree.ElementTree as ET
 import numpy as np
 import cv2
 import skimage
 import skimage.io
 import skimage.color
 import skimage.measure
 import skimage.draw
 import PIL.Image
 import PIL.ImageOps
-import tempfile
-import pycocotools.coco
-import pycocotools.cocoeval
 
 
 
 class JsonEncoder(json.JSONEncoder):
     """Convert NumPy object to JSON object
     
     Convert NumPy objects to JSON object during writting process.
@@ -193,28 +191,36 @@
         if annotation_format == 'auto':
             annotation_format = self.__estimate_annotation_format(annotation)
         
         if annotation_format == None:
             return annotation
         if annotation_format == 'base':
             return annotation
+        elif annotation_format == 'json':
+            return self.__set_regions_from_json(annotation)
         elif annotation_format == 'array':
             return self.__set_regions_from_array(annotation)
         elif annotation_format == 'rgbmask':
             return self.__set_regions_from_rgbmask(annotation)
         elif annotation_format == 'vott':
             return self.__set_regions_from_vott(annotation)
         elif 'voc' in annotation_format:
             return self.__set_regions_from_voc(annotation)
         elif annotation_format == 'coco':
             return self.__set_regions_from_coco(annotation)
         else:
             raise ValueError('Undefined format.')
     
     
+    def __set_regions_from_json(self, json_fpath):
+        with open(json_fpath, 'r') as infh:
+            regions = json.load(infh)
+        return regions
+
+
     def __set_regions_from_coco(self, coco):
         regions = []
         coco_data = None
         with open(coco, 'r') as jsonfh:
             coco_data = json.load(jsonfh)
         
         # find image ID
@@ -464,15 +470,15 @@
         Additionally, this method supports the conversion of class object
         :class:`ImageAnnotation <justdeepit.utils.ImageAnnotation>`
         into a mask image represented by
         class object :class:`numpy.ndarray`.
         
         Args:
             annotation_format (str): A string to specify the format to be formatted.
-                                     ``coco``, ``voc``, or ``mask`` can be
+                                     ``json``, ``coco``, ``voc``, or ``mask`` can be
                                      specified.
             file_path (str): A path to save the converted annotation.
                              If ``None`` is given, return the converted annotation
                              in string or dictionary.
         
         Returns:
             If ``file_path`` is ``None``, return a string (for Pascal VOC format),
@@ -489,15 +495,18 @@
             >>> 
             >>> ann.format('voc', './path/to/image.xml')
         
         """
         fmt_obj = None
         if annotation_format == 'base':
             return self.regions
-        
+
+        if annotation_format == 'json':
+            return self.__format2base(file_path)
+
         elif annotation_format.lower() == 'array' or annotation_format.lower() == 'numpy' or annotation_format.lower() == 'mask':
             return self.__format2mask(file_path)[1]
         
         #elif annotation_format.lower() == 'vott':
         #    return self.__format2vott(file_path)
     
         elif annotation_format.lower() == 'coco':
@@ -519,17 +528,18 @@
     
     
     def __format2base(self, output_fpath=None):
         if output_fpath is None:
             return self.regions
         else:
             with open(output_fpath, 'w', encoding='utf-8') as fh:
-                json.dump(self.regions, fh, cls=JsonEncoder, ensure_ascii=False)
+                json.dump(self.regions, fh, cls=JsonEncoder, ensure_ascii=False, indent=4)
+
+
 
-    
     def __format2voc(self, output_fpath=None):
         tmpl_voc = '''<annotation>
   <folder></folder>
   <filename>{}</filename>
   <source>
     <database>Unknown</database>
     <annotation>Unknown</annotation>
@@ -610,30 +620,28 @@
                 'image_id': image_id,
                 'category_id': cate2id[region['class']],
                 'bbox': [region['bbox'][0],
                          region['bbox'][1],
                          region['bbox'][2] - region['bbox'][0],
                          region['bbox'][3] - region['bbox'][1]],
                 'area': (region['bbox'][2] - region['bbox'][0]) * (region['bbox'][3] - region['bbox'][1]),
-                'score': region['score'],
                 'iscrowd': 0
             }
             if 'contour' in region and region['contour'] is not None:
                 ann['segmentation'] = [region['contour'].flatten(order='C').tolist()]
                 ann['area'] = self.__calc_area_from_polygon(region['contour'])
             
             tmpl['annotations'].append(ann) 
         
         
         if output_fpath is None:
             return tmpl
         else:
             with open(output_fpath, 'w', encoding='utf-8') as fh:
-                json.dump(tmpl, fh, cls=JsonEncoder, ensure_ascii=False)
-                #json.dump(tmpl, fh, cls=JsonEncoder, ensure_ascii=False, indent=4)
+                json.dump(tmpl, fh, cls=JsonEncoder, ensure_ascii=False, indent=4)
 
 
 
     
     def __format2vott(self, output_fpath=None):
         tmpl = {}
         
@@ -669,23 +677,21 @@
             tmpl['regions'].append(r)
         
         if output_fpath is None:
             return tmpl
         else:
             if os.path.basename(output_fpath) == 'md5':
                 with open(os.path.join(os.path.dirname(output_fpath), tmpl['asset']['id'] + '-asset.json'), 'w', encoding='utf-8') as fh:
-                    json.dump(tmpl, fh, cls=JsonEncoder, ensure_ascii=False)
-                    #json.dump(tmpl, fh, cls=JsonEncoder, ensure_ascii=False, indent=4)
+                    json.dump(tmpl, fh, cls=JsonEncoder, ensure_ascii=False, indent=4)
             elif os.path.splitext(output_fpath)[1] in ['.gzip', '.gz']:
                 with gzip.open(output_fpath, 'wt', encoding='utf-8') as fh:
-                    json.dump(tmpl, fh, cls=JsonEncoder, ensure_ascii=False)
+                    json.dump(tmpl, fh, cls=JsonEncoder, ensure_ascii=False, indent=4)
             else:
                 with open(output_fpath, 'w', encoding='utf-8') as fh:
-                    json.dump(tmpl, fh, cls=JsonEncoder, ensure_ascii=False)
-                    #json.dump(tmpl, fh, cls=JsonEncoder, ensure_ascii=False, indent=4)
+                    json.dump(tmpl, fh, cls=JsonEncoder, ensure_ascii=False, indent=4)
    
     
     
     
     def __format2mask(self, output_fpath=None):
         if self.mask is None:
             mask = []
@@ -1386,124 +1392,20 @@
         
         # save project.vott
             
         # save assets.json
             
 
 
-def __load_json(fpath):
-    with open(fpath) as fh:
-        d = json.load(fh)
-    return d
-
-def __index_common_images(gt_fpath, pred_fpath):
-    # ground truth
-    gt2id = {}
-    d = __load_json(gt_fpath)
-    for im in d['images']:
-        gt2id[os.path.basename(im['file_name'])] = str(im['id'])
-
-    # prediction result
-    pred2id = {}
-    d = __load_json(pred_fpath)
-    for im in d['images']:
-        pred2id[os.path.basename(im['file_name'])] = str(im['id'])
-
-    # common images betweeen groundtruth and prediction reuslt
-    common_images = set(gt2id.keys()) & set(pred2id.keys())
-    im2id = {}
-    for i, common_image in enumerate(sorted(list(common_images))):
-        im2id[common_image] = i + 1
-
-    id2id = {'gt': {}, 'pred': {}}
-    for im_fname, im_id in im2id.items():
-        id2id['gt'][gt2id[im_fname]] = im_id
-        id2id['pred'][pred2id[im_fname]] = im_id
-
-    return id2id
-
-
-def __modify_coco(coco_fpath, id2id):
-    d = __load_json(coco_fpath)
-    d_new = {}
-
-    for coco_key in d.keys():
-        if coco_key == 'images':
-            d_new['images'] = []
-            for x in d['images']:
-                if str(x['id']) in id2id:
-                    x['id'] = id2id[str(x['id'])]
-                    d_new['images'].append(x)
-        elif coco_key == 'annotations':
-            d_new['annotations'] = []
-            for x in d['annotations']:
-                if str(x['image_id']) in id2id:
-                    x['image_id'] = id2id[str(x['image_id'])]
-                    d_new['annotations'].append(x)
-        else:
-            d_new[coco_key] = d[coco_key]
-
-    return d_new
-
-
-
-def __save_json(d, k=None):
-    fd, temp_fpath = tempfile.mkstemp()
-    with open(temp_fpath, 'w') as fh:
-        if k is None:
-            json.dump(d, fh, indent=4)
-        else:
-            json.dump(d[k], fh, indent=4)
-    return temp_fpath
-
-
-
-def coco_eval(gt_fpath, pred_fpath):
-    """Calculate validation scores from inference results
-    
-    This function calculate the validation scores (mAP, mPR) from inference results.
-    This function requires two COCO format files as inputs, one is ground truth and
-    the other is inference result. The image IDs are allowed to be different between
-    two COCO format files, as this function will reindex image IDs according image
-    name between two COCO format files.
-    
-    Args:
-        gt_fpath (str): A path to COCO format file storing the ground truth annotations.
-        pred_fpath (str): A path to COCO format file storing the inference result.
-    
-    Returns:
-        A list contains validation scores.
-    
-    Examples:
-        >>> from justdeepit.utils import coco_eval
-        >>> 
-        >>> scores = coco_eval('gt.coco.json', 'predicted.coco.json')
-        >>> print(scores)
-        
-    """
-
-    id2id = __index_common_images(gt_fpath, pred_fpath)
-    gt_coco_dict = __modify_coco(gt_fpath, id2id['gt'])
-    pred_coco_dict = __modify_coco(pred_fpath, id2id['pred'])
-    gt_coco_fpath = __save_json(gt_coco_dict)
-    pred_coco_fpath = __save_json(pred_coco_dict, 'annotations')
-
-    gt_coco = pycocotools.coco.COCO(gt_coco_fpath)
-    pred_coco = gt_coco.loadRes(pred_coco_fpath)
-    coco_eval = pycocotools.cocoeval.COCOeval(gt_coco, pred_coco, 'bbox')
-    coco_eval.evaluate()
-    coco_eval.accumulate()
-    coco_eval.summarize()
-    
-    os.remove(gt_coco_fpath)
-    os.remove(pred_coco_fpath)
-    
-    return coco_eval.stats
-
-
-
-
-
-
-
+def load_images(images):
+    image_list = []
+    if isinstance(images, list):
+        image_list = images
+    elif os.path.isfile(images):
+        image_list = [images]
+    else:
+        for f in glob.glob(os.path.join(images, '*')):
+            if os.path.splitext(f)[1].lower() in ['.jpg', '.png', '.tiff']:
+                image_list.append(f)
 
+    return image_list
```

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/app.py` & `justdeepit-0.2.0/justdeepit/webapp/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,14 @@
         params = {}
         params.update({'module': module_id})
         
         if module_id == 'OD' or module_id == 'IS':
             params.update({
                 'config': {
                     'status': 'WAITING',
-                    'backend': 'MMDetection',
                     'architecture': 'Faster R-CNN' if module_id == 'OD' else 'Mask R-CNN',
                     'config': '',
                     'class_label': '',
                     'cpu': 4,
                     'gpu': 1 if torch.cuda.is_available() else 0,
                     'workspace': self.workspace,
                 },
@@ -254,21 +253,19 @@
     moduleframe.activate_module(module_id)
     # initialize module and parameters
     req_dict = {
         'request': request,
         'justdeepit_version': justdeepit.__version__,
         'module': module_id,
         'module_name': moduleframe.module_desc,
-        'backend': moduleframe.params['config']['backend'],
         'supported_formats': get_supported_formats(module_id),
     }
     if module_id == 'OD' or module_id == 'IS':
         req_dict.update({
-            'backends': ['MMDetection', 'Detectron2'],
-            'architectures': get_architectures(module_id, moduleframe.params['config']['backend'], 'list'),
+            'architectures': get_architectures(module_id, moduleframe.params['config'], 'list'),
         })
     elif module_id == 'SOD':
         req_dict.update({
             'architectures': get_architectures(module_id, output_format='list'),
         })
     else:
         raise NotImplementedError('JustDeepIt only supports OD, IS, and SOD.')
@@ -381,21 +378,19 @@
                                 moduleframe.params['training']['model_weight'],
                                 moduleframe.params['training']['optimizer'],
                                 moduleframe.params['training']['scheduler'],
                                 moduleframe.params['training']['batchsize'],
                                 moduleframe.params['training']['epoch'],
                                 moduleframe.params['training']['cutoff'],
                                 moduleframe.params['config']['cpu'],
-                                moduleframe.params['config']['gpu'],
-                                moduleframe.params['config']['backend'])
+                                moduleframe.params['config']['gpu'])
             
             status = validate_status(status)
             if status == 'COMPLETED':
-                model_config_ext = '.py' if moduleframe.params['config']['backend'][0].lower() == 'm' else '.yaml'
-                moduleframe.update_params({'config': os.path.splitext(moduleframe.params['training']['model_weight'])[0] + model_config_ext},
+                moduleframe.update_params({'config': os.path.splitext(moduleframe.params['training']['model_weight'])[0] + '.py'},
                                           'config')
                 moduleframe.update_params({'model_weight': moduleframe.params['training']['model_weight']},
                                           'inference')
             moduleframe.update_status('training', status)
     
         except BaseException as e:
             traceback.print_exc()
@@ -420,16 +415,15 @@
                                 moduleframe.params['inference']['image_folder'],
                                 moduleframe.params['config']['architecture'],
                                 moduleframe.params['config']['config'],
                                 moduleframe.params['inference']['model_weight'],
                                 moduleframe.params['inference']['cutoff'],
                                 moduleframe.params['inference']['batchsize'],
                                 moduleframe.params['config']['cpu'],
-                                moduleframe.params['config']['gpu'],
-                                moduleframe.params['config']['backend'])
+                                moduleframe.params['config']['gpu'])
             status_2 = moduleframe.module.summarize_objects(moduleframe.params['config']['cpu'])
             
             status = validate_status([status_1, status_2])
             moduleframe.update_status('inference', status)
         
         except BaseException as e:
             traceback.print_exc()
@@ -559,33 +553,26 @@
 @app.get('/api/params')
 def get_params():
     return JSONResponse(content=moduleframe.params)
     
 
 
 @app.get('/api/architecture')
-def get_architectures(module: str = '', backend: str = 'mmdetection', output_format: str = 'json'):
-    backend = backend.lower()
+def get_architectures(module: str = '', output_format: str = 'json'):
     m = None
     if module == 'OD':
-        if backend not in ['mmdetection', 'detectron2']:
-            backend = 'mmdetection'
         m = justdeepit.models.OD(model_arch=None)
     elif module == 'IS':
-        if backend not in ['mmdetection', 'detectron2']:
-            backend = 'mmdetection'
         m = justdeepit.models.IS(model_arch=None)
     elif module == 'SOD':
-        if backend not in ['pytorch']:
-            backend = 'pytorch'
         m = justdeepit.models.SOD(model_arch=None)
     
     archs = None
     if m is not None:
-        archs = m.available_architectures(backend)
+        archs = m.available_architectures()
     
     if output_format == 'json':
         return JSONResponse(content=archs)
     else:
         return archs
```

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/appbase.py` & `justdeepit-0.2.0/justdeepit/webapp/appbase.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/appis.py` & `justdeepit-0.2.0/justdeepit/webapp/appis.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,23 +13,23 @@
         self.app = 'IS'
         self.images = []
     
     
     def train_model(self, class_label, image_dpath, annotation_path, annotation_format,
                     model_arch='maskrcnn', model_config=None, model_weight=None, 
                     optimizer=None, scheduler=None,
-                    batchsize=8, epoch=100, score_cutoff=0.5, cpu=4, gpu=1, backend='mmdetection'):
+                    batchsize=8, epoch=100, score_cutoff=0.5, cpu=4, gpu=1):
         return super().train_model(class_label, image_dpath, annotation_path, annotation_format,
                                    model_arch, model_config, model_weight, 
                                    optimizer, scheduler,
-                                   batchsize, epoch, score_cutoff, cpu, gpu, backend)
+                                   batchsize, epoch, score_cutoff, cpu, gpu)
     
     
     def detect_objects(self, class_label, image_dpath,
                        model_arch='maskrcnn', model_config=None, model_weight=None,
-                       score_cutoff=0.5, batchsize=8, cpu=4, gpu=1, backend='mmdetection'):
+                       score_cutoff=0.5, batchsize=8, cpu=4, gpu=1):
         return super().detect_objects(class_label, image_dpath,
                                       model_arch, model_config, model_weight,
-                                      score_cutoff, batchsize, cpu, gpu, backend)
+                                      score_cutoff, batchsize, cpu, gpu)
```

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/appod.py` & `justdeepit-0.2.0/justdeepit/webapp/appod.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,33 +22,33 @@
     
     def __init__(self, workspace):
         super().__init__(workspace)
         self.app = 'OD'
     
     
      
-    def __build_model(self, class_label, model_arch, model_config, model_weight, backend):
+    def __build_model(self, class_label, model_arch, model_config, model_weight):
         init_model_weight = model_weight if os.path.exists(model_weight) else None
         if self.app == 'OD':
             return justdeepit.models.OD(class_label, model_arch, model_config, init_model_weight,
-                                        os.path.join(self.workspace_, 'tmp'), backend)
+                                        os.path.join(self.workspace_, 'tmp'))
         elif self.app == 'IS':
             return justdeepit.models.IS(class_label, model_arch, model_config, init_model_weight,
-                                        os.path.join(self.workspace_, 'tmp'), backend)
+                                        os.path.join(self.workspace_, 'tmp'))
     
     
     
     def train_model(self, class_label, image_dpath, annotation_path, annotation_format,
                     model_arch='fasterrcnn', model_config=None, model_weight=None, 
                     optimizer=None, scheduler=None,
-                    batchsize=8, epoch=100, score_cutoff=0.5, cpu=4, gpu=1, backend='mmdetection'):
+                    batchsize=8, epoch=100, score_cutoff=0.5, cpu=4, gpu=1):
         job_status = self.set_jobstatus(self.code.TRAINING, self.code.JOB__TRAIN_MODEL, self.code.STARTED, '')
         try:
             self.check_training_images(image_dpath, annotation_path, annotation_format, class_label)
-            model = self.__build_model(class_label, model_arch, model_config, model_weight, backend)
+            model = self.__build_model(class_label, model_arch, model_config, model_weight)
             model.train(image_dpath, annotation_path, annotation_format,
                         optimizer, scheduler,
                         batchsize, epoch, score_cutoff, cpu, gpu)
             model.save(model_weight)
             
             job_status = self.set_jobstatus(self.code.TRAINING, self.code.JOB__TRAIN_MODEL, self.code.FINISHED, '')
         except KeyboardInterrupt:
@@ -63,15 +63,15 @@
         
         return job_status
     
     
     
     def detect_objects(self, class_label, image_dpath,
                        model_arch='fasterrcnn', model_config=None, model_weight=None,
-                       score_cutoff=0.8, batchsize=8, cpu=4, gpu=1, backend='mmdetection'):
+                       score_cutoff=0.8, batchsize=8, cpu=4, gpu=1):
         
         def __save_outputs(ws, image_fpath, output, app_id):
             image_name = os.path.splitext(os.path.basename(image_fpath))[0]
             if app_id == 'OD':
                 output.draw('bbox', os.path.join(ws, 'outputs', image_name + '.bbox.png'), label=True, score=True)
             elif app_id == 'IS':
                 output.draw('contour+bbox', os.path.join(ws, 'outputs', image_name + '.bbox.png'), label=True, score=True)
@@ -81,15 +81,15 @@
             self.check_query_images(image_dpath)
             self.seek_query_images()
         
             valid_ws = os.path.join(self.workspace_, 'tmp')
             # if config is not given, use the config saved during training process
             if model_config is None or model_config == '':
                 model_config = os.path.join(os.path.splitext(model_weight)[0] + '.yaml')
-            model = self.__build_model(class_label, model_arch, model_config, model_weight, backend)
+            model = self.__build_model(class_label, model_arch, model_config, model_weight)
             outputs = model.inference(self.images, score_cutoff, batchsize, cpu, gpu)
                 
             joblib.Parallel(n_jobs=cpu)(
                 joblib.delayed(__save_outputs)(self.workspace_, self.images[i], outputs[i], self.app) for i in range(len(self.images)))
             outputs.format('coco', os.path.join(self.workspace_, 'outputs', 'annotation.json'))
             
             job_status = self.set_jobstatus(self.code.INFERENCE, self.code.JOB__INFER, self.code.FINISHED, '')
```

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/appsod.py` & `justdeepit-0.2.0/justdeepit/webapp/appsod.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/static/jquery-3.6.0.min.js` & `justdeepit-0.2.0/justdeepit/webapp/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/static/jquery-3.6.0.min.map` & `justdeepit-0.2.0/justdeepit/webapp/static/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/static/styles.css` & `justdeepit-0.2.0/justdeepit/webapp/static/styles.css`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/static/tree.jquery.js` & `justdeepit-0.2.0/justdeepit/webapp/static/tree.jquery.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/static/tree.jquery.js.map` & `justdeepit-0.2.0/justdeepit/webapp/static/tree.jquery.js.map`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/static/utils.js` & `justdeepit-0.2.0/justdeepit/webapp/static/utils.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/templates/index.html` & `justdeepit-0.2.0/justdeepit/webapp/templates/index.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/templates/module.html` & `justdeepit-0.2.0/justdeepit/webapp/templates/module.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.30/justdeepit/webapp/templates/shutdown.html` & `justdeepit-0.2.0/justdeepit/webapp/templates/shutdown.html`

 * *Files identical despite different names*

