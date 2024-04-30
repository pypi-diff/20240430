# Comparing `tmp/gc_google_services_api-1.4.0.tar.gz` & `tmp/gc_google_services_api-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gc_google_services_api-1.4.0.tar", max compression
+gzip compressed data, was "gc_google_services_api-1.5.0.tar", max compression
```

## Comparing `gc_google_services_api-1.4.0.tar` & `gc_google_services_api-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0    35149 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/LICENSE
--rw-r--r--   0        0        0     4789 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/README.md
--rw-r--r--   0        0        0        0 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/gc_google_services_api/__init__.py
--rw-r--r--   0        0        0      796 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/gc_google_services_api/auth/__init__.py
--rw-r--r--   0        0        0        0 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/gc_google_services_api/auth/__tests__/__init__.py
--rw-r--r--   0        0        0     2192 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/gc_google_services_api/auth/__tests__/test_auth.py
--rw-r--r--   0        0        0     3699 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/gc_google_services_api/bigquery/__init__.py
--rw-r--r--   0        0        0        0 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/gc_google_services_api/bigquery/__tests__/__init__.py
--rw-r--r--   0        0        0      988 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/gc_google_services_api/bigquery/__tests__/test_bigquery.py
--rw-r--r--   0        0        0     4192 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/gc_google_services_api/calendar_api/__init__.py
--rw-r--r--   0        0        0        0 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/gc_google_services_api/calendar_api/__tests__/__init__.py
--rw-r--r--   0        0        0     7927 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/gc_google_services_api/calendar_api/__tests__/test_calendar.py
--rw-r--r--   0        0        0     1711 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/gc_google_services_api/gmail/__init__.py
--rw-r--r--   0        0        0        0 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/gc_google_services_api/gmail/__tests__/__init__.py
--rw-r--r--   0        0        0     2827 2024-01-22 11:46:10.432105 gc_google_services_api-1.4.0/gc_google_services_api/gmail/__tests__/test_gmail.py
--rw-r--r--   0        0        0     2085 2024-01-22 11:46:10.436105 gc_google_services_api-1.4.0/gc_google_services_api/gsheet/__init__.py
--rw-r--r--   0        0        0        0 2024-01-22 11:46:10.436105 gc_google_services_api-1.4.0/gc_google_services_api/gsheet/__tests__/__init__.py
--rw-r--r--   0        0        0     3635 2024-01-22 11:46:10.436105 gc_google_services_api-1.4.0/gc_google_services_api/gsheet/__tests__/test_gsheet.py
--rw-r--r--   0        0        0        0 2024-01-22 11:46:10.436105 gc_google_services_api-1.4.0/gc_google_services_api/permissions/__init__.py
--rw-r--r--   0        0        0     3281 2024-01-22 11:46:10.436105 gc_google_services_api-1.4.0/gc_google_services_api/permissions/drive.py
--rw-r--r--   0        0        0     3506 2024-01-22 11:46:10.436105 gc_google_services_api-1.4.0/gc_google_services_api/permissions/workspace.py
--rw-r--r--   0        0        0      656 2024-01-22 11:46:10.436105 gc_google_services_api-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     5498 1970-01-01 00:00:00.000000 gc_google_services_api-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/LICENSE
+-rw-r--r--   0        0        0     4789 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/__init__.py
+-rw-r--r--   0        0        0      796 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/auth/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/auth/__tests__/__init__.py
+-rw-r--r--   0        0        0     2192 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/auth/__tests__/test_auth.py
+-rw-r--r--   0        0        0     3699 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/bigquery/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/bigquery/__tests__/__init__.py
+-rw-r--r--   0        0        0      988 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/bigquery/__tests__/test_bigquery.py
+-rw-r--r--   0        0        0     4192 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/calendar_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/calendar_api/__tests__/__init__.py
+-rw-r--r--   0        0        0     7927 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/calendar_api/__tests__/test_calendar.py
+-rw-r--r--   0        0        0     1711 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/gmail/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/gmail/__tests__/__init__.py
+-rw-r--r--   0        0        0     2827 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/gmail/__tests__/test_gmail.py
+-rw-r--r--   0        0        0     2085 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/gsheet/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:47:49.392791 gc_google_services_api-1.5.0/gc_google_services_api/gsheet/__tests__/__init__.py
+-rw-r--r--   0        0        0     3635 2024-04-30 17:47:49.396791 gc_google_services_api-1.5.0/gc_google_services_api/gsheet/__tests__/test_gsheet.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:47:49.396791 gc_google_services_api-1.5.0/gc_google_services_api/permissions/__init__.py
+-rw-r--r--   0        0        0     3281 2024-04-30 17:47:49.396791 gc_google_services_api-1.5.0/gc_google_services_api/permissions/drive.py
+-rw-r--r--   0        0        0     3506 2024-04-30 17:47:49.396791 gc_google_services_api-1.5.0/gc_google_services_api/permissions/workspace.py
+-rw-r--r--   0        0        0     3339 2024-04-30 17:47:49.396791 gc_google_services_api-1.5.0/gc_google_services_api/pubsub/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:47:49.396791 gc_google_services_api-1.5.0/gc_google_services_api/pubsub/__tests__/__init__.py
+-rw-r--r--   0        0        0     5553 2024-04-30 17:47:49.396791 gc_google_services_api-1.5.0/gc_google_services_api/pubsub/__tests__/test_pubsub.py
+-rw-r--r--   0        0        0      688 2024-04-30 17:47:49.396791 gc_google_services_api-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5551 1970-01-01 00:00:00.000000 gc_google_services_api-1.5.0/PKG-INFO
```

### Comparing `gc_google_services_api-1.4.0/LICENSE` & `gc_google_services_api-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/README.md` & `gc_google_services_api-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/gc_google_services_api/auth/__init__.py` & `gc_google_services_api-1.5.0/gc_google_services_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/gc_google_services_api/auth/__tests__/test_auth.py` & `gc_google_services_api-1.5.0/gc_google_services_api/auth/__tests__/test_auth.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/gc_google_services_api/bigquery/__init__.py` & `gc_google_services_api-1.5.0/gc_google_services_api/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/gc_google_services_api/bigquery/__tests__/test_bigquery.py` & `gc_google_services_api-1.5.0/gc_google_services_api/bigquery/__tests__/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/gc_google_services_api/calendar_api/__init__.py` & `gc_google_services_api-1.5.0/gc_google_services_api/calendar_api/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/gc_google_services_api/calendar_api/__tests__/test_calendar.py` & `gc_google_services_api-1.5.0/gc_google_services_api/calendar_api/__tests__/test_calendar.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/gc_google_services_api/gmail/__init__.py` & `gc_google_services_api-1.5.0/gc_google_services_api/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/gc_google_services_api/gmail/__tests__/test_gmail.py` & `gc_google_services_api-1.5.0/gc_google_services_api/gmail/__tests__/test_gmail.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/gc_google_services_api/gsheet/__init__.py` & `gc_google_services_api-1.5.0/gc_google_services_api/gsheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/gc_google_services_api/gsheet/__tests__/test_gsheet.py` & `gc_google_services_api-1.5.0/gc_google_services_api/gsheet/__tests__/test_gsheet.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/gc_google_services_api/permissions/drive.py` & `gc_google_services_api-1.5.0/gc_google_services_api/permissions/drive.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/gc_google_services_api/permissions/workspace.py` & `gc_google_services_api-1.5.0/gc_google_services_api/permissions/workspace.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.4.0/pyproject.toml` & `gc_google_services_api-1.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "gc-google-services-api"
-version = "1.4.0"
+version = "1.5.0"
 description = ""
 authors = ["Jonathan Rodríguez Alejos <jrodriguez.5716@gmail.com>"]
 readme = "README.md"
 packages = [{include = "gc_google_services_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 flake8 = "^6.0.0"
 google-api-python-client = "^2.80.0"
 google-cloud-bigquery = "^3.6.0"
 isort = "^5.12.0"
 pre-commit = "^3.3.2"
+google-cloud-pubsub = "^2.21.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.source]]
 name = "syscorp-librarian"
```

### Comparing `gc_google_services_api-1.4.0/PKG-INFO` & `gc_google_services_api-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: gc-google-services-api
-Version: 1.4.0
+Version: 1.5.0
 Summary: 
 Author: Jonathan Rodríguez Alejos
 Author-email: jrodriguez.5716@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: google-api-python-client (>=2.80.0,<3.0.0)
 Requires-Dist: google-cloud-bigquery (>=3.6.0,<4.0.0)
+Requires-Dist: google-cloud-pubsub (>=2.21.1,<3.0.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: pre-commit (>=3.3.2,<4.0.0)
 Description-Content-Type: text/markdown
 
 [![Publish to PyPI.org](https://github.com/GoodCod3/gc-google-services-api/actions/workflows/pr.yml/badge.svg)](https://github.com/GoodCod3/gc-google-services-api/actions/workflows/pr.yml)
 
 # How to contribute
```

