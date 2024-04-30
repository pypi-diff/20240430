# Comparing `tmp/layerborn.cdk-git-tagger-0.0.8.tar.gz` & `tmp/layerborn.cdk-git-tagger-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layerborn.cdk-git-tagger-0.0.8.tar", last modified: Sun Jan 28 02:51:10 2024, max compression
+gzip compressed data, was "layerborn.cdk-git-tagger-0.0.9.tar", last modified: Mon Jan 29 16:36:02 2024, max compression
```

## Comparing `layerborn.cdk-git-tagger-0.0.8.tar` & `layerborn.cdk-git-tagger-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:51:10.835072 layerborn.cdk-git-tagger-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-28 02:50:55.000000 layerborn.cdk-git-tagger-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-28 02:50:55.000000 layerborn.cdk-git-tagger-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-01-28 02:51:10.835072 layerborn.cdk-git-tagger-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-01-28 02:50:55.000000 layerborn.cdk-git-tagger-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-28 02:50:55.000000 layerborn.cdk-git-tagger-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 02:51:10.835072 layerborn.cdk-git-tagger-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-01-28 02:50:55.000000 layerborn.cdk-git-tagger-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:51:10.835072 layerborn.cdk-git-tagger-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:51:10.835072 layerborn.cdk-git-tagger-0.0.8/src/layerborn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:51:10.835072 layerborn.cdk-git-tagger-0.0.8/src/layerborn/cdk_git_tagger/
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-01-28 02:50:55.000000 layerborn.cdk-git-tagger-0.0.8/src/layerborn/cdk_git_tagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:51:10.835072 layerborn.cdk-git-tagger-0.0.8/src/layerborn/cdk_git_tagger/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-01-28 02:50:55.000000 layerborn.cdk-git-tagger-0.0.8/src/layerborn/cdk_git_tagger/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20463 2024-01-28 02:50:55.000000 layerborn.cdk-git-tagger-0.0.8/src/layerborn/cdk_git_tagger/_jsii/cdk-git-tagger@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 02:50:55.000000 layerborn.cdk-git-tagger-0.0.8/src/layerborn/cdk_git_tagger/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:51:10.835072 layerborn.cdk-git-tagger-0.0.8/src/layerborn.cdk_git_tagger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-01-28 02:51:10.000000 layerborn.cdk-git-tagger-0.0.8/src/layerborn.cdk_git_tagger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-01-28 02:51:10.000000 layerborn.cdk-git-tagger-0.0.8/src/layerborn.cdk_git_tagger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 02:51:10.000000 layerborn.cdk-git-tagger-0.0.8/src/layerborn.cdk_git_tagger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-28 02:51:10.000000 layerborn.cdk-git-tagger-0.0.8/src/layerborn.cdk_git_tagger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-28 02:51:10.000000 layerborn.cdk-git-tagger-0.0.8/src/layerborn.cdk_git_tagger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:36:02.153904 layerborn.cdk-git-tagger-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-29 16:35:48.000000 layerborn.cdk-git-tagger-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-29 16:35:48.000000 layerborn.cdk-git-tagger-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-01-29 16:36:02.153904 layerborn.cdk-git-tagger-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-01-29 16:35:48.000000 layerborn.cdk-git-tagger-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-29 16:35:48.000000 layerborn.cdk-git-tagger-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 16:36:02.153904 layerborn.cdk-git-tagger-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-01-29 16:35:48.000000 layerborn.cdk-git-tagger-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:36:02.153904 layerborn.cdk-git-tagger-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:36:02.153904 layerborn.cdk-git-tagger-0.0.9/src/layerborn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:36:02.153904 layerborn.cdk-git-tagger-0.0.9/src/layerborn/cdk_git_tagger/
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-01-29 16:35:48.000000 layerborn.cdk-git-tagger-0.0.9/src/layerborn/cdk_git_tagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:36:02.153904 layerborn.cdk-git-tagger-0.0.9/src/layerborn/cdk_git_tagger/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-01-29 16:35:48.000000 layerborn.cdk-git-tagger-0.0.9/src/layerborn/cdk_git_tagger/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20461 2024-01-29 16:35:48.000000 layerborn.cdk-git-tagger-0.0.9/src/layerborn/cdk_git_tagger/_jsii/cdk-git-tagger@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 16:35:48.000000 layerborn.cdk-git-tagger-0.0.9/src/layerborn/cdk_git_tagger/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:36:02.153904 layerborn.cdk-git-tagger-0.0.9/src/layerborn.cdk_git_tagger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-01-29 16:36:02.000000 layerborn.cdk-git-tagger-0.0.9/src/layerborn.cdk_git_tagger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-01-29 16:36:02.000000 layerborn.cdk-git-tagger-0.0.9/src/layerborn.cdk_git_tagger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 16:36:02.000000 layerborn.cdk-git-tagger-0.0.9/src/layerborn.cdk_git_tagger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-29 16:36:02.000000 layerborn.cdk-git-tagger-0.0.9/src/layerborn.cdk_git_tagger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-29 16:36:02.000000 layerborn.cdk-git-tagger-0.0.9/src/layerborn.cdk_git_tagger.egg-info/top_level.txt
```

### Comparing `layerborn.cdk-git-tagger-0.0.8/LICENSE` & `layerborn.cdk-git-tagger-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `layerborn.cdk-git-tagger-0.0.8/PKG-INFO` & `layerborn.cdk-git-tagger-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layerborn.cdk-git-tagger
-Version: 0.0.8
+Version: 0.0.9
 Summary: CDK Aspect to tag resources with git metadata.  This provides a nice connection between the construct and the git repository.
 Home-page: https://github.com/layerborn/cdk-git-tagger-aspect.git
 Author: Jayson Rawlins<jayson.rawlins@layerborn.io>
 License: Apache-2.0
 Project-URL: Source, https://github.com/layerborn/cdk-git-tagger-aspect.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `layerborn.cdk-git-tagger-0.0.8/README.md` & `layerborn.cdk-git-tagger-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `layerborn.cdk-git-tagger-0.0.8/setup.py` & `layerborn.cdk-git-tagger-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "layerborn.cdk-git-tagger",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "CDK Aspect to tag resources with git metadata.  This provides a nice connection between the construct and the git repository.",
     "license": "Apache-2.0",
     "url": "https://github.com/layerborn/cdk-git-tagger-aspect.git",
     "long_description_content_type": "text/markdown",
     "author": "Jayson Rawlins<jayson.rawlins@layerborn.io>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "layerborn.cdk_git_tagger",
         "layerborn.cdk_git_tagger._jsii"
     ],
     "package_data": {
         "layerborn.cdk_git_tagger._jsii": [
-            "cdk-git-tagger@0.0.8.jsii.tgz"
+            "cdk-git-tagger@0.0.9.jsii.tgz"
         ],
         "layerborn.cdk_git_tagger": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `layerborn.cdk-git-tagger-0.0.8/src/layerborn/cdk_git_tagger/__init__.py` & `layerborn.cdk-git-tagger-0.0.9/src/layerborn/cdk_git_tagger/__init__.py`

 * *Files identical despite different names*

### Comparing `layerborn.cdk-git-tagger-0.0.8/src/layerborn.cdk_git_tagger.egg-info/PKG-INFO` & `layerborn.cdk-git-tagger-0.0.9/src/layerborn.cdk_git_tagger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layerborn.cdk-git-tagger
-Version: 0.0.8
+Version: 0.0.9
 Summary: CDK Aspect to tag resources with git metadata.  This provides a nice connection between the construct and the git repository.
 Home-page: https://github.com/layerborn/cdk-git-tagger-aspect.git
 Author: Jayson Rawlins<jayson.rawlins@layerborn.io>
 License: Apache-2.0
 Project-URL: Source, https://github.com/layerborn/cdk-git-tagger-aspect.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

