# Comparing `tmp/hurricaneapi-0.1.5.tar.gz` & `tmp/hurricaneapi-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hurricaneapi-0.1.5.tar", last modified: Sun Jun 18 13:41:13 2023, max compression
+gzip compressed data, was "hurricaneapi-0.1.7.tar", last modified: Tue Apr 30 09:54:44 2024, max compression
```

## Comparing `hurricaneapi-0.1.5.tar` & `hurricaneapi-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 13:41:13.458942 hurricaneapi-0.1.5/
--rw-rw-rw-   0        0        0     1093 2023-02-25 18:34:13.000000 hurricaneapi-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      282 2023-06-18 13:41:13.458942 hurricaneapi-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-02-25 18:34:13.000000 hurricaneapi-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 13:41:13.444942 hurricaneapi-0.1.5/hurricaneapi/
--rw-rw-rw-   0        0        0      107 2023-06-18 13:41:04.000000 hurricaneapi-0.1.5/hurricaneapi/__init__.py
--rw-rw-rw-   0        0        0     1538 2023-03-01 18:38:34.000000 hurricaneapi-0.1.5/hurricaneapi/application.py
-drwxrwxrwx   0        0        0        0 2023-06-18 13:41:13.455942 hurricaneapi-0.1.5/hurricaneapi/responses/
--rw-rw-rw-   0        0        0      254 2023-03-01 18:51:02.000000 hurricaneapi-0.1.5/hurricaneapi/responses/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-01 18:38:35.000000 hurricaneapi-0.1.5/hurricaneapi/responses/file_response.py
--rw-rw-rw-   0        0        0      365 2023-03-01 18:43:47.000000 hurricaneapi-0.1.5/hurricaneapi/responses/html_response.py
--rw-rw-rw-   0        0        0      507 2023-03-01 18:48:19.000000 hurricaneapi-0.1.5/hurricaneapi/responses/json_response.py
--rw-rw-rw-   0        0        0      371 2023-03-01 18:50:37.000000 hurricaneapi-0.1.5/hurricaneapi/responses/plain_text_response.py
--rw-rw-rw-   0        0        0        0 2023-03-01 18:38:35.000000 hurricaneapi-0.1.5/hurricaneapi/responses/redirect_response.py
--rw-rw-rw-   0        0        0     2332 2023-03-01 18:36:49.000000 hurricaneapi-0.1.5/hurricaneapi/responses/response.py
--rw-rw-rw-   0        0        0        0 2023-03-01 18:38:35.000000 hurricaneapi-0.1.5/hurricaneapi/responses/streaming_response.py
-drwxrwxrwx   0        0        0        0 2023-06-18 13:41:13.457941 hurricaneapi-0.1.5/hurricaneapi/routing/
--rw-rw-rw-   0        0        0        0 2023-06-18 13:38:35.000000 hurricaneapi-0.1.5/hurricaneapi/routing/__init__.py
--rw-rw-rw-   0        0        0      351 2023-03-01 18:36:49.000000 hurricaneapi-0.1.5/hurricaneapi/routing/route.py
--rw-rw-rw-   0        0        0     1143 2023-03-01 18:36:49.000000 hurricaneapi-0.1.5/hurricaneapi/routing/router.py
-drwxrwxrwx   0        0        0        0 2023-06-18 13:41:13.448943 hurricaneapi-0.1.5/hurricaneapi.egg-info/
--rw-rw-rw-   0        0        0      282 2023-06-18 13:41:13.000000 hurricaneapi-0.1.5/hurricaneapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      702 2023-06-18 13:41:13.000000 hurricaneapi-0.1.5/hurricaneapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 13:41:13.000000 hurricaneapi-0.1.5/hurricaneapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-18 13:41:13.000000 hurricaneapi-0.1.5/hurricaneapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-18 13:41:13.000000 hurricaneapi-0.1.5/hurricaneapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      455 2023-06-18 13:11:47.000000 hurricaneapi-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 13:41:13.458942 hurricaneapi-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      448 2023-06-18 13:41:04.000000 hurricaneapi-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:54:44.433414 hurricaneapi-0.1.7/
+-rw-rw-rw-   0        0        0     1093 2023-02-25 18:34:13.000000 hurricaneapi-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      493 2024-04-30 09:54:44.433414 hurricaneapi-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 09:54:44.397415 hurricaneapi-0.1.7/hurricaneapi/
+-rw-rw-rw-   0        0        0      107 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/__init__.py
+-rw-rw-rw-   0        0        0     5334 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/application.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:54:44.414431 hurricaneapi-0.1.7/hurricaneapi/middleware/
+-rw-rw-rw-   0        0        0      219 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/middleware/__init__.py
+-rw-rw-rw-   0        0        0      292 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/middleware/base_middleware.py
+-rw-rw-rw-   0        0        0     1931 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/middleware/cors_middleware.py
+-rw-rw-rw-   0        0        0      928 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/middleware/trusted_host_middleware.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:54:44.426429 hurricaneapi-0.1.7/hurricaneapi/responses/
+-rw-rw-rw-   0        0        0      388 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/responses/__init__.py
+-rw-rw-rw-   0        0        0     2852 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/responses/file_response.py
+-rw-rw-rw-   0        0        0      426 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/responses/html_response.py
+-rw-rw-rw-   0        0        0      568 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/responses/json_response.py
+-rw-rw-rw-   0        0        0      432 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/responses/plain_text_response.py
+-rw-rw-rw-   0        0        0      959 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/responses/redirect_response.py
+-rw-rw-rw-   0        0        0     2332 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/responses/response.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:54:44.431414 hurricaneapi-0.1.7/hurricaneapi/routing/
+-rw-rw-rw-   0        0        0        0 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/routing/__init__.py
+-rw-rw-rw-   0        0        0      351 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/routing/route.py
+-rw-rw-rw-   0        0        0     2461 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/hurricaneapi/routing/router.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:54:44.407417 hurricaneapi-0.1.7/hurricaneapi.egg-info/
+-rw-rw-rw-   0        0        0      493 2024-04-30 09:54:44.000000 hurricaneapi-0.1.7/hurricaneapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      865 2024-04-30 09:54:44.000000 hurricaneapi-0.1.7/hurricaneapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 09:54:44.000000 hurricaneapi-0.1.7/hurricaneapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-18 13:41:13.000000 hurricaneapi-0.1.7/hurricaneapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       48 2024-04-30 09:54:44.000000 hurricaneapi-0.1.7/hurricaneapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 09:54:44.000000 hurricaneapi-0.1.7/hurricaneapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      804 2024-04-30 09:25:15.000000 hurricaneapi-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 09:54:44.434414 hurricaneapi-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      561 2024-04-30 09:54:39.000000 hurricaneapi-0.1.7/setup.py
```

### Comparing `hurricaneapi-0.1.5/LICENSE` & `hurricaneapi-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hurricaneapi-0.1.5/hurricaneapi/responses/response.py` & `hurricaneapi-0.1.7/hurricaneapi/responses/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional, Mapping, List
+from typing import Any, List, Mapping, Optional
 
 
 class Response:
     def __init__(
         self,
         content: Any = None,
         media_type: Optional[str] = None,
```

