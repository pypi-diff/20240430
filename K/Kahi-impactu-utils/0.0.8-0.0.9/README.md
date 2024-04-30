# Comparing `tmp/Kahi_impactu_utils-0.0.8.tar.gz` & `tmp/kahi_impactu_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kahi_impactu_utils-0.0.8.tar", last modified: Sat Mar 16 02:26:00 2024, max compression
+gzip compressed data, was "kahi_impactu_utils-0.0.9.tar", last modified: Tue Apr 23 15:20:09 2024, max compression
```

## Comparing `Kahi_impactu_utils-0.0.8.tar` & `kahi_impactu_utils-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:26:00.328414 Kahi_impactu_utils-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:26:00.324414 Kahi_impactu_utils-0.0.8/Kahi_impactu_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-16 02:26:00.000000 Kahi_impactu_utils-0.0.8/Kahi_impactu_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-16 02:26:00.000000 Kahi_impactu_utils-0.0.8/Kahi_impactu_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 02:26:00.000000 Kahi_impactu_utils-0.0.8/Kahi_impactu_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-16 02:26:00.000000 Kahi_impactu_utils-0.0.8/Kahi_impactu_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-16 02:26:00.000000 Kahi_impactu_utils-0.0.8/Kahi_impactu_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-16 02:25:48.000000 Kahi_impactu_utils-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-16 02:26:00.328414 Kahi_impactu_utils-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-16 02:25:48.000000 Kahi_impactu_utils-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:26:00.324414 Kahi_impactu_utils-0.0.8/kahi_impactu_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-16 02:25:48.000000 Kahi_impactu_utils-0.0.8/kahi_impactu_utils/String.py
--rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-03-16 02:25:48.000000 Kahi_impactu_utils-0.0.8/kahi_impactu_utils/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 02:25:48.000000 Kahi_impactu_utils-0.0.8/kahi_impactu_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-16 02:25:48.000000 Kahi_impactu_utils-0.0.8/kahi_impactu_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 02:26:00.328414 Kahi_impactu_utils-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-16 02:25:48.000000 Kahi_impactu_utils-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:20:09.910932 kahi_impactu_utils-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:20:09.910932 kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-23 15:20:09.000000 kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-23 15:20:09.000000 kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:20:09.000000 kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-23 15:20:09.000000 kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 15:20:09.000000 kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-23 15:20:09.910932 kahi_impactu_utils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:20:09.910932 kahi_impactu_utils-0.0.9/kahi_impactu_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/kahi_impactu_utils/String.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/kahi_impactu_utils/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/kahi_impactu_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/kahi_impactu_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:20:09.910932 kahi_impactu_utils-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/setup.py
```

### Comparing `Kahi_impactu_utils-0.0.8/Kahi_impactu_utils.egg-info/PKG-INFO` & `kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kahi_impactu_utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utils for Kahi Impactu project.
 Home-page: https://github.com/colav/Kahi_impactu_utils
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Kahi_impactu_utils-0.0.8/LICENSE` & `kahi_impactu_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Kahi_impactu_utils-0.0.8/PKG-INFO` & `kahi_impactu_utils-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kahi_impactu_utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utils for Kahi Impactu project.
 Home-page: https://github.com/colav/Kahi_impactu_utils
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Kahi_impactu_utils-0.0.8/README.md` & `kahi_impactu_utils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Kahi_impactu_utils-0.0.8/kahi_impactu_utils/Utils.py` & `kahi_impactu_utils-0.0.9/kahi_impactu_utils/Utils.py`

 * *Files identical despite different names*

### Comparing `Kahi_impactu_utils-0.0.8/setup.py` & `kahi_impactu_utils-0.0.9/setup.py`

 * *Files identical despite different names*

