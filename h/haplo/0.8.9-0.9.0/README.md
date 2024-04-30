# Comparing `tmp/haplo-0.8.9.tar.gz` & `tmp/haplo-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haplo-0.8.9.tar", max compression
+gzip compressed data, was "haplo-0.9.0.tar", max compression
```

## Comparing `haplo-0.8.9.tar` & `haplo-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      634 2024-02-10 15:51:45.380419 haplo-0.8.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-06 19:11:59.663820 haplo-0.8.9/readme.md
--rw-r--r--   0        0        0        0 2023-10-29 03:30:08.510519 haplo-0.8.9/src/haplo/__init__.py
--rw-r--r--   0        0        0     3187 2023-11-06 19:11:59.664797 haplo-0.8.9/src/haplo/data_column_name.py
--rw-r--r--   0        0        0     1872 2023-12-09 16:00:51.503610 haplo-0.8.9/src/haplo/data_paths.py
--rw-r--r--   0        0        0     5184 2024-01-27 18:20:10.214978 haplo-0.8.9/src/haplo/data_preparation.py
--rw-r--r--   0        0        0     1841 2024-01-25 19:37:00.546565 haplo-0.8.9/src/haplo/distributed.py
--rw-r--r--   0        0        0     1619 2024-01-16 16:22:12.552243 haplo-0.8.9/src/haplo/export_onnx.py
--rw-r--r--   0        0        0      990 2024-02-10 15:51:45.381417 haplo-0.8.9/src/haplo/logging.py
--rw-r--r--   0        0        0     1530 2023-10-29 03:30:08.511300 haplo-0.8.9/src/haplo/losses.py
--rw-r--r--   0        0        0     8431 2023-11-10 17:35:54.143511 haplo-0.8.9/src/haplo/models.py
--rw-r--r--   0        0        0     7443 2024-02-10 15:51:45.381705 haplo-0.8.9/src/haplo/nicer_dataset.py
--rw-r--r--   0        0        0     3005 2024-01-27 18:20:21.146216 haplo-0.8.9/src/haplo/nicer_parameters_to_phase_amplitudes_infer.py
--rw-r--r--   0        0        0     1627 2023-10-29 03:30:08.512183 haplo-0.8.9/src/haplo/nicer_transform.py
--rw-r--r--   0        0        0     1967 2024-01-26 21:10:54.300075 haplo-0.8.9/src/haplo/pbs_helper.py
--rw-r--r--   0        0        0     5816 2024-02-10 15:51:45.381927 haplo-0.8.9/src/haplo/rank_constant_distributed_sampler.py
--rw-r--r--   0        0        0     1138 2023-12-20 21:14:15.422006 haplo-0.8.9/src/haplo/train_hyperparameter_configuration.py
--rw-r--r--   0        0        0     1822 2024-01-27 18:54:52.415079 haplo-0.8.9/src/haplo/train_logging_configuration.py
--rw-r--r--   0        0        0    18015 2024-02-10 15:51:45.382084 haplo-0.8.9/src/haplo/train_session.py
--rw-r--r--   0        0        0      858 2024-01-21 23:58:23.710535 haplo-0.8.9/src/haplo/train_system_configuration.py
--rw-r--r--   0        0        0      355 2024-02-10 15:51:45.382323 haplo-0.8.9/src/haplo/unwrap_model.py
--rw-r--r--   0        0        0     1884 2024-01-24 23:36:20.141990 haplo-0.8.9/src/haplo/wandb_liaison.py
--rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 haplo-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0      634 2024-02-21 21:46:28.073069 haplo-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-06 19:11:59.663820 haplo-0.9.0/readme.md
+-rw-r--r--   0        0        0        0 2023-10-29 03:30:08.510519 haplo-0.9.0/src/haplo/__init__.py
+-rw-r--r--   0        0        0     3187 2023-11-06 19:11:59.664797 haplo-0.9.0/src/haplo/data_column_name.py
+-rw-r--r--   0        0        0     1872 2023-12-09 16:00:51.503610 haplo-0.9.0/src/haplo/data_paths.py
+-rw-r--r--   0        0        0     5184 2024-01-27 18:20:10.214978 haplo-0.9.0/src/haplo/data_preparation.py
+-rw-r--r--   0        0        0     1841 2024-01-25 19:37:00.546565 haplo-0.9.0/src/haplo/distributed.py
+-rw-r--r--   0        0        0     1619 2024-01-16 16:22:12.552243 haplo-0.9.0/src/haplo/export_onnx.py
+-rw-r--r--   0        0        0      990 2024-02-10 15:51:45.381417 haplo-0.9.0/src/haplo/logging.py
+-rw-r--r--   0        0        0     1530 2023-10-29 03:30:08.511300 haplo-0.9.0/src/haplo/losses.py
+-rw-r--r--   0        0        0     8431 2023-11-10 17:35:54.143511 haplo-0.9.0/src/haplo/models.py
+-rw-r--r--   0        0        0     7443 2024-02-10 15:51:45.381705 haplo-0.9.0/src/haplo/nicer_dataset.py
+-rw-r--r--   0        0        0     3005 2024-01-27 18:20:21.146216 haplo-0.9.0/src/haplo/nicer_parameters_to_phase_amplitudes_infer.py
+-rw-r--r--   0        0        0     1627 2023-10-29 03:30:08.512183 haplo-0.9.0/src/haplo/nicer_transform.py
+-rw-r--r--   0        0        0     1967 2024-01-26 21:10:54.300075 haplo-0.9.0/src/haplo/pbs_helper.py
+-rw-r--r--   0        0        0     5816 2024-02-10 15:51:45.381927 haplo-0.9.0/src/haplo/rank_constant_distributed_sampler.py
+-rw-r--r--   0        0        0     1138 2023-12-20 21:14:15.422006 haplo-0.9.0/src/haplo/train_hyperparameter_configuration.py
+-rw-r--r--   0        0        0     2041 2024-02-21 21:38:50.754520 haplo-0.9.0/src/haplo/train_logging_configuration.py
+-rw-r--r--   0        0        0    18379 2024-02-21 21:38:50.754717 haplo-0.9.0/src/haplo/train_session.py
+-rw-r--r--   0        0        0      858 2024-01-21 23:58:23.710535 haplo-0.9.0/src/haplo/train_system_configuration.py
+-rw-r--r--   0        0        0      355 2024-02-10 15:51:45.382323 haplo-0.9.0/src/haplo/unwrap_model.py
+-rw-r--r--   0        0        0     1884 2024-01-24 23:36:20.141990 haplo-0.9.0/src/haplo/wandb_liaison.py
+-rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 haplo-0.9.0/PKG-INFO
```

### Comparing `haplo-0.8.9/pyproject.toml` & `haplo-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "haplo"
-version = "0.8.9"
+version = "0.9.0"
 description = ""
 authors = ["golmschenk <greg@olmschenk.com>"]
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
 stringcase = "^1.2.0"
```

### Comparing `haplo-0.8.9/src/haplo/data_column_name.py` & `haplo-0.9.0/src/haplo/data_column_name.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/data_paths.py` & `haplo-0.9.0/src/haplo/data_paths.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/data_preparation.py` & `haplo-0.9.0/src/haplo/data_preparation.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/distributed.py` & `haplo-0.9.0/src/haplo/distributed.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/export_onnx.py` & `haplo-0.9.0/src/haplo/export_onnx.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/logging.py` & `haplo-0.9.0/src/haplo/logging.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/losses.py` & `haplo-0.9.0/src/haplo/losses.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/models.py` & `haplo-0.9.0/src/haplo/models.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/nicer_dataset.py` & `haplo-0.9.0/src/haplo/nicer_dataset.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/nicer_parameters_to_phase_amplitudes_infer.py` & `haplo-0.9.0/src/haplo/nicer_parameters_to_phase_amplitudes_infer.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/nicer_transform.py` & `haplo-0.9.0/src/haplo/nicer_transform.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/pbs_helper.py` & `haplo-0.9.0/src/haplo/pbs_helper.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/rank_constant_distributed_sampler.py` & `haplo-0.9.0/src/haplo/rank_constant_distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/train_hyperparameter_configuration.py` & `haplo-0.9.0/src/haplo/train_hyperparameter_configuration.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/train_logging_configuration.py` & `haplo-0.9.0/src/haplo/train_logging_configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 import os
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict
 
 
@@ -14,21 +16,23 @@
     :ivar wandb_entity: The wandb entity to log to.
     :ivar additional_log_dictionary: The dictionary of additional values to log.
     """
     wandb_project: str
     wandb_entity: str
     additional_log_dictionary: Dict[str, Any]
     session_directory: Path
+    model_save_cycle_frequency: int | None = None
 
     @classmethod
     def new(cls,
             wandb_project: str = 'ramjet',
             wandb_entity: str = 'example',
             additional_log_dictionary: Dict[str, Any] | None = None,
-            session_directory: Path | None = None):
+            session_directory: Path | None = None,
+            model_save_cycle_frequency: int | None = None):
         if additional_log_dictionary is None:
             additional_log_dictionary = {}
         session_directory_environment_variable = os.environ.get('HAPLO_SESSION_DIRECTORY')
         if session_directory_environment_variable is not None and session_directory is not None:
             raise ValueError(f'Passing a `session_directory` is not allowed when the environment variable '
                              f'`HAPLO_SESSION_DIRECTORY` is set.')
         session_directory = session_directory_environment_variable
@@ -36,8 +40,9 @@
             datetime_string = datetime.datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
             session_directory = Path(f'sessions/{datetime_string}')
         if isinstance(session_directory, str):
             session_directory = Path(session_directory)
         return cls(wandb_project=wandb_project,
                    wandb_entity=wandb_entity,
                    additional_log_dictionary=additional_log_dictionary,
-                   session_directory=session_directory)
+                   session_directory=session_directory,
+                   model_save_cycle_frequency=model_save_cycle_frequency)
```

### Comparing `haplo-0.8.9/src/haplo/train_session.py` & `haplo-0.9.0/src/haplo/train_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,21 @@
                     world_size=world_size)
         validation_cycle_loss = validation_phase(validation_dataloader, model, loss_function,
                                                  network_device=network_device,
                                                  loss_device=loss_device, cycle=cycle,
                                                  metric_functions=metric_functions,
                                                  process_rank=process_rank, world_size=world_size)
         save_state(model, optimizer, logging_configuration, state_name_prefix='latest', process_rank=process_rank)
+        if (
+                logging_configuration.model_save_cycle_frequency is not None and
+                cycle != 0 and
+                cycle % logging_configuration.model_save_cycle_frequency == 0
+        ):
+            save_state(model, optimizer, logging_configuration, state_name_prefix=f'cycle_{cycle}',
+                       process_rank=process_rank)
         if validation_cycle_loss < lowest_validation_cycle_loss:
             lowest_validation_cycle_loss = validation_cycle_loss
             save_state(model, optimizer, logging_configuration, state_name_prefix='lowest_validation',
                        process_rank=process_rank)
         wandb_log('epoch', cycle, process_rank=process_rank)
         wandb_log('cycle', cycle, process_rank=process_rank)
         wandb_commit(process_rank=process_rank)
```

### Comparing `haplo-0.8.9/src/haplo/train_system_configuration.py` & `haplo-0.9.0/src/haplo/train_system_configuration.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/src/haplo/wandb_liaison.py` & `haplo-0.9.0/src/haplo/wandb_liaison.py`

 * *Files identical despite different names*

### Comparing `haplo-0.8.9/PKG-INFO` & `haplo-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haplo
-Version: 0.8.9
+Version: 0.9.0
 Summary: 
 Author: golmschenk
 Author-email: greg@olmschenk.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

