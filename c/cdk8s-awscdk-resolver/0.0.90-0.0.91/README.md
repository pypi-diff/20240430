# Comparing `tmp/cdk8s-awscdk-resolver-0.0.90.tar.gz` & `tmp/cdk8s-awscdk-resolver-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-awscdk-resolver-0.0.90.tar", last modified: Mon Apr 29 12:10:39 2024, max compression
+gzip compressed data, was "cdk8s-awscdk-resolver-0.0.91.tar", last modified: Tue Apr 30 06:14:24 2024, max compression
```

## Comparing `cdk8s-awscdk-resolver-0.0.90.tar` & `cdk8s-awscdk-resolver-0.0.91.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:10:39.871917 cdk8s-awscdk-resolver-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-29 12:10:26.000000 cdk8s-awscdk-resolver-0.0.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 12:10:26.000000 cdk8s-awscdk-resolver-0.0.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-29 12:10:39.871917 cdk8s-awscdk-resolver-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-29 12:10:26.000000 cdk8s-awscdk-resolver-0.0.90/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 12:10:26.000000 cdk8s-awscdk-resolver-0.0.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:10:39.871917 cdk8s-awscdk-resolver-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-29 12:10:26.000000 cdk8s-awscdk-resolver-0.0.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:10:39.867917 cdk8s-awscdk-resolver-0.0.90/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:10:39.867917 cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver/
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-29 12:10:26.000000 cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:10:39.867917 cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-29 12:10:26.000000 cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   979092 2024-04-29 12:10:26.000000 cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.90.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:10:26.000000 cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:10:39.867917 cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-29 12:10:39.000000 cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-29 12:10:39.000000 cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:10:39.000000 cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-29 12:10:39.000000 cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 12:10:39.000000 cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:14:24.621275 cdk8s-awscdk-resolver-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-30 06:14:14.000000 cdk8s-awscdk-resolver-0.0.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 06:14:14.000000 cdk8s-awscdk-resolver-0.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-30 06:14:24.621275 cdk8s-awscdk-resolver-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-30 06:14:14.000000 cdk8s-awscdk-resolver-0.0.91/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-30 06:14:14.000000 cdk8s-awscdk-resolver-0.0.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:14:24.621275 cdk8s-awscdk-resolver-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-30 06:14:14.000000 cdk8s-awscdk-resolver-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:14:24.617275 cdk8s-awscdk-resolver-0.0.91/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:14:24.617275 cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-30 06:14:14.000000 cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:14:24.617275 cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-30 06:14:14.000000 cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   899986 2024-04-30 06:14:14.000000 cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.91.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:14:14.000000 cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:14:24.617275 cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-30 06:14:24.000000 cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-30 06:14:24.000000 cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:14:24.000000 cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-30 06:14:24.000000 cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 06:14:24.000000 cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver.egg-info/top_level.txt
```

### Comparing `cdk8s-awscdk-resolver-0.0.90/LICENSE` & `cdk8s-awscdk-resolver-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.90/PKG-INFO` & `cdk8s-awscdk-resolver-0.0.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-awscdk-resolver
-Version: 0.0.90
+Version: 0.0.91
 Summary: @cdk8s/awscdk-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-awscdk-resolver-0.0.90/README.md` & `cdk8s-awscdk-resolver-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.90/setup.py` & `cdk8s-awscdk-resolver-0.0.91/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-awscdk-resolver",
-    "version": "0.0.90",
+    "version": "0.0.91",
     "description": "@cdk8s/awscdk-resolver",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk8s_awscdk_resolver",
         "cdk8s_awscdk_resolver._jsii"
     ],
     "package_data": {
         "cdk8s_awscdk_resolver._jsii": [
-            "awscdk-resolver@0.0.90.jsii.tgz"
+            "awscdk-resolver@0.0.91.jsii.tgz"
         ],
         "cdk8s_awscdk_resolver": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver/__init__.py` & `cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver/_jsii/__init__.py` & `cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import cdk8s._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdk8s/awscdk-resolver",
-    "0.0.90",
+    "0.0.91",
     __name__[0:-6],
-    "awscdk-resolver@0.0.90.jsii.tgz",
+    "awscdk-resolver@0.0.91.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk8s-awscdk-resolver-0.0.90/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO` & `cdk8s-awscdk-resolver-0.0.91/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-awscdk-resolver
-Version: 0.0.90
+Version: 0.0.91
 Summary: @cdk8s/awscdk-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

