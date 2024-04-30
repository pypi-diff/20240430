# Comparing `tmp/zodchy_fastapi-0.2.2.tar.gz` & `tmp/zodchy_fastapi-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_fastapi-0.2.2.tar", max compression
+gzip compressed data, was "zodchy_fastapi-0.2.3.tar", max compression
```

## Comparing `zodchy_fastapi-0.2.2.tar` & `zodchy_fastapi-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       16 2024-04-13 13:32:10.912348 zodchy_fastapi-0.2.2/README.md
--rw-r--r--   0        0        0      467 2024-04-29 15:38:41.581713 zodchy_fastapi-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       72 2024-04-29 11:12:28.828914 zodchy_fastapi-0.2.2/zodchy_fastapi/__init__.py
--rw-r--r--   0        0        0       40 2024-04-29 15:35:10.919519 zodchy_fastapi-0.2.2/zodchy_fastapi/adapters/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-29 11:12:28.953487 zodchy_fastapi-0.2.2/zodchy_fastapi/adapters/query.py
--rw-r--r--   0        0        0      293 2024-04-29 11:12:28.838554 zodchy_fastapi-0.2.2/zodchy_fastapi/contracts/__init__.py
--rw-r--r--   0        0        0      618 2024-04-28 15:36:57.385697 zodchy_fastapi-0.2.2/zodchy_fastapi/contracts/request.py
--rw-r--r--   0        0        0     1306 2024-04-13 13:35:16.447762 zodchy_fastapi-0.2.2/zodchy_fastapi/contracts/response.py
--rw-r--r--   0        0        0      173 2024-04-29 11:12:28.960486 zodchy_fastapi-0.2.2/zodchy_fastapi/contracts/tools.py
--rw-r--r--   0        0        0     1209 2024-04-11 07:57:07.719841 zodchy_fastapi-0.2.2/zodchy_fastapi/handlers.py
--rw-r--r--   0        0        0      784 2024-04-11 07:57:07.719982 zodchy_fastapi-0.2.2/zodchy_fastapi/router.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 zodchy_fastapi-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-13 13:32:10.912348 zodchy_fastapi-0.2.3/README.md
+-rw-r--r--   0        0        0      467 2024-04-30 09:04:07.189871 zodchy_fastapi-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-04-29 11:12:28.828914 zodchy_fastapi-0.2.3/zodchy_fastapi/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-29 15:35:10.919519 zodchy_fastapi-0.2.3/zodchy_fastapi/adapters/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-29 11:12:28.953487 zodchy_fastapi-0.2.3/zodchy_fastapi/adapters/query.py
+-rw-r--r--   0        0        0      293 2024-04-29 11:12:28.838554 zodchy_fastapi-0.2.3/zodchy_fastapi/contracts/__init__.py
+-rw-r--r--   0        0        0      618 2024-04-28 15:36:57.385697 zodchy_fastapi-0.2.3/zodchy_fastapi/contracts/request.py
+-rw-r--r--   0        0        0     1306 2024-04-13 13:35:16.447762 zodchy_fastapi-0.2.3/zodchy_fastapi/contracts/response.py
+-rw-r--r--   0        0        0      173 2024-04-29 11:12:28.960486 zodchy_fastapi-0.2.3/zodchy_fastapi/contracts/tools.py
+-rw-r--r--   0        0        0     1209 2024-04-11 07:57:07.719841 zodchy_fastapi-0.2.3/zodchy_fastapi/handlers.py
+-rw-r--r--   0        0        0      784 2024-04-11 07:57:07.719982 zodchy_fastapi-0.2.3/zodchy_fastapi/router.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 zodchy_fastapi-0.2.3/PKG-INFO
```

### Comparing `zodchy_fastapi-0.2.2/zodchy_fastapi/adapters/query.py` & `zodchy_fastapi-0.2.3/zodchy_fastapi/adapters/query.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.2.2/zodchy_fastapi/contracts/request.py` & `zodchy_fastapi-0.2.3/zodchy_fastapi/contracts/request.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.2.2/zodchy_fastapi/contracts/response.py` & `zodchy_fastapi-0.2.3/zodchy_fastapi/contracts/response.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.2.2/zodchy_fastapi/handlers.py` & `zodchy_fastapi-0.2.3/zodchy_fastapi/handlers.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.2.2/zodchy_fastapi/router.py` & `zodchy_fastapi-0.2.3/zodchy_fastapi/router.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.2.2/PKG-INFO` & `zodchy_fastapi-0.2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zodchy-fastapi
-Version: 0.2.2
+Version: 0.2.3
 Summary: Collection of tools to integrate fastapi to zodchy architecture
 Home-page: https://github.com/smairon/zodchy-fastapi
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

