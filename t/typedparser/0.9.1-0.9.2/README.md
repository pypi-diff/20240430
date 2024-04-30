# Comparing `tmp/typedparser-0.9.1.tar.gz` & `tmp/typedparser-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedparser-0.9.1.tar", last modified: Mon Jan 22 09:10:53 2024, max compression
+gzip compressed data, was "typedparser-0.9.2.tar", last modified: Mon Jan 22 09:22:39 2024, max compression
```

## Comparing `typedparser-0.9.1.tar` & `typedparser-0.9.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:10:53.777115 typedparser-0.9.1/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11339 2024-01-22 09:09:15.000000 typedparser-0.9.1/LICENSE
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     6391 2024-01-22 09:10:53.773115 typedparser-0.9.1/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)     5530 2024-01-22 09:10:44.000000 typedparser-0.9.1/README.md
--rw-------   0 gings    (14999) lmb-mit   (1061)     2564 2024-01-22 09:09:15.000000 typedparser-0.9.1/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       12 2024-01-22 09:10:44.000000 typedparser-0.9.1/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2024-01-22 09:10:53.777115 typedparser-0.9.1/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:10:53.709113 typedparser-0.9.1/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:10:53.733114 typedparser-0.9.1/src/typedparser/
--rw-------   0 gings    (14999) lmb-mit   (1061)      534 2024-01-22 09:10:44.000000 typedparser-0.9.1/src/typedparser/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    13757 2024-01-22 09:10:44.000000 typedparser-0.9.1/src/typedparser/_typedattr.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3838 2024-01-22 09:10:44.000000 typedparser-0.9.1/src/typedparser/_typedparser.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2356 2024-01-22 09:10:44.000000 typedparser-0.9.1/src/typedparser/custom_format.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     6823 2024-01-22 09:10:44.000000 typedparser-0.9.1/src/typedparser/funcs.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    11172 2024-01-22 09:10:44.000000 typedparser-0.9.1/src/typedparser/objects.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:10:53.769115 typedparser-0.9.1/src/typedparser.egg-info/
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     6391 2024-01-22 09:10:53.000000 typedparser-0.9.1/src/typedparser.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      452 2024-01-22 09:10:53.000000 typedparser-0.9.1/src/typedparser.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2024-01-22 09:10:53.000000 typedparser-0.9.1/src/typedparser.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       12 2024-01-22 09:10:53.000000 typedparser-0.9.1/src/typedparser.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       12 2024-01-22 09:10:53.000000 typedparser-0.9.1/src/typedparser.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 09:37:17.000000 typedparser-0.9.1/src/typedparser.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:22:39.396626 typedparser-0.9.2/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11339 2024-01-22 09:09:15.000000 typedparser-0.9.2/LICENSE
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     6391 2024-01-22 09:22:39.392626 typedparser-0.9.2/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5530 2024-01-22 09:22:30.000000 typedparser-0.9.2/README.md
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2564 2024-01-22 09:09:15.000000 typedparser-0.9.2/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       12 2024-01-22 09:22:30.000000 typedparser-0.9.2/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2024-01-22 09:22:39.396626 typedparser-0.9.2/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:22:39.348625 typedparser-0.9.2/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:22:39.368625 typedparser-0.9.2/src/typedparser/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      534 2024-01-22 09:22:30.000000 typedparser-0.9.2/src/typedparser/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    13757 2024-01-22 09:22:30.000000 typedparser-0.9.2/src/typedparser/_typedattr.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3838 2024-01-22 09:22:30.000000 typedparser-0.9.2/src/typedparser/_typedparser.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2356 2024-01-22 09:22:30.000000 typedparser-0.9.2/src/typedparser/custom_format.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     6823 2024-01-22 09:22:30.000000 typedparser-0.9.2/src/typedparser/funcs.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11172 2024-01-22 09:22:30.000000 typedparser-0.9.2/src/typedparser/objects.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:22:39.392626 typedparser-0.9.2/src/typedparser.egg-info/
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     6391 2024-01-22 09:22:39.000000 typedparser-0.9.2/src/typedparser.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      452 2024-01-22 09:22:39.000000 typedparser-0.9.2/src/typedparser.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2024-01-22 09:22:39.000000 typedparser-0.9.2/src/typedparser.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       12 2024-01-22 09:22:39.000000 typedparser-0.9.2/src/typedparser.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       12 2024-01-22 09:22:39.000000 typedparser-0.9.2/src/typedparser.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-21 09:37:17.000000 typedparser-0.9.2/src/typedparser.egg-info/zip-safe
```

### Comparing `typedparser-0.9.1/LICENSE` & `typedparser-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `typedparser-0.9.1/PKG-INFO` & `typedparser-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedparser
-Version: 0.9.1
+Version: 0.9.2
 Summary: Extension for python argparse with typehints and typechecks.
 Author: simonging
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/simonging/typedparser
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `typedparser-0.9.1/README.md` & `typedparser-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `typedparser-0.9.1/pyproject.toml` & `typedparser-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedparser-0.9.1/src/typedparser/__init__.py` & `typedparser-0.9.2/src/typedparser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
     "add_argument",
     "TypedParser",
     "VerboseQuietArgs",
     "CustomArgparseFmt",
     "get_attr_names",
     "define",  # deprecated, use `from attr import define` directly instead
 ]
-__version__ = "0.9.1"
+__version__ = "0.9.2"
```

### Comparing `typedparser-0.9.1/src/typedparser/_typedattr.py` & `typedparser-0.9.2/src/typedparser/_typedattr.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.9.1/src/typedparser/_typedparser.py` & `typedparser-0.9.2/src/typedparser/_typedparser.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.9.1/src/typedparser/custom_format.py` & `typedparser-0.9.2/src/typedparser/custom_format.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.9.1/src/typedparser/funcs.py` & `typedparser-0.9.2/src/typedparser/funcs.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.9.1/src/typedparser/objects.py` & `typedparser-0.9.2/src/typedparser/objects.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.9.1/src/typedparser.egg-info/PKG-INFO` & `typedparser-0.9.2/src/typedparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedparser
-Version: 0.9.1
+Version: 0.9.2
 Summary: Extension for python argparse with typehints and typechecks.
 Author: simonging
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/simonging/typedparser
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

