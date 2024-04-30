# Comparing `tmp/drf_simple_api_errors-1.0.0.tar.gz` & `tmp/drf_simple_api_errors-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_simple_api_errors-1.0.0.tar", max compression
+gzip compressed data, was "drf_simple_api_errors-1.0.1.tar", max compression
```

## Comparing `drf_simple_api_errors-1.0.0.tar` & `drf_simple_api_errors-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1082 2024-04-26 20:19:30.955622 drf_simple_api_errors-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     6179 2024-04-26 20:19:30.955622 drf_simple_api_errors-1.0.0/README.md
--rw-r--r--   0        0        0      105 2024-04-26 20:19:30.955622 drf_simple_api_errors-1.0.0/drf_simple_api_errors/__init__.py
--rw-r--r--   0        0        0      108 2024-04-26 20:19:30.955622 drf_simple_api_errors-1.0.0/drf_simple_api_errors/apps.py
--rw-r--r--   0        0        0     2465 2024-04-26 20:19:30.955622 drf_simple_api_errors-1.0.0/drf_simple_api_errors/exception_handler.py
--rw-r--r--   0        0        0      391 2024-04-26 20:19:30.955622 drf_simple_api_errors-1.0.0/drf_simple_api_errors/exceptions.py
--rw-r--r--   0        0        0     2248 2024-04-26 20:19:30.955622 drf_simple_api_errors-1.0.0/drf_simple_api_errors/handlers.py
--rw-r--r--   0        0        0      414 2024-04-26 20:19:30.955622 drf_simple_api_errors-1.0.0/drf_simple_api_errors/settings.py
--rw-r--r--   0        0        0     1008 2024-04-26 20:19:30.955622 drf_simple_api_errors-1.0.0/drf_simple_api_errors/utils.py
--rw-r--r--   0        0        0     1957 2024-04-26 20:19:30.955622 drf_simple_api_errors-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7515 1970-01-01 00:00:00.000000 drf_simple_api_errors-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-30 18:44:15.284941 drf_simple_api_errors-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     6572 2024-04-30 18:44:15.284941 drf_simple_api_errors-1.0.1/README.md
+-rw-r--r--   0        0        0      105 2024-04-30 18:44:15.284941 drf_simple_api_errors-1.0.1/drf_simple_api_errors/__init__.py
+-rw-r--r--   0        0        0      108 2024-04-30 18:44:15.284941 drf_simple_api_errors-1.0.1/drf_simple_api_errors/apps.py
+-rw-r--r--   0        0        0     2465 2024-04-30 18:44:15.284941 drf_simple_api_errors-1.0.1/drf_simple_api_errors/exception_handler.py
+-rw-r--r--   0        0        0      391 2024-04-30 18:44:15.284941 drf_simple_api_errors-1.0.1/drf_simple_api_errors/exceptions.py
+-rw-r--r--   0        0        0     2248 2024-04-30 18:44:15.284941 drf_simple_api_errors-1.0.1/drf_simple_api_errors/handlers.py
+-rw-r--r--   0        0        0      414 2024-04-30 18:44:15.284941 drf_simple_api_errors-1.0.1/drf_simple_api_errors/settings.py
+-rw-r--r--   0        0        0     1008 2024-04-30 18:44:15.284941 drf_simple_api_errors-1.0.1/drf_simple_api_errors/utils.py
+-rw-r--r--   0        0        0     2048 2024-04-30 18:44:15.284941 drf_simple_api_errors-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7908 1970-01-01 00:00:00.000000 drf_simple_api_errors-1.0.1/PKG-INFO
```

### Comparing `drf_simple_api_errors-1.0.0/LICENSE.md` & `drf_simple_api_errors-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `drf_simple_api_errors-1.0.0/README.md` & `drf_simple_api_errors-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # Django Rest Framework Simple API Errors
 
+![PyPI](https://img.shields.io/pypi/v/drf-simple-api-errors)
+![test workflow](https://github.com/gripep/drf-simple-api-errors/actions/workflows/build.yaml/badge.svg)
+[![codecov](https://codecov.io/gh/gripep/drf-simple-api-errors/graph/badge.svg?token=1LJV518KMD)](https://codecov.io/gh/gripep/drf-simple-api-errors)
+![pyversions](https://img.shields.io/pypi/pyversions/drf-simple-api-errors.svg)
+
 ## What is this?
 
-A library for [Django Rest Framework](https://www.django-rest-framework.org/) returning **consistent and easy-to-parse API error messages**.
+A library for [Django Rest Framework](https://www.django-rest-framework.org/) returning **consistent, predictable and easy-to-parse API error messages**.
 
 This library was built with [RFC7807](https://tools.ietf.org/html/rfc7807) guidelines in mind, but with a small twist: it defines a "problem detail" as a `list` but it still serves as a way to include errors in a predictable and easy-to-parse format for any API consumer.
 
 Errors are formatted with RFC7807 keywords and DRF exception data.
 This library was designed to be used by anyone who had enough of DRF API error messages format.
 
 ## Table of Contents
@@ -47,17 +52,17 @@
 
 ### Error structure overview
 
 API error messages typically include the following keys:
 
 - `"title"` (`str`): A brief summary that describes the problem type
 - `"detail"` (`list[str] | None`): A list of specific explanations related to the problem
-- `"invalid_params"` (`list[dict] | None`): A list of strings containing details about parameters that were invalid or malformed in the request. Each object within this list provides:
-  - `"name"` (`str`): The name of the parameter that was found to be invalid.
-  - `"reasons"` (`list[str]`): A list of strings describing the specific issues or reasons why the parameter was considered invalid or malformed.
+- `"invalid_params"` (`list[dict] | None`): A list of dict containing details about parameters that were invalid or malformed in the request. Each dict within this list provides:
+  - `"name"` (`str`): The name of the parameter that was found to be invalid
+  - `"reasons"` (`list[str]`): A list of strings describing the specific reasons why the parameter was considered invalid or malformed
 
 ```json
 {
     "title": "Error message.",
     "detail": [
         "error",
         ...
```

### Comparing `drf_simple_api_errors-1.0.0/drf_simple_api_errors/exception_handler.py` & `drf_simple_api_errors-1.0.1/drf_simple_api_errors/exception_handler.py`

 * *Files identical despite different names*

### Comparing `drf_simple_api_errors-1.0.0/drf_simple_api_errors/handlers.py` & `drf_simple_api_errors-1.0.1/drf_simple_api_errors/handlers.py`

 * *Files identical despite different names*

### Comparing `drf_simple_api_errors-1.0.0/drf_simple_api_errors/utils.py` & `drf_simple_api_errors-1.0.1/drf_simple_api_errors/utils.py`

 * *Files identical despite different names*

### Comparing `drf_simple_api_errors-1.0.0/pyproject.toml` & `drf_simple_api_errors-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-simple-api-errors"
-version = "1.0.0"
+version = "1.0.1"
 description = "A library for Django Rest Framework returning consistent and easy-to-parse API error messages."
 authors = ["Gian <30044863+gripep@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/gripep/drf-simple-api-errors"
 repository = "https://github.com/gripep/drf-simple-api-errors"
 documentation = "https://github.com/gripep/drf-simple-api-errors/blob/master/README.md"
@@ -22,25 +22,28 @@
     "Framework :: Django",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
+    'Framework :: Django',
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = ["drf_simple_api_errors", "LICENSE.md"]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 
-Django = { version = ">=2.2" }
-djangorestframework = { version = ">=3.0" }
+Django = ">=2.2"
+djangorestframework = ">=3.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `drf_simple_api_errors-1.0.0/PKG-INFO` & `drf_simple_api_errors-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-simple-api-errors
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for Django Rest Framework returning consistent and easy-to-parse API error messages.
 Home-page: https://github.com/gripep/drf-simple-api-errors
 License: MIT
 Keywords: python,django,django rest framework,drf,error handling,errors,exceptions
 Author: Gian
 Author-email: 30044863+gripep@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0
@@ -24,17 +24,22 @@
 Requires-Dist: djangorestframework (>=3.0)
 Project-URL: Documentation, https://github.com/gripep/drf-simple-api-errors/blob/master/README.md
 Project-URL: Repository, https://github.com/gripep/drf-simple-api-errors
 Description-Content-Type: text/markdown
 
 # Django Rest Framework Simple API Errors
 
+![PyPI](https://img.shields.io/pypi/v/drf-simple-api-errors)
+![test workflow](https://github.com/gripep/drf-simple-api-errors/actions/workflows/build.yaml/badge.svg)
+[![codecov](https://codecov.io/gh/gripep/drf-simple-api-errors/graph/badge.svg?token=1LJV518KMD)](https://codecov.io/gh/gripep/drf-simple-api-errors)
+![pyversions](https://img.shields.io/pypi/pyversions/drf-simple-api-errors.svg)
+
 ## What is this?
 
-A library for [Django Rest Framework](https://www.django-rest-framework.org/) returning **consistent and easy-to-parse API error messages**.
+A library for [Django Rest Framework](https://www.django-rest-framework.org/) returning **consistent, predictable and easy-to-parse API error messages**.
 
 This library was built with [RFC7807](https://tools.ietf.org/html/rfc7807) guidelines in mind, but with a small twist: it defines a "problem detail" as a `list` but it still serves as a way to include errors in a predictable and easy-to-parse format for any API consumer.
 
 Errors are formatted with RFC7807 keywords and DRF exception data.
 This library was designed to be used by anyone who had enough of DRF API error messages format.
 
 ## Table of Contents
@@ -75,17 +80,17 @@
 
 ### Error structure overview
 
 API error messages typically include the following keys:
 
 - `"title"` (`str`): A brief summary that describes the problem type
 - `"detail"` (`list[str] | None`): A list of specific explanations related to the problem
-- `"invalid_params"` (`list[dict] | None`): A list of strings containing details about parameters that were invalid or malformed in the request. Each object within this list provides:
-  - `"name"` (`str`): The name of the parameter that was found to be invalid.
-  - `"reasons"` (`list[str]`): A list of strings describing the specific issues or reasons why the parameter was considered invalid or malformed.
+- `"invalid_params"` (`list[dict] | None`): A list of dict containing details about parameters that were invalid or malformed in the request. Each dict within this list provides:
+  - `"name"` (`str`): The name of the parameter that was found to be invalid
+  - `"reasons"` (`list[str]`): A list of strings describing the specific reasons why the parameter was considered invalid or malformed
 
 ```json
 {
     "title": "Error message.",
     "detail": [
         "error",
         ...
```

