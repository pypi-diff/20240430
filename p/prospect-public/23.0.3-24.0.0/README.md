# Comparing `tmp/prospect-public-23.0.3.tar.gz` & `tmp/prospect_public-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prospect-public-23.0.3.tar", last modified: Mon Dec 18 12:34:47 2023, max compression
+gzip compressed data, was "prospect_public-24.0.0.tar", last modified: Tue Apr 30 12:08:33 2024, max compression
```

## Comparing `prospect-public-23.0.3.tar` & `prospect_public-24.0.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:34:47.571992 prospect-public-23.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2023-12-18 12:34:47.571992 prospect-public-23.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2023-12-18 12:34:26.000000 prospect-public-23.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:34:47.567992 prospect-public-23.0.3/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2023-12-18 12:34:26.000000 prospect-public-23.0.3/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:34:47.567992 prospect-public-23.0.3/prospect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:34:47.571992 prospect-public-23.0.3/prospect/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/kernels/analytical_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/kernels/base_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/kernels/cobaya_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/kernels/initialisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/kernels/montepython_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8333 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/optimiser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15719 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:34:47.571992 prospect-public-23.0.3/prospect/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22147 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/tasks/analyse_profile_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/tasks/base_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/tasks/initialise.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/tasks/initialise_optimiser_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/tasks/initialise_profile_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/tasks/mcmc_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2023-12-18 12:34:26.000000 prospect-public-23.0.3/prospect/tasks/optimise_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:34:47.571992 prospect-public-23.0.3/prospect_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2023-12-18 12:34:47.000000 prospect-public-23.0.3/prospect_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      895 2023-12-18 12:34:47.000000 prospect-public-23.0.3/prospect_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 12:34:47.000000 prospect-public-23.0.3/prospect_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-18 12:34:47.000000 prospect-public-23.0.3/prospect_public.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-18 12:34:47.000000 prospect-public-23.0.3/prospect_public.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-12-18 12:34:26.000000 prospect-public-23.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 12:34:47.571992 prospect-public-23.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-18 12:34:26.000000 prospect-public-23.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:33.146351 prospect_public-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-04-30 12:08:33.146351 prospect_public-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-04-30 12:08:16.000000 prospect_public-24.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:33.142351 prospect_public-24.0.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-30 12:08:16.000000 prospect_public-24.0.0/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:33.142351 prospect_public-24.0.0/prospect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:33.146351 prospect_public-24.0.0/prospect/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/kernels/analytical_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/kernels/base_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/kernels/cobaya_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/kernels/initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/kernels/montepython_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16341 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:33.146351 prospect_public-24.0.0/prospect/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7577 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/tasks/analyse_global_optimisation_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21382 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/tasks/analyse_profile_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/tasks/base_analyse_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/tasks/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/tasks/initialise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/tasks/initialise_optimiser_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/tasks/initialise_profile_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/tasks/mcmc_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-30 12:08:16.000000 prospect_public-24.0.0/prospect/tasks/optimise_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:33.146351 prospect_public-24.0.0/prospect_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-04-30 12:08:33.000000 prospect_public-24.0.0/prospect_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-30 12:08:33.000000 prospect_public-24.0.0/prospect_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:08:33.000000 prospect_public-24.0.0/prospect_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-30 12:08:33.000000 prospect_public-24.0.0/prospect_public.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 12:08:33.000000 prospect_public-24.0.0/prospect_public.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-30 12:08:16.000000 prospect_public-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:08:33.146351 prospect_public-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-30 12:08:16.000000 prospect_public-24.0.0/setup.py
```

### Comparing `prospect-public-23.0.3/PKG-INFO` & `prospect_public-24.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prospect-public
-Version: 23.0.3
+Version: 24.0.0
 Summary: A profile likelihood code for frequentist cosmological parameter inference
 Author-email: Emil Brinch Holm <ebholm@phys.au.dk>, Thomas Tram <thomas.tram@phys.au.dk>
 Project-URL: Homepage, https://github.com/AarhusCosmology/prospect_public
 Project-URL: Bug Tracker, https://github.com/AarhusCosmology/prospect_public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -58,14 +58,20 @@
 PROSPECT provides a quick tool to load the profile likelihood in Python as follows:
 ```
 from prospect.profile import load_profile
 profile_dict = load_profile('path_to_my_run')
 ```
 whence `profile_dict` is a dictionary with the best-fitting parameter values at each point in the profile, along with the associated likelihood values. 
 
+#### Global optimisation
+
+The efficient optimiser of PROSPECT can also be used to find global bestfits of your cosmology. An example for such an input .yaml file is found in the `input/example_toy/example_global_optimisation_toy.yaml` file. Starting from a .yaml file for a profile likelihood, you only need to change the `jobtype` input of the `run` section to 'global_optimisation' (rather than the usual 'profile'). All of the settings of the optimiser defined in the `profile` section are then used to carry out global optimisation of your model, giving an output folder similar in structure to that obtained from profile likelihoods runs. 
+
+*Note that when running with `jobtype: 'global_optimisation'`, the inputs `parameter`, `values`, `start_bin_fraction` as well as `plot_profile`, `detailed_plot`, `plot_Delta_chi2` and `confidence_levels` of the `profile` section are ignored, but the rest of the input, such as the schedules and initialisation procedures, are still used to define the settings of the optimiser.*
+
 #### Reoptimising
 
 Not satisfied with your profile? You can always queue new `OptimiseTask`s with the reoptimising feature. Add extra tasks from the terminal by running
 ```
 prospect-reoptimise -y my_reoptimise_settings.yaml -o folder_to_reoptimise (--override)
 ```
 Here, `my_reoptimise_settings.yaml` should be a yaml file similar in structure to PROSPECT input files, but only containing the "profile" substructure. For example:
```

### Comparing `prospect-public-23.0.3/README.md` & `prospect_public-24.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,20 @@
 PROSPECT provides a quick tool to load the profile likelihood in Python as follows:
 ```
 from prospect.profile import load_profile
 profile_dict = load_profile('path_to_my_run')
 ```
 whence `profile_dict` is a dictionary with the best-fitting parameter values at each point in the profile, along with the associated likelihood values. 
 
+#### Global optimisation
+
+The efficient optimiser of PROSPECT can also be used to find global bestfits of your cosmology. An example for such an input .yaml file is found in the `input/example_toy/example_global_optimisation_toy.yaml` file. Starting from a .yaml file for a profile likelihood, you only need to change the `jobtype` input of the `run` section to 'global_optimisation' (rather than the usual 'profile'). All of the settings of the optimiser defined in the `profile` section are then used to carry out global optimisation of your model, giving an output folder similar in structure to that obtained from profile likelihoods runs. 
+
+*Note that when running with `jobtype: 'global_optimisation'`, the inputs `parameter`, `values`, `start_bin_fraction` as well as `plot_profile`, `detailed_plot`, `plot_Delta_chi2` and `confidence_levels` of the `profile` section are ignored, but the rest of the input, such as the schedules and initialisation procedures, are still used to define the settings of the optimiser.*
+
 #### Reoptimising
 
 Not satisfied with your profile? You can always queue new `OptimiseTask`s with the reoptimising feature. Add extra tasks from the terminal by running
 ```
 prospect-reoptimise -y my_reoptimise_settings.yaml -o folder_to_reoptimise (--override)
 ```
 Here, `my_reoptimise_settings.yaml` should be a yaml file similar in structure to PROSPECT input files, but only containing the "profile" substructure. For example:
```

### Comparing `prospect-public-23.0.3/doc/conf.py` & `prospect_public-24.0.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `prospect-public-23.0.3/prospect/analysis.py` & `prospect_public-24.0.0/prospect/analysis.py`

 * *Files identical despite different names*

### Comparing `prospect-public-23.0.3/prospect/communication.py` & `prospect_public-24.0.0/prospect/communication.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import traceback
 from collections import defaultdict
 from datetime import datetime
 from typing import Type
 from dataclasses import dataclass
 from prospect.input import Configuration
 from prospect.tasks.base_task import BaseTask
+from prospect.tasks.base_analyse_task import BaseAnalyseTask
 from prospect.tasks.analyse_profile_task import AnalyseProfileTask
+from prospect.tasks.analyse_global_optimisation_task import AnalyseGlobalOptimisationTask
 from prospect.tasks.initialise import initialise_tasks
 from multiprocessing import Condition
 
 @dataclass
 class TasksState:
     queued: list[Type[BaseTask]]
     # All task dicts are indexed by the task ids 
@@ -67,14 +69,17 @@
 
     def finalize(self, executor) -> None:
         # Things to do before shutting down
         if self.config.io.write:
             if self.config.run.jobtype == 'profile':
                 analysis_task = self.get_profile_analysis()
                 analysis_task.run([task for task in self.tasks.done.values() if task.id in analysis_task.required_task_ids])
+            elif self.config.run.jobtype == 'global_optimisation':
+                analysis_task = self.get_global_optimisation_analysis()
+                analysis_task.run([task for task in self.tasks.done.values() if task.id in analysis_task.required_task_ids])
             self.dump_snapshot()
             self.status_update()
 
     def push_task(self, task: Type[BaseTask]) -> None:
         # Pushes task and sets dependencies
         task.time_emit = datetime.now()
         if self.is_task_ready(task):
@@ -138,18 +143,18 @@
                     heapq.heappush(self.tasks.queued, new_task)
 
         with self.condition:
             self.condition.notify_all()
 
         if self.config.io.write:
             if time.time() > self.next_dump_time:
-                if self.config.run.jobtype == 'profile' and finished_task.type != 'AnalyseProfileTask':
-                    if 'AnalyseProfileTask' not in [queued_task.type for queued_task in self.tasks.queued]:
-                        if 'AnalyseProfileTask' not in [ongoing_task.type for ongoing_task in self.tasks.ongoing.values()]:
-                            self.push_task(self.get_profile_analysis())
+                if finished_task.type != 'AnalyseProfileTask' and finished_task.type != 'AnalyseGlobalOptimisationTask':
+                    analyse_task = self.get_analysis_task()
+                    if analyse_task is not None:
+                        self.push_task(analyse_task)
                 self.dump_snapshot()
                 self.status_update()
 
                 self.next_dump_time = time.time() + self.config.io.snapshot_interval
     
     def dump_snapshot(self) -> None:
         print("Dumping snapshot...")
@@ -198,18 +203,25 @@
                 status_file.write(get_write_line(task_unready))
             status_file.write("\n\n=== DONE ================================================")
             status_file.write(header)
             for task_id, task_done in self.tasks.done.items():
                 status_file.write(get_write_line(task_done))
             status_file.write("\n")
     
-    def get_profile_analysis(self) -> AnalyseProfileTask:
+    def get_analysis_task(self) -> Type[BaseAnalyseTask]:
         required_tasks = [id for id, task in self.tasks.done.items() if task.type == 'OptimiseTask' or task.type == 'InitialiseOptimiserTask']
-        return AnalyseProfileTask(self.config, required_tasks)
-    
+        if self.config.run.jobtype == 'profile':
+            if 'AnalyseProfileTask' not in [queued_task.type for queued_task in self.tasks.queued]:
+                if 'AnalyseProfileTask' not in [ongoing_task.type for ongoing_task in self.tasks.ongoing.values()]:
+                    return AnalyseProfileTask(self.config, required_tasks)
+        elif self.config.run.jobtype == 'global_optimisation':
+            if 'AnalyseGlobalOptimisationTask' not in [queued_task.type for queued_task in self.tasks.queued]:
+                if 'AnalyseGlobalOptimisationTask' not in [ongoing_task.type for ongoing_task in self.tasks.ongoing.values()]:
+                    return AnalyseGlobalOptimisationTask(self.config, required_tasks)
+
 class SerialContext:
     class MockFuture:
         def __init__(self, finished_task: Type[BaseTask]) -> None:
             self.finished_task = finished_task
 
         def add_done_callback(self, finalize_func) -> None:
             finalize_func(self)
```

### Comparing `prospect-public-23.0.3/prospect/input.py` & `prospect_public-24.0.0/prospect/input.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,17 @@
             'kernel': import_module('prospect.kernels.base_kernel')
         }
         if 'run' in config_yaml and 'jobtype' in config_yaml['run']:
             if config_yaml['run']['jobtype'] == 'mcmc':
                 modules['mcmc'] = import_module('prospect.mcmc')
             elif config_yaml['run']['jobtype'] == 'profile':
                 modules['profile'] = import_module('prospect.profile')
+            elif config_yaml['run']['jobtype'] == 'global_optimisation':
+                # Global optimisation uses profiling inputs for optimisation
+                modules['profile'] = import_module('prospect.profile')
             else:
                 raise ValueError("The given value of 'jobtype' is not recognised. Choose either 'mcmc' or 'profile'.")
         else:
             raise ValueError("You must give 'jobtype' as an input under the 'run' category.")
 
         str_eval_arguments = [('profile', 'values')]
         for arg_module, arg_name in str_eval_arguments:
```

### Comparing `prospect-public-23.0.3/prospect/io.py` & `prospect_public-24.0.0/prospect/io.py`

 * *Files identical despite different names*

### Comparing `prospect-public-23.0.3/prospect/kernels/analytical_kernel.py` & `prospect_public-24.0.0/prospect/kernels/analytical_kernel.py`

 * *Files identical despite different names*

### Comparing `prospect-public-23.0.3/prospect/kernels/base_kernel.py` & `prospect_public-24.0.0/prospect/kernels/base_kernel.py`

 * *Files identical despite different names*

### Comparing `prospect-public-23.0.3/prospect/kernels/cobaya_kernel.py` & `prospect_public-24.0.0/prospect/kernels/cobaya_kernel.py`

 * *Files identical despite different names*

### Comparing `prospect-public-23.0.3/prospect/kernels/initialisation.py` & `prospect_public-24.0.0/prospect/kernels/initialisation.py`

 * *Files identical despite different names*

### Comparing `prospect-public-23.0.3/prospect/kernels/montepython_kernel.py` & `prospect_public-24.0.0/prospect/kernels/montepython_kernel.py`

 * *Files identical despite different names*

### Comparing `prospect-public-23.0.3/prospect/mcmc.py` & `prospect_public-24.0.0/prospect/mcmc.py`

 * *Files identical despite different names*

### Comparing `prospect-public-23.0.3/prospect/optimiser.py` & `prospect_public-24.0.0/prospect/optimiser.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,18 @@
                             [self.kernel.loglkl(self.initial_position)],
                             self.initial_position
                         )
         }
         self.mcmc = MetropolisHastings(config_mcmc, self.kernel, **mcmc_args)
 
     def optimise(self):
-        print(f"Running a simulated annealing iteration of parameter {self.config.profile.parameter}={self.settings['fixed_param_val']} with temperature {self.settings['temperature']}")
+        if self.config.run.jobtype == 'profile':
+            print(f"Running a simulated annealing iteration of parameter {self.config.profile.parameter}={self.settings['fixed_param_val']} with temperature {self.settings['temperature']}")
+        else:
+            print(f"Running a simulated annealing iteration with temperature {self.settings['temperature']}")
         if self.config.profile.steps_per_iteration is not None:
             self.mcmc.run_steps(self.config.profile.steps_per_iteration)
         elif self.config.profile.minutes_per_iteration is not None:
             self.mcmc.run_minutes(self.config.profile.minutes_per_iteration)
     
     def set_bestfit(self):
         bestfit_idx = np.argmin(self.mcmc.chain.loglkls)
@@ -143,16 +146,17 @@
                     # Step size is inside target interval, don't change
                     new_step_size = self.settings['step_size']
         else:
             raise ValueError('Invalid temperature schedule.')
         
         optimise_settings = {
             'current_best_loglkl': self.bestfit['loglkl'],
-            'fixed_param_val': self.settings['fixed_param_val'],
             'initial_position': self.mcmc.chain.last_position,
             'covmat': self.covmat,
             'temperature': new_temp,
             'temperature_change': self.settings['temperature_change'],
             'step_size': new_step_size,
             'step_size_change': self.settings['step_size_change']
         }
+        if self.config.run.jobtype == 'profile':
+            optimise_settings['fixed_param_val'] = self.settings['fixed_param_val']
         return optimise_settings
```

### Comparing `prospect-public-23.0.3/prospect/profile.py` & `prospect_public-24.0.0/prospect/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,19 +125,30 @@
 """
     Definition of user arguments related to mcmc.py
 """
 
 @dataclass
 class Arguments:
     class parameter(InputArgument):
-        val_type = str
+        val_type = str | NoneType
+        def get_default(self, config_yaml: dict[str, Any]):
+            if config_yaml['run']['jobtype'] == 'global_optimisation':
+                # None corresponds to global optimisation
+                return None
+            else:
+                raise ValueError("You need to specify the 'parameter' input of the profile section.")
     
     class values(InputArgument):
         """Parameter values where the profile is evaluated"""
         val_type = list[float] | list[int] | np.ndarray | list
+        def get_default(self, config_yaml: dict[str, Any]):
+            if config_yaml['run']['jobtype'] == 'global_optimisation':
+                return []
+            else:
+                raise ValueError("You need to specify the 'values' input of the profile section.")
     
     class optimiser(InputArgument):
         allowed_values = ['simulated annealing']
         def get_default(self, config_yaml: dict[str, Any]):
             return 'simulated annealing'
 
     class temperature_schedule(InputArgument):
```

### Comparing `prospect-public-23.0.3/prospect/run.py` & `prospect_public-24.0.0/prospect/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,15 +90,18 @@
     state = load_state(prospect_folder)
     return Scheduler(config, state)
 
 def analyse(prospect_folder):
     snapshot = load(prospect_folder)
     if snapshot.config.run.jobtype == 'profile':
         print(f"Analysing {prospect_folder} as a profile likelihood run.")
-        analysis_task = snapshot.get_profile_analysis()
+        analysis_task = snapshot.get_analysis_task()
+    if snapshot.config.run.jobtype == 'global_optimisation':
+        print(f"Analysing {prospect_folder} as a global optimisation likelihood run.")
+        analysis_task = snapshot.get_analysis_task()
 
     elif snapshot.config.run.jobtype == 'mcmc':
         print(f"Analysing {prospect_folder} as an MCMC run.")
         from prospect.tasks.mcmc_task import AnalyseMCMCTask
         # Pick out the unique task of largest id belonging to each chain
         final_tasks = {}
         for chain_id, mcmc_task in {task.mcmc_args['chain_id']: task for task in snapshot.tasks.done.values() if task.type == 'MCMCTask'}:
@@ -129,15 +132,15 @@
     Definition of user arguments related to run.py
 """
 
 @dataclass
 class Arguments:
     class jobtype(InputArgument):
         val_type = str
-        allowed_values = ['mcmc', 'profile']
+        allowed_values = ['mcmc', 'profile', 'global_optimisation']
     
     class mode(InputArgument):
         val_type = str
         default = 'threaded'
         allowed_values = ['mpi', 'threaded', 'serial']
     
     class num_processes(InputArgument):
```

### Comparing `prospect-public-23.0.3/prospect/tasks/analyse_profile_task.py` & `prospect_public-24.0.0/prospect/tasks/analyse_profile_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,42 +6,25 @@
 import matplotlib
 import matplotlib.pyplot as plt 
 import numpy as np 
 from scipy.interpolate import interp1d
 from scipy import stats
 from prospect.input import Configuration
 from prospect.kernels.initialisation import initialise_kernel
-from prospect.tasks.base_task import BaseTask
+from prospect.tasks.base_analyse_task import BaseAnalyseTask
 from prospect.tasks.optimise_task import OptimiseTask
 
 # Switch matplotlib backend to one that doesn't pop up figures
 matplotlib.use('Agg')
 
 def argmax(iterable):
     """From https://stackoverflow.com/questions/16945518/finding-the-index-of-the-value-which-is-the-min-or-max-in-python"""
     return max(enumerate(iterable), key=lambda x: x[1])[0]
 
-class AnalyseProfileTask(BaseTask):
-    priority = 75.0
-
-    # Figure settings
-    cm = 1/2.54  # centimeters in inches
-    fig = {
-        'width': 8.6*cm, # PRL figure width
-        'height': 2,
-        'fontsize': 11/1.1,
-        'rep_colors': ['b', 'r', 'g', 'c', 'y', 'm']*50,
-        'rep_ms': [4.5, 4.0, 3.5, 3, 2.5, 2., 1.5, 1., 0.5]*50,
-        'interval_styles': ['--', ':']*5
-    }
-
-    def __init__(self, config: Configuration, required_task_ids: list[int]):
-        super().__init__(config, required_task_ids)
-        self.dir = os.path.join(config.io.dir, config.run.jobtype)
-
+class AnalyseProfileTask(BaseAnalyseTask):
     def run(self, tasks: list[OptimiseTask]): 
         if not tasks:
             print(f"No tasks to analyse. Ending AnalyseProfileTask.")
             return
         print("Running profile analysis script...")
         kernel = initialise_kernel(self.config.kernel, self.config.io.dir, self.id)
         optimise_tasks, initialise_tasks = [], []
@@ -54,17 +37,14 @@
             elif task.type == 'InitialiseOptimiserTask':
                 initialise_tasks.append(task)
 
         param_vals = np.sort(param_vals)
         old_param_vals = deepcopy(self.config.profile.values)
         self.config.profile.values = param_vals
 
-        if not os.path.isdir(self.dir):
-            os.makedirs(self.dir)
-        
         self.bestfits = self.sort_tasks(optimise_tasks, initialise_tasks)
         profile = self.compute_profile(self.bestfits)
         self.write_results(self.bestfits, kernel)
         self.write_profile_status(optimise_tasks, initialise_tasks)
 
         intervals = self.compute_intervals_neyman(profile)
         self.write_intervals(profile, intervals, kernel)
@@ -103,18 +83,14 @@
                         pad_current = 13
                         pad_best = 9
                         write_string = f"| rep {idx_rep+1} \t {current_iter:<{pad_current}} \t {current_loglkl:.10e} \t {best_iter:<{pad_best}} \t {best_loglkl:.10e} \t {current_task.converged} "
                         if idx_rep == 0:
                             file.write(f"\t {write_string}")
                         else:
                             file.write(f"\n\t\t\t\t {write_string}")
-
-    def emit_tasks(self) -> list[Type[BaseTask]]:
-        # Never emit anything; the OptimiseTasks manage convergence themselves.
-        return []
     
     def sort_tasks(self, optimise_tasks, initialise_tasks):
         # Order the tasks
         bestfits = {}
         for fixed_value in self.config.profile.values:
             bestfits[fixed_value] = {}
             for idx_rep in range(self.config.profile.repetitions):
```

### Comparing `prospect-public-23.0.3/prospect/tasks/base_task.py` & `prospect_public-24.0.0/prospect/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `prospect-public-23.0.3/prospect/tasks/initialise.py` & `prospect_public-24.0.0/prospect/tasks/initialise.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 from prospect.tasks.base_task import BaseTask
 from prospect.tasks.mcmc_task import initialise_mcmc_tasks
 from prospect.tasks.initialise_profile_task import initialise_profile_tasks
 
 def initialise_tasks(config) -> list[Type[BaseTask]]:
     if config.run.jobtype == 'mcmc':
         new_tasks = initialise_mcmc_tasks(config, mcmc_id=0)
-    elif config.run.jobtype == 'profile':
+    elif config.run.jobtype == 'profile' or config.run.jobtype == 'global_optimisation':
         new_tasks = initialise_profile_tasks(config)
     else:
-        raise ValueError(f'No tasks to start at initialization with jobtype {config["jobtype"]}.')
+        raise ValueError(f'No tasks to start at initialization with jobtype {[config.run.jobtype]}.')
     return new_tasks
```

### Comparing `prospect-public-23.0.3/prospect/tasks/initialise_optimiser_task.py` & `prospect_public-24.0.0/prospect/tasks/initialise_optimiser_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+from types import NoneType
 from typing import Type
 import numpy as np 
 from getdist import loadMCSamples
 from prospect.input import Configuration
 from prospect.kernels.initialisation import initialise_kernel
 from prospect.mcmc import Chain, collapse_chains, compute_covariance_matrix
 from prospect.tasks.base_task import BaseTask
@@ -13,29 +14,31 @@
         This task initialises a profile from a finished MCMC
         The MCMC must be made with the chosen kernel 
         (i.e. cannot start a MontePython-based profile from a cobaya chain)
 
     """
     priority = 80.0
 
-    def __init__(self, config: Configuration, fixed_param_val: float, repetition_number: int = 0):
+    def __init__(self, config: Configuration, fixed_param_val: float | NoneType, repetition_number: int = 0):
         super().__init__(config)
-        self.fixed_param_val = fixed_param_val
+        if self.config.run.jobtype == 'profile':
+            self.fixed_param_val = fixed_param_val
         self.repetition_number = repetition_number
 
     def run(self, _):
         kernel = initialise_kernel(self.config.kernel, self.config.io.dir, self.id)
-        try:
-            self.profile_param_idx = np.where(np.array(list(kernel.param['varying'].keys())) == self.config.profile.parameter)[0][0]
-        except Exception as e:
-            print("EXCEPTION:")
-            print(f"The requested profile parameter {self.config.profile.parameter} is not recognized by the kernel. Check that your kernel parameter file has the parameter enabled.")
-            print("Original exception:")
-            raise e
-        kernel.set_fixed_parameters({self.config.profile.parameter: self.fixed_param_val})
+        if self.config.run.jobtype == 'profile':
+            try:
+                self.profile_param_idx = np.where(np.array(list(kernel.param['varying'].keys())) == self.config.profile.parameter)[0][0]
+            except Exception as e:
+                print("EXCEPTION:")
+                print(f"The requested profile parameter {self.config.profile.parameter} is not recognized by the kernel. Check that your kernel parameter file has the parameter enabled.")
+                print("Original exception:")
+                raise e
+            kernel.set_fixed_parameters({self.config.profile.parameter: self.fixed_param_val})
 
         if self.config.profile.start_from_position is not None and self.config.profile.start_from_covmat is not None:
             self.set_initial_position(kernel, kernel.read_initial_position(self.config.profile.start_from_position))
             self.set_covmat(kernel.read_covmat(self.config.profile.start_from_covmat))
             print(f"Read initial position from {self.config.profile.start_from_position}\n and initial covmat from {self.config.profile.start_from_covmat}.")
 
         elif self.config.profile.start_from_profile is not None:
@@ -44,47 +47,52 @@
                 self.set_covmat(compute_covariance_matrix([self.get_binned_mcmc_reduced(kernel)]))
             elif self.config.profile.start_from_covmat is not None:
                 print("You have set 'start_from_profile' and 'start_from_covmat'. Initialising position from profile and covmat from files.")
                 self.set_covmat(kernel.read_covmat(self.config.profile.start_from_covmat))
 
             from prospect.profile import load_profile
             start_profile = load_profile(self.config.profile.start_from_profile, direct_txt=True)
-            idx_closest = np.argmin(np.abs(start_profile[self.config.profile.parameter] - self.fixed_param_val))
+            if self.config.run.jobtype == 'profile':
+                idx_closest = np.argmin(np.abs(start_profile[self.config.profile.parameter] - self.fixed_param_val))
+                print(f"Set initial bestfit for {self.config.profile.parameter}={self.fixed_param_val} from the point {self.config.profile.parameter}={start_profile[self.config.profile.parameter][idx_closest]} in {self.config.profile.start_from_profile}.")
+            else:
+                # Start from best point of the profile
+                idx_closest = np.argmin(start_profile['-loglkl'])
+                print(f"Set initial bestfit for from the best point in the profile {self.config.profile.start_from_profile}.")
             position = {param: [start_profile[param][idx_closest]] for param in kernel.param['varying'].keys()}
             self.set_initial_position(kernel, position)
-            print(f"Set initial bestfit for {self.config.profile.parameter}={self.fixed_param_val} from the point {self.config.profile.parameter}={start_profile[self.config.profile.parameter][idx_closest]} in {self.config.profile.start_from_profile}.")
         
         elif self.config.profile.start_from_mcmc is not None:
             binned_points = self.get_binned_mcmc_reduced(kernel)
             self.set_covmat(compute_covariance_matrix([binned_points]))
 
             # Get bestfit among these points
             bestfit_index = np.argmin(binned_points.loglkls)
             bf = binned_points[bestfit_index]
-            bf[self.config.profile.parameter] = [self.fixed_param_val]
-            del bf[self.config.profile.parameter]
+            if self.config.run.jobtype == 'profile' and self.config.profile.parameter in bf:
+                del bf[self.config.profile.parameter]
+                print(f"Constructed local bestfit and covariance matrix around {self.config.profile.parameter}={self.fixed_param_val}.")
             self.set_initial_position(kernel, bf)
-
-            print(f"Constructed local bestfit and covariance matrix around {self.config.profile.parameter}={self.fixed_param_val}.")
         else:
             raise ValueError('InitialiseOptimiserTask could not construct an initial position and/or covariance matrix. Make sure to supply either "start_from_mcmc" or "start_from_position" and "start_from_covmat" in the profile section of the input.')
 
     def emit_tasks(self) -> list[Type[BaseTask]]:
         optimise_settings = {
             'current_best_loglkl': self.initial_loglkl,
-            'fixed_param_val': self.fixed_param_val,
             'initial_position': self.initial_bestfit,
             'covmat': self.initial_covmat,
             'temperature': self.config.profile.temperature_range[0],
             'temperature_change': get_temperature_change(self.config),
             'step_size': self.config.profile.step_size_range[0],
             'step_size_change': get_initial_step_size_change(self.config),
             'iteration_number': 0,
             'repetition_number': self.repetition_number
         }
+        if self.config.run.jobtype == 'profile':
+            optimise_settings['fixed_param_val'] = self.fixed_param_val
         return [OptimiseTask(self.config, optimise_settings)]
     
     def get_binned_mcmc_reduced(self, kernel):
         tic = time.perf_counter()
         initial_chain = load_mcmc(self.config.profile.start_from_mcmc, kernel, collapse=True)
         print(f"Loaded MCMC {self.config.profile.start_from_mcmc} in {time.perf_counter() - tic:.4} s")
         for param_name in kernel.param['varying']:
@@ -101,25 +109,29 @@
             if param_name not in kernel.param['varying']:
                 if param_name not in kernel.param['derived']:
                     if param_name not in kernel.param['fixed']:
                         unneeded_params.append(param_name)
         for name in unneeded_params:
             del initial_chain.positions[name]
 
-        # Get start_bin_fraction fraction of total points closest to the param_val
-        return get_fraction_of_points_in_bin(initial_chain, self.fixed_param_val, self.config.profile.parameter, self.config.profile.start_bin_fraction)
+        if self.config.run.jobtype == 'profile':
+            # Get start_bin_fraction fraction of total points closest to the param_val
+            return get_fraction_of_points_in_bin(initial_chain, self.fixed_param_val, self.config.profile.parameter, self.config.profile.start_bin_fraction)
+        else:
+            return initial_chain.from_indices(range(len(initial_chain.mults)))
 
     def set_initial_position(self, kernel, position):
         self.initial_bestfit = position
         self.initial_loglkl = kernel.loglkl(self.initial_bestfit)
 
     def set_covmat(self, covmat):
         self.initial_covmat = covmat
-        self.initial_covmat = np.delete(self.initial_covmat, [self.profile_param_idx], 0) # remove row of profile param
-        self.initial_covmat = np.delete(self.initial_covmat, [self.profile_param_idx], 1) # remove column of profile param 
+        if self.config.run.jobtype == 'profile':
+            self.initial_covmat = np.delete(self.initial_covmat, [self.profile_param_idx], 0) # remove row of profile param
+            self.initial_covmat = np.delete(self.initial_covmat, [self.profile_param_idx], 1) # remove column of profile param 
 
 
 def get_temperature_change(config):
     temp_change = 0.
     if config.profile.temperature_schedule == 'exponential':
         # The temperature change parameter is the rate, i.e. the number that
         # the temperature is multiplied by at each iteration
```

### Comparing `prospect-public-23.0.3/prospect/tasks/initialise_profile_task.py` & `prospect_public-24.0.0/prospect/tasks/initialise_profile_task.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from typing import Type
 from prospect.input import Configuration
 from prospect.tasks.base_task import BaseTask
 from prospect.tasks.initialise_optimiser_task import InitialiseOptimiserTask
+from prospect.tasks.initialise_optimiser_task import InitialiseOptimiserTask
 
 class InitialiseProfileTask(BaseTask):
     """
         Task which finds a sampling of the profile and emits optimizations at each point in the profile.
 
     """
     priority = 90.0
 
     def run(self, _):
         pass
     
     def emit_tasks(self) -> list[Type[BaseTask]]:
         task_list = []
-        for idx_rep in range(self.config.profile.repetitions):
-            for param_val in self.config.profile.values:
-                task_list.append(InitialiseOptimiserTask(self.config, param_val, idx_rep))
+        if self.config.run.jobtype == 'global_optimisation':
+            # Do global optimisation
+            for idx_rep in range(self.config.profile.repetitions):
+                task_list.append(InitialiseOptimiserTask(self.config, None, idx_rep))
+        else:
+            for idx_rep in range(self.config.profile.repetitions):
+                for param_val in self.config.profile.values:
+                    task_list.append(InitialiseOptimiserTask(self.config, param_val, idx_rep))
         return task_list
 
 def initialise_profile_tasks(config: Configuration) -> list[Type[BaseTask]]:
     return [InitialiseProfileTask(config)]
```

### Comparing `prospect-public-23.0.3/prospect/tasks/mcmc_task.py` & `prospect_public-24.0.0/prospect/tasks/mcmc_task.py`

 * *Files identical despite different names*

### Comparing `prospect-public-23.0.3/prospect/tasks/optimise_task.py` & `prospect_public-24.0.0/prospect/tasks/optimise_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,18 @@
     def run(self, _):
         kernel = initialise_kernel(self.config.kernel, self.config.io.dir, self.id)
         if 'fixed_param_val' in self.optimise_settings:
             kernel.set_fixed_parameters({self.config.profile.parameter: self.optimise_settings['fixed_param_val']})
         self.optimiser = initialise_optimiser(self.config, kernel, self.optimise_settings)
         self.optimiser.optimise()
         self.optimiser.set_bestfit()
-        print(f"OptimiseTask id={self.id}, iteration {self.optimise_settings['iteration_number']} at {self.config.profile.parameter}={self.optimise_settings['fixed_param_val']:.4e} finished:")
+        if self.config.run.jobtype == 'profile':
+            print(f"OptimiseTask id={self.id}, iteration {self.optimise_settings['iteration_number']} at {self.config.profile.parameter}={self.optimise_settings['fixed_param_val']:.4e} finished:")
+        else:
+            print(f"OptimiseTask id={self.id}, iteration {self.optimise_settings['iteration_number']} finished:")
         print(f"\tBestfit loglkl={self.optimiser.bestfit['loglkl']:.10} | Acceptance rate={self.optimiser.bestfit['acceptance_rate']:.4} | Num_evals={np.sum(self.optimiser.mcmc.chain.mults)} | Temp={self.optimise_settings['temperature']:.4e} | Step size={self.optimise_settings['step_size']:.4e}")
 
     def finalize(self):
         del self.optimiser.mcmc.kernel
         del self.optimiser.kernel
 
     def emit_tasks(self) -> list[Type[BaseTask]]:
```

### Comparing `prospect-public-23.0.3/prospect_public.egg-info/PKG-INFO` & `prospect_public-24.0.0/prospect_public.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prospect-public
-Version: 23.0.3
+Version: 24.0.0
 Summary: A profile likelihood code for frequentist cosmological parameter inference
 Author-email: Emil Brinch Holm <ebholm@phys.au.dk>, Thomas Tram <thomas.tram@phys.au.dk>
 Project-URL: Homepage, https://github.com/AarhusCosmology/prospect_public
 Project-URL: Bug Tracker, https://github.com/AarhusCosmology/prospect_public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -58,14 +58,20 @@
 PROSPECT provides a quick tool to load the profile likelihood in Python as follows:
 ```
 from prospect.profile import load_profile
 profile_dict = load_profile('path_to_my_run')
 ```
 whence `profile_dict` is a dictionary with the best-fitting parameter values at each point in the profile, along with the associated likelihood values. 
 
+#### Global optimisation
+
+The efficient optimiser of PROSPECT can also be used to find global bestfits of your cosmology. An example for such an input .yaml file is found in the `input/example_toy/example_global_optimisation_toy.yaml` file. Starting from a .yaml file for a profile likelihood, you only need to change the `jobtype` input of the `run` section to 'global_optimisation' (rather than the usual 'profile'). All of the settings of the optimiser defined in the `profile` section are then used to carry out global optimisation of your model, giving an output folder similar in structure to that obtained from profile likelihoods runs. 
+
+*Note that when running with `jobtype: 'global_optimisation'`, the inputs `parameter`, `values`, `start_bin_fraction` as well as `plot_profile`, `detailed_plot`, `plot_Delta_chi2` and `confidence_levels` of the `profile` section are ignored, but the rest of the input, such as the schedules and initialisation procedures, are still used to define the settings of the optimiser.*
+
 #### Reoptimising
 
 Not satisfied with your profile? You can always queue new `OptimiseTask`s with the reoptimising feature. Add extra tasks from the terminal by running
 ```
 prospect-reoptimise -y my_reoptimise_settings.yaml -o folder_to_reoptimise (--override)
 ```
 Here, `my_reoptimise_settings.yaml` should be a yaml file similar in structure to PROSPECT input files, but only containing the "profile" substructure. For example:
```

### Comparing `prospect-public-23.0.3/prospect_public.egg-info/SOURCES.txt` & `prospect_public-24.0.0/prospect_public.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 prospect/kernels/__init__.py
 prospect/kernels/analytical_kernel.py
 prospect/kernels/base_kernel.py
 prospect/kernels/cobaya_kernel.py
 prospect/kernels/initialisation.py
 prospect/kernels/montepython_kernel.py
 prospect/tasks/__init__.py
+prospect/tasks/analyse_global_optimisation_task.py
 prospect/tasks/analyse_profile_task.py
+prospect/tasks/base_analyse_task.py
 prospect/tasks/base_task.py
 prospect/tasks/initialise.py
 prospect/tasks/initialise_optimiser_task.py
 prospect/tasks/initialise_profile_task.py
 prospect/tasks/mcmc_task.py
 prospect/tasks/optimise_task.py
 prospect_public.egg-info/PKG-INFO
```

### Comparing `prospect-public-23.0.3/pyproject.toml` & `prospect_public-24.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools', 'numpy>=1.17.0', 'scipy>=1.5', 'PyYAML>=5.1', 'GetDist>=1.3.1']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prospect-public"
-version = "23.0.3"
+version = "24.0.0"
 requires-python = ">3.10.0"
 authors = [
   { name="Emil Brinch Holm", email="ebholm@phys.au.dk"},
   { name="Thomas Tram", email="thomas.tram@phys.au.dk"},
 ]
 description = "A profile likelihood code for frequentist cosmological parameter inference"
 readme = "README.md"
```

