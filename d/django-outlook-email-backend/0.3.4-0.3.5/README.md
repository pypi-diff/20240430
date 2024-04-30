# Comparing `tmp/django_outlook_email_backend-0.3.4.tar.gz` & `tmp/django_outlook_email_backend-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_outlook_email_backend-0.3.4.tar", last modified: Tue Apr 30 18:58:38 2024, max compression
+gzip compressed data, was "django_outlook_email_backend-0.3.5.tar", last modified: Tue Apr 30 19:30:23 2024, max compression
```

## Comparing `django_outlook_email_backend-0.3.4.tar` & `django_outlook_email_backend-0.3.5.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:58:38.009746 django_outlook_email_backend-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 18:58:38.009746 django_outlook_email_backend-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 18:58:34.000000 django_outlook_email_backend-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-30 18:58:34.000000 django_outlook_email_backend-0.3.4/django_oauth2_email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:58:38.009746 django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 18:58:38.000000 django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-30 18:58:38.000000 django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:58:38.000000 django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 18:58:38.000000 django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:58:37.000000 django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:58:38.009746 django_outlook_email_backend-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-30 18:58:34.000000 django_outlook_email_backend-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:30:23.283704 django_outlook_email_backend-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 19:30:23.283704 django_outlook_email_backend-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 19:30:19.000000 django_outlook_email_backend-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:30:23.279704 django_outlook_email_backend-0.3.5/django_outlook_email_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:30:19.000000 django_outlook_email_backend-0.3.5/django_outlook_email_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-30 19:30:19.000000 django_outlook_email_backend-0.3.5/django_outlook_email_backend/django_oauth2_email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:30:23.283704 django_outlook_email_backend-0.3.5/django_outlook_email_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 19:30:23.000000 django_outlook_email_backend-0.3.5/django_outlook_email_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-30 19:30:23.000000 django_outlook_email_backend-0.3.5/django_outlook_email_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:30:23.000000 django_outlook_email_backend-0.3.5/django_outlook_email_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 19:30:23.000000 django_outlook_email_backend-0.3.5/django_outlook_email_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:30:23.000000 django_outlook_email_backend-0.3.5/django_outlook_email_backend.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:30:23.283704 django_outlook_email_backend-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-30 19:30:19.000000 django_outlook_email_backend-0.3.5/setup.py
```

### Comparing `django_outlook_email_backend-0.3.4/PKG-INFO` & `django_outlook_email_backend-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-outlook-email-backend
-Version: 0.3.4
+Version: 0.3.5
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_outlook_email_backend-0.3.4/django_oauth2_email.py` & `django_outlook_email_backend-0.3.5/django_outlook_email_backend/django_oauth2_email.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/PKG-INFO` & `django_outlook_email_backend-0.3.5/django_outlook_email_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-outlook-email-backend
-Version: 0.3.4
+Version: 0.3.5
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_outlook_email_backend-0.3.4/setup.py` & `django_outlook_email_backend-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='django-outlook-email-backend',
-    version='0.3.4',
+    version='0.3.5',
     description='Ouauth2 outlook email backend for Django',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Marc Claramunt',
     author_email='mclaramunt@enley.com',
     license='MIT',
     zip_safe=True,
```

