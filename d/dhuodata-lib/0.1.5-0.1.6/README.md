# Comparing `tmp/dhuodata-lib-0.1.5.tar.gz` & `tmp/dhuodata-lib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata-lib-0.1.5.tar", last modified: Mon Apr 29 18:42:51 2024, max compression
+gzip compressed data, was "dhuodata-lib-0.1.6.tar", last modified: Tue Apr 30 01:51:35 2024, max compression
```

## Comparing `dhuodata-lib-0.1.5.tar` & `dhuodata-lib-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.1.5/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-29 18:42:03.000000 dhuodata-lib-0.1.5/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     2528 2024-04-29 18:42:51.000000 dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-04-29 18:42:51.000000 dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-29 18:42:51.000000 dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-04-29 18:42:51.000000 dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-29 18:42:51.000000 dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata-lib-0.1.5/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata-lib-0.1.5/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     4134 2024-04-29 12:51:47.000000 dhuodata-lib-0.1.5/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata-lib-0.1.5/src/dhuolib/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata-lib-0.1.5/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1388 2024-04-29 11:48:37.000000 dhuodata-lib-0.1.5/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      750 2024-04-29 11:53:52.000000 dhuodata-lib-0.1.5/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata-lib-0.1.5/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2540 2024-04-29 12:52:51.000000 dhuodata-lib-0.1.5/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 01:51:35.781590 dhuodata-lib-0.1.6/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-30 01:51:35.781590 dhuodata-lib-0.1.6/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.1.6/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-30 01:51:35.781590 dhuodata-lib-0.1.6/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-30 01:51:12.000000 dhuodata-lib-0.1.6/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 01:51:35.781590 dhuodata-lib-0.1.6/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 01:51:35.781590 dhuodata-lib-0.1.6/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     2528 2024-04-30 01:51:35.000000 dhuodata-lib-0.1.6/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-04-30 01:51:35.000000 dhuodata-lib-0.1.6/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-30 01:51:35.000000 dhuodata-lib-0.1.6/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-04-30 01:51:35.000000 dhuodata-lib-0.1.6/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-30 01:51:35.000000 dhuodata-lib-0.1.6/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 01:51:35.781590 dhuodata-lib-0.1.6/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata-lib-0.1.6/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata-lib-0.1.6/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     4160 2024-04-30 01:48:57.000000 dhuodata-lib-0.1.6/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata-lib-0.1.6/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata-lib-0.1.6/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1353 2024-04-30 01:49:26.000000 dhuodata-lib-0.1.6/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      750 2024-04-29 11:53:52.000000 dhuodata-lib-0.1.6/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata-lib-0.1.6/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 01:51:35.781590 dhuodata-lib-0.1.6/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2540 2024-04-29 12:52:51.000000 dhuodata-lib-0.1.6/tests/test_dhuolib.py
```

### Comparing `dhuodata-lib-0.1.5/PKG-INFO` & `dhuodata-lib-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuodata-lib-0.1.5/README.md` & `dhuodata-lib-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.1.5/setup.py` & `dhuodata-lib-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.1.5",
+    version="0.1.6",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata-lib-0.1.6/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuodata-lib-0.1.5/src/dhuolib/clients.py` & `dhuodata-lib-0.1.6/src/dhuolib/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
             ExperimentBody.model_validate(experiment_params)
             try:
                 requirements_file = open(experiment_params['requirements_file'], 'rb')
                 model_pkl = open(experiment_params['model_pkl_file'], 'rb')
             except FileNotFoundError as e:
                 logger.error(f"Error: {e}")
                 return {"error": str(e)}
-
+            
             files = {
-                'requirements': ('requirements.txt', requirements_file, 'text/plain'),
-                'model': ('model.pkl', model_pkl, 'application/octet-stream')
+                'requirements_file': ('requirements.txt', requirements_file, 'text/plain'),
+                'model_pkl_file': ('model.pkl', model_pkl, 'application/octet-stream')
             }
 
             response = self.service.create_experiment_by_conf_json(
                 experiment_params=experiment_params,
                 files=files)
 
             experiment = response.json()
```

### Comparing `dhuodata-lib-0.1.5/src/dhuolib/predict.py` & `dhuodata-lib-0.1.6/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.1.5/src/dhuolib/services.py` & `dhuodata-lib-0.1.6/src/dhuolib/services.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     def create_experiment_by_conf_json(self, experiment_params, files):
         if experiment_params is None and isinstance(experiment_params, dict):
             raise ValueError("json_data must be a dict")
 
         response = requests.post(
             f"{self.service_endpoint}/save",
             data=json.dumps(experiment_params),
-            files=files,
-            headers=self.headers,
+            files=files
         )
         return response
 
     def run_experiment(self, run_params, files=None):
         if run_params is None and isinstance(run_params, str):
             raise ValueError("json_data must be a dict")
         if files:
```

### Comparing `dhuodata-lib-0.1.5/src/dhuolib/validations.py` & `dhuodata-lib-0.1.6/src/dhuolib/validations.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.1.5/tests/test_dhuolib.py` & `dhuodata-lib-0.1.6/tests/test_dhuolib.py`

 * *Files identical despite different names*

