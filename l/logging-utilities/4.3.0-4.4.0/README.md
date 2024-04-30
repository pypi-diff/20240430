# Comparing `tmp/logging-utilities-4.3.0.tar.gz` & `tmp/logging_utilities-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logging-utilities-4.3.0.tar", last modified: Tue Mar 19 15:26:13 2024, max compression
+gzip compressed data, was "logging_utilities-4.4.0.tar", last modified: Tue Apr 30 06:34:34 2024, max compression
```

## Comparing `logging-utilities-4.3.0.tar` & `logging_utilities-4.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 15:26:13.619670 logging-utilities-4.3.0/
--rw-r--r--   0 root         (0) root         (0)     1517 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    47752 2024-03-19 15:26:13.619670 logging-utilities-4.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    46409 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 15:26:13.615670 logging-utilities-4.3.0/logging_utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/logging_utilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 15:26:13.615670 logging-utilities-4.3.0/logging_utilities/context/
--rw-r--r--   0 root         (0) root         (0)      126 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/logging_utilities/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)      649 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/logging_utilities/context/base.py
--rw-r--r--   0 root         (0) root         (0)     1828 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/logging_utilities/context/context.py
--rw-r--r--   0 root         (0) root         (0)     1620 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/logging_utilities/context/thread_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 15:26:13.615670 logging-utilities-4.3.0/logging_utilities/filters/
--rw-r--r--   0 root         (0) root         (0)     3858 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/logging_utilities/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2484 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/logging_utilities/filters/attr_type_filter.py
--rw-r--r--   0 root         (0) root         (0)     5667 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/logging_utilities/filters/django_request.py
--rw-r--r--   0 root         (0) root         (0)     2698 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/logging_utilities/filters/flask_attribute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 15:26:13.615670 logging-utilities-4.3.0/logging_utilities/formatters/
--rw-r--r--   0 root         (0) root         (0)      361 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/logging_utilities/formatters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3962 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/logging_utilities/formatters/extra_formatter.py
--rw-r--r--   0 root         (0) root         (0)    19017 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/logging_utilities/formatters/json_formatter.py
--rw-r--r--   0 root         (0) root         (0)     2017 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/logging_utilities/log_record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 15:26:13.619670 logging-utilities-4.3.0/logging_utilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)    47752 2024-03-19 15:26:13.000000 logging-utilities-4.3.0/logging_utilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2024-03-19 15:26:13.000000 logging-utilities-4.3.0/logging_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 15:26:13.000000 logging-utilities-4.3.0/logging_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-19 15:26:13.000000 logging-utilities-4.3.0/logging_utilities.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1673 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-19 15:26:13.619670 logging-utilities-4.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 15:26:13.619670 logging-utilities-4.3.0/tests/
--rw-r--r--   0 root         (0) root         (0)     6577 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/tests/test_attr_type_filter.py
--rw-r--r--   0 root         (0) root         (0)     2088 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/tests/test_const_attribute.py
--rw-r--r--   0 root         (0) root         (0)     8699 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/tests/test_django_attribute.py
--rw-r--r--   0 root         (0) root         (0)    11513 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/tests/test_extra_formatter.py
--rw-r--r--   0 root         (0) root         (0)    12243 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/tests/test_flask_attribute.py
--rw-r--r--   0 root         (0) root         (0)     6171 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/tests/test_flask_json_formatter.py
--rw-r--r--   0 root         (0) root         (0)    31498 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/tests/test_json_formatter.py
--rw-r--r--   0 root         (0) root         (0)     5006 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/tests/test_log_record_missing.py
--rw-r--r--   0 root         (0) root         (0)    10110 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/tests/test_logging_context.py
--rw-r--r--   0 root         (0) root         (0)     1267 2024-03-19 15:25:10.000000 logging-utilities-4.3.0/tests/test_regex.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:34:34.075782 logging_utilities-4.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1517 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    47752 2024-04-30 06:34:34.075782 logging_utilities-4.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    46409 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:34:34.075782 logging_utilities-4.4.0/logging_utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/logging_utilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:34:34.075782 logging_utilities-4.4.0/logging_utilities/context/
+-rw-r--r--   0 root         (0) root         (0)      126 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/logging_utilities/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      649 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/logging_utilities/context/base.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/logging_utilities/context/context.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/logging_utilities/context/thread_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:34:34.075782 logging_utilities-4.4.0/logging_utilities/filters/
+-rw-r--r--   0 root         (0) root         (0)     3858 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/logging_utilities/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/logging_utilities/filters/attr_type_filter.py
+-rw-r--r--   0 root         (0) root         (0)     5667 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/logging_utilities/filters/django_request.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/logging_utilities/filters/flask_attribute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:34:34.075782 logging_utilities-4.4.0/logging_utilities/formatters/
+-rw-r--r--   0 root         (0) root         (0)      361 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/logging_utilities/formatters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3962 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/logging_utilities/formatters/extra_formatter.py
+-rw-r--r--   0 root         (0) root         (0)    19017 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/logging_utilities/formatters/json_formatter.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/logging_utilities/log_record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:34:34.075782 logging_utilities-4.4.0/logging_utilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    47752 2024-04-30 06:34:34.000000 logging_utilities-4.4.0/logging_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-04-30 06:34:34.000000 logging_utilities-4.4.0/logging_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 06:34:34.000000 logging_utilities-4.4.0/logging_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-30 06:34:34.000000 logging_utilities-4.4.0/logging_utilities.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 06:34:34.075782 logging_utilities-4.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:34:34.075782 logging_utilities-4.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     6577 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/tests/test_attr_type_filter.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/tests/test_const_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     8699 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/tests/test_django_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    11513 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/tests/test_extra_formatter.py
+-rw-r--r--   0 root         (0) root         (0)    12243 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/tests/test_flask_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     6171 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/tests/test_flask_json_formatter.py
+-rw-r--r--   0 root         (0) root         (0)    31498 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/tests/test_json_formatter.py
+-rw-r--r--   0 root         (0) root         (0)     5006 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/tests/test_log_record_missing.py
+-rw-r--r--   0 root         (0) root         (0)    10110 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/tests/test_logging_context.py
+-rw-r--r--   0 root         (0) root         (0)     1267 2024-04-30 06:32:35.000000 logging_utilities-4.4.0/tests/test_regex.py
```

### Comparing `logging-utilities-4.3.0/LICENSE` & `logging_utilities-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/PKG-INFO` & `logging_utilities-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logging-utilities
-Version: 4.3.0
+Version: 4.4.0
 Summary: A collection of useful logging formatters and filters.Logging Context, JSON Formatter, Extra Formatter, ISO Time Filter, Flask Filter, Django Filter, ...
 Author-email: Brice Schaffner <brice.schaffner@swisstopo.ch>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/geoadmin/lib-py-logging-utilities
 Project-URL: Documentation, https://github.com/geoadmin/lib-py-logging-utilities#readme
 Project-URL: Source, https://github.com/geoadmin/lib-py-logging-utilities
 Project-URL: Tracker, https://github.com/geoadmin/lib-py-logging-utilities/issues
```

### Comparing `logging-utilities-4.3.0/README.md` & `logging_utilities-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/logging_utilities/context/base.py` & `logging_utilities-4.4.0/logging_utilities/context/base.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/logging_utilities/context/context.py` & `logging_utilities-4.4.0/logging_utilities/context/context.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/logging_utilities/context/thread_context.py` & `logging_utilities-4.4.0/logging_utilities/context/thread_context.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/logging_utilities/filters/__init__.py` & `logging_utilities-4.4.0/logging_utilities/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/logging_utilities/filters/attr_type_filter.py` & `logging_utilities-4.4.0/logging_utilities/filters/attr_type_filter.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/logging_utilities/filters/django_request.py` & `logging_utilities-4.4.0/logging_utilities/filters/django_request.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/logging_utilities/filters/flask_attribute.py` & `logging_utilities-4.4.0/logging_utilities/filters/flask_attribute.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/logging_utilities/formatters/extra_formatter.py` & `logging_utilities-4.4.0/logging_utilities/formatters/extra_formatter.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/logging_utilities/formatters/json_formatter.py` & `logging_utilities-4.4.0/logging_utilities/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/logging_utilities/log_record.py` & `logging_utilities-4.4.0/logging_utilities/log_record.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/logging_utilities.egg-info/PKG-INFO` & `logging_utilities-4.4.0/logging_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logging-utilities
-Version: 4.3.0
+Version: 4.4.0
 Summary: A collection of useful logging formatters and filters.Logging Context, JSON Formatter, Extra Formatter, ISO Time Filter, Flask Filter, Django Filter, ...
 Author-email: Brice Schaffner <brice.schaffner@swisstopo.ch>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/geoadmin/lib-py-logging-utilities
 Project-URL: Documentation, https://github.com/geoadmin/lib-py-logging-utilities#readme
 Project-URL: Source, https://github.com/geoadmin/lib-py-logging-utilities
 Project-URL: Tracker, https://github.com/geoadmin/lib-py-logging-utilities/issues
```

### Comparing `logging-utilities-4.3.0/logging_utilities.egg-info/SOURCES.txt` & `logging_utilities-4.4.0/logging_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/pyproject.toml` & `logging_utilities-4.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/tests/test_attr_type_filter.py` & `logging_utilities-4.4.0/tests/test_attr_type_filter.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/tests/test_const_attribute.py` & `logging_utilities-4.4.0/tests/test_const_attribute.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/tests/test_django_attribute.py` & `logging_utilities-4.4.0/tests/test_django_attribute.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/tests/test_extra_formatter.py` & `logging_utilities-4.4.0/tests/test_extra_formatter.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/tests/test_flask_attribute.py` & `logging_utilities-4.4.0/tests/test_flask_attribute.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/tests/test_flask_json_formatter.py` & `logging_utilities-4.4.0/tests/test_flask_json_formatter.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/tests/test_json_formatter.py` & `logging_utilities-4.4.0/tests/test_json_formatter.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/tests/test_log_record_missing.py` & `logging_utilities-4.4.0/tests/test_log_record_missing.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/tests/test_logging_context.py` & `logging_utilities-4.4.0/tests/test_logging_context.py`

 * *Files identical despite different names*

### Comparing `logging-utilities-4.3.0/tests/test_regex.py` & `logging_utilities-4.4.0/tests/test_regex.py`

 * *Files identical despite different names*

