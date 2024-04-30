# Comparing `tmp/opengeodeweb_back-4.1.0rc1.tar.gz` & `tmp/opengeodeweb_back-4.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengeodeweb_back-4.1.0rc1.tar", last modified: Mon Apr 29 12:53:53 2024, max compression
+gzip compressed data, was "opengeodeweb_back-4.1.0rc2.tar", last modified: Mon Apr 29 13:06:01 2024, max compression
```

## Comparing `opengeodeweb_back-4.1.0rc1.tar` & `opengeodeweb_back-4.1.0rc2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.632957 opengeodeweb_back-4.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-29 12:53:53.628957 opengeodeweb_back-4.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-29 12:53:45.000000 opengeodeweb_back-4.1.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:53:53.632957 opengeodeweb_back-4.1.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.624957 opengeodeweb_back-4.1.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.628957 opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-29 12:53:53.000000 opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-29 12:53:53.000000 opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:53:53.000000 opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-29 12:53:53.000000 opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 12:53:53.000000 opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.628957 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/geode_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20286 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/geode_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.628957 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/blueprint_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.628957 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/allowed_files.json
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/allowed_objects.json
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/geode_objects_and_output_extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/geographic_coordinate_systems.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/inspect_file.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/missing_files.json
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/upload_file.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.628957 opengeodeweb_back-4.1.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/tests/test_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:06:01.819586 opengeodeweb_back-4.1.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-29 13:06:01.819586 opengeodeweb_back-4.1.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-29 13:05:49.000000 opengeodeweb_back-4.1.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:06:01.819586 opengeodeweb_back-4.1.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:06:01.815586 opengeodeweb_back-4.1.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:06:01.819586 opengeodeweb_back-4.1.0rc2/src/OpenGeodeWeb_Back.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-29 13:06:01.000000 opengeodeweb_back-4.1.0rc2/src/OpenGeodeWeb_Back.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-29 13:06:01.000000 opengeodeweb_back-4.1.0rc2/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:06:01.000000 opengeodeweb_back-4.1.0rc2/src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-29 13:06:01.000000 opengeodeweb_back-4.1.0rc2/src/OpenGeodeWeb_Back.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 13:06:01.000000 opengeodeweb_back-4.1.0rc2/src/OpenGeodeWeb_Back.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:06:01.819586 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/geode_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20286 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/geode_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:06:01.819586 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/routes/blueprint_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:06:01.819586 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/routes/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/routes/schemas/allowed_files.json
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/routes/schemas/allowed_objects.json
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/routes/schemas/geode_objects_and_output_extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/routes/schemas/geographic_coordinate_systems.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/routes/schemas/inspect_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/routes/schemas/missing_files.json
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/routes/schemas/upload_file.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:06:01.819586 opengeodeweb_back-4.1.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-29 13:05:43.000000 opengeodeweb_back-4.1.0rc2/tests/test_routes.py
```

### Comparing `opengeodeweb_back-4.1.0rc1/LICENSE` & `opengeodeweb_back-4.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.1.0rc1/PKG-INFO` & `opengeodeweb_back-4.1.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Back
-Version: 4.1.0rc1
+Version: 4.1.0rc2
 Summary: OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <team-web@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opengeodeweb_back-4.1.0rc1/README.md` & `opengeodeweb_back-4.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.1.0rc1/pyproject.toml` & `opengeodeweb_back-4.1.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "OpenGeodeWeb-Back"
-version = "4.1.0-rc.1"
+version = "4.1.0-rc.2"
 dynamic = ["dependencies"]
 authors = [
   { name="Geode-solutions", email="team-web@geode-solutions.com" },
 ]
 description = "OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `opengeodeweb_back-4.1.0rc1/requirements.txt` & `opengeodeweb_back-4.1.0rc2/requirements.txt`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO` & `opengeodeweb_back-4.1.0rc2/src/OpenGeodeWeb_Back.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Back
-Version: 4.1.0rc1
+Version: 4.1.0rc2
 Summary: OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <team-web@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt` & `opengeodeweb_back-4.1.0rc2/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/requires.txt` & `opengeodeweb_back-4.1.0rc2/src/OpenGeodeWeb_Back.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/geode_functions.py` & `opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/geode_functions.py`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/geode_objects.py` & `opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/geode_objects.py`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/blueprint_routes.py` & `opengeodeweb_back-4.1.0rc2/src/opengeodeweb_back/routes/blueprint_routes.py`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.1.0rc1/tests/test_functions.py` & `opengeodeweb_back-4.1.0rc2/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.1.0rc1/tests/test_routes.py` & `opengeodeweb_back-4.1.0rc2/tests/test_routes.py`

 * *Files identical despite different names*

