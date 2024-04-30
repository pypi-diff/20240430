# Comparing `tmp/XenAPI-24.4.0.tar.gz` & `tmp/XenAPI-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XenAPI-24.4.0.tar", last modified: Tue Jan 30 13:55:11 2024, max compression
+gzip compressed data, was "XenAPI-24.5.0.tar", last modified: Mon Feb 12 14:04:45 2024, max compression
```

## Comparing `XenAPI-24.4.0.tar` & `XenAPI-24.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:55:11.133893 XenAPI-24.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-30 13:54:40.000000 XenAPI-24.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-30 13:55:11.133893 XenAPI-24.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-01-30 13:54:40.000000 XenAPI-24.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:55:11.129893 XenAPI-24.4.0/XenAPI/
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-01-30 13:54:40.000000 XenAPI-24.4.0/XenAPI/XenAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-30 13:54:40.000000 XenAPI-24.4.0/XenAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 13:55:11.129893 XenAPI-24.4.0/XenAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-30 13:55:10.000000 XenAPI-24.4.0/XenAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-01-30 13:55:11.000000 XenAPI-24.4.0/XenAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 13:55:10.000000 XenAPI-24.4.0/XenAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-30 13:55:10.000000 XenAPI-24.4.0/XenAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-01-30 13:54:40.000000 XenAPI-24.4.0/XenAPIPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-30 13:54:40.000000 XenAPI-24.4.0/echo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5771 2024-01-30 13:54:40.000000 XenAPI-24.4.0/exportimport.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-30 13:54:40.000000 XenAPI-24.4.0/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-30 13:54:40.000000 XenAPI-24.4.0/lvhd-api-test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-01-30 13:54:40.000000 XenAPI-24.4.0/mini-xenrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-01-30 13:54:40.000000 XenAPI-24.4.0/monitor-unwanted-domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-01-30 13:54:40.000000 XenAPI-24.4.0/provision.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-30 13:54:40.000000 XenAPI-24.4.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     6377 2024-01-30 13:54:40.000000 XenAPI-24.4.0/renameif.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-30 13:55:11.133893 XenAPI-24.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-01-30 13:54:40.000000 XenAPI-24.4.0/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:04:45.419432 XenAPI-24.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-12 14:04:14.000000 XenAPI-24.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-02-12 14:04:45.419432 XenAPI-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-02-12 14:04:14.000000 XenAPI-24.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:04:45.415432 XenAPI-24.5.0/XenAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-02-12 14:04:14.000000 XenAPI-24.5.0/XenAPI/XenAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 14:04:14.000000 XenAPI-24.5.0/XenAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:04:45.419432 XenAPI-24.5.0/XenAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-02-12 14:04:44.000000 XenAPI-24.5.0/XenAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-12 14:04:45.000000 XenAPI-24.5.0/XenAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 14:04:44.000000 XenAPI-24.5.0/XenAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-12 14:04:44.000000 XenAPI-24.5.0/XenAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-02-12 14:04:14.000000 XenAPI-24.5.0/XenAPIPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-12 14:04:14.000000 XenAPI-24.5.0/echo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5771 2024-02-12 14:04:14.000000 XenAPI-24.5.0/exportimport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-12 14:04:14.000000 XenAPI-24.5.0/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-12 14:04:14.000000 XenAPI-24.5.0/lvhd-api-test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-02-12 14:04:14.000000 XenAPI-24.5.0/mini-xenrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-02-12 14:04:14.000000 XenAPI-24.5.0/monitor-unwanted-domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-02-12 14:04:14.000000 XenAPI-24.5.0/provision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-12 14:04:14.000000 XenAPI-24.5.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6377 2024-02-12 14:04:14.000000 XenAPI-24.5.0/renameif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-02-12 14:04:45.419432 XenAPI-24.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-02-12 14:04:14.000000 XenAPI-24.5.0/shell.py
```

### Comparing `XenAPI-24.4.0/PKG-INFO` & `XenAPI-24.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XenAPI
-Version: 24.4.0
+Version: 24.5.0
 Summary: XenAPI SDK, for communication with XenServer.
 Home-page: https://xapi-project.github.io/
 Author: Xapi project developers and maintainers
 Author-email: xen-api@lists.xenproject.org
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/xapi-project/xen-api/issues
 Project-URL: Source Code, https://github.com/xapi-project/xen-api
```

### Comparing `XenAPI-24.4.0/README.md` & `XenAPI-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `XenAPI-24.4.0/XenAPI/XenAPI.py` & `XenAPI-24.5.0/XenAPI/XenAPI.py`

 * *Files identical despite different names*

### Comparing `XenAPI-24.4.0/XenAPI.egg-info/PKG-INFO` & `XenAPI-24.5.0/XenAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XenAPI
-Version: 24.4.0
+Version: 24.5.0
 Summary: XenAPI SDK, for communication with XenServer.
 Home-page: https://xapi-project.github.io/
 Author: Xapi project developers and maintainers
 Author-email: xen-api@lists.xenproject.org
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/xapi-project/xen-api/issues
 Project-URL: Source Code, https://github.com/xapi-project/xen-api
```

### Comparing `XenAPI-24.4.0/XenAPIPlugin.py` & `XenAPI-24.5.0/XenAPIPlugin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-#!/usr/bin/python3
+"""XenAPI python plugin boilerplate code"""
+# pylint: disable=invalid-name
+# Module name "XenAPIPlugin" doesn't conform to snake_case naming style
+# For usage, see: https://wiki.xenproject.org/wiki/XAPI_Host_Plugins
 
-# XenAPI python plugin boilerplate code
 
 from __future__ import print_function
 
 import sys
 
 import XenAPI
```

### Comparing `XenAPI-24.4.0/exportimport.py` & `XenAPI-24.5.0/exportimport.py`

 * *Files identical despite different names*

### Comparing `XenAPI-24.4.0/inventory.py` & `XenAPI-24.5.0/inventory.py`

 * *Files identical despite different names*

### Comparing `XenAPI-24.4.0/lvhd-api-test.py` & `XenAPI-24.5.0/lvhd-api-test.py`

 * *Files identical despite different names*

### Comparing `XenAPI-24.4.0/mini-xenrt.py` & `XenAPI-24.5.0/mini-xenrt.py`

 * *Files identical despite different names*

### Comparing `XenAPI-24.4.0/monitor-unwanted-domains.py` & `XenAPI-24.5.0/monitor-unwanted-domains.py`

 * *Files identical despite different names*

### Comparing `XenAPI-24.4.0/provision.py` & `XenAPI-24.5.0/provision.py`

 * *Files identical despite different names*

### Comparing `XenAPI-24.4.0/renameif.py` & `XenAPI-24.5.0/renameif.py`

 * *Files identical despite different names*

### Comparing `XenAPI-24.4.0/setup.cfg` & `XenAPI-24.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `XenAPI-24.4.0/shell.py` & `XenAPI-24.5.0/shell.py`

 * *Files identical despite different names*

