# Comparing `tmp/finitelycomputable-idtrust-falcon-peewee-24.3.tar.gz` & `tmp/finitelycomputable_idtrust_falcon_peewee-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable-idtrust-falcon-peewee-24.3.tar", last modified: Mon Apr  1 03:35:11 2024, max compression
+gzip compressed data, was "finitelycomputable_idtrust_falcon_peewee-24.4.tar", last modified: Tue Apr 30 04:47:31 2024, max compression
```

## Comparing `finitelycomputable-idtrust-falcon-peewee-24.3.tar` & `finitelycomputable_idtrust_falcon_peewee-24.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:11.649153 finitelycomputable-idtrust-falcon-peewee-24.3/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2375 2024-04-01 03:35:11.649153 finitelycomputable-idtrust-falcon-peewee-24.3/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      330 2024-03-18 03:42:34.000000 finitelycomputable-idtrust-falcon-peewee-24.3/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:11.645152 finitelycomputable-idtrust-falcon-peewee-24.3/finitelycomputable/
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:11.645152 finitelycomputable-idtrust-falcon-peewee-24.3/finitelycomputable/idtrust_falcon/
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       55 2024-03-18 04:20:08.000000 finitelycomputable-idtrust-falcon-peewee-24.3/finitelycomputable/idtrust_falcon/__init__.py
--rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      119 2024-03-18 04:22:15.000000 finitelycomputable-idtrust-falcon-peewee-24.3/finitelycomputable/idtrust_falcon/peewee.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:11.645152 finitelycomputable-idtrust-falcon-peewee-24.3/finitelycomputable_idtrust_falcon_peewee.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2375 2024-04-01 03:35:11.000000 finitelycomputable-idtrust-falcon-peewee-24.3/finitelycomputable_idtrust_falcon_peewee.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      501 2024-04-01 03:35:11.000000 finitelycomputable-idtrust-falcon-peewee-24.3/finitelycomputable_idtrust_falcon_peewee.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-01 03:35:11.000000 finitelycomputable-idtrust-falcon-peewee-24.3/finitelycomputable_idtrust_falcon_peewee.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       99 2024-04-01 03:35:11.000000 finitelycomputable-idtrust-falcon-peewee-24.3/finitelycomputable_idtrust_falcon_peewee.egg-info/entry_points.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      240 2024-04-01 03:35:11.000000 finitelycomputable-idtrust-falcon-peewee-24.3/finitelycomputable_idtrust_falcon_peewee.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-01 03:35:11.000000 finitelycomputable-idtrust-falcon-peewee-24.3/finitelycomputable_idtrust_falcon_peewee.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1845 2024-03-18 04:27:39.000000 finitelycomputable-idtrust-falcon-peewee-24.3/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-01 03:35:11.649153 finitelycomputable-idtrust-falcon-peewee-24.3/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:31.127909 finitelycomputable_idtrust_falcon_peewee-24.4/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2433 2024-04-30 04:47:31.127909 finitelycomputable_idtrust_falcon_peewee-24.4/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      330 2024-03-18 03:42:34.000000 finitelycomputable_idtrust_falcon_peewee-24.4/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:31.127909 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable/
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:31.127909 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable/idtrust_falcon/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       55 2024-03-18 04:20:08.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable/idtrust_falcon/__init__.py
+-rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      119 2024-03-18 04:22:15.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable/idtrust_falcon/peewee.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:31.127909 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2433 2024-04-30 04:47:31.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      501 2024-04-30 04:47:31.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:47:31.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      103 2024-04-30 04:47:31.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/entry_points.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      265 2024-04-30 04:47:31.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:47:31.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1877 2024-04-28 21:51:18.000000 finitelycomputable_idtrust_falcon_peewee-24.4/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:47:31.127909 finitelycomputable_idtrust_falcon_peewee-24.4/setup.cfg
```

### Comparing `finitelycomputable-idtrust-falcon-peewee-24.3/PKG-INFO` & `finitelycomputable_idtrust_falcon_peewee-24.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-falcon-peewee
-Version: 24.3
+Version: 24.4
 Summary: A Falcon+peewee microsite to explore identifying game-theory strategies
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -28,14 +28,15 @@
 Description-Content-Type: text/x-rst
 Requires-Dist: finitelycomputable-idtrust-app-falcon
 Requires-Dist: finitelycomputable-idtrust-db-peewee
 Requires-Dist: falcon~=3.1
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

### Comparing `finitelycomputable-idtrust-falcon-peewee-24.3/finitelycomputable_idtrust_falcon_peewee.egg-info/PKG-INFO` & `finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-falcon-peewee
-Version: 24.3
+Version: 24.4
 Summary: A Falcon+peewee microsite to explore identifying game-theory strategies
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -28,14 +28,15 @@
 Description-Content-Type: text/x-rst
 Requires-Dist: finitelycomputable-idtrust-app-falcon
 Requires-Dist: finitelycomputable-idtrust-db-peewee
 Requires-Dist: falcon~=3.1
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

### Comparing `finitelycomputable-idtrust-falcon-peewee-24.3/pyproject.toml` & `finitelycomputable_idtrust_falcon_peewee-24.4/pyproject.toml`

 * *Files 6% similar despite different names*

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
 name = "finitelycomputable-idtrust-falcon-peewee"
 requires-python = ">=3.8"
 description = "A Falcon+peewee microsite to explore identifying game-theory strategies"
 dependencies = [
   "finitelycomputable-idtrust-app-falcon",
   "finitelycomputable-idtrust-db-peewee",
   "falcon~=3.1",
@@ -29,23 +29,23 @@
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
-finitelycomputable-idtrust-falcon-peewee = "finitelycomputable.idtrust_falcon:run"
+finitelycomputable-idtrust-falcon-peewee = "finitelycomputable.idtrust_app_falcon:run"
 
 [project.urls]
 Homepage = "https://www.finitelycomputable.net/identification_of_trust"
 Documentation = "https://github.com/thrasymache/microsites"
 Source = "https://github.com/thrasymache/microsites"
 Gitlab = "https://gitlab.com/thrasymache/microsites"
 sourcehut = "https://git.sr.ht/~thrasymache/finitelycomputable-microsites"
```

