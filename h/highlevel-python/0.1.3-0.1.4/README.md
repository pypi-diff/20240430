# Comparing `tmp/highlevel_python-0.1.3.tar.gz` & `tmp/highlevel_python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highlevel_python-0.1.3.tar", max compression
+gzip compressed data, was "highlevel_python-0.1.4.tar", max compression
```

## Comparing `highlevel_python-0.1.3.tar` & `highlevel_python-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-25 14:16:23.563971 highlevel_python-0.1.3/highlevel/__init__.py
--rw-r--r--   0        0        0     4706 2024-04-25 14:16:23.563971 highlevel_python-0.1.3/highlevel/client.py
--rw-r--r--   0        0        0      143 2024-04-25 14:16:23.564970 highlevel_python-0.1.3/highlevel/exceptions.py
--rw-r--r--   0        0        0      437 2024-04-25 14:16:23.565970 highlevel_python-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1596 2024-04-25 14:16:23.562971 highlevel_python-0.1.3/README.md
--rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 highlevel_python-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-25 14:16:23.563971 highlevel_python-0.1.4/highlevel/__init__.py
+-rw-r--r--   0        0        0     4697 2024-04-30 19:39:19.709088 highlevel_python-0.1.4/highlevel/client.py
+-rw-r--r--   0        0        0      143 2024-04-25 14:16:23.564970 highlevel_python-0.1.4/highlevel/exceptions.py
+-rw-r--r--   0        0        0      437 2024-04-30 19:39:19.716101 highlevel_python-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1596 2024-04-25 14:16:23.562971 highlevel_python-0.1.4/README.md
+-rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 highlevel_python-0.1.4/PKG-INFO
```

### Comparing `highlevel_python-0.1.3/highlevel/client.py` & `highlevel_python-0.1.4/highlevel/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from urllib.parse import urlencode
 from requests_oauthlib import OAuth2Session
 from typing import Optional, Union, Dict, Any
 
 from highlevel.exceptions import UnauthorizedError, WrongFormatInputError
 
 
-class HighLevelClient:
+class Client:
     BASE_URL = "https://api.highlevel.com/"
     AUTH_URL = "https://api.highlevel.com/oauth/authorize"
     TOKEN_URL = "https://api.highlevel.com/oauth/token"
     HEADERS = {"Content-Type": "application/json", "Accept": "application/json"}
 
     def __init__(
         self,
```

### Comparing `highlevel_python-0.1.3/README.md` & `highlevel_python-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `highlevel_python-0.1.3/PKG-INFO` & `highlevel_python-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highlevel-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: API wrapper for Highlevel written in Python
 License: MIT
 Author: Gearplug Team
 Author-email: apps@gearplug.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

