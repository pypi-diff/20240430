# Comparing `tmp/finitelycomputable-helloworld-morepath-falcon-24.3.tar.gz` & `tmp/finitelycomputable_helloworld_morepath_falcon-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable-helloworld-morepath-falcon-24.3.tar", last modified: Mon Apr  1 03:34:21 2024, max compression
+gzip compressed data, was "finitelycomputable_helloworld_morepath_falcon-24.4.tar", last modified: Tue Apr 30 04:46:32 2024, max compression
```

## Comparing `finitelycomputable-helloworld-morepath-falcon-24.3.tar` & `finitelycomputable_helloworld_morepath_falcon-24.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:34:21.732634 finitelycomputable-helloworld-morepath-falcon-24.3/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2256 2024-04-01 03:34:21.732634 finitelycomputable-helloworld-morepath-falcon-24.3/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      267 2024-01-21 20:38:50.000000 finitelycomputable-helloworld-morepath-falcon-24.3/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:34:21.728634 finitelycomputable-helloworld-morepath-falcon-24.3/finitelycomputable/
--rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      965 2024-03-02 07:39:00.000000 finitelycomputable-helloworld-morepath-falcon-24.3/finitelycomputable/helloworld_morepath.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:34:21.728634 finitelycomputable-helloworld-morepath-falcon-24.3/finitelycomputable_helloworld_morepath_falcon.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2256 2024-04-01 03:34:21.000000 finitelycomputable-helloworld-morepath-falcon-24.3/finitelycomputable_helloworld_morepath_falcon.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      527 2024-04-01 03:34:21.000000 finitelycomputable-helloworld-morepath-falcon-24.3/finitelycomputable_helloworld_morepath_falcon.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-01 03:34:21.000000 finitelycomputable-helloworld-morepath-falcon-24.3/finitelycomputable_helloworld_morepath_falcon.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      102 2024-04-01 03:34:21.000000 finitelycomputable-helloworld-morepath-falcon-24.3/finitelycomputable_helloworld_morepath_falcon.egg-info/entry_points.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      188 2024-04-01 03:34:21.000000 finitelycomputable-helloworld-morepath-falcon-24.3/finitelycomputable_helloworld_morepath_falcon.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-01 03:34:21.000000 finitelycomputable-helloworld-morepath-falcon-24.3/finitelycomputable_helloworld_morepath_falcon.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1774 2024-03-16 18:34:55.000000 finitelycomputable-helloworld-morepath-falcon-24.3/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-01 03:34:21.732634 finitelycomputable-helloworld-morepath-falcon-24.3/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:46:32.863644 finitelycomputable_helloworld_morepath_falcon-24.4/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2314 2024-04-30 04:46:32.863644 finitelycomputable_helloworld_morepath_falcon-24.4/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      267 2024-01-21 20:38:50.000000 finitelycomputable_helloworld_morepath_falcon-24.4/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:46:32.863644 finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable/
+-rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      965 2024-03-02 07:39:00.000000 finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable/helloworld_morepath.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:46:32.863644 finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable/tests/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      665 2024-04-30 03:36:46.000000 finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable/tests/test_helloworld_morepath.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:46:32.863644 finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable_helloworld_morepath_falcon.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2314 2024-04-30 04:46:32.000000 finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable_helloworld_morepath_falcon.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      580 2024-04-30 04:46:32.000000 finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable_helloworld_morepath_falcon.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:46:32.000000 finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable_helloworld_morepath_falcon.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      102 2024-04-30 04:46:32.000000 finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable_helloworld_morepath_falcon.egg-info/entry_points.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      213 2024-04-30 04:46:32.000000 finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable_helloworld_morepath_falcon.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:46:32.000000 finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable_helloworld_morepath_falcon.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1802 2024-04-28 21:51:18.000000 finitelycomputable_helloworld_morepath_falcon-24.4/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:46:32.863644 finitelycomputable_helloworld_morepath_falcon-24.4/setup.cfg
```

### Comparing `finitelycomputable-helloworld-morepath-falcon-24.3/PKG-INFO` & `finitelycomputable_helloworld_morepath_falcon-24.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-helloworld-morepath-falcon
-Version: 24.3
+Version: 24.4
 Summary: hello_world in Morepath from an implementation in Falcon
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/hello_world
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -28,14 +28,15 @@
 Description-Content-Type: text/x-rst
 Requires-Dist: morepath~=0.19
 Requires-Dist: falcon~=3.1
 Provides-Extra: tests
 Requires-Dist: webtest; extra == "tests"
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

### Comparing `finitelycomputable-helloworld-morepath-falcon-24.3/finitelycomputable/helloworld_morepath.py` & `finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable/helloworld_morepath.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-helloworld-morepath-falcon-24.3/finitelycomputable_helloworld_morepath_falcon.egg-info/PKG-INFO` & `finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable_helloworld_morepath_falcon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-helloworld-morepath-falcon
-Version: 24.3
+Version: 24.4
 Summary: hello_world in Morepath from an implementation in Falcon
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/hello_world
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -28,14 +28,15 @@
 Description-Content-Type: text/x-rst
 Requires-Dist: morepath~=0.19
 Requires-Dist: falcon~=3.1
 Provides-Extra: tests
 Requires-Dist: webtest; extra == "tests"
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

### Comparing `finitelycomputable-helloworld-morepath-falcon-24.3/finitelycomputable_helloworld_morepath_falcon.egg-info/SOURCES.txt` & `finitelycomputable_helloworld_morepath_falcon-24.4/finitelycomputable_helloworld_morepath_falcon.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.rst
 pyproject.toml
 ./finitelycomputable/helloworld_morepath.py
 finitelycomputable/helloworld_morepath.py
+finitelycomputable/tests/test_helloworld_morepath.py
 finitelycomputable_helloworld_morepath_falcon.egg-info/PKG-INFO
 finitelycomputable_helloworld_morepath_falcon.egg-info/SOURCES.txt
 finitelycomputable_helloworld_morepath_falcon.egg-info/dependency_links.txt
 finitelycomputable_helloworld_morepath_falcon.egg-info/entry_points.txt
 finitelycomputable_helloworld_morepath_falcon.egg-info/requires.txt
 finitelycomputable_helloworld_morepath_falcon.egg-info/top_level.txt
```

### Comparing `finitelycomputable-helloworld-morepath-falcon-24.3/pyproject.toml` & `finitelycomputable_helloworld_morepath_falcon-24.4/pyproject.toml`

 * *Files 4% similar despite different names*

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
 name = "finitelycomputable-helloworld-morepath-falcon"
 requires-python = ">=3.8"
 description = "hello_world in Morepath from an implementation in Falcon"
 dependencies = [
   "morepath~=0.19",
   "falcon~=3.1",
 ]
@@ -29,15 +29,15 @@
   "Programming Language :: Python :: 3.11",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 
 [project.optional-dependencies]
 tests = ["webtest",
-  "pytest", "pytest-env"]
+  "pytest", "pytest-env", "finitelycomputable-tests"]
 waitress = ["waitress~=2.1"]
 cherrypy = ["cherrypy~=18.0"]
 cheroot = ["cheroot~=9.0"]
 bjoern = ["bjoern~=3.0"]
 gunicorn = ["gunicorn~=21.2"]
 
 [project.scripts]
```

