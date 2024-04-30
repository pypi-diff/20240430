# Comparing `tmp/pulumiverse_doppler-0.1.1.tar.gz` & `tmp/pulumiverse_doppler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_doppler-0.1.1.tar", last modified: Tue Apr 30 08:44:23 2024, max compression
+gzip compressed data, was "pulumiverse_doppler-0.1.2.tar", last modified: Tue Apr 30 09:20:21 2024, max compression
```

## Comparing `pulumiverse_doppler-0.1.1.tar` & `pulumiverse_doppler-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:44:23.644851 pulumiverse_doppler-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 08:44:23.644851 pulumiverse_doppler-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:44:23.644851 pulumiverse_doppler-0.1.1/pulumiverse_doppler/
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/branch_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:44:23.644851 pulumiverse_doppler-0.1.1/pulumiverse_doppler/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/donfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11569 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12697 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler/service_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:44:23.644851 pulumiverse_doppler-0.1.1/pulumiverse_doppler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/pulumiverse_doppler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 08:44:23.644851 pulumiverse_doppler-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-30 08:44:23.000000 pulumiverse_doppler-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:20:21.258834 pulumiverse_doppler-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 09:20:21.254835 pulumiverse_doppler-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:20:21.254835 pulumiverse_doppler-0.1.2/pulumiverse_doppler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/branch_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:20:21.254835 pulumiverse_doppler-0.1.2/pulumiverse_doppler/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/donfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11569 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12697 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/service_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:20:21.254835 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 09:20:21.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-30 09:20:21.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:20:21.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:20:21.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 09:20:21.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 09:20:21.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:20:21.258834 pulumiverse_doppler-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/setup.py
```

### Comparing `pulumiverse_doppler-0.1.1/PKG-INFO` & `pulumiverse_doppler-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_doppler
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.1.1/README.md` & `pulumiverse_doppler-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler/__init__.py` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler/_utilities.py` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler/branch_config.py` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler/branch_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler/config/vars.py` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler/config.py` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler/config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler/donfig.py` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler/donfig.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler/environment.py` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler/environment.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler/project.py` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler/project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler/provider.py` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler/secret.py` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler/secret.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler/secrets.py` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler/secrets.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler/service_token.py` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler/service_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler.egg-info/PKG-INFO` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-doppler
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.1.1/pulumiverse_doppler.egg-info/SOURCES.txt` & `pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.1/setup.py` & `pulumiverse_doppler-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "doppler Pulumi Package - Development Version"
```

