# Comparing `tmp/pynpdc-0.13.0.tar.gz` & `tmp/pynpdc-0.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynpdc-0.13.0.tar", last modified: Mon Apr 29 05:55:08 2024, max compression
+gzip compressed data, was "pynpdc-0.13.1.tar", last modified: Tue Apr 30 10:57:59 2024, max compression
```

## Comparing `pynpdc-0.13.0.tar` & `pynpdc-0.13.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-29 05:55:08.297320 pynpdc-0.13.0/
--rw-r--r--   0 olaf      (1000) olaf      (1000)     7415 2024-04-29 05:55:08.297320 pynpdc-0.13.0/PKG-INFO
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     6577 2024-04-11 12:20:53.000000 pynpdc-0.13.0/README.md
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-29 05:55:08.297320 pynpdc-0.13.0/pynpdc/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      911 2024-04-26 08:39:05.000000 pynpdc-0.13.0/pynpdc/__init__.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)    10261 2024-04-11 09:18:52.000000 pynpdc-0.13.0/pynpdc/auth.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)    39423 2024-04-26 08:29:11.000000 pynpdc-0.13.0/pynpdc/dataset.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      443 2024-04-11 09:18:52.000000 pynpdc-0.13.0/pynpdc/exception.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        0 2024-04-26 08:07:44.000000 pynpdc-0.13.0/pynpdc/py.typed
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     1504 2024-04-11 09:18:52.000000 pynpdc-0.13.0/pynpdc/types.py
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-29 05:55:08.297320 pynpdc-0.13.0/pynpdc.egg-info/
--rw-r--r--   0 olaf      (1000) olaf      (1000)     7415 2024-04-29 05:55:08.000000 pynpdc-0.13.0/pynpdc.egg-info/PKG-INFO
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      318 2024-04-29 05:55:08.000000 pynpdc-0.13.0/pynpdc.egg-info/SOURCES.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2024-04-29 05:55:08.000000 pynpdc-0.13.0/pynpdc.egg-info/dependency_links.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)       54 2024-04-29 05:55:08.000000 pynpdc-0.13.0/pynpdc.egg-info/requires.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        7 2024-04-29 05:55:08.000000 pynpdc-0.13.0/pynpdc.egg-info/top_level.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      932 2024-04-29 05:51:50.000000 pynpdc-0.13.0/pyproject.toml
--rw-rw-r--   0 olaf      (1000) olaf      (1000)       38 2024-04-29 05:55:08.297320 pynpdc-0.13.0/setup.cfg
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-29 05:55:08.297320 pynpdc-0.13.0/tests/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     7253 2024-04-11 09:18:52.000000 pynpdc-0.13.0/tests/test_auth.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)    27966 2024-04-26 11:20:41.000000 pynpdc-0.13.0/tests/test_dataset.py
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-30 10:57:59.805313 pynpdc-0.13.1/
+-rw-r--r--   0 olaf      (1000) olaf      (1000)     7415 2024-04-30 10:57:59.805313 pynpdc-0.13.1/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     6577 2024-04-11 12:20:53.000000 pynpdc-0.13.1/README.md
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-30 10:57:59.805313 pynpdc-0.13.1/pynpdc/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      911 2024-04-26 08:39:05.000000 pynpdc-0.13.1/pynpdc/__init__.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)    10243 2024-04-30 10:50:07.000000 pynpdc-0.13.1/pynpdc/auth.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)    39423 2024-04-26 08:29:11.000000 pynpdc-0.13.1/pynpdc/dataset.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      443 2024-04-11 09:18:52.000000 pynpdc-0.13.1/pynpdc/exception.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        0 2024-04-26 08:07:44.000000 pynpdc-0.13.1/pynpdc/py.typed
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     1504 2024-04-11 09:18:52.000000 pynpdc-0.13.1/pynpdc/types.py
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-30 10:57:59.805313 pynpdc-0.13.1/pynpdc.egg-info/
+-rw-r--r--   0 olaf      (1000) olaf      (1000)     7415 2024-04-30 10:57:59.000000 pynpdc-0.13.1/pynpdc.egg-info/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      318 2024-04-30 10:57:59.000000 pynpdc-0.13.1/pynpdc.egg-info/SOURCES.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2024-04-30 10:57:59.000000 pynpdc-0.13.1/pynpdc.egg-info/dependency_links.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)       54 2024-04-30 10:57:59.000000 pynpdc-0.13.1/pynpdc.egg-info/requires.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        7 2024-04-30 10:57:59.000000 pynpdc-0.13.1/pynpdc.egg-info/top_level.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      932 2024-04-30 10:55:29.000000 pynpdc-0.13.1/pyproject.toml
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)       38 2024-04-30 10:57:59.805313 pynpdc-0.13.1/setup.cfg
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-30 10:57:59.805313 pynpdc-0.13.1/tests/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     7253 2024-04-11 09:18:52.000000 pynpdc-0.13.1/tests/test_auth.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)    27966 2024-04-26 11:20:41.000000 pynpdc-0.13.1/tests/test_dataset.py
```

### Comparing `pynpdc-0.13.0/PKG-INFO` & `pynpdc-0.13.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynpdc
-Version: 0.13.0
+Version: 0.13.1
 Summary: Python lib to interact with the NPDC stack
 Author-email: Olaf Schneider <olaf.schneider@npolar.no>, Mikhail Itkin <mikhail.itkin@npolar.no>
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pynpdc-0.13.0/README.md` & `pynpdc-0.13.1/README.md`

 * *Files identical despite different names*

### Comparing `pynpdc-0.13.0/pynpdc/__init__.py` & `pynpdc-0.13.1/pynpdc/__init__.py`

 * *Files identical despite different names*

### Comparing `pynpdc-0.13.0/pynpdc/auth.py` & `pynpdc-0.13.1/pynpdc/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,22 +92,22 @@
         raw (AccountWithTokenAPIResponse): The API response data parsed from JSON
         client (AuthClient | None) The client for the auth module
     """
 
     raw: AccountWithTokenAPIResponse
 
     @property
-    def token(self) -> str | None:
+    def token(self) -> str:
         """
         Retrieve the login token.
 
         Returns:
-            str | None: the login token
+            str: the login token
         """
-        return self.raw.get("token")
+        return self.raw["token"]
 
     @token.setter
     def token(self, token: str) -> None:
         """
         Replace token value
 
         Args:
```

### Comparing `pynpdc-0.13.0/pynpdc/dataset.py` & `pynpdc-0.13.1/pynpdc/dataset.py`

 * *Files identical despite different names*

### Comparing `pynpdc-0.13.0/pynpdc/types.py` & `pynpdc-0.13.1/pynpdc/types.py`

 * *Files identical despite different names*

### Comparing `pynpdc-0.13.0/pynpdc.egg-info/PKG-INFO` & `pynpdc-0.13.1/pynpdc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynpdc
-Version: 0.13.0
+Version: 0.13.1
 Summary: Python lib to interact with the NPDC stack
 Author-email: Olaf Schneider <olaf.schneider@npolar.no>, Mikhail Itkin <mikhail.itkin@npolar.no>
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pynpdc-0.13.0/pyproject.toml` & `pynpdc-0.13.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pynpdc"
-version = "0.13.0"
+version = "0.13.1"
 dependencies = [
     "requests",
     "requests-toolbelt",
     "typing-extensions",
     "werkzeug",
 ]
 requires-python = ">= 3.8"
```

### Comparing `pynpdc-0.13.0/tests/test_auth.py` & `pynpdc-0.13.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pynpdc-0.13.0/tests/test_dataset.py` & `pynpdc-0.13.1/tests/test_dataset.py`

 * *Files identical despite different names*

