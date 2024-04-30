# Comparing `tmp/request_response_logging-0.0.9.tar.gz` & `tmp/request_response_logging-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "request_response_logging-0.0.9.tar", last modified: Wed Feb  7 12:36:34 2024, max compression
+gzip compressed data, was "request_response_logging-1.0.0.tar", last modified: Tue Apr 30 07:10:43 2024, max compression
```

## Comparing `request_response_logging-0.0.9.tar` & `request_response_logging-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-02-07 12:36:34.683732 request_response_logging-0.0.9/
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     5941 2024-02-07 12:36:34.683732 request_response_logging-0.0.9/PKG-INFO
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     4558 2024-02-07 12:35:50.000000 request_response_logging-0.0.9/README.md
-drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-02-07 12:36:34.683732 request_response_logging-0.0.9/request_logging/
-drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-02-07 12:36:34.683732 request_response_logging-0.0.9/request_logging/Filters/
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     1638 2024-01-21 16:59:31.000000 request_response_logging-0.0.9/request_logging/Filters/LoggingFilters.py
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       59 2024-01-21 03:11:04.000000 request_response_logging-0.0.9/request_logging/Filters/__init__.py
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      107 2024-01-21 11:20:31.000000 request_response_logging-0.0.9/request_logging/__init__.py
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      522 2024-01-21 11:26:55.000000 request_response_logging-0.0.9/request_logging/decorators.py
-drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-02-07 12:36:34.683732 request_response_logging-0.0.9/request_logging/middleware/
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     6057 2024-02-07 12:17:32.000000 request_response_logging-0.0.9/request_logging/middleware/RequestResponseLogging.py
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       53 2024-01-21 03:14:15.000000 request_response_logging-0.0.9/request_logging/middleware/__init__.py
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      247 2024-02-02 17:51:13.000000 request_response_logging-0.0.9/request_logging/utils.py
-drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-02-07 12:36:34.683732 request_response_logging-0.0.9/request_response_logging.egg-info/
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     5941 2024-02-07 12:36:34.000000 request_response_logging-0.0.9/request_response_logging.egg-info/PKG-INFO
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      510 2024-02-07 12:36:34.000000 request_response_logging-0.0.9/request_response_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)        1 2024-02-07 12:36:34.000000 request_response_logging-0.0.9/request_response_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       11 2024-02-07 12:36:34.000000 request_response_logging-0.0.9/request_response_logging.egg-info/requires.txt
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       16 2024-02-07 12:36:34.000000 request_response_logging-0.0.9/request_response_logging.egg-info/top_level.txt
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       38 2024-02-07 12:36:34.683732 request_response_logging-0.0.9/setup.cfg
--rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      590 2024-02-07 12:20:36.000000 request_response_logging-0.0.9/setup.py
+drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-04-30 07:10:43.499419 request_response_logging-1.0.0/
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     5941 2024-04-30 07:10:43.499419 request_response_logging-1.0.0/PKG-INFO
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     4558 2024-02-07 12:35:50.000000 request_response_logging-1.0.0/README.md
+drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-04-30 07:10:43.487419 request_response_logging-1.0.0/request_logging/
+drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-04-30 07:10:43.491419 request_response_logging-1.0.0/request_logging/Filters/
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     1638 2024-01-21 16:59:31.000000 request_response_logging-1.0.0/request_logging/Filters/LoggingFilters.py
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       59 2024-01-21 03:11:04.000000 request_response_logging-1.0.0/request_logging/Filters/__init__.py
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      107 2024-01-21 11:20:31.000000 request_response_logging-1.0.0/request_logging/__init__.py
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      522 2024-01-21 11:26:55.000000 request_response_logging-1.0.0/request_logging/decorators.py
+drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-04-30 07:10:43.495419 request_response_logging-1.0.0/request_logging/middleware/
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     6131 2024-04-30 07:05:46.000000 request_response_logging-1.0.0/request_logging/middleware/RequestResponseLogging.py
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       53 2024-01-21 03:14:15.000000 request_response_logging-1.0.0/request_logging/middleware/__init__.py
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      247 2024-02-02 17:51:13.000000 request_response_logging-1.0.0/request_logging/utils.py
+drwxrwxr-x   0 praveentiwari  (1001) praveentiwari  (1001)        0 2024-04-30 07:10:43.499419 request_response_logging-1.0.0/request_response_logging.egg-info/
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)     5941 2024-04-30 07:10:43.000000 request_response_logging-1.0.0/request_response_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      510 2024-04-30 07:10:43.000000 request_response_logging-1.0.0/request_response_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)        1 2024-04-30 07:10:43.000000 request_response_logging-1.0.0/request_response_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       11 2024-04-30 07:10:43.000000 request_response_logging-1.0.0/request_response_logging.egg-info/requires.txt
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       16 2024-04-30 07:10:43.000000 request_response_logging-1.0.0/request_response_logging.egg-info/top_level.txt
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)       38 2024-04-30 07:10:43.499419 request_response_logging-1.0.0/setup.cfg
+-rw-rw-r--   0 praveentiwari  (1001) praveentiwari  (1001)      590 2024-04-30 07:10:26.000000 request_response_logging-1.0.0/setup.py
```

### Comparing `request_response_logging-0.0.9/PKG-INFO` & `request_response_logging-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: request_response_logging
-Version: 0.0.9
+Version: 1.0.0
 Summary: Django logger to log request response
 Home-page: UNKNOWN
 Author: Pravin Tiwari
 Author-email: pravint198@gmail.com
 License: UNKNOWN
 Description: # request-response-logging
```

### Comparing `request_response_logging-0.0.9/README.md` & `request_response_logging-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `request_response_logging-0.0.9/request_logging/Filters/LoggingFilters.py` & `request_response_logging-1.0.0/request_logging/Filters/LoggingFilters.py`

 * *Files identical despite different names*

### Comparing `request_response_logging-0.0.9/request_logging/decorators.py` & `request_response_logging-1.0.0/request_logging/decorators.py`

 * *Files identical despite different names*

### Comparing `request_response_logging-0.0.9/request_logging/middleware/RequestResponseLogging.py` & `request_response_logging-1.0.0/request_logging/middleware/RequestResponseLogging.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,21 +117,24 @@
 
 
         logger.info(json.dumps(log_request))
 
     @staticmethod
     def log_error_request(request, error):
         request_data = None
-        if request.method == 'GET':
-            request_data = request.GET
-        elif request.method == 'POST':
-            if request.POST:
-                request_data = request.POST
-            else:
-                request_data = request.body
+        try:
+            if request.method == 'GET':
+                request_data = request.GET
+            elif request.method == 'POST':
+                if request.POST:
+                    request_data = request.POST
+                else:
+                    request_data = request.body
+        except:
+            pass
         logger.error(f'request_data: {request_data}, '
                      f'request_error: {error}')
 
     def log_response(self, request, response):
         response_content = None
         try:
             if hasattr(response, 'streaming_content'):
```

### Comparing `request_response_logging-0.0.9/request_response_logging.egg-info/PKG-INFO` & `request_response_logging-1.0.0/request_response_logging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: request-response-logging
-Version: 0.0.9
+Version: 1.0.0
 Summary: Django logger to log request response
 Home-page: UNKNOWN
 Author: Pravin Tiwari
 Author-email: pravint198@gmail.com
 License: UNKNOWN
 Description: # request-response-logging
```

