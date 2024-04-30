# Comparing `tmp/gardener_cicd_whd-1.2387.0.tar.gz` & `tmp/gardener_cicd_whd-1.2388.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener_cicd_whd-1.2387.0.tar", last modified: Fri Apr 26 17:05:10 2024, max compression
+gzip compressed data, was "gardener_cicd_whd-1.2388.0.tar", last modified: Tue Apr 30 05:06:02 2024, max compression
```

## Comparing `gardener_cicd_whd-1.2387.0.tar` & `gardener_cicd_whd-1.2388.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:05:10.616506 gardener_cicd_whd-1.2387.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      292 2024-04-26 17:05:10.616506 gardener_cicd_whd-1.2387.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2093 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:05:10.616506 gardener_cicd_whd-1.2387.0/gardener_cicd_whd.egg-info/
--rw-r--r--   0 root         (0) root         (0)      292 2024-04-26 17:05:10.000000 gardener_cicd_whd-1.2387.0/gardener_cicd_whd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2024-04-26 17:05:10.000000 gardener_cicd_whd-1.2387.0/gardener_cicd_whd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 17:05:10.000000 gardener_cicd_whd-1.2387.0/gardener_cicd_whd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-26 17:05:10.000000 gardener_cicd_whd-1.2387.0/gardener_cicd_whd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-04-26 17:05:10.000000 gardener_cicd_whd-1.2387.0/gardener_cicd_whd.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-26 17:05:10.616506 gardener_cicd_whd-1.2387.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2174 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      864 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/setup.whd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:05:10.616506 gardener_cicd_whd-1.2387.0/whd/
--rw-r--r--   0 root         (0) root         (0)      664 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/whd/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16633 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/whd/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)     2959 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/whd/metric.py
--rw-r--r--   0 root         (0) root         (0)     5690 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/whd/model.py
--rw-r--r--   0 root         (0) root         (0)     3268 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/whd/pipelines.py
--rw-r--r--   0 root         (0) root         (0)    18333 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/whd/pull_request.py
--rw-r--r--   0 root         (0) root         (0)     1705 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/whd/server.py
--rw-r--r--   0 root         (0) root         (0)      707 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/whd/util.py
--rw-r--r--   0 root         (0) root         (0)     3097 2024-04-26 17:04:22.000000 gardener_cicd_whd-1.2387.0/whd/webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:06:02.557183 gardener_cicd_whd-1.2388.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      292 2024-04-30 05:06:02.557183 gardener_cicd_whd-1.2388.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:06:02.557183 gardener_cicd_whd-1.2388.0/gardener_cicd_whd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      292 2024-04-30 05:06:02.000000 gardener_cicd_whd-1.2388.0/gardener_cicd_whd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2024-04-30 05:06:02.000000 gardener_cicd_whd-1.2388.0/gardener_cicd_whd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 05:06:02.000000 gardener_cicd_whd-1.2388.0/gardener_cicd_whd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-30 05:06:02.000000 gardener_cicd_whd-1.2388.0/gardener_cicd_whd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-30 05:06:02.000000 gardener_cicd_whd-1.2388.0/gardener_cicd_whd.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-30 05:06:02.557183 gardener_cicd_whd-1.2388.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      864 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/setup.whd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:06:02.557183 gardener_cicd_whd-1.2388.0/whd/
+-rw-r--r--   0 root         (0) root         (0)      664 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/whd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16633 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/whd/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)     2959 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/whd/metric.py
+-rw-r--r--   0 root         (0) root         (0)     5690 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/whd/model.py
+-rw-r--r--   0 root         (0) root         (0)     3268 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/whd/pipelines.py
+-rw-r--r--   0 root         (0) root         (0)    18333 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/whd/pull_request.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/whd/server.py
+-rw-r--r--   0 root         (0) root         (0)      707 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/whd/util.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2024-04-30 04:58:56.000000 gardener_cicd_whd-1.2388.0/whd/webhook.py
```

### Comparing `gardener_cicd_whd-1.2387.0/LICENSE` & `gardener_cicd_whd-1.2388.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gardener_cicd_whd-1.2387.0/README.md` & `gardener_cicd_whd-1.2388.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener_cicd_whd-1.2387.0/setup.py` & `gardener_cicd_whd-1.2388.0/setup.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_whd-1.2387.0/setup.whd.py` & `gardener_cicd_whd-1.2388.0/setup.whd.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         return f.read().strip()
 
 
 setuptools.setup(
     name='gardener-cicd-whd',
     version=version(),
     description='Gardener CI/CD Webhook Dispatcher',
-    python_requires='>=3.10',
+    python_requires='>=3.11',
     py_modules=modules(),
     packages=['whd'],
     package_data={
         'ci':['version'],
     },
     install_requires=list(requirements()),
     entry_points={
```

### Comparing `gardener_cicd_whd-1.2387.0/whd/__init__.py` & `gardener_cicd_whd-1.2388.0/whd/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_whd-1.2387.0/whd/dispatcher.py` & `gardener_cicd_whd-1.2388.0/whd/dispatcher.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_whd-1.2387.0/whd/metric.py` & `gardener_cicd_whd-1.2388.0/whd/metric.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_whd-1.2387.0/whd/model.py` & `gardener_cicd_whd-1.2388.0/whd/model.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_whd-1.2387.0/whd/pipelines.py` & `gardener_cicd_whd-1.2388.0/whd/pipelines.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_whd-1.2387.0/whd/pull_request.py` & `gardener_cicd_whd-1.2388.0/whd/pull_request.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_whd-1.2387.0/whd/server.py` & `gardener_cicd_whd-1.2388.0/whd/server.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_whd-1.2387.0/whd/util.py` & `gardener_cicd_whd-1.2388.0/whd/util.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_whd-1.2387.0/whd/webhook.py` & `gardener_cicd_whd-1.2388.0/whd/webhook.py`

 * *Files identical despite different names*
