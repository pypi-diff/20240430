# Comparing `tmp/pulumi_null-0.0.4a1714111001.tar.gz` & `tmp/pulumi_null-0.1.0a1714456711.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_null-0.0.4a1714111001.tar", last modified: Fri Apr 26 06:05:02 2024, max compression
+gzip compressed data, was "pulumi_null-0.1.0a1714456711.tar", last modified: Tue Apr 30 06:09:50 2024, max compression
```

## Comparing `pulumi_null-0.0.4a1714111001.tar` & `pulumi_null-0.1.0a1714456711.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:05:02.645071 pulumi_null-0.0.4a1714111001/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-26 06:05:02.645071 pulumi_null-0.0.4a1714111001/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-26 06:04:55.000000 pulumi_null-0.0.4a1714111001/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:05:02.645071 pulumi_null-0.0.4a1714111001/pulumi_null/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-26 06:04:55.000000 pulumi_null-0.0.4a1714111001/pulumi_null/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-26 06:04:55.000000 pulumi_null-0.0.4a1714111001/pulumi_null/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-04-26 06:04:55.000000 pulumi_null-0.0.4a1714111001/pulumi_null/get_data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-26 06:04:55.000000 pulumi_null-0.0.4a1714111001/pulumi_null/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 06:04:55.000000 pulumi_null-0.0.4a1714111001/pulumi_null/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 06:04:55.000000 pulumi_null-0.0.4a1714111001/pulumi_null/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-26 06:04:55.000000 pulumi_null-0.0.4a1714111001/pulumi_null/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:05:02.645071 pulumi_null-0.0.4a1714111001/pulumi_null.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-26 06:05:02.000000 pulumi_null-0.0.4a1714111001/pulumi_null.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-26 06:05:02.000000 pulumi_null-0.0.4a1714111001/pulumi_null.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:05:02.000000 pulumi_null-0.0.4a1714111001/pulumi_null.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 06:05:02.000000 pulumi_null-0.0.4a1714111001/pulumi_null.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 06:05:02.000000 pulumi_null-0.0.4a1714111001/pulumi_null.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-26 06:04:55.000000 pulumi_null-0.0.4a1714111001/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 06:05:02.645071 pulumi_null-0.0.4a1714111001/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:09:50.885767 pulumi_null-0.1.0a1714456711/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-30 06:09:50.885767 pulumi_null-0.1.0a1714456711/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-30 06:09:44.000000 pulumi_null-0.1.0a1714456711/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:09:50.885767 pulumi_null-0.1.0a1714456711/pulumi_null/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-30 06:09:44.000000 pulumi_null-0.1.0a1714456711/pulumi_null/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-30 06:09:44.000000 pulumi_null-0.1.0a1714456711/pulumi_null/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-04-30 06:09:44.000000 pulumi_null-0.1.0a1714456711/pulumi_null/get_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-30 06:09:44.000000 pulumi_null-0.1.0a1714456711/pulumi_null/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 06:09:44.000000 pulumi_null-0.1.0a1714456711/pulumi_null/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:09:44.000000 pulumi_null-0.1.0a1714456711/pulumi_null/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-30 06:09:44.000000 pulumi_null-0.1.0a1714456711/pulumi_null/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:09:50.885767 pulumi_null-0.1.0a1714456711/pulumi_null.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-30 06:09:50.000000 pulumi_null-0.1.0a1714456711/pulumi_null.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-30 06:09:50.000000 pulumi_null-0.1.0a1714456711/pulumi_null.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:09:50.000000 pulumi_null-0.1.0a1714456711/pulumi_null.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 06:09:50.000000 pulumi_null-0.1.0a1714456711/pulumi_null.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 06:09:50.000000 pulumi_null-0.1.0a1714456711/pulumi_null.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-30 06:09:44.000000 pulumi_null-0.1.0a1714456711/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:09:50.885767 pulumi_null-0.1.0a1714456711/setup.cfg
```

### Comparing `pulumi_null-0.0.4a1714111001/PKG-INFO` & `pulumi_null-0.1.0a1714456711/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_null
-Version: 0.0.4a1714111001
+Version: 0.1.0a1714456711
 Summary: A Pulumi package for creating and managing Null cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-null
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_null-0.0.4a1714111001/README.md` & `pulumi_null-0.1.0a1714456711/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.4a1714111001/pulumi_null/__init__.py` & `pulumi_null-0.1.0a1714456711/pulumi_null/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.4a1714111001/pulumi_null/_utilities.py` & `pulumi_null-0.1.0a1714456711/pulumi_null/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.4a1714111001/pulumi_null/get_data_source.py` & `pulumi_null-0.1.0a1714456711/pulumi_null/get_data_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.4a1714111001/pulumi_null/provider.py` & `pulumi_null-0.1.0a1714456711/pulumi_null/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.4a1714111001/pulumi_null/resource.py` & `pulumi_null-0.1.0a1714456711/pulumi_null/resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.4a1714111001/pulumi_null.egg-info/PKG-INFO` & `pulumi_null-0.1.0a1714456711/pulumi_null.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_null
-Version: 0.0.4a1714111001
+Version: 0.1.0a1714456711
 Summary: A Pulumi package for creating and managing Null cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-null
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_null-0.0.4a1714111001/pyproject.toml` & `pulumi_null-0.1.0a1714456711/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_null"
   description = "A Pulumi package for creating and managing Null cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.4a1714111001"
+  version = "0.1.0a1714456711"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com/"
     Repository = "https://github.com/pulumi/pulumi-null"
 
 [build-system]
```

