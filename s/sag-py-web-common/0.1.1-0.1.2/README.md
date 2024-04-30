# Comparing `tmp/sag-py-web-common-0.1.1.tar.gz` & `tmp/sag-py-web-common-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-web-common-0.1.1.tar", last modified: Tue Jul  4 09:11:11 2023, max compression
+gzip compressed data, was "sag-py-web-common-0.1.2.tar", last modified: Tue Jul  4 13:43:10 2023, max compression
```

## Comparing `sag-py-web-common-0.1.1.tar` & `sag-py-web-common-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:11:11.150767 sag-py-web-common-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-04 09:11:11.150767 sag-py-web-common-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:11:11.150767 sag-py-web-common-0.1.1/sag_py_web_common/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/sag_py_web_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/sag_py_web_common/default_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/sag_py_web_common/filtered_access_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/sag_py_web_common/json_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/sag_py_web_common/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/sag_py_web_common/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:11:11.150767 sag-py-web-common-0.1.1/sag_py_web_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-04 09:11:11.000000 sag-py-web-common-0.1.1/sag_py_web_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 09:11:11.000000 sag-py-web-common-0.1.1/sag_py_web_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:11:11.000000 sag-py-web-common-0.1.1/sag_py_web_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-04 09:11:11.000000 sag-py-web-common-0.1.1/sag_py_web_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 09:11:11.000000 sag-py-web-common-0.1.1/sag_py_web_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-04 09:11:11.150767 sag-py-web-common-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:11:11.150767 sag-py-web-common-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/tests/test_build_default_route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:43:10.960298 sag-py-web-common-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-04 13:42:58.000000 sag-py-web-common-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-04 13:43:10.960298 sag-py-web-common-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-04 13:42:58.000000 sag-py-web-common-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-04 13:42:58.000000 sag-py-web-common-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:43:10.960298 sag-py-web-common-0.1.2/sag_py_web_common/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-04 13:42:58.000000 sag-py-web-common-0.1.2/sag_py_web_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-04 13:42:58.000000 sag-py-web-common-0.1.2/sag_py_web_common/default_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-04 13:42:58.000000 sag-py-web-common-0.1.2/sag_py_web_common/filtered_access_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-04 13:42:58.000000 sag-py-web-common-0.1.2/sag_py_web_common/json_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:42:58.000000 sag-py-web-common-0.1.2/sag_py_web_common/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-04 13:42:58.000000 sag-py-web-common-0.1.2/sag_py_web_common/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:43:10.960298 sag-py-web-common-0.1.2/sag_py_web_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-04 13:43:10.000000 sag-py-web-common-0.1.2/sag_py_web_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 13:43:10.000000 sag-py-web-common-0.1.2/sag_py_web_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:43:10.000000 sag-py-web-common-0.1.2/sag_py_web_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-04 13:43:10.000000 sag-py-web-common-0.1.2/sag_py_web_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 13:43:10.000000 sag-py-web-common-0.1.2/sag_py_web_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-04 13:43:10.960298 sag-py-web-common-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-04 13:42:58.000000 sag-py-web-common-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:43:10.960298 sag-py-web-common-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 13:42:58.000000 sag-py-web-common-0.1.2/tests/test_build_default_route.py
```

### Comparing `sag-py-web-common-0.1.1/LICENSE.txt` & `sag-py-web-common-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-web-common-0.1.1/PKG-INFO` & `sag-py-web-common-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-web-common
-Version: 0.1.1
+Version: 0.1.2
 Summary: Small helper functions for web projects
 Home-page: https://github.com/SamhammerAG/sag_py_web_common
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_web_common
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_web_common/issues
```

### Comparing `sag-py-web-common-0.1.1/README.md` & `sag-py-web-common-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sag-py-web-common-0.1.1/sag_py_web_common/default_route.py` & `sag-py-web-common-0.1.2/sag_py_web_common/default_route.py`

 * *Files identical despite different names*

### Comparing `sag-py-web-common-0.1.1/sag_py_web_common/filtered_access_logger.py` & `sag-py-web-common-0.1.2/sag_py_web_common/filtered_access_logger.py`

 * *Files identical despite different names*

### Comparing `sag-py-web-common-0.1.1/sag_py_web_common/json_exception_handler.py` & `sag-py-web-common-0.1.2/sag_py_web_common/json_exception_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,10 +18,10 @@
         JSONResponse: A json response that contains the field 'detail' with the exception message.
     """
     logger.error("An unknown Error!", exc_info=True, extra={"response_status": 500})
     return JSONResponse(status_code=500, content=jsonable_encoder({"detail": str(exception)}))
 
 
 async def log_exception(_, exception: StarletteHTTPException) -> Response:  # type: ignore
-    logger.error("An HTTP Error! %s", exception.detail, exc_info=True, extra={"response_status": exception.status_code})
+    logger.error("An HTTP Error! %s", exception.detail, extra={"response_status": exception.status_code})
 
     return await http_exception_handler(_, exception)
```

### Comparing `sag-py-web-common-0.1.1/sag_py_web_common.egg-info/PKG-INFO` & `sag-py-web-common-0.1.2/sag_py_web_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-web-common
-Version: 0.1.1
+Version: 0.1.2
 Summary: Small helper functions for web projects
 Home-page: https://github.com/SamhammerAG/sag_py_web_common
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_web_common
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_web_common/issues
```

### Comparing `sag-py-web-common-0.1.1/setup.py` & `sag-py-web-common-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="sag-py-web-common",
-    version="0.1.1",
+    version="0.1.2",
     description="Small helper functions for web projects",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_web_common",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

