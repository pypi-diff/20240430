# Comparing `tmp/cmder-3.8.tar.gz` & `tmp/cmder-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmder-3.8.tar", last modified: Mon Feb  7 00:22:53 2022, max compression
+gzip compressed data, was "cmder-4.0.tar", last modified: Tue Apr 30 04:41:42 2024, max compression
```

## Comparing `cmder-3.8.tar` & `cmder-4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 00:22:53.832158 cmder-3.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-02-07 00:22:40.000000 cmder-3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-02-07 00:22:53.832158 cmder-3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-02-07 00:22:40.000000 cmder-3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-02-07 00:22:40.000000 cmder-3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-02-07 00:22:53.832158 cmder-3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 00:22:53.832158 cmder-3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 00:22:53.832158 cmder-3.8/src/cmder/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-02-07 00:22:40.000000 cmder-3.8/src/cmder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7173 2022-02-07 00:22:40.000000 cmder-3.8/src/cmder/cmder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 00:22:53.832158 cmder-3.8/src/cmder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-02-07 00:22:53.000000 cmder-3.8/src/cmder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-02-07 00:22:53.000000 cmder-3.8/src/cmder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 00:22:53.000000 cmder-3.8/src/cmder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-07 00:22:53.000000 cmder-3.8/src/cmder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:41:42.428839 cmder-4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 04:41:36.000000 cmder-4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-30 04:41:42.428839 cmder-4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-30 04:41:36.000000 cmder-4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-30 04:41:36.000000 cmder-4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-30 04:41:42.428839 cmder-4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:41:42.428839 cmder-4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:41:42.428839 cmder-4.0/src/cmder/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 04:41:36.000000 cmder-4.0/src/cmder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-30 04:41:36.000000 cmder-4.0/src/cmder/cmder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:41:42.428839 cmder-4.0/src/cmder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-30 04:41:42.000000 cmder-4.0/src/cmder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 04:41:42.000000 cmder-4.0/src/cmder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 04:41:42.000000 cmder-4.0/src/cmder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 04:41:42.000000 cmder-4.0/src/cmder.egg-info/top_level.txt
```

### Comparing `cmder-3.8/LICENSE` & `cmder-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmder-3.8/PKG-INFO` & `cmder-4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: cmder
-Version: 3.8
+Version: 4.0
 Summary: A shortcut for running shell command.
 Home-page: https://github.com/iBiology/cmder.git
 Author: FEI YUAN
 Author-email: yuanfeifuzzy@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -68,9 +66,7 @@
   on BSD system.
 2. Since the argument `shell=True` was pre-filled when call `subprocess.Popen`, user should be aware 
   of the potential security issue and use this module with caution.
 
 
 
 
-
-
```

### Comparing `cmder-3.8/README.md` & `cmder-4.0/README.md`

 * *Files identical despite different names*

### Comparing `cmder-3.8/setup.cfg` & `cmder-4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cmder
-version = 3.8
+version = 4.0
 author = FEI YUAN
 author_email = yuanfeifuzzy@gmail.com
 description = A shortcut for running shell command.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/iBiology/cmder.git
 project_urls =
```

### Comparing `cmder-3.8/src/cmder.egg-info/PKG-INFO` & `cmder-4.0/src/cmder.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: cmder
-Version: 3.8
+Version: 4.0
 Summary: A shortcut for running shell command.
 Home-page: https://github.com/iBiology/cmder.git
 Author: FEI YUAN
 Author-email: yuanfeifuzzy@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -68,9 +66,7 @@
   on BSD system.
 2. Since the argument `shell=True` was pre-filled when call `subprocess.Popen`, user should be aware 
   of the potential security issue and use this module with caution.
 
 
 
 
-
-
```

