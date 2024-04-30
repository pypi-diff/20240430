# Comparing `tmp/mozdebug-0.3.0.tar.gz` & `tmp/mozdebug-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mozdebug-0.3.0.tar", last modified: Fri Mar 19 14:11:09 2021, max compression
+gzip compressed data, was "mozdebug-0.3.1.tar", last modified: Tue Apr 30 10:25:47 2024, max compression
```

## Comparing `mozdebug-0.3.0.tar` & `mozdebug-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2021-03-19 14:11:09.605958 mozdebug-0.3.0/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      531 2021-03-19 14:11:09.605958 mozdebug-0.3.0/PKG-INFO
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2021-03-19 14:11:09.605958 mozdebug-0.3.0/mozdebug/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      946 2020-09-07 04:47:39.000000 mozdebug-0.3.0/mozdebug/__init__.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)    11038 2021-03-02 19:14:08.000000 mozdebug-0.3.0/mozdebug/mozdebug.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2021-03-19 14:11:09.605958 mozdebug-0.3.0/mozdebug.egg-info/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      531 2021-03-19 14:11:09.000000 mozdebug-0.3.0/mozdebug.egg-info/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)      250 2021-03-19 14:11:09.000000 mozdebug-0.3.0/mozdebug.egg-info/SOURCES.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2021-03-19 14:11:09.000000 mozdebug-0.3.0/mozdebug.egg-info/dependency_links.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2021-03-19 14:11:09.000000 mozdebug-0.3.0/mozdebug.egg-info/not-zip-safe
--rw-r--r--   0 ahal      (1000) ahal      (1000)        8 2021-03-19 14:11:09.000000 mozdebug-0.3.0/mozdebug.egg-info/requires.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)        9 2021-03-19 14:11:09.000000 mozdebug-0.3.0/mozdebug.egg-info/top_level.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       67 2021-03-19 14:11:09.605958 mozdebug-0.3.0/setup.cfg
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1095 2021-03-18 20:35:00.000000 mozdebug-0.3.0/setup.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-30 10:25:47.764227 mozdebug-0.3.1/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      501 2024-04-30 10:25:47.764227 mozdebug-0.3.1/PKG-INFO
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-30 10:25:47.763227 mozdebug-0.3.1/mozdebug/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      906 2024-02-27 12:31:33.000000 mozdebug-0.3.1/mozdebug/__init__.py
+-rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)    10962 2024-04-08 09:20:58.000000 mozdebug-0.3.1/mozdebug/mozdebug.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-30 10:25:47.763227 mozdebug-0.3.1/mozdebug.egg-info/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      501 2024-04-30 10:25:47.000000 mozdebug-0.3.1/mozdebug.egg-info/PKG-INFO
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      264 2024-04-30 10:25:47.000000 mozdebug-0.3.1/mozdebug.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2024-04-30 10:25:47.000000 mozdebug-0.3.1/mozdebug.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2024-04-30 10:25:47.000000 mozdebug-0.3.1/mozdebug.egg-info/not-zip-safe
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        8 2024-04-30 10:25:47.000000 mozdebug-0.3.1/mozdebug.egg-info/requires.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        9 2024-04-30 10:25:47.000000 mozdebug-0.3.1/mozdebug.egg-info/top_level.txt
+-rw-r--r--   0 jgraham   (1000) jgraham   (1000)       67 2024-04-30 10:25:47.764227 mozdebug-0.3.1/setup.cfg
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1055 2024-04-30 10:25:22.000000 mozdebug-0.3.1/setup.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-04-30 10:25:47.763227 mozdebug-0.3.1/tests/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1733 2024-02-27 12:31:33.000000 mozdebug-0.3.1/tests/test.py
```

### Comparing `mozdebug-0.3.0/mozdebug/__init__.py` & `mozdebug-0.3.1/mozdebug/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,10 +23,8 @@
 
   processArgs = [self.debuggerInfo.path] + self.debuggerInfo.args
   processArgs.append(debuggeePath)
 
   run_process(args, ...)
 
 """
-from __future__ import absolute_import
-
 from .mozdebug import *
```

### Comparing `mozdebug-0.3.0/mozdebug/mozdebug.py` & `mozdebug-0.3.1/mozdebug/mozdebug.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import, print_function
-
 import json
 import os
-import mozinfo
+import shutil
 import sys
 from collections import namedtuple
-from distutils.spawn import find_executable
 from subprocess import check_output
 
+import mozinfo
+
 __all__ = [
     "get_debugger_info",
     "get_default_debugger_name",
     "DebuggerSearch",
     "get_default_valgrind_args",
     "DebuggerInfo",
 ]
@@ -105,47 +104,47 @@
         try:
             path = check_output(
                 ["xcrun", "--find", "lldb"], universal_newlines=True
             ).strip()
             if path:
                 return path
         except Exception:
-            # Just default to find_executable instead.
+            # Just default to shutil.which instead.
             pass
 
     if mozinfo.os == "win" and debugger == "devenv.exe":
         # Attempt to use vswhere to find the path.
         try:
             encoding = "mbcs" if sys.platform == "win32" else "utf-8"
             vswhere = _vswhere_path()
             vsinfo = check_output([vswhere, "-format", "json", "-latest"])
             vsinfo = json.loads(vsinfo.decode(encoding, "replace"))
             return os.path.join(
                 vsinfo[0]["installationPath"], "Common7", "IDE", "devenv.exe"
             )
         except Exception:
-            # Just default to find_executable instead.
+            # Just default to shutil.which instead.
             pass
 
-    return find_executable(debugger)
+    return shutil.which(debugger)
 
 
 def get_debugger_info(debugger, debuggerArgs=None, debuggerInteractive=False):
     """
     Get the information about the requested debugger.
 
-    Returns a dictionary containing the |path| of the debugger executable,
-    if it will run in |interactive| mode, its arguments and whether it needs
-    to escape arguments it passes to the debugged program (|requiresEscapedArgs|).
-    If the debugger cannot be found in the system, returns |None|.
+    Returns a dictionary containing the ``path`` of the debugger executable,
+    if it will run in ``interactive`` mode, its arguments and whether it needs
+    to escape arguments it passes to the debugged program (``requiresEscapedArgs``).
+    If the debugger cannot be found in the system, returns ``None``.
 
     :param debugger: The name of the debugger.
     :param debuggerArgs: If specified, it's the arguments to pass to the debugger,
-    as a string. Any debugger-specific separator arguments are appended after these
-    arguments.
+       as a string. Any debugger-specific separator arguments are appended after
+       these arguments.
     :param debuggerInteractive: If specified, forces the debugger to be interactive.
     """
 
     debuggerPath = None
 
     if debugger:
         # Append '.exe' to the debugger on Windows if it's not present,
@@ -214,16 +213,16 @@
 
 
 def get_default_debugger_name(search=DebuggerSearch.OnlyFirst):
     """
     Get the debugger name for the default debugger on current platform.
 
     :param search: If specified, stops looking for the debugger if the
-     default one is not found (|DebuggerSearch.OnlyFirst|) or keeps
-     looking for other compatible debuggers (|DebuggerSearch.KeepLooking|).
+     default one is not found (``DebuggerSearch.OnlyFirst``) or keeps
+     looking for other compatible debuggers (``DebuggerSearch.KeepLooking``).
     """
 
     mozinfo.find_and_update_from_json()
     os = mozinfo.info["os"]
 
     # Find out which debuggers are preferred for use on this platform.
     debuggerPriorities = _DEBUGGER_PRIORITIES[
```

### Comparing `mozdebug-0.3.0/setup.py` & `mozdebug-0.3.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 from setuptools import setup
 
-PACKAGE_VERSION = "0.3.0"
+PACKAGE_VERSION = "0.3.1"
 DEPS = ["mozinfo"]
 
 
 setup(
     name="mozdebug",
     version=PACKAGE_VERSION,
     description="Utilities for running applications under native code debuggers "
```

