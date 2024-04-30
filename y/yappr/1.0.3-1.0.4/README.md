# Comparing `tmp/yappr-1.0.3.tar.gz` & `tmp/yappr-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yappr-1.0.3.tar", last modified: Sun Apr 28 04:28:45 2024, max compression
+gzip compressed data, was "yappr-1.0.4.tar", last modified: Tue Apr 30 16:16:24 2024, max compression
```

## Comparing `yappr-1.0.3.tar` & `yappr-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:28:45.904341 yappr-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-28 04:28:39.000000 yappr-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-28 04:28:39.000000 yappr-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-28 04:28:45.904341 yappr-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-28 04:28:39.000000 yappr-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-28 04:28:39.000000 yappr-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 04:28:45.904341 yappr-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:28:45.900341 yappr-1.0.3/yappr/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-28 04:28:39.000000 yappr-1.0.3/yappr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-28 04:28:39.000000 yappr-1.0.3/yappr/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-28 04:28:39.000000 yappr-1.0.3/yappr/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:28:39.000000 yappr-1.0.3/yappr/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-28 04:28:39.000000 yappr-1.0.3/yappr/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:28:45.900341 yappr-1.0.3/yappr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-28 04:28:45.000000 yappr-1.0.3/yappr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-28 04:28:45.000000 yappr-1.0.3/yappr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 04:28:45.000000 yappr-1.0.3/yappr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 04:28:45.000000 yappr-1.0.3/yappr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:16:24.721383 yappr-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-30 16:16:20.000000 yappr-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-30 16:16:20.000000 yappr-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-30 16:16:24.721383 yappr-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-30 16:16:20.000000 yappr-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-30 16:16:20.000000 yappr-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 16:16:24.721383 yappr-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:16:24.721383 yappr-1.0.4/yappr/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 16:16:20.000000 yappr-1.0.4/yappr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-30 16:16:20.000000 yappr-1.0.4/yappr/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-30 16:16:20.000000 yappr-1.0.4/yappr/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:16:20.000000 yappr-1.0.4/yappr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-30 16:16:20.000000 yappr-1.0.4/yappr/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:16:24.721383 yappr-1.0.4/yappr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-30 16:16:24.000000 yappr-1.0.4/yappr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 16:16:24.000000 yappr-1.0.4/yappr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:16:24.000000 yappr-1.0.4/yappr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 16:16:24.000000 yappr-1.0.4/yappr.egg-info/top_level.txt
```

### Comparing `yappr-1.0.3/LICENSE` & `yappr-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yappr-1.0.3/PKG-INFO` & `yappr-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yappr
-Version: 1.0.3
+Version: 1.0.4
 Summary: Yet another python package updater
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `yappr-1.0.3/README.md` & `yappr-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `yappr-1.0.3/pyproject.toml` & `yappr-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yappr"
-version = "1.0.3"
+version = "1.0.4"
 dependencies = []
 requires-python = ">=3"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Yet another python package updater"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
```

### Comparing `yappr-1.0.3/yappr/decorator.py` & `yappr-1.0.4/yappr/decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import sys
 import tkinter as tk
 import traceback
 from argparse import ArgumentParser
+from pathlib import Path
 from threading import Thread
 from tkinter.messagebox import showerror  # type: ignore
 from typing import Any
 from typing import Callable
 from typing import ParamSpec
 
 from yappr import logger
@@ -43,15 +44,16 @@
                     logger.info("Gracefully shutting down...")
 
                     # If exit flag was set by user, stop the script
                     if not updater.new_update_flag.is_set():
                         return
 
                     # if exit flag was set by updater
-                    os.execl(sys.executable, sys.executable, *sys.argv)
+                    p = Path(sys.executable)
+                    os.execl(p, p.stem, *sys.argv)
                 except Exception:
                     logger.exception("Unhandled Exception")
                     root = tk.Tk()
                     root.withdraw()
                     root.after(30000, root.destroy)
                     out = showerror(
                         "Unhandled Exception",
```

### Comparing `yappr-1.0.3/yappr/logger.py` & `yappr-1.0.4/yappr/logger.py`

 * *Files identical despite different names*

### Comparing `yappr-1.0.3/yappr/updater.py` & `yappr-1.0.4/yappr/updater.py`

 * *Files identical despite different names*

### Comparing `yappr-1.0.3/yappr.egg-info/PKG-INFO` & `yappr-1.0.4/yappr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yappr
-Version: 1.0.3
+Version: 1.0.4
 Summary: Yet another python package updater
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

