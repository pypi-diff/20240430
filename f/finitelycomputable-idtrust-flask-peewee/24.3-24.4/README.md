# Comparing `tmp/finitelycomputable-idtrust-flask-peewee-24.3.tar.gz` & `tmp/finitelycomputable_idtrust_flask_peewee-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable-idtrust-flask-peewee-24.3.tar", last modified: Mon Apr  1 03:35:03 2024, max compression
+gzip compressed data, was "finitelycomputable_idtrust_flask_peewee-24.4.tar", last modified: Tue Apr 30 04:47:21 2024, max compression
```

## Comparing `finitelycomputable-idtrust-flask-peewee-24.3.tar` & `finitelycomputable_idtrust_flask_peewee-24.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:03.329066 finitelycomputable-idtrust-flask-peewee-24.3/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2397 2024-04-01 03:35:03.329066 finitelycomputable-idtrust-flask-peewee-24.3/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      325 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-flask-peewee-24.3/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:03.325066 finitelycomputable-idtrust-flask-peewee-24.3/finitelycomputable/
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:03.329066 finitelycomputable-idtrust-flask-peewee-24.3/finitelycomputable/idtrust_flask/
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       54 2024-03-18 04:00:03.000000 finitelycomputable-idtrust-flask-peewee-24.3/finitelycomputable/idtrust_flask/__init__.py
--rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      386 2024-03-25 18:09:15.000000 finitelycomputable-idtrust-flask-peewee-24.3/finitelycomputable/idtrust_flask/peewee.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:03.329066 finitelycomputable-idtrust-flask-peewee-24.3/finitelycomputable_idtrust_flask_peewee.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2397 2024-04-01 03:35:03.000000 finitelycomputable-idtrust-flask-peewee-24.3/finitelycomputable_idtrust_flask_peewee.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      493 2024-04-01 03:35:03.000000 finitelycomputable-idtrust-flask-peewee-24.3/finitelycomputable_idtrust_flask_peewee.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-01 03:35:03.000000 finitelycomputable-idtrust-flask-peewee-24.3/finitelycomputable_idtrust_flask_peewee.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       97 2024-04-01 03:35:03.000000 finitelycomputable-idtrust-flask-peewee-24.3/finitelycomputable_idtrust_flask_peewee.egg-info/entry_points.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      238 2024-04-01 03:35:03.000000 finitelycomputable-idtrust-flask-peewee-24.3/finitelycomputable_idtrust_flask_peewee.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-01 03:35:03.000000 finitelycomputable-idtrust-flask-peewee-24.3/finitelycomputable_idtrust_flask_peewee.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1863 2024-03-16 18:34:55.000000 finitelycomputable-idtrust-flask-peewee-24.3/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-01 03:35:03.329066 finitelycomputable-idtrust-flask-peewee-24.3/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:21.959867 finitelycomputable_idtrust_flask_peewee-24.4/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2455 2024-04-30 04:47:21.959867 finitelycomputable_idtrust_flask_peewee-24.4/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      325 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_flask_peewee-24.4/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:21.955867 finitelycomputable_idtrust_flask_peewee-24.4/finitelycomputable/
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:21.959867 finitelycomputable_idtrust_flask_peewee-24.4/finitelycomputable/idtrust_flask/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       54 2024-03-18 04:00:03.000000 finitelycomputable_idtrust_flask_peewee-24.4/finitelycomputable/idtrust_flask/__init__.py
+-rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      386 2024-03-25 18:09:15.000000 finitelycomputable_idtrust_flask_peewee-24.4/finitelycomputable/idtrust_flask/peewee.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:21.959867 finitelycomputable_idtrust_flask_peewee-24.4/finitelycomputable_idtrust_flask_peewee.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2455 2024-04-30 04:47:21.000000 finitelycomputable_idtrust_flask_peewee-24.4/finitelycomputable_idtrust_flask_peewee.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      493 2024-04-30 04:47:21.000000 finitelycomputable_idtrust_flask_peewee-24.4/finitelycomputable_idtrust_flask_peewee.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:47:21.000000 finitelycomputable_idtrust_flask_peewee-24.4/finitelycomputable_idtrust_flask_peewee.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      101 2024-04-30 04:47:21.000000 finitelycomputable_idtrust_flask_peewee-24.4/finitelycomputable_idtrust_flask_peewee.egg-info/entry_points.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      263 2024-04-30 04:47:21.000000 finitelycomputable_idtrust_flask_peewee-24.4/finitelycomputable_idtrust_flask_peewee.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:47:21.000000 finitelycomputable_idtrust_flask_peewee-24.4/finitelycomputable_idtrust_flask_peewee.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1895 2024-04-28 21:51:18.000000 finitelycomputable_idtrust_flask_peewee-24.4/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:47:21.959867 finitelycomputable_idtrust_flask_peewee-24.4/setup.cfg
```

### Comparing `finitelycomputable-idtrust-flask-peewee-24.3/PKG-INFO` & `finitelycomputable_idtrust_flask_peewee-24.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-flask-peewee
-Version: 24.3
+Version: 24.4
 Summary: A Flask+peewee microsite to explore identifying game-theory strategies
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -29,14 +29,15 @@
 Description-Content-Type: text/x-rst
 Requires-Dist: finitelycomputable-idtrust-app-flask
 Requires-Dist: finitelycomputable-idtrust-db-peewee
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

### Comparing `finitelycomputable-idtrust-flask-peewee-24.3/finitelycomputable_idtrust_flask_peewee.egg-info/PKG-INFO` & `finitelycomputable_idtrust_flask_peewee-24.4/finitelycomputable_idtrust_flask_peewee.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-flask-peewee
-Version: 24.3
+Version: 24.4
 Summary: A Flask+peewee microsite to explore identifying game-theory strategies
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -29,14 +29,15 @@
 Description-Content-Type: text/x-rst
 Requires-Dist: finitelycomputable-idtrust-app-flask
 Requires-Dist: finitelycomputable-idtrust-db-peewee
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

### Comparing `finitelycomputable-idtrust-flask-peewee-24.3/pyproject.toml` & `finitelycomputable_idtrust_flask_peewee-24.4/pyproject.toml`

 * *Files 8% similar despite different names*

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
 name = "finitelycomputable-idtrust-flask-peewee"
 requires-python = ">=3.8"
 description = "A Flask+peewee microsite to explore identifying game-theory strategies"
 dependencies = [
   "finitelycomputable-idtrust-app-flask",
   "finitelycomputable-idtrust-db-peewee",
   "Flask~=3.0",
@@ -30,23 +30,23 @@
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
-finitelycomputable-idtrust-flask-peewee = "finitelycomputable.idtrust_flask:run"
+finitelycomputable-idtrust-flask-peewee = "finitelycomputable.idtrust_app_flask:run"
 
 [project.urls]
 Homepage = "https://www.finitelycomputable.net/identification_of_trust"
 Documentation = "https://github.com/thrasymache/microsites"
 Source = "https://github.com/thrasymache/microsites"
 Gitlab = "https://gitlab.com/thrasymache/microsites"
 sourcehut = "https://git.sr.ht/~thrasymache/finitelycomputable-microsites"
```

