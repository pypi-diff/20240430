# Comparing `tmp/remixqq_python_sdk-20240430.tar.gz` & `tmp/remixqq_python_sdk-202404300043.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remixqq_python_sdk-20240430.tar", last modified: Tue Apr 30 16:21:02 2024, max compression
+gzip compressed data, was "remixqq_python_sdk-202404300043.tar", last modified: Tue Apr 30 16:44:49 2024, max compression
```

## Comparing `remixqq_python_sdk-20240430.tar` & `remixqq_python_sdk-202404300043.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 16:21:02.619431 remixqq_python_sdk-20240430/
--rw-rw-rw-   0        0        0     1090 2024-04-10 11:58:02.000000 remixqq_python_sdk-20240430/LICENSE
--rw-rw-rw-   0        0        0     2362 2024-04-30 16:21:02.618432 remixqq_python_sdk-20240430/PKG-INFO
--rw-rw-rw-   0        0        0     1892 2024-04-30 15:37:51.000000 remixqq_python_sdk-20240430/README.md
--rw-rw-rw-   0        0        0      736 2024-04-30 16:20:57.000000 remixqq_python_sdk-20240430/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 16:21:02.619431 remixqq_python_sdk-20240430/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 16:21:02.613431 remixqq_python_sdk-20240430/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 16:21:02.618432 remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/
--rw-rw-rw-   0        0        0     2362 2024-04-30 16:21:02.000000 remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2024-04-30 16:21:02.000000 remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 16:21:02.000000 remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-30 16:21:02.000000 remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-30 16:21:02.000000 remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 16:21:02.617431 remixqq_python_sdk-20240430/src/remixqq_python_sdk/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:16:24.000000 remixqq_python_sdk-20240430/src/remixqq_python_sdk/__init__.py
--rw-rw-rw-   0        0        0    12210 2024-04-30 14:48:27.000000 remixqq_python_sdk-20240430/src/remixqq_python_sdk/app.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:21:02.617431 remixqq_python_sdk-20240430/tests/
--rw-rw-rw-   0        0        0      162 2024-04-10 13:30:43.000000 remixqq_python_sdk-20240430/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:44:49.977484 remixqq_python_sdk-202404300043/
+-rw-rw-rw-   0        0        0     1090 2024-04-10 11:58:02.000000 remixqq_python_sdk-202404300043/LICENSE
+-rw-rw-rw-   0        0        0     2366 2024-04-30 16:44:49.976485 remixqq_python_sdk-202404300043/PKG-INFO
+-rw-rw-rw-   0        0        0     1892 2024-04-30 15:37:51.000000 remixqq_python_sdk-202404300043/README.md
+-rw-rw-rw-   0        0        0      740 2024-04-30 16:44:20.000000 remixqq_python_sdk-202404300043/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 16:44:49.977484 remixqq_python_sdk-202404300043/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 16:44:49.968483 remixqq_python_sdk-202404300043/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 16:44:49.976485 remixqq_python_sdk-202404300043/src/RemixQQ_Python_SDK.egg-info/
+-rw-rw-rw-   0        0        0     2366 2024-04-30 16:44:49.000000 remixqq_python_sdk-202404300043/src/RemixQQ_Python_SDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2024-04-30 16:44:49.000000 remixqq_python_sdk-202404300043/src/RemixQQ_Python_SDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 16:44:49.000000 remixqq_python_sdk-202404300043/src/RemixQQ_Python_SDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-30 16:44:49.000000 remixqq_python_sdk-202404300043/src/RemixQQ_Python_SDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-30 16:44:49.000000 remixqq_python_sdk-202404300043/src/RemixQQ_Python_SDK.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 16:44:49.975485 remixqq_python_sdk-202404300043/src/remixqq_python_sdk/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:16:24.000000 remixqq_python_sdk-202404300043/src/remixqq_python_sdk/__init__.py
+-rw-rw-rw-   0        0        0    12210 2024-04-30 14:48:27.000000 remixqq_python_sdk-202404300043/src/remixqq_python_sdk/app.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:44:49.975485 remixqq_python_sdk-202404300043/tests/
+-rw-rw-rw-   0        0        0      162 2024-04-10 13:30:43.000000 remixqq_python_sdk-202404300043/tests/test.py
```

### Comparing `remixqq_python_sdk-20240430/LICENSE` & `remixqq_python_sdk-202404300043/LICENSE`

 * *Files identical despite different names*

### Comparing `remixqq_python_sdk-20240430/PKG-INFO` & `remixqq_python_sdk-202404300043/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RemixQQ_Python_SDK
-Version: 20240430
+Version: 202404300043
 Summary: A python SDK for RemixQQ connected by httpapi
 Author-email: 404_NOT_FOUND <1127738407@qq.com>
 License: MIT
 Project-URL: Homepage, https://github.com/willyautoman/RemixQQ_Python_SDK
 Project-URL: Bug Tracker, https://github.com/willyautoman/RemixQQ_Python_SDK/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `remixqq_python_sdk-20240430/README.md` & `remixqq_python_sdk-202404300043/README.md`

 * *Files identical despite different names*

### Comparing `remixqq_python_sdk-20240430/pyproject.toml` & `remixqq_python_sdk-202404300043/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "RemixQQ_Python_SDK"
-version = "20240430"
+version = "202404300043"
 description = "A python SDK for RemixQQ connected by httpapi"
 authors = [
     {name = "404_NOT_FOUND", email = "1127738407@qq.com"},
 ]
 dependencies = [
     "requests>=2.31.0",
 ]
```

### Comparing `remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/PKG-INFO` & `remixqq_python_sdk-202404300043/src/RemixQQ_Python_SDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RemixQQ_Python_SDK
-Version: 20240430
+Version: 202404300043
 Summary: A python SDK for RemixQQ connected by httpapi
 Author-email: 404_NOT_FOUND <1127738407@qq.com>
 License: MIT
 Project-URL: Homepage, https://github.com/willyautoman/RemixQQ_Python_SDK
 Project-URL: Bug Tracker, https://github.com/willyautoman/RemixQQ_Python_SDK/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `remixqq_python_sdk-20240430/src/remixqq_python_sdk/app.py` & `remixqq_python_sdk-202404300043/src/remixqq_python_sdk/app.py`

 * *Files identical despite different names*

