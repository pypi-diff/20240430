# Comparing `tmp/dacutil-0.4.0.tar.gz` & `tmp/dacutil-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dacutil-0.4.0.tar", max compression
+gzip compressed data, was "dacutil-0.4.2.tar", max compression
```

## Comparing `dacutil-0.4.0.tar` & `dacutil-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      723 2024-02-09 09:12:52.124549 dacutil-0.4.0/README.md
--rw-r--r--   0        0        0      456 2024-03-19 04:31:32.012959 dacutil-0.4.0/dacutil/__init__.py
--rw-r--r--   0        0        0     4985 2024-02-07 08:23:14.673797 dacutil-0.4.0/dacutil/addict.py
--rw-r--r--   0        0        0     4334 2024-03-19 06:02:26.465638 dacutil-0.4.0/dacutil/config.py
--rw-r--r--   0        0        0     4881 2024-03-19 04:49:01.770472 dacutil-0.4.0/dacutil/crypt.py
--rw-r--r--   0        0        0     2659 2023-12-22 07:20:50.710357 dacutil-0.4.0/dacutil/dateutil.py
--rw-r--r--   0        0        0     1305 2024-04-23 05:11:48.225404 dacutil-0.4.0/dacutil/pyencryption.py
--rw-r--r--   0        0        0     1537 2024-03-05 06:12:40.996347 dacutil-0.4.0/dacutil/strutil.py
--rw-r--r--   0        0        0     1256 2023-12-22 05:44:36.724417 dacutil-0.4.0/dacutil/thai_mod11.py
--rw-r--r--   0        0        0     1329 2023-12-22 05:44:20.003573 dacutil-0.4.0/dacutil/worker.py
--rw-r--r--   0        0        0      542 2024-04-23 05:15:18.541452 dacutil-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 dacutil-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      723 2024-02-09 09:12:52.124549 dacutil-0.4.2/README.md
+-rw-r--r--   0        0        0      582 2024-04-30 05:47:39.908388 dacutil-0.4.2/dacutil/__init__.py
+-rw-r--r--   0        0        0     4985 2024-02-07 08:23:14.673797 dacutil-0.4.2/dacutil/addict.py
+-rw-r--r--   0        0        0     4334 2024-03-19 06:02:26.465638 dacutil-0.4.2/dacutil/config.py
+-rw-r--r--   0        0        0     4881 2024-03-19 04:49:01.770472 dacutil-0.4.2/dacutil/crypt.py
+-rw-r--r--   0        0        0     2659 2023-12-22 07:20:50.710357 dacutil-0.4.2/dacutil/dateutil.py
+-rw-r--r--   0        0        0     2315 2024-04-30 03:23:38.056171 dacutil-0.4.2/dacutil/pyencryption.py
+-rw-r--r--   0        0        0     1537 2024-03-05 06:12:40.996347 dacutil-0.4.2/dacutil/strutil.py
+-rw-r--r--   0        0        0     2519 2024-04-30 05:45:43.842511 dacutil-0.4.2/dacutil/thai_mod11.py
+-rw-r--r--   0        0        0     1329 2023-12-22 05:44:20.003573 dacutil-0.4.2/dacutil/worker.py
+-rw-r--r--   0        0        0      542 2024-04-30 05:46:33.384032 dacutil-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 dacutil-0.4.2/PKG-INFO
```

### Comparing `dacutil-0.4.0/README.md` & `dacutil-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dacutil-0.4.0/dacutil/addict.py` & `dacutil-0.4.2/dacutil/addict.py`

 * *Files identical despite different names*

### Comparing `dacutil-0.4.0/dacutil/config.py` & `dacutil-0.4.2/dacutil/config.py`

 * *Files identical despite different names*

### Comparing `dacutil-0.4.0/dacutil/crypt.py` & `dacutil-0.4.2/dacutil/crypt.py`

 * *Files identical despite different names*

### Comparing `dacutil-0.4.0/dacutil/dateutil.py` & `dacutil-0.4.2/dacutil/dateutil.py`

 * *Files identical despite different names*

### Comparing `dacutil-0.4.0/dacutil/strutil.py` & `dacutil-0.4.2/dacutil/strutil.py`

 * *Files identical despite different names*

### Comparing `dacutil-0.4.0/dacutil/worker.py` & `dacutil-0.4.2/dacutil/worker.py`

 * *Files identical despite different names*

### Comparing `dacutil-0.4.0/pyproject.toml` & `dacutil-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dacutil"
-version = "0.4.0"
+version = "0.4.2"
 description = "For Data Analytic"
 authors = ["Attapon Thanawong <attapon_srem@hotmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dacutil-0.4.0/PKG-INFO` & `dacutil-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dacutil
-Version: 0.4.0
+Version: 0.4.2
 Summary: For Data Analytic
 Author: Attapon Thanawong
 Author-email: attapon_srem@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

