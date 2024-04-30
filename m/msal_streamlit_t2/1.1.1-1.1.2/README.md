# Comparing `tmp/msal_streamlit_t2-1.1.1.tar.gz` & `tmp/msal_streamlit_t2-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msal_streamlit_t2-1.1.1.tar", max compression
+gzip compressed data, was "msal_streamlit_t2-1.1.2.tar", max compression
```

## Comparing `msal_streamlit_t2-1.1.1.tar` & `msal_streamlit_t2-1.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1076 2024-04-26 21:37:22.650102 msal_streamlit_t2-1.1.1/LICENSE
--rw-r--r--   0        0        0     3830 2024-04-26 21:37:22.661333 msal_streamlit_t2-1.1.1/README.md
--rw-r--r--   0        0        0     1192 2024-04-29 12:58:41.131067 msal_streamlit_t2-1.1.1/msal_streamlit_t2/__init__.py
--rw-r--r--   0        0        0      372 2024-04-29 13:15:24.077422 msal_streamlit_t2-1.1.1/msal_streamlit_t2/frontend/dist/assets/index-297265e4.css
--rw-r--r--   0        0        0   622361 2024-04-29 13:15:24.077650 msal_streamlit_t2-1.1.1/msal_streamlit_t2/frontend/dist/assets/index-d9a76572.js
--rw-r--r--   0        0        0      399 2024-04-29 13:15:24.077391 msal_streamlit_t2-1.1.1/msal_streamlit_t2/frontend/dist/index.html
--rw-r--r--   0        0        0      934 2024-04-29 13:15:58.643086 msal_streamlit_t2-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 msal_streamlit_t2-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-26 21:37:22.650102 msal_streamlit_t2-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3873 2024-04-29 14:12:47.133744 msal_streamlit_t2-1.1.2/README.md
+-rw-r--r--   0        0        0     1192 2024-04-29 12:58:41.131067 msal_streamlit_t2-1.1.2/msal_streamlit_t2/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-29 13:15:24.077422 msal_streamlit_t2-1.1.2/msal_streamlit_t2/frontend/dist/assets/index-297265e4.css
+-rw-r--r--   0        0        0   622361 2024-04-29 13:15:24.077650 msal_streamlit_t2-1.1.2/msal_streamlit_t2/frontend/dist/assets/index-d9a76572.js
+-rw-r--r--   0        0        0      399 2024-04-29 13:15:24.077391 msal_streamlit_t2-1.1.2/msal_streamlit_t2/frontend/dist/index.html
+-rw-r--r--   0        0        0      934 2024-04-29 14:15:17.462909 msal_streamlit_t2-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4586 1970-01-01 00:00:00.000000 msal_streamlit_t2-1.1.2/PKG-INFO
```

### Comparing `msal_streamlit_t2-1.1.1/LICENSE` & `msal_streamlit_t2-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `msal_streamlit_t2-1.1.1/README.md` & `msal_streamlit_t2-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 
 Below is a sample Python snippet displaying how to apply the component. Visually, the component gives rise to a single button
 in the Streamlit Dashboard with a text that depends on whether an active login session exists. The `auth` and `cache`
 parameters are entirely equivalent to the properties mentioned in the [Github documentation](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-browser/docs/initialization.md).
 The `login_request` and `logout_request` parameters are covered [here](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-browser/docs/login-user.md).
 ```python
 import streamlit as st
-from msal_streamlit_authentication import msal_authentication
+from msal_streamlit_t2 import msal_authentication
 
 
 login_token = msal_authentication(
     auth={
         "clientId": "aaaaaaa-bbbb-cccc-dddd-eeeeeeeeeee",
         "authority": "https://login.microsoftonline.com/aaaaaaa-bbbb-cccc-dddd-eeeeeeeeeee",
         "redirectUri": "/",
         "postLogoutRedirectUri": "/"
     }, # Corresponds to the 'auth' configuration for an MSAL Instance
     cache={
-        "cacheLocation": "sessionStorage",
+        "cacheLocation": "sessionStorage", # or 'localStorage' for sharing sessions between tabs 
         "storeAuthStateInCookie": False
     }, # Corresponds to the 'cache' configuration for an MSAL Instance
     login_request={
         "scopes": ["aaaaaaa-bbbb-cccc-dddd-eeeeeeeeeee/.default"]
     }, # Optional
     logout_request={}, # Optional
     login_button_text="Login", # Optional, defaults to "Login"
```

### Comparing `msal_streamlit_t2-1.1.1/msal_streamlit_t2/__init__.py` & `msal_streamlit_t2-1.1.2/msal_streamlit_t2/__init__.py`

 * *Files identical despite different names*

### Comparing `msal_streamlit_t2-1.1.1/msal_streamlit_t2/frontend/dist/assets/index-d9a76572.js` & `msal_streamlit_t2-1.1.2/msal_streamlit_t2/frontend/dist/assets/index-d9a76572.js`

 * *Files identical despite different names*

### Comparing `msal_streamlit_t2-1.1.1/pyproject.toml` & `msal_streamlit_t2-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msal_streamlit_t2"
-version = "1.1.1"
+version = "1.1.2"
 description = "Streamlit Authentication library based on MSAL.JS"
 readme = "README.md"
 repository = "https://github.com/mstaal/msal_streamlit_t2"
 authors = ["Michael Staal-Olsen"]
 packages=[
     { include="msal_streamlit_t2" }
 ]
```

### Comparing `msal_streamlit_t2-1.1.1/PKG-INFO` & `msal_streamlit_t2-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal_streamlit_t2
-Version: 1.1.1
+Version: 1.1.2
 Summary: Streamlit Authentication library based on MSAL.JS
 Home-page: https://github.com/mstaal/msal_streamlit_t2
 Author: Michael Staal-Olsen
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -28,26 +28,26 @@
 
 Below is a sample Python snippet displaying how to apply the component. Visually, the component gives rise to a single button
 in the Streamlit Dashboard with a text that depends on whether an active login session exists. The `auth` and `cache`
 parameters are entirely equivalent to the properties mentioned in the [Github documentation](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-browser/docs/initialization.md).
 The `login_request` and `logout_request` parameters are covered [here](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-browser/docs/login-user.md).
 ```python
 import streamlit as st
-from msal_streamlit_authentication import msal_authentication
+from msal_streamlit_t2 import msal_authentication
 
 
 login_token = msal_authentication(
     auth={
         "clientId": "aaaaaaa-bbbb-cccc-dddd-eeeeeeeeeee",
         "authority": "https://login.microsoftonline.com/aaaaaaa-bbbb-cccc-dddd-eeeeeeeeeee",
         "redirectUri": "/",
         "postLogoutRedirectUri": "/"
     }, # Corresponds to the 'auth' configuration for an MSAL Instance
     cache={
-        "cacheLocation": "sessionStorage",
+        "cacheLocation": "sessionStorage", # or 'localStorage' for sharing sessions between tabs 
         "storeAuthStateInCookie": False
     }, # Corresponds to the 'cache' configuration for an MSAL Instance
     login_request={
         "scopes": ["aaaaaaa-bbbb-cccc-dddd-eeeeeeeeeee/.default"]
     }, # Optional
     logout_request={}, # Optional
     login_button_text="Login", # Optional, defaults to "Login"
```

