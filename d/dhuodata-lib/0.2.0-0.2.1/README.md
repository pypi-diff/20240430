# Comparing `tmp/dhuodata-lib-0.2.0.tar.gz` & `tmp/dhuodata-lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata-lib-0.2.0.tar", last modified: Tue Apr 30 02:41:58 2024, max compression
+gzip compressed data, was "dhuodata-lib-0.2.1.tar", last modified: Tue Apr 30 03:05:04 2024, max compression
```

## Comparing `dhuodata-lib-0.2.0.tar` & `dhuodata-lib-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 02:41:58.127828 dhuodata-lib-0.2.0/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-30 02:41:58.127828 dhuodata-lib-0.2.0/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.2.0/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-30 02:41:58.127828 dhuodata-lib-0.2.0/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-30 02:41:51.000000 dhuodata-lib-0.2.0/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 02:41:58.123828 dhuodata-lib-0.2.0/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 02:41:58.123828 dhuodata-lib-0.2.0/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     2528 2024-04-30 02:41:58.000000 dhuodata-lib-0.2.0/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-04-30 02:41:58.000000 dhuodata-lib-0.2.0/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-30 02:41:58.000000 dhuodata-lib-0.2.0/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-04-30 02:41:58.000000 dhuodata-lib-0.2.0/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-30 02:41:58.000000 dhuodata-lib-0.2.0/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 02:41:58.127828 dhuodata-lib-0.2.0/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata-lib-0.2.0/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata-lib-0.2.0/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     4125 2024-04-30 02:11:57.000000 dhuodata-lib-0.2.0/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata-lib-0.2.0/src/dhuolib/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata-lib-0.2.0/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1329 2024-04-30 02:41:36.000000 dhuodata-lib-0.2.0/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      750 2024-04-29 11:53:52.000000 dhuodata-lib-0.2.0/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata-lib-0.2.0/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 02:41:58.127828 dhuodata-lib-0.2.0/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2540 2024-04-29 12:52:51.000000 dhuodata-lib-0.2.0/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 03:05:04.156993 dhuodata-lib-0.2.1/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-30 03:05:04.156993 dhuodata-lib-0.2.1/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.2.1/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-30 03:05:04.156993 dhuodata-lib-0.2.1/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-30 03:04:54.000000 dhuodata-lib-0.2.1/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 03:05:04.156993 dhuodata-lib-0.2.1/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 03:05:04.156993 dhuodata-lib-0.2.1/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     2528 2024-04-30 03:05:04.000000 dhuodata-lib-0.2.1/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-04-30 03:05:04.000000 dhuodata-lib-0.2.1/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-30 03:05:04.000000 dhuodata-lib-0.2.1/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-04-30 03:05:04.000000 dhuodata-lib-0.2.1/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-30 03:05:04.000000 dhuodata-lib-0.2.1/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 03:05:04.156993 dhuodata-lib-0.2.1/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata-lib-0.2.1/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata-lib-0.2.1/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     4125 2024-04-30 02:11:57.000000 dhuodata-lib-0.2.1/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata-lib-0.2.1/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata-lib-0.2.1/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1353 2024-04-30 03:04:47.000000 dhuodata-lib-0.2.1/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      750 2024-04-29 11:53:52.000000 dhuodata-lib-0.2.1/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata-lib-0.2.1/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 03:05:04.156993 dhuodata-lib-0.2.1/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2540 2024-04-29 12:52:51.000000 dhuodata-lib-0.2.1/tests/test_dhuolib.py
```

### Comparing `dhuodata-lib-0.2.0/PKG-INFO` & `dhuodata-lib-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.2.0
+Version: 0.2.1
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuodata-lib-0.2.0/README.md` & `dhuodata-lib-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.2.0/setup.py` & `dhuodata-lib-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.2.0",
+    version="0.2.1",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata-lib-0.2.0/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata-lib-0.2.1/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.2.0
+Version: 0.2.1
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuodata-lib-0.2.0/src/dhuolib/clients.py` & `dhuodata-lib-0.2.1/src/dhuolib/clients.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.2.0/src/dhuolib/predict.py` & `dhuodata-lib-0.2.1/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.2.0/src/dhuolib/services.py` & `dhuodata-lib-0.2.1/src/dhuolib/services.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 
     def create_experiment_by_conf_json(self, experiment_params, files):
         if experiment_params is None and isinstance(experiment_params, dict):
             raise ValueError("json_data must be a dict")
 
         response = requests.post(
             f"{self.service_endpoint}/save",
-            json=experiment_params,
+            data=json.dumps(experiment_params),
             files=files
         )
         return response
 
     def run_experiment(self, run_params, files=None):
         if run_params is None and isinstance(run_params, str):
             raise ValueError("json_data must be a dict")
         if files:
             response = requests.post(
                 f"{self.service_endpoint}/run",
-                json=run_params,
+                data=json.dumps(run_params),
                 headers=self.headers,
                 files=files
             )
             return response
 
         response = requests.post(
             f"{self.service_endpoint}/run",
```

### Comparing `dhuodata-lib-0.2.0/src/dhuolib/validations.py` & `dhuodata-lib-0.2.1/src/dhuolib/validations.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.2.0/tests/test_dhuolib.py` & `dhuodata-lib-0.2.1/tests/test_dhuolib.py`

 * *Files identical despite different names*

