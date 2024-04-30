# Comparing `tmp/pulumi_kafka-3.8.0a1714110387.tar.gz` & `tmp/pulumi_kafka-3.8.0a1714455824.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kafka-3.8.0a1714110387.tar", last modified: Fri Apr 26 05:50:51 2024, max compression
+gzip compressed data, was "pulumi_kafka-3.8.0a1714455824.tar", last modified: Tue Apr 30 05:46:47 2024, max compression
```

## Comparing `pulumi_kafka-3.8.0a1714110387.tar` & `pulumi_kafka-3.8.0a1714455824.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:50:51.832517 pulumi_kafka-3.8.0a1714110387/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-26 05:50:51.832517 pulumi_kafka-3.8.0a1714110387/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:50:51.828517 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    23117 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/acl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:50:51.832517 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/get_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    31331 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/quota.py
--rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka/user_scram_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:50:51.832517 pulumi_kafka-3.8.0a1714110387/pulumi_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-26 05:50:51.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-26 05:50:51.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 05:50:51.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 05:50:51.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 05:50:51.000000 pulumi_kafka-3.8.0a1714110387/pulumi_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-26 05:50:45.000000 pulumi_kafka-3.8.0a1714110387/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 05:50:51.832517 pulumi_kafka-3.8.0a1714110387/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:46:47.285396 pulumi_kafka-3.8.0a1714455824/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-30 05:46:47.285396 pulumi_kafka-3.8.0a1714455824/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:46:47.281396 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23117 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/acl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:46:47.285396 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/get_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31331 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka/user_scram_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:46:47.285396 pulumi_kafka-3.8.0a1714455824/pulumi_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-30 05:46:47.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-30 05:46:47.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 05:46:47.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 05:46:47.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 05:46:47.000000 pulumi_kafka-3.8.0a1714455824/pulumi_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-30 05:46:40.000000 pulumi_kafka-3.8.0a1714455824/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 05:46:47.285396 pulumi_kafka-3.8.0a1714455824/setup.cfg
```

### Comparing `pulumi_kafka-3.8.0a1714110387/PKG-INFO` & `pulumi_kafka-3.8.0a1714455824/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kafka
-Version: 3.8.0a1714110387
+Version: 3.8.0a1714455824
 Summary: A Pulumi package for creating and managing Kafka.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi,kafka
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.8.0a1714110387/README.md` & `pulumi_kafka-3.8.0a1714455824/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1714110387/pulumi_kafka/__init__.py` & `pulumi_kafka-3.8.0a1714455824/pulumi_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1714110387/pulumi_kafka/_utilities.py` & `pulumi_kafka-3.8.0a1714455824/pulumi_kafka/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1714110387/pulumi_kafka/acl.py` & `pulumi_kafka-3.8.0a1714455824/pulumi_kafka/acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1714110387/pulumi_kafka/config/__init__.pyi` & `pulumi_kafka-3.8.0a1714455824/pulumi_kafka/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1714110387/pulumi_kafka/config/vars.py` & `pulumi_kafka-3.8.0a1714455824/pulumi_kafka/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1714110387/pulumi_kafka/get_topic.py` & `pulumi_kafka-3.8.0a1714455824/pulumi_kafka/get_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1714110387/pulumi_kafka/provider.py` & `pulumi_kafka-3.8.0a1714455824/pulumi_kafka/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1714110387/pulumi_kafka/quota.py` & `pulumi_kafka-3.8.0a1714455824/pulumi_kafka/quota.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1714110387/pulumi_kafka/topic.py` & `pulumi_kafka-3.8.0a1714455824/pulumi_kafka/topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1714110387/pulumi_kafka/user_scram_credential.py` & `pulumi_kafka-3.8.0a1714455824/pulumi_kafka/user_scram_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1714110387/pulumi_kafka.egg-info/PKG-INFO` & `pulumi_kafka-3.8.0a1714455824/pulumi_kafka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kafka
-Version: 3.8.0a1714110387
+Version: 3.8.0a1714455824
 Summary: A Pulumi package for creating and managing Kafka.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi,kafka
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.8.0a1714110387/pulumi_kafka.egg-info/SOURCES.txt` & `pulumi_kafka-3.8.0a1714455824/pulumi_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1714110387/pyproject.toml` & `pulumi_kafka-3.8.0a1714455824/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kafka"
   description = "A Pulumi package for creating and managing Kafka."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "kafka"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.8.0a1714110387"
+  version = "3.8.0a1714455824"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-kafka"
 
 [build-system]
```
