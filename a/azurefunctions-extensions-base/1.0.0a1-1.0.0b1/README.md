# Comparing `tmp/azurefunctions-extensions-base-1.0.0a1.tar.gz` & `tmp/azurefunctions_extensions_base-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azurefunctions-extensions-base-1.0.0a1.tar", last modified: Wed Apr 10 19:37:59 2024, max compression
+gzip compressed data, was "azurefunctions_extensions_base-1.0.0b1.tar", last modified: Tue Apr 30 18:51:19 2024, max compression
```

## Comparing `azurefunctions-extensions-base-1.0.0a1.tar` & `azurefunctions_extensions_base-1.0.0b1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 19:37:59.963938 azurefunctions-extensions-base-1.0.0a1/
--rw-rw-rw-   0        0        0     1093 2024-04-10 19:22:55.000000 azurefunctions-extensions-base-1.0.0a1/LICENSE
--rw-rw-rw-   0        0        0       91 2024-04-10 19:22:55.000000 azurefunctions-extensions-base-1.0.0a1/MANIFEST.in
--rw-rw-rw-   0        0        0     1497 2024-04-10 19:37:59.958423 azurefunctions-extensions-base-1.0.0a1/PKG-INFO
--rw-rw-rw-   0        0        0      326 2024-04-10 19:31:47.000000 azurefunctions-extensions-base-1.0.0a1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 19:37:59.854150 azurefunctions-extensions-base-1.0.0a1/azurefunctions/
-drwxrwxrwx   0        0        0        0 2024-04-10 19:37:59.854468 azurefunctions-extensions-base-1.0.0a1/azurefunctions/extensions/
-drwxrwxrwx   0        0        0        0 2024-04-10 19:37:59.885357 azurefunctions-extensions-base-1.0.0a1/azurefunctions/extensions/base/
--rw-rw-rw-   0        0        0      856 2024-04-10 19:37:51.000000 azurefunctions-extensions-base-1.0.0a1/azurefunctions/extensions/base/__init__.py
--rw-rw-rw-   0        0        0     5754 2024-04-10 19:25:13.000000 azurefunctions-extensions-base-1.0.0a1/azurefunctions/extensions/base/meta.py
--rw-rw-rw-   0        0        0      296 2024-04-10 19:22:55.000000 azurefunctions-extensions-base-1.0.0a1/azurefunctions/extensions/base/sdkType.py
--rw-rw-rw-   0        0        0     9063 2024-04-10 19:22:55.000000 azurefunctions-extensions-base-1.0.0a1/azurefunctions/extensions/base/utils.py
--rw-rw-rw-   0        0        0     5010 2024-04-10 19:22:55.000000 azurefunctions-extensions-base-1.0.0a1/azurefunctions/extensions/base/web.py
-drwxrwxrwx   0        0        0        0 2024-04-10 19:37:59.954609 azurefunctions-extensions-base-1.0.0a1/azurefunctions_extensions_base.egg-info/
--rw-rw-rw-   0        0        0     1497 2024-04-10 19:37:59.000000 azurefunctions-extensions-base-1.0.0a1/azurefunctions_extensions_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      613 2024-04-10 19:37:59.000000 azurefunctions-extensions-base-1.0.0a1/azurefunctions_extensions_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 19:37:59.000000 azurefunctions-extensions-base-1.0.0a1/azurefunctions_extensions_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-10 19:37:59.000000 azurefunctions-extensions-base-1.0.0a1/azurefunctions_extensions_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-10 19:37:59.000000 azurefunctions-extensions-base-1.0.0a1/azurefunctions_extensions_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1395 2024-04-10 19:25:13.000000 azurefunctions-extensions-base-1.0.0a1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 19:37:59.965259 azurefunctions-extensions-base-1.0.0a1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 19:37:59.951483 azurefunctions-extensions-base-1.0.0a1/tests/
--rw-rw-rw-   0        0        0      519 2024-04-10 19:22:55.000000 azurefunctions-extensions-base-1.0.0a1/tests/__init__.py
--rw-rw-rw-   0        0        0    11526 2024-04-10 19:25:13.000000 azurefunctions-extensions-base-1.0.0a1/tests/test_meta.py
--rw-rw-rw-   0        0        0      656 2024-04-10 19:25:13.000000 azurefunctions-extensions-base-1.0.0a1/tests/test_sdk_type.py
--rw-rw-rw-   0        0        0    12756 2024-04-10 19:25:13.000000 azurefunctions-extensions-base-1.0.0a1/tests/test_utils.py
--rw-rw-rw-   0        0        0    14624 2024-04-10 19:25:13.000000 azurefunctions-extensions-base-1.0.0a1/tests/test_web.py
+drwxrwxrwx   0        0        0        0 2024-04-30 18:51:19.280423 azurefunctions_extensions_base-1.0.0b1/
+-rw-rw-rw-   0        0        0     1093 2024-04-11 00:07:36.000000 azurefunctions_extensions_base-1.0.0b1/LICENSE
+-rw-rw-rw-   0        0        0       91 2024-04-11 00:07:36.000000 azurefunctions_extensions_base-1.0.0b1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1512 2024-04-30 18:51:19.278414 azurefunctions_extensions_base-1.0.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2024-04-30 18:50:12.000000 azurefunctions_extensions_base-1.0.0b1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 18:51:19.108026 azurefunctions_extensions_base-1.0.0b1/azurefunctions/
+drwxrwxrwx   0        0        0        0 2024-04-30 18:51:19.108026 azurefunctions_extensions_base-1.0.0b1/azurefunctions/extensions/
+drwxrwxrwx   0        0        0        0 2024-04-30 18:51:19.183079 azurefunctions_extensions_base-1.0.0b1/azurefunctions/extensions/base/
+-rw-rw-rw-   0        0        0      856 2024-04-30 18:50:12.000000 azurefunctions_extensions_base-1.0.0b1/azurefunctions/extensions/base/__init__.py
+-rw-rw-rw-   0        0        0     5754 2024-04-11 00:07:36.000000 azurefunctions_extensions_base-1.0.0b1/azurefunctions/extensions/base/meta.py
+-rw-rw-rw-   0        0        0      296 2024-04-11 00:07:36.000000 azurefunctions_extensions_base-1.0.0b1/azurefunctions/extensions/base/sdkType.py
+-rw-rw-rw-   0        0        0     9063 2024-04-11 00:07:36.000000 azurefunctions_extensions_base-1.0.0b1/azurefunctions/extensions/base/utils.py
+-rw-rw-rw-   0        0        0     5010 2024-04-11 00:07:36.000000 azurefunctions_extensions_base-1.0.0b1/azurefunctions/extensions/base/web.py
+drwxrwxrwx   0        0        0        0 2024-04-30 18:51:19.276801 azurefunctions_extensions_base-1.0.0b1/azurefunctions_extensions_base.egg-info/
+-rw-rw-rw-   0        0        0     1512 2024-04-30 18:51:19.000000 azurefunctions_extensions_base-1.0.0b1/azurefunctions_extensions_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      613 2024-04-30 18:51:19.000000 azurefunctions_extensions_base-1.0.0b1/azurefunctions_extensions_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 18:51:19.000000 azurefunctions_extensions_base-1.0.0b1/azurefunctions_extensions_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-30 18:51:19.000000 azurefunctions_extensions_base-1.0.0b1/azurefunctions_extensions_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-30 18:51:19.000000 azurefunctions_extensions_base-1.0.0b1/azurefunctions_extensions_base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1395 2024-04-11 00:07:36.000000 azurefunctions_extensions_base-1.0.0b1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 18:51:19.281422 azurefunctions_extensions_base-1.0.0b1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 18:51:19.274802 azurefunctions_extensions_base-1.0.0b1/tests/
+-rw-rw-rw-   0        0        0      519 2024-04-11 00:07:36.000000 azurefunctions_extensions_base-1.0.0b1/tests/__init__.py
+-rw-rw-rw-   0        0        0    11526 2024-04-11 00:07:36.000000 azurefunctions_extensions_base-1.0.0b1/tests/test_meta.py
+-rw-rw-rw-   0        0        0      656 2024-04-11 00:07:36.000000 azurefunctions_extensions_base-1.0.0b1/tests/test_sdk_type.py
+-rw-rw-rw-   0        0        0    12756 2024-04-11 00:07:36.000000 azurefunctions_extensions_base-1.0.0b1/tests/test_utils.py
+-rw-rw-rw-   0        0        0    14624 2024-04-11 00:07:36.000000 azurefunctions_extensions_base-1.0.0b1/tests/test_web.py
```

### Comparing `azurefunctions-extensions-base-1.0.0a1/LICENSE` & `azurefunctions_extensions_base-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-base-1.0.0a1/PKG-INFO` & `azurefunctions_extensions_base-1.0.0b1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azurefunctions-extensions-base
-Version: 1.0.0a1
+Version: 1.0.0b1
 Summary: Base Python worker extension for Azure Functions.
 Author-email: "Azure Functions team at Microsoft Corp." <azurefunctions@microsoft.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -22,12 +22,12 @@
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-instafail; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
-# Azure Functions Extension Base library for Python
+# Azure Functions Extensions Base library for Python
 This is the base library for allowing Python Function Apps to recognize and bind to SDk-types and HttpV2-types. It is not to be used directly.
 Instead, please reference one of the extending packages:
-* azurefunctions-extensions-blob
-* azurefunctions-extensions-fastapi
+* azurefunctions-extensions-bindings-blob
+* azurefunctions-extensions-http-fastapi
```

### Comparing `azurefunctions-extensions-base-1.0.0a1/azurefunctions/extensions/base/__init__.py` & `azurefunctions_extensions_base-1.0.0b1/azurefunctions/extensions/base/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,8 +35,8 @@
     "HttpV2FeatureChecker",
     "ResponseLabels",
     "WebServer",
     "WebApp",
     "RequestSynchronizer",
 ]
 
-__version__ = "1.0.0a1"
+__version__ = "1.0.0b1"
```

### Comparing `azurefunctions-extensions-base-1.0.0a1/azurefunctions/extensions/base/meta.py` & `azurefunctions_extensions_base-1.0.0b1/azurefunctions/extensions/base/meta.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-base-1.0.0a1/azurefunctions/extensions/base/utils.py` & `azurefunctions_extensions_base-1.0.0b1/azurefunctions/extensions/base/utils.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-base-1.0.0a1/azurefunctions/extensions/base/web.py` & `azurefunctions_extensions_base-1.0.0b1/azurefunctions/extensions/base/web.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-base-1.0.0a1/azurefunctions_extensions_base.egg-info/PKG-INFO` & `azurefunctions_extensions_base-1.0.0b1/azurefunctions_extensions_base.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azurefunctions-extensions-base
-Version: 1.0.0a1
+Version: 1.0.0b1
 Summary: Base Python worker extension for Azure Functions.
 Author-email: "Azure Functions team at Microsoft Corp." <azurefunctions@microsoft.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -22,12 +22,12 @@
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-instafail; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
-# Azure Functions Extension Base library for Python
+# Azure Functions Extensions Base library for Python
 This is the base library for allowing Python Function Apps to recognize and bind to SDk-types and HttpV2-types. It is not to be used directly.
 Instead, please reference one of the extending packages:
-* azurefunctions-extensions-blob
-* azurefunctions-extensions-fastapi
+* azurefunctions-extensions-bindings-blob
+* azurefunctions-extensions-http-fastapi
```

### Comparing `azurefunctions-extensions-base-1.0.0a1/azurefunctions_extensions_base.egg-info/SOURCES.txt` & `azurefunctions_extensions_base-1.0.0b1/azurefunctions_extensions_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-base-1.0.0a1/pyproject.toml` & `azurefunctions_extensions_base-1.0.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-base-1.0.0a1/tests/__init__.py` & `azurefunctions_extensions_base-1.0.0b1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-base-1.0.0a1/tests/test_meta.py` & `azurefunctions_extensions_base-1.0.0b1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-base-1.0.0a1/tests/test_sdk_type.py` & `azurefunctions_extensions_base-1.0.0b1/tests/test_sdk_type.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-base-1.0.0a1/tests/test_utils.py` & `azurefunctions_extensions_base-1.0.0b1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-base-1.0.0a1/tests/test_web.py` & `azurefunctions_extensions_base-1.0.0b1/tests/test_web.py`

 * *Files identical despite different names*

