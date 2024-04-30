# Comparing `tmp/finitelycomputable-helloworld-quart-flask-24.3.tar.gz` & `tmp/finitelycomputable_helloworld_quart_flask-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable-helloworld-quart-flask-24.3.tar", last modified: Mon Apr  1 03:34:46 2024, max compression
+gzip compressed data, was "finitelycomputable_helloworld_quart_flask-24.4.tar", last modified: Tue Apr 30 04:47:03 2024, max compression
```

## Comparing `finitelycomputable-helloworld-quart-flask-24.3.tar` & `finitelycomputable_helloworld_quart_flask-24.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:34:46.708893 finitelycomputable-helloworld-quart-flask-24.3/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1790 2024-04-01 03:34:46.708893 finitelycomputable-helloworld-quart-flask-24.3/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      250 2024-01-20 16:29:52.000000 finitelycomputable-helloworld-quart-flask-24.3/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:34:46.708893 finitelycomputable-helloworld-quart-flask-24.3/finitelycomputable/
--rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      922 2024-03-02 07:07:20.000000 finitelycomputable-helloworld-quart-flask-24.3/finitelycomputable/helloworld_quart.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:34:46.708893 finitelycomputable-helloworld-quart-flask-24.3/finitelycomputable_helloworld_quart_flask.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1790 2024-04-01 03:34:46.000000 finitelycomputable-helloworld-quart-flask-24.3/finitelycomputable_helloworld_quart_flask.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      497 2024-04-01 03:34:46.000000 finitelycomputable-helloworld-quart-flask-24.3/finitelycomputable_helloworld_quart_flask.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-01 03:34:46.000000 finitelycomputable-helloworld-quart-flask-24.3/finitelycomputable_helloworld_quart_flask.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       96 2024-04-01 03:34:46.000000 finitelycomputable-helloworld-quart-flask-24.3/finitelycomputable_helloworld_quart_flask.egg-info/entry_points.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       54 2024-04-01 03:34:46.000000 finitelycomputable-helloworld-quart-flask-24.3/finitelycomputable_helloworld_quart_flask.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-01 03:34:46.000000 finitelycomputable-helloworld-quart-flask-24.3/finitelycomputable_helloworld_quart_flask.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1563 2024-03-16 18:34:55.000000 finitelycomputable-helloworld-quart-flask-24.3/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-01 03:34:46.708893 finitelycomputable-helloworld-quart-flask-24.3/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:03.515783 finitelycomputable_helloworld_quart_flask-24.4/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1848 2024-04-30 04:47:03.515783 finitelycomputable_helloworld_quart_flask-24.4/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      250 2024-01-20 16:29:52.000000 finitelycomputable_helloworld_quart_flask-24.4/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:03.515783 finitelycomputable_helloworld_quart_flask-24.4/finitelycomputable/
+-rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      922 2024-03-02 07:07:20.000000 finitelycomputable_helloworld_quart_flask-24.4/finitelycomputable/helloworld_quart.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:03.515783 finitelycomputable_helloworld_quart_flask-24.4/finitelycomputable/tests/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      783 2024-04-30 03:36:52.000000 finitelycomputable_helloworld_quart_flask-24.4/finitelycomputable/tests/test_helloworld_quart.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:03.515783 finitelycomputable_helloworld_quart_flask-24.4/finitelycomputable_helloworld_quart_flask.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1848 2024-04-30 04:47:03.000000 finitelycomputable_helloworld_quart_flask-24.4/finitelycomputable_helloworld_quart_flask.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      547 2024-04-30 04:47:03.000000 finitelycomputable_helloworld_quart_flask-24.4/finitelycomputable_helloworld_quart_flask.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:47:03.000000 finitelycomputable_helloworld_quart_flask-24.4/finitelycomputable_helloworld_quart_flask.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       96 2024-04-30 04:47:03.000000 finitelycomputable_helloworld_quart_flask-24.4/finitelycomputable_helloworld_quart_flask.egg-info/entry_points.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       79 2024-04-30 04:47:03.000000 finitelycomputable_helloworld_quart_flask-24.4/finitelycomputable_helloworld_quart_flask.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:47:03.000000 finitelycomputable_helloworld_quart_flask-24.4/finitelycomputable_helloworld_quart_flask.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1591 2024-04-28 21:51:18.000000 finitelycomputable_helloworld_quart_flask-24.4/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:47:03.515783 finitelycomputable_helloworld_quart_flask-24.4/setup.cfg
```

### Comparing `finitelycomputable-helloworld-quart-flask-24.3/PKG-INFO` & `finitelycomputable_helloworld_quart_flask-24.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-helloworld-quart-flask
-Version: 24.3
+Version: 24.4
 Summary: hello_world in Quart from an implementation in Flask
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/hello_world
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -26,14 +26,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: Quart~=0.19
 Provides-Extra: tests
 Requires-Dist: pytest-asyncio; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
+Requires-Dist: finitelycomputable-tests; extra == "tests"
 
 =======================
 HelloWorld-Quart-Flask
 =======================
 
 This application adapts the hello_world endpoint provided in
 finitelycomputable.helloworld_flask to be provided in
```

### Comparing `finitelycomputable-helloworld-quart-flask-24.3/finitelycomputable/helloworld_quart.py` & `finitelycomputable_helloworld_quart_flask-24.4/finitelycomputable/helloworld_quart.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-helloworld-quart-flask-24.3/finitelycomputable_helloworld_quart_flask.egg-info/PKG-INFO` & `finitelycomputable_helloworld_quart_flask-24.4/finitelycomputable_helloworld_quart_flask.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-helloworld-quart-flask
-Version: 24.3
+Version: 24.4
 Summary: hello_world in Quart from an implementation in Flask
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/hello_world
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -26,14 +26,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: Quart~=0.19
 Provides-Extra: tests
 Requires-Dist: pytest-asyncio; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
+Requires-Dist: finitelycomputable-tests; extra == "tests"
 
 =======================
 HelloWorld-Quart-Flask
 =======================
 
 This application adapts the hello_world endpoint provided in
 finitelycomputable.helloworld_flask to be provided in
```

### Comparing `finitelycomputable-helloworld-quart-flask-24.3/pyproject.toml` & `finitelycomputable_helloworld_quart_flask-24.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 authors = [{name = "Samuel Newbold", email = "sam@rwsh.org"}]
 license = {text = "AGPL-3.0-only"}
 readme = "README.rst"
-version = "24.3"
+version = "24.4"
 name = "finitelycomputable-helloworld-quart-flask"
 requires-python = ">=3.8"
 description = "hello_world in Quart from an implementation in Flask"
 dependencies = [
   "Quart~=0.19",
 ]
 classifiers = [
@@ -27,15 +27,15 @@
   "Programming Language :: Python :: 3.11",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 
 [project.optional-dependencies]
 tests = ["pytest-asyncio",
-  "pytest", "pytest-env"]
+  "pytest", "pytest-env", "finitelycomputable-tests"]
 
 [project.scripts]
 finitelycomputable-helloworld-quart = "finitelycomputable.helloworld_quart:run"
 
 [project.urls]
 Homepage = "https://www.finitelycomputable.net/hello_world"
 Documentation = "https://github.com/thrasymache/microsites"
```

