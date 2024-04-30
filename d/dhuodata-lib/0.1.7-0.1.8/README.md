# Comparing `tmp/dhuodata-lib-0.1.7.tar.gz` & `tmp/dhuodata-lib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata-lib-0.1.7.tar", last modified: Tue Apr 30 01:58:55 2024, max compression
+gzip compressed data, was "dhuodata-lib-0.1.8.tar", last modified: Tue Apr 30 02:12:15 2024, max compression
```

## Comparing `dhuodata-lib-0.1.7.tar` & `dhuodata-lib-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 01:58:55.556068 dhuodata-lib-0.1.7/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-30 01:58:55.552068 dhuodata-lib-0.1.7/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.1.7/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-30 01:58:55.556068 dhuodata-lib-0.1.7/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-30 01:58:50.000000 dhuodata-lib-0.1.7/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 01:58:55.552068 dhuodata-lib-0.1.7/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 01:58:55.552068 dhuodata-lib-0.1.7/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     2528 2024-04-30 01:58:55.000000 dhuodata-lib-0.1.7/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-04-30 01:58:55.000000 dhuodata-lib-0.1.7/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-30 01:58:55.000000 dhuodata-lib-0.1.7/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-04-30 01:58:55.000000 dhuodata-lib-0.1.7/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-30 01:58:55.000000 dhuodata-lib-0.1.7/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 01:58:55.552068 dhuodata-lib-0.1.7/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata-lib-0.1.7/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata-lib-0.1.7/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     4135 2024-04-30 01:58:21.000000 dhuodata-lib-0.1.7/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata-lib-0.1.7/src/dhuolib/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata-lib-0.1.7/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1341 2024-04-30 01:55:04.000000 dhuodata-lib-0.1.7/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      750 2024-04-29 11:53:52.000000 dhuodata-lib-0.1.7/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata-lib-0.1.7/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 01:58:55.552068 dhuodata-lib-0.1.7/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2540 2024-04-29 12:52:51.000000 dhuodata-lib-0.1.7/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 02:12:15.468085 dhuodata-lib-0.1.8/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-30 02:12:15.468085 dhuodata-lib-0.1.8/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.1.8/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-30 02:12:15.468085 dhuodata-lib-0.1.8/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-30 02:12:09.000000 dhuodata-lib-0.1.8/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 02:12:15.468085 dhuodata-lib-0.1.8/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 02:12:15.468085 dhuodata-lib-0.1.8/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     2528 2024-04-30 02:12:15.000000 dhuodata-lib-0.1.8/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-04-30 02:12:15.000000 dhuodata-lib-0.1.8/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-30 02:12:15.000000 dhuodata-lib-0.1.8/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-04-30 02:12:15.000000 dhuodata-lib-0.1.8/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-30 02:12:15.000000 dhuodata-lib-0.1.8/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 02:12:15.468085 dhuodata-lib-0.1.8/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata-lib-0.1.8/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata-lib-0.1.8/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     4125 2024-04-30 02:11:57.000000 dhuodata-lib-0.1.8/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata-lib-0.1.8/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata-lib-0.1.8/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1341 2024-04-30 01:55:04.000000 dhuodata-lib-0.1.8/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      750 2024-04-29 11:53:52.000000 dhuodata-lib-0.1.8/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata-lib-0.1.8/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 02:12:15.468085 dhuodata-lib-0.1.8/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2540 2024-04-29 12:52:51.000000 dhuodata-lib-0.1.8/tests/test_dhuolib.py
```

### Comparing `dhuodata-lib-0.1.7/PKG-INFO` & `dhuodata-lib-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.1.7
+Version: 0.1.8
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuodata-lib-0.1.7/README.md` & `dhuodata-lib-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.1.7/setup.py` & `dhuodata-lib-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.1.7",
+    version="0.1.8",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata-lib-0.1.7/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata-lib-0.1.8/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.1.7
+Version: 0.1.8
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuodata-lib-0.1.7/src/dhuolib/clients.py` & `dhuodata-lib-0.1.8/src/dhuolib/clients.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         if not service_endpoint:
             raise ValueError("service_endpoint is required")
 
         self.service = ServiceAPIML(service_endpoint)
 
     def create_experiment(self, experiment_params: dict) -> dict:
         try:
-            ExperimentBody.model_validate(experiment_params)
+            ExperimentBody.parse_obj(experiment_params)
             files = {}
             try:
                 files = {
                     'requirements_file': ('requirements.txt', open(experiment_params['requirements_file'], 'rb'), 'text/plain'),
                     'model_pkl_file': ('model.pkl', open(experiment_params['model_pkl_file'], 'rb'), 'application/octet-stream')
                 }
                 print(experiment_params)
@@ -38,15 +38,15 @@
             return experiment
         except ValidationError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
 
     def run_experiment(self, run_params) -> dict:
         try:
-            RunExperimentBody.model_validate(run_params)
+            RunExperimentBody.parse_obj(run_params)
             if run_params["experiment_id"] is None:
                 experiment_id = self.create_experiment(run_params)
                 run_params["experiment_id"] = experiment_id
 
             response = self.service.run_experiment(run_params)
             logger.info(f"Experiment ID: {run_params['experiment_id']} running")
             return response.json()
```

### Comparing `dhuodata-lib-0.1.7/src/dhuolib/predict.py` & `dhuodata-lib-0.1.8/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.1.7/src/dhuolib/services.py` & `dhuodata-lib-0.1.8/src/dhuolib/services.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.1.7/src/dhuolib/validations.py` & `dhuodata-lib-0.1.8/src/dhuolib/validations.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.1.7/tests/test_dhuolib.py` & `dhuodata-lib-0.1.8/tests/test_dhuolib.py`

 * *Files identical despite different names*

