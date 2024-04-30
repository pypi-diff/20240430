# Comparing `tmp/django_outlook_email_backend-0.3.3.tar.gz` & `tmp/django_outlook_email_backend-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_outlook_email_backend-0.3.3.tar", last modified: Tue Apr 30 18:18:03 2024, max compression
+gzip compressed data, was "django_outlook_email_backend-0.3.4.tar", last modified: Tue Apr 30 18:58:38 2024, max compression
```

## Comparing `django_outlook_email_backend-0.3.3.tar` & `django_outlook_email_backend-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:18:03.125608 django_outlook_email_backend-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 18:18:03.125608 django_outlook_email_backend-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 18:17:53.000000 django_outlook_email_backend-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-30 18:17:53.000000 django_outlook_email_backend-0.3.3/django_oauth2_email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:18:03.125608 django_outlook_email_backend-0.3.3/django_outlook_email_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 18:18:03.000000 django_outlook_email_backend-0.3.3/django_outlook_email_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-30 18:18:03.000000 django_outlook_email_backend-0.3.3/django_outlook_email_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:18:03.000000 django_outlook_email_backend-0.3.3/django_outlook_email_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 18:18:03.000000 django_outlook_email_backend-0.3.3/django_outlook_email_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:18:02.000000 django_outlook_email_backend-0.3.3/django_outlook_email_backend.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:18:03.125608 django_outlook_email_backend-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-30 18:17:53.000000 django_outlook_email_backend-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:58:38.009746 django_outlook_email_backend-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 18:58:38.009746 django_outlook_email_backend-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 18:58:34.000000 django_outlook_email_backend-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-30 18:58:34.000000 django_outlook_email_backend-0.3.4/django_oauth2_email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:58:38.009746 django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 18:58:38.000000 django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-30 18:58:38.000000 django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:58:38.000000 django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 18:58:38.000000 django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:58:37.000000 django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:58:38.009746 django_outlook_email_backend-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-30 18:58:34.000000 django_outlook_email_backend-0.3.4/setup.py
```

### Comparing `django_outlook_email_backend-0.3.3/PKG-INFO` & `django_outlook_email_backend-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-outlook-email-backend
-Version: 0.3.3
+Version: 0.3.4
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_outlook_email_backend-0.3.3/django_oauth2_email.py` & `django_outlook_email_backend-0.3.4/django_oauth2_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 from django.core.mail.backends.smtp import EmailBackend
 import msal
-import environ
 import requests
 from django.core.mail.message import sanitize_address
 from django.conf import settings
 
 
 
 
-env = environ.Env(
-    # set casting, default value
-    DEBUG=(bool, False)
-)
-environ.Env.read_env()
 
 class OutlookOauth2EmailBackend(EmailBackend):
 
     access_token = None
-    client_id = env("outlook_client_id")
-    client_secret = env("outlook_client_secret")
+    client_id = settings.OUTLOOK_CLIENT_ID
+    client_secret = settings.OUTLOOK_CLIENT_SECRET
 
     def send_messages(self, email_messages):
         self._set_access_token()
 
         if not email_messages:
             return 0
         with self._lock:
```

### Comparing `django_outlook_email_backend-0.3.3/django_outlook_email_backend.egg-info/PKG-INFO` & `django_outlook_email_backend-0.3.4/django_outlook_email_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-outlook-email-backend
-Version: 0.3.3
+Version: 0.3.4
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_outlook_email_backend-0.3.3/setup.py` & `django_outlook_email_backend-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='django-outlook-email-backend',
-    version='0.3.3',
+    version='0.3.4',
     description='Ouauth2 outlook email backend for Django',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Marc Claramunt',
     author_email='mclaramunt@enley.com',
     license='MIT',
     zip_safe=True,
```
