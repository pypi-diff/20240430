# Comparing `tmp/postoffice_django-0.8.2.tar.gz` & `tmp/postoffice_django-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postoffice_django-0.8.2.tar", last modified: Fri Jan  8 17:05:37 2021, max compression
+gzip compressed data, was "postoffice_django-0.9.0.tar", last modified: Mon Jan 11 12:13:31 2021, max compression
```

## Comparing `postoffice_django-0.8.2.tar` & `postoffice_django-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:37.009755 postoffice_django-0.8.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8201 2021-01-08 17:05:37.009755 postoffice_django-0.8.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5812 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:37.005755 postoffice_django-0.8.2/postoffice_django/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       69 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      435 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/admin.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:37.009755 postoffice_django-0.8.2/postoffice_django/api/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/api/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1097 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/api/views.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      178 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/apps.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      383 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2872 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/exceptions.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:37.009755 postoffice_django-0.8.2/postoffice_django/management/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/management/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:37.009755 postoffice_django-0.8.2/postoffice_django/management/commands/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/management/commands/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      306 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/management/commands/configure_postoffice.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      274 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/management/commands/configure_postoffice_publishers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      265 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/management/commands/configure_postoffice_topics.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:37.009755 postoffice_django-0.8.2/postoffice_django/migrations/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      856 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/migrations/0001_initial.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      344 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/migrations/0002_add_bulk_field.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/migrations/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      390 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3985 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/publishing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      319 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/serializers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1515 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/settings.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/postoffice_django/urls.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:37.009755 postoffice_django-0.8.2/postoffice_django.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8201 2021-01-08 17:05:36.000000 postoffice_django-0.8.2/postoffice_django.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1056 2021-01-08 17:05:36.000000 postoffice_django-0.8.2/postoffice_django.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-01-08 17:05:36.000000 postoffice_django-0.8.2/postoffice_django.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-01-08 17:05:36.000000 postoffice_django-0.8.2/postoffice_django.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      405 2021-01-08 17:05:37.009755 postoffice_django-0.8.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1883 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:37.005755 postoffice_django-0.8.2/tests/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:37.009755 postoffice_django-0.8.2/tests/api/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/tests/api/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3410 2021-01-08 17:05:33.000000 postoffice_django-0.8.2/tests/api/test_views.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:31.138668 postoffice_django-0.9.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8201 2021-01-11 12:13:31.138668 postoffice_django-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5812 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:31.138668 postoffice_django-0.9.0/postoffice_django/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       69 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      435 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/admin.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:31.138668 postoffice_django-0.9.0/postoffice_django/api/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/api/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1097 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/api/views.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      178 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/apps.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      383 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2872 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/exceptions.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:31.138668 postoffice_django-0.9.0/postoffice_django/management/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/management/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:31.138668 postoffice_django-0.9.0/postoffice_django/management/commands/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/management/commands/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      306 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/management/commands/configure_postoffice.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      274 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/management/commands/configure_postoffice_publishers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      265 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/management/commands/configure_postoffice_topics.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:31.138668 postoffice_django-0.9.0/postoffice_django/migrations/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      856 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/migrations/0001_initial.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      344 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/migrations/0002_add_bulk_field.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      723 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/migrations/0003_set_json_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/migrations/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      487 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3985 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/publishing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      319 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/serializers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1515 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/settings.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/postoffice_django/urls.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:31.138668 postoffice_django-0.9.0/postoffice_django.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8201 2021-01-11 12:13:30.000000 postoffice_django-0.9.0/postoffice_django.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1110 2021-01-11 12:13:31.000000 postoffice_django-0.9.0/postoffice_django.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-01-11 12:13:30.000000 postoffice_django-0.9.0/postoffice_django.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-01-11 12:13:30.000000 postoffice_django-0.9.0/postoffice_django.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      405 2021-01-11 12:13:31.138668 postoffice_django-0.9.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1883 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:31.134668 postoffice_django-0.9.0/tests/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:31.138668 postoffice_django-0.9.0/tests/api/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/tests/api/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3410 2021-01-11 12:13:24.000000 postoffice_django-0.9.0/tests/api/test_views.py
```

### Comparing `postoffice_django-0.8.2/PKG-INFO` & `postoffice_django-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postoffice_django
-Version: 0.8.2
+Version: 0.9.0
 Summary: A simple Django app to comunicate with postoffice
 Home-page: https://github.com/mercadona/postoffice_django/
 Author: Mercadona
 Author-email: sofware.online@mercadona.es
 License: APACHE License
 Description: # Post office django client
```

### Comparing `postoffice_django-0.8.2/README.md` & `postoffice_django-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `postoffice_django-0.8.2/postoffice_django/api/views.py` & `postoffice_django-0.9.0/postoffice_django/api/views.py`

 * *Files identical despite different names*

### Comparing `postoffice_django-0.8.2/postoffice_django/config.py` & `postoffice_django-0.9.0/postoffice_django/config.py`

 * *Files identical despite different names*

### Comparing `postoffice_django-0.8.2/postoffice_django/exceptions.py` & `postoffice_django-0.9.0/postoffice_django/exceptions.py`

 * *Files identical despite different names*

### Comparing `postoffice_django-0.8.2/postoffice_django/migrations/0001_initial.py` & `postoffice_django-0.9.0/postoffice_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `postoffice_django-0.8.2/postoffice_django/publishing.py` & `postoffice_django-0.9.0/postoffice_django/publishing.py`

 * *Files identical despite different names*

### Comparing `postoffice_django-0.8.2/postoffice_django/settings.py` & `postoffice_django-0.9.0/postoffice_django/settings.py`

 * *Files identical despite different names*

### Comparing `postoffice_django-0.8.2/postoffice_django.egg-info/PKG-INFO` & `postoffice_django-0.9.0/postoffice_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postoffice-django
-Version: 0.8.2
+Version: 0.9.0
 Summary: A simple Django app to comunicate with postoffice
 Home-page: https://github.com/mercadona/postoffice_django/
 Author: Mercadona
 Author-email: sofware.online@mercadona.es
 License: APACHE License
 Description: # Post office django client
```

### Comparing `postoffice_django-0.8.2/postoffice_django.egg-info/SOURCES.txt` & `postoffice_django-0.9.0/postoffice_django.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,10 +21,11 @@
 postoffice_django/management/__init__.py
 postoffice_django/management/commands/__init__.py
 postoffice_django/management/commands/configure_postoffice.py
 postoffice_django/management/commands/configure_postoffice_publishers.py
 postoffice_django/management/commands/configure_postoffice_topics.py
 postoffice_django/migrations/0001_initial.py
 postoffice_django/migrations/0002_add_bulk_field.py
+postoffice_django/migrations/0003_set_json_encoder.py
 postoffice_django/migrations/__init__.py
 tests/api/__init__.py
 tests/api/test_views.py
```

### Comparing `postoffice_django-0.8.2/setup.py` & `postoffice_django-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 current_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(current_directory, 'README.md'), encoding='utf-8') as file:
     long_description = file.read()
 
 
-VERSION = '0.8.2'
+VERSION = '0.9.0'
 
 
 class VerifyVersionCommand(install):
     description = 'Verify that the git tag matches our version'
 
     def run(self):
         tag = os.getenv('CIRCLE_TAG')
```

### Comparing `postoffice_django-0.8.2/tests/api/test_views.py` & `postoffice_django-0.9.0/tests/api/test_views.py`

 * *Files identical despite different names*

