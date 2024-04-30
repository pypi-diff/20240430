# Comparing `tmp/django_outlook_email_backend-0.3.6.tar.gz` & `tmp/django_outlook_email_backend-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_outlook_email_backend-0.3.6.tar", last modified: Tue Apr 30 19:39:48 2024, max compression
+gzip compressed data, was "django_outlook_email_backend-0.3.7.tar", last modified: Tue Apr 30 19:47:14 2024, max compression
```

## Comparing `django_outlook_email_backend-0.3.6.tar` & `django_outlook_email_backend-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:39:48.189041 django_outlook_email_backend-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 19:39:48.189041 django_outlook_email_backend-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 19:39:44.000000 django_outlook_email_backend-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:39:48.189041 django_outlook_email_backend-0.3.6/django_outlook_email_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:39:44.000000 django_outlook_email_backend-0.3.6/django_outlook_email_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-30 19:39:44.000000 django_outlook_email_backend-0.3.6/django_outlook_email_backend/django_oauth2_email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:39:48.189041 django_outlook_email_backend-0.3.6/django_outlook_email_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 19:39:48.000000 django_outlook_email_backend-0.3.6/django_outlook_email_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-30 19:39:48.000000 django_outlook_email_backend-0.3.6/django_outlook_email_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:39:48.000000 django_outlook_email_backend-0.3.6/django_outlook_email_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 19:39:48.000000 django_outlook_email_backend-0.3.6/django_outlook_email_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:39:48.000000 django_outlook_email_backend-0.3.6/django_outlook_email_backend.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:39:48.189041 django_outlook_email_backend-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-30 19:39:44.000000 django_outlook_email_backend-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:47:14.085568 django_outlook_email_backend-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 19:47:14.085568 django_outlook_email_backend-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 19:47:10.000000 django_outlook_email_backend-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-30 19:47:10.000000 django_outlook_email_backend-0.3.7/django_oauth2_email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:47:14.085568 django_outlook_email_backend-0.3.7/django_outlook_email_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 19:47:14.000000 django_outlook_email_backend-0.3.7/django_outlook_email_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-30 19:47:14.000000 django_outlook_email_backend-0.3.7/django_outlook_email_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:47:14.000000 django_outlook_email_backend-0.3.7/django_outlook_email_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 19:47:14.000000 django_outlook_email_backend-0.3.7/django_outlook_email_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:47:13.000000 django_outlook_email_backend-0.3.7/django_outlook_email_backend.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:47:14.085568 django_outlook_email_backend-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-30 19:47:10.000000 django_outlook_email_backend-0.3.7/setup.py
```

### Comparing `django_outlook_email_backend-0.3.6/PKG-INFO` & `django_outlook_email_backend-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-outlook-email-backend
-Version: 0.3.6
+Version: 0.3.7
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_outlook_email_backend-0.3.6/django_outlook_email_backend/django_oauth2_email.py` & `django_outlook_email_backend-0.3.7/django_oauth2_email.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-0.3.6/django_outlook_email_backend.egg-info/PKG-INFO` & `django_outlook_email_backend-0.3.7/django_outlook_email_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-outlook-email-backend
-Version: 0.3.6
+Version: 0.3.7
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_outlook_email_backend-0.3.6/setup.py` & `django_outlook_email_backend-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='django-outlook-email-backend',
-    version='0.3.6',
+    version='0.3.7',
     description='Ouauth2 outlook email backend for Django',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Marc Claramunt',
     author_email='mclaramunt@enley.com',
     license='MIT',
     zip_safe=True,
```

