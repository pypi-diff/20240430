# Comparing `tmp/dctrackclient-1.2.2.tar.gz` & `tmp/dctrackclient-9.1.1.tar.gz`

## Comparing `dctrackclient-1.2.2.tar` & `dctrackclient-9.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    44315 2020-02-02 00:00:00.000000 dctrackclient-1.2.2/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 dctrackclient-1.2.2/.gitignore
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 dctrackclient-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    45979 2020-02-02 00:00:00.000000 dctrackclient-1.2.2/../README.md
--rw-r--r--   0        0        0    46669 2020-02-02 00:00:00.000000 dctrackclient-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    44315 2020-02-02 00:00:00.000000 dctrackclient-9.1.1/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 dctrackclient-9.1.1/.gitignore
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 dctrackclient-9.1.1/pyproject.toml
+-rw-r--r--   0        0        0    45979 2020-02-02 00:00:00.000000 dctrackclient-9.1.1/../README.md
+-rw-r--r--   0        0        0    46669 2020-02-02 00:00:00.000000 dctrackclient-9.1.1/PKG-INFO
```

### Comparing `dctrackclient-1.2.2/src/dcTrackClient/__init__.py` & `dctrackclient-9.1.1/src/dcTrackClient/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 
 
 class Client:
-    """Sunbird dcTrack API client version 1.2.2 in Python"""
+    """Sunbird dcTrack API client version 9.1.1 in Python"""
 
     def __init__(self, baseUrl: str, username: str = '', password: str = '', apiToken: str = '', httpProxy: str = '', httpsProxy: str = ''):
         """Provide either a username and password, or an API token to access the dcTrack database with Python."""
         self.__BASE_URL = baseUrl
         self.__USERNAME = username
         self.__PASSWORD = password
         self.__APITOKEN = apiToken
```

### Comparing `dctrackclient-1.2.2/pyproject.toml` & `dctrackclient-9.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "1.2.2"
+version = "9.1.1"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "../README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-1.2.2/../README.md` & `dctrackclient-9.1.1/../README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==1.2.2
+pip install dcTrackClient==9.1.1
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@1.2.2
+npm i dctrackclient@9.1.1
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -201,15 +201,15 @@
 { "itemId": 1234 }
 ```
 
 # Official DcTrack Documentation
 
 Visit this link for the official documentation on request bodies and attrribute names.
 
-https://www.sunbirddcim.com/help/dcTrack/v910/API/en/Default.htm
+https://www.sunbirddcim.com/help/dcTrack/v911/API/en/Default.htm
 
 # Package Documentation
 
 The section below shows all the functions contained within this client along with basic usage.
 
 ## getItem(id)
 > Get item details using the item ID. Returns an Item JSON object.
```

### Comparing `dctrackclient-1.2.2/PKG-INFO` & `dctrackclient-9.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dcTrackClient
-Version: 1.2.2
+Version: 9.1.1
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -20,20 +20,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==1.2.2
+pip install dcTrackClient==9.1.1
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@1.2.2
+npm i dctrackclient@9.1.1
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -219,15 +219,15 @@
 { "itemId": 1234 }
 ```
 
 # Official DcTrack Documentation
 
 Visit this link for the official documentation on request bodies and attrribute names.
 
-https://www.sunbirddcim.com/help/dcTrack/v910/API/en/Default.htm
+https://www.sunbirddcim.com/help/dcTrack/v911/API/en/Default.htm
 
 # Package Documentation
 
 The section below shows all the functions contained within this client along with basic usage.
 
 ## getItem(id)
 > Get item details using the item ID. Returns an Item JSON object.
```

