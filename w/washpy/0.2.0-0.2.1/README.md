# Comparing `tmp/washpy-0.2.0.tar.gz` & `tmp/washpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "washpy-0.2.0.tar", max compression
+gzip compressed data, was "washpy-0.2.1.tar", max compression
```

## Comparing `washpy-0.2.0.tar` & `washpy-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    42028 2024-04-23 21:57:43.954435 washpy-0.2.0/LICENSE
--rw-r--r--   0        0        0     2045 2024-04-23 21:57:43.954435 washpy-0.2.0/README.md
--rw-r--r--   0        0        0      472 2024-04-24 19:35:10.382448 washpy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      315 2024-04-23 21:57:43.991103 washpy-0.2.0/washpy/__init__.py
--rw-r--r--   0        0        0     1086 2024-04-23 21:57:43.987770 washpy-0.2.0/washpy/authenticate.py
--rw-r--r--   0        0        0     3111 2024-04-24 19:26:06.083745 washpy-0.2.0/washpy/device_user.py
--rw-r--r--   0        0        0     4549 2024-04-24 16:21:19.635915 washpy-0.2.0/washpy/pExtended.py
--rw-r--r--   0        0        0      778 2024-04-23 21:57:43.987770 washpy-0.2.0/washpy/post_new_password.py
--rw-r--r--   0        0        0     9487 2024-04-24 19:32:43.580101 washpy-0.2.0/washpy/state.py
--rw-r--r--   0        0        0     3453 2024-04-23 21:57:43.987770 washpy-0.2.0/washpy/status.py
--rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 washpy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    42028 2024-04-23 21:57:43.954435 washpy-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2045 2024-04-23 21:57:43.954435 washpy-0.2.1/README.md
+-rw-r--r--   0        0        0      528 2024-04-30 21:23:51.840448 washpy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      315 2024-04-23 21:57:43.991103 washpy-0.2.1/washpy/__init__.py
+-rw-r--r--   0        0        0     1086 2024-04-23 21:57:43.987770 washpy-0.2.1/washpy/authenticate.py
+-rw-r--r--   0        0        0     3111 2024-04-24 19:26:06.083745 washpy-0.2.1/washpy/device_user.py
+-rw-r--r--   0        0        0     1224 2024-04-30 21:21:21.958949 washpy-0.2.1/washpy/pExtended.py
+-rw-r--r--   0        0        0      778 2024-04-23 21:57:43.987770 washpy-0.2.1/washpy/post_new_password.py
+-rw-r--r--   0        0        0     6158 2024-04-30 21:12:46.347166 washpy-0.2.1/washpy/state.py
+-rw-r--r--   0        0        0     3453 2024-04-23 21:57:43.987770 washpy-0.2.1/washpy/status.py
+-rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 washpy-0.2.1/PKG-INFO
```

### Comparing `washpy-0.2.0/LICENSE` & `washpy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `washpy-0.2.0/README.md` & `washpy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `washpy-0.2.0/washpy/authenticate.py` & `washpy-0.2.1/washpy/authenticate.py`

 * *Files identical despite different names*

### Comparing `washpy-0.2.0/washpy/device_user.py` & `washpy-0.2.1/washpy/device_user.py`

 * *Files identical despite different names*

### Comparing `washpy-0.2.0/washpy/post_new_password.py` & `washpy-0.2.1/washpy/post_new_password.py`

 * *Files identical despite different names*

### Comparing `washpy-0.2.0/washpy/status.py` & `washpy-0.2.1/washpy/status.py`

 * *Files identical despite different names*

### Comparing `washpy-0.2.0/PKG-INFO` & `washpy-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: washpy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A partial implementation of the Miele Professional IP Profile API
 Home-page: https://codeberg.org/johann.carl/washpy
 License: LGPL-3.0-only
 Author: Johann Carl Meyer
 Author-email: info@johannc.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

