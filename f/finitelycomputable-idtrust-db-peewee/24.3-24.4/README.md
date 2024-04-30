# Comparing `tmp/finitelycomputable-idtrust-db-peewee-24.3.tar.gz` & `tmp/finitelycomputable_idtrust_db_peewee-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable-idtrust-db-peewee-24.3.tar", last modified: Mon Apr  1 03:35:15 2024, max compression
+gzip compressed data, was "finitelycomputable_idtrust_db_peewee-24.4.tar", last modified: Tue Apr 30 04:47:35 2024, max compression
```

## Comparing `finitelycomputable-idtrust-db-peewee-24.3.tar` & `finitelycomputable_idtrust_db_peewee-24.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:15.801196 finitelycomputable-idtrust-db-peewee-24.3/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1863 2024-04-01 03:35:15.801196 finitelycomputable-idtrust-db-peewee-24.3/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      334 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-db-peewee-24.3/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:15.801196 finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable/
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:15.801196 finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable/idtrust_db/
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        0 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable/idtrust_db/__init__.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     3224 2024-03-25 18:32:19.000000 finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable/idtrust_db/controller.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1816 2024-03-07 18:10:18.000000 finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable/idtrust_db/helpers_for_tests.py
--rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)     1651 2024-03-25 18:18:18.000000 finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable/idtrust_db/models.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:15.801196 finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable_idtrust_db_peewee.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1863 2024-04-01 03:35:15.000000 finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable_idtrust_db_peewee.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      633 2024-04-01 03:35:15.000000 finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable_idtrust_db_peewee.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-01 03:35:15.000000 finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable_idtrust_db_peewee.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       40 2024-04-01 03:35:15.000000 finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable_idtrust_db_peewee.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-01 03:35:15.000000 finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable_idtrust_db_peewee.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1481 2024-03-16 18:34:55.000000 finitelycomputable-idtrust-db-peewee-24.3/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-01 03:35:15.801196 finitelycomputable-idtrust-db-peewee-24.3/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:35.819930 finitelycomputable_idtrust_db_peewee-24.4/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1921 2024-04-30 04:47:35.819930 finitelycomputable_idtrust_db_peewee-24.4/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      334 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_db_peewee-24.4/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:35.815930 finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable/
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:35.815930 finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable/idtrust_db/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        0 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable/idtrust_db/__init__.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     3224 2024-03-25 18:32:19.000000 finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable/idtrust_db/controller.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1816 2024-03-07 18:10:18.000000 finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable/idtrust_db/helpers_for_tests.py
+-rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)     1651 2024-03-25 18:18:18.000000 finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable/idtrust_db/models.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:35.819930 finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable_idtrust_db_peewee.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1921 2024-04-30 04:47:35.000000 finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable_idtrust_db_peewee.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      633 2024-04-30 04:47:35.000000 finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable_idtrust_db_peewee.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:47:35.000000 finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable_idtrust_db_peewee.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       65 2024-04-30 04:47:35.000000 finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable_idtrust_db_peewee.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:47:35.000000 finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable_idtrust_db_peewee.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1509 2024-04-28 21:51:18.000000 finitelycomputable_idtrust_db_peewee-24.4/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:47:35.819930 finitelycomputable_idtrust_db_peewee-24.4/setup.cfg
```

### Comparing `finitelycomputable-idtrust-db-peewee-24.3/PKG-INFO` & `finitelycomputable_idtrust_db_peewee-24.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-db-peewee
-Version: 24.3
+Version: 24.4
 Summary: Peewee implementation of database layer for the Identification of Trust microsite
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -25,14 +25,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: peewee~=3.15
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
+Requires-Dist: finitelycomputable-tests; extra == "tests"
 
 ===============================================
 Identification of Trust (Peewee Database Layer)
 ===============================================
 
 This contains a database layer for implementations of the
 Identification of Trust microsite. It should not depend upon a specific
```

### Comparing `finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable/idtrust_db/controller.py` & `finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable/idtrust_db/controller.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable/idtrust_db/helpers_for_tests.py` & `finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable/idtrust_db/helpers_for_tests.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable/idtrust_db/models.py` & `finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable/idtrust_db/models.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable_idtrust_db_peewee.egg-info/PKG-INFO` & `finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable_idtrust_db_peewee.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-db-peewee
-Version: 24.3
+Version: 24.4
 Summary: Peewee implementation of database layer for the Identification of Trust microsite
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -25,14 +25,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: peewee~=3.15
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
+Requires-Dist: finitelycomputable-tests; extra == "tests"
 
 ===============================================
 Identification of Trust (Peewee Database Layer)
 ===============================================
 
 This contains a database layer for implementations of the
 Identification of Trust microsite. It should not depend upon a specific
```

### Comparing `finitelycomputable-idtrust-db-peewee-24.3/finitelycomputable_idtrust_db_peewee.egg-info/SOURCES.txt` & `finitelycomputable_idtrust_db_peewee-24.4/finitelycomputable_idtrust_db_peewee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-db-peewee-24.3/pyproject.toml` & `finitelycomputable_idtrust_db_peewee-24.4/pyproject.toml`

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
 name = "finitelycomputable-idtrust-db-peewee"
 requires-python = ">=3.8"
 description = "Peewee implementation of database layer for the Identification of Trust microsite"
 dependencies = [
   "peewee~=3.15",
 ]
 classifiers = [
@@ -26,15 +26,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 
 [project.optional-dependencies]
-tests = ["pytest", "pytest-env"]
+tests = ["pytest", "pytest-env", "finitelycomputable-tests"]
 
 [project.urls]
 Homepage = "https://www.finitelycomputable.net/identification_of_trust"
 Documentation = "https://github.com/thrasymache/microsites"
 Source = "https://github.com/thrasymache/microsites"
 Gitlab = "https://gitlab.com/thrasymache/microsites"
 sourcehut = "https://git.sr.ht/~thrasymache/finitelycomputable-microsites"
```

