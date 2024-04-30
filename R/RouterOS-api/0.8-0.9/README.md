# Comparing `tmp/RouterOS-api-0.8.tar.gz` & `tmp/RouterOS-api-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/RouterOS-api-0.8.tar", last modified: Mon Oct 27 09:37:52 2014, max compression
+gzip compressed data, was "dist/RouterOS-api-0.9.tar", last modified: Tue Nov  4 08:50:51 2014, max compression
```

## Comparing `RouterOS-api-0.8.tar` & `RouterOS-api-0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 hagaren   (1015) developers  (1100)        0 2014-10-27 09:37:52.000000 RouterOS-api-0.8/
--rw-r--r--   0 hagaren   (1015) developers  (1100)      248 2014-10-27 09:37:52.000000 RouterOS-api-0.8/PKG-INFO
-drwxr-xr-x   0 hagaren   (1015) developers  (1100)        0 2014-10-27 09:37:52.000000 RouterOS-api-0.8/tests/
--rw-r--r--   0 hagaren   (1015) developers  (1100)     2942 2014-09-01 10:10:40.000000 RouterOS-api-0.8/tests/test_resource.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)     1341 2014-07-31 15:26:13.000000 RouterOS-api-0.8/tests/test_socket.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)     2037 2014-07-03 07:40:02.000000 RouterOS-api-0.8/tests/test_sentence.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)        0 2014-06-13 12:24:20.000000 RouterOS-api-0.8/tests/__init__.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)     3664 2014-07-11 08:51:46.000000 RouterOS-api-0.8/tests/test_base_api.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)     3395 2014-08-21 12:42:39.000000 RouterOS-api-0.8/tests/test_api_communicator.py
-drwxr-xr-x   0 hagaren   (1015) developers  (1100)        0 2014-10-27 09:37:52.000000 RouterOS-api-0.8/routeros_api/
--rw-r--r--   0 hagaren   (1015) developers  (1100)     2460 2014-09-22 09:05:39.000000 RouterOS-api-0.8/routeros_api/base_api.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)      595 2014-10-13 13:51:14.000000 RouterOS-api-0.8/routeros_api/exceptions.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)     2521 2014-06-28 13:46:46.000000 RouterOS-api-0.8/routeros_api/sentence.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)     3229 2014-09-01 10:08:41.000000 RouterOS-api-0.8/routeros_api/resource.py
-drwxr-xr-x   0 hagaren   (1015) developers  (1100)        0 2014-10-27 09:37:52.000000 RouterOS-api-0.8/routeros_api/api_communicator/
--rw-r--r--   0 hagaren   (1015) developers  (1100)     3811 2014-10-13 13:51:14.000000 RouterOS-api-0.8/routeros_api/api_communicator/base.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)     1265 2014-08-21 13:05:18.000000 RouterOS-api-0.8/routeros_api/api_communicator/encoding_decorator.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)      887 2014-10-13 13:51:14.000000 RouterOS-api-0.8/routeros_api/api_communicator/exception_decorator.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)     1134 2014-08-21 13:05:02.000000 RouterOS-api-0.8/routeros_api/api_communicator/key_cleaner_decorator.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)      526 2014-07-04 13:00:59.000000 RouterOS-api-0.8/routeros_api/api_communicator/async_decorator.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)     1031 2014-08-21 12:21:40.000000 RouterOS-api-0.8/routeros_api/api_communicator/__init__.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)      720 2014-10-23 13:34:06.000000 RouterOS-api-0.8/routeros_api/communication_exception_parsers.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)      647 2014-08-21 13:41:21.000000 RouterOS-api-0.8/routeros_api/api_structure.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)      120 2014-06-28 08:17:57.000000 RouterOS-api-0.8/routeros_api/utils.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)     1264 2014-06-28 08:18:35.000000 RouterOS-api-0.8/routeros_api/query.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)      220 2014-10-02 09:41:57.000000 RouterOS-api-0.8/routeros_api/__init__.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)     2931 2014-10-13 14:47:31.000000 RouterOS-api-0.8/routeros_api/api.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)     2049 2014-09-30 13:36:26.000000 RouterOS-api-0.8/routeros_api/api_socket.py
--rw-r--r--   0 hagaren   (1015) developers  (1100)       59 2014-10-27 09:37:52.000000 RouterOS-api-0.8/setup.cfg
--rw-r--r--   0 hagaren   (1015) developers  (1100)      483 2014-10-13 12:38:44.000000 RouterOS-api-0.8/setup.py
-drwxr-xr-x   0 hagaren   (1015) developers  (1100)        0 2014-10-27 09:37:52.000000 RouterOS-api-0.8/RouterOS_api.egg-info/
--rw-r--r--   0 hagaren   (1015) developers  (1100)      248 2014-10-27 09:37:50.000000 RouterOS-api-0.8/RouterOS_api.egg-info/PKG-INFO
--rw-r--r--   0 hagaren   (1015) developers  (1100)       19 2014-10-27 09:37:50.000000 RouterOS-api-0.8/RouterOS_api.egg-info/top_level.txt
--rw-r--r--   0 hagaren   (1015) developers  (1100)      876 2014-10-27 09:37:52.000000 RouterOS-api-0.8/RouterOS_api.egg-info/SOURCES.txt
--rw-r--r--   0 hagaren   (1015) developers  (1100)        1 2014-10-27 09:37:50.000000 RouterOS-api-0.8/RouterOS_api.egg-info/dependency_links.txt
+drwxr-xr-x   0 hagaren   (1015) developers  (1100)        0 2014-11-04 08:50:51.000000 RouterOS-api-0.9/
+-rw-r--r--   0 hagaren   (1015) developers  (1100)      248 2014-11-04 08:50:51.000000 RouterOS-api-0.9/PKG-INFO
+drwxr-xr-x   0 hagaren   (1015) developers  (1100)        0 2014-11-04 08:50:51.000000 RouterOS-api-0.9/tests/
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     2942 2014-09-01 10:10:40.000000 RouterOS-api-0.9/tests/test_resource.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     1341 2014-07-31 15:26:13.000000 RouterOS-api-0.9/tests/test_socket.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     2037 2014-07-03 07:40:02.000000 RouterOS-api-0.9/tests/test_sentence.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)        0 2014-06-13 12:24:20.000000 RouterOS-api-0.9/tests/__init__.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     3664 2014-07-11 08:51:46.000000 RouterOS-api-0.9/tests/test_base_api.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     3395 2014-08-21 12:42:39.000000 RouterOS-api-0.9/tests/test_api_communicator.py
+drwxr-xr-x   0 hagaren   (1015) developers  (1100)        0 2014-11-04 08:50:51.000000 RouterOS-api-0.9/routeros_api/
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     2460 2014-09-22 09:05:39.000000 RouterOS-api-0.9/routeros_api/base_api.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)      595 2014-10-13 13:51:14.000000 RouterOS-api-0.9/routeros_api/exceptions.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     2521 2014-06-28 13:46:46.000000 RouterOS-api-0.9/routeros_api/sentence.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     3229 2014-09-01 10:08:41.000000 RouterOS-api-0.9/routeros_api/resource.py
+drwxr-xr-x   0 hagaren   (1015) developers  (1100)        0 2014-11-04 08:50:51.000000 RouterOS-api-0.9/routeros_api/api_communicator/
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     3811 2014-10-13 13:51:14.000000 RouterOS-api-0.9/routeros_api/api_communicator/base.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     1265 2014-08-21 13:05:18.000000 RouterOS-api-0.9/routeros_api/api_communicator/encoding_decorator.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)      887 2014-10-13 13:51:14.000000 RouterOS-api-0.9/routeros_api/api_communicator/exception_decorator.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     1134 2014-08-21 13:05:02.000000 RouterOS-api-0.9/routeros_api/api_communicator/key_cleaner_decorator.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)      526 2014-07-04 13:00:59.000000 RouterOS-api-0.9/routeros_api/api_communicator/async_decorator.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     1031 2014-08-21 12:21:40.000000 RouterOS-api-0.9/routeros_api/api_communicator/__init__.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)      720 2014-10-23 13:34:06.000000 RouterOS-api-0.9/routeros_api/communication_exception_parsers.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)      647 2014-08-21 13:41:21.000000 RouterOS-api-0.9/routeros_api/api_structure.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)      120 2014-06-28 08:17:57.000000 RouterOS-api-0.9/routeros_api/utils.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     1264 2014-06-28 08:18:35.000000 RouterOS-api-0.9/routeros_api/query.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)      220 2014-10-02 09:41:57.000000 RouterOS-api-0.9/routeros_api/__init__.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     2928 2014-11-03 14:49:04.000000 RouterOS-api-0.9/routeros_api/api.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)     2049 2014-09-30 13:36:26.000000 RouterOS-api-0.9/routeros_api/api_socket.py
+-rw-r--r--   0 hagaren   (1015) developers  (1100)       59 2014-11-04 08:50:51.000000 RouterOS-api-0.9/setup.cfg
+-rw-r--r--   0 hagaren   (1015) developers  (1100)      483 2014-11-03 14:49:04.000000 RouterOS-api-0.9/setup.py
+drwxr-xr-x   0 hagaren   (1015) developers  (1100)        0 2014-11-04 08:50:51.000000 RouterOS-api-0.9/RouterOS_api.egg-info/
+-rw-r--r--   0 hagaren   (1015) developers  (1100)      248 2014-11-04 08:50:50.000000 RouterOS-api-0.9/RouterOS_api.egg-info/PKG-INFO
+-rw-r--r--   0 hagaren   (1015) developers  (1100)       19 2014-11-04 08:50:50.000000 RouterOS-api-0.9/RouterOS_api.egg-info/top_level.txt
+-rw-r--r--   0 hagaren   (1015) developers  (1100)      876 2014-11-04 08:50:51.000000 RouterOS-api-0.9/RouterOS_api.egg-info/SOURCES.txt
+-rw-r--r--   0 hagaren   (1015) developers  (1100)        1 2014-11-04 08:50:50.000000 RouterOS-api-0.9/RouterOS_api.egg-info/dependency_links.txt
```

### Comparing `RouterOS-api-0.8/tests/test_resource.py` & `RouterOS-api-0.9/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/tests/test_socket.py` & `RouterOS-api-0.9/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/tests/test_sentence.py` & `RouterOS-api-0.9/tests/test_sentence.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/tests/test_base_api.py` & `RouterOS-api-0.9/tests/test_base_api.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/tests/test_api_communicator.py` & `RouterOS-api-0.9/tests/test_api_communicator.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/base_api.py` & `RouterOS-api-0.9/routeros_api/base_api.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/exceptions.py` & `RouterOS-api-0.9/routeros_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/sentence.py` & `RouterOS-api-0.9/routeros_api/sentence.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/resource.py` & `RouterOS-api-0.9/routeros_api/resource.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/api_communicator/base.py` & `RouterOS-api-0.9/routeros_api/api_communicator/base.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/api_communicator/encoding_decorator.py` & `RouterOS-api-0.9/routeros_api/api_communicator/encoding_decorator.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/api_communicator/exception_decorator.py` & `RouterOS-api-0.9/routeros_api/api_communicator/exception_decorator.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/api_communicator/key_cleaner_decorator.py` & `RouterOS-api-0.9/routeros_api/api_communicator/key_cleaner_decorator.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/api_communicator/async_decorator.py` & `RouterOS-api-0.9/routeros_api/api_communicator/async_decorator.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/api_communicator/__init__.py` & `RouterOS-api-0.9/routeros_api/api_communicator/__init__.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/communication_exception_parsers.py` & `RouterOS-api-0.9/routeros_api/communication_exception_parsers.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/api_structure.py` & `RouterOS-api-0.9/routeros_api/api_structure.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/query.py` & `RouterOS-api-0.9/routeros_api/query.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/routeros_api/api.py` & `RouterOS-api-0.9/routeros_api/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,11 +71,11 @@
 
 class CloseConnectionExceptionHandler:
     def __init__(self, pool):
         self.pool = pool
 
     def handle(self, exception):
         connection_closed = isinstance(
-            exception, exceptions.RouterOsApiCommunicationError)
+            exception, exceptions.RouterOsApiConnectionError)
         fatal_error = isinstance(exception, exceptions.FatalRouterOsApiError)
         if connection_closed or fatal_error:
             self.pool.disconnect()
```

### Comparing `RouterOS-api-0.8/routeros_api/api_socket.py` & `RouterOS-api-0.9/routeros_api/api_socket.py`

 * *Files identical despite different names*

### Comparing `RouterOS-api-0.8/RouterOS_api.egg-info/SOURCES.txt` & `RouterOS-api-0.9/RouterOS_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

