# Comparing `tmp/scitbx-0.0.8.tar.gz` & `tmp/scitbx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\scitbx-0.0.8.tar", last modified: Wed Feb 17 10:44:35 2021, max compression
+gzip compressed data, was "dist\scitbx-0.0.9.tar", last modified: Wed Feb 17 12:25:39 2021, max compression
```

## Comparing `scitbx-0.0.8.tar` & `scitbx-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2021-02-17 10:44:35.000000 scitbx-0.0.8/
--rw-rw-rw-   0        0        0      307 2021-02-17 10:44:35.000000 scitbx-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2020-06-01 08:22:10.000000 scitbx-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-02-17 10:44:35.000000 scitbx-0.0.8/scitbx/
--rw-rw-rw-   0        0        0      449 2021-02-17 10:43:39.000000 scitbx-0.0.8/scitbx/__init__.py
--rw-rw-rw-   0        0        0      192 2020-07-04 07:44:47.000000 scitbx-0.0.8/scitbx/load_google_drive.py
--rw-rw-rw-   0        0        0     2260 2020-07-04 21:40:29.000000 scitbx-0.0.8/scitbx/manage_file.py
--rw-rw-rw-   0        0        0     2230 2020-07-04 07:47:22.000000 scitbx-0.0.8/scitbx/manage_time.py
--rw-rw-rw-   0        0        0      569 2020-06-26 13:31:36.000000 scitbx-0.0.8/scitbx/manage_yaml.py
--rw-rw-rw-   0        0        0      239 2021-02-07 13:53:48.000000 scitbx-0.0.8/scitbx/pickle_wrapper.py
--rw-rw-rw-   0        0        0     2890 2020-06-01 10:01:30.000000 scitbx-0.0.8/scitbx/scientific_plot.py
--rw-rw-rw-   0        0        0      169 2021-02-17 10:43:22.000000 scitbx-0.0.8/scitbx/utils.py
-drwxrwxrwx   0        0        0        0 2021-02-17 10:44:35.000000 scitbx-0.0.8/scitbx.egg-info/
--rw-rw-rw-   0        0        0      307 2021-02-17 10:44:35.000000 scitbx-0.0.8/scitbx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2021-02-17 10:44:35.000000 scitbx-0.0.8/scitbx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-17 10:44:35.000000 scitbx-0.0.8/scitbx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2021-02-17 10:44:35.000000 scitbx-0.0.8/scitbx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-02-17 10:44:35.000000 scitbx-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      743 2021-02-17 10:44:25.000000 scitbx-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-02-17 12:25:39.000000 scitbx-0.0.9/
+-rw-rw-rw-   0        0        0      307 2021-02-17 12:25:39.000000 scitbx-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2020-06-01 08:22:10.000000 scitbx-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2021-02-17 12:25:39.000000 scitbx-0.0.9/scitbx/
+-rw-rw-rw-   0        0        0      442 2021-02-17 12:25:10.000000 scitbx-0.0.9/scitbx/__init__.py
+-rw-rw-rw-   0        0        0      192 2020-07-04 07:44:47.000000 scitbx-0.0.9/scitbx/load_google_drive.py
+-rw-rw-rw-   0        0        0     2260 2020-07-04 21:40:29.000000 scitbx-0.0.9/scitbx/manage_file.py
+-rw-rw-rw-   0        0        0     2230 2020-07-04 07:47:22.000000 scitbx-0.0.9/scitbx/manage_time.py
+-rw-rw-rw-   0        0        0      569 2020-06-26 13:31:36.000000 scitbx-0.0.9/scitbx/manage_yaml.py
+-rw-rw-rw-   0        0        0      239 2021-02-07 13:53:48.000000 scitbx-0.0.9/scitbx/pickle_wrapper.py
+-rw-rw-rw-   0        0        0     2890 2020-06-01 10:01:30.000000 scitbx-0.0.9/scitbx/scientific_plot.py
+-rw-rw-rw-   0        0        0      169 2021-02-17 10:43:22.000000 scitbx-0.0.9/scitbx/utils.py
+drwxrwxrwx   0        0        0        0 2021-02-17 12:25:39.000000 scitbx-0.0.9/scitbx.egg-info/
+-rw-rw-rw-   0        0        0      307 2021-02-17 12:25:39.000000 scitbx-0.0.9/scitbx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2021-02-17 12:25:39.000000 scitbx-0.0.9/scitbx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-02-17 12:25:39.000000 scitbx-0.0.9/scitbx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2021-02-17 12:25:39.000000 scitbx-0.0.9/scitbx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-02-17 12:25:39.000000 scitbx-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      743 2021-02-17 12:25:23.000000 scitbx-0.0.9/setup.py
```

### Comparing `scitbx-0.0.8/scitbx/manage_file.py` & `scitbx-0.0.9/scitbx/manage_file.py`

 * *Files identical despite different names*

### Comparing `scitbx-0.0.8/scitbx/manage_time.py` & `scitbx-0.0.9/scitbx/manage_time.py`

 * *Files identical despite different names*

### Comparing `scitbx-0.0.8/scitbx/manage_yaml.py` & `scitbx-0.0.9/scitbx/manage_yaml.py`

 * *Files identical despite different names*

### Comparing `scitbx-0.0.8/scitbx/scientific_plot.py` & `scitbx-0.0.9/scitbx/scientific_plot.py`

 * *Files identical despite different names*

### Comparing `scitbx-0.0.8/setup.py` & `scitbx-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
 	name = "scitbx",
-	version = "0.0.8",
+	version = "0.0.9",
 	keywords = ("atmos/geo science assitance"),
 	description = "draw and basic calculations/conversions",
 	long_description = "coming soon",
 	license = "MIT Licence",
 
 	url="https://github.com/soonyenju/scitbx",
 	author = "Songyan Zhu",
```

