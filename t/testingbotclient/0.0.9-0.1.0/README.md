# Comparing `tmp/testingbotclient-0.0.9.tar.gz` & `tmp/testingbotclient-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testingbotclient-0.0.9.tar", last modified: Sun Aug  7 09:25:16 2022, max compression
+gzip compressed data, was "testingbotclient-0.1.0.tar", last modified: Tue Apr 30 13:59:14 2024, max compression
```

## Comparing `testingbotclient-0.0.9.tar` & `testingbotclient-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jochen     (501) staff       (20)        0 2022-08-07 09:25:16.265902 testingbotclient-0.0.9/
--rw-r--r--   0 jochen     (501) staff       (20)     1073 2021-05-05 09:38:16.000000 testingbotclient-0.0.9/LICENSE.txt
--rw-r--r--   0 jochen     (501) staff       (20)     1205 2022-08-07 09:25:16.265998 testingbotclient-0.0.9/PKG-INFO
--rw-r--r--   0 jochen     (501) staff       (20)     4980 2021-05-05 09:49:33.000000 testingbotclient-0.0.9/README.md
--rw-r--r--   0 jochen     (501) staff       (20)       79 2022-08-07 09:25:16.266328 testingbotclient-0.0.9/setup.cfg
--rw-r--r--   0 jochen     (501) staff       (20)     1506 2021-05-05 09:38:16.000000 testingbotclient-0.0.9/setup.py
-drwxr-xr-x   0 jochen     (501) staff       (20)        0 2022-08-07 09:25:16.265733 testingbotclient-0.0.9/testingbotclient.egg-info/
--rw-r--r--   0 jochen     (501) staff       (20)     1205 2022-08-07 09:25:15.000000 testingbotclient-0.0.9/testingbotclient.egg-info/PKG-INFO
--rw-r--r--   0 jochen     (501) staff       (20)      259 2022-08-07 09:25:16.000000 testingbotclient-0.0.9/testingbotclient.egg-info/SOURCES.txt
--rw-r--r--   0 jochen     (501) staff       (20)        1 2022-08-07 09:25:15.000000 testingbotclient-0.0.9/testingbotclient.egg-info/dependency_links.txt
--rw-r--r--   0 jochen     (501) staff       (20)        9 2022-08-07 09:25:16.000000 testingbotclient-0.0.9/testingbotclient.egg-info/requires.txt
--rw-r--r--   0 jochen     (501) staff       (20)       17 2022-08-07 09:25:16.000000 testingbotclient-0.0.9/testingbotclient.egg-info/top_level.txt
--rw-r--r--   0 jochen     (501) staff       (20)     8106 2022-08-07 09:14:24.000000 testingbotclient-0.0.9/testingbotclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:59:14.233294 testingbotclient-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 13:59:10.000000 testingbotclient-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-30 13:59:14.233294 testingbotclient-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-30 13:59:10.000000 testingbotclient-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 13:59:14.237294 testingbotclient-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-30 13:59:10.000000 testingbotclient-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:59:14.233294 testingbotclient-0.1.0/testingbotclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-30 13:59:14.000000 testingbotclient-0.1.0/testingbotclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-30 13:59:14.000000 testingbotclient-0.1.0/testingbotclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:59:14.000000 testingbotclient-0.1.0/testingbotclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 13:59:14.000000 testingbotclient-0.1.0/testingbotclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 13:59:14.000000 testingbotclient-0.1.0/testingbotclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-30 13:59:10.000000 testingbotclient-0.1.0/testingbotclient.py
```

### Comparing `testingbotclient-0.0.9/LICENSE.txt` & `testingbotclient-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testingbotclient-0.0.9/PKG-INFO` & `testingbotclient-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testingbotclient
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python client library for TestingBot API.
 Home-page: https://github.com/testingbot/testingbotclient
 Download-URL: http://pypi.python.org/pypi/testingbotclient
 Author: TestingBot
 Author-email: info@testingbot.com
 License: Apache v2.0
 Keywords: testingbot,selenium,testing
@@ -19,9 +19,10 @@
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 License-File: LICENSE.txt
+Requires-Dist: requests
 
 Update test details on TestingBot.com with this library. Set success state/name of test after running the Selenium test.
```

### Comparing `testingbotclient-0.0.9/README.md` & `testingbotclient-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `testingbotclient-0.0.9/setup.py` & `testingbotclient-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `testingbotclient-0.0.9/testingbotclient.egg-info/PKG-INFO` & `testingbotclient-0.1.0/testingbotclient.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testingbotclient
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python client library for TestingBot API.
 Home-page: https://github.com/testingbot/testingbotclient
 Download-URL: http://pypi.python.org/pypi/testingbotclient
 Author: TestingBot
 Author-email: info@testingbot.com
 License: Apache v2.0
 Keywords: testingbot,selenium,testing
@@ -19,9 +19,10 @@
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 License-File: LICENSE.txt
+Requires-Dist: requests
 
 Update test details on TestingBot.com with this library. Set success state/name of test after running the Selenium test.
```

### Comparing `testingbotclient-0.0.9/testingbotclient.py` & `testingbotclient-0.1.0/testingbotclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 import json
 import os
 import requests
 from requests.auth import HTTPBasicAuth
 import hashlib
 
-__version__ = '0.0.9'
+__version__ = '0.1.0'
 
 class TestingBotException(Exception):
     def __init__(self, *args, **kwargs):
         super(TestingBotException, self).__init__(*args)
         self.response = kwargs.get('response')
 
 class TestingBotClient(object):
@@ -81,15 +81,15 @@
     def get_test_ids(self):
         """List all tests sessionId's belonging to the user."""
         url = '/tests'
         tests = self.client.get(method, url)
         test_ids = [attr['session_id'] for attr in tests['data']]
         return test_ids
 
-    def get_tests(self, offset = 0, limit = 30):
+    def get_tests(self, offset = 0, limit = 10):
         """List all tests belonging to the user."""
         url = '/tests?offset=' + str(offset) + '&count=' + str(limit)
         tests = self.client.get(url)
         return tests["data"]
 
     def get_test(self, sessionId):
         """Get meta-data for a specific test"""
@@ -126,28 +126,29 @@
 
 class Storage(object):
     def __init__(self, client):
         self.client = client
 
     def upload_local_file(self, filepath):
         """Uploads a local file to TestingBot Storage."""
-        return requests.post(self.client.api_url + "/storage", files={'file': open(filepath, 'rb')}, auth=(self.client.testingbotKey, self.client.testingbotSecret)).json()
+        with open(filepath, 'rb') as f: file_contents = f.read()
+        return requests.post(self.client.api_url + "/storage", files={'file': file_contents}, auth=(self.client.testingbotKey, self.client.testingbotSecret)).json()
 
     def upload_remote_file(self, remoteUrl):
         return self.client.post("/storage", { 'url': remoteUrl })
 
     def get_stored_file(self, app_url):
         """Retrieves meta-data for a file previously uploaded to TestingBot Storage."""
         return self.client.get("/storage/" + app_url.replace("tb://", ""))
 
     def remove_file(self, app_url):
         """Removes a file previously uploaded to TestingBot Storage."""
         return self.client.delete("/storage/" + app_url.replace("tb://", ""))
 
-    def get_stored_files(self, offset = 0, limit = 30):
+    def get_stored_files(self, offset = 0, limit = 10):
         """Retrieves all files previously uploaded to TestingBot Storage."""
         return self.client.get("/storage/?count=" + str(limit) + "&offset=" + str(offset))
 
 class Information(object):
     def __init__(self, client):
         self.client = client
 
@@ -187,15 +188,15 @@
         """Delete a specific TestingBot Tunnel"""
         return self.client.delete('/tunnel/' + tunnelId)
 
 class Build(object):
     def __init__(self, client):
         self.client = client
 
-    def get_builds(self, offset = 0, limit = 30):
+    def get_builds(self, offset = 0, limit = 10):
         """Get all builds"""
         return self.client.get('/builds?offset=' + str(offset) + '&count=' + str(limit))
 
     def get_tests_for_build(self, buildId):
         """Get tests for a specific build"""
         return self.client.get('/builds/' + buildId)
 
@@ -213,9 +214,9 @@
         url = '/user'
         info = self.client.get(url)
         return info
 
     def update_user_information(self, newUser):
         """Update current user information"""
         url = '/user'
-        info = self.client.put(url)
+        info = self.client.put(url, newUser)
         return info
```

