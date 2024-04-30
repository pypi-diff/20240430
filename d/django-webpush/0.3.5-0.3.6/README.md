# Comparing `tmp/django-webpush-0.3.5.tar.gz` & `tmp/django-webpush-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/safwan/test/django-webpush/dist/.tmp-7d6eazl2/django-webpush-0.3.5.tar", last modified: Tue Mar 14 17:58:44 2023, max compression
+gzip compressed data, was "/Users/safwan/test/django-webpush/dist/.tmp-it9p9e6t/django-webpush-0.3.6.tar", last modified: Tue Apr 30 21:05:38 2024, max compression
```

## Comparing `django-webpush-0.3.5.tar` & `django-webpush-0.3.6.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 safwan     (501) staff       (20)        0 2023-03-14 17:58:44.000000 django-webpush-0.3.5/
--rw-r--r--   0 safwan     (501) staff       (20)    35147 2018-02-13 23:42:43.000000 django-webpush-0.3.5/LICENSE
--rw-r--r--   0 safwan     (501) staff       (20)      108 2018-02-13 23:42:43.000000 django-webpush-0.3.5/MANIFEST.in
--rw-r--r--   0 safwan     (501) staff       (20)     8685 2023-03-14 17:58:44.000000 django-webpush-0.3.5/PKG-INFO
--rw-r--r--   0 safwan     (501) staff       (20)     7750 2022-01-11 20:26:58.000000 django-webpush-0.3.5/README.md
-drwxr-xr-x   0 safwan     (501) staff       (20)        0 2023-03-14 17:58:44.000000 django-webpush-0.3.5/django_webpush.egg-info/
--rw-r--r--   0 safwan     (501) staff       (20)     8685 2023-03-14 17:58:44.000000 django-webpush-0.3.5/django_webpush.egg-info/PKG-INFO
--rw-r--r--   0 safwan     (501) staff       (20)      857 2023-03-14 17:58:44.000000 django-webpush-0.3.5/django_webpush.egg-info/SOURCES.txt
--rw-r--r--   0 safwan     (501) staff       (20)        1 2023-03-14 17:58:44.000000 django-webpush-0.3.5/django_webpush.egg-info/dependency_links.txt
--rw-r--r--   0 safwan     (501) staff       (20)       17 2023-03-14 17:58:44.000000 django-webpush-0.3.5/django_webpush.egg-info/requires.txt
--rw-r--r--   0 safwan     (501) staff       (20)        8 2023-03-14 17:58:44.000000 django-webpush-0.3.5/django_webpush.egg-info/top_level.txt
--rw-r--r--   0 safwan     (501) staff       (20)       67 2023-03-14 17:58:44.000000 django-webpush-0.3.5/setup.cfg
--rw-r--r--   0 safwan     (501) staff       (20)     1406 2023-03-14 17:57:51.000000 django-webpush-0.3.5/setup.py
-drwxr-xr-x   0 safwan     (501) staff       (20)        0 2023-03-14 17:58:44.000000 django-webpush-0.3.5/webpush/
--rw-r--r--   0 safwan     (501) staff       (20)      372 2019-02-15 21:19:26.000000 django-webpush-0.3.5/webpush/__init__.py
--rw-r--r--   0 safwan     (501) staff       (20)      744 2019-06-03 00:43:50.000000 django-webpush-0.3.5/webpush/admin.py
--rw-r--r--   0 safwan     (501) staff       (20)        0 2019-02-15 21:19:26.000000 django-webpush-0.3.5/webpush/config.py
--rw-r--r--   0 safwan     (501) staff       (20)     1429 2023-03-14 17:57:26.000000 django-webpush-0.3.5/webpush/forms.py
--rw-r--r--   0 safwan     (501) staff       (20)     1130 2020-03-28 06:22:02.000000 django-webpush-0.3.5/webpush/jinja2.py
-drwxr-xr-x   0 safwan     (501) staff       (20)        0 2023-03-14 17:58:44.000000 django-webpush-0.3.5/webpush/migrations/
--rw-r--r--   0 safwan     (501) staff       (20)     1936 2019-02-15 21:19:26.000000 django-webpush-0.3.5/webpush/migrations/0001_initial.py
--rw-r--r--   0 safwan     (501) staff       (20)      387 2019-06-03 00:43:50.000000 django-webpush-0.3.5/webpush/migrations/0002_auto_20190603_0005.py
--rw-r--r--   0 safwan     (501) staff       (20)      447 2023-03-14 17:57:26.000000 django-webpush-0.3.5/webpush/migrations/0003_subscriptioninfo_user_agent.py
--rw-r--r--   0 safwan     (501) staff       (20)      889 2023-03-14 17:57:26.000000 django-webpush-0.3.5/webpush/migrations/0004_auto_20220831_1500.py
--rw-r--r--   0 safwan     (501) staff       (20)        0 2018-02-13 23:42:43.000000 django-webpush-0.3.5/webpush/migrations/__init__.py
--rw-r--r--   0 safwan     (501) staff       (20)     1306 2023-03-14 17:57:26.000000 django-webpush-0.3.5/webpush/models.py
-drwxr-xr-x   0 safwan     (501) staff       (20)        0 2023-03-14 17:58:44.000000 django-webpush-0.3.5/webpush/static/
-drwxr-xr-x   0 safwan     (501) staff       (20)        0 2023-03-14 17:58:44.000000 django-webpush-0.3.5/webpush/static/webpush/
--rw-r--r--   0 safwan     (501) staff       (20)     7337 2023-03-14 17:57:26.000000 django-webpush-0.3.5/webpush/static/webpush/webpush.js
-drwxr-xr-x   0 safwan     (501) staff       (20)        0 2023-03-14 17:58:44.000000 django-webpush-0.3.5/webpush/templates/
--rw-r--r--   0 safwan     (501) staff       (20)      308 2020-03-28 06:22:02.000000 django-webpush-0.3.5/webpush/templates/webpush_button.html
--rw-r--r--   0 safwan     (501) staff       (20)      473 2022-01-11 20:26:58.000000 django-webpush-0.3.5/webpush/templates/webpush_header.html
--rw-r--r--   0 safwan     (501) staff       (20)     1288 2019-06-02 23:36:55.000000 django-webpush-0.3.5/webpush/templates/webpush_serviceworker.js
-drwxr-xr-x   0 safwan     (501) staff       (20)        0 2023-03-14 17:58:44.000000 django-webpush-0.3.5/webpush/templatetags/
--rw-r--r--   0 safwan     (501) staff       (20)        0 2018-02-13 23:42:43.000000 django-webpush-0.3.5/webpush/templatetags/__init__.py
--rw-r--r--   0 safwan     (501) staff       (20)      656 2020-03-28 06:22:02.000000 django-webpush-0.3.5/webpush/templatetags/webpush_notifications.py
--rw-r--r--   0 safwan     (501) staff       (20)       60 2018-02-13 23:42:43.000000 django-webpush-0.3.5/webpush/tests.py
--rw-r--r--   0 safwan     (501) staff       (20)      817 2022-01-11 20:26:58.000000 django-webpush-0.3.5/webpush/urls.py
--rw-r--r--   0 safwan     (501) staff       (20)     2671 2019-06-03 00:43:50.000000 django-webpush-0.3.5/webpush/utils.py
--rw-r--r--   0 safwan     (501) staff       (20)     2927 2023-03-14 17:57:26.000000 django-webpush-0.3.5/webpush/views.py
+drwxr-xr-x   0 safwan     (501) staff       (20)        0 2024-04-30 21:05:38.000000 django-webpush-0.3.6/
+-rw-r--r--   0 safwan     (501) staff       (20)    35147 2018-02-13 23:42:43.000000 django-webpush-0.3.6/LICENSE
+-rw-r--r--   0 safwan     (501) staff       (20)      108 2018-02-13 23:42:43.000000 django-webpush-0.3.6/MANIFEST.in
+-rw-r--r--   0 safwan     (501) staff       (20)     8700 2024-04-30 21:05:38.000000 django-webpush-0.3.6/PKG-INFO
+-rw-r--r--   0 safwan     (501) staff       (20)     7765 2024-04-30 21:01:28.000000 django-webpush-0.3.6/README.md
+drwxr-xr-x   0 safwan     (501) staff       (20)        0 2024-04-30 21:05:38.000000 django-webpush-0.3.6/django_webpush.egg-info/
+-rw-r--r--   0 safwan     (501) staff       (20)     8700 2024-04-30 21:05:38.000000 django-webpush-0.3.6/django_webpush.egg-info/PKG-INFO
+-rw-r--r--   0 safwan     (501) staff       (20)      919 2024-04-30 21:05:38.000000 django-webpush-0.3.6/django_webpush.egg-info/SOURCES.txt
+-rw-r--r--   0 safwan     (501) staff       (20)        1 2024-04-30 21:05:38.000000 django-webpush-0.3.6/django_webpush.egg-info/dependency_links.txt
+-rw-r--r--   0 safwan     (501) staff       (20)       18 2024-04-30 21:05:38.000000 django-webpush-0.3.6/django_webpush.egg-info/requires.txt
+-rw-r--r--   0 safwan     (501) staff       (20)        8 2024-04-30 21:05:38.000000 django-webpush-0.3.6/django_webpush.egg-info/top_level.txt
+-rw-r--r--   0 safwan     (501) staff       (20)       67 2024-04-30 21:05:38.000000 django-webpush-0.3.6/setup.cfg
+-rw-r--r--   0 safwan     (501) staff       (20)     1407 2024-04-30 21:02:28.000000 django-webpush-0.3.6/setup.py
+drwxr-xr-x   0 safwan     (501) staff       (20)        0 2024-04-30 21:05:38.000000 django-webpush-0.3.6/webpush/
+-rw-r--r--   0 safwan     (501) staff       (20)      409 2024-04-30 21:01:28.000000 django-webpush-0.3.6/webpush/__init__.py
+-rw-r--r--   0 safwan     (501) staff       (20)      744 2019-06-03 00:43:50.000000 django-webpush-0.3.6/webpush/admin.py
+-rw-r--r--   0 safwan     (501) staff       (20)      143 2024-04-30 21:01:28.000000 django-webpush-0.3.6/webpush/apps.py
+-rw-r--r--   0 safwan     (501) staff       (20)        0 2019-02-15 21:19:26.000000 django-webpush-0.3.6/webpush/config.py
+-rw-r--r--   0 safwan     (501) staff       (20)     1429 2023-03-14 17:57:26.000000 django-webpush-0.3.6/webpush/forms.py
+-rw-r--r--   0 safwan     (501) staff       (20)     1304 2024-04-30 21:01:28.000000 django-webpush-0.3.6/webpush/jinja2.py
+drwxr-xr-x   0 safwan     (501) staff       (20)        0 2024-04-30 21:05:38.000000 django-webpush-0.3.6/webpush/migrations/
+-rw-r--r--   0 safwan     (501) staff       (20)     1936 2019-02-15 21:19:26.000000 django-webpush-0.3.6/webpush/migrations/0001_initial.py
+-rw-r--r--   0 safwan     (501) staff       (20)      387 2019-06-03 00:43:50.000000 django-webpush-0.3.6/webpush/migrations/0002_auto_20190603_0005.py
+-rw-r--r--   0 safwan     (501) staff       (20)      447 2023-03-14 17:57:26.000000 django-webpush-0.3.6/webpush/migrations/0003_subscriptioninfo_user_agent.py
+-rw-r--r--   0 safwan     (501) staff       (20)      889 2023-03-14 17:57:26.000000 django-webpush-0.3.6/webpush/migrations/0004_auto_20220831_1500.py
+-rw-r--r--   0 safwan     (501) staff       (20)      873 2024-04-30 21:01:28.000000 django-webpush-0.3.6/webpush/migrations/0005_auto_20230614_1529.py
+-rw-r--r--   0 safwan     (501) staff       (20)        0 2018-02-13 23:42:43.000000 django-webpush-0.3.6/webpush/migrations/__init__.py
+-rw-r--r--   0 safwan     (501) staff       (20)     1318 2024-04-30 21:01:28.000000 django-webpush-0.3.6/webpush/models.py
+drwxr-xr-x   0 safwan     (501) staff       (20)        0 2024-04-30 21:05:38.000000 django-webpush-0.3.6/webpush/static/
+drwxr-xr-x   0 safwan     (501) staff       (20)        0 2024-04-30 21:05:38.000000 django-webpush-0.3.6/webpush/static/webpush/
+-rw-r--r--   0 safwan     (501) staff       (20)     7216 2024-04-30 21:01:28.000000 django-webpush-0.3.6/webpush/static/webpush/webpush.js
+drwxr-xr-x   0 safwan     (501) staff       (20)        0 2024-04-30 21:05:38.000000 django-webpush-0.3.6/webpush/templates/
+-rw-r--r--   0 safwan     (501) staff       (20)      308 2020-03-28 06:22:02.000000 django-webpush-0.3.6/webpush/templates/webpush_button.html
+-rw-r--r--   0 safwan     (501) staff       (20)      473 2022-01-11 20:26:58.000000 django-webpush-0.3.6/webpush/templates/webpush_header.html
+-rw-r--r--   0 safwan     (501) staff       (20)     1288 2019-06-02 23:36:55.000000 django-webpush-0.3.6/webpush/templates/webpush_serviceworker.js
+drwxr-xr-x   0 safwan     (501) staff       (20)        0 2024-04-30 21:05:38.000000 django-webpush-0.3.6/webpush/templatetags/
+-rw-r--r--   0 safwan     (501) staff       (20)        0 2018-02-13 23:42:43.000000 django-webpush-0.3.6/webpush/templatetags/__init__.py
+-rw-r--r--   0 safwan     (501) staff       (20)      656 2020-03-28 06:22:02.000000 django-webpush-0.3.6/webpush/templatetags/webpush_notifications.py
+-rw-r--r--   0 safwan     (501) staff       (20)       60 2018-02-13 23:42:43.000000 django-webpush-0.3.6/webpush/tests.py
+-rw-r--r--   0 safwan     (501) staff       (20)      817 2022-01-11 20:26:58.000000 django-webpush-0.3.6/webpush/urls.py
+-rw-r--r--   0 safwan     (501) staff       (20)     2948 2024-04-30 21:01:28.000000 django-webpush-0.3.6/webpush/utils.py
+-rw-r--r--   0 safwan     (501) staff       (20)     2937 2024-04-30 21:01:28.000000 django-webpush-0.3.6/webpush/views.py
```

### Comparing `django-webpush-0.3.5/LICENSE` & `django-webpush-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webpush-0.3.5/PKG-INFO` & `django-webpush-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webpush
-Version: 0.3.5
+Version: 0.3.6
 Summary: A simple Django package to integrate Web Push Notification in your Application
 Home-page: https://www.github.com/safwanrahman/django-webpush
 Author: Safwan Rahman
 Author-email: safwan.rahman15@gmail.com
 License: GNU Public License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -20,19 +20,19 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ﻿
 Django-Webpush
 ==============
-[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/safwan.rahman15@gmail.com)
+[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/safwanrahman)
 
 Django-Webpush is a Package made for integrating and sending [Web Push Notification](https://developer.mozilla.org/en/docs/Web/API/Push_API) in Django Application.
 
-Currently, it Supports Sending Push Notification to **Firefox 46+ and Chrome 52+**.
+Currently, it Supports Sending Push Notification to **Firefox 46+, Chrome 52+ and Apple devices on iOS 16.4+**.
 
 ----------
 
 
 Installation and Setup
 ----------------------
```

### Comparing `django-webpush-0.3.5/README.md` & `django-webpush-0.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ﻿
 Django-Webpush
 ==============
-[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/safwan.rahman15@gmail.com)
+[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/safwanrahman)
 
 Django-Webpush is a Package made for integrating and sending [Web Push Notification](https://developer.mozilla.org/en/docs/Web/API/Push_API) in Django Application.
 
-Currently, it Supports Sending Push Notification to **Firefox 46+ and Chrome 52+**.
+Currently, it Supports Sending Push Notification to **Firefox 46+, Chrome 52+ and Apple devices on iOS 16.4+**.
 
 ----------
 
 
 Installation and Setup
 ----------------------
```

### Comparing `django-webpush-0.3.5/django_webpush.egg-info/PKG-INFO` & `django-webpush-0.3.6/django_webpush.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webpush
-Version: 0.3.5
+Version: 0.3.6
 Summary: A simple Django package to integrate Web Push Notification in your Application
 Home-page: https://www.github.com/safwanrahman/django-webpush
 Author: Safwan Rahman
 Author-email: safwan.rahman15@gmail.com
 License: GNU Public License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -20,19 +20,19 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ﻿
 Django-Webpush
 ==============
-[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/safwan.rahman15@gmail.com)
+[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/safwanrahman)
 
 Django-Webpush is a Package made for integrating and sending [Web Push Notification](https://developer.mozilla.org/en/docs/Web/API/Push_API) in Django Application.
 
-Currently, it Supports Sending Push Notification to **Firefox 46+ and Chrome 52+**.
+Currently, it Supports Sending Push Notification to **Firefox 46+, Chrome 52+ and Apple devices on iOS 16.4+**.
 
 ----------
 
 
 Installation and Setup
 ----------------------
```

### Comparing `django-webpush-0.3.5/django_webpush.egg-info/SOURCES.txt` & `django-webpush-0.3.6/django_webpush.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 django_webpush.egg-info/PKG-INFO
 django_webpush.egg-info/SOURCES.txt
 django_webpush.egg-info/dependency_links.txt
 django_webpush.egg-info/requires.txt
 django_webpush.egg-info/top_level.txt
 webpush/__init__.py
 webpush/admin.py
+webpush/apps.py
 webpush/config.py
 webpush/forms.py
 webpush/jinja2.py
 webpush/models.py
 webpush/tests.py
 webpush/urls.py
 webpush/utils.py
 webpush/views.py
 webpush/migrations/0001_initial.py
 webpush/migrations/0002_auto_20190603_0005.py
 webpush/migrations/0003_subscriptioninfo_user_agent.py
 webpush/migrations/0004_auto_20220831_1500.py
+webpush/migrations/0005_auto_20230614_1529.py
 webpush/migrations/__init__.py
 webpush/static/webpush/webpush.js
 webpush/templates/webpush_button.html
 webpush/templates/webpush_header.html
 webpush/templates/webpush_serviceworker.js
 webpush/templatetags/__init__.py
 webpush/templatetags/webpush_notifications.py
```

### Comparing `django-webpush-0.3.5/setup.py` & `django-webpush-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-webpush',
-    version='0.3.5',
+    version='0.3.6',
     packages=find_packages(),
     include_package_data=True,
     license='GNU Public License',
     description='A simple Django package to integrate Web Push Notification in your Application',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://www.github.com/safwanrahman/django-webpush',
@@ -30,10 +30,10 @@
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
     install_requires=[
-        'pywebpush==1.9.4'
+        'pywebpush>=1.14.0'
     ]
 )
```

### Comparing `django-webpush-0.3.5/webpush/admin.py` & `django-webpush-0.3.6/webpush/admin.py`

 * *Files identical despite different names*

### Comparing `django-webpush-0.3.5/webpush/forms.py` & `django-webpush-0.3.6/webpush/forms.py`

 * *Files identical despite different names*

### Comparing `django-webpush-0.3.5/webpush/jinja2.py` & `django-webpush-0.3.6/webpush/jinja2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import arrow
 from django.template.loader import render_to_string
 from django.utils.safestring import mark_safe
-from jinja2 import contextfunction
-
+try:
+    from jinja2 import pass_context as pass_context
+except ImportError:
+    # NOTE(willkg): We can get rid of this when we stop supporting Jinja2 < 3.
+    from jinja2 import contextfunction as pass_context
+    
 from jinja2 import nodes
 from jinja2.ext import Extension
 from markupsafe import Markup
 
 from webpush.utils import get_templatetag_context
 
 
 class WebPushExtension(Extension):
 
     def __init__(self, environment):
         super(WebPushExtension, self).__init__(environment)
         environment.globals['webpush_header'] = self.webpush_header
         environment.globals['webpush_button'] = self.webpush_button
 
-    @contextfunction
+    @pass_context
     def webpush_header(self, context):
         template_context = get_templatetag_context(context)
         data = render_to_string('webpush_header.html', template_context, using='django')
         return mark_safe(data)
 
-    @contextfunction
+    @pass_context
     def webpush_button(self, context, with_class=None):
         template_context = get_templatetag_context(context)
         if with_class:
             template_context['class'] = with_class
         data = render_to_string('webpush_button.html', template_context, using='django')
         return mark_safe(data)
```

### Comparing `django-webpush-0.3.5/webpush/migrations/0001_initial.py` & `django-webpush-0.3.6/webpush/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webpush-0.3.5/webpush/migrations/0004_auto_20220831_1500.py` & `django-webpush-0.3.6/webpush/migrations/0004_auto_20220831_1500.py`

 * *Files identical despite different names*

### Comparing `django-webpush-0.3.5/webpush/models.py` & `django-webpush-0.3.6/webpush/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class Group(models.Model):
     name = models.CharField(max_length=255, unique=True)
 
 
 class SubscriptionInfo(models.Model):
     browser = models.CharField(max_length=100)
-    user_agent = models.CharField(max_length=500)
+    user_agent = models.CharField(max_length=500, blank=True)
     endpoint = models.URLField(max_length=500)
     auth = models.CharField(max_length=100)
     p256dh = models.CharField(max_length=100)
 
 
 class PushInformation(models.Model):
     user = models.ForeignKey(settings.AUTH_USER_MODEL, related_name='webpush_info', blank=True, null=True, on_delete=models.CASCADE)
```

### Comparing `django-webpush-0.3.5/webpush/static/webpush/webpush.js` & `django-webpush-0.3.6/webpush/static/webpush/webpush.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,14 +3,16 @@
 var isPushEnabled = false,
     registration,
     subBtn;
 
 window.addEventListener('load', function() {
     subBtn = document.getElementById('webpush-subscribe-button');
 
+    subBtn.textContent = gettext('Subscribe to Push Messaging');
+
     subBtn.addEventListener('click',
         function() {
             subBtn.disabled = true;
             if (isPushEnabled) {
                 return unsubscribe(registration);
             }
             return subscribe(registration);
@@ -32,34 +34,31 @@
     }
 
     // Once the service worker is registered set the initial state
     function initialiseState(reg) {
         // Are Notifications supported in the service worker?
         if (!(reg.showNotification)) {
             // Show a message and activate the button
-            subBtn.textContent = 'Subscribe to Push Messaging';
             showMessage(gettext('Showing notifications are not supported in your browser.'));
             return;
         }
 
         // Check the current Notification permission.
         // If its denied, it's a permanent block until the
         // user changes the permission
         if (Notification.permission === 'denied') {
             // Show a message and activate the button
-            subBtn.textContent = gettext('Subscribe to Push Messaging');
             subBtn.disabled = false;
             showMessage(gettext('Push notifications are blocked by your browser.'));
             return;
         }
 
         // Check if push messaging is supported
         if (!('PushManager' in window)) {
             // Show a message and activate the button
-            subBtn.textContent = 'Subscribe to Push Messaging';
             subBtn.disabled = false;
             showMessage(gettext('Push notifications are not available in your browser.'));
             return;
         }
 
         // We need to get subscription state for push notifications and send the information to server
         reg.pushManager.getSubscription().then(
```

### Comparing `django-webpush-0.3.5/webpush/templates/webpush_serviceworker.js` & `django-webpush-0.3.6/webpush/templates/webpush_serviceworker.js`

 * *Files identical despite different names*

### Comparing `django-webpush-0.3.5/webpush/templatetags/webpush_notifications.py` & `django-webpush-0.3.6/webpush/templatetags/webpush_notifications.py`

 * *Files identical despite different names*

### Comparing `django-webpush-0.3.5/webpush/urls.py` & `django-webpush-0.3.6/webpush/urls.py`

 * *Files identical despite different names*

### Comparing `django-webpush-0.3.5/webpush/utils.py` & `django-webpush-0.3.6/webpush/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,23 +9,29 @@
     # Get all the push_info of the user
 
     push_infos = user.webpush_info.select_related("subscription")
     for push_info in push_infos:
         _send_notification(push_info.subscription, payload, ttl)
 
 
-def send_notification_to_group(group_name, payload, ttl=0):
+def send_notification_to_group(group_name, payload, ttl=0, exclude_user_id=None):
     from .models import Group
-    # Get all the subscription related to the group
 
     push_infos = Group.objects.get(name=group_name).webpush_info.select_related("subscription")
+
+    # Exclude the current user from receiving notifications if they are part of the target group.
+    # This prevents users from receiving redundant notifications when they trigger an event themselves.
+    if exclude_user_id is not None:
+        push_infos = push_infos.exclude(user__id=exclude_user_id)
+
     for push_info in push_infos:
         _send_notification(push_info.subscription, payload, ttl)
 
 
+
 def send_to_subscription(subscription, payload, ttl=0):
     return _send_notification(subscription, payload, ttl)
 
 
 def _send_notification(subscription, payload, ttl):
     subscription_data = _process_subscription_info(subscription)
     vapid_data = {}
```

### Comparing `django-webpush-0.3.5/webpush/views.py` & `django-webpush-0.3.6/webpush/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
     """Process the subscription data according to out model"""
     subscription_data = post_data.pop("subscription", {})
     # As our database saves the auth and p256dh key in separate field,
     # we need to refactor it and insert the auth and p256dh keys in the same dictionary
     keys = subscription_data.pop("keys", {})
     subscription_data.update(keys)
     # Insert the browser name and user agent
-    subscription_data["browser"] = post_data.pop("browser")
-    subscription_data["user_agent"] = post_data.pop("user_agent")
+    subscription_data["browser"] = post_data.pop("browser", None)
+    subscription_data["user_agent"] = post_data.pop("user_agent", '')
     return subscription_data
 
 
 class ServiceWorkerView(TemplateView):
     """
     Service Worker need to be loaded from same domain.
     Therefore, use TemplateView in order to server the webpush_serviceworker.js
```

