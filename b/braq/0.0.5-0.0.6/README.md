# Comparing `tmp/braq-0.0.5.tar.gz` & `tmp/braq-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/braq-0.0.5.tar", last modified: Wed Mar 13 23:07:36 2024, max compression
+gzip compressed data, was "dist/braq-0.0.6.tar", last modified: Tue Apr 30 20:02:46 2024, max compression
```

## Comparing `braq-0.0.5.tar` & `braq-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:07:36.760472 braq-0.0.5/
--rw-rw-r--   0 alex      (1002) alex      (1003)     1082 2024-03-13 19:31:00.000000 braq-0.0.5/LICENSE
--rw-rw-r--   0 alex      (1002) alex      (1003)       66 2023-09-25 15:48:16.000000 braq-0.0.5/MANIFEST.in
--rw-rw-r--   0 alex      (1002) alex      (1003)    21782 2024-03-13 23:07:36.760472 braq-0.0.5/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)    21108 2024-03-13 19:29:40.000000 braq-0.0.5/README.md
--rw-rw-r--   0 alex      (1002) alex      (1003)        5 2024-01-05 12:25:31.000000 braq-0.0.5/VERSION
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:07:36.540470 braq-0.0.5/braq/
--rw-rw-r--   0 alex      (1002) alex      (1003)      541 2024-03-13 16:45:38.000000 braq-0.0.5/braq/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      130 2023-10-09 17:20:27.000000 braq-0.0.5/braq/__main__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:07:36.576471 braq-0.0.5/braq/document/
--rw-rw-r--   0 alex      (1002) alex      (1003)     9591 2024-03-13 16:43:46.000000 braq-0.0.5/braq/document/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:07:36.576471 braq-0.0.5/braq/errors/
--rw-rw-r--   0 alex      (1002) alex      (1003)       55 2024-03-07 00:49:13.000000 braq-0.0.5/braq/errors/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:07:36.596471 braq-0.0.5/braq/filedoc/
--rw-rw-r--   0 alex      (1002) alex      (1003)     5898 2024-03-07 09:10:20.000000 braq-0.0.5/braq/filedoc/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:07:36.604471 braq-0.0.5/braq/fileio/
--rw-rw-r--   0 alex      (1002) alex      (1003)     2325 2024-03-07 08:20:59.000000 braq-0.0.5/braq/fileio/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:07:36.624471 braq-0.0.5/braq/misc/
--rw-rw-r--   0 alex      (1002) alex      (1003)      119 2024-01-05 12:21:35.000000 braq-0.0.5/braq/misc/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:07:36.644471 braq-0.0.5/braq/parser/
--rw-rw-r--   0 alex      (1002) alex      (1003)     4769 2024-03-07 08:15:19.000000 braq-0.0.5/braq/parser/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:07:36.660471 braq-0.0.5/braq/section/
--rw-rw-r--   0 alex      (1002) alex      (1003)     2111 2024-03-07 07:34:18.000000 braq-0.0.5/braq/section/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:07:36.576471 braq-0.0.5/braq.egg-info/
--rw-r--r--   0 alex      (1002) alex      (1003)    21782 2024-03-13 23:07:36.000000 braq-0.0.5/braq.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)      640 2024-03-13 23:07:36.000000 braq-0.0.5/braq.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2024-03-13 23:07:36.000000 braq-0.0.5/braq.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       45 2024-03-13 23:07:36.000000 braq-0.0.5/braq.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-09-25 15:49:48.000000 braq-0.0.5/braq.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1002) alex      (1003)       17 2024-03-13 23:07:36.000000 braq-0.0.5/braq.egg-info/requires.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       11 2024-03-13 23:07:36.000000 braq-0.0.5/braq.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2023-09-25 15:48:16.000000 braq-0.0.5/pyproject.toml
--rw-rw-r--   0 alex      (1002) alex      (1003)      891 2024-03-13 23:07:36.764472 braq-0.0.5/setup.cfg
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2023-09-25 15:48:16.000000 braq-0.0.5/setup.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:07:36.748472 braq-0.0.5/tests/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-09-25 15:48:16.000000 braq-0.0.5/tests/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    13325 2024-03-05 10:51:30.000000 braq-0.0.5/tests/test_document.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    17600 2024-03-07 09:06:32.000000 braq-0.0.5/tests/test_filedoc.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     4277 2024-03-07 08:21:21.000000 braq-0.0.5/tests/test_fileio.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      763 2024-03-01 10:48:32.000000 braq-0.0.5/tests/test_imports.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      520 2024-02-29 18:45:48.000000 braq-0.0.5/tests/test_misc.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     4432 2024-02-29 19:42:08.000000 braq-0.0.5/tests/test_parser.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2254 2024-02-29 20:20:00.000000 braq-0.0.5/tests/test_section.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:02:46.020860 braq-0.0.6/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1082 2024-03-13 19:31:00.000000 braq-0.0.6/LICENSE
+-rw-rw-r--   0 alex      (1002) alex      (1003)       66 2023-09-25 15:48:16.000000 braq-0.0.6/MANIFEST.in
+-rw-rw-r--   0 alex      (1002) alex      (1003)    22082 2024-04-30 20:02:46.020860 braq-0.0.6/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)    21408 2024-04-30 15:05:20.000000 braq-0.0.6/README.md
+-rw-rw-r--   0 alex      (1002) alex      (1003)        5 2024-03-13 23:07:37.000000 braq-0.0.6/VERSION
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:02:45.800851 braq-0.0.6/braq/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      541 2024-03-13 16:45:38.000000 braq-0.0.6/braq/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      145 2024-04-30 00:56:29.000000 braq-0.0.6/braq/__main__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:02:45.848853 braq-0.0.6/braq/document/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     9561 2024-04-30 00:56:29.000000 braq-0.0.6/braq/document/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:02:45.848853 braq-0.0.6/braq/errors/
+-rw-rw-r--   0 alex      (1002) alex      (1003)       55 2024-03-07 00:49:13.000000 braq-0.0.6/braq/errors/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:02:45.864853 braq-0.0.6/braq/filedoc/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     5907 2024-04-30 00:56:29.000000 braq-0.0.6/braq/filedoc/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:02:45.884854 braq-0.0.6/braq/fileio/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2353 2024-04-30 00:56:29.000000 braq-0.0.6/braq/fileio/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:02:45.888855 braq-0.0.6/braq/misc/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      119 2024-01-05 12:21:35.000000 braq-0.0.6/braq/misc/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:02:45.904855 braq-0.0.6/braq/parser/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4830 2024-04-30 00:56:28.000000 braq-0.0.6/braq/parser/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:02:45.928856 braq-0.0.6/braq/section/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2134 2024-04-30 00:56:29.000000 braq-0.0.6/braq/section/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:02:45.848853 braq-0.0.6/braq.egg-info/
+-rw-r--r--   0 alex      (1002) alex      (1003)    22082 2024-04-30 20:02:45.000000 braq-0.0.6/braq.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)      640 2024-04-30 20:02:45.000000 braq-0.0.6/braq.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2024-04-30 20:02:45.000000 braq-0.0.6/braq.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       45 2024-04-30 20:02:45.000000 braq-0.0.6/braq.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-09-25 15:49:48.000000 braq-0.0.6/braq.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1002) alex      (1003)       17 2024-04-30 20:02:45.000000 braq-0.0.6/braq.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       11 2024-04-30 20:02:45.000000 braq-0.0.6/braq.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2023-09-25 15:48:16.000000 braq-0.0.6/pyproject.toml
+-rw-rw-r--   0 alex      (1002) alex      (1003)      891 2024-04-30 20:02:46.020860 braq-0.0.6/setup.cfg
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2023-09-25 15:48:16.000000 braq-0.0.6/setup.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:02:46.008859 braq-0.0.6/tests/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-09-25 15:48:16.000000 braq-0.0.6/tests/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    13325 2024-03-05 10:51:30.000000 braq-0.0.6/tests/test_document.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    17600 2024-03-07 09:06:32.000000 braq-0.0.6/tests/test_filedoc.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4277 2024-03-07 08:21:21.000000 braq-0.0.6/tests/test_fileio.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      763 2024-03-01 10:48:32.000000 braq-0.0.6/tests/test_imports.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      520 2024-02-29 18:45:48.000000 braq-0.0.6/tests/test_misc.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4432 2024-02-29 19:42:08.000000 braq-0.0.6/tests/test_parser.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2254 2024-02-29 20:20:00.000000 braq-0.0.6/tests/test_section.py
```

### Comparing `braq-0.0.5/LICENSE` & `braq-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `braq-0.0.5/PKG-INFO` & `braq-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braq
-Version: 0.0.5
+Version: 0.0.6
 Summary: Customizable data format for config files, AI prompts, and more
 Home-page: https://github.com/pyrustic/braq
 Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com
 Maintainer: Pyrustic Evangelist
 Maintainer-email: rusticalex@yahoo.com
 License: MIT
@@ -329,15 +329,15 @@
 # beware, the 'validate' method may raise an exception
 # for good reasons !
 ```
 
 > There is more to discover about the `Document` class, such as the `clear`, `remove`, and `render` methods, exposed properties, and more.
 
 
-> Check out the documentation for `braq.Document` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.Document` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/class-Document.md).
 
 
 ## File document class
 The `FileDoc` class is based on the **Document** class and focuses specifically on documents with associated disk files such as **config files**.
 
 > As with the `Document` class, a schema can be passed to a `FileDoc` instance to validate dict sections.
 
@@ -367,15 +367,15 @@
     # perform several changes here !
     # ...
     confile.embed("gui", {"color": "blue"})
 ```
 
 > There is more to discover about the **FileDoc** class, such as the `load`, `save`, and `save_to` methods, exposed properties, and more.
 
-> Check out the documentation for `braq.FileDoc` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.FileDoc` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/class-FileDoc.md).
 
 <p align="right"><a href="#readme">Back to top</a></p>
 
 # Section class
 The `Section` class is an abstraction representing a Braq section. It exposes the `header` and `body` properties and renders itself when its `__str__` method is called implicitly.
 
 ```python
@@ -421,15 +421,15 @@
 
 # check headers
 assert tuple(d.keys()) == ("", "section 1")
 # check the body of 'section 1'
 assert d["section 1"] == "this is section 1"
 ```
 
-> Check out the documentation for `braq.parse` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.parse` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#parse).
 
 ## Parse a document iteratively
 A document can be parsed line by line as following:
 
 ```python
 import braq
 
@@ -452,15 +452,15 @@
 this is the unnamed section
 
 [section 1]
 this is section 1
 ```
 
 
-> Check out the documentation for `braq.parse_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.parse_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#parse_iter).
 
 ## Read a file
 The library exposes the `read` function which takes as input the path to a file to parse, then returns a dictionary whose keys and values are strings representing headers and bodies respectively.
 
 > Sections sharing the same header are concatenated !
 
 ```python
@@ -468,15 +468,15 @@
 
 path = "/home/alex/braqfile.txt"
 
 r = braq.read(path)
 assert tuple(r.keys()) == ("", "section 1")
 ```
 
-> Check out the documentation for `braq.read` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.read` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#read).
 
 ## Read a file iteratively
 A large text file can be parsed line by line as following:
 
 ```python
 import braq
 
@@ -493,15 +493,15 @@
 ```text
 this is the unnamed section
 
 [section 1]
 this is section 1
 ```
 
-> Check out the documentation for `braq.read_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.read_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#read_iter).
 
 ## Render a document
 Rendering a document involves transforming Python objects representing sections into Braq text which is a string that can be displayed on the screen or stored in a file.
 
 The library exposes the `render` function which accepts as input a sequence of sections (either header-body tuples or `Section` objects) and returns a Braq document.
 
 ```python
@@ -533,15 +533,15 @@
 line e
 line f
 ```
 
 > The `render` function also accepts the `spacing` argument which defaults to 1 and represents the number of lines of spacing between two adjacent sections.
 
 
-> Check out the documentation for `braq.render` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.render` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#render).
 
 ## Write to file
 Following is a snippet for writting a Braq document to a file:
 
 ```python
 import braq
 
@@ -563,15 +563,15 @@
 
 [section 3]
 line a
 line b
 ```
 
 
-> Check out the documentation for `braq.write` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.write` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#write).
 
 
 <p align="right"><a href="#readme">Back to top</a></p>
 
 # Braq schema for data validation
 Dict sections can be validated against a Braq schema. A Braq schema is a Python dictionary object that can be passed to a `Document` or a `FileDoc`. The keys of this dictionary are the headers of dict sections to validate and the values are [Paradict](https://github.com/pyrustic/paradict) schemas.
 
@@ -632,15 +632,15 @@
 
 line_1 = "[my header]"
 line_2 = "[this isn't a header] at all"
 assert braq.get_header(line_1) == "my header"
 assert braq.get_header(line_2) is None
 ```
 
-> Check out the documentation for `braq.check_header` and `braq.get_header` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.check_header` and `braq.get_header` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#check_header).
 
 <p align="right"><a href="#readme">Back to top</a></p>
 
 # Miscellaneous
 Collection of miscellaneous notes.
 
 ## Cover image
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: braq Version: 0.0.5 Summary: Customizable data
+Metadata-Version: 2.1 Name: braq Version: 0.0.6 Summary: Customizable data
 format for config files, AI prompts, and more Home-page: https://github.com/
 pyrustic/braq Author: Pyrustic Evangelist Author-email: rusticalex@yahoo.com
 Maintainer: Pyrustic Evangelist Maintainer-email: rusticalex@yahoo.com License:
 MIT Keywords: data-format,config,configuration,configfile,config-
 files,customizable,versatile,ai-prompts,pyrustic Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.5
@@ -144,32 +144,33 @@
 section server_conf = {"ip-address": "127.0.0.1", "port": 80} document.embed
 ("server", server_conf) # list headers assert document.list_headers() == ("",
 "user", "server") # validate specific dict sections # (no args implies that the
 entire doc will be the target) document.validate("user", "server") # returns a
 bool # beware, the 'validate' method may raise an exception # for good reasons
 ! ``` > There is more to discover about the `Document` class, such as the
 `clear`, `remove`, and `render` methods, exposed properties, and more. > Check
-out the documentation for `braq.Document` [here](https://github.com/pyrustic/
-braq/blob/master/docs/README.md). ## File document class The `FileDoc` class is
-based on the **Document** class and focuses specifically on documents with
-associated disk files such as **config files**. > As with the `Document` class,
-a schema can be passed to a `FileDoc` instance to validate dict sections.
-```python from braq import FileDoc confile = FileDoc("config-file.braq") #
-build the 'user' section user = confile.build("user") # test assert user ==
-{"id": 42, "name": "alex"} # retrieve the unnamed section as a text text =
-confile.get("") # notice the empty header str # retrieve the 'user' dict
-section as a text text = confile.get("user") # embed a 'server' dict section
-server_conf = {"ip-address": "127.0.0.1", "port": 80} confile.embed("server",
-server_conf) # change persisted # batch edit mode (changes are persisted at the
-end) with confile.edit_model(): # by default, autosave==True # perform several
-changes here ! # ... confile.embed("gui", {"color": "blue"}) ``` > There is
-more to discover about the **FileDoc** class, such as the `load`, `save`, and
-`save_to` methods, exposed properties, and more. > Check out the documentation
-for `braq.FileDoc` [here](https://github.com/pyrustic/braq/blob/master/docs/
-README.md).
+out the API reference for `braq.Document` [here](https://github.com/pyrustic/
+braq/blob/master/docs/api/modules/braq/__init__/class-Document.md). ## File
+document class The `FileDoc` class is based on the **Document** class and
+focuses specifically on documents with associated disk files such as **config
+files**. > As with the `Document` class, a schema can be passed to a `FileDoc`
+instance to validate dict sections. ```python from braq import FileDoc confile
+= FileDoc("config-file.braq") # build the 'user' section user = confile.build
+("user") # test assert user == {"id": 42, "name": "alex"} # retrieve the
+unnamed section as a text text = confile.get("") # notice the empty header str
+# retrieve the 'user' dict section as a text text = confile.get("user") # embed
+a 'server' dict section server_conf = {"ip-address": "127.0.0.1", "port": 80}
+confile.embed("server", server_conf) # change persisted # batch edit mode
+(changes are persisted at the end) with confile.edit_model(): # by default,
+autosave==True # perform several changes here ! # ... confile.embed("gui",
+{"color": "blue"}) ``` > There is more to discover about the **FileDoc** class,
+such as the `load`, `save`, and `save_to` methods, exposed properties, and
+more. > Check out the API reference for `braq.FileDoc` [here](https://
+github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/class-
+FileDoc.md).
                                                                     _B_a_c_k_ _t_o_ _t_o_p
 # Section class The `Section` class is an abstraction representing a Braq
 section. It exposes the `header` and `body` properties and renders itself when
 its `__str__` method is called implicitly. ```python import braq # create a
 Section object header, body = "my header", ("line a", "line b") section =
 braq.Section(header, body) # test the properties assert section.header == "my
 header" assert section.body == "line a\nline b" # test the rendering assert str
@@ -183,55 +184,57 @@
 parsed, then returns a **dictionary** whose keys and values are strings
 representing headers and bodies respectively. > Sections sharing the same
 header are concatenated ! > The header of an unnamed section is an empty
 string. ```python import braq text = """\ this is the unnamed section at the
 top of this document... [section 1] this is section 1""" d = braq.parse(text) #
 check headers assert tuple(d.keys()) == ("", "section 1") # check the body of
 'section 1' assert d["section 1"] == "this is section 1" ``` > Check out the
-documentation for `braq.parse` [here](https://github.com/pyrustic/braq/blob/
-master/docs/README.md). ## Parse a document iteratively A document can be
-parsed line by line as following: ```python import braq text = """\ this is the
-unnamed section [section 1] this is section 1""" for header, body in
-braq.parse_iter(text): if header: print("[" + header + "]") for line in body:
-print(line) ``` Output: ```text this is the unnamed section [section 1] this is
-section 1 ``` > Check out the documentation for `braq.parse_iter` [here](https:
-//github.com/pyrustic/braq/blob/master/docs/README.md). ## Read a file The
-library exposes the `read` function which takes as input the path to a file to
-parse, then returns a dictionary whose keys and values are strings representing
-headers and bodies respectively. > Sections sharing the same header are
-concatenated ! ```python import braq path = "/home/alex/braqfile.txt" r =
-braq.read(path) assert tuple(r.keys()) == ("", "section 1") ``` > Check out the
-documentation for `braq.read` [here](https://github.com/pyrustic/braq/blob/
-master/docs/README.md). ## Read a file iteratively A large text file can be
-parsed line by line as following: ```python import braq path = "/home/alex/
-braqfile.txt" for header, body in braq.read_iter(path): if header: print("[" +
-header + "]") for line in body: print(line) ``` Output: ```text this is the
-unnamed section [section 1] this is section 1 ``` > Check out the documentation
-for `braq.read_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/
-README.md). ## Render a document Rendering a document involves transforming
-Python objects representing sections into Braq text which is a string that can
-be displayed on the screen or stored in a file. The library exposes the
-`render` function which accepts as input a sequence of sections (either header-
-body tuples or `Section` objects) and returns a Braq document. ```python import
-braq # sections section_1 = braq.Section("section 1", "line a\nline b")
-section_2 = "section 2", "line c\nline d" section_3 = "section 3", ("line e",
-"line f") # rendering r = braq.render(section_1, section_2, section_3) print(r)
-``` Output: ```text [section 1] line a line b [section 2] line c line d
-[section 3] line e line f ``` > The `render` function also accepts the
-`spacing` argument which defaults to 1 and represents the number of lines of
-spacing between two adjacent sections. > Check out the documentation for
-`braq.render` [here](https://github.com/pyrustic/braq/blob/master/docs/
-README.md). ## Write to file Following is a snippet for writting a Braq
+API reference for `braq.parse` [here](https://github.com/pyrustic/braq/blob/
+master/docs/api/modules/braq/__init__/funcs.md#parse). ## Parse a document
+iteratively A document can be parsed line by line as following: ```python
+import braq text = """\ this is the unnamed section [section 1] this is section
+1""" for header, body in braq.parse_iter(text): if header: print("[" + header +
+"]") for line in body: print(line) ``` Output: ```text this is the unnamed
+section [section 1] this is section 1 ``` > Check out the API reference for
+`braq.parse_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/api/
+modules/braq/__init__/funcs.md#parse_iter). ## Read a file The library exposes
+the `read` function which takes as input the path to a file to parse, then
+returns a dictionary whose keys and values are strings representing headers and
+bodies respectively. > Sections sharing the same header are concatenated !
+```python import braq path = "/home/alex/braqfile.txt" r = braq.read(path)
+assert tuple(r.keys()) == ("", "section 1") ``` > Check out the API reference
+for `braq.read` [here](https://github.com/pyrustic/braq/blob/master/docs/api/
+modules/braq/__init__/funcs.md#read). ## Read a file iteratively A large text
+file can be parsed line by line as following: ```python import braq path = "/
+home/alex/braqfile.txt" for header, body in braq.read_iter(path): if header:
+print("[" + header + "]") for line in body: print(line) ``` Output: ```text
+this is the unnamed section [section 1] this is section 1 ``` > Check out the
+API reference for `braq.read_iter` [here](https://github.com/pyrustic/braq/
+blob/master/docs/api/modules/braq/__init__/funcs.md#read_iter). ## Render a
+document Rendering a document involves transforming Python objects representing
+sections into Braq text which is a string that can be displayed on the screen
+or stored in a file. The library exposes the `render` function which accepts as
+input a sequence of sections (either header-body tuples or `Section` objects)
+and returns a Braq document. ```python import braq # sections section_1 =
+braq.Section("section 1", "line a\nline b") section_2 = "section 2", "line
+c\nline d" section_3 = "section 3", ("line e", "line f") # rendering r =
+braq.render(section_1, section_2, section_3) print(r) ``` Output: ```text
+[section 1] line a line b [section 2] line c line d [section 3] line e line f
+``` > The `render` function also accepts the `spacing` argument which defaults
+to 1 and represents the number of lines of spacing between two adjacent
+sections. > Check out the API reference for `braq.render` [here](https://
+github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/
+funcs.md#render). ## Write to file Following is a snippet for writting a Braq
 document to a file: ```python import braq # sections section_1 = braq.Section
 ("", "welcome") section_2 = braq.Section("section 2") section_3 = "section 3",
 ("line a", "line b") # path to file path = "/home/alex/braqfile.txt" # write to
 file r = braq.write(section_1, section_2, section_3, dest=path) ``` The
 contents of the Braq file: ```text welcome [section 2] [section 3] line a line
-b ``` > Check out the documentation for `braq.write` [here](https://github.com/
-pyrustic/braq/blob/master/docs/README.md).
+b ``` > Check out the API reference for `braq.write` [here](https://github.com/
+pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#write).
                                                                     _B_a_c_k_ _t_o_ _t_o_p
 # Braq schema for data validation Dict sections can be validated against a Braq
 schema. A Braq schema is a Python dictionary object that can be passed to a
 `Document` or a `FileDoc`. The keys of this dictionary are the headers of dict
 sections to validate and the values are [Paradict](https://github.com/pyrustic/
 paradict) schemas. A Paradict schema is a dictionary containing specs for data
 validation. A spec is either simply a string that represents an expected data
@@ -250,17 +253,17 @@
 and then returns a boolean to indicate whether this line is a header or not.
 ```python import braq line_1 = "[my header]" line_2 = "[this isn't a header] at
 all" assert braq.check_header(line_1) is True assert braq.check_header(line_2)
 is False ``` The `get_header` function accepts a line of text as input and
 returns a string if the line is a header. Otherwise, `None` is returned.
 ```python import braq line_1 = "[my header]" line_2 = "[this isn't a header] at
 all" assert braq.get_header(line_1) == "my header" assert braq.get_header
-(line_2) is None ``` > Check out the documentation for `braq.check_header` and
-`braq.get_header` [here](https://github.com/pyrustic/braq/blob/master/docs/
-README.md).
+(line_2) is None ``` > Check out the API reference for `braq.check_header` and
+`braq.get_header` [here](https://github.com/pyrustic/braq/blob/master/docs/api/
+modules/braq/__init__/funcs.md#check_header).
                                                                     _B_a_c_k_ _t_o_ _t_o_p
 # Miscellaneous Collection of miscellaneous notes. ## Cover image The beautiful
 cover image is generated with [Carbon](https://carbon.now.sh/about).
                                                                     _B_a_c_k_ _t_o_ _t_o_p
 # Testing and contributing Feel free to **open an issue** to report a bug,
 suggest some changes, show some useful code snippets, or discuss anything
 related to this project. You can also directly email [me](https://
```

### Comparing `braq-0.0.5/README.md` & `braq-0.0.6/braq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: braq
+Version: 0.0.6
+Summary: Customizable data format for config files, AI prompts, and more
+Home-page: https://github.com/pyrustic/braq
+Author: Pyrustic Evangelist
+Author-email: rusticalex@yahoo.com
+Maintainer: Pyrustic Evangelist
+Maintainer-email: rusticalex@yahoo.com
+License: MIT
+Keywords: data-format,config,configuration,configfile,config-files,customizable,versatile,ai-prompts,pyrustic
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI package version](https://img.shields.io/pypi/v/braq)](https://pypi.org/project/braq)
 [![Downloads](https://static.pepy.tech/badge/braq)](https://pepy.tech/project/braq)
 
 <!-- Cover -->
 <div align="center">
     <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/braq/cover.png" alt="Cover image" width="650">
@@ -310,15 +329,15 @@
 # beware, the 'validate' method may raise an exception
 # for good reasons !
 ```
 
 > There is more to discover about the `Document` class, such as the `clear`, `remove`, and `render` methods, exposed properties, and more.
 
 
-> Check out the documentation for `braq.Document` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.Document` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/class-Document.md).
 
 
 ## File document class
 The `FileDoc` class is based on the **Document** class and focuses specifically on documents with associated disk files such as **config files**.
 
 > As with the `Document` class, a schema can be passed to a `FileDoc` instance to validate dict sections.
 
@@ -348,15 +367,15 @@
     # perform several changes here !
     # ...
     confile.embed("gui", {"color": "blue"})
 ```
 
 > There is more to discover about the **FileDoc** class, such as the `load`, `save`, and `save_to` methods, exposed properties, and more.
 
-> Check out the documentation for `braq.FileDoc` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.FileDoc` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/class-FileDoc.md).
 
 <p align="right"><a href="#readme">Back to top</a></p>
 
 # Section class
 The `Section` class is an abstraction representing a Braq section. It exposes the `header` and `body` properties and renders itself when its `__str__` method is called implicitly.
 
 ```python
@@ -402,15 +421,15 @@
 
 # check headers
 assert tuple(d.keys()) == ("", "section 1")
 # check the body of 'section 1'
 assert d["section 1"] == "this is section 1"
 ```
 
-> Check out the documentation for `braq.parse` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.parse` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#parse).
 
 ## Parse a document iteratively
 A document can be parsed line by line as following:
 
 ```python
 import braq
 
@@ -433,15 +452,15 @@
 this is the unnamed section
 
 [section 1]
 this is section 1
 ```
 
 
-> Check out the documentation for `braq.parse_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.parse_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#parse_iter).
 
 ## Read a file
 The library exposes the `read` function which takes as input the path to a file to parse, then returns a dictionary whose keys and values are strings representing headers and bodies respectively.
 
 > Sections sharing the same header are concatenated !
 
 ```python
@@ -449,15 +468,15 @@
 
 path = "/home/alex/braqfile.txt"
 
 r = braq.read(path)
 assert tuple(r.keys()) == ("", "section 1")
 ```
 
-> Check out the documentation for `braq.read` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.read` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#read).
 
 ## Read a file iteratively
 A large text file can be parsed line by line as following:
 
 ```python
 import braq
 
@@ -474,15 +493,15 @@
 ```text
 this is the unnamed section
 
 [section 1]
 this is section 1
 ```
 
-> Check out the documentation for `braq.read_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.read_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#read_iter).
 
 ## Render a document
 Rendering a document involves transforming Python objects representing sections into Braq text which is a string that can be displayed on the screen or stored in a file.
 
 The library exposes the `render` function which accepts as input a sequence of sections (either header-body tuples or `Section` objects) and returns a Braq document.
 
 ```python
@@ -514,15 +533,15 @@
 line e
 line f
 ```
 
 > The `render` function also accepts the `spacing` argument which defaults to 1 and represents the number of lines of spacing between two adjacent sections.
 
 
-> Check out the documentation for `braq.render` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.render` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#render).
 
 ## Write to file
 Following is a snippet for writting a Braq document to a file:
 
 ```python
 import braq
 
@@ -544,15 +563,15 @@
 
 [section 3]
 line a
 line b
 ```
 
 
-> Check out the documentation for `braq.write` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.write` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#write).
 
 
 <p align="right"><a href="#readme">Back to top</a></p>
 
 # Braq schema for data validation
 Dict sections can be validated against a Braq schema. A Braq schema is a Python dictionary object that can be passed to a `Document` or a `FileDoc`. The keys of this dictionary are the headers of dict sections to validate and the values are [Paradict](https://github.com/pyrustic/paradict) schemas.
 
@@ -613,15 +632,15 @@
 
 line_1 = "[my header]"
 line_2 = "[this isn't a header] at all"
 assert braq.get_header(line_1) == "my header"
 assert braq.get_header(line_2) is None
 ```
 
-> Check out the documentation for `braq.check_header` and `braq.get_header` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.check_header` and `braq.get_header` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#check_header).
 
 <p align="right"><a href="#readme">Back to top</a></p>
 
 # Miscellaneous
 Collection of miscellaneous notes.
 
 ## Cover image
@@ -687,7 +706,9 @@
 Hello world, I'm Alex, a tech enthusiast ! Feel free to get in touch with [me](https://pyrustic.github.io/#contact) !
 
 <br>
 <br>
 <br>
 
 [Back to top](#readme)
+
+
```

#### html2text {}

```diff
@@ -1,11 +1,20 @@
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
-opensource.org/licenses/MIT) [![PyPI package version](https://img.shields.io/
-pypi/v/braq)](https://pypi.org/project/braq) [![Downloads](https://
-static.pepy.tech/badge/braq)](https://pepy.tech/project/braq)
+Metadata-Version: 2.1 Name: braq Version: 0.0.6 Summary: Customizable data
+format for config files, AI prompts, and more Home-page: https://github.com/
+pyrustic/braq Author: Pyrustic Evangelist Author-email: rusticalex@yahoo.com
+Maintainer: Pyrustic Evangelist Maintainer-email: rusticalex@yahoo.com License:
+MIT Keywords: data-format,config,configuration,configfile,config-
+files,customizable,versatile,ai-prompts,pyrustic Platform: UNKNOWN Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.5
+Description-Content-Type: text/markdown License-File: LICENSE [![License: MIT]
+(https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/
+licenses/MIT) [![PyPI package version](https://img.shields.io/pypi/v/braq)]
+(https://pypi.org/project/braq) [![Downloads](https://static.pepy.tech/badge/
+braq)](https://pepy.tech/project/braq)
                                  [Cover image]
                          Braq document with 3 sections
 # Braq CCuussttoommiizzaabbllee ddaattaa ffoorrmmaatt ffoorr ccoonnffiigg ffiilleess,, AAII pprroommppttss,, aanndd mmoorree This
 project is part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
 ## Table of contents - [Overview](#overview) - [Data format specification]
 (#data-format-specification) - [Notable use cases](#notable-use-cases) -
 [Config files](#config-files) - [AI prompts](#ai-prompts) - [Source code
@@ -135,32 +144,33 @@
 section server_conf = {"ip-address": "127.0.0.1", "port": 80} document.embed
 ("server", server_conf) # list headers assert document.list_headers() == ("",
 "user", "server") # validate specific dict sections # (no args implies that the
 entire doc will be the target) document.validate("user", "server") # returns a
 bool # beware, the 'validate' method may raise an exception # for good reasons
 ! ``` > There is more to discover about the `Document` class, such as the
 `clear`, `remove`, and `render` methods, exposed properties, and more. > Check
-out the documentation for `braq.Document` [here](https://github.com/pyrustic/
-braq/blob/master/docs/README.md). ## File document class The `FileDoc` class is
-based on the **Document** class and focuses specifically on documents with
-associated disk files such as **config files**. > As with the `Document` class,
-a schema can be passed to a `FileDoc` instance to validate dict sections.
-```python from braq import FileDoc confile = FileDoc("config-file.braq") #
-build the 'user' section user = confile.build("user") # test assert user ==
-{"id": 42, "name": "alex"} # retrieve the unnamed section as a text text =
-confile.get("") # notice the empty header str # retrieve the 'user' dict
-section as a text text = confile.get("user") # embed a 'server' dict section
-server_conf = {"ip-address": "127.0.0.1", "port": 80} confile.embed("server",
-server_conf) # change persisted # batch edit mode (changes are persisted at the
-end) with confile.edit_model(): # by default, autosave==True # perform several
-changes here ! # ... confile.embed("gui", {"color": "blue"}) ``` > There is
-more to discover about the **FileDoc** class, such as the `load`, `save`, and
-`save_to` methods, exposed properties, and more. > Check out the documentation
-for `braq.FileDoc` [here](https://github.com/pyrustic/braq/blob/master/docs/
-README.md).
+out the API reference for `braq.Document` [here](https://github.com/pyrustic/
+braq/blob/master/docs/api/modules/braq/__init__/class-Document.md). ## File
+document class The `FileDoc` class is based on the **Document** class and
+focuses specifically on documents with associated disk files such as **config
+files**. > As with the `Document` class, a schema can be passed to a `FileDoc`
+instance to validate dict sections. ```python from braq import FileDoc confile
+= FileDoc("config-file.braq") # build the 'user' section user = confile.build
+("user") # test assert user == {"id": 42, "name": "alex"} # retrieve the
+unnamed section as a text text = confile.get("") # notice the empty header str
+# retrieve the 'user' dict section as a text text = confile.get("user") # embed
+a 'server' dict section server_conf = {"ip-address": "127.0.0.1", "port": 80}
+confile.embed("server", server_conf) # change persisted # batch edit mode
+(changes are persisted at the end) with confile.edit_model(): # by default,
+autosave==True # perform several changes here ! # ... confile.embed("gui",
+{"color": "blue"}) ``` > There is more to discover about the **FileDoc** class,
+such as the `load`, `save`, and `save_to` methods, exposed properties, and
+more. > Check out the API reference for `braq.FileDoc` [here](https://
+github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/class-
+FileDoc.md).
                                                                     _B_a_c_k_ _t_o_ _t_o_p
 # Section class The `Section` class is an abstraction representing a Braq
 section. It exposes the `header` and `body` properties and renders itself when
 its `__str__` method is called implicitly. ```python import braq # create a
 Section object header, body = "my header", ("line a", "line b") section =
 braq.Section(header, body) # test the properties assert section.header == "my
 header" assert section.body == "line a\nline b" # test the rendering assert str
@@ -174,55 +184,57 @@
 parsed, then returns a **dictionary** whose keys and values are strings
 representing headers and bodies respectively. > Sections sharing the same
 header are concatenated ! > The header of an unnamed section is an empty
 string. ```python import braq text = """\ this is the unnamed section at the
 top of this document... [section 1] this is section 1""" d = braq.parse(text) #
 check headers assert tuple(d.keys()) == ("", "section 1") # check the body of
 'section 1' assert d["section 1"] == "this is section 1" ``` > Check out the
-documentation for `braq.parse` [here](https://github.com/pyrustic/braq/blob/
-master/docs/README.md). ## Parse a document iteratively A document can be
-parsed line by line as following: ```python import braq text = """\ this is the
-unnamed section [section 1] this is section 1""" for header, body in
-braq.parse_iter(text): if header: print("[" + header + "]") for line in body:
-print(line) ``` Output: ```text this is the unnamed section [section 1] this is
-section 1 ``` > Check out the documentation for `braq.parse_iter` [here](https:
-//github.com/pyrustic/braq/blob/master/docs/README.md). ## Read a file The
-library exposes the `read` function which takes as input the path to a file to
-parse, then returns a dictionary whose keys and values are strings representing
-headers and bodies respectively. > Sections sharing the same header are
-concatenated ! ```python import braq path = "/home/alex/braqfile.txt" r =
-braq.read(path) assert tuple(r.keys()) == ("", "section 1") ``` > Check out the
-documentation for `braq.read` [here](https://github.com/pyrustic/braq/blob/
-master/docs/README.md). ## Read a file iteratively A large text file can be
-parsed line by line as following: ```python import braq path = "/home/alex/
-braqfile.txt" for header, body in braq.read_iter(path): if header: print("[" +
-header + "]") for line in body: print(line) ``` Output: ```text this is the
-unnamed section [section 1] this is section 1 ``` > Check out the documentation
-for `braq.read_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/
-README.md). ## Render a document Rendering a document involves transforming
-Python objects representing sections into Braq text which is a string that can
-be displayed on the screen or stored in a file. The library exposes the
-`render` function which accepts as input a sequence of sections (either header-
-body tuples or `Section` objects) and returns a Braq document. ```python import
-braq # sections section_1 = braq.Section("section 1", "line a\nline b")
-section_2 = "section 2", "line c\nline d" section_3 = "section 3", ("line e",
-"line f") # rendering r = braq.render(section_1, section_2, section_3) print(r)
-``` Output: ```text [section 1] line a line b [section 2] line c line d
-[section 3] line e line f ``` > The `render` function also accepts the
-`spacing` argument which defaults to 1 and represents the number of lines of
-spacing between two adjacent sections. > Check out the documentation for
-`braq.render` [here](https://github.com/pyrustic/braq/blob/master/docs/
-README.md). ## Write to file Following is a snippet for writting a Braq
+API reference for `braq.parse` [here](https://github.com/pyrustic/braq/blob/
+master/docs/api/modules/braq/__init__/funcs.md#parse). ## Parse a document
+iteratively A document can be parsed line by line as following: ```python
+import braq text = """\ this is the unnamed section [section 1] this is section
+1""" for header, body in braq.parse_iter(text): if header: print("[" + header +
+"]") for line in body: print(line) ``` Output: ```text this is the unnamed
+section [section 1] this is section 1 ``` > Check out the API reference for
+`braq.parse_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/api/
+modules/braq/__init__/funcs.md#parse_iter). ## Read a file The library exposes
+the `read` function which takes as input the path to a file to parse, then
+returns a dictionary whose keys and values are strings representing headers and
+bodies respectively. > Sections sharing the same header are concatenated !
+```python import braq path = "/home/alex/braqfile.txt" r = braq.read(path)
+assert tuple(r.keys()) == ("", "section 1") ``` > Check out the API reference
+for `braq.read` [here](https://github.com/pyrustic/braq/blob/master/docs/api/
+modules/braq/__init__/funcs.md#read). ## Read a file iteratively A large text
+file can be parsed line by line as following: ```python import braq path = "/
+home/alex/braqfile.txt" for header, body in braq.read_iter(path): if header:
+print("[" + header + "]") for line in body: print(line) ``` Output: ```text
+this is the unnamed section [section 1] this is section 1 ``` > Check out the
+API reference for `braq.read_iter` [here](https://github.com/pyrustic/braq/
+blob/master/docs/api/modules/braq/__init__/funcs.md#read_iter). ## Render a
+document Rendering a document involves transforming Python objects representing
+sections into Braq text which is a string that can be displayed on the screen
+or stored in a file. The library exposes the `render` function which accepts as
+input a sequence of sections (either header-body tuples or `Section` objects)
+and returns a Braq document. ```python import braq # sections section_1 =
+braq.Section("section 1", "line a\nline b") section_2 = "section 2", "line
+c\nline d" section_3 = "section 3", ("line e", "line f") # rendering r =
+braq.render(section_1, section_2, section_3) print(r) ``` Output: ```text
+[section 1] line a line b [section 2] line c line d [section 3] line e line f
+``` > The `render` function also accepts the `spacing` argument which defaults
+to 1 and represents the number of lines of spacing between two adjacent
+sections. > Check out the API reference for `braq.render` [here](https://
+github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/
+funcs.md#render). ## Write to file Following is a snippet for writting a Braq
 document to a file: ```python import braq # sections section_1 = braq.Section
 ("", "welcome") section_2 = braq.Section("section 2") section_3 = "section 3",
 ("line a", "line b") # path to file path = "/home/alex/braqfile.txt" # write to
 file r = braq.write(section_1, section_2, section_3, dest=path) ``` The
 contents of the Braq file: ```text welcome [section 2] [section 3] line a line
-b ``` > Check out the documentation for `braq.write` [here](https://github.com/
-pyrustic/braq/blob/master/docs/README.md).
+b ``` > Check out the API reference for `braq.write` [here](https://github.com/
+pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#write).
                                                                     _B_a_c_k_ _t_o_ _t_o_p
 # Braq schema for data validation Dict sections can be validated against a Braq
 schema. A Braq schema is a Python dictionary object that can be passed to a
 `Document` or a `FileDoc`. The keys of this dictionary are the headers of dict
 sections to validate and the values are [Paradict](https://github.com/pyrustic/
 paradict) schemas. A Paradict schema is a dictionary containing specs for data
 validation. A spec is either simply a string that represents an expected data
@@ -241,17 +253,17 @@
 and then returns a boolean to indicate whether this line is a header or not.
 ```python import braq line_1 = "[my header]" line_2 = "[this isn't a header] at
 all" assert braq.check_header(line_1) is True assert braq.check_header(line_2)
 is False ``` The `get_header` function accepts a line of text as input and
 returns a string if the line is a header. Otherwise, `None` is returned.
 ```python import braq line_1 = "[my header]" line_2 = "[this isn't a header] at
 all" assert braq.get_header(line_1) == "my header" assert braq.get_header
-(line_2) is None ``` > Check out the documentation for `braq.check_header` and
-`braq.get_header` [here](https://github.com/pyrustic/braq/blob/master/docs/
-README.md).
+(line_2) is None ``` > Check out the API reference for `braq.check_header` and
+`braq.get_header` [here](https://github.com/pyrustic/braq/blob/master/docs/api/
+modules/braq/__init__/funcs.md#check_header).
                                                                     _B_a_c_k_ _t_o_ _t_o_p
 # Miscellaneous Collection of miscellaneous notes. ## Cover image The beautiful
 cover image is generated with [Carbon](https://carbon.now.sh/about).
                                                                     _B_a_c_k_ _t_o_ _t_o_p
 # Testing and contributing Feel free to **open an issue** to report a bug,
 suggest some changes, show some useful code snippets, or discuss anything
 related to this project. You can also directly email [me](https://
```

### Comparing `braq-0.0.5/braq/__init__.py` & `braq-0.0.6/braq/__init__.py`

 * *Files identical despite different names*

### Comparing `braq-0.0.5/braq/document/__init__.py` & `braq-0.0.6/braq/document/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Braq Document class"""
 from paradict.typeref import TypeRef
 from paradict import validator, encode, decode, CONFIG_MODE
 import braq
 from braq import errors
 
 
+__all__ = ["Document"]
+
+
 class Document:
     """This class represents an editable model of a Braq document"""
     def __init__(self, init_text="", *, schema=None,
                  type_ref=None, obj_builder=None,
                  spacing=1, encoding_mode=CONFIG_MODE):
         """
         Init
 
-        [parameters]
+        [param]
         - init_text: Braq text for initializing the model
         - schema: a Python dict that serves as schema to validate the sections
         of the document. It is a dictionary of dictionaries, with root keys
         representing a section header.
         - type_ref: optional TypeRef object
         - obj_builder: function that accepts a paradict.box.Obj container and
         returns a fresh new Python object
@@ -72,42 +75,42 @@
     def type_ref(self, val):
         self._type_ref = val if val else TypeRef()
 
     def get(self, header):
         """
         Get the textual body of the section whose header is provided
 
-        [parameters]
+        [param]
         - header: the header (str) of the section
 
         [return]
         Return a string or None if this section doesn't exist
         """
         return self._sections.get(header)
 
     def get_lines(self, header):
         """
         Get the body lines of the section whose header is provided
 
-        [parameters]
+        [param]
         - header: the header (str) of the section
 
         [return]
         Return a list of strings or None if this section doesn't exist
         """
         body = self._sections.get(header)
         if body is None:
             return
         return body.splitlines(keepends=False)
 
     def set(self, header, body):
         """
         Create or update a section by providing its header and the body
 
-        [parameters]
+        [param]
         - header: the header (str) of the section
         - body: the body of the section, either a string or a list of string (lines)
 
         [return]
         Return the body as a string
         """
         if not isinstance(body, str):
@@ -115,15 +118,15 @@
         self._sections[header] = body.rstrip()
         return body
 
     def build(self, header, skip_comments=True):
         """
         Decode and return the section whose header is provided
 
-        [parameters]
+        [param]
         - header: the string header of the section
         - skip_comments: boolean to tell whether comments should be ignored or not
 
         [return]
         Return the body as a Python dictionary built with Paradict
         """
         body = self._sections.get(header)
@@ -133,15 +136,15 @@
                       skip_comments=skip_comments,
                       type_ref=self._type_ref)
         return body
 
     def build_config(self, *headers, skip_comments=True, on_error=None):
         """Build a configuration dictionary from the document and return it
 
-        [parameters]
+        [param]
         - *headers: Headers of sections meant to be part of the config.
         Not providing headers implies that the entire document can be treated as config data
         - skip_comments: boolean to tell whether comments should be ignored or not
         - on_error: callback called when an exception is raised while converting a section into
         a dict with Paradict. The callback must accept two arguments which are the header and
         the exception object
 
@@ -181,15 +184,15 @@
         return tuple(self._sections.keys())
 
     def render(self, *headers):
         """
         Render the entire document or a specific set of sections, i.e.,
         return a textual Paradict string that may be stored in a file.
 
-        [parameters]
+        [param]
         - *headers: Headers of sections to render.
         Omitting this will render the entire document
 
         [return]
         Returns a string that contains sections (each made of square-brackets delimited header
         and the associated body)
         """
@@ -206,29 +209,29 @@
             sections.append((header, self._sections.get(header)))
         return braq.render(*sections, spacing=self._spacing)
 
     def load_schema(self, src):
         """
         Load a schema file
 
-        [parameters]
+        [param]
         - src: either a path, a pathlib.Path object, or a file like object
         """
         r = braq.read(src)
         self._schema = dict()
         for header, body in r.items():
             body = decode(body, type_ref=self._type_ref, obj_builder=self._obj_builder,
                           skip_comments=True)
             self._schema[header] = body
 
     def validate(self, *headers):
         """
         Validate this entire document or only specific section(s)
 
-        [parameters]
+        [param]
         - *headers: headers to validate. If you ignore this parameter, the entire document will
         be checked against the schema.
 
         [return]
         Return true if the document is valid. Raise an exception if the schema is missing
         """
         if self._schema is None:
@@ -251,30 +254,30 @@
         a path string or pathlib.Path object"""
         self._sections = braq.read(path)
 
     def save_to(self, path):
         """
         Save the contents of this document to a specific file
 
-        [parameters]
+        [param]
         - path: path to filename. Path may be a pathlib.Path instance
         """
         if not path:
             return False
         sections = list()
         for header, body in self._sections.items():
             sections.append((header, body))
         braq.write(*sections, dst=path, spacing=self._spacing)
         return True
 
     def remove(self, *headers):
         """
         Remove specific section(s) from this document
 
-        [parameters]
+        [param]
         - *headers: the headers of the sections to remove
         """
         for header in headers:
             try:
                 del self._sections[header]
             except KeyError as e:
                 pass
```

### Comparing `braq-0.0.5/braq/filedoc/__init__.py` & `braq-0.0.6/braq/filedoc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 import os.path
 import braq
 from contextlib import contextmanager
 from braq.document import Document
 from paradict import CONFIG_MODE
 
 
+__all__ = ["FileDoc"]
+
+
 class FileDoc(Document):
     """File-based Braq document"""
     def __init__(self, path, *, autosave=True, schema=None,
                  type_ref=None, obj_builder=None,
                  lazy_loading=True, spacing=1,
                  encoding_mode=CONFIG_MODE):
         """
         Init
 
-        [parameters]
+        [param]
         - path: path string or a pathlib.Path instance
         - autosave: bool to tell whether data should be saved to disk right after modification
         - schema: a Python dict that serves as schema to validate the sections
         of the document. It is a dictionary of dictionaries, with root keys
         representing a section header.
         - type_ref: optional TypeRef object
         - obj_builder: function that accepts a paradict.box.Obj container and
@@ -70,15 +73,15 @@
         if self._autosave:
             self.save()
 
     def build(self, header, skip_comments=True):
         """
         Decode and return the section whose header is provided
 
-        [parameters]
+        [param]
         - header: the string header of the section
         - skip_comments: boolean to tell whether comments should be ignored or not
         """
         self._ensure_sections()
         return super().build(header, skip_comments=skip_comments)
 
     def build_config(self, *headers, skip_comments=True, on_error=None):
@@ -117,15 +120,15 @@
         return super().list_headers()
 
     def render(self, *headers):
         """
         Render the entire document or a specific set of sections, i.e.,
         return a textual Paradict string that may be stored in a file.
 
-        [parameters]
+        [param]
         - *headers: Headers of sections to render.
         Omitting this will render the entire document
 
         [return]
         Returns a string that contains sections (each made of square-brackets delimited header
         and the associated body)
         """
```

### Comparing `braq-0.0.5/braq/fileio/__init__.py` & `braq-0.0.6/braq/fileio/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import pathlib
 import written
 from braq.section import render
 from braq.parser import parse_iter
 
 
+__all__ = ["read_iter", "read", "write"]
+
+
 def read_iter(filename, end_of_stream=None):
     """
     Iteratively read a file. This generator yields a 2-tuple made
     of a header string and an iterator to iterate over the body line by line.
 
-    [parameters]
+    [param]
     - filename: is either a path string, a pathlib.Path instance, or a file object which
     might expose binary text encoded with UTF-8
     - end_of_stream: string to indicate the end of the stream
 
     [return]
     Yields a 2-tuple made of a header string and a body iterator to iterate
     over the body line by line
@@ -35,15 +38,15 @@
         yield from parse_iter(filename, end_of_stream=end_of_stream)
 
 
 def read(filename, end_of_stream=None):
     """
     Read a file then flatten its contents (concatenate sections with same header).
 
-    [parameters]
+    [param]
     - filename: is either a path string, a pathlib.Path instance, or a file object which
     might expose binary text encoded with UTF-8
     - end_of_stream: string to indicate the end of the stream
 
     [return]
     returns the dict of sections where keys are headers and
     values are section's bodies. A section body is a text string"""
@@ -57,14 +60,14 @@
     return sections
 
 
 def write(*sections, dst=None, spacing=1):
     """
     Write to a file
 
-    [parameters]
+    [param]
     - *sections: sections objects or header-body 2-tuples
     - dst: is either a path string, a pathlib.Path instance
     - spacing: number of lines between two sections, defaults to 1
     """
     r = render(*sections, spacing=spacing)
     written.write(r, dst)
```

### Comparing `braq-0.0.5/braq/parser/__init__.py` & `braq-0.0.6/braq/parser/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from braq import misc
 
 
+__all__ = ["parse_iter", "parse", "Parser", "check_header", "get_header"]
+
+
 def parse_iter(stream, end_of_stream=None):
     """
     Iteratively parse a stream
 
-    [parameters]
+    [param]
     - stream: either a text string, UTF-8 binary, a sequence of or an iterator of lines
     - end_of_stream: string representing the end of stream
 
     [return]
     Yield header and body for each section until end of stream.
     The header is a string and the body is an iterator that yield each line (string)
     of the body.
@@ -26,15 +29,15 @@
     yield from parser.parse(stream)
 
 
 def parse(stream, end_of_stream=None):
     """
     Parse and flatten a Braq text stream
 
-    [parameters]
+    [param]
     - stream: either a text string, UTF-8 binary, a sequence of or an iterator of lines
     - end_of_stream: string representing the end of stream
 
     [return]
     Returns the dict of sections (keys are headers and
     values are section's bodies. a section body is a text string
     """
@@ -66,15 +69,15 @@
     def end_of_stream(self, val):
         self._end_of_stream = val
 
     def parse(self, stream):
         """
         Iteratively parse a stream
 
-        [parameters]
+        [param]
         - stream: iterator, sequence of lines, text string or UTF-8 encoded binary
 
         [return]
         Yield header and body for each section until end of stream.
         The header is a string and the body is an iterator that yield each line (string)
         of the body.
```

### Comparing `braq-0.0.5/braq/section/__init__.py` & `braq-0.0.6/braq/section/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 
+__all__ = ["Section", "render"]
+
 
 class Section:
 
     def __init__(self, header, body=None):
         """
         Init
 
-        [parameters]
+        [param]
         - header: the header (str) of the section
         - body: the body of the section, either a string or a list of string (lines)
         """
         self._header = header
         self._body = _ensure_body(body)
 
     @property
@@ -51,15 +53,15 @@
     
 
 def render(*sections, spacing=1):
     """
     Render sections, i.e., transform the sequence of sections
     into a Braq text document (string)
 
-    [parameters]
+    [param]
     - sections: Section objects or header-body tuples.
     Note that a body is either a text string or a sequence of lines
     - spacing: number of empty lines between two sections, defaults to 1
 
     [return]
     A string representing a Braq text document
     """
```

### Comparing `braq-0.0.5/braq.egg-info/PKG-INFO` & `braq-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: braq
-Version: 0.0.5
-Summary: Customizable data format for config files, AI prompts, and more
-Home-page: https://github.com/pyrustic/braq
-Author: Pyrustic Evangelist
-Author-email: rusticalex@yahoo.com
-Maintainer: Pyrustic Evangelist
-Maintainer-email: rusticalex@yahoo.com
-License: MIT
-Keywords: data-format,config,configuration,configfile,config-files,customizable,versatile,ai-prompts,pyrustic
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI package version](https://img.shields.io/pypi/v/braq)](https://pypi.org/project/braq)
 [![Downloads](https://static.pepy.tech/badge/braq)](https://pepy.tech/project/braq)
 
 <!-- Cover -->
 <div align="center">
     <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/braq/cover.png" alt="Cover image" width="650">
@@ -329,15 +310,15 @@
 # beware, the 'validate' method may raise an exception
 # for good reasons !
 ```
 
 > There is more to discover about the `Document` class, such as the `clear`, `remove`, and `render` methods, exposed properties, and more.
 
 
-> Check out the documentation for `braq.Document` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.Document` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/class-Document.md).
 
 
 ## File document class
 The `FileDoc` class is based on the **Document** class and focuses specifically on documents with associated disk files such as **config files**.
 
 > As with the `Document` class, a schema can be passed to a `FileDoc` instance to validate dict sections.
 
@@ -367,15 +348,15 @@
     # perform several changes here !
     # ...
     confile.embed("gui", {"color": "blue"})
 ```
 
 > There is more to discover about the **FileDoc** class, such as the `load`, `save`, and `save_to` methods, exposed properties, and more.
 
-> Check out the documentation for `braq.FileDoc` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.FileDoc` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/class-FileDoc.md).
 
 <p align="right"><a href="#readme">Back to top</a></p>
 
 # Section class
 The `Section` class is an abstraction representing a Braq section. It exposes the `header` and `body` properties and renders itself when its `__str__` method is called implicitly.
 
 ```python
@@ -421,15 +402,15 @@
 
 # check headers
 assert tuple(d.keys()) == ("", "section 1")
 # check the body of 'section 1'
 assert d["section 1"] == "this is section 1"
 ```
 
-> Check out the documentation for `braq.parse` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.parse` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#parse).
 
 ## Parse a document iteratively
 A document can be parsed line by line as following:
 
 ```python
 import braq
 
@@ -452,15 +433,15 @@
 this is the unnamed section
 
 [section 1]
 this is section 1
 ```
 
 
-> Check out the documentation for `braq.parse_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.parse_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#parse_iter).
 
 ## Read a file
 The library exposes the `read` function which takes as input the path to a file to parse, then returns a dictionary whose keys and values are strings representing headers and bodies respectively.
 
 > Sections sharing the same header are concatenated !
 
 ```python
@@ -468,15 +449,15 @@
 
 path = "/home/alex/braqfile.txt"
 
 r = braq.read(path)
 assert tuple(r.keys()) == ("", "section 1")
 ```
 
-> Check out the documentation for `braq.read` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.read` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#read).
 
 ## Read a file iteratively
 A large text file can be parsed line by line as following:
 
 ```python
 import braq
 
@@ -493,15 +474,15 @@
 ```text
 this is the unnamed section
 
 [section 1]
 this is section 1
 ```
 
-> Check out the documentation for `braq.read_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.read_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#read_iter).
 
 ## Render a document
 Rendering a document involves transforming Python objects representing sections into Braq text which is a string that can be displayed on the screen or stored in a file.
 
 The library exposes the `render` function which accepts as input a sequence of sections (either header-body tuples or `Section` objects) and returns a Braq document.
 
 ```python
@@ -533,15 +514,15 @@
 line e
 line f
 ```
 
 > The `render` function also accepts the `spacing` argument which defaults to 1 and represents the number of lines of spacing between two adjacent sections.
 
 
-> Check out the documentation for `braq.render` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.render` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#render).
 
 ## Write to file
 Following is a snippet for writting a Braq document to a file:
 
 ```python
 import braq
 
@@ -563,15 +544,15 @@
 
 [section 3]
 line a
 line b
 ```
 
 
-> Check out the documentation for `braq.write` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.write` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#write).
 
 
 <p align="right"><a href="#readme">Back to top</a></p>
 
 # Braq schema for data validation
 Dict sections can be validated against a Braq schema. A Braq schema is a Python dictionary object that can be passed to a `Document` or a `FileDoc`. The keys of this dictionary are the headers of dict sections to validate and the values are [Paradict](https://github.com/pyrustic/paradict) schemas.
 
@@ -632,15 +613,15 @@
 
 line_1 = "[my header]"
 line_2 = "[this isn't a header] at all"
 assert braq.get_header(line_1) == "my header"
 assert braq.get_header(line_2) is None
 ```
 
-> Check out the documentation for `braq.check_header` and `braq.get_header` [here](https://github.com/pyrustic/braq/blob/master/docs/README.md).
+> Check out the API reference for `braq.check_header` and `braq.get_header` [here](https://github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#check_header).
 
 <p align="right"><a href="#readme">Back to top</a></p>
 
 # Miscellaneous
 Collection of miscellaneous notes.
 
 ## Cover image
@@ -706,9 +687,7 @@
 Hello world, I'm Alex, a tech enthusiast ! Feel free to get in touch with [me](https://pyrustic.github.io/#contact) !
 
 <br>
 <br>
 <br>
 
 [Back to top](#readme)
-
-
```

#### html2text {}

```diff
@@ -1,20 +1,11 @@
-Metadata-Version: 2.1 Name: braq Version: 0.0.5 Summary: Customizable data
-format for config files, AI prompts, and more Home-page: https://github.com/
-pyrustic/braq Author: Pyrustic Evangelist Author-email: rusticalex@yahoo.com
-Maintainer: Pyrustic Evangelist Maintainer-email: rusticalex@yahoo.com License:
-MIT Keywords: data-format,config,configuration,configfile,config-
-files,customizable,versatile,ai-prompts,pyrustic Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.5
-Description-Content-Type: text/markdown License-File: LICENSE [![License: MIT]
-(https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/
-licenses/MIT) [![PyPI package version](https://img.shields.io/pypi/v/braq)]
-(https://pypi.org/project/braq) [![Downloads](https://static.pepy.tech/badge/
-braq)](https://pepy.tech/project/braq)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
+opensource.org/licenses/MIT) [![PyPI package version](https://img.shields.io/
+pypi/v/braq)](https://pypi.org/project/braq) [![Downloads](https://
+static.pepy.tech/badge/braq)](https://pepy.tech/project/braq)
                                  [Cover image]
                          Braq document with 3 sections
 # Braq CCuussttoommiizzaabbllee ddaattaa ffoorrmmaatt ffoorr ccoonnffiigg ffiilleess,, AAII pprroommppttss,, aanndd mmoorree This
 project is part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
 ## Table of contents - [Overview](#overview) - [Data format specification]
 (#data-format-specification) - [Notable use cases](#notable-use-cases) -
 [Config files](#config-files) - [AI prompts](#ai-prompts) - [Source code
@@ -144,32 +135,33 @@
 section server_conf = {"ip-address": "127.0.0.1", "port": 80} document.embed
 ("server", server_conf) # list headers assert document.list_headers() == ("",
 "user", "server") # validate specific dict sections # (no args implies that the
 entire doc will be the target) document.validate("user", "server") # returns a
 bool # beware, the 'validate' method may raise an exception # for good reasons
 ! ``` > There is more to discover about the `Document` class, such as the
 `clear`, `remove`, and `render` methods, exposed properties, and more. > Check
-out the documentation for `braq.Document` [here](https://github.com/pyrustic/
-braq/blob/master/docs/README.md). ## File document class The `FileDoc` class is
-based on the **Document** class and focuses specifically on documents with
-associated disk files such as **config files**. > As with the `Document` class,
-a schema can be passed to a `FileDoc` instance to validate dict sections.
-```python from braq import FileDoc confile = FileDoc("config-file.braq") #
-build the 'user' section user = confile.build("user") # test assert user ==
-{"id": 42, "name": "alex"} # retrieve the unnamed section as a text text =
-confile.get("") # notice the empty header str # retrieve the 'user' dict
-section as a text text = confile.get("user") # embed a 'server' dict section
-server_conf = {"ip-address": "127.0.0.1", "port": 80} confile.embed("server",
-server_conf) # change persisted # batch edit mode (changes are persisted at the
-end) with confile.edit_model(): # by default, autosave==True # perform several
-changes here ! # ... confile.embed("gui", {"color": "blue"}) ``` > There is
-more to discover about the **FileDoc** class, such as the `load`, `save`, and
-`save_to` methods, exposed properties, and more. > Check out the documentation
-for `braq.FileDoc` [here](https://github.com/pyrustic/braq/blob/master/docs/
-README.md).
+out the API reference for `braq.Document` [here](https://github.com/pyrustic/
+braq/blob/master/docs/api/modules/braq/__init__/class-Document.md). ## File
+document class The `FileDoc` class is based on the **Document** class and
+focuses specifically on documents with associated disk files such as **config
+files**. > As with the `Document` class, a schema can be passed to a `FileDoc`
+instance to validate dict sections. ```python from braq import FileDoc confile
+= FileDoc("config-file.braq") # build the 'user' section user = confile.build
+("user") # test assert user == {"id": 42, "name": "alex"} # retrieve the
+unnamed section as a text text = confile.get("") # notice the empty header str
+# retrieve the 'user' dict section as a text text = confile.get("user") # embed
+a 'server' dict section server_conf = {"ip-address": "127.0.0.1", "port": 80}
+confile.embed("server", server_conf) # change persisted # batch edit mode
+(changes are persisted at the end) with confile.edit_model(): # by default,
+autosave==True # perform several changes here ! # ... confile.embed("gui",
+{"color": "blue"}) ``` > There is more to discover about the **FileDoc** class,
+such as the `load`, `save`, and `save_to` methods, exposed properties, and
+more. > Check out the API reference for `braq.FileDoc` [here](https://
+github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/class-
+FileDoc.md).
                                                                     _B_a_c_k_ _t_o_ _t_o_p
 # Section class The `Section` class is an abstraction representing a Braq
 section. It exposes the `header` and `body` properties and renders itself when
 its `__str__` method is called implicitly. ```python import braq # create a
 Section object header, body = "my header", ("line a", "line b") section =
 braq.Section(header, body) # test the properties assert section.header == "my
 header" assert section.body == "line a\nline b" # test the rendering assert str
@@ -183,55 +175,57 @@
 parsed, then returns a **dictionary** whose keys and values are strings
 representing headers and bodies respectively. > Sections sharing the same
 header are concatenated ! > The header of an unnamed section is an empty
 string. ```python import braq text = """\ this is the unnamed section at the
 top of this document... [section 1] this is section 1""" d = braq.parse(text) #
 check headers assert tuple(d.keys()) == ("", "section 1") # check the body of
 'section 1' assert d["section 1"] == "this is section 1" ``` > Check out the
-documentation for `braq.parse` [here](https://github.com/pyrustic/braq/blob/
-master/docs/README.md). ## Parse a document iteratively A document can be
-parsed line by line as following: ```python import braq text = """\ this is the
-unnamed section [section 1] this is section 1""" for header, body in
-braq.parse_iter(text): if header: print("[" + header + "]") for line in body:
-print(line) ``` Output: ```text this is the unnamed section [section 1] this is
-section 1 ``` > Check out the documentation for `braq.parse_iter` [here](https:
-//github.com/pyrustic/braq/blob/master/docs/README.md). ## Read a file The
-library exposes the `read` function which takes as input the path to a file to
-parse, then returns a dictionary whose keys and values are strings representing
-headers and bodies respectively. > Sections sharing the same header are
-concatenated ! ```python import braq path = "/home/alex/braqfile.txt" r =
-braq.read(path) assert tuple(r.keys()) == ("", "section 1") ``` > Check out the
-documentation for `braq.read` [here](https://github.com/pyrustic/braq/blob/
-master/docs/README.md). ## Read a file iteratively A large text file can be
-parsed line by line as following: ```python import braq path = "/home/alex/
-braqfile.txt" for header, body in braq.read_iter(path): if header: print("[" +
-header + "]") for line in body: print(line) ``` Output: ```text this is the
-unnamed section [section 1] this is section 1 ``` > Check out the documentation
-for `braq.read_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/
-README.md). ## Render a document Rendering a document involves transforming
-Python objects representing sections into Braq text which is a string that can
-be displayed on the screen or stored in a file. The library exposes the
-`render` function which accepts as input a sequence of sections (either header-
-body tuples or `Section` objects) and returns a Braq document. ```python import
-braq # sections section_1 = braq.Section("section 1", "line a\nline b")
-section_2 = "section 2", "line c\nline d" section_3 = "section 3", ("line e",
-"line f") # rendering r = braq.render(section_1, section_2, section_3) print(r)
-``` Output: ```text [section 1] line a line b [section 2] line c line d
-[section 3] line e line f ``` > The `render` function also accepts the
-`spacing` argument which defaults to 1 and represents the number of lines of
-spacing between two adjacent sections. > Check out the documentation for
-`braq.render` [here](https://github.com/pyrustic/braq/blob/master/docs/
-README.md). ## Write to file Following is a snippet for writting a Braq
+API reference for `braq.parse` [here](https://github.com/pyrustic/braq/blob/
+master/docs/api/modules/braq/__init__/funcs.md#parse). ## Parse a document
+iteratively A document can be parsed line by line as following: ```python
+import braq text = """\ this is the unnamed section [section 1] this is section
+1""" for header, body in braq.parse_iter(text): if header: print("[" + header +
+"]") for line in body: print(line) ``` Output: ```text this is the unnamed
+section [section 1] this is section 1 ``` > Check out the API reference for
+`braq.parse_iter` [here](https://github.com/pyrustic/braq/blob/master/docs/api/
+modules/braq/__init__/funcs.md#parse_iter). ## Read a file The library exposes
+the `read` function which takes as input the path to a file to parse, then
+returns a dictionary whose keys and values are strings representing headers and
+bodies respectively. > Sections sharing the same header are concatenated !
+```python import braq path = "/home/alex/braqfile.txt" r = braq.read(path)
+assert tuple(r.keys()) == ("", "section 1") ``` > Check out the API reference
+for `braq.read` [here](https://github.com/pyrustic/braq/blob/master/docs/api/
+modules/braq/__init__/funcs.md#read). ## Read a file iteratively A large text
+file can be parsed line by line as following: ```python import braq path = "/
+home/alex/braqfile.txt" for header, body in braq.read_iter(path): if header:
+print("[" + header + "]") for line in body: print(line) ``` Output: ```text
+this is the unnamed section [section 1] this is section 1 ``` > Check out the
+API reference for `braq.read_iter` [here](https://github.com/pyrustic/braq/
+blob/master/docs/api/modules/braq/__init__/funcs.md#read_iter). ## Render a
+document Rendering a document involves transforming Python objects representing
+sections into Braq text which is a string that can be displayed on the screen
+or stored in a file. The library exposes the `render` function which accepts as
+input a sequence of sections (either header-body tuples or `Section` objects)
+and returns a Braq document. ```python import braq # sections section_1 =
+braq.Section("section 1", "line a\nline b") section_2 = "section 2", "line
+c\nline d" section_3 = "section 3", ("line e", "line f") # rendering r =
+braq.render(section_1, section_2, section_3) print(r) ``` Output: ```text
+[section 1] line a line b [section 2] line c line d [section 3] line e line f
+``` > The `render` function also accepts the `spacing` argument which defaults
+to 1 and represents the number of lines of spacing between two adjacent
+sections. > Check out the API reference for `braq.render` [here](https://
+github.com/pyrustic/braq/blob/master/docs/api/modules/braq/__init__/
+funcs.md#render). ## Write to file Following is a snippet for writting a Braq
 document to a file: ```python import braq # sections section_1 = braq.Section
 ("", "welcome") section_2 = braq.Section("section 2") section_3 = "section 3",
 ("line a", "line b") # path to file path = "/home/alex/braqfile.txt" # write to
 file r = braq.write(section_1, section_2, section_3, dest=path) ``` The
 contents of the Braq file: ```text welcome [section 2] [section 3] line a line
-b ``` > Check out the documentation for `braq.write` [here](https://github.com/
-pyrustic/braq/blob/master/docs/README.md).
+b ``` > Check out the API reference for `braq.write` [here](https://github.com/
+pyrustic/braq/blob/master/docs/api/modules/braq/__init__/funcs.md#write).
                                                                     _B_a_c_k_ _t_o_ _t_o_p
 # Braq schema for data validation Dict sections can be validated against a Braq
 schema. A Braq schema is a Python dictionary object that can be passed to a
 `Document` or a `FileDoc`. The keys of this dictionary are the headers of dict
 sections to validate and the values are [Paradict](https://github.com/pyrustic/
 paradict) schemas. A Paradict schema is a dictionary containing specs for data
 validation. A spec is either simply a string that represents an expected data
@@ -250,17 +244,17 @@
 and then returns a boolean to indicate whether this line is a header or not.
 ```python import braq line_1 = "[my header]" line_2 = "[this isn't a header] at
 all" assert braq.check_header(line_1) is True assert braq.check_header(line_2)
 is False ``` The `get_header` function accepts a line of text as input and
 returns a string if the line is a header. Otherwise, `None` is returned.
 ```python import braq line_1 = "[my header]" line_2 = "[this isn't a header] at
 all" assert braq.get_header(line_1) == "my header" assert braq.get_header
-(line_2) is None ``` > Check out the documentation for `braq.check_header` and
-`braq.get_header` [here](https://github.com/pyrustic/braq/blob/master/docs/
-README.md).
+(line_2) is None ``` > Check out the API reference for `braq.check_header` and
+`braq.get_header` [here](https://github.com/pyrustic/braq/blob/master/docs/api/
+modules/braq/__init__/funcs.md#check_header).
                                                                     _B_a_c_k_ _t_o_ _t_o_p
 # Miscellaneous Collection of miscellaneous notes. ## Cover image The beautiful
 cover image is generated with [Carbon](https://carbon.now.sh/about).
                                                                     _B_a_c_k_ _t_o_ _t_o_p
 # Testing and contributing Feel free to **open an issue** to report a bug,
 suggest some changes, show some useful code snippets, or discuss anything
 related to this project. You can also directly email [me](https://
```

### Comparing `braq-0.0.5/braq.egg-info/SOURCES.txt` & `braq-0.0.6/braq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braq-0.0.5/setup.cfg` & `braq-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `braq-0.0.5/tests/test_document.py` & `braq-0.0.6/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `braq-0.0.5/tests/test_filedoc.py` & `braq-0.0.6/tests/test_filedoc.py`

 * *Files identical despite different names*

### Comparing `braq-0.0.5/tests/test_fileio.py` & `braq-0.0.6/tests/test_fileio.py`

 * *Files identical despite different names*

### Comparing `braq-0.0.5/tests/test_imports.py` & `braq-0.0.6/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `braq-0.0.5/tests/test_misc.py` & `braq-0.0.6/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `braq-0.0.5/tests/test_parser.py` & `braq-0.0.6/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `braq-0.0.5/tests/test_section.py` & `braq-0.0.6/tests/test_section.py`

 * *Files identical despite different names*

