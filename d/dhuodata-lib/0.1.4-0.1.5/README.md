# Comparing `tmp/dhuodata_lib-0.1.4.tar.gz` & `tmp/dhuodata-lib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata_lib-0.1.4.tar", last modified: Thu Apr 25 13:54:28 2024, max compression
+gzip compressed data, was "dhuodata-lib-0.1.5.tar", last modified: Mon Apr 29 18:42:51 2024, max compression
```

## Comparing `dhuodata_lib-0.1.4.tar` & `dhuodata-lib-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,23 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-25 13:54:28.617021 dhuodata_lib-0.1.4/
--rw-r--r--   0 diego     (1000) diego     (1000)     2983 2024-04-25 13:54:28.617021 dhuodata_lib-0.1.4/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.1.4/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-25 13:54:28.617021 dhuodata_lib-0.1.4/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-25 13:53:45.000000 dhuodata_lib-0.1.4/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-25 13:54:28.613021 dhuodata_lib-0.1.4/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-25 13:54:28.613021 dhuodata_lib-0.1.4/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     2983 2024-04-25 13:54:28.000000 dhuodata_lib-0.1.4/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      489 2024-04-25 13:54:28.000000 dhuodata_lib-0.1.4/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-25 13:54:28.000000 dhuodata_lib-0.1.4/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      128 2024-04-25 13:54:28.000000 dhuodata_lib-0.1.4/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-25 13:54:28.000000 dhuodata_lib-0.1.4/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-25 13:54:28.613021 dhuodata_lib-0.1.4/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.1.4/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.1.4/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     3847 2024-04-24 22:37:49.000000 dhuodata_lib-0.1.4/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      358 2024-04-23 16:51:37.000000 dhuodata_lib-0.1.4/src/dhuolib/config.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-25 13:54:28.613021 dhuodata_lib-0.1.4/src/dhuolib/oci_tools/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:52:32.000000 dhuodata_lib-0.1.4/src/dhuolib/oci_tools/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      716 2024-04-24 18:22:15.000000 dhuodata_lib-0.1.4/src/dhuolib/oci_tools/utils.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.1.4/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1087 2024-04-23 16:51:03.000000 dhuodata_lib-0.1.4/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      761 2024-04-25 13:51:55.000000 dhuodata_lib-0.1.4/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.1.4/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-25 13:54:28.613021 dhuodata_lib-0.1.4/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     3491 2024-04-25 13:54:25.000000 dhuodata_lib-0.1.4/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.1.5/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-29 18:42:03.000000 dhuodata-lib-0.1.5/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     2528 2024-04-29 18:42:51.000000 dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-04-29 18:42:51.000000 dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-29 18:42:51.000000 dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-04-29 18:42:51.000000 dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-29 18:42:51.000000 dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata-lib-0.1.5/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata-lib-0.1.5/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     4134 2024-04-29 12:51:47.000000 dhuodata-lib-0.1.5/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata-lib-0.1.5/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata-lib-0.1.5/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1388 2024-04-29 11:48:37.000000 dhuodata-lib-0.1.5/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      750 2024-04-29 11:53:52.000000 dhuodata-lib-0.1.5/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata-lib-0.1.5/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-29 18:42:51.976436 dhuodata-lib-0.1.5/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2540 2024-04-29 12:52:51.000000 dhuodata-lib-0.1.5/tests/test_dhuolib.py
```

### Comparing `dhuodata_lib-0.1.4/PKG-INFO` & `dhuodata-lib-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
-Requires-Dist: mlflow
-Requires-Dist: oci==2.125.3
 Provides-Extra: interactive
-Requires-Dist: mypy==1.5.1; extra == "interactive"
-Requires-Dist: flake8==6.1.0; extra == "interactive"
-Requires-Dist: black==22.3.0; extra == "interactive"
-Requires-Dist: pytest-cov~=4.0; extra == "interactive"
-Requires-Dist: pytest~=7.0; extra == "interactive"
-Requires-Dist: twine; extra == "interactive"
-Requires-Dist: wheel; extra == "interactive"
-Requires-Dist: oci==2.125.3; extra == "interactive"
 
 # DHuO LIb
 
 ## Board
 
 ![](assets/imgs/board.png)
```

### Comparing `dhuodata_lib-0.1.4/README.md` & `dhuodata-lib-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.1.4/setup.py` & `dhuodata-lib-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.1.4",
+    version="0.1.5",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata_lib-0.1.4/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata-lib-0.1.5/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
-Requires-Dist: mlflow
-Requires-Dist: oci==2.125.3
 Provides-Extra: interactive
-Requires-Dist: mypy==1.5.1; extra == "interactive"
-Requires-Dist: flake8==6.1.0; extra == "interactive"
-Requires-Dist: black==22.3.0; extra == "interactive"
-Requires-Dist: pytest-cov~=4.0; extra == "interactive"
-Requires-Dist: pytest~=7.0; extra == "interactive"
-Requires-Dist: twine; extra == "interactive"
-Requires-Dist: wheel; extra == "interactive"
-Requires-Dist: oci==2.125.3; extra == "interactive"
 
 # DHuO LIb
 
 ## Board
 
 ![](assets/imgs/board.png)
```

### Comparing `dhuodata_lib-0.1.4/src/dhuolib/clients.py` & `dhuodata-lib-0.1.5/src/dhuolib/clients.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,64 @@
 from pydantic import ValidationError
 
 from dhuolib.config import logger
-from dhuolib.oci_tools.utils import OCIUtils
 from dhuolib.services import ServiceAPIML
 from dhuolib.validations import ExperimentBody, RunExperimentBody
 
 
 class DhuolibClient:
-    def __init__(self, service_endpoint=None, config_file_path='~/.oci/config'):
+    def __init__(self, service_endpoint=None):
         if not service_endpoint:
             raise ValueError("service_endpoint is required")
 
         self.service = ServiceAPIML(service_endpoint)
-        self.oci = OCIUtils(config_file_path=config_file_path)
 
     def create_experiment(self, experiment_params: dict) -> dict:
         try:
-            ExperimentBody.parse_obj(experiment_params)
+            ExperimentBody.model_validate(experiment_params)
+            try:
+                requirements_file = open(experiment_params['requirements_file'], 'rb')
+                model_pkl = open(experiment_params['model_pkl_file'], 'rb')
+            except FileNotFoundError as e:
+                logger.error(f"Error: {e}")
+                return {"error": str(e)}
+
+            files = {
+                'requirements': ('requirements.txt', requirements_file, 'text/plain'),
+                'model': ('model.pkl', model_pkl, 'application/octet-stream')
+            }
+
+            response = self.service.create_experiment_by_conf_json(
+                experiment_params=experiment_params,
+                files=files)
+
+            experiment = response.json()
+            logger.info(
+                f"Experiment Name: {experiment_params['experiment_name']}"
+                f"Experiment ID: {experiment['experiment_id']} created"
+            )
+            return experiment
         except ValidationError as e:
             logger.error(f"Error: {e}")
-            raise e
-
-        self.oci.upload_file(
-            file_path=experiment_params["file"]["filepath"],
-            bucket_name=experiment_params["file"]["bucket"],
-            namespace=experiment_params["file"]["namespace"]
-        )
-
-        response = self.service.create_experiment_by_conf_json(experiment_params)
-        experiment = response.json()
-        logger.info(
-            f"Experiment Name: {experiment_params['experiment_name']}"
-            f"Experiment ID: {experiment['experiment_id']} created"
-        )
-        return experiment
+            return {"error": str(e)}
 
     def run_experiment(self, run_params) -> dict:
         try:
-            RunExperimentBody.parse_obj(run_params)
+            RunExperimentBody.model_validate(run_params)
+            if run_params["experiment_id"] is None:
+                experiment_id = self.create_experiment(run_params)
+                run_params["experiment_id"] = experiment_id
+
+            response = self.service.run_experiment(run_params)
+            logger.info(f"Experiment ID: {run_params['experiment_id']} running")
+            return response.json()
         except ValidationError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
 
-        if run_params["experiment_id"] is None:
-            experiment_id = self.create_experiment(run_params)
-            run_params["experiment_id"] = experiment_id
-
-        response = self.service.run_experiment(run_params)
-        logger.info(f"Experiment ID: {run_params['experiment_id']} running")
-        return response.json()
-
     def load_model(self, model_name, tag) -> str:
         print("loading model")
         return "model_name.pkl"
 
     def predict(self):
         pass
```

### Comparing `dhuodata_lib-0.1.4/src/dhuolib/predict.py` & `dhuodata-lib-0.1.5/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.1.4/src/dhuolib/services.py` & `dhuodata-lib-0.1.5/src/dhuolib/services.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,27 +8,37 @@
 
         if not isinstance(service_endpoint, str):
             raise ValueError("service_endpoint must be a string")
 
         self.service_endpoint = f"{service_endpoint}/api/experiment"
         self.headers = {"Content-Type": "application/json"}
 
-    def create_experiment_by_conf_json(self, experiment_params):
+    def create_experiment_by_conf_json(self, experiment_params, files):
         if experiment_params is None and isinstance(experiment_params, dict):
             raise ValueError("json_data must be a dict")
 
         response = requests.post(
             f"{self.service_endpoint}/save",
             data=json.dumps(experiment_params),
+            files=files,
             headers=self.headers,
         )
         return response
 
-    def run_experiment(self, run_params):
+    def run_experiment(self, run_params, files=None):
         if run_params is None and isinstance(run_params, str):
             raise ValueError("json_data must be a dict")
+        if files:
+            response = requests.post(
+                f"{self.service_endpoint}/run",
+                data=json.dumps(run_params),
+                headers=self.headers,
+                files=files
+            )
+            return response
+
         response = requests.post(
             f"{self.service_endpoint}/run",
             data=json.dumps(run_params),
-            headers=self.headers,
+            headers=self.headers
         )
         return response
```

### Comparing `dhuodata_lib-0.1.4/tests/test_dhuolib.py` & `dhuodata-lib-0.1.5/tests/test_dhuolib.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,68 @@
 import json
+import sys
 import unittest
 from unittest.mock import MagicMock, patch
-import sys
-import pytest
-from pydantic import ValidationError
 
 sys.path.append("src")
 from dhuolib.clients import DhuolibClient
 
 
 class TestDhuolibUtils(unittest.TestCase):
     def setUp(self):
         self.end_point = "http://fake-endpoint"
         self.dhuolib = DhuolibClient(service_endpoint=self.end_point)
         self.namespace = "engdb"
         self.bucket_name = "dhuodata-mlops"
         self.file_path = "tests/files/LogisticRegression_best.pickle"
-        self.experiment_id = None
 
     def test_deve_lancar_excecao_com_valores_run_params_incorretos(self):
-        experiments_params = {
-            "file": {
-                "bucket": self.bucket_name,
-                "filepath": self.file_path,
-            },
+        experiment_params = {
+            "experiment_name": "test_experiment",
+            "experiment_tags": {"version": "v1", "priority": "P1"}
         }
-
-        with pytest.raises(ValidationError):
-            self.dhuolib.create_experiment(experiments_params)
+        response = self.dhuolib.create_experiment(experiment_params)
+        self.assertEqual(list(response.keys()), ["error"])
 
     @patch("requests.post")
-    @patch('dhuolib.clients.OCIUtils')
-    def test_deve_criar_o_experimento_com_run_params_corretos(self, mock_oci_utils, mock_post):
-        client = DhuolibClient(service_endpoint="http://fake-endpoint")
+    def test_deve_criar_o_experimento_com_run_params_corretos(
+        self, mock_post
+    ):
+        client = DhuolibClient(service_endpoint=self.end_point)
 
         mock_response = mock_post.return_value
         mock_response.status_code = 201
         mock_response.json.return_value = {"experiment_id": "1"}
 
-        mock_oci = mock_oci_utils.return_value
-        mock_oci.upload_file = MagicMock()
-
         experiment_params = {
             "experiment_name": "test_experiment",
             "experiment_tags": {"version": "v1", "priority": "P1"},
-            "file": {
-                "bucket": "example_bucket",
-                "namespace": "example_namespace",
-                "filepath": "tests/files/LogisticRegression_best.pickle"
-            }
+            "model_pkl_file": "tests/files/LogisticRegression_best.pickle",
+            "requirements_file": "tests/files/requirements.txt"
         }
-
+        
         response = client.create_experiment(experiment_params)
-
-        mock_oci.upload_file.assert_called_once_with(
-            file_path="tests/files/LogisticRegression_best.pickle",
-            bucket_name="example_bucket",
-            namespace="example_namespace"
-        )
-
         self.assertEqual(response, mock_response.json.return_value)
-
-        mock_post.assert_called_once_with(
-            "http://fake-endpoint/api/experiment/save",
-            data=json.dumps(experiment_params),
-            headers={"Content-Type": "application/json"},
-        )
-
+        
     @patch("requests.post")
     def test_deve_executar_o_experimento_com_run_params_corretos(self, mock_post):
         mock_response = mock_post.return_value
         mock_response.status_code = 201
         mock_response.json.return_value = {
             "current_stage": "Production",
             "last_updated_timestamp": 1713582060414,
             "model_version": "1",
             "run_id": "9434e517ed104958b6f5f47d33c79184",
             "status": "READY",
         }
 
         run_params = {
-            "experiment_id": 2,
+            "experiment_id": '2',
             "stage": "Production",
             "modelname": "nlp_framework",
             "modeltag": "v1",
-            "file": {
-                "bucket": self.bucket_name,
-                "namespace": self.namespace,
-                "filepath": "LogisticRegression_best.pickle",
-            },
+            "model_pkl_file": "tests/files/LogisticRegression_best.pickle",
+            "requirements_file": "tests/files/requirements.txt"
         }
         response = self.dhuolib.run_experiment(run_params)
 
-        self.assertEqual(response, mock_response.json.return_value)
-
-        mock_post.assert_called_once_with(
-            "http://fake-endpoint/api/experiment/run",
-            data=json.dumps(run_params),
-            headers={"Content-Type": "application/json"},
-        )
+        self.assertEqual(response, mock_response.json.return_value)
```

