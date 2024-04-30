# Comparing `tmp/edgegap_settings-1.0.1.tar.gz` & `tmp/edgegap_settings-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_settings-1.0.1.tar", max compression
+gzip compressed data, was "edgegap_settings-1.0.2.tar", max compression
```

## Comparing `edgegap_settings-1.0.1.tar` & `edgegap_settings-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1993 2024-04-29 18:21:35.347370 edgegap_settings-1.0.1/LICENSE
--rw-r--r--   0        0        0     2182 2024-04-29 18:21:35.347370 edgegap_settings-1.0.1/README.md
--rw-r--r--   0        0        0      358 2024-04-29 18:21:35.347370 edgegap_settings-1.0.1/edgegap_settings/__init__.py
--rw-r--r--   0        0        0      531 2024-04-29 18:21:35.347370 edgegap_settings-1.0.1/edgegap_settings/_apm.py
--rw-r--r--   0        0        0      872 2024-04-29 18:21:35.347370 edgegap_settings-1.0.1/edgegap_settings/_base.py
--rw-r--r--   0        0        0      119 2024-04-29 18:21:35.347370 edgegap_settings-1.0.1/edgegap_settings/_configuration.py
--rw-r--r--   0        0        0     3016 2024-04-29 18:21:35.347370 edgegap_settings-1.0.1/edgegap_settings/_factory.py
--rw-r--r--   0        0        0      963 2024-04-29 18:21:35.347370 edgegap_settings-1.0.1/edgegap_settings/_fields.py
--rw-r--r--   0        0        0      427 2024-04-29 18:21:35.347370 edgegap_settings-1.0.1/edgegap_settings/_logstash.py
--rw-r--r--   0        0        0      567 2024-04-29 18:21:50.419489 edgegap_settings-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 edgegap_settings-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 18:23:33.441036 edgegap_settings-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2182 2024-04-29 18:23:33.441036 edgegap_settings-1.0.2/README.md
+-rw-r--r--   0        0        0      358 2024-04-29 18:23:33.441036 edgegap_settings-1.0.2/edgegap_settings/__init__.py
+-rw-r--r--   0        0        0      531 2024-04-29 18:23:33.441036 edgegap_settings-1.0.2/edgegap_settings/_apm.py
+-rw-r--r--   0        0        0      872 2024-04-29 18:23:33.441036 edgegap_settings-1.0.2/edgegap_settings/_base.py
+-rw-r--r--   0        0        0      119 2024-04-29 18:23:33.441036 edgegap_settings-1.0.2/edgegap_settings/_configuration.py
+-rw-r--r--   0        0        0     3016 2024-04-29 18:23:33.441036 edgegap_settings-1.0.2/edgegap_settings/_factory.py
+-rw-r--r--   0        0        0      963 2024-04-29 18:23:33.441036 edgegap_settings-1.0.2/edgegap_settings/_fields.py
+-rw-r--r--   0        0        0      427 2024-04-29 18:23:33.441036 edgegap_settings-1.0.2/edgegap_settings/_logstash.py
+-rw-r--r--   0        0        0      567 2024-04-29 18:23:52.749128 edgegap_settings-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 edgegap_settings-1.0.2/PKG-INFO
```

### Comparing `edgegap_settings-1.0.1/LICENSE` & `edgegap_settings-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.0.1/README.md` & `edgegap_settings-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.0.1/edgegap_settings/_apm.py` & `edgegap_settings-1.0.2/edgegap_settings/_apm.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.0.1/edgegap_settings/_base.py` & `edgegap_settings-1.0.2/edgegap_settings/_base.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.0.1/edgegap_settings/_factory.py` & `edgegap_settings-1.0.2/edgegap_settings/_factory.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.0.1/edgegap_settings/_fields.py` & `edgegap_settings-1.0.2/edgegap_settings/_fields.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.0.1/pyproject.toml` & `edgegap_settings-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "edgegap-settings"
-version = "1.0.1"
+version = "1.0.2"
 description = "The Edgegap Settings library includes various tools and helpers for interacting with Explicit Settings Models. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic-settings = "^2.2.1"
 pydantic = "^2.7.1"
 python-dotenv = "^1.0.1"
-edgegap-logging = "^0.1.0"
-edgegap-consul = "^0.1.0"
+edgegap-logging = "^1.0.0"
+edgegap-consul = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `edgegap_settings-1.0.1/PKG-INFO` & `edgegap_settings-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: edgegap-settings
-Version: 1.0.1
+Version: 1.0.2
 Summary: The Edgegap Settings library includes various tools and helpers for interacting with Explicit Settings Models. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: edgegap-consul (>=0.1.0,<0.2.0)
-Requires-Dist: edgegap-logging (>=0.1.0,<0.2.0)
+Requires-Dist: edgegap-consul (>=1.0.0,<2.0.0)
+Requires-Dist: edgegap-logging (>=1.0.0,<2.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Edgegap Settings Library
```

