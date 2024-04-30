# Comparing `tmp/icepap-3.8.1.tar.gz` & `tmp/icepap-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icepap-3.8.1.tar", last modified: Fri Nov  3 12:16:23 2023, max compression
+gzip compressed data, was "icepap-3.9.0.tar", last modified: Wed Jan 17 08:13:41 2024, max compression
```

## Comparing `icepap-3.8.1.tar` & `icepap-3.9.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-11-03 12:16:23.391708 icepap-3.8.1/
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     8234 2023-11-03 12:15:30.000000 icepap-3.8.1/CHANGELOG.md
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    35149 2019-07-24 09:07:48.000000 icepap-3.8.1/LICENSE.txt
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      331 2019-07-24 09:07:48.000000 icepap-3.8.1/MANIFEST.in
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      820 2023-11-03 12:16:23.391708 icepap-3.8.1/PKG-INFO
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1292 2023-01-17 18:42:24.000000 icepap-3.8.1/README.md
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-11-03 12:16:23.379708 icepap-3.8.1/doc/
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-11-03 12:16:23.383708 icepap-3.8.1/doc/source/
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-11-03 12:16:23.383708 icepap-3.8.1/doc/source/_static/
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    43840 2019-07-24 09:07:48.000000 icepap-3.8.1/doc/source/_static/ALBALogo_WHITE.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)   270686 2019-07-24 09:07:48.000000 icepap-3.8.1/doc/source/_static/IcePAP_3D.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      249 2023-01-17 18:42:24.000000 icepap-3.8.1/doc/source/api.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      257 2023-01-17 18:42:24.000000 icepap-3.8.1/doc/source/applications.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      201 2023-01-17 18:42:24.000000 icepap-3.8.1/doc/source/axis.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      201 2023-01-17 18:42:24.000000 icepap-3.8.1/doc/source/backups.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      240 2023-01-17 18:42:24.000000 icepap-3.8.1/doc/source/communication.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     8661 2023-01-17 18:42:24.000000 icepap-3.8.1/doc/source/conf.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      231 2023-01-17 18:42:24.000000 icepap-3.8.1/doc/source/controller.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      212 2023-01-17 18:42:24.000000 icepap-3.8.1/doc/source/fwversion.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      634 2023-01-17 18:42:24.000000 icepap-3.8.1/doc/source/index.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      223 2019-07-24 09:07:48.000000 icepap-3.8.1/doc/source/low_level_methods.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      321 2023-01-17 18:42:24.000000 icepap-3.8.1/doc/source/programming.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      197 2023-01-17 18:42:24.000000 icepap-3.8.1/doc/source/utils.rst
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-11-03 12:16:23.387708 icepap-3.8.1/icepap/
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      898 2023-11-03 12:15:54.000000 icepap-3.8.1/icepap/__init__.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    48178 2023-11-03 12:14:13.000000 icepap-3.8.1/icepap/axis.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-11-03 12:16:23.391708 icepap-3.8.1/icepap/cli/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2023-01-17 18:42:24.000000 icepap-3.8.1/icepap/cli/__init__.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      698 2023-01-17 18:42:24.000000 icepap-3.8.1/icepap/cli/__main__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     9843 2023-03-16 16:30:32.000000 icepap-3.8.1/icepap/cli/cli.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    11305 2023-01-17 18:42:24.000000 icepap-3.8.1/icepap/cli/progress_bar.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     8332 2023-03-02 11:10:19.000000 icepap-3.8.1/icepap/cli/repl.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     6700 2023-01-17 18:42:24.000000 icepap-3.8.1/icepap/cli/tables.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      565 2023-01-17 18:42:24.000000 icepap-3.8.1/icepap/cli/utils.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     5389 2023-03-16 16:30:32.000000 icepap-3.8.1/icepap/communication.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    24083 2023-03-16 16:30:32.000000 icepap-3.8.1/icepap/controller.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     9892 2023-01-17 18:42:24.000000 icepap-3.8.1/icepap/fwversion.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     5219 2023-01-17 18:42:24.000000 icepap-3.8.1/icepap/group.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     8743 2023-01-17 18:42:24.000000 icepap-3.8.1/icepap/tcp.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    17403 2023-01-17 18:42:24.000000 icepap-3.8.1/icepap/utils.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     7130 2023-01-17 18:42:24.000000 icepap-3.8.1/icepap/vdatalib.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-11-03 12:16:23.387708 icepap-3.8.1/icepap.egg-info/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      820 2023-11-03 12:16:23.000000 icepap-3.8.1/icepap.egg-info/PKG-INFO
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      973 2023-11-03 12:16:23.000000 icepap-3.8.1/icepap.egg-info/SOURCES.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        1 2023-11-03 12:16:23.000000 icepap-3.8.1/icepap.egg-info/dependency_links.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       49 2023-11-03 12:16:23.000000 icepap-3.8.1/icepap.egg-info/entry_points.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      114 2023-11-03 12:16:23.000000 icepap-3.8.1/icepap.egg-info/requires.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        7 2023-11-03 12:16:23.000000 icepap-3.8.1/icepap.egg-info/top_level.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       38 2023-11-03 12:16:23.391708 icepap-3.8.1/setup.cfg
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     2116 2023-11-03 12:15:54.000000 icepap-3.8.1/setup.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-11-03 12:16:23.391708 icepap-3.8.1/tests/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1601 2023-01-17 18:42:24.000000 icepap-3.8.1/tests/test_cli.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1212 2023-01-17 18:42:24.000000 icepap-3.8.1/tests/test_group.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     9701 2023-01-17 18:42:24.000000 icepap-3.8.1/tests/test_icepap.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2024-01-17 08:13:41.964429 icepap-3.9.0/
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     8347 2024-01-17 08:05:22.000000 icepap-3.9.0/CHANGELOG.md
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    35149 2019-07-24 09:07:48.000000 icepap-3.9.0/LICENSE.txt
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      331 2019-07-24 09:07:48.000000 icepap-3.9.0/MANIFEST.in
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1053 2024-01-17 08:13:41.964429 icepap-3.9.0/PKG-INFO
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1292 2023-01-17 18:42:24.000000 icepap-3.9.0/README.md
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2024-01-17 08:13:41.956428 icepap-3.9.0/doc/
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2024-01-17 08:13:41.956428 icepap-3.9.0/doc/source/
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2024-01-17 08:13:41.960428 icepap-3.9.0/doc/source/_static/
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    43840 2019-07-24 09:07:48.000000 icepap-3.9.0/doc/source/_static/ALBALogo_WHITE.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)   270686 2019-07-24 09:07:48.000000 icepap-3.9.0/doc/source/_static/IcePAP_3D.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      249 2023-01-17 18:42:24.000000 icepap-3.9.0/doc/source/api.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      257 2023-01-17 18:42:24.000000 icepap-3.9.0/doc/source/applications.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      201 2023-01-17 18:42:24.000000 icepap-3.9.0/doc/source/axis.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      201 2023-01-17 18:42:24.000000 icepap-3.9.0/doc/source/backups.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      240 2023-01-17 18:42:24.000000 icepap-3.9.0/doc/source/communication.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     8661 2023-01-17 18:42:24.000000 icepap-3.9.0/doc/source/conf.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      231 2023-01-17 18:42:24.000000 icepap-3.9.0/doc/source/controller.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      212 2023-01-17 18:42:24.000000 icepap-3.9.0/doc/source/fwversion.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      634 2023-01-17 18:42:24.000000 icepap-3.9.0/doc/source/index.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      223 2019-07-24 09:07:48.000000 icepap-3.9.0/doc/source/low_level_methods.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      321 2023-01-17 18:42:24.000000 icepap-3.9.0/doc/source/programming.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      197 2023-01-17 18:42:24.000000 icepap-3.9.0/doc/source/utils.rst
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2024-01-17 08:13:41.960428 icepap-3.9.0/icepap/
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      898 2024-01-17 08:05:22.000000 icepap-3.9.0/icepap/__init__.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    48178 2023-11-07 08:12:49.000000 icepap-3.9.0/icepap/axis.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2024-01-17 08:13:41.964429 icepap-3.9.0/icepap/cli/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2023-11-07 08:12:49.000000 icepap-3.9.0/icepap/cli/__init__.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      698 2023-11-07 08:12:49.000000 icepap-3.9.0/icepap/cli/__main__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     9843 2023-11-07 08:12:49.000000 icepap-3.9.0/icepap/cli/cli.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    11305 2023-11-07 08:12:49.000000 icepap-3.9.0/icepap/cli/progress_bar.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     8332 2023-11-07 08:12:49.000000 icepap-3.9.0/icepap/cli/repl.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     6700 2023-11-07 08:12:49.000000 icepap-3.9.0/icepap/cli/tables.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      565 2023-11-07 08:12:49.000000 icepap-3.9.0/icepap/cli/utils.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     5389 2023-11-07 08:14:03.000000 icepap-3.9.0/icepap/communication.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    24470 2024-01-17 08:05:22.000000 icepap-3.9.0/icepap/controller.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     9892 2023-01-17 18:42:24.000000 icepap-3.9.0/icepap/fwversion.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     5219 2023-11-07 08:14:03.000000 icepap-3.9.0/icepap/group.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     8743 2023-11-07 08:14:05.000000 icepap-3.9.0/icepap/tcp.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    17403 2023-11-07 08:12:49.000000 icepap-3.9.0/icepap/utils.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     7130 2023-01-17 18:42:24.000000 icepap-3.9.0/icepap/vdatalib.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2024-01-17 08:13:41.964429 icepap-3.9.0/icepap.egg-info/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1053 2024-01-17 08:13:41.000000 icepap-3.9.0/icepap.egg-info/PKG-INFO
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      973 2024-01-17 08:13:41.000000 icepap-3.9.0/icepap.egg-info/SOURCES.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        1 2024-01-17 08:13:41.000000 icepap-3.9.0/icepap.egg-info/dependency_links.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       49 2024-01-17 08:13:41.000000 icepap-3.9.0/icepap.egg-info/entry_points.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      114 2024-01-17 08:13:41.000000 icepap-3.9.0/icepap.egg-info/requires.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        7 2024-01-17 08:13:41.000000 icepap-3.9.0/icepap.egg-info/top_level.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       38 2024-01-17 08:13:41.964429 icepap-3.9.0/setup.cfg
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     2116 2024-01-17 08:05:22.000000 icepap-3.9.0/setup.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2024-01-17 08:13:41.964429 icepap-3.9.0/tests/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1601 2023-01-17 18:42:24.000000 icepap-3.9.0/tests/test_cli.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1212 2023-01-17 18:42:24.000000 icepap-3.9.0/tests/test_group.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     9701 2023-01-17 18:42:24.000000 icepap-3.9.0/tests/test_icepap.py
```

### Comparing `icepap-3.8.1/CHANGELOG.md` & `icepap-3.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [3.9.x]
+### Added
+    - Add method for getting linked axes at IcePAPController class
+
+### Removed
+
+### Fixed
+
 ## [3.8.x] 
 ### Added
     - Add axis list track command
 
 ### Removed
 
 ### Fixed
```

### Comparing `icepap-3.8.1/LICENSE.txt` & `icepap-3.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/README.md` & `icepap-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/doc/source/_static/ALBALogo_WHITE.png` & `icepap-3.9.0/doc/source/_static/ALBALogo_WHITE.png`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/doc/source/_static/IcePAP_3D.png` & `icepap-3.9.0/doc/source/_static/IcePAP_3D.png`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/doc/source/conf.py` & `icepap-3.9.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/doc/source/index.rst` & `icepap-3.9.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap/__init__.py` & `icepap-3.9.0/icepap/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 from .communication import IcePAPCommunication
 from .controller import IcePAPController
 from .fwversion import *
 from .utils import *
 
 # The version is updated automatically with bumpversion
 # Do not update manually
-version = '3.8.1'
+version = '3.9.0'
```

### Comparing `icepap-3.8.1/icepap/axis.py` & `icepap-3.9.0/icepap/axis.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap/cli/__main__.py` & `icepap-3.9.0/icepap/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap/cli/cli.py` & `icepap-3.9.0/icepap/cli/cli.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap/cli/progress_bar.py` & `icepap-3.9.0/icepap/cli/progress_bar.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap/cli/repl.py` & `icepap-3.9.0/icepap/cli/repl.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap/cli/tables.py` & `icepap-3.9.0/icepap/cli/tables.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap/cli/utils.py` & `icepap-3.9.0/icepap/cli/utils.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap/communication.py` & `icepap-3.9.0/icepap/communication.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap/controller.py` & `icepap-3.9.0/icepap/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -712,14 +712,26 @@
         Returns a list of the current signals sources used as axis indexers
         (IcePAP user manual, page 107).
 
         :return: list of multiplexer configurations.
         """
         return self.send_cmd('?PMUX')
 
+    def get_linked(self):
+        """
+        Returns the current list of groups of linked drivers. 
+        Each group is returned in a separate line starting by the name 
+        of the group and followed by the corresponding list of axes.
+
+        (IcePAP user manual, page 80).
+
+        :return: list of groups of linked drivers.
+        """
+        return self.send_cmd('?LINKED')
+
     def sprog(self, filename, component=None, force=False, saving=False,
               options=''):
         """
         Firmware programming command. This command assumes that the firmware
         code will be transferred as a binary data block (IcePAP user manual,
         page 112).
         :param filename: firmware filename
```

### Comparing `icepap-3.8.1/icepap/fwversion.py` & `icepap-3.9.0/icepap/fwversion.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap/group.py` & `icepap-3.9.0/icepap/group.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap/tcp.py` & `icepap-3.9.0/icepap/tcp.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap/utils.py` & `icepap-3.9.0/icepap/utils.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap/vdatalib.py` & `icepap-3.9.0/icepap/vdatalib.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/icepap.egg-info/SOURCES.txt` & `icepap-3.9.0/icepap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/setup.py` & `icepap-3.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # setup.py
 import sys
 from setuptools import setup
 from setuptools import find_packages
 
 # The version is updated automatically with bumpversion
 # Do not update manually
-__version = '3.8.1'
+__version = '3.9.0'
 
 # windows installer:
 # python setup.py bdist_wininst
 
 # patch distutils if it can't cope with the "classifiers" or
 # "download_url" keywords
```

### Comparing `icepap-3.8.1/tests/test_cli.py` & `icepap-3.9.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/tests/test_group.py` & `icepap-3.9.0/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `icepap-3.8.1/tests/test_icepap.py` & `icepap-3.9.0/tests/test_icepap.py`

 * *Files identical despite different names*

