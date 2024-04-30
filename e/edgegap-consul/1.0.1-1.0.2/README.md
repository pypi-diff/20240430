# Comparing `tmp/edgegap_consul-1.0.1.tar.gz` & `tmp/edgegap_consul-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_consul-1.0.1.tar", max compression
+gzip compressed data, was "edgegap_consul-1.0.2.tar", max compression
```

## Comparing `edgegap_consul-1.0.1.tar` & `edgegap_consul-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1993 2024-04-29 18:21:35.339371 edgegap_consul-1.0.1/LICENSE
--rw-r--r--   0        0        0     2152 2024-04-29 18:21:35.343371 edgegap_consul-1.0.1/README.md
--rw-r--r--   0        0        0      256 2024-04-29 18:21:35.343371 edgegap_consul-1.0.1/edgegap_consul/__init__.py
--rw-r--r--   0        0        0     2300 2024-04-29 18:21:35.343371 edgegap_consul-1.0.1/edgegap_consul/_client.py
--rw-r--r--   0        0        0      399 2024-04-29 18:21:35.343371 edgegap_consul-1.0.1/edgegap_consul/_configuration.py
--rw-r--r--   0        0        0     1298 2024-04-29 18:21:35.343371 edgegap_consul-1.0.1/edgegap_consul/_factory.py
--rw-r--r--   0        0        0     1471 2024-04-29 18:21:35.343371 edgegap_consul-1.0.1/edgegap_consul/_reader.py
--rw-r--r--   0        0        0      519 2024-04-29 18:21:39.443403 edgegap_consul-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 edgegap_consul-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 18:23:33.437036 edgegap_consul-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2152 2024-04-29 18:23:33.437036 edgegap_consul-1.0.2/README.md
+-rw-r--r--   0        0        0      256 2024-04-29 18:23:33.437036 edgegap_consul-1.0.2/edgegap_consul/__init__.py
+-rw-r--r--   0        0        0     2300 2024-04-29 18:23:33.437036 edgegap_consul-1.0.2/edgegap_consul/_client.py
+-rw-r--r--   0        0        0      399 2024-04-29 18:23:33.437036 edgegap_consul-1.0.2/edgegap_consul/_configuration.py
+-rw-r--r--   0        0        0     1298 2024-04-29 18:23:33.437036 edgegap_consul-1.0.2/edgegap_consul/_factory.py
+-rw-r--r--   0        0        0     1471 2024-04-29 18:23:33.437036 edgegap_consul-1.0.2/edgegap_consul/_reader.py
+-rw-r--r--   0        0        0      519 2024-04-29 18:23:45.665094 edgegap_consul-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 edgegap_consul-1.0.2/PKG-INFO
```

### Comparing `edgegap_consul-1.0.1/LICENSE` & `edgegap_consul-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.0.1/README.md` & `edgegap_consul-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.0.1/edgegap_consul/_client.py` & `edgegap_consul-1.0.2/edgegap_consul/_client.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.0.1/edgegap_consul/_factory.py` & `edgegap_consul-1.0.2/edgegap_consul/_factory.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.0.1/edgegap_consul/_reader.py` & `edgegap_consul-1.0.2/edgegap_consul/_reader.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.0.1/pyproject.toml` & `edgegap_consul-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-consul"
-version = "1.0.1"
+version = "1.0.2"
 description = "The Edgegap Consul library includes various tools and helpers for interacting with Consul. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = { version = "^3.9.5", extras = ["speedups"] }
```

### Comparing `edgegap_consul-1.0.1/PKG-INFO` & `edgegap_consul-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-consul
-Version: 1.0.1
+Version: 1.0.2
 Summary: The Edgegap Consul library includes various tools and helpers for interacting with Consul. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

