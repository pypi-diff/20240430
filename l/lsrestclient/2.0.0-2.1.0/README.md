# Comparing `tmp/lsrestclient-2.0.0.tar.gz` & `tmp/lsrestclient-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsrestclient-2.0.0.tar", max compression
+gzip compressed data, was "lsrestclient-2.1.0.tar", max compression
```

## Comparing `lsrestclient-2.0.0.tar` & `lsrestclient-2.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6181 2023-07-25 09:41:02.649481 lsrestclient-2.0.0/README.md
--rw-r--r--   0        0        0       72 2023-07-27 14:36:50.038756 lsrestclient-2.0.0/lsrestclient/__init__.py
--rw-r--r--   0        0        0      468 2023-10-13 13:20:34.663834 lsrestclient-2.0.0/lsrestclient/auth.py
--rw-r--r--   0        0        0    11159 2024-04-08 13:43:39.869341 lsrestclient-2.0.0/lsrestclient/client.py
--rw-r--r--   0        0        0        0 2023-08-23 13:22:18.238446 lsrestclient-2.0.0/lsrestclient/contexts/__init__.py
--rw-r--r--   0        0        0      753 2023-08-23 13:22:18.238446 lsrestclient-2.0.0/lsrestclient/contexts/bearer_token.py
--rw-r--r--   0        0        0     2197 2024-04-25 08:10:43.168133 lsrestclient-2.0.0/lsrestclient/exceptions.py
--rw-r--r--   0        0        0      239 2023-10-11 08:49:21.282413 lsrestclient-2.0.0/lsrestclient/fixtures.py
--rw-r--r--   0        0        0     1376 2024-04-25 08:10:43.176133 lsrestclient-2.0.0/lsrestclient/mock.py
--rw-r--r--   0        0        0     1923 2024-04-08 14:47:34.966071 lsrestclient-2.0.0/lsrestclient/response.py
--rw-r--r--   0        0        0      871 2024-04-25 08:11:39.083721 lsrestclient-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     6748 1970-01-01 00:00:00.000000 lsrestclient-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6181 2023-07-25 09:41:02.000000 lsrestclient-2.1.0/README.md
+-rw-r--r--   0        0        0       72 2023-07-27 14:36:50.000000 lsrestclient-2.1.0/lsrestclient/__init__.py
+-rw-r--r--   0        0        0      468 2023-10-13 13:20:34.000000 lsrestclient-2.1.0/lsrestclient/auth.py
+-rw-r--r--   0        0        0    11159 2024-04-08 13:43:39.000000 lsrestclient-2.1.0/lsrestclient/client.py
+-rw-r--r--   0        0        0        0 2023-08-23 13:22:18.000000 lsrestclient-2.1.0/lsrestclient/contexts/__init__.py
+-rw-r--r--   0        0        0      753 2023-08-23 13:22:18.000000 lsrestclient-2.1.0/lsrestclient/contexts/bearer_token.py
+-rw-r--r--   0        0        0     2197 2024-04-25 08:10:43.000000 lsrestclient-2.1.0/lsrestclient/exceptions.py
+-rw-r--r--   0        0        0      239 2023-10-11 08:49:21.000000 lsrestclient-2.1.0/lsrestclient/fixtures.py
+-rw-r--r--   0        0        0     1376 2024-04-25 08:10:43.000000 lsrestclient-2.1.0/lsrestclient/mock.py
+-rw-r--r--   0        0        0     2165 2024-04-30 12:45:15.800990 lsrestclient-2.1.0/lsrestclient/response.py
+-rw-r--r--   0        0        0      871 2024-04-30 12:47:34.256787 lsrestclient-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6748 1970-01-01 00:00:00.000000 lsrestclient-2.1.0/PKG-INFO
```

### Comparing `lsrestclient-2.0.0/README.md` & `lsrestclient-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lsrestclient-2.0.0/lsrestclient/client.py` & `lsrestclient-2.1.0/lsrestclient/client.py`

 * *Files identical despite different names*

### Comparing `lsrestclient-2.0.0/lsrestclient/contexts/bearer_token.py` & `lsrestclient-2.1.0/lsrestclient/contexts/bearer_token.py`

 * *Files identical despite different names*

### Comparing `lsrestclient-2.0.0/lsrestclient/exceptions.py` & `lsrestclient-2.1.0/lsrestclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `lsrestclient-2.0.0/lsrestclient/mock.py` & `lsrestclient-2.1.0/lsrestclient/mock.py`

 * *Files identical despite different names*

### Comparing `lsrestclient-2.0.0/lsrestclient/response.py` & `lsrestclient-2.1.0/lsrestclient/response.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Optional
 
 import lsjsonclasses
 import pydash
 from requests import Response
 from requests.structures import CaseInsensitiveDict
 
-
 @dataclass
 class LsRestClientResponse:
     """
     Represents a response from the LsRestClient.
     """
 
     status_code: int
@@ -32,17 +31,24 @@
         :param response: The requests Response object.
         :type response: Response
         :return: An instance of LsRestClientResponse representing the response.
         :rtype: LsRestClientResponse
         """
 
         encoding = pydash.get(response, "encoding", None)
+        headers = pydash.get(response, "headers", None)
+        content_type = headers.get("Content-Type", None)
+        if content_type == 'application/pdf':
+            content = response.content
+        else:
+            content = response.content.decode("utf8" if encoding is None else encoding)
+
         return cls(
             status_code=response.status_code,
-            content=response.content.decode("utf8" if encoding is None else encoding),
+            content=content,
             headers=response.headers,
         )
 
     @classmethod
     def from_dict(cls, status_code: int = 200, data: dict = None, headers: CaseInsensitiveDict = None):
         """
         Converts a dictionary into an instance of the LsRestClientResponse class.
```

### Comparing `lsrestclient-2.0.0/pyproject.toml` & `lsrestclient-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lsrestclient"
-version = "2.0.0"
+version = "2.1.0"
 description = "REST Api Client"
 authors = ["mba <bartel@electronic-shop.lu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
```

### Comparing `lsrestclient-2.0.0/PKG-INFO` & `lsrestclient-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsrestclient
-Version: 2.0.0
+Version: 2.1.0
 Summary: REST Api Client
 Author: mba
 Author-email: bartel@electronic-shop.lu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

