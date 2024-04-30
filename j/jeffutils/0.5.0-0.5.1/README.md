# Comparing `tmp/jeffutils-0.5.0.tar.gz` & `tmp/jeffutils-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.5.0.tar", last modified: Tue Apr 23 20:51:17 2024, max compression
+gzip compressed data, was "jeffutils-0.5.1.tar", last modified: Tue Apr 30 20:42:19 2024, max compression
```

## Comparing `jeffutils-0.5.0.tar` & `jeffutils-0.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-23 20:51:17.689698 jeffutils-0.5.0/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.0/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-23 20:51:17.689698 jeffutils-0.5.0/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.0/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.0/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-04-23 20:51:17.689698 jeffutils-0.5.0/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-04-23 20:51:12.000000 jeffutils-0.5.0/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-23 20:51:17.689698 jeffutils-0.5.0/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-23 20:51:17.689698 jeffutils-0.5.0/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.0/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    16230 2024-04-23 20:50:46.000000 jeffutils-0.5.0/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-23 20:51:17.689698 jeffutils-0.5.0/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-23 20:51:17.000000 jeffutils-0.5.0/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-04-23 20:51:17.000000 jeffutils-0.5.0/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-04-23 20:51:17.000000 jeffutils-0.5.0/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-04-23 20:51:17.000000 jeffutils-0.5.0/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-30 20:42:19.202553 jeffutils-0.5.1/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.1/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-30 20:42:19.202553 jeffutils-0.5.1/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.1/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.1/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-04-30 20:42:19.202553 jeffutils-0.5.1/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-04-30 20:42:13.000000 jeffutils-0.5.1/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-30 20:42:19.202553 jeffutils-0.5.1/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-30 20:42:19.202553 jeffutils-0.5.1/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.1/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    16258 2024-04-30 20:41:26.000000 jeffutils-0.5.1/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-30 20:42:19.202553 jeffutils-0.5.1/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-30 20:42:19.000000 jeffutils-0.5.1/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-04-30 20:42:19.000000 jeffutils-0.5.1/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-04-30 20:42:19.000000 jeffutils-0.5.1/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-04-30 20:42:19.000000 jeffutils-0.5.1/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.5.0/LICENSE.txt` & `jeffutils-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.5.0/setup.py` & `jeffutils-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.5.0',
+    version='0.5.1',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.5.0/src/jeffutils/utils.py` & `jeffutils-0.5.1/src/jeffutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from time import perf_counter
 import time
-from datetime import datetime
+from datetime import datetime, timezone
 import json
 import numpy as np
 import pandas as pd
 import io
 import os
 import pstats
 import cProfile
@@ -29,25 +29,25 @@
     """returns a string representation of the stack trace to
     help with debugging and error messages
     """
     return "".join(traceback.TracebackException.from_exception(e).format())
 
 def curr_time_str():
     """returns the current time as a string YYYY-MM-DD"""
-    now = datetime.utcnow()
+    now = datetime.now(timezone.utc)
     now_str = now.strftime("%m-%d-%Y")
     return now_str
 
 def current_time(utc=True, string=True, timestamp=False, hour_24=False):
     """prints the current time in YYYY-MM-DD HH:MM pm/am format
     can specify current utc time or current local time
     default local
     """
     if utc:
-        now = datetime.utcnow()
+        now = datetime.now(timezone.utc)
     else:
         now = datetime.now()
 
     if timestamp:
         return now.timestamp()
 
     if not string:
```

