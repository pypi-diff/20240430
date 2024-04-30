# Comparing `tmp/pulumi_kubernetes_cert_manager-0.0.7a1713503099.tar.gz` & `tmp/pulumi_kubernetes_cert_manager-0.0.7a1714496222.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_cert_manager-0.0.7a1713503099.tar", last modified: Fri Apr 19 05:10:36 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_cert_manager-0.0.7a1714496222.tar", last modified: Tue Apr 30 17:04:11 2024, max compression
```

## Comparing `pulumi_kubernetes_cert_manager-0.0.7a1713503099.tar` & `pulumi_kubernetes_cert_manager-0.0.7a1714496222.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-19 05:10:36.336100 pulumi_kubernetes_cert_manager-0.0.7a1713503099/
--rw-r--r--   0 runner    (1000) runner    (1000)     1951 2024-04-19 05:10:36.336100 pulumi_kubernetes_cert_manager-0.0.7a1713503099/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-04-19 05:10:35.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-19 05:10:36.336100 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/
--rw-------   0 runner    (1000) runner    (1000)      782 2024-04-19 05:10:35.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/__init__.py
--rw-------   0 runner    (1000) runner    (1000)    90893 2024-04-19 05:10:35.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/_inputs.py
--rw-------   0 runner    (1000) runner    (1000)     9228 2024-04-19 05:10:35.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/_utilities.py
--rw-------   0 runner    (1000) runner    (1000)    37520 2024-04-19 05:10:35.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/cert_manager.py
--rw-------   0 runner    (1000) runner    (1000)     3383 2024-04-19 05:10:35.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/outputs.py
--rw-------   0 runner    (1000) runner    (1000)     2781 2024-04-19 05:10:35.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/provider.py
--rw-------   0 runner    (1000) runner    (1000)       60 2024-04-19 05:10:35.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/pulumi-plugin.json
--rw-------   0 runner    (1000) runner    (1000)        0 2024-04-19 05:10:35.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/py.typed
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-19 05:10:36.336100 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1951 2024-04-19 05:10:36.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      692 2024-04-19 05:10:36.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-19 05:10:36.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-19 05:10:36.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)       81 2024-04-19 05:10:36.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       31 2024-04-19 05:10:36.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-19 05:10:36.336100 pulumi_kubernetes_cert_manager-0.0.7a1713503099/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)     1427 2024-04-19 05:10:35.000000 pulumi_kubernetes_cert_manager-0.0.7a1713503099/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-30 17:04:11.142454 pulumi_kubernetes_cert_manager-0.0.7a1714496222/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1951 2024-04-30 17:04:11.142454 pulumi_kubernetes_cert_manager-0.0.7a1714496222/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-04-30 17:04:10.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-30 17:04:11.142454 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/
+-rw-------   0 runner    (1000) runner    (1000)      782 2024-04-30 17:04:10.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)    90893 2024-04-30 17:04:10.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/_inputs.py
+-rw-------   0 runner    (1000) runner    (1000)     9228 2024-04-30 17:04:10.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/_utilities.py
+-rw-------   0 runner    (1000) runner    (1000)    37520 2024-04-30 17:04:10.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/cert_manager.py
+-rw-------   0 runner    (1000) runner    (1000)     3383 2024-04-30 17:04:10.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/outputs.py
+-rw-------   0 runner    (1000) runner    (1000)     2781 2024-04-30 17:04:10.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/provider.py
+-rw-------   0 runner    (1000) runner    (1000)       60 2024-04-30 17:04:10.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/pulumi-plugin.json
+-rw-------   0 runner    (1000) runner    (1000)        0 2024-04-30 17:04:10.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/py.typed
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-30 17:04:11.142454 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1951 2024-04-30 17:04:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      692 2024-04-30 17:04:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-30 17:04:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-30 17:04:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)       81 2024-04-30 17:04:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       31 2024-04-30 17:04:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-30 17:04:11.142454 pulumi_kubernetes_cert_manager-0.0.7a1714496222/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)     1427 2024-04-30 17:04:10.000000 pulumi_kubernetes_cert_manager-0.0.7a1714496222/setup.py
```

### Comparing `pulumi_kubernetes_cert_manager-0.0.7a1713503099/PKG-INFO` & `pulumi_kubernetes_cert_manager-0.0.7a1714496222/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_cert_manager
-Version: 0.0.7a1713503099
+Version: 0.0.7a1714496222
 Summary: Strongly-typed Cert Manager installation
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-kubernetes-cert-manager
 Keywords: pulumi kubernetes cert-manager kind/component category/infrastructure
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kubernetes_cert_manager-0.0.7a1713503099/README.md` & `pulumi_kubernetes_cert_manager-0.0.7a1714496222/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/__init__.py` & `pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/_inputs.py` & `pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/_utilities.py` & `pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/cert_manager.py` & `pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/cert_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/outputs.py` & `pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager/provider.py` & `pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager.egg-info/PKG-INFO` & `pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-kubernetes-cert-manager
-Version: 0.0.7a1713503099
+Version: 0.0.7a1714496222
 Summary: Strongly-typed Cert Manager installation
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-kubernetes-cert-manager
 Keywords: pulumi kubernetes cert-manager kind/component category/infrastructure
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kubernetes_cert_manager-0.0.7a1713503099/pulumi_kubernetes_cert_manager.egg-info/SOURCES.txt` & `pulumi_kubernetes_cert_manager-0.0.7a1714496222/pulumi_kubernetes_cert_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_cert_manager-0.0.7a1713503099/setup.py` & `pulumi_kubernetes_cert_manager-0.0.7a1714496222/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.7a1713503099"
+VERSION = "0.0.7a1714496222"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "kubernetes-cert-manager Pulumi Package - Development Version"
```

