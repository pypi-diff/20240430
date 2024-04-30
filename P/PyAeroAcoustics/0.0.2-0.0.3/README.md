# Comparing `tmp/PyAeroAcoustics-0.0.2.tar.gz` & `tmp/PyAeroAcoustics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAeroAcoustics-0.0.2.tar", last modified: Mon Apr 29 15:33:16 2024, max compression
+gzip compressed data, was "PyAeroAcoustics-0.0.3.tar", last modified: Mon Apr 29 15:45:14 2024, max compression
```

## Comparing `PyAeroAcoustics-0.0.2.tar` & `PyAeroAcoustics-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-29 15:33:16.250267 PyAeroAcoustics-0.0.2/
--rw-r--r--   0 brunnerth (76394) p71694   (71694)      549 2024-04-29 15:33:16.249552 PyAeroAcoustics-0.0.2/PKG-INFO
-drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-29 15:33:16.244797 PyAeroAcoustics-0.0.2/PyAeroAcoustics/
-drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-29 15:33:16.248700 PyAeroAcoustics-0.0.2/PyAeroAcoustics/Spectrum/
--rw-r--r--   0 brunnerth (76394) p71694   (71694)     2395 2024-04-29 15:31:09.000000 PyAeroAcoustics-0.0.2/PyAeroAcoustics/Spectrum/Spectrum.py
--rw-r--r--   0 brunnerth (76394) p71694   (71694)       29 2024-04-29 15:14:45.000000 PyAeroAcoustics-0.0.2/PyAeroAcoustics/Spectrum/__init__.py
--rw-r--r--   0 brunnerth (76394) p71694   (71694)       38 2024-04-29 15:30:55.000000 PyAeroAcoustics-0.0.2/PyAeroAcoustics/__init__.py
-drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-29 15:33:16.247628 PyAeroAcoustics-0.0.2/PyAeroAcoustics.egg-info/
--rw-r--r--   0 brunnerth (76394) p71694   (71694)      549 2024-04-29 15:33:16.245602 PyAeroAcoustics-0.0.2/PyAeroAcoustics.egg-info/PKG-INFO
--rw-r--r--   0 brunnerth (76394) p71694   (71694)      266 2024-04-29 15:33:16.246344 PyAeroAcoustics-0.0.2/PyAeroAcoustics.egg-info/SOURCES.txt
--rw-r--r--   0 brunnerth (76394) p71694   (71694)        1 2024-04-29 15:33:16.247111 PyAeroAcoustics-0.0.2/PyAeroAcoustics.egg-info/dependency_links.txt
--rw-r--r--   0 brunnerth (76394) p71694   (71694)       16 2024-04-29 15:33:16.247703 PyAeroAcoustics-0.0.2/PyAeroAcoustics.egg-info/top_level.txt
--rw-r--r--   0 brunnerth (76394) p71694   (71694)       38 2024-04-29 15:33:16.250350 PyAeroAcoustics-0.0.2/setup.cfg
--rw-r--r--   0 brunnerth (76394) p71694   (71694)      920 2024-04-29 15:33:11.000000 PyAeroAcoustics-0.0.2/setup.py
+drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-29 15:45:14.475635 PyAeroAcoustics-0.0.3/
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)      549 2024-04-29 15:45:14.474944 PyAeroAcoustics-0.0.3/PKG-INFO
+drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-29 15:45:14.470311 PyAeroAcoustics-0.0.3/PyAeroAcoustics/
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)       30 2024-04-29 15:44:32.000000 PyAeroAcoustics-0.0.3/PyAeroAcoustics/PyAeroAcoustics.py
+drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-29 15:45:14.474305 PyAeroAcoustics-0.0.3/PyAeroAcoustics/Spectrum/
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)     2395 2024-04-29 15:31:09.000000 PyAeroAcoustics-0.0.3/PyAeroAcoustics/Spectrum/Spectrum.py
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)       22 2024-04-29 15:44:17.000000 PyAeroAcoustics-0.0.3/PyAeroAcoustics/Spectrum/__init__.py
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)       22 2024-04-29 15:44:44.000000 PyAeroAcoustics-0.0.3/PyAeroAcoustics/__init__.py
+drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-29 15:45:14.473257 PyAeroAcoustics-0.0.3/PyAeroAcoustics.egg-info/
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)      549 2024-04-29 15:45:14.471179 PyAeroAcoustics-0.0.3/PyAeroAcoustics.egg-info/PKG-INFO
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)      301 2024-04-29 15:45:14.472225 PyAeroAcoustics-0.0.3/PyAeroAcoustics.egg-info/SOURCES.txt
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)        1 2024-04-29 15:45:14.472980 PyAeroAcoustics-0.0.3/PyAeroAcoustics.egg-info/dependency_links.txt
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)       16 2024-04-29 15:45:14.473342 PyAeroAcoustics-0.0.3/PyAeroAcoustics.egg-info/top_level.txt
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)       38 2024-04-29 15:45:14.475744 PyAeroAcoustics-0.0.3/setup.cfg
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)      920 2024-04-29 15:45:07.000000 PyAeroAcoustics-0.0.3/setup.py
```

### Comparing `PyAeroAcoustics-0.0.2/PKG-INFO` & `PyAeroAcoustics-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PyAeroAcoustics
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyAeroAcoustics
 Home-page: UNKNOWN
 Author: Thomas Brunner
 Author-email: <thomas.brunner@tugraz.at>
 License: UNKNOWN
 Description: PyAeroAcoustics
 Keywords: python,PyAeroAcoustics
```

### Comparing `PyAeroAcoustics-0.0.2/PyAeroAcoustics/Spectrum/Spectrum.py` & `PyAeroAcoustics-0.0.3/PyAeroAcoustics/Spectrum/Spectrum.py`

 * *Files identical despite different names*

### Comparing `PyAeroAcoustics-0.0.2/PyAeroAcoustics.egg-info/PKG-INFO` & `PyAeroAcoustics-0.0.3/PyAeroAcoustics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PyAeroAcoustics
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyAeroAcoustics
 Home-page: UNKNOWN
 Author: Thomas Brunner
 Author-email: <thomas.brunner@tugraz.at>
 License: UNKNOWN
 Description: PyAeroAcoustics
 Keywords: python,PyAeroAcoustics
```

### Comparing `PyAeroAcoustics-0.0.2/setup.py` & `PyAeroAcoustics-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'PyAeroAcoustics'
 LONG_DESCRIPTION = 'PyAeroAcoustics'
 
 setup(
         name="PyAeroAcoustics", 
         version=VERSION,
         author="Thomas Brunner",
```

