# Comparing `tmp/finitelycomputable-helloworld-flask-quart-24.3.tar.gz` & `tmp/finitelycomputable_helloworld_flask_quart-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable-helloworld-flask-quart-24.3.tar", last modified: Mon Apr  1 03:34:09 2024, max compression
+gzip compressed data, was "finitelycomputable_helloworld_flask_quart-24.4.tar", last modified: Tue Apr 30 04:46:18 2024, max compression
```

## Comparing `finitelycomputable-helloworld-flask-quart-24.3.tar` & `finitelycomputable_helloworld_flask_quart-24.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:34:09.276504 finitelycomputable-helloworld-flask-quart-24.3/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2190 2024-04-01 03:34:09.276504 finitelycomputable-helloworld-flask-quart-24.3/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      250 2024-01-20 16:29:50.000000 finitelycomputable-helloworld-flask-quart-24.3/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:34:09.276504 finitelycomputable-helloworld-flask-quart-24.3/finitelycomputable/
--rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      943 2024-03-02 07:05:01.000000 finitelycomputable-helloworld-flask-quart-24.3/finitelycomputable/helloworld_flask.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:34:09.276504 finitelycomputable-helloworld-flask-quart-24.3/finitelycomputable_helloworld_flask_quart.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2190 2024-04-01 03:34:09.000000 finitelycomputable-helloworld-flask-quart-24.3/finitelycomputable_helloworld_flask_quart.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      497 2024-04-01 03:34:09.000000 finitelycomputable-helloworld-flask-quart-24.3/finitelycomputable_helloworld_flask_quart.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-01 03:34:09.000000 finitelycomputable-helloworld-flask-quart-24.3/finitelycomputable_helloworld_flask_quart.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       96 2024-04-01 03:34:09.000000 finitelycomputable-helloworld-flask-quart-24.3/finitelycomputable_helloworld_flask_quart.egg-info/entry_points.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      164 2024-04-01 03:34:09.000000 finitelycomputable-helloworld-flask-quart-24.3/finitelycomputable_helloworld_flask_quart.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-01 03:34:09.000000 finitelycomputable-helloworld-flask-quart-24.3/finitelycomputable_helloworld_flask_quart.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1750 2024-03-16 18:34:55.000000 finitelycomputable-helloworld-flask-quart-24.3/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-01 03:34:09.276504 finitelycomputable-helloworld-flask-quart-24.3/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:46:18.819579 finitelycomputable_helloworld_flask_quart-24.4/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2248 2024-04-30 04:46:18.819579 finitelycomputable_helloworld_flask_quart-24.4/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      250 2024-01-20 16:29:50.000000 finitelycomputable_helloworld_flask_quart-24.4/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:46:18.815579 finitelycomputable_helloworld_flask_quart-24.4/finitelycomputable/
+-rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      943 2024-03-02 07:05:01.000000 finitelycomputable_helloworld_flask_quart-24.4/finitelycomputable/helloworld_flask.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:46:18.815579 finitelycomputable_helloworld_flask_quart-24.4/finitelycomputable/tests/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      757 2024-04-30 03:36:39.000000 finitelycomputable_helloworld_flask_quart-24.4/finitelycomputable/tests/test_helloworld_flask.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:46:18.815579 finitelycomputable_helloworld_flask_quart-24.4/finitelycomputable_helloworld_flask_quart.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2248 2024-04-30 04:46:18.000000 finitelycomputable_helloworld_flask_quart-24.4/finitelycomputable_helloworld_flask_quart.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      547 2024-04-30 04:46:18.000000 finitelycomputable_helloworld_flask_quart-24.4/finitelycomputable_helloworld_flask_quart.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:46:18.000000 finitelycomputable_helloworld_flask_quart-24.4/finitelycomputable_helloworld_flask_quart.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       96 2024-04-30 04:46:18.000000 finitelycomputable_helloworld_flask_quart-24.4/finitelycomputable_helloworld_flask_quart.egg-info/entry_points.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      189 2024-04-30 04:46:18.000000 finitelycomputable_helloworld_flask_quart-24.4/finitelycomputable_helloworld_flask_quart.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:46:18.000000 finitelycomputable_helloworld_flask_quart-24.4/finitelycomputable_helloworld_flask_quart.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1778 2024-04-28 21:51:18.000000 finitelycomputable_helloworld_flask_quart-24.4/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:46:18.819579 finitelycomputable_helloworld_flask_quart-24.4/setup.cfg
```

### Comparing `finitelycomputable-helloworld-flask-quart-24.3/PKG-INFO` & `finitelycomputable_helloworld_flask_quart-24.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-helloworld-flask-quart
-Version: 24.3
+Version: 24.4
 Summary: hello_world in Flask from an implementation in Quart
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/hello_world
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -27,14 +27,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: Flask~=3.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
+Requires-Dist: finitelycomputable-tests; extra == "tests"
 Provides-Extra: waitress
 Requires-Dist: waitress~=2.1; extra == "waitress"
 Provides-Extra: cherrypy
 Requires-Dist: cherrypy~=18.0; extra == "cherrypy"
 Provides-Extra: cheroot
 Requires-Dist: cheroot~=9.0; extra == "cheroot"
 Provides-Extra: bjoern
```

### Comparing `finitelycomputable-helloworld-flask-quart-24.3/finitelycomputable/helloworld_flask.py` & `finitelycomputable_helloworld_flask_quart-24.4/finitelycomputable/helloworld_flask.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-helloworld-flask-quart-24.3/finitelycomputable_helloworld_flask_quart.egg-info/PKG-INFO` & `finitelycomputable_helloworld_flask_quart-24.4/finitelycomputable_helloworld_flask_quart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-helloworld-flask-quart
-Version: 24.3
+Version: 24.4
 Summary: hello_world in Flask from an implementation in Quart
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/hello_world
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -27,14 +27,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: Flask~=3.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
+Requires-Dist: finitelycomputable-tests; extra == "tests"
 Provides-Extra: waitress
 Requires-Dist: waitress~=2.1; extra == "waitress"
 Provides-Extra: cherrypy
 Requires-Dist: cherrypy~=18.0; extra == "cherrypy"
 Provides-Extra: cheroot
 Requires-Dist: cheroot~=9.0; extra == "cheroot"
 Provides-Extra: bjoern
```

### Comparing `finitelycomputable-helloworld-flask-quart-24.3/pyproject.toml` & `finitelycomputable_helloworld_flask_quart-24.4/pyproject.toml`

 * *Files 5% similar despite different names*

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
 name = "finitelycomputable-helloworld-flask-quart"
 requires-python = ">=3.8"
 description = "hello_world in Flask from an implementation in Quart"
 dependencies = [
   "Flask~=3.0",
 ]
 classifiers = [
@@ -28,15 +28,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 
 [project.optional-dependencies]
-tests = ["pytest", "pytest-env"]
+tests = ["pytest", "pytest-env", "finitelycomputable-tests"]
 waitress = ["waitress~=2.1"]
 cherrypy = ["cherrypy~=18.0"]
 cheroot = ["cheroot~=9.0"]
 bjoern = ["bjoern~=3.0"]
 gunicorn = ["gunicorn~=21.2"]
 
 [project.scripts]
```

