# Comparing `tmp/jam_twitter_api-0.1.tar.gz` & `tmp/jam_twitter_api-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jam_twitter_api-0.1.tar", last modified: Tue Apr 30 13:17:28 2024, max compression
+gzip compressed data, was "jam_twitter_api-0.2.tar", last modified: Tue Apr 30 13:26:10 2024, max compression
```

## Comparing `jam_twitter_api-0.1.tar` & `jam_twitter_api-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 13:17:28.263314 jam_twitter_api-0.1/
-drwxrwxrwx   0        0        0        0 2024-04-30 13:17:28.238093 jam_twitter_api-0.1/Jam_Twitter_API/
--rw-rw-rw-   0        0        0    61917 2024-04-30 12:58:29.000000 jam_twitter_api-0.1/Jam_Twitter_API/account.py
--rw-rw-rw-   0        0        0    34314 2024-04-24 11:59:57.000000 jam_twitter_api-0.1/Jam_Twitter_API/constants.py
--rw-rw-rw-   0        0        0     2888 2024-03-29 16:21:39.000000 jam_twitter_api-0.1/Jam_Twitter_API/errors.py
--rw-rw-rw-   0        0        0     5597 2024-04-24 12:48:05.000000 jam_twitter_api-0.1/Jam_Twitter_API/util.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:17:28.261313 jam_twitter_api-0.1/Jam_Twitter_API.egg-info/
--rw-rw-rw-   0        0        0     3245 2024-04-30 13:17:28.000000 jam_twitter_api-0.1/Jam_Twitter_API.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-04-30 13:17:28.000000 jam_twitter_api-0.1/Jam_Twitter_API.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 13:17:28.000000 jam_twitter_api-0.1/Jam_Twitter_API.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-30 13:17:28.000000 jam_twitter_api-0.1/Jam_Twitter_API.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2024-04-30 12:25:11.000000 jam_twitter_api-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3245 2024-04-30 13:17:28.262313 jam_twitter_api-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2697 2024-04-30 13:09:57.000000 jam_twitter_api-0.1/README.md
--rw-rw-rw-   0        0        0      620 2024-04-30 13:16:46.000000 jam_twitter_api-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 13:17:28.264548 jam_twitter_api-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 13:26:10.222004 jam_twitter_api-0.2/
+drwxrwxrwx   0        0        0        0 2024-04-30 13:26:10.199246 jam_twitter_api-0.2/Jam_Twitter_API/
+-rw-rw-rw-   0        0        0    61921 2024-04-30 13:24:36.000000 jam_twitter_api-0.2/Jam_Twitter_API/account.py
+-rw-rw-rw-   0        0        0    34314 2024-04-24 11:59:57.000000 jam_twitter_api-0.2/Jam_Twitter_API/constants.py
+-rw-rw-rw-   0        0        0     2888 2024-03-29 16:21:39.000000 jam_twitter_api-0.2/Jam_Twitter_API/errors.py
+-rw-rw-rw-   0        0        0     5597 2024-04-24 12:48:05.000000 jam_twitter_api-0.2/Jam_Twitter_API/util.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:26:10.219401 jam_twitter_api-0.2/Jam_Twitter_API.egg-info/
+-rw-rw-rw-   0        0        0     3249 2024-04-30 13:26:10.000000 jam_twitter_api-0.2/Jam_Twitter_API.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2024-04-30 13:26:10.000000 jam_twitter_api-0.2/Jam_Twitter_API.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 13:26:10.000000 jam_twitter_api-0.2/Jam_Twitter_API.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-30 13:26:10.000000 jam_twitter_api-0.2/Jam_Twitter_API.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2024-04-30 12:25:11.000000 jam_twitter_api-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3249 2024-04-30 13:26:10.220604 jam_twitter_api-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2701 2024-04-30 13:22:02.000000 jam_twitter_api-0.2/README.md
+-rw-rw-rw-   0        0        0      620 2024-04-30 13:25:55.000000 jam_twitter_api-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 13:26:10.222004 jam_twitter_api-0.2/setup.cfg
```

### Comparing `jam_twitter_api-0.1/Jam_Twitter_API/account.py` & `jam_twitter_api-0.2/Jam_Twitter_API/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,25 +21,27 @@
 from tqdm import tqdm
 
 from .constants import *
 from .errors import TwitterAccountSuspended, RateLimitError, IncorrectData
 from .util import *
 
 
+
 if platform.system() != "Windows":
     try:
         import uvloop
 
         uvloop.install()
     except ImportError as e:
         ...
     except:
         ...
 
 
+
 class TwitterAccount:
     def __init__(self):
         self._session: requests.Session = requests.Session()
 
         self.gql_api = "https://twitter.com/i/api/graphql"
         self.v1_api = "https://api.twitter.com/1.1"
         self.v2_api = "https://twitter.com/i/api/2"
```

### Comparing `jam_twitter_api-0.1/Jam_Twitter_API/constants.py` & `jam_twitter_api-0.2/Jam_Twitter_API/constants.py`

 * *Files identical despite different names*

### Comparing `jam_twitter_api-0.1/Jam_Twitter_API/errors.py` & `jam_twitter_api-0.2/Jam_Twitter_API/errors.py`

 * *Files identical despite different names*

### Comparing `jam_twitter_api-0.1/Jam_Twitter_API/util.py` & `jam_twitter_api-0.2/Jam_Twitter_API/util.py`

 * *Files identical despite different names*

### Comparing `jam_twitter_api-0.1/Jam_Twitter_API.egg-info/PKG-INFO` & `jam_twitter_api-0.2/Jam_Twitter_API.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jam_Twitter_API
-Version: 0.1
+Version: 0.2
 Summary: Implementation of X/Twitter v1, v2, and GraphQL APIs
 Author-email: Jaammerr <jaammer.dev@gmail.com>
 Project-URL: Homepage, https://github.com/Jaammerr/Twitter-API
 Project-URL: Issues, https://github.com/Jaammerr/Twitter-API/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,22 +13,22 @@
 License-File: LICENSE.txt
 
 # Twitter API
 
 ## Installation
 
 ```bash 
-pip install twitter_api
+pip install Jam-Twitter-API
 ```
 
 ## Usage
 
 ```python
-from jam_twitter_api.account import TwitterAccount
-from jam_twitter_api.errors import *
+from Jam_Twitter_API.account import TwitterAccount
+from Jam_Twitter_API.errors import *
 
 
 # Create a TwitterAccount object
 # Set up a session using auth_token or cookies (it will auto create needed headers and cookies)
 try:
     account = TwitterAccount.run(
         auth_token="0idfidfgdfgidfgijodfgjoidfgijo43",
```

### Comparing `jam_twitter_api-0.1/LICENSE.txt` & `jam_twitter_api-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jam_twitter_api-0.1/PKG-INFO` & `jam_twitter_api-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jam_Twitter_API
-Version: 0.1
+Version: 0.2
 Summary: Implementation of X/Twitter v1, v2, and GraphQL APIs
 Author-email: Jaammerr <jaammer.dev@gmail.com>
 Project-URL: Homepage, https://github.com/Jaammerr/Twitter-API
 Project-URL: Issues, https://github.com/Jaammerr/Twitter-API/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,22 +13,22 @@
 License-File: LICENSE.txt
 
 # Twitter API
 
 ## Installation
 
 ```bash 
-pip install twitter_api
+pip install Jam-Twitter-API
 ```
 
 ## Usage
 
 ```python
-from jam_twitter_api.account import TwitterAccount
-from jam_twitter_api.errors import *
+from Jam_Twitter_API.account import TwitterAccount
+from Jam_Twitter_API.errors import *
 
 
 # Create a TwitterAccount object
 # Set up a session using auth_token or cookies (it will auto create needed headers and cookies)
 try:
     account = TwitterAccount.run(
         auth_token="0idfidfgdfgidfgijodfgjoidfgijo43",
```

### Comparing `jam_twitter_api-0.1/README.md` & `jam_twitter_api-0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Twitter API
 
 ## Installation
 
 ```bash 
-pip install twitter_api
+pip install Jam-Twitter-API
 ```
 
 ## Usage
 
 ```python
-from jam_twitter_api.account import TwitterAccount
-from jam_twitter_api.errors import *
+from Jam_Twitter_API.account import TwitterAccount
+from Jam_Twitter_API.errors import *
 
 
 # Create a TwitterAccount object
 # Set up a session using auth_token or cookies (it will auto create needed headers and cookies)
 try:
     account = TwitterAccount.run(
         auth_token="0idfidfgdfgidfgijodfgjoidfgijo43",
```

### Comparing `jam_twitter_api-0.1/pyproject.toml` & `jam_twitter_api-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Jam_Twitter_API"
-version = "0.1"
+version = "0.2"
 authors = [
   { name="Jaammerr", email="jaammer.dev@gmail.com" },
 ]
 description = "Implementation of X/Twitter v1, v2, and GraphQL APIs"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

