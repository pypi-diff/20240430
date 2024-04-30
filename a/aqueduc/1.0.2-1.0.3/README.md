# Comparing `tmp/aqueduc-1.0.2.tar.gz` & `tmp/aqueduc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduc-1.0.2.tar", last modified: Tue Apr 30 12:06:41 2024, max compression
+gzip compressed data, was "aqueduc-1.0.3.tar", last modified: Tue Apr 30 12:29:00 2024, max compression
```

## Comparing `aqueduc-1.0.2.tar` & `aqueduc-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 12:06:41.881492 aqueduc-1.0.2/
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1051 2024-04-30 10:37:44.000000 aqueduc-1.0.2/LICENSE
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-04-30 12:06:41.881492 aqueduc-1.0.2/PKG-INFO
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1585 2024-04-29 14:32:26.000000 aqueduc-1.0.2/README.md
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)      362 2024-04-30 12:05:41.000000 aqueduc-1.0.2/pyproject.toml
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       38 2024-04-30 12:06:41.881492 aqueduc-1.0.2/setup.cfg
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       37 2024-04-29 14:32:26.000000 aqueduc-1.0.2/setup.py
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 12:06:41.881492 aqueduc-1.0.2/src/
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       84 2024-04-30 11:44:58.000000 aqueduc-1.0.2/src/__main__.py
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 12:06:41.881492 aqueduc-1.0.2/src/aqueduc.egg-info/
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-04-30 12:06:41.000000 aqueduc-1.0.2/src/aqueduc.egg-info/PKG-INFO
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)      262 2024-04-30 12:06:41.000000 aqueduc-1.0.2/src/aqueduc.egg-info/SOURCES.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)        1 2024-04-30 12:06:41.000000 aqueduc-1.0.2/src/aqueduc.egg-info/dependency_links.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       50 2024-04-30 12:06:41.000000 aqueduc-1.0.2/src/aqueduc.egg-info/entry_points.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       22 2024-04-30 12:06:41.000000 aqueduc-1.0.2/src/aqueduc.egg-info/top_level.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     4542 2024-04-30 11:44:13.000000 aqueduc-1.0.2/src/aqueduc.py
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2793 2024-04-29 15:04:50.000000 aqueduc-1.0.2/src/test.py
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 12:29:00.741086 aqueduc-1.0.3/
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1051 2024-04-30 10:37:44.000000 aqueduc-1.0.3/LICENSE
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-04-30 12:29:00.741086 aqueduc-1.0.3/PKG-INFO
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1585 2024-04-29 14:32:26.000000 aqueduc-1.0.3/README.md
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)      354 2024-04-30 12:19:34.000000 aqueduc-1.0.3/pyproject.toml
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       38 2024-04-30 12:29:00.741086 aqueduc-1.0.3/setup.cfg
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       37 2024-04-29 14:32:26.000000 aqueduc-1.0.3/setup.py
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 12:29:00.741086 aqueduc-1.0.3/src/
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       84 2024-04-30 11:44:58.000000 aqueduc-1.0.3/src/__main__.py
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 12:29:00.741086 aqueduc-1.0.3/src/aqueduc.egg-info/
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-04-30 12:29:00.000000 aqueduc-1.0.3/src/aqueduc.egg-info/PKG-INFO
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)      262 2024-04-30 12:29:00.000000 aqueduc-1.0.3/src/aqueduc.egg-info/SOURCES.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)        1 2024-04-30 12:29:00.000000 aqueduc-1.0.3/src/aqueduc.egg-info/dependency_links.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       42 2024-04-30 12:29:00.000000 aqueduc-1.0.3/src/aqueduc.egg-info/entry_points.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       22 2024-04-30 12:29:00.000000 aqueduc-1.0.3/src/aqueduc.egg-info/top_level.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     4542 2024-04-30 11:44:13.000000 aqueduc-1.0.3/src/aqueduc.py
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2793 2024-04-29 15:04:50.000000 aqueduc-1.0.3/src/test.py
```

### Comparing `aqueduc-1.0.2/LICENSE` & `aqueduc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aqueduc-1.0.2/PKG-INFO` & `aqueduc-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduc
-Version: 1.0.2
+Version: 1.0.3
 Author: Mozenn
 License: Copyright 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
         and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `aqueduc-1.0.2/README.md` & `aqueduc-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aqueduc-1.0.2/src/aqueduc.egg-info/PKG-INFO` & `aqueduc-1.0.3/src/aqueduc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduc
-Version: 1.0.2
+Version: 1.0.3
 Author: Mozenn
 License: Copyright 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
         and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `aqueduc-1.0.2/src/aqueduc.py` & `aqueduc-1.0.3/src/aqueduc.py`

 * *Files identical despite different names*

### Comparing `aqueduc-1.0.2/src/test.py` & `aqueduc-1.0.3/src/test.py`

 * *Files identical despite different names*

