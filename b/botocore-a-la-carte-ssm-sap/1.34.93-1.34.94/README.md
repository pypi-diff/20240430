# Comparing `tmp/botocore-a-la-carte-ssm-sap-1.34.93.tar.gz` & `tmp/botocore-a-la-carte-ssm-sap-1.34.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ssm-sap-1.34.93.tar", last modified: Sat Apr 27 01:01:07 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-ssm-sap-1.34.94.tar", last modified: Tue Apr 30 01:01:45 2024, max compression
```

## Comparing `botocore-a-la-carte-ssm-sap-1.34.93.tar` & `botocore-a-la-carte-ssm-sap-1.34.94.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:01:07.201269 botocore-a-la-carte-ssm-sap-1.34.93/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-27 01:01:06.000000 botocore-a-la-carte-ssm-sap-1.34.93/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-27 01:01:07.201269 botocore-a-la-carte-ssm-sap-1.34.93/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:01:07.201269 botocore-a-la-carte-ssm-sap-1.34.93/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:01:07.201269 botocore-a-la-carte-ssm-sap-1.34.93/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:01:07.201269 botocore-a-la-carte-ssm-sap-1.34.93/botocore/data/ssm-sap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:01:07.201269 botocore-a-la-carte-ssm-sap-1.34.93/botocore/data/ssm-sap/2018-05-10/
--rw-r--r--   0 runner    (1001) docker     (127)    17628 2024-04-27 01:00:35.000000 botocore-a-la-carte-ssm-sap-1.34.93/botocore/data/ssm-sap/2018-05-10/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-27 01:00:35.000000 botocore-a-la-carte-ssm-sap-1.34.93/botocore/data/ssm-sap/2018-05-10/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    52374 2024-04-27 01:00:35.000000 botocore-a-la-carte-ssm-sap-1.34.93/botocore/data/ssm-sap/2018-05-10/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:01:07.201269 botocore-a-la-carte-ssm-sap-1.34.93/botocore_a_la_carte_ssm_sap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-27 01:01:07.000000 botocore-a-la-carte-ssm-sap-1.34.93/botocore_a_la_carte_ssm_sap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-27 01:01:07.000000 botocore-a-la-carte-ssm-sap-1.34.93/botocore_a_la_carte_ssm_sap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 01:01:07.000000 botocore-a-la-carte-ssm-sap-1.34.93/botocore_a_la_carte_ssm_sap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 01:01:07.000000 botocore-a-la-carte-ssm-sap-1.34.93/botocore_a_la_carte_ssm_sap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 01:01:07.201269 botocore-a-la-carte-ssm-sap-1.34.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-27 01:01:06.000000 botocore-a-la-carte-ssm-sap-1.34.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:45.747334 botocore-a-la-carte-ssm-sap-1.34.94/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-30 01:01:45.000000 botocore-a-la-carte-ssm-sap-1.34.94/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-30 01:01:45.743334 botocore-a-la-carte-ssm-sap-1.34.94/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:45.743334 botocore-a-la-carte-ssm-sap-1.34.94/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:45.743334 botocore-a-la-carte-ssm-sap-1.34.94/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:45.743334 botocore-a-la-carte-ssm-sap-1.34.94/botocore/data/ssm-sap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:45.743334 botocore-a-la-carte-ssm-sap-1.34.94/botocore/data/ssm-sap/2018-05-10/
+-rw-r--r--   0 runner    (1001) docker     (127)    17628 2024-04-30 01:01:14.000000 botocore-a-la-carte-ssm-sap-1.34.94/botocore/data/ssm-sap/2018-05-10/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-30 01:01:14.000000 botocore-a-la-carte-ssm-sap-1.34.94/botocore/data/ssm-sap/2018-05-10/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    52374 2024-04-30 01:01:14.000000 botocore-a-la-carte-ssm-sap-1.34.94/botocore/data/ssm-sap/2018-05-10/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:45.743334 botocore-a-la-carte-ssm-sap-1.34.94/botocore_a_la_carte_ssm_sap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-30 01:01:45.000000 botocore-a-la-carte-ssm-sap-1.34.94/botocore_a_la_carte_ssm_sap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-30 01:01:45.000000 botocore-a-la-carte-ssm-sap-1.34.94/botocore_a_la_carte_ssm_sap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 01:01:45.000000 botocore-a-la-carte-ssm-sap-1.34.94/botocore_a_la_carte_ssm_sap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 01:01:45.000000 botocore-a-la-carte-ssm-sap-1.34.94/botocore_a_la_carte_ssm_sap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 01:01:45.747334 botocore-a-la-carte-ssm-sap-1.34.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-30 01:01:45.000000 botocore-a-la-carte-ssm-sap-1.34.94/setup.py
```

### Comparing `botocore-a-la-carte-ssm-sap-1.34.93/LICENSE.txt` & `botocore-a-la-carte-ssm-sap-1.34.94/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ssm-sap-1.34.93/PKG-INFO` & `botocore-a-la-carte-ssm-sap-1.34.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ssm-sap
-Version: 1.34.93
+Version: 1.34.94
 Summary: ssm-sap data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ssm-sap-1.34.93/botocore/data/ssm-sap/2018-05-10/endpoint-rule-set-1.json` & `botocore-a-la-carte-ssm-sap-1.34.94/botocore/data/ssm-sap/2018-05-10/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ssm-sap-1.34.93/botocore/data/ssm-sap/2018-05-10/paginators-1.json` & `botocore-a-la-carte-ssm-sap-1.34.94/botocore/data/ssm-sap/2018-05-10/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ssm-sap-1.34.93/botocore/data/ssm-sap/2018-05-10/service-2.json` & `botocore-a-la-carte-ssm-sap-1.34.94/botocore/data/ssm-sap/2018-05-10/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ssm-sap-1.34.93/botocore_a_la_carte_ssm_sap.egg-info/PKG-INFO` & `botocore-a-la-carte-ssm-sap-1.34.94/botocore_a_la_carte_ssm_sap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ssm-sap
-Version: 1.34.93
+Version: 1.34.94
 Summary: ssm-sap data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ssm-sap-1.34.93/setup.py` & `botocore-a-la-carte-ssm-sap-1.34.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ssm-sap',
-    version="1.34.93",
+    version="1.34.94",
     description='ssm-sap data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ssm-sap/*/*.json'],
```

