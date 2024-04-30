# Comparing `tmp/finitelycomputable-morepath-mount-24.3.tar.gz` & `tmp/finitelycomputable_morepath_mount-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable-morepath-mount-24.3.tar", last modified: Mon Apr  1 03:33:02 2024, max compression
+gzip compressed data, was "finitelycomputable_morepath_mount-24.4.tar", last modified: Tue Apr 30 04:45:01 2024, max compression
```

## Comparing `finitelycomputable-morepath-mount-24.3.tar` & `finitelycomputable_morepath_mount-24.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:33:02.747814 finitelycomputable-morepath-mount-24.3/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2289 2024-04-01 03:33:02.747814 finitelycomputable-morepath-mount-24.3/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      193 2023-09-12 03:23:48.000000 finitelycomputable-morepath-mount-24.3/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:33:02.747814 finitelycomputable-morepath-mount-24.3/finitelycomputable/
--rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)     1560 2023-11-30 06:01:53.000000 finitelycomputable-morepath-mount-24.3/finitelycomputable/morepath_mount.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:33:02.747814 finitelycomputable-morepath-mount-24.3/finitelycomputable_morepath_mount.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2289 2024-04-01 03:33:02.000000 finitelycomputable-morepath-mount-24.3/finitelycomputable_morepath_mount.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      445 2024-04-01 03:33:02.000000 finitelycomputable-morepath-mount-24.3/finitelycomputable_morepath_mount.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-01 03:33:02.000000 finitelycomputable-morepath-mount-24.3/finitelycomputable_morepath_mount.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       92 2024-04-01 03:33:02.000000 finitelycomputable-morepath-mount-24.3/finitelycomputable_morepath_mount.egg-info/entry_points.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      229 2024-04-01 03:33:02.000000 finitelycomputable-morepath-mount-24.3/finitelycomputable_morepath_mount.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-01 03:33:02.000000 finitelycomputable-morepath-mount-24.3/finitelycomputable_morepath_mount.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1833 2024-03-16 18:34:55.000000 finitelycomputable-morepath-mount-24.3/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-01 03:33:02.747814 finitelycomputable-morepath-mount-24.3/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:45:01.039219 finitelycomputable_morepath_mount-24.4/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2347 2024-04-30 04:45:01.039219 finitelycomputable_morepath_mount-24.4/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      193 2023-09-12 03:23:48.000000 finitelycomputable_morepath_mount-24.4/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:45:01.035219 finitelycomputable_morepath_mount-24.4/finitelycomputable/
+-rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)     1560 2023-11-30 06:01:53.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable/morepath_mount.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:45:01.035219 finitelycomputable_morepath_mount-24.4/finitelycomputable/tests/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      566 2024-04-30 03:37:13.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable/tests/test_morepath_mount.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:45:01.039219 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2347 2024-04-30 04:45:01.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      493 2024-04-30 04:45:01.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:45:01.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       92 2024-04-30 04:45:01.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/entry_points.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      254 2024-04-30 04:45:01.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:45:01.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1861 2024-04-28 21:51:18.000000 finitelycomputable_morepath_mount-24.4/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:45:01.039219 finitelycomputable_morepath_mount-24.4/setup.cfg
```

### Comparing `finitelycomputable-morepath-mount-24.3/PKG-INFO` & `finitelycomputable_morepath_mount-24.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-morepath-mount
-Version: 24.3
+Version: 24.4
 Summary: The Morepath-based wsgi app using Morepath.mount to combine the microsites of finitelycomputable.net
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/wsgi_info
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -27,14 +27,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: morepath~=0.19
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

### Comparing `finitelycomputable-morepath-mount-24.3/finitelycomputable/morepath_mount.py` & `finitelycomputable_morepath_mount-24.4/finitelycomputable/morepath_mount.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-morepath-mount-24.3/finitelycomputable_morepath_mount.egg-info/PKG-INFO` & `finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-morepath-mount
-Version: 24.3
+Version: 24.4
 Summary: The Morepath-based wsgi app using Morepath.mount to combine the microsites of finitelycomputable.net
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/wsgi_info
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -27,14 +27,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: morepath~=0.19
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

### Comparing `finitelycomputable-morepath-mount-24.3/pyproject.toml` & `finitelycomputable_morepath_mount-24.4/pyproject.toml`

 * *Files 3% similar despite different names*

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
 name = "finitelycomputable-morepath-mount"
 requires-python = ">=3.8"
 description = "The Morepath-based wsgi app using Morepath.mount to combine the microsites of finitelycomputable.net"
 dependencies = [
   "morepath~=0.19",
 ]
 classifiers = [
@@ -28,15 +28,15 @@
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
 helloworld = ["finitelycomputable-helloworld-morepath"]
 gunicorn = ["gunicorn~=21.2"]
```

