# Comparing `tmp/finitelycomputable-idtrust-django-24.3.tar.gz` & `tmp/finitelycomputable_idtrust_django-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable-idtrust-django-24.3.tar", last modified: Mon Apr  1 03:35:19 2024, max compression
+gzip compressed data, was "finitelycomputable_idtrust_django-24.4.tar", last modified: Tue Apr 30 04:47:40 2024, max compression
```

## Comparing `finitelycomputable-idtrust-django-24.3.tar` & `finitelycomputable_idtrust_django-24.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:19.961239 finitelycomputable-idtrust-django-24.3/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2532 2024-04-01 03:35:19.961239 finitelycomputable-idtrust-django-24.3/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      410 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:19.957239 finitelycomputable-idtrust-django-24.3/finitelycomputable/
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:19.961239 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        0 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/__init__.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      130 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/admin.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      192 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/apps.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:19.961239 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1136 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/0001_initial.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      659 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/0002_auto_20180311_0154.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      505 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/0003_interaction_user_guess.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1668 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/0004_miscommunication.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      354 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/0005_auto_20210228_1729.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      831 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/0006_journey.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      752 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/0007_strategy_enum.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        0 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/__init__.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1399 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/models.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        0 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/services.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     4956 2024-03-07 06:38:00.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/tests.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1016 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/urls.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     7038 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/views.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:35:19.961239 finitelycomputable-idtrust-django-24.3/finitelycomputable_idtrust_django.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2532 2024-04-01 03:35:19.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable_idtrust_django.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     2171 2024-04-01 03:35:19.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable_idtrust_django.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-01 03:35:19.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable_idtrust_django.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       92 2024-04-01 03:35:19.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable_idtrust_django.egg-info/entry_points.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      227 2024-04-01 03:35:19.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable_idtrust_django.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-01 03:35:19.000000 finitelycomputable-idtrust-django-24.3/finitelycomputable_idtrust_django.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1873 2024-03-16 18:34:55.000000 finitelycomputable-idtrust-django-24.3/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-01 03:35:19.961239 finitelycomputable-idtrust-django-24.3/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:40.539951 finitelycomputable_idtrust_django-24.4/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2590 2024-04-30 04:47:40.539951 finitelycomputable_idtrust_django-24.4/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      410 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:40.535951 finitelycomputable_idtrust_django-24.4/finitelycomputable/
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:40.535951 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        0 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/__init__.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      130 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/admin.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      192 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/apps.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:40.539951 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1136 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/0001_initial.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      659 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/0002_auto_20180311_0154.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      505 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/0003_interaction_user_guess.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1668 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/0004_miscommunication.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      354 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/0005_auto_20210228_1729.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      831 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/0006_journey.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      752 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/0007_strategy_enum.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        0 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/__init__.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1399 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/models.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        0 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/services.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     4956 2024-03-07 06:38:00.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/tests.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1016 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/urls.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     7038 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/views.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:40.539951 finitelycomputable_idtrust_django-24.4/finitelycomputable_idtrust_django.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2590 2024-04-30 04:47:40.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable_idtrust_django.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     2171 2024-04-30 04:47:40.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable_idtrust_django.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:47:40.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable_idtrust_django.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       92 2024-04-30 04:47:40.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable_idtrust_django.egg-info/entry_points.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      252 2024-04-30 04:47:40.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable_idtrust_django.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:47:40.000000 finitelycomputable_idtrust_django-24.4/finitelycomputable_idtrust_django.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1901 2024-04-28 21:51:18.000000 finitelycomputable_idtrust_django-24.4/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:47:40.539951 finitelycomputable_idtrust_django-24.4/setup.cfg
```

### Comparing `finitelycomputable-idtrust-django-24.3/PKG-INFO` & `finitelycomputable_idtrust_django-24.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-django
-Version: 24.3
+Version: 24.4
 Summary: A Django microsite to explore identifying game-theory strategies
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -31,14 +31,15 @@
 Requires-Dist: finitelycomputable-idtrust-common
 Requires-Dist: jinja2~=3.1
 Requires-Dist: Django~=4.2.6
 Provides-Extra: tests
 Requires-Dist: pytest-django; extra == "tests"
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

### Comparing `finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/0001_initial.py` & `finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/0002_auto_20180311_0154.py` & `finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/0002_auto_20180311_0154.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/0004_miscommunication.py` & `finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/0004_miscommunication.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/0006_journey.py` & `finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/0006_journey.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/migrations/0007_strategy_enum.py` & `finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/migrations/0007_strategy_enum.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/models.py` & `finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/models.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/tests.py` & `finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/tests.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/urls.py` & `finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/urls.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-django-24.3/finitelycomputable/idtrust_django/views.py` & `finitelycomputable_idtrust_django-24.4/finitelycomputable/idtrust_django/views.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-django-24.3/finitelycomputable_idtrust_django.egg-info/PKG-INFO` & `finitelycomputable_idtrust_django-24.4/finitelycomputable_idtrust_django.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-django
-Version: 24.3
+Version: 24.4
 Summary: A Django microsite to explore identifying game-theory strategies
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -31,14 +31,15 @@
 Requires-Dist: finitelycomputable-idtrust-common
 Requires-Dist: jinja2~=3.1
 Requires-Dist: Django~=4.2.6
 Provides-Extra: tests
 Requires-Dist: pytest-django; extra == "tests"
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

### Comparing `finitelycomputable-idtrust-django-24.3/finitelycomputable_idtrust_django.egg-info/SOURCES.txt` & `finitelycomputable_idtrust_django-24.4/finitelycomputable_idtrust_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finitelycomputable-idtrust-django-24.3/pyproject.toml` & `finitelycomputable_idtrust_django-24.4/pyproject.toml`

 * *Files 7% similar despite different names*

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
 name = "finitelycomputable-idtrust-django"
 requires-python = ">=3.8"
 description = "A Django microsite to explore identifying game-theory strategies"
 dependencies = [
   "finitelycomputable-idtrust-common",
   "jinja2~=3.1",
   "Django~=4.2.6",
@@ -32,15 +32,15 @@
   "Programming Language :: Python :: 3.11",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 
 [project.optional-dependencies]
 tests = ["pytest-django",
-  "pytest", "pytest-env"]
+  "pytest", "pytest-env", "finitelycomputable-tests"]
 waitress = ["waitress~=2.1"]
 cherrypy = ["cherrypy~=18.0"]
 cheroot = ["cheroot~=9.0"]
 bjoern = ["bjoern~=3.0"]
 gunicorn = ["gunicorn~=21.2"]
 
 [project.scripts]
```

