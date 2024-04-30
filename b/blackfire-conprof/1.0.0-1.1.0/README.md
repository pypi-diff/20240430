# Comparing `tmp/blackfire_conprof-1.0.0-py3-none-any.whl.zip` & `tmp/blackfire_conprof-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,13 @@
-Zip file size: 4710 bytes, number of entries: 8
--rw-r--r--  2.0 unx       33 b- defN 23-Dec-21 13:37 blackfire_conprof/__init__.py
--rw-r--r--  2.0 unx     1955 b- defN 23-Dec-21 13:37 blackfire_conprof/log.py
--rw-r--r--  2.0 unx     3477 b- defN 23-Dec-21 13:37 blackfire_conprof/profiler.py
--rw-r--r--  2.0 unx       22 b- defN 23-Dec-21 13:38 blackfire_conprof/version.py
--rw-r--r--  2.0 unx     1998 b- defN 23-Dec-21 13:38 blackfire_conprof-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-21 13:38 blackfire_conprof-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Dec-21 13:38 blackfire_conprof-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      672 b- defN 23-Dec-21 13:38 blackfire_conprof-1.0.0.dist-info/RECORD
-8 files, 8267 bytes uncompressed, 3524 bytes compressed:  57.4%
+Zip file size: 6730 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1264 b- defN 24-Apr-30 11:12 blackfire_conprof/__init__.py
+-rw-r--r--  2.0 unx     1955 b- defN 24-Apr-30 11:12 blackfire_conprof/log.py
+-rw-r--r--  2.0 unx     3646 b- defN 24-Apr-30 11:12 blackfire_conprof/profiler.py
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-30 11:12 blackfire_conprof/version.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-30 11:12 blackfire_conprof/bootstrap/__init__.py
+-rw-r--r--  2.0 unx     1076 b- defN 24-Apr-30 11:12 blackfire_conprof/bootstrap/sitecustomize.py
+-rw-r--r--  2.0 unx     2599 b- defN 24-Apr-30 11:12 blackfire_conprof-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 11:12 blackfire_conprof-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 24-Apr-30 11:12 blackfire_conprof-1.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-30 11:12 blackfire_conprof-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      973 b- defN 24-Apr-30 11:12 blackfire_conprof-1.1.0.dist-info/RECORD
+11 files, 11718 bytes uncompressed, 5050 bytes compressed:  56.9%
```

## zipnote {}

```diff
@@ -6,20 +6,29 @@
 
 Filename: blackfire_conprof/profiler.py
 Comment: 
 
 Filename: blackfire_conprof/version.py
 Comment: 
 
-Filename: blackfire_conprof-1.0.0.dist-info/METADATA
+Filename: blackfire_conprof/bootstrap/__init__.py
 Comment: 
 
-Filename: blackfire_conprof-1.0.0.dist-info/WHEEL
+Filename: blackfire_conprof/bootstrap/sitecustomize.py
 Comment: 
 
-Filename: blackfire_conprof-1.0.0.dist-info/top_level.txt
+Filename: blackfire_conprof-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: blackfire_conprof-1.0.0.dist-info/RECORD
+Filename: blackfire_conprof-1.1.0.dist-info/WHEEL
+Comment: 
+
+Filename: blackfire_conprof-1.1.0.dist-info/entry_points.txt
+Comment: 
+
+Filename: blackfire_conprof-1.1.0.dist-info/top_level.txt
+Comment: 
+
+Filename: blackfire_conprof-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## blackfire_conprof/__init__.py

```diff
@@ -1 +1,47 @@
+import sys, os
+from blackfire_conprof import log
 from .version import __version__
+
+logger = log.get_logger(__name__)
+
+def _print_help():
+    help_string = '''Usage: blackfire-conprof <application>
+       Runs the application with the Blackfire Continuous Profiler enabled.
+'''
+    print(help_string)
+
+
+def _add_bootstrap_to_pythonpath(bootstrap_dir):
+    python_path = os.environ.get('PYTHONPATH', '')
+
+    if python_path:
+        new_path = '%s%s%s' % (
+            bootstrap_dir, os.path.pathsep, os.environ['PYTHONPATH']
+        )
+        os.environ['PYTHONPATH'] = new_path
+    else:
+        os.environ['PYTHONPATH'] = bootstrap_dir
+
+def bootstrap_python():
+    ext_dir = os.path.dirname(os.path.abspath(__file__))
+    bootstrap_dir = os.path.join(ext_dir, 'bootstrap')
+
+    _add_bootstrap_to_pythonpath(bootstrap_dir)
+
+    logger.debug('PYTHONPATH: %s' % os.environ['PYTHONPATH'])
+
+    cmd = sys.argv[1:]
+
+    if len(cmd) == 0:
+        _print_help()
+        sys.exit(1)
+
+    executable = sys.argv[1]
+    args = sys.argv[2:]
+
+    from shutil import which
+    executable_path = which(executable)
+
+    # execl(...) propagates current env. vars to the new process and thus runs 
+    # with the new PYTHONPATH
+    os.execl(executable_path, executable_path, *args)
```

## blackfire_conprof/profiler.py

```diff
@@ -1,9 +1,14 @@
 import re
 import os
+
+# DD profiler requires this for patching the runtime. Example: for gevent to work
+# correctly, this needs to be imported before gevent.patch_all()
+import ddtrace.auto
+
 import platform
 import collections
 from blackfire_conprof import log
 from .version import __version__
 
 from ddtrace.profiling import Profiler as DDProfiler
 log.bridge_ddtrace_logging()
```

## blackfire_conprof/version.py

```diff
@@ -1 +1 @@
-__version__ = "v1.0.0"
+__version__ = "v1.1.0"
```

## Comparing `blackfire_conprof-1.0.0.dist-info/METADATA` & `blackfire_conprof-1.1.0.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackfire-conprof
-Version: 1.0.0
+Version: 1.1.0
 Summary: Blackfire Continuous Profiler
 Home-page: https://blackfire.io
 Author: Blackfire.io
 Author-email: support@blackfire.io
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -62,11 +62,39 @@
 ```
 BLACKFIRE_SOCKET="tcp://127.0.0.1:8307" blackfire agent --log-level=4
 ```
 
 4. Run the example application. (`python example.py`)
 5. Profiler will send data to the Agent, and Agent will forward it to the Blackfire backend. Data then can be visualized at https://blackfire.io
 
+# Enabling the profiler
+
+There are two ways to enable the profiler:
+ - via Code,
+ - via Command Line.
+
+## Code
+
+```python
+from blackfire_conprof.profiler import Profiler
+
+profiler = Profiler()
+profiler.start()
+```
+
+Please note that the above needs to be done as early as possible in your application. Example: for gevent applications to work
+correctly, this needs to be imported before `gevent.monkey.patch_all()`.
+
+## Command line
+
+Run your Python application as following:
+
+```bash
+blackfire-conprof python app.py
+```
+
+This will automatically enable the profiler just before your application runs.
+
 # Contributing
 
 Use `make help` to display an overview of useful commands for your dev environment.
```

