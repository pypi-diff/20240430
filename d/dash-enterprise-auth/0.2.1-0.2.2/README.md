# Comparing `tmp/dash_enterprise_auth-0.2.1.tar.gz` & `tmp/dash_enterprise_auth-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_enterprise_auth-0.2.1.tar", last modified: Fri Oct 13 15:59:51 2023, max compression
+gzip compressed data, was "dash_enterprise_auth-0.2.2.tar", last modified: Tue Apr 30 19:29:54 2024, max compression
```

## Comparing `dash_enterprise_auth-0.2.1.tar` & `dash_enterprise_auth-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-10-13 15:59:51.467739 dash_enterprise_auth-0.2.1/
--rw-r--r--   0 alex       (501) staff       (20)     1078 2023-09-20 15:18:07.000000 dash_enterprise_auth-0.2.1/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)       18 2021-10-04 19:59:18.000000 dash_enterprise_auth-0.2.1/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)     1245 2023-10-13 15:59:51.467303 dash_enterprise_auth-0.2.1/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      397 2023-09-20 15:18:07.000000 dash_enterprise_auth-0.2.1/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-10-13 15:59:51.462491 dash_enterprise_auth-0.2.1/dash_enterprise_auth/
--rw-r--r--   0 alex       (501) staff       (20)     4526 2023-09-20 17:25:42.000000 dash_enterprise_auth-0.2.1/dash_enterprise_auth/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)       22 2023-10-13 15:57:40.000000 dash_enterprise_auth-0.2.1/dash_enterprise_auth/version.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-10-13 15:59:51.465752 dash_enterprise_auth-0.2.1/dash_enterprise_auth.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     1245 2023-10-13 15:59:51.000000 dash_enterprise_auth-0.2.1/dash_enterprise_auth.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      357 2023-10-13 15:59:51.000000 dash_enterprise_auth-0.2.1/dash_enterprise_auth.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-10-13 15:59:51.000000 dash_enterprise_auth-0.2.1/dash_enterprise_auth.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)      150 2023-10-13 15:59:51.000000 dash_enterprise_auth-0.2.1/dash_enterprise_auth.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       21 2023-10-13 15:59:51.000000 dash_enterprise_auth-0.2.1/dash_enterprise_auth.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-10-13 15:59:51.467908 dash_enterprise_auth-0.2.1/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     1490 2023-10-13 15:57:40.000000 dash_enterprise_auth-0.2.1/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-10-13 15:59:51.466333 dash_enterprise_auth-0.2.1/tests/
--rw-r--r--   0 alex       (501) staff       (20)     2435 2023-09-20 17:25:42.000000 dash_enterprise_auth-0.2.1/tests/test_dash_enterprise_auth.py
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2024-04-30 19:29:54.861909 dash_enterprise_auth-0.2.2/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1078 2024-04-29 14:20:47.000000 dash_enterprise_auth-0.2.2/LICENSE
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       18 2024-04-29 14:20:47.000000 dash_enterprise_auth-0.2.2/MANIFEST.in
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1265 2024-04-30 19:29:54.861909 dash_enterprise_auth-0.2.2/PKG-INFO
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      397 2024-04-29 14:20:47.000000 dash_enterprise_auth-0.2.2/README.md
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2024-04-30 19:29:54.861909 dash_enterprise_auth-0.2.2/dash_enterprise_auth/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     4573 2024-04-29 14:20:47.000000 dash_enterprise_auth-0.2.2/dash_enterprise_auth/__init__.py
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       22 2024-04-30 19:28:27.000000 dash_enterprise_auth-0.2.2/dash_enterprise_auth/version.py
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2024-04-30 19:29:54.861909 dash_enterprise_auth-0.2.2/dash_enterprise_auth.egg-info/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1265 2024-04-30 19:29:54.000000 dash_enterprise_auth-0.2.2/dash_enterprise_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      322 2024-04-30 19:29:54.000000 dash_enterprise_auth-0.2.2/dash_enterprise_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)        1 2024-04-30 19:29:54.000000 dash_enterprise_auth-0.2.2/dash_enterprise_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      146 2024-04-30 19:29:54.000000 dash_enterprise_auth-0.2.2/dash_enterprise_auth.egg-info/requires.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       21 2024-04-30 19:29:54.000000 dash_enterprise_auth-0.2.2/dash_enterprise_auth.egg-info/top_level.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       38 2024-04-30 19:29:54.861909 dash_enterprise_auth-0.2.2/setup.cfg
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1486 2024-04-30 19:28:27.000000 dash_enterprise_auth-0.2.2/setup.py
```

### Comparing `dash_enterprise_auth-0.2.1/LICENSE` & `dash_enterprise_auth-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_enterprise_auth-0.2.1/PKG-INFO` & `dash_enterprise_auth-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: dash_enterprise_auth
-Version: 0.2.1
+Version: 0.2.2
 Summary: Authentication integrations for apps using Dash Enterprise
 Home-page: https://plotly.com/dash
 Author: Antoine Roy-Gobeil
 Author-email: antoine@plotly.com
 License: MIT
 Keywords: dash dash-enterprise dash-auth plotly
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Dash
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -34,7 +35,9 @@
 def private_data(...):
     username = auth.get_username()
     if username:
         return get_view_for_user(username)
     else:
         return public_view()
 ```
+
+
```

### Comparing `dash_enterprise_auth-0.2.1/dash_enterprise_auth/__init__.py` & `dash_enterprise_auth-0.2.2/dash_enterprise_auth/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import json as _json
 import urllib as _urllib
 from typing import Any
 
 import flask as _flask
 import jwt as _jwt
 import requests as _requests
+import traceback
 
 
 import dash as _dash
 if hasattr(_dash, "dcc"):
     _dcc = _dash.dcc
 else:
     import dash_core_components as _dcc
@@ -133,14 +134,15 @@
             response.raise_for_status()
             data = response.json()
             info.update(data)
 
         return info
     except Exception as e:
         print("JWT decode error: " + repr(e))
+        traceback.print_exc()
     return {}
 
 
 @_need_request_context
 def get_username():
     """
     Get the current user.
```

### Comparing `dash_enterprise_auth-0.2.1/dash_enterprise_auth.egg-info/PKG-INFO` & `dash_enterprise_auth-0.2.2/dash_enterprise_auth.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: dash-enterprise-auth
-Version: 0.2.1
+Version: 0.2.2
 Summary: Authentication integrations for apps using Dash Enterprise
 Home-page: https://plotly.com/dash
 Author: Antoine Roy-Gobeil
 Author-email: antoine@plotly.com
 License: MIT
 Keywords: dash dash-enterprise dash-auth plotly
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Dash
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -34,7 +35,9 @@
 def private_data(...):
     username = auth.get_username()
     if username:
         return get_view_for_user(username)
     else:
         return public_view()
 ```
+
+
```

### Comparing `dash_enterprise_auth-0.2.1/setup.py` & `dash_enterprise_auth-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     author_email="antoine@plotly.com",
     license="MIT",
     packages=[
         "dash_enterprise_auth"
     ],
     install_requires=[
         "dash",
-        "Flask>=1.0.4,<2.3.0",
-        "Werkzeug<2.3.0",
+        "Flask>=1.0.4,<3.1",
+        "Werkzeug<3.1",
         "requests[security]",
         "PyJWT",
         'cryptography;python_version>="3.7"',
         'cryptography<3.4;python_version<"3.7"'
     ],
     python_requires=">=3.6",
     url="https://plotly.com/dash",
```

