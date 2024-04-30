# Comparing `tmp/pulumi_kong-4.6.0a1714110449.tar.gz` & `tmp/pulumi_kong-4.6.0a1714455955.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kong-4.6.0a1714110449.tar", last modified: Fri Apr 26 05:50:59 2024, max compression
+gzip compressed data, was "pulumi_kong-4.6.0a1714455955.tar", last modified: Tue Apr 30 05:51:52 2024, max compression
```

## Comparing `pulumi_kong-4.6.0a1714110449.tar` & `pulumi_kong-4.6.0a1714455955.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:50:59.114412 pulumi_kong-4.6.0a1714110449/
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-26 05:50:59.114412 pulumi_kong-4.6.0a1714110449/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:50:59.110412 pulumi_kong-4.6.0a1714110449/pulumi_kong/
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16572 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    13605 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:50:59.114412 pulumi_kong-4.6.0a1714110449/pulumi_kong/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/consumer_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/consumer_basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    18776 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/consumer_jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/consumer_key_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    22596 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/consumer_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25552 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13775 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    54556 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/route.py
--rw-r--r--   0 runner    (1001) docker     (127)    36145 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/target.py
--rw-r--r--   0 runner    (1001) docker     (127)    73112 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong/upstream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:50:59.114412 pulumi_kong-4.6.0a1714110449/pulumi_kong.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-26 05:50:59.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-26 05:50:59.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 05:50:59.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 05:50:59.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 05:50:59.000000 pulumi_kong-4.6.0a1714110449/pulumi_kong.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-26 05:50:52.000000 pulumi_kong-4.6.0a1714110449/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 05:50:59.114412 pulumi_kong-4.6.0a1714110449/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:51:52.616174 pulumi_kong-4.6.0a1714455955/
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-30 05:51:52.616174 pulumi_kong-4.6.0a1714455955/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:51:52.612173 pulumi_kong-4.6.0a1714455955/pulumi_kong/
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16572 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13605 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:51:52.616174 pulumi_kong-4.6.0a1714455955/pulumi_kong/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/consumer_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/consumer_basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18776 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/consumer_jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/consumer_key_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22596 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/consumer_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25552 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13775 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54556 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36145 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73112 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong/upstream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:51:52.616174 pulumi_kong-4.6.0a1714455955/pulumi_kong.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-30 05:51:52.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-30 05:51:52.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 05:51:52.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 05:51:52.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 05:51:52.000000 pulumi_kong-4.6.0a1714455955/pulumi_kong.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-30 05:51:46.000000 pulumi_kong-4.6.0a1714455955/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 05:51:52.616174 pulumi_kong-4.6.0a1714455955/setup.cfg
```

### Comparing `pulumi_kong-4.6.0a1714110449/PKG-INFO` & `pulumi_kong-4.6.0a1714455955/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kong
-Version: 4.6.0a1714110449
+Version: 4.6.0a1714455955
 Summary: A Pulumi package for creating and managing Kong resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kong
 Keywords: pulumi,kong
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kong-4.6.0a1714110449/README.md` & `pulumi_kong-4.6.0a1714455955/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/__init__.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/_inputs.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/_utilities.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/certificate.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/config/__init__.pyi` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/config/vars.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/consumer.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/consumer.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/consumer_acl.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/consumer_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/consumer_basic_auth.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/consumer_basic_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/consumer_jwt_auth.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/consumer_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/consumer_key_auth.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/consumer_key_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/consumer_oauth2.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/consumer_oauth2.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/outputs.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/plugin.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/provider.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/route.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/route.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/service.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/target.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/target.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong/upstream.py` & `pulumi_kong-4.6.0a1714455955/pulumi_kong/upstream.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong.egg-info/PKG-INFO` & `pulumi_kong-4.6.0a1714455955/pulumi_kong.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kong
-Version: 4.6.0a1714110449
+Version: 4.6.0a1714455955
 Summary: A Pulumi package for creating and managing Kong resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kong
 Keywords: pulumi,kong
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kong-4.6.0a1714110449/pulumi_kong.egg-info/SOURCES.txt` & `pulumi_kong-4.6.0a1714455955/pulumi_kong.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1714110449/pyproject.toml` & `pulumi_kong-4.6.0a1714455955/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kong"
   description = "A Pulumi package for creating and managing Kong resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "kong"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "4.6.0a1714110449"
+  version = "4.6.0a1714455955"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-kong"
 
 [build-system]
```

