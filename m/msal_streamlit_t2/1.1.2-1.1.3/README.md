# Comparing `tmp/msal_streamlit_t2-1.1.2.tar.gz` & `tmp/msal_streamlit_t2-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msal_streamlit_t2-1.1.2.tar", max compression
+gzip compressed data, was "msal_streamlit_t2-1.1.3.tar", max compression
```

## Comparing `msal_streamlit_t2-1.1.2.tar` & `msal_streamlit_t2-1.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1076 2024-04-26 21:37:22.650102 msal_streamlit_t2-1.1.2/LICENSE
--rw-r--r--   0        0        0     3873 2024-04-29 14:12:47.133744 msal_streamlit_t2-1.1.2/README.md
--rw-r--r--   0        0        0     1192 2024-04-29 12:58:41.131067 msal_streamlit_t2-1.1.2/msal_streamlit_t2/__init__.py
--rw-r--r--   0        0        0      372 2024-04-29 13:15:24.077422 msal_streamlit_t2-1.1.2/msal_streamlit_t2/frontend/dist/assets/index-297265e4.css
--rw-r--r--   0        0        0   622361 2024-04-29 13:15:24.077650 msal_streamlit_t2-1.1.2/msal_streamlit_t2/frontend/dist/assets/index-d9a76572.js
--rw-r--r--   0        0        0      399 2024-04-29 13:15:24.077391 msal_streamlit_t2-1.1.2/msal_streamlit_t2/frontend/dist/index.html
--rw-r--r--   0        0        0      934 2024-04-29 14:15:17.462909 msal_streamlit_t2-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     4586 1970-01-01 00:00:00.000000 msal_streamlit_t2-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-26 21:37:22.650102 msal_streamlit_t2-1.1.3/LICENSE
+-rw-r--r--   0        0        0     4092 2024-04-30 10:33:45.328731 msal_streamlit_t2-1.1.3/README.md
+-rw-r--r--   0        0        0     1192 2024-04-29 12:58:41.131067 msal_streamlit_t2-1.1.3/msal_streamlit_t2/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-29 13:15:24.077422 msal_streamlit_t2-1.1.3/msal_streamlit_t2/frontend/dist/assets/index-297265e4.css
+-rw-r--r--   0        0        0   622361 2024-04-29 13:15:24.077650 msal_streamlit_t2-1.1.3/msal_streamlit_t2/frontend/dist/assets/index-d9a76572.js
+-rw-r--r--   0        0        0      399 2024-04-29 13:15:24.077391 msal_streamlit_t2-1.1.3/msal_streamlit_t2/frontend/dist/index.html
+-rw-r--r--   0        0        0      934 2024-04-30 10:34:05.419229 msal_streamlit_t2-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4805 1970-01-01 00:00:00.000000 msal_streamlit_t2-1.1.3/PKG-INFO
```

### Comparing `msal_streamlit_t2-1.1.2/LICENSE` & `msal_streamlit_t2-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `msal_streamlit_t2-1.1.2/README.md` & `msal_streamlit_t2-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,8 +44,9 @@
 
 The component currently expects for the user to go through a popup based login flow.
 Further flows may be supported at a later time. As discussed [here](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-browser/docs/initialization.md#optional-configure-authority),
 the `protocolMode` parameter in `auth` can be used to configure OIDC providers that differ from Azure AD.
 
 ## Inspiration
 Inspired by [official Streamlit template](https://github.com/streamlit/component-template), [this tutorial](https://youtu.be/htXgwEXwmNs) ([Github](https://github.com/andfanilo/streamlit-plotly-component-tutorial)) and the official [Streamlit NPM component-lib](https://github.com/streamlit/streamlit/tree/develop/component-lib).
+Speciall thanks to [msal_streamlit_authentication](https://github.com/mstaal/msal_streamlit_authentication), which is a project hasn't been updated for a long time. This library is basically an updated version of that.
```

### Comparing `msal_streamlit_t2-1.1.2/msal_streamlit_t2/__init__.py` & `msal_streamlit_t2-1.1.3/msal_streamlit_t2/__init__.py`

 * *Files identical despite different names*

### Comparing `msal_streamlit_t2-1.1.2/msal_streamlit_t2/frontend/dist/assets/index-d9a76572.js` & `msal_streamlit_t2-1.1.3/msal_streamlit_t2/frontend/dist/assets/index-d9a76572.js`

 * *Files identical despite different names*

### Comparing `msal_streamlit_t2-1.1.2/pyproject.toml` & `msal_streamlit_t2-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msal_streamlit_t2"
-version = "1.1.2"
+version = "1.1.3"
 description = "Streamlit Authentication library based on MSAL.JS"
 readme = "README.md"
 repository = "https://github.com/mstaal/msal_streamlit_t2"
 authors = ["Michael Staal-Olsen"]
 packages=[
     { include="msal_streamlit_t2" }
 ]
```

### Comparing `msal_streamlit_t2-1.1.2/PKG-INFO` & `msal_streamlit_t2-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal_streamlit_t2
-Version: 1.1.2
+Version: 1.1.3
 Summary: Streamlit Authentication library based on MSAL.JS
 Home-page: https://github.com/mstaal/msal_streamlit_t2
 Author: Michael Staal-Olsen
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -62,9 +62,10 @@
 
 The component currently expects for the user to go through a popup based login flow.
 Further flows may be supported at a later time. As discussed [here](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/lib/msal-browser/docs/initialization.md#optional-configure-authority),
 the `protocolMode` parameter in `auth` can be used to configure OIDC providers that differ from Azure AD.
 
 ## Inspiration
 Inspired by [official Streamlit template](https://github.com/streamlit/component-template), [this tutorial](https://youtu.be/htXgwEXwmNs) ([Github](https://github.com/andfanilo/streamlit-plotly-component-tutorial)) and the official [Streamlit NPM component-lib](https://github.com/streamlit/streamlit/tree/develop/component-lib).
+Speciall thanks to [msal_streamlit_authentication](https://github.com/mstaal/msal_streamlit_authentication), which is a project hasn't been updated for a long time. This library is basically an updated version of that.
```

