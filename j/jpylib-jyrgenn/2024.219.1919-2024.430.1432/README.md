# Comparing `tmp/jpylib-jyrgenn-2024.219.1919.tar.gz` & `tmp/jpylib-jyrgenn-2024.430.1432.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jpylib-jyrgenn-2024.219.1919.tar", last modified: Mon Feb 19 18:19:45 2024, max compression
+gzip compressed data, was "jpylib-jyrgenn-2024.430.1432.tar", last modified: Tue Apr 30 12:32:20 2024, max compression
```

## Comparing `jpylib-jyrgenn-2024.219.1919.tar` & `jpylib-jyrgenn-2024.430.1432.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ni         (501) staff       (20)        0 2024-02-19 18:19:45.696440 jpylib-jyrgenn-2024.219.1919/
--rw-r--r--   0 ni         (501) staff       (20)     1031 2024-02-19 18:19:45.696313 jpylib-jyrgenn-2024.219.1919/PKG-INFO
--rw-r--r--   0 ni         (501) staff       (20)      516 2022-03-11 11:18:51.000000 jpylib-jyrgenn-2024.219.1919/README.md
-drwxr-xr-x   0 ni         (501) staff       (20)        0 2024-02-19 18:19:45.695687 jpylib-jyrgenn-2024.219.1919/jpylib/
--rwxr-xr-x   0 ni         (501) staff       (20)     2601 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/__init__.py
--rwxr-xr-x   0 ni         (501) staff       (20)    12305 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/alerts.py
--rwxr-xr-x   0 ni         (501) staff       (20)     1828 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/assorted.py
--rwxr-xr-x   0 ni         (501) staff       (20)     4537 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/capture.py
--rwxr-xr-x   0 ni         (501) staff       (20)     3329 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/config.py
--rwxr-xr-x   0 ni         (501) staff       (20)      508 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/fntrace.py
--rw-r--r--   0 ni         (501) staff       (20)     5040 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/iohelper.py
--rwxr-xr-x   0 ni         (501) staff       (20)     5860 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/kvs.py
--rw-r--r--   0 ni         (501) staff       (20)     2418 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/multiset.py
--rwxr-xr-x   0 ni         (501) staff       (20)     2720 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/namespace.py
--rw-r--r--   0 ni         (501) staff       (20)     1756 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/numeric.py
--rwxr-xr-x   0 ni         (501) staff       (20)    12346 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/options.py
--rwxr-xr-x   0 ni         (501) staff       (20)     4286 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/process.py
--rwxr-xr-x   0 ni         (501) staff       (20)    10543 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/secrets.py
--rwxr-xr-x   0 ni         (501) staff       (20)     1687 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/sighandler.py
--rw-r--r--   0 ni         (501) staff       (20)      454 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/singleton.py
--rwxr-xr-x   0 ni         (501) staff       (20)     1569 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/stringreader.py
--rwxr-xr-x   0 ni         (501) staff       (20)    10669 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/table.py
--rwxr-xr-x   0 ni         (501) staff       (20)     2988 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/table_templates.py
--rwxr-xr-x   0 ni         (501) staff       (20)     1179 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/terminal.py
--rw-r--r--   0 ni         (501) staff       (20)      518 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/text.py
--rwxr-xr-x   0 ni         (501) staff       (20)      695 2024-02-19 18:19:44.000000 jpylib-jyrgenn-2024.219.1919/jpylib/time.py
-drwxr-xr-x   0 ni         (501) staff       (20)        0 2024-02-19 18:19:45.696140 jpylib-jyrgenn-2024.219.1919/jpylib_jyrgenn.egg-info/
--rw-r--r--   0 ni         (501) staff       (20)     1031 2024-02-19 18:19:45.000000 jpylib-jyrgenn-2024.219.1919/jpylib_jyrgenn.egg-info/PKG-INFO
--rw-r--r--   0 ni         (501) staff       (20)      577 2024-02-19 18:19:45.000000 jpylib-jyrgenn-2024.219.1919/jpylib_jyrgenn.egg-info/SOURCES.txt
--rw-r--r--   0 ni         (501) staff       (20)        1 2024-02-19 18:19:45.000000 jpylib-jyrgenn-2024.219.1919/jpylib_jyrgenn.egg-info/dependency_links.txt
--rw-r--r--   0 ni         (501) staff       (20)        7 2024-02-19 18:19:45.000000 jpylib-jyrgenn-2024.219.1919/jpylib_jyrgenn.egg-info/top_level.txt
--rw-r--r--   0 ni         (501) staff       (20)       38 2024-02-19 18:19:45.696481 jpylib-jyrgenn-2024.219.1919/setup.cfg
--rwxr-xr-x   0 ni         (501) staff       (20)     1067 2022-03-11 11:19:38.000000 jpylib-jyrgenn-2024.219.1919/setup.py
+drwxr-xr-x   0 jnic       (501) staff       (20)        0 2024-04-30 12:32:20.214824 jpylib-jyrgenn-2024.430.1432/
+-rw-r--r--   0 jnic       (501) staff       (20)     1031 2024-04-30 12:32:20.214339 jpylib-jyrgenn-2024.430.1432/PKG-INFO
+-rw-r--r--   0 jnic       (501) staff       (20)      516 2022-11-03 11:48:24.000000 jpylib-jyrgenn-2024.430.1432/README.md
+drwxr-xr-x   0 jnic       (501) staff       (20)        0 2024-04-30 12:32:20.211394 jpylib-jyrgenn-2024.430.1432/jpylib/
+-rwxr-xr-x   0 jnic       (501) staff       (20)     2601 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/__init__.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)    12305 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/alerts.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)     1828 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/assorted.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)     4537 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/capture.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)     3329 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/config.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)      508 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/fntrace.py
+-rw-r--r--   0 jnic       (501) staff       (20)     5040 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/iohelper.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)     5860 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/kvs.py
+-rw-r--r--   0 jnic       (501) staff       (20)     2418 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/multiset.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)     2720 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/namespace.py
+-rw-r--r--   0 jnic       (501) staff       (20)     1756 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/numeric.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)    12346 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/options.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)     4769 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/process.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)    10543 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/secrets.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)     1687 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/sighandler.py
+-rw-r--r--   0 jnic       (501) staff       (20)      454 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/singleton.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)     1569 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/stringreader.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)    10669 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/table.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)     2988 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/table_templates.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)     1179 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/terminal.py
+-rw-r--r--   0 jnic       (501) staff       (20)      518 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/text.py
+-rwxr-xr-x   0 jnic       (501) staff       (20)      695 2024-04-30 12:32:19.000000 jpylib-jyrgenn-2024.430.1432/jpylib/time.py
+drwxr-xr-x   0 jnic       (501) staff       (20)        0 2024-04-30 12:32:20.213804 jpylib-jyrgenn-2024.430.1432/jpylib_jyrgenn.egg-info/
+-rw-r--r--   0 jnic       (501) staff       (20)     1031 2024-04-30 12:32:20.000000 jpylib-jyrgenn-2024.430.1432/jpylib_jyrgenn.egg-info/PKG-INFO
+-rw-r--r--   0 jnic       (501) staff       (20)      577 2024-04-30 12:32:20.000000 jpylib-jyrgenn-2024.430.1432/jpylib_jyrgenn.egg-info/SOURCES.txt
+-rw-r--r--   0 jnic       (501) staff       (20)        1 2024-04-30 12:32:20.000000 jpylib-jyrgenn-2024.430.1432/jpylib_jyrgenn.egg-info/dependency_links.txt
+-rw-r--r--   0 jnic       (501) staff       (20)        7 2024-04-30 12:32:20.000000 jpylib-jyrgenn-2024.430.1432/jpylib_jyrgenn.egg-info/top_level.txt
+-rw-r--r--   0 jnic       (501) staff       (20)       38 2024-04-30 12:32:20.215092 jpylib-jyrgenn-2024.430.1432/setup.cfg
+-rwxr-xr-x   0 jnic       (501) staff       (20)     1067 2022-11-03 11:48:24.000000 jpylib-jyrgenn-2024.430.1432/setup.py
```

### Comparing `jpylib-jyrgenn-2024.219.1919/PKG-INFO` & `jpylib-jyrgenn-2024.430.1432/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: jpylib-jyrgenn
-Version: 2024.219.1919
+Version: 2024.430.1432
 Summary: Utilities library with several more or less independent components
 Home-page: https://git.w21.org/ni/jpylib/
 Author: Juergen Nickelsen
 Author-email: ni@w21.org
-Project-URL: Documentation, https://git.w21.org/ni/jpylib//-/blob/v2024.219.1919/doc/jpylib.md
+Project-URL: Documentation, https://git.w21.org/ni/jpylib//-/blob/v2024.430.1432/doc/jpylib.md
 Project-URL: Source, https://git.w21.org/ni/jpylib/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
@@ -17,10 +17,10 @@
 
 This library is mainly intended for myself, so I can access it from
 anywhere. But anyone else is welcome to have a look. Documentation
 is still lacking, I know, but that shall change. Testing is better.
 
 The full documentation (what already exists of it) for this version
 is at
-<https://git.w21.org/ni/jpylib/-/blob/v2024.219.1919/doc/jpylib.md>
+<https://git.w21.org/ni/jpylib/-/blob/v2024.430.1432/doc/jpylib.md>
 
 [ni@w21.org 2022-03-11]
```

### Comparing `jpylib-jyrgenn-2024.219.1919/README.md` & `jpylib-jyrgenn-2024.430.1432/README.md`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/__init__.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
      avg_midrange, remove_outliers
 from .iohelper import all_input_lines, read_items, read_mapping
 from .time import isotime, isotime_ms, iso_time, iso_time_ms, iso_time_us
 from .table import format_table
 from .singleton import Singleton
 from .multiset import Multiset
 
-version = "2024.219.1919"
+version = "2024.430.1432"
 """The version of the `jpylib` package."""
 
 program = os.path.basename(sys.argv[0])
 """The name of the current program without its directory path."""
 
 real_home = pwd.getpwuid(os.getuid()).pw_dir
 """The home directory of the current user as defined for its user id."""
```

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/alerts.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/alerts.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/assorted.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/assorted.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/capture.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/capture.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/config.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/config.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/iohelper.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/iohelper.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/kvs.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/kvs.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/multiset.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/multiset.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/namespace.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/namespace.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/numeric.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/numeric.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/options.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/options.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/process.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/process.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- python -*-
 
 # Do things with processes.
 
+import selectors
 import subprocess
 from .alerts import *
 
 # we take these characters as the indication to run a command in the shell, if
 # not otherwise indicated
 shellmeta = "\"'`|&;[(<>)]*?$"
 
@@ -52,21 +53,40 @@
                 command = ["/bin/sh", "-c", command]
                 run_shell = True
             else:
                 command = command.split()
         else:
             command = command.split()
 
+    outbuf = []
+    errbuf = []
+
+    sel = selectors.DefaultSelector()
+    fds_active = 2
+
+    def read_callback(f, buf):
+        nonlocal fds_active
+        data = f.read().decode("utf-8")
+        if len(data) == 0:
+            fds_active -= 1
+        buf.append(data)
+
+    
     with subprocess.Popen(command, stdin=subprocess.DEVNULL,
                           stderr=subprocess.PIPE,
                           stdout=subprocess.PIPE) as proc:
+        sel.register(proc.stdout, selectors.EVENT_READ, outbuf)
+        sel.register(proc.stderr, selectors.EVENT_READ, errbuf)
+
+        while fds_active:
+            for key, mask in sel.select():
+                read_callback(key.fileobj, key.data)
+            
         proc.wait()
-        result = (proc.stdout.read().decode("utf-8"),
-                  proc.stderr.read().decode("utf-8"),
-                  proc.returncode)
+        result = ("".join(outbuf), "".join(errbuf), proc.returncode)
     if full_result:
         if full_result == "plus":
             return result, run_shell
         return result
     else:
         if not silent and (result[1] or result[2]):
             raise ChildProcessError("command {} exited status {}; stderr: {}"
```

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/secrets.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/secrets.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/sighandler.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/sighandler.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/stringreader.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/stringreader.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/table.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/table.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/table_templates.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/table_templates.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/terminal.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/terminal.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/text.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/text.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib/time.py` & `jpylib-jyrgenn-2024.430.1432/jpylib/time.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib_jyrgenn.egg-info/PKG-INFO` & `jpylib-jyrgenn-2024.430.1432/jpylib_jyrgenn.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: jpylib-jyrgenn
-Version: 2024.219.1919
+Version: 2024.430.1432
 Summary: Utilities library with several more or less independent components
 Home-page: https://git.w21.org/ni/jpylib/
 Author: Juergen Nickelsen
 Author-email: ni@w21.org
-Project-URL: Documentation, https://git.w21.org/ni/jpylib//-/blob/v2024.219.1919/doc/jpylib.md
+Project-URL: Documentation, https://git.w21.org/ni/jpylib//-/blob/v2024.430.1432/doc/jpylib.md
 Project-URL: Source, https://git.w21.org/ni/jpylib/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
@@ -17,10 +17,10 @@
 
 This library is mainly intended for myself, so I can access it from
 anywhere. But anyone else is welcome to have a look. Documentation
 is still lacking, I know, but that shall change. Testing is better.
 
 The full documentation (what already exists of it) for this version
 is at
-<https://git.w21.org/ni/jpylib/-/blob/v2024.219.1919/doc/jpylib.md>
+<https://git.w21.org/ni/jpylib/-/blob/v2024.430.1432/doc/jpylib.md>
 
 [ni@w21.org 2022-03-11]
```

### Comparing `jpylib-jyrgenn-2024.219.1919/jpylib_jyrgenn.egg-info/SOURCES.txt` & `jpylib-jyrgenn-2024.430.1432/jpylib_jyrgenn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2024.219.1919/setup.py` & `jpylib-jyrgenn-2024.430.1432/setup.py`

 * *Files identical despite different names*

