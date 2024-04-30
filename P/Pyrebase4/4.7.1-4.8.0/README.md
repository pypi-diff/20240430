# Comparing `tmp/Pyrebase4-4.7.1.tar.gz` & `tmp/pyrebase4-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pyrebase4-4.7.1.tar", last modified: Tue Jun 13 18:20:27 2023, max compression
+gzip compressed data, was "pyrebase4-4.8.0.tar", last modified: Tue Apr 30 18:18:52 2024, max compression
```

## Comparing `Pyrebase4-4.7.1.tar` & `pyrebase4-4.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-06-13 18:20:27.215499 Pyrebase4-4.7.1/
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      412 2023-06-13 18:20:27.215499 Pyrebase4-4.7.1/PKG-INFO
-drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-06-13 18:20:27.215499 Pyrebase4-4.7.1/Pyrebase4.egg-info/
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      412 2023-06-13 18:20:27.000000 Pyrebase4-4.7.1/Pyrebase4.egg-info/PKG-INFO
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      294 2023-06-13 18:20:27.000000 Pyrebase4-4.7.1/Pyrebase4.egg-info/SOURCES.txt
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)        1 2023-06-13 18:20:27.000000 Pyrebase4-4.7.1/Pyrebase4.egg-info/dependency_links.txt
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      145 2023-06-13 18:20:27.000000 Pyrebase4-4.7.1/Pyrebase4.egg-info/requires.txt
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)        9 2023-06-13 18:20:27.000000 Pyrebase4-4.7.1/Pyrebase4.egg-info/top_level.txt
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)    13752 2023-05-14 14:05:14.000000 Pyrebase4-4.7.1/README.md
-drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-06-13 18:20:27.215499 Pyrebase4-4.7.1/pyrebase/
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       36 2022-11-30 18:49:25.000000 Pyrebase4-4.7.1/pyrebase/__init__.py
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)     5395 2022-11-30 18:49:25.000000 Pyrebase4-4.7.1/pyrebase/pyre_sseclient.py
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)    26616 2023-05-14 13:59:31.000000 Pyrebase4-4.7.1/pyrebase/pyrebase.py
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       38 2023-06-13 18:20:27.215499 Pyrebase4-4.7.1/setup.cfg
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      802 2023-06-13 18:20:25.000000 Pyrebase4-4.7.1/setup.py
-drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-06-13 18:20:27.215499 Pyrebase4-4.7.1/tests/
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)     5247 2022-11-30 18:49:25.000000 Pyrebase4-4.7.1/tests/test_database.py
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       95 2022-11-30 18:49:25.000000 Pyrebase4-4.7.1/tests/test_setup.py
+drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2024-04-30 18:18:52.909222 pyrebase4-4.8.0/
+-rw-r--r--   0 nhorvath  (1001) nhorvath  (1001)      654 2024-04-30 18:18:52.905222 pyrebase4-4.8.0/PKG-INFO
+drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2024-04-30 18:18:52.905222 pyrebase4-4.8.0/Pyrebase4.egg-info/
+-rw-r--r--   0 nhorvath  (1001) nhorvath  (1001)      654 2024-04-30 18:18:52.000000 pyrebase4-4.8.0/Pyrebase4.egg-info/PKG-INFO
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      294 2024-04-30 18:18:52.000000 pyrebase4-4.8.0/Pyrebase4.egg-info/SOURCES.txt
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)        1 2024-04-30 18:18:52.000000 pyrebase4-4.8.0/Pyrebase4.egg-info/dependency_links.txt
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      137 2024-04-30 18:18:52.000000 pyrebase4-4.8.0/Pyrebase4.egg-info/requires.txt
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)        9 2024-04-30 18:18:52.000000 pyrebase4-4.8.0/Pyrebase4.egg-info/top_level.txt
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)    12485 2024-04-30 18:16:47.000000 pyrebase4-4.8.0/README.md
+drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2024-04-30 18:18:52.905222 pyrebase4-4.8.0/pyrebase/
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       36 2024-04-30 18:16:47.000000 pyrebase4-4.8.0/pyrebase/__init__.py
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)     5395 2024-04-30 18:16:47.000000 pyrebase4-4.8.0/pyrebase/pyre_sseclient.py
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)    26842 2024-04-30 18:16:47.000000 pyrebase4-4.8.0/pyrebase/pyrebase.py
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       38 2024-04-30 18:18:52.909222 pyrebase4-4.8.0/setup.cfg
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      794 2024-04-30 18:18:00.000000 pyrebase4-4.8.0/setup.py
+drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2024-04-30 18:18:52.905222 pyrebase4-4.8.0/tests/
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)     5247 2024-04-30 18:16:47.000000 pyrebase4-4.8.0/tests/test_database.py
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       95 2024-04-30 18:16:47.000000 pyrebase4-4.8.0/tests/test_setup.py
```

### Comparing `Pyrebase4-4.7.1/README.md` & `pyrebase4-4.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -292,56 +292,25 @@
 #### each
 Returns a list of objects on each of which you can call ```val()``` and ```key()```.
 
 ```
 all_users = db.child("users").get()
 for user in all_users.each():
     print(user.key()) # Morty
-    print(user.val()) # {name": "Mortimer 'Morty' Smith"}
+    print(user.val()) # {"name": "Mortimer 'Morty' Smith"}
 ```
 
 #### get
 
 To return data from a path simply call the ```get()``` method.
 
 ```python
 all_users = db.child("users").get()
 ```
 
-#### Conditional Requests
-
-It's possible to do conditional sets and removes by using the `conditional_set()` and `conitional_remove()` methods respectively. You can read more about conditional requests in Firebase [here](https://firebase.google.com/docs/reference/rest/database/#section-conditional-requests).
-
-To use these methods, you first get the ETag of a particular path by using the `get_etag()` method. You can then use that tag in your conditional request.
-
-```python
-etag = db.child("users").child("Morty").get_etag()
-data = {"name": "Mortimer 'Morty' Smith"}
-db.child("users").child("Morty").conditional_set(data, etag)
-```
-
-If the passed ETag does not match the ETag of the path in the database, the data will not be written, and both conditional request methods will return a single key-value pair with the new ETag to use of the following form:
-
-```json
-{ "ETag": "8KnE63B6HiKp67Wf3HQrXanujSM=" }
-```
-
-Here's an example of checking whether or not a conditional removal was successful:
-
-```python
-etag = db.child("users").child("Morty").get_etag()
-response = db.child("users").child("Morty").conditional_remove(etag)
-
-if "ETag" in response:
-    etag = response["ETag"] # our ETag was out-of-date
-else:
-    print("We removed the data successfully!")
-```
-
-
 #### shallow
 
 To return just the keys at a particular path use the ```shallow()``` method.
 
 ```python
 all_user_ids = db.child("users").shallow().get()
 ```
```

### Comparing `Pyrebase4-4.7.1/pyrebase/pyre_sseclient.py` & `pyrebase4-4.8.0/pyrebase/pyre_sseclient.py`

 * *Files identical despite different names*

### Comparing `Pyrebase4-4.7.1/pyrebase/pyrebase.py` & `pyrebase4-4.8.0/pyrebase/pyrebase.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import requests
 from requests import Session
+from requests.adapters import HTTPAdapter
 from requests.exceptions import HTTPError
+from urllib3.contrib.appengine import is_appengine_sandbox
 
-try:
-    from urllib.parse import urlencode, quote
-except:
-    from urllib import urlencode, quote
+from urllib.parse import urlencode, quote
 import json
 import math
 from random import randrange
 import time
 from collections import OrderedDict
 from .pyre_sseclient import SSEClient
 import threading
 import socket
 from oauth2client.service_account import ServiceAccountCredentials
 from gcloud import storage
-from requests.packages.urllib3.contrib.appengine import is_appengine_sandbox
 from requests_toolbelt.adapters import appengine
 from uuid import uuid4
 
 import python_jwt as jwt
 from Crypto.PublicKey import RSA
 import datetime
 
@@ -51,15 +49,15 @@
                 self.credentials = ServiceAccountCredentials.from_json_keyfile_dict(config["serviceAccount"], scopes)
         if is_appengine_sandbox():
             # Fix error in standard GAE environment
             # is releated to https://github.com/kennethreitz/requests/issues/3187
             # ProtocolError('Connection aborted.', error(13, 'Permission denied'))
             adapter = appengine.AppEngineAdapter(max_retries=3)
         else:
-            adapter = requests.adapters.HTTPAdapter(max_retries=3)
+            adapter = HTTPAdapter()
 
         for scheme in ('http://', 'https://'):
             self.requests.mount(scheme, adapter)
 
     def auth(self):
         return Auth(self.api_key, self.requests, self.credentials)
 
@@ -278,15 +276,16 @@
     def build_headers(self, token=None):
         headers = {"content-type": "application/json; charset=UTF-8"}
         if not token and self.credentials:
             access_token = self.credentials.get_access_token().access_token
             headers['Authorization'] = 'Bearer ' + access_token
         return headers
 
-    def get(self, token=None, json_kwargs={}):
+    def get(self, token=None, json_kwargs=None):
+        json_kwargs = json_kwargs or {}
         build_query = self.build_query
         query_key = self.path.split("/")[-1]
         request_ref = self.build_request_url(token)
         # headers
         headers = self.build_headers(token)
         # do request
         request_object = self.requests.get(request_ref, headers=headers)
@@ -310,31 +309,34 @@
                 sorted_response = sorted(request_dict.items(), key=lambda item: item[0])
             elif build_query["orderBy"] == "$value":
                 sorted_response = sorted(request_dict.items(), key=lambda item: item[1])
             else:
                 sorted_response = sorted(request_dict.items(), key=lambda item: (build_query["orderBy"] in item[1], item[1].get(build_query["orderBy"], "")))
         return PyreResponse(convert_to_pyre(sorted_response), query_key)
 
-    def push(self, data, token=None, json_kwargs={}):
+    def push(self, data, token=None, json_kwargs=None):
+        json_kwargs = json_kwargs or {}
         request_ref = self.check_token(self.database_url, self.path, token)
         self.path = ""
         headers = self.build_headers(token)
         request_object = self.requests.post(request_ref, headers=headers, data=json.dumps(data, **json_kwargs).encode("utf-8"))
         raise_detailed_error(request_object)
         return request_object.json()
 
-    def set(self, data, token=None, json_kwargs={}):
+    def set(self, data, token=None, json_kwargs=None):
+        json_kwargs = json_kwargs or {}
         request_ref = self.check_token(self.database_url, self.path, token)
         self.path = ""
         headers = self.build_headers(token)
         request_object = self.requests.put(request_ref, headers=headers, data=json.dumps(data, **json_kwargs).encode("utf-8"))
         raise_detailed_error(request_object)
         return request_object.json()
 
-    def update(self, data, token=None, json_kwargs={}):
+    def update(self, data, token=None, json_kwargs=None):
+        json_kwargs = json_kwargs or {}
         request_ref = self.check_token(self.database_url, self.path, token)
         self.path = ""
         headers = self.build_headers(token)
         request_object = self.requests.patch(request_ref, headers=headers, data=json.dumps(data, **json_kwargs).encode("utf-8"))
         raise_detailed_error(request_object)
         return request_object.json()
 
@@ -383,27 +385,29 @@
         new_list = []
         for pyre in pyres:
             new_list.append(pyre.item)
         # sort
         data = sorted(dict(new_list).items(), key=lambda item: item[1][by_key], reverse=reverse)
         return PyreResponse(convert_to_pyre(data), origin.key())
 
-    def get_etag(self, token=None, json_kwargs={}):
+    def get_etag(self, token=None, json_kwargs=None):
+        json_kwargs = json_kwargs or {}
         request_ref = self.build_request_url(token)
         headers = self.build_headers(token)
         # extra header to get ETag
         headers['X-Firebase-ETag'] = 'true'
         request_object = self.requests.get(request_ref, headers=headers)
         raise_detailed_error(request_object)
         return {
            'ETag': request_object.headers['ETag'],
            'value': request_object.json()
         }
 
-    def conditional_set(self, data, etag, token=None, json_kwargs={}):
+    def conditional_set(self, data, etag, token=None, json_kwargs=None):
+        json_kwargs = json_kwargs or {}
         request_ref = self.check_token(self.database_url, self.path, token)
         self.path = ""
         headers = self.build_headers(token)
         headers['if-match'] = etag
         request_object = self.requests.put(request_ref, headers=headers, data=json.dumps(data, **json_kwargs).encode("utf-8"))
 
         # ETag didn't match, so we should return the correct one for the user to try again
@@ -487,27 +491,27 @@
             raise_detailed_error(request_object)
             return request_object.json()
 
     def delete(self, name, token):
         if self.credentials:
             self.bucket.delete_blob(name)
         else:
-            request_ref = self.storage_bucket + "/o?name={0}".format(name)
+            request_ref = self.storage_bucket + "/o/?name={0}".format(name)
             if token:
                 headers = {"Authorization": "Firebase " + token}
                 request_object = self.requests.delete(request_ref, headers=headers)
             else:
                 request_object = self.requests.delete(request_ref)
             raise_detailed_error(request_object)
 
     def download(self, path, filename, token=None):
         # remove leading backlash
         url = self.get_url(token)
         if path.startswith('/'):
-            path = path[1:]
+            path = path.lstrip('/')
         if self.credentials:
             blob = self.bucket.get_blob(path)
             if not blob is None:
                 blob.download_to_filename(filename)
         elif token:
              headers = {"Authorization": "Firebase " + token}
              r = requests.get(url, stream=True, headers=headers)
@@ -519,18 +523,18 @@
             r = requests.get(url, stream=True)
             if r.status_code == 200:
                 with open(filename, 'wb') as f:
                     for chunk in r:
                         f.write(chunk)
 
     def get_url(self, token):
-        path = self.path
+        path = self.path if self.path else ''
         self.path = None
         if path.startswith('/'):
-            path = path[1:]
+            path = path.lstrip('/')
         if token:
             return "{0}/o/{1}?alt=media&token={2}".format(self.storage_bucket, quote(path, safe=''), token)
         return "{0}/o/{1}?alt=media".format(self.storage_bucket, quote(path, safe=''))
 
     def list_files(self):
         return self.bucket.list_blobs()
```

### Comparing `Pyrebase4-4.7.1/setup.py` & `pyrebase4-4.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Pyrebase4',
-    version='4.7.1',
+    version='4.8.0',
     url='https://github.com/nhorvath/Pyrebase4',
     description='A simple python wrapper for the Firebase API with current deps',
     author='nhorvath',
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.4',
     ],
     keywords='Firebase',
     packages=find_packages(exclude=['tests']),
     install_requires=[
         'requests-toolbelt>=0.7.1,<1.0',
-        'requests>=2.19.1,<2.30',
+        'requests>=2.31',
         'urllib3>=1.21.1,<2',
         'gcloud>=0.18.3',
         'oauth2client>=4.1.2',
         'python-jwt>=2.0.1',
         'pycryptodome>=3.6.4'
     ]
 )
```

### Comparing `Pyrebase4-4.7.1/tests/test_database.py` & `pyrebase4-4.8.0/tests/test_database.py`

 * *Files identical despite different names*

