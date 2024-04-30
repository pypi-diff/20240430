# Comparing `tmp/figurify-0.0.7.tar.gz` & `tmp/figurify-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figurify-0.0.7.tar", last modified: Mon Apr 29 18:59:29 2024, max compression
+gzip compressed data, was "figurify-0.0.8.tar", last modified: Mon Apr 29 19:02:52 2024, max compression
```

## Comparing `figurify-0.0.7.tar` & `figurify-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 18:59:29.123898 figurify-0.0.7/
--rw-r--r--   0 julian    (1000) julian    (1000)     1068 2024-04-28 15:07:49.000000 figurify-0.0.7/LICENSE
--rw-r--r--   0 julian    (1000) julian    (1000)       60 2024-04-29 12:55:00.000000 figurify-0.0.7/MANIFEST.in
--rw-r--r--   0 julian    (1000) julian    (1000)    11470 2024-04-29 18:59:29.123898 figurify-0.0.7/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)     1945 2024-04-29 16:03:47.000000 figurify-0.0.7/README.md
--rw-r--r--   0 julian    (1000) julian    (1000)        5 2024-04-29 18:59:03.000000 figurify-0.0.7/VERSION.txt
--rw-r--r--   0 julian    (1000) julian    (1000)    11005 2024-04-29 16:31:38.000000 figurify-0.0.7/documentation.md
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 18:59:29.123898 figurify-0.0.7/figurify/
--rw-r--r--   0 julian    (1000) julian    (1000)        0 2024-04-29 18:58:20.000000 figurify-0.0.7/figurify/__init__.py
--rw-r--r--   0 julian    (1000) julian    (1000)      824 2024-04-28 06:24:04.000000 figurify-0.0.7/figurify/material_properties.py
--rw-r--r--   0 julian    (1000) julian    (1000)     2114 2024-04-28 06:52:47.000000 figurify-0.0.7/figurify/units.py
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 18:59:29.123898 figurify-0.0.7/figurify.egg-info/
--rw-r--r--   0 julian    (1000) julian    (1000)    11470 2024-04-29 18:59:29.000000 figurify-0.0.7/figurify.egg-info/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)      266 2024-04-29 18:59:29.000000 figurify-0.0.7/figurify.egg-info/SOURCES.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-04-29 18:59:29.000000 figurify-0.0.7/figurify.egg-info/dependency_links.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        9 2024-04-29 18:59:29.000000 figurify-0.0.7/figurify.egg-info/top_level.txt
--rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-04-29 18:59:29.123898 figurify-0.0.7/setup.cfg
--rw-r--r--   0 julian    (1000) julian    (1000)      762 2024-04-29 17:52:07.000000 figurify-0.0.7/setup.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 19:02:52.543905 figurify-0.0.8/
+-rw-r--r--   0 julian    (1000) julian    (1000)     1068 2024-04-28 15:07:49.000000 figurify-0.0.8/LICENSE
+-rw-r--r--   0 julian    (1000) julian    (1000)       60 2024-04-29 12:55:00.000000 figurify-0.0.8/MANIFEST.in
+-rw-r--r--   0 julian    (1000) julian    (1000)    11470 2024-04-29 19:02:52.543905 figurify-0.0.8/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)     1945 2024-04-29 16:03:47.000000 figurify-0.0.8/README.md
+-rw-r--r--   0 julian    (1000) julian    (1000)        5 2024-04-29 19:02:18.000000 figurify-0.0.8/VERSION.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)    11005 2024-04-29 16:31:38.000000 figurify-0.0.8/documentation.md
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 19:02:52.543905 figurify-0.0.8/figurify/
+-rw-r--r--   0 julian    (1000) julian    (1000)     1351 2024-04-29 19:02:06.000000 figurify-0.0.8/figurify/__init__.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      824 2024-04-28 06:24:04.000000 figurify-0.0.8/figurify/material_properties.py
+-rw-r--r--   0 julian    (1000) julian    (1000)     2114 2024-04-28 06:52:47.000000 figurify-0.0.8/figurify/units.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 19:02:52.543905 figurify-0.0.8/figurify.egg-info/
+-rw-r--r--   0 julian    (1000) julian    (1000)    11470 2024-04-29 19:02:52.000000 figurify-0.0.8/figurify.egg-info/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)      266 2024-04-29 19:02:52.000000 figurify-0.0.8/figurify.egg-info/SOURCES.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-04-29 19:02:52.000000 figurify-0.0.8/figurify.egg-info/dependency_links.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        9 2024-04-29 19:02:52.000000 figurify-0.0.8/figurify.egg-info/top_level.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-04-29 19:02:52.543905 figurify-0.0.8/setup.cfg
+-rw-r--r--   0 julian    (1000) julian    (1000)      762 2024-04-29 17:52:07.000000 figurify-0.0.8/setup.py
```

### Comparing `figurify-0.0.7/LICENSE` & `figurify-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `figurify-0.0.7/PKG-INFO` & `figurify-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figurify
-Version: 0.0.7
+Version: 0.0.8
 Summary: With figurify you can calculate figures, surfaces and physics.
 Author: Julian Hess
 Project-URL: Source, https://github.com/julian-hess/Figurify.git
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `figurify-0.0.7/README.md` & `figurify-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `figurify-0.0.7/documentation.md` & `figurify-0.0.8/documentation.md`

 * *Files identical despite different names*

### Comparing `figurify-0.0.7/figurify/material_properties.py` & `figurify-0.0.8/figurify/material_properties.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.7/figurify/units.py` & `figurify-0.0.8/figurify/units.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.7/figurify.egg-info/PKG-INFO` & `figurify-0.0.8/figurify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figurify
-Version: 0.0.7
+Version: 0.0.8
 Summary: With figurify you can calculate figures, surfaces and physics.
 Author: Julian Hess
 Project-URL: Source, https://github.com/julian-hess/Figurify.git
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `figurify-0.0.7/setup.py` & `figurify-0.0.8/setup.py`

 * *Files identical despite different names*

