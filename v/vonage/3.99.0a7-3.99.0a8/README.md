# Comparing `tmp/vonage-3.99.0a7.tar.gz` & `tmp/vonage-3.99.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage-3.99.0a7.tar", last modified: Tue Apr 23 14:16:53 2024, max compression
+gzip compressed data, was "vonage-3.99.0a8.tar", last modified: Mon Apr 29 01:52:08 2024, max compression
```

## Comparing `vonage-3.99.0a7.tar` & `vonage-3.99.0a8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.222067 vonage-3.99.0a7/
--rw-r--r--   0 mkahan     (503) staff       (20)     2452 2024-04-23 14:16:53.221305 vonage-3.99.0a7/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     1429 2024-04-23 14:16:51.000000 vonage-3.99.0a7/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-23 14:16:51.000000 vonage-3.99.0a7/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1099 2024-04-23 14:16:51.000000 vonage-3.99.0a7/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-23 14:16:53.222118 vonage-3.99.0a7/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.213378 vonage-3.99.0a7/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.216748 vonage-3.99.0a7/src/vonage/
--rw-r--r--   0 mkahan     (503) staff       (20)      390 2024-04-23 14:16:51.000000 vonage-3.99.0a7/src/vonage/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)       25 2024-04-23 14:16:51.000000 vonage-3.99.0a7/src/vonage/_version.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1534 2024-04-23 14:16:51.000000 vonage-3.99.0a7/src/vonage/vonage.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.220396 vonage-3.99.0a7/src/vonage.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     2452 2024-04-23 14:16:53.000000 vonage-3.99.0a7/src/vonage.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      276 2024-04-23 14:16:53.000000 vonage-3.99.0a7/src/vonage.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-23 14:16:53.000000 vonage-3.99.0a7/src/vonage.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)      206 2024-04-23 14:16:53.000000 vonage-3.99.0a7/src/vonage.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        7 2024-04-23 14:16:53.000000 vonage-3.99.0a7/src/vonage.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:08.203313 vonage-3.99.0a8/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2496 2024-04-29 01:52:08.202703 vonage-3.99.0a8/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     1429 2024-04-29 01:52:07.000000 vonage-3.99.0a8/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-29 01:52:07.000000 vonage-3.99.0a8/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1133 2024-04-29 01:52:07.000000 vonage-3.99.0a8/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-29 01:52:08.203377 vonage-3.99.0a8/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:08.196635 vonage-3.99.0a8/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:08.198550 vonage-3.99.0a8/src/vonage/
+-rw-r--r--   0 mkahan     (503) staff       (20)      430 2024-04-29 01:52:07.000000 vonage-3.99.0a8/src/vonage/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)       25 2024-04-29 01:52:07.000000 vonage-3.99.0a8/src/vonage/_version.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1645 2024-04-29 01:52:07.000000 vonage-3.99.0a8/src/vonage/vonage.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:08.202040 vonage-3.99.0a8/src/vonage.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2496 2024-04-29 01:52:08.000000 vonage-3.99.0a8/src/vonage.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      276 2024-04-29 01:52:08.000000 vonage-3.99.0a8/src/vonage.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-29 01:52:08.000000 vonage-3.99.0a8/src/vonage.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)      235 2024-04-29 01:52:08.000000 vonage-3.99.0a8/src/vonage.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        7 2024-04-29 01:52:08.000000 vonage-3.99.0a8/src/vonage.egg-info/top_level.txt
```

### Comparing `vonage-3.99.0a7/PKG-INFO` & `vonage-3.99.0a8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: vonage
-Version: 3.99.0a7
+Version: 3.99.0a8
 Summary: Python Server SDK for using Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-utils>=1.1.0
-Requires-Dist: vonage-http-client>=1.3.0
-Requires-Dist: vonage-messages>=1.1.0
-Requires-Dist: vonage-number-insight-v2>=0.1.0b0
-Requires-Dist: vonage-sms>=1.1.0
-Requires-Dist: vonage-users>=1.1.0
-Requires-Dist: vonage-verify>=1.1.0
-Requires-Dist: vonage-verify-v2>=1.1.0
-Requires-Dist: vonage-voice>=1.0.1
+Requires-Dist: vonage-utils>=1.1.1
+Requires-Dist: vonage-http-client>=1.3.1
+Requires-Dist: vonage-messages>=1.1.1
+Requires-Dist: vonage-number-insight>=1.0.0
+Requires-Dist: vonage-number-insight-v2>=0.1.1b0
+Requires-Dist: vonage-sms>=1.1.1
+Requires-Dist: vonage-users>=1.1.1
+Requires-Dist: vonage-verify>=1.1.1
+Requires-Dist: vonage-verify-v2>=1.1.1
+Requires-Dist: vonage-voice>=1.0.2
 
 # Vonage Python SDK
 
 The Vonage Python SDK Package `vonage` provides a streamlined interface for using Vonage APIs in Python projects. This package includes the `Vonage` class, which simplifies API interactions.
 
 The Vonage class in this package serves as the main entry point for using Vonage APIs. It abstracts away complexities with authentication, HTTP requests and more.
```

### Comparing `vonage-3.99.0a7/README.md` & `vonage-3.99.0a8/README.md`

 * *Files identical despite different names*

### Comparing `vonage-3.99.0a7/backend_shim.py` & `vonage-3.99.0a8/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage-3.99.0a7/pyproject.toml` & `vonage-3.99.0a8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 name = "vonage"
 dynamic = ["version"]
 description = "Python Server SDK for using Vonage APIs"
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 requires-python = ">=3.8"
 dependencies = [
-  "vonage-utils>=1.1.0",
-  "vonage-http-client>=1.3.0",
-  "vonage-messages>=1.1.0",
-  "vonage-number-insight-v2>=0.1.0b0",
-  "vonage-sms>=1.1.0",
-  "vonage-users>=1.1.0",
-  "vonage-verify>=1.1.0",
-  "vonage-verify-v2>=1.1.0",
-  "vonage-voice>=1.0.1",
+  "vonage-utils>=1.1.1",
+  "vonage-http-client>=1.3.1",
+  "vonage-messages>=1.1.1",
+  "vonage-number-insight>=1.0.0",
+  "vonage-number-insight-v2>=0.1.1b0",
+  "vonage-sms>=1.1.1",
+  "vonage-users>=1.1.1",
+  "vonage-verify>=1.1.1",
+  "vonage-verify-v2>=1.1.1",
+  "vonage-voice>=1.0.2",
 ]
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `vonage-3.99.0a7/src/vonage/vonage.py` & `vonage-3.99.0a8/src/vonage/vonage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 
 from vonage_http_client import Auth, HttpClient, HttpClientOptions
 from vonage_messages import Messages
+from vonage_number_insight import NumberInsight
 from vonage_number_insight_v2 import NumberInsightV2
 from vonage_sms import Sms
 from vonage_users import Users
 from vonage_verify import Verify
 from vonage_verify_v2 import VerifyV2
 from vonage_voice import Voice
 
@@ -27,14 +28,15 @@
 
     def __init__(
         self, auth: Auth, http_client_options: Optional[HttpClientOptions] = None
     ):
         self._http_client = HttpClient(auth, http_client_options, __version__)
 
         self.messages = Messages(self._http_client)
+        self.number_insight = NumberInsight(self._http_client)
         self.number_insight_v2 = NumberInsightV2(self._http_client)
         self.sms = Sms(self._http_client)
         self.users = Users(self._http_client)
         self.verify = Verify(self._http_client)
         self.verify_v2 = VerifyV2(self._http_client)
         self.voice = Voice(self._http_client)
```

### Comparing `vonage-3.99.0a7/src/vonage.egg-info/PKG-INFO` & `vonage-3.99.0a8/src/vonage.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: vonage
-Version: 3.99.0a7
+Version: 3.99.0a8
 Summary: Python Server SDK for using Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-utils>=1.1.0
-Requires-Dist: vonage-http-client>=1.3.0
-Requires-Dist: vonage-messages>=1.1.0
-Requires-Dist: vonage-number-insight-v2>=0.1.0b0
-Requires-Dist: vonage-sms>=1.1.0
-Requires-Dist: vonage-users>=1.1.0
-Requires-Dist: vonage-verify>=1.1.0
-Requires-Dist: vonage-verify-v2>=1.1.0
-Requires-Dist: vonage-voice>=1.0.1
+Requires-Dist: vonage-utils>=1.1.1
+Requires-Dist: vonage-http-client>=1.3.1
+Requires-Dist: vonage-messages>=1.1.1
+Requires-Dist: vonage-number-insight>=1.0.0
+Requires-Dist: vonage-number-insight-v2>=0.1.1b0
+Requires-Dist: vonage-sms>=1.1.1
+Requires-Dist: vonage-users>=1.1.1
+Requires-Dist: vonage-verify>=1.1.1
+Requires-Dist: vonage-verify-v2>=1.1.1
+Requires-Dist: vonage-voice>=1.0.2
 
 # Vonage Python SDK
 
 The Vonage Python SDK Package `vonage` provides a streamlined interface for using Vonage APIs in Python projects. This package includes the `Vonage` class, which simplifies API interactions.
 
 The Vonage class in this package serves as the main entry point for using Vonage APIs. It abstracts away complexities with authentication, HTTP requests and more.
```

