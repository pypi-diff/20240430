# Comparing `tmp/dawgie-1.4.3rc2.tar.gz` & `tmp/dawgie-1.4.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawgie-1.4.3rc2.tar", last modified: Sat Mar 23 23:53:53 2024, max compression
+gzip compressed data, was "dawgie-1.4.3rc3.tar", last modified: Tue Apr 30 17:23:48 2024, max compression
```

## Comparing `dawgie-1.4.3rc2.tar` & `dawgie-1.4.3rc3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2024-03-23 23:53:53.245155 dawgie-1.4.3rc2/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2024-03-23 23:53:52.000000 dawgie-1.4.3rc2/LICENSE
--rw-r--r--   0 niessner  (1000) niessner  (1000)     9940 2024-03-23 23:53:53.245155 dawgie-1.4.3rc2/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2024-03-23 23:53:52.000000 dawgie-1.4.3rc2/README.md
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2024-03-23 23:53:53.245155 dawgie-1.4.3rc2/dawgie.egg-info/
--rw-r--r--   0 niessner  (1000) niessner  (1000)     9940 2024-03-23 23:53:53.000000 dawgie-1.4.3rc2/dawgie.egg-info/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6632 2024-03-23 23:53:53.000000 dawgie-1.4.3rc2/dawgie.egg-info/SOURCES.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2024-03-23 23:53:53.000000 dawgie-1.4.3rc2/dawgie.egg-info/dependency_links.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      245 2024-03-23 23:53:53.000000 dawgie-1.4.3rc2/dawgie.egg-info/requires.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2024-03-23 23:53:53.000000 dawgie-1.4.3rc2/dawgie.egg-info/top_level.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2024-03-23 23:53:53.245155 dawgie-1.4.3rc2/setup.cfg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6410 2024-03-23 23:51:14.000000 dawgie-1.4.3rc2/setup.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2024-04-30 17:23:48.070226 dawgie-1.4.3rc3/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2024-04-30 17:23:47.000000 dawgie-1.4.3rc3/LICENSE
+-rw-r--r--   0 niessner  (1000) niessner  (1000)     9940 2024-04-30 17:23:48.070226 dawgie-1.4.3rc3/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2024-04-30 17:23:47.000000 dawgie-1.4.3rc3/README.md
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2024-04-30 17:23:48.066226 dawgie-1.4.3rc3/dawgie.egg-info/
+-rw-r--r--   0 niessner  (1000) niessner  (1000)     9940 2024-04-30 17:23:48.000000 dawgie-1.4.3rc3/dawgie.egg-info/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6632 2024-04-30 17:23:48.000000 dawgie-1.4.3rc3/dawgie.egg-info/SOURCES.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2024-04-30 17:23:48.000000 dawgie-1.4.3rc3/dawgie.egg-info/dependency_links.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      245 2024-04-30 17:23:48.000000 dawgie-1.4.3rc3/dawgie.egg-info/requires.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2024-04-30 17:23:48.000000 dawgie-1.4.3rc3/dawgie.egg-info/top_level.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2024-04-30 17:23:48.070226 dawgie-1.4.3rc3/setup.cfg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6410 2024-04-30 17:17:50.000000 dawgie-1.4.3rc3/setup.py
```

### Comparing `dawgie-1.4.3rc2/LICENSE` & `dawgie-1.4.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.3rc2/PKG-INFO` & `dawgie-1.4.3rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.3rc2
+Version: 1.4.3rc3
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dawgie-1.4.3rc2/README.md` & `dawgie-1.4.3rc3/README.md`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.3rc2/dawgie.egg-info/PKG-INFO` & `dawgie-1.4.3rc3/dawgie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.3rc2
+Version: 1.4.3rc3
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dawgie-1.4.3rc2/setup.py` & `dawgie-1.4.3rc3/setup.py`

 * *Files identical despite different names*

