# Comparing `tmp/squad-django-monaco-1.2.1.tar.gz` & `tmp/squad-django-monaco-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/django-monaco/django-monaco/dist/tmph23ae_ez/squad-django-monaco-1.2.1.tar", last modified: Fri Mar  1 10:45:01 2024, max compression
+gzip compressed data, was "/home/runner/work/django-monaco/django-monaco/dist/tmpheybjbxp/squad-django-monaco-1.2.2.tar", last modified: Tue Apr 30 12:15:24 2024, max compression
```

## Comparing `squad-django-monaco-1.2.1.tar` & `squad-django-monaco-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:45:01.000000 squad-django-monaco-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-01 10:44:47.000000 squad-django-monaco-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:45:01.000000 squad-django-monaco-1.2.1/squad_django_monaco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-01 10:45:01.000000 squad-django-monaco-1.2.1/squad_django_monaco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-01 10:45:01.000000 squad-django-monaco-1.2.1/squad_django_monaco.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-01 10:45:01.000000 squad-django-monaco-1.2.1/squad_django_monaco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-01 10:45:01.000000 squad-django-monaco-1.2.1/squad_django_monaco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 10:45:01.000000 squad-django-monaco-1.2.1/squad_django_monaco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-01 10:45:01.000000 squad-django-monaco-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 10:45:01.000000 squad-django-monaco-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-01 10:44:47.000000 squad-django-monaco-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:45:01.000000 squad-django-monaco-1.2.1/monaco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 10:44:47.000000 squad-django-monaco-1.2.1/monaco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 10:44:47.000000 squad-django-monaco-1.2.1/monaco/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-01 10:44:47.000000 squad-django-monaco-1.2.1/monaco/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:15:24.000000 squad-django-monaco-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-30 12:15:09.000000 squad-django-monaco-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-30 12:15:24.000000 squad-django-monaco-1.2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:15:24.000000 squad-django-monaco-1.2.2/squad_django_monaco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-30 12:15:24.000000 squad-django-monaco-1.2.2/squad_django_monaco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 12:15:24.000000 squad-django-monaco-1.2.2/squad_django_monaco.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 12:15:24.000000 squad-django-monaco-1.2.2/squad_django_monaco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:15:24.000000 squad-django-monaco-1.2.2/squad_django_monaco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 12:15:24.000000 squad-django-monaco-1.2.2/squad_django_monaco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:15:24.000000 squad-django-monaco-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-30 12:15:09.000000 squad-django-monaco-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:15:24.000000 squad-django-monaco-1.2.2/monaco/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-30 12:15:09.000000 squad-django-monaco-1.2.2/monaco/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:15:09.000000 squad-django-monaco-1.2.2/monaco/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:15:09.000000 squad-django-monaco-1.2.2/monaco/__init__.py
```

### Comparing `squad-django-monaco-1.2.1/squad_django_monaco.egg-info/PKG-INFO` & `squad-django-monaco-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squad-django-monaco
-Version: 1.2.1
+Version: 1.2.2
 Summary: Monaco editor widgets in the Django Admin
 Home-page: UNKNOWN
 Author: Ayush Shanker
 License: MIT
 Description: # Django Monaco Editor
         
         This works with django 1.9 & 1.11
```

### Comparing `squad-django-monaco-1.2.1/PKG-INFO` & `squad-django-monaco-1.2.2/squad_django_monaco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squad-django-monaco
-Version: 1.2.1
+Version: 1.2.2
 Summary: Monaco editor widgets in the Django Admin
 Home-page: UNKNOWN
 Author: Ayush Shanker
 License: MIT
 Description: # Django Monaco Editor
         
         This works with django 1.9 & 1.11
```

### Comparing `squad-django-monaco-1.2.1/setup.py` & `squad-django-monaco-1.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 README = open(
     os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")
 ).read()
 
 setup(
     name="squad-django-monaco",
-    version="1.2.1",
+    version="1.2.2",
     packages=["monaco"],
     description="Monaco editor widgets in the Django Admin",
     include_package_data=True,
     long_description=README,
     long_description_content_type="text/markdown",
     author="Ayush Shanker",
     keywords=[
         "monaco",
     ],
     platforms=["OS Independent"],
     license="MIT",
     install_requires=[
-        "Django<=2.0",
+        "Django<=4.0",
     ],
 )
```

### Comparing `squad-django-monaco-1.2.1/monaco/widgets.py` & `squad-django-monaco-1.2.2/monaco/widgets.py`

 * *Files identical despite different names*

