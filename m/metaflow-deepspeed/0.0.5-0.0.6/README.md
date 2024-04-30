# Comparing `tmp/metaflow-deepspeed-0.0.5.tar.gz` & `tmp/metaflow_deepspeed-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-deepspeed-0.0.5.tar", last modified: Wed Mar 27 20:53:29 2024, max compression
+gzip compressed data, was "metaflow_deepspeed-0.0.6.tar", last modified: Tue Apr 30 21:47:41 2024, max compression
```

## Comparing `metaflow-deepspeed-0.0.5.tar` & `metaflow_deepspeed-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,39 @@
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-03-27 20:53:29.080132 metaflow-deepspeed-0.0.5/
--rw-r--r--   0 eddie      (501) staff       (20)    11348 2023-10-12 22:01:35.000000 metaflow-deepspeed-0.0.5/LICENSE
--rw-r--r--   0 eddie      (501) staff       (20)      199 2024-03-27 20:53:29.079929 metaflow-deepspeed-0.0.5/PKG-INFO
--rw-r--r--   0 eddie      (501) staff       (20)     4072 2024-03-13 21:45:36.000000 metaflow-deepspeed-0.0.5/README.md
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-03-27 20:53:29.079724 metaflow-deepspeed-0.0.5/metaflow_deepspeed.egg-info/
--rw-r--r--   0 eddie      (501) staff       (20)      199 2024-03-27 20:53:29.000000 metaflow-deepspeed-0.0.5/metaflow_deepspeed.egg-info/PKG-INFO
--rw-r--r--   0 eddie      (501) staff       (20)      902 2024-03-27 20:53:29.000000 metaflow-deepspeed-0.0.5/metaflow_deepspeed.egg-info/SOURCES.txt
--rw-r--r--   0 eddie      (501) staff       (20)        1 2024-03-27 20:53:29.000000 metaflow-deepspeed-0.0.5/metaflow_deepspeed.egg-info/dependency_links.txt
--rw-r--r--   0 eddie      (501) staff       (20)       20 2024-03-27 20:53:29.000000 metaflow-deepspeed-0.0.5/metaflow_deepspeed.egg-info/top_level.txt
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-03-27 20:53:29.075667 metaflow-deepspeed-0.0.5/metaflow_extensions/
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-03-27 20:53:29.075720 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-03-27 20:53:29.077780 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/
--rw-r--r--   0 eddie      (501) staff       (20)     6404 2024-03-13 21:45:36.000000 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/az_store.py
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-03-27 20:53:29.079496 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/
--rw-r--r--   0 eddie      (501) staff       (20)        0 2024-03-13 21:45:36.000000 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/__init__.py
--rw-r--r--   0 eddie      (501) staff       (20)      436 2024-03-13 21:45:36.000000 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/constants.py
--rw-r--r--   0 eddie      (501) staff       (20)     7950 2024-03-13 21:45:36.000000 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/datastore.py
--rw-r--r--   0 eddie      (501) staff       (20)     3230 2024-03-13 21:45:36.000000 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/deepspeed_decorator.py
--rw-r--r--   0 eddie      (501) staff       (20)     2332 2024-03-13 21:45:36.000000 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/exceptions.py
--rw-r--r--   0 eddie      (501) staff       (20)    13101 2024-03-27 19:24:24.000000 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/executor.py
--rw-r--r--   0 eddie      (501) staff       (20)    10663 2024-03-14 00:20:19.000000 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/mpi_setup.py
--rw-r--r--   0 eddie      (501) staff       (20)     3754 2024-03-13 21:45:36.000000 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/status_notifier.py
--rw-r--r--   0 eddie      (501) staff       (20)     9112 2024-03-13 21:45:36.000000 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/hf_callbacks.py
--rw-r--r--   0 eddie      (501) staff       (20)      178 2024-03-13 21:45:36.000000 metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/mfextinit_deepspeed.py
--rw-r--r--   0 eddie      (501) staff       (20)       38 2024-03-27 20:53:29.080180 metaflow-deepspeed-0.0.5/setup.cfg
--rw-r--r--   0 eddie      (501) staff       (20)      424 2024-03-27 20:50:14.000000 metaflow-deepspeed-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:47:41.625471 metaflow_deepspeed-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-30 21:47:41.625471 metaflow_deepspeed-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:47:41.625471 metaflow_deepspeed-0.0.6/metaflow_deepspeed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-30 21:47:41.000000 metaflow_deepspeed-0.0.6/metaflow_deepspeed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-30 21:47:41.000000 metaflow_deepspeed-0.0.6/metaflow_deepspeed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:47:41.000000 metaflow_deepspeed-0.0.6/metaflow_deepspeed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 21:47:41.000000 metaflow_deepspeed-0.0.6/metaflow_deepspeed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:47:41.617471 metaflow_deepspeed-0.0.6/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:47:41.621471 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:47:41.621471 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/az_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:47:41.621471 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:47:41.621471 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/card_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/card_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/card_utilities/async_cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/card_utilities/extra_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/card_utilities/injector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/deepspeed_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:47:41.625471 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/hugging_face/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/hugging_face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/hugging_face/card_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/hugging_face/card_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/hugging_face/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10663 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/mpi_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/status_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/hf_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/mfextinit_deepspeed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:47:41.625471 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/toplevel/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/toplevel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/toplevel/toplevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 21:47:41.625471 metaflow_deepspeed-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-30 21:47:31.000000 metaflow_deepspeed-0.0.6/setup.py
```

### Comparing `metaflow-deepspeed-0.0.5/LICENSE` & `metaflow_deepspeed-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-deepspeed-0.0.5/README.md` & `metaflow_deepspeed-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-deepspeed-0.0.5/metaflow_deepspeed.egg-info/SOURCES.txt` & `metaflow_deepspeed-0.0.6/metaflow_deepspeed.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,8 +11,18 @@
 metaflow_extensions/deepspeed/plugins/deepspeed_libs/__init__.py
 metaflow_extensions/deepspeed/plugins/deepspeed_libs/constants.py
 metaflow_extensions/deepspeed/plugins/deepspeed_libs/datastore.py
 metaflow_extensions/deepspeed/plugins/deepspeed_libs/deepspeed_decorator.py
 metaflow_extensions/deepspeed/plugins/deepspeed_libs/exceptions.py
 metaflow_extensions/deepspeed/plugins/deepspeed_libs/executor.py
 metaflow_extensions/deepspeed/plugins/deepspeed_libs/mpi_setup.py
-metaflow_extensions/deepspeed/plugins/deepspeed_libs/status_notifier.py
+metaflow_extensions/deepspeed/plugins/deepspeed_libs/status_notifier.py
+metaflow_extensions/deepspeed/plugins/deepspeed_libs/card_utilities/__init__.py
+metaflow_extensions/deepspeed/plugins/deepspeed_libs/card_utilities/async_cards.py
+metaflow_extensions/deepspeed/plugins/deepspeed_libs/card_utilities/extra_components.py
+metaflow_extensions/deepspeed/plugins/deepspeed_libs/card_utilities/injector.py
+metaflow_extensions/deepspeed/plugins/deepspeed_libs/hugging_face/__init__.py
+metaflow_extensions/deepspeed/plugins/deepspeed_libs/hugging_face/card_callback.py
+metaflow_extensions/deepspeed/plugins/deepspeed_libs/hugging_face/card_decorator.py
+metaflow_extensions/deepspeed/plugins/deepspeed_libs/hugging_face/constants.py
+metaflow_extensions/deepspeed/toplevel/__init__.py
+metaflow_extensions/deepspeed/toplevel/toplevel.py
```

### Comparing `metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/az_store.py` & `metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/az_store.py`

 * *Files identical despite different names*

### Comparing `metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/datastore.py` & `metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/deepspeed_decorator.py` & `metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/deepspeed_decorator.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from metaflow.plugins.parallel_decorator import (
     ParallelDecorator,
     _local_multinode_control_task_step_func,
 )
 
 from .executor import DeepspeedExecutor
 from .mpi_setup import setup_mpi_env
+import os
 
 """
 Control Flow : 
 1. Task pre-step sets the UBF Context. 
 2. The @parallel decorator mutates the step function based because it task decorates. 
     - This mutation is essential because, we are running the actual user code differently for each task based on the type of task (worker / control).
     - The `@parallel` decorator exposes a `setup_distributed_env` method that is called by the `@deepspeed` decorator to set up the distributed environment.
@@ -50,22 +51,30 @@
         )
 
     def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
 
         self.environment = environment
         self.flow_datastore = flow_datastore
 
-        for deco in decos: 
+        for deco in decos:
             if deco.name in ["resources", "kubernetes", "batch"]:
-                if deco.attributes['gpu']:
+                if deco.attributes["gpu"]:
                     self.is_gpu = True
-                    self.n_slots = deco.attributes['gpu']
+                    self.n_slots = deco.attributes["gpu"]
                 else:
                     self.is_gpu = False
-                    self.n_slots = deco.attributes['cpu']
+                    self.n_slots = deco.attributes["cpu"]
+            # Since Netflix/metaflow#1775 and Netflix/metaflow#1776 add the
+            # port and the `jobsets` implementation without services, we
+            # can just go about setting the port to 22 if it is not set.
+            # If the older implementation with `requires_passwordless_ssh` is
+            # if being used then as a fallback the attribute will still exist.
+            if deco.name == "kubernetes":
+                if "port" in deco.defaults:
+                    deco.attributes["port"] = 22
 
     def task_pre_step(
         self,
         step_name,
         task_datastore,
         metadata,
         run_id,
```

### Comparing `metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/exceptions.py` & `metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/exceptions.py`

 * *Files identical despite different names*

### Comparing `metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/executor.py` & `metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,18 @@
                 except UnicodeDecodeError:
                     text = ""
                 print(
                     text, end="", flush=True
                 )  # TODO: other mechanism to flush buffer, especially in progress bar case.
 
             if process.returncode != 0:
-                return False, process.stderr.read().decode("utf-8")
+                if process.stderr is not None:
+                    return False, process.stderr.read().decode("utf-8")
+                else:
+                    return False, None
             return True, None
 
     def _resolve_storage_paths(
         self, push_results_dir_to_cloud, datastore, local_output_dir, cloud_output_dir
     ) -> str:
         if push_results_dir_to_cloud and (
             datastore._backend.TYPE != "s3" and datastore._backend.TYPE != "azure"
```

### Comparing `metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/mpi_setup.py` & `metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/mpi_setup.py`

 * *Files identical despite different names*

### Comparing `metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/deepspeed_libs/status_notifier.py` & `metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/deepspeed_libs/status_notifier.py`

 * *Files identical despite different names*

### Comparing `metaflow-deepspeed-0.0.5/metaflow_extensions/deepspeed/plugins/hf_callbacks.py` & `metaflow_deepspeed-0.0.6/metaflow_extensions/deepspeed/plugins/hf_callbacks.py`

 * *Files identical despite different names*

