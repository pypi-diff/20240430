# Comparing `tmp/netbox_napalm_plugin-0.1.8.tar.gz` & `tmp/netbox_napalm_plugin-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_napalm_plugin-0.1.8.tar", last modified: Tue Apr 16 16:26:37 2024, max compression
+gzip compressed data, was "netbox_napalm_plugin-0.1.9.tar", last modified: Mon Apr 29 22:57:49 2024, max compression
```

## Comparing `netbox_napalm_plugin-0.1.8.tar` & `netbox_napalm_plugin-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:26:37.619276 netbox_napalm_plugin-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-16 16:26:37.615276 netbox_napalm_plugin-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:26:37.611276 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:26:37.615276 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:26:37.615276 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:26:37.611276 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:26:37.615276 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/templates/netbox_napalm_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:26:37.615276 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-16 16:26:37.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-16 16:26:37.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:26:37.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-16 16:26:37.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 16:26:37.000000 netbox_napalm_plugin-0.1.8/netbox_napalm_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 16:26:37.619276 netbox_napalm_plugin-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:26:37.615276 netbox_napalm_plugin-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-16 16:26:33.000000 netbox_napalm_plugin-0.1.8/tests/test_netbox_napalm_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.469242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.469242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.469242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.465242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.465242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/netbox_napalm_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/netbox_napalm_plugin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   196388 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/netbox_napalm_plugin/js/config.js
+-rw-r--r--   0 runner    (1001) docker     (127)   198227 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/netbox_napalm_plugin/js/lldp.js
+-rw-r--r--   0 runner    (1001) docker     (127)   234145 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/netbox_napalm_plugin/js/status.js
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.465242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-29 22:57:49.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-29 22:57:49.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:57:49.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-29 22:57:49.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 22:57:49.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/tests/test_netbox_napalm_plugin.py
```

### Comparing `netbox_napalm_plugin-0.1.8/CONTRIBUTING.md` & `netbox_napalm_plugin-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/LICENSE` & `netbox_napalm_plugin-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/PKG-INFO` & `netbox_napalm_plugin-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-napalm-plugin
-Version: 0.1.8
+Version: 0.1.9
 Summary: NetBox plugin for Napalm.
 Author-email: Arthur Hanson <ahanson@netboxlabs.com>
 Project-URL: Documentation, https://github.com/netbox-community/netbox-napalm-plugin/blob/main/README.md
 Project-URL: Source, https://github.com/netbox-community/netbox-napalm-plugin
 Project-URL: Tracker, https://github.com/netbox-community/netbox-napalm-plugin/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `netbox_napalm_plugin-0.1.8/README.md` & `netbox_napalm_plugin-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/__init__.py` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for NetBox Napalm Plugin."""
 
 __author__ = """Arthur Hanson"""
 __email__ = "ahanson@netboxlabs.com"
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 
 from extras.plugins import PluginConfig
 
 
 class NapalmPlatformConfig(PluginConfig):
     name = "netbox_napalm_plugin"
```

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/api/serializers.py` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/api/views.py` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/filtersets.py` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/migrations/0001_initial.py` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/models.py` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/models.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/tables.py` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/urls.py` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin/views.py` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/views.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin.egg-info/PKG-INFO` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-napalm-plugin
-Version: 0.1.8
+Version: 0.1.9
 Summary: NetBox plugin for Napalm.
 Author-email: Arthur Hanson <ahanson@netboxlabs.com>
 Project-URL: Documentation, https://github.com/netbox-community/netbox-napalm-plugin/blob/main/README.md
 Project-URL: Source, https://github.com/netbox-community/netbox-napalm-plugin
 Project-URL: Tracker, https://github.com/netbox-community/netbox-napalm-plugin/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `netbox_napalm_plugin-0.1.8/netbox_napalm_plugin.egg-info/SOURCES.txt` & `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -19,13 +19,16 @@
 netbox_napalm_plugin/api/__init__.py
 netbox_napalm_plugin/api/serializers.py
 netbox_napalm_plugin/api/urls.py
 netbox_napalm_plugin/api/views.py
 netbox_napalm_plugin/migrations/0001_initial.py
 netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py
 netbox_napalm_plugin/migrations/__init__.py
+netbox_napalm_plugin/static/netbox_napalm_plugin/js/config.js
+netbox_napalm_plugin/static/netbox_napalm_plugin/js/lldp.js
+netbox_napalm_plugin/static/netbox_napalm_plugin/js/status.js
 netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html
 netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html
 netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html
 netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html
 tests/__init__.py
 tests/test_netbox_napalm_plugin.py
```

### Comparing `netbox_napalm_plugin-0.1.8/pyproject.toml` & `netbox_napalm_plugin-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name =  "netbox-napalm-plugin"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
     {name = "Arthur Hanson", email = "ahanson@netboxlabs.com"},
 ]
 description = "NetBox plugin for Napalm."
 readme = "README.md"
 
 classifiers=[
```

