# Comparing `tmp/aqueduc-1.0.4.tar.gz` & `tmp/aqueduc-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduc-1.0.4.tar", last modified: Tue Apr 30 13:05:28 2024, max compression
+gzip compressed data, was "aqueduc-1.0.5.tar", last modified: Tue Apr 30 13:06:49 2024, max compression
```

## Comparing `aqueduc-1.0.4.tar` & `aqueduc-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 13:05:28.930423 aqueduc-1.0.4/
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1051 2024-04-30 10:37:44.000000 aqueduc-1.0.4/LICENSE
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-04-30 13:05:28.920423 aqueduc-1.0.4/PKG-INFO
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1585 2024-04-29 14:32:26.000000 aqueduc-1.0.4/README.md
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)      354 2024-04-30 13:05:17.000000 aqueduc-1.0.4/pyproject.toml
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       38 2024-04-30 13:05:28.930423 aqueduc-1.0.4/setup.cfg
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       37 2024-04-29 14:32:26.000000 aqueduc-1.0.4/setup.py
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 13:05:28.920423 aqueduc-1.0.4/src/
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 13:05:28.920423 aqueduc-1.0.4/src/aqueduc/
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       84 2024-04-30 11:44:58.000000 aqueduc-1.0.4/src/aqueduc/__main__.py
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     4542 2024-04-30 11:44:13.000000 aqueduc-1.0.4/src/aqueduc/aqueduc.py
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 13:05:28.920423 aqueduc-1.0.4/src/aqueduc.egg-info/
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-04-30 13:05:28.000000 aqueduc-1.0.4/src/aqueduc.egg-info/PKG-INFO
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)      278 2024-04-30 13:05:28.000000 aqueduc-1.0.4/src/aqueduc.egg-info/SOURCES.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)        1 2024-04-30 13:05:28.000000 aqueduc-1.0.4/src/aqueduc.egg-info/dependency_links.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       42 2024-04-30 13:05:28.000000 aqueduc-1.0.4/src/aqueduc.egg-info/entry_points.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       13 2024-04-30 13:05:28.000000 aqueduc-1.0.4/src/aqueduc.egg-info/top_level.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2793 2024-04-29 15:04:50.000000 aqueduc-1.0.4/src/test.py
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 13:06:49.310397 aqueduc-1.0.5/
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1051 2024-04-30 10:37:44.000000 aqueduc-1.0.5/LICENSE
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-04-30 13:06:49.310397 aqueduc-1.0.5/PKG-INFO
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1585 2024-04-29 14:32:26.000000 aqueduc-1.0.5/README.md
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)      362 2024-04-30 13:06:42.000000 aqueduc-1.0.5/pyproject.toml
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       38 2024-04-30 13:06:49.310397 aqueduc-1.0.5/setup.cfg
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       37 2024-04-29 14:32:26.000000 aqueduc-1.0.5/setup.py
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 13:06:49.300397 aqueduc-1.0.5/src/
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 13:06:49.300397 aqueduc-1.0.5/src/aqueduc/
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       84 2024-04-30 11:44:58.000000 aqueduc-1.0.5/src/aqueduc/__main__.py
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     4542 2024-04-30 11:44:13.000000 aqueduc-1.0.5/src/aqueduc/aqueduc.py
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 13:06:49.300397 aqueduc-1.0.5/src/aqueduc.egg-info/
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-04-30 13:06:49.000000 aqueduc-1.0.5/src/aqueduc.egg-info/PKG-INFO
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)      278 2024-04-30 13:06:49.000000 aqueduc-1.0.5/src/aqueduc.egg-info/SOURCES.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)        1 2024-04-30 13:06:49.000000 aqueduc-1.0.5/src/aqueduc.egg-info/dependency_links.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       50 2024-04-30 13:06:49.000000 aqueduc-1.0.5/src/aqueduc.egg-info/entry_points.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       13 2024-04-30 13:06:49.000000 aqueduc-1.0.5/src/aqueduc.egg-info/top_level.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2793 2024-04-29 15:04:50.000000 aqueduc-1.0.5/src/test.py
```

### Comparing `aqueduc-1.0.4/LICENSE` & `aqueduc-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aqueduc-1.0.4/PKG-INFO` & `aqueduc-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduc
-Version: 1.0.4
+Version: 1.0.5
 Author: Mozenn
 License: Copyright 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
         and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `aqueduc-1.0.4/README.md` & `aqueduc-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aqueduc-1.0.4/src/aqueduc/aqueduc.py` & `aqueduc-1.0.5/src/aqueduc/aqueduc.py`

 * *Files identical despite different names*

### Comparing `aqueduc-1.0.4/src/aqueduc.egg-info/PKG-INFO` & `aqueduc-1.0.5/src/aqueduc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduc
-Version: 1.0.4
+Version: 1.0.5
 Author: Mozenn
 License: Copyright 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
         and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `aqueduc-1.0.4/src/test.py` & `aqueduc-1.0.5/src/test.py`

 * *Files identical despite different names*

