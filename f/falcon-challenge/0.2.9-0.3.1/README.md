# Comparing `tmp/falcon_challenge-0.2.9.tar.gz` & `tmp/falcon_challenge-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_challenge-0.2.9.tar", last modified: Thu Apr 25 16:36:54 2024, max compression
+gzip compressed data, was "falcon_challenge-0.3.1.tar", last modified: Mon Apr 29 14:26:21 2024, max compression
```

## Comparing `falcon_challenge-0.2.9.tar` & `falcon_challenge-0.3.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:54.377393 falcon_challenge-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-25 16:36:54.377393 falcon_challenge-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:54.373393 falcon_challenge-0.2.9/decoder_demos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/decoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/ndt2_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/ndt2_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/random_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13336 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/sklearn_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:54.373393 falcon_challenge-0.2.9/falcon_challenge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/falcon_challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/falcon_challenge/challenge_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/falcon_challenge/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/falcon_challenge/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    25871 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/falcon_challenge/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/falcon_challenge/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:54.377393 falcon_challenge-0.2.9/falcon_challenge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-25 16:36:54.000000 falcon_challenge-0.2.9/falcon_challenge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 16:36:54.000000 falcon_challenge-0.2.9/falcon_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:36:54.000000 falcon_challenge-0.2.9/falcon_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 16:36:54.000000 falcon_challenge-0.2.9/falcon_challenge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 16:36:54.000000 falcon_challenge-0.2.9/falcon_challenge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:54.377393 falcon_challenge-0.2.9/preproc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/assemble_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/h2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/m1_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/m1_reachgrasp_preprocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/m2_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/m2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/merge_answers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/nwb_create_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/wrapper_convert_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/zip_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:36:54.377393 falcon_challenge-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:26:21.851815 falcon_challenge-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-29 14:26:21.851815 falcon_challenge-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:26:21.847815 falcon_challenge-0.3.1/decoder_demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/decoder_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/decoder_demos/decoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/decoder_demos/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/decoder_demos/ndt2_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/decoder_demos/ndt2_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/decoder_demos/random_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/decoder_demos/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13694 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/decoder_demos/sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/decoder_demos/sklearn_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:26:21.847815 falcon_challenge-0.3.1/falcon_challenge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/falcon_challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/falcon_challenge/challenge_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/falcon_challenge/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/falcon_challenge/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26203 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/falcon_challenge/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/falcon_challenge/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:26:21.851815 falcon_challenge-0.3.1/falcon_challenge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-29 14:26:21.000000 falcon_challenge-0.3.1/falcon_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-29 14:26:21.000000 falcon_challenge-0.3.1/falcon_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:26:21.000000 falcon_challenge-0.3.1/falcon_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-29 14:26:21.000000 falcon_challenge-0.3.1/falcon_challenge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 14:26:21.000000 falcon_challenge-0.3.1/falcon_challenge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:26:21.851815 falcon_challenge-0.3.1/preproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/preproc/assemble_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/preproc/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/preproc/h2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/preproc/m1_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/preproc/m1_reachgrasp_preprocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/preproc/m2_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/preproc/m2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/preproc/merge_answers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/preproc/nwb_create_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/preproc/wrapper_convert_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/preproc/zip_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:26:21.851815 falcon_challenge-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-29 14:26:15.000000 falcon_challenge-0.3.1/setup.py
```

### Comparing `falcon_challenge-0.2.9/LICENSE` & `falcon_challenge-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/PKG-INFO` & `falcon_challenge-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.2.9
+Version: 0.3.1
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.2.9/README.md` & `falcon_challenge-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/decoder_demos/decoding_utils.py` & `falcon_challenge-0.3.1/decoder_demos/decoding_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/decoder_demos/filtering.py` & `falcon_challenge-0.3.1/decoder_demos/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/decoder_demos/ndt2_decoder.py` & `falcon_challenge-0.3.1/decoder_demos/ndt2_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/decoder_demos/ndt2_sample.py` & `falcon_challenge-0.3.1/decoder_demos/ndt2_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/decoder_demos/random_decoder.py` & `falcon_challenge-0.3.1/decoder_demos/random_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/decoder_demos/rnn_decoder.py` & `falcon_challenge-0.3.1/decoder_demos/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/decoder_demos/sklearn_decoder.py` & `falcon_challenge-0.3.1/decoder_demos/sklearn_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,28 +96,26 @@
             MAX_HISTORY = int(NEURAL_TAU_MS / task_config.bin_size_ms) * 5 # bin size ms
             self.x_mean = payload['x_mean']
             self.x_std = payload['x_std']
             self.raw_history_buffer = np.zeros((MAX_HISTORY, batch_size, task_config.n_channels))
             self.observation_buffer = np.zeros((self.history, batch_size, task_config.n_channels))
 
     def reset(self, dataset_tags: List[Path] = [""]):
+        dataset_tags = [self._task_config.hash_dataset(dset.stem) for dset in dataset_tags]
         if isinstance(self.x_mean, dict):
-            # TODO retrieve a list of x_means
-            dataset_tags = [self._task_config.hash_dataset(dset.stem) for dset in dataset_tags]
             for dataset_tag in dataset_tags:
                 if dataset_tag not in self.x_mean:
                     raise ValueError(f"Dataset tag {dataset_tag} not found in calibration set {self.x_mean.keys()} - did you calibrate on this dataset?")
             self.local_x_mean = [self.x_mean[dset_tag] for dset_tag in dataset_tags]
             self.local_x_std = [self.x_std[dset_tag] for dset_tag in dataset_tags]
         else:
             self.local_x_mean = self.x_mean
             self.local_x_std = self.x_std
-        # TODO this one too...
+        
         if isinstance(self.clf, dict):
-            dataset_tags = [self._task_config.hash_dataset(dset.stem) for dset in dataset_tags]
             for dataset_tag in dataset_tags:
                 if dataset_tag not in self.clf:
                     raise ValueError(f"Dataset tag {dataset_tag} not found decoder set {self.clf.keys()}")
             self.local_clf = [self.clf[dataset_tag] for dataset_tag in dataset_tags]
         else:
             self.local_clf = self.clf
         self.raw_history_buffer = np.zeros_like(self.raw_history_buffer)
@@ -228,15 +226,19 @@
 def fit_last_session(
     datafiles: List[Path],
     calibration_datafiles: List[Path],
     task_config: FalconConfig,
     save_path: Path,
     history = 0,
 ):
-    day_unique = set([f.stem.split('_')[0] for f in datafiles])
+    hashes = [task_config.hash_dataset(f.stem) for f in datafiles]
+    if task_config.task == FalconTask.h1:
+        day_unique = set([h.split('_set_')[0] for h in hashes])
+    else:
+        day_unique = set([f.stem.split('_')[1] for f in datafiles])
     last_day = sorted(day_unique)[-1]
     fit_datafiles = [d for d in datafiles if last_day in d.stem]
     return fit_sklearn_decoder(
         fit_datafiles,
         calibration_datafiles,
         task_config,
         save_path,
@@ -247,21 +249,25 @@
     datafiles: List[Path],
     calibration_datafiles: List[Path],
     task_config: FalconConfig,
     save_path: Path,
     history = 0,
 ):
     all_datafiles = [*calibration_datafiles, *datafiles]
-    day_unique = set([f.stem.split('_')[0] for f in all_datafiles])
+    hashes = [task_config.hash_dataset(f.stem) for f in all_datafiles]
+    if task_config.task == FalconTask.h1:
+        day_unique = set([h.split('_set_')[0] for h in hashes])
+    else:
+        day_unique = set([f.stem.split('_')[1] for f in all_datafiles])
     all_decoders = {}
     x_means = {}
     x_stds = {}
-    for day in sorted(day_unique):
+    for day in sorted(day_unique): # separate decoder
         print(f"Training on day {day}")
-        fit_datafiles = [d for d in all_datafiles if day == d.stem.split('_')[0]]
+        fit_datafiles = [d for d in all_datafiles if day in task_config.hash_dataset(d)]
         (
             neural_data,
             covariates,
             trial_change,
             eval_mask
         ) = zip(*[load_nwb(fn, task_config.task) for fn in fit_datafiles])
         neural_data = np.concatenate(neural_data)
@@ -273,17 +279,17 @@
             train_y,
             test_x,
             test_y,
             x_mean,
             x_std,
             y_mean,
             y_std
-        ) = prepare_train_test(neural_data, covariates, ~eval_mask, history=history)
+        ) = prepare_train_test(neural_data, covariates, ~eval_mask, history=history, mask_still_times=task_config.task == FalconTask.h1)
         score, decoder = fit_and_eval_decoder(train_x, train_y, test_x, test_y)
-        for f in fit_datafiles:
+        for f in fit_datafiles: # write in mean for this subset of data
             fn = task_config.hash_dataset(f.stem)
             all_decoders[fn] = decoder
             x_means[fn], x_stds[fn] = np.mean(neural_data, axis=0), np.std(neural_data, axis=0)
             if np.any(x_stds[fn] == 0):
                 x_stds[fn][x_stds[fn] == 0] = 1
         print(f"CV Fit score: {score:.2f}")
     decoder_obj = {
@@ -318,15 +324,15 @@
     fit_fn(datafiles, calibration_datafiles, task_config, save_path, history=history)
     print(f"Saved to {save_path}")
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description='Train sklearn decoder')
 
     parser.add_argument('--task', type=str, choices=['h1', 'm1', 'm2'], help='Task for training')
-    parser.add_argument('--training_dir', '-t', type=str, help='Root directory for training files')
-    parser.add_argument('--calibration_dir', '-c', type=str, help='Root directory for calibration files')
+    parser.add_argument('--training_dir', '-t', type=str, help='Root directory for training files', required=True)
+    parser.add_argument('--calibration_dir', '-c', type=str, help='Root directory for calibration files', required=True)
     parser.add_argument('--mode', '-m', type=str, choices=['all', 'last', 'per-day'], help='Mode for training')
     parser.add_argument('--history', type=int, default=0, help='History for decoder')
 
     args = parser.parse_args()
 
     main(args.task, args.training_dir, args.calibration_dir, args.history, args.mode)
```

### Comparing `falcon_challenge-0.2.9/decoder_demos/sklearn_sample.py` & `falcon_challenge-0.3.1/decoder_demos/sklearn_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/falcon_challenge/dataloaders.py` & `falcon_challenge-0.3.1/falcon_challenge/dataloaders.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/falcon_challenge/evaluator.py` & `falcon_challenge-0.3.1/falcon_challenge/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     FalconTask.h2: DATASET_HELDINOUT_MAP['h2']['held_out'],
 }
 
 RECOMMENDED_BATCH_SIZES = {
     FalconTask.h1: 8,
     FalconTask.m1: 4,
     FalconTask.h2: 1,
-    FalconTask.m2: 1, # TODO up
+    FalconTask.m2: 6,
 }
 
 # Development time flag. False allows direct evaluation without payload writing, only usable for local minival.
 # Should be set to true for remote evaluation.
 # USE_PKLS = False
 USE_PKLS = True
 
@@ -209,15 +209,15 @@
             else:
                 tgt = np.concatenate(tgt_dict[in_or_out])
             mask = np.concatenate(mask_dict[in_or_out])
             eval_fn = FalconEvaluator.compute_metrics_edit_distance if 'h2' in datasplit else FalconEvaluator.compute_metrics_regression
             try:
                 metrics = eval_fn(pred, tgt, mask)
             except Exception as e:
-                raise ValueError(f"Failed to compute metrics for {datasplit} {in_or_out}: {e}")
+                raise ValueError(f"Failed to compute metrics for {datasplit} {in_or_out}: {e}. Lengths submitted: {[len(piece) for piece in pred_dict[in_or_out]]}")
             for k in metrics:
                 split_result[f'{HELDIN_OR_OUT_MAP[in_or_out]} {k}'] = metrics[k]
         result.append({f'{phase_codename}_split_{datasplit}': split_result})
 
     print(f"Returning result from phase: {phase_codename}: {result}")
     # Out struct according to https://evalai.readthedocs.io/en/latest/evaluation_scripts.html
     return {"result": result, 'submission_result': result[0]}
@@ -290,18 +290,22 @@
         else: # possibly docker or local
             if os.path.exists(f"./data/{dataset.name}"):
                 logger.info("Using local data directory.")
                 data_dir = "data"
             else:
                 data_dir = os.environ.get("EVAL_DATA_PATH") # a local docker eval
         data_dir = Path(data_dir) / dataset.name
+        if not data_dir.exists():
+            raise FileNotFoundError(f"Evaluation data directory {data_dir} not found.")
         if phase == 'test': # TODO wire wherever test is actually stored on remote
             eval_dir = data_dir / f"eval"
         else:
             eval_dir = data_dir / "minival"
+        if not eval_dir.exists():
+            raise FileNotFoundError(f"Evaluation directory {eval_dir} found but requested phase {phase} not found.")
         return sorted(list(eval_dir.glob("*val*.nwb")))
 
     def get_eval_files(self, phase: str = 'minival'):
         logger.info("Searching for evaluation data.")
         handles = self.get_eval_handles(self.eval_remote, self.dataset, phase=phase)
         logger.info(f"Found {len(handles)} files.")
         if len(handles) == 0:
```

### Comparing `falcon_challenge-0.2.9/falcon_challenge/interface.py` & `falcon_challenge-0.3.1/falcon_challenge/interface.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/falcon_challenge.egg-info/PKG-INFO` & `falcon_challenge-0.3.1/falcon_challenge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.2.9
+Version: 0.3.1
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.2.9/falcon_challenge.egg-info/SOURCES.txt` & `falcon_challenge-0.3.1/falcon_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/preproc/assemble_data.py` & `falcon_challenge-0.3.1/preproc/assemble_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/preproc/filtering.py` & `falcon_challenge-0.3.1/preproc/filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import torch.nn.functional as F
 
 r"""
     H1 filtering
 """
 NEURAL_TAU_MS = 240. # exponential filter from H1 Lab
 def apply_exponential_filter(
-        x, tau=NEURAL_TAU_MS, bin_size=10, extent: int=1
+        x, tau=NEURAL_TAU_MS, bin_size=20, extent: int=1
     ):
     """
     Apply a **causal** exponential filter to the neural signal.
 
     :param x: NumPy array of shape (time, channels)
     :param tau: Decay rate (time constant) of the exponential filter
     :param bin_size: Bin size in ms (default is 10ms)
```

### Comparing `falcon_challenge-0.2.9/preproc/h2_preproc.py` & `falcon_challenge-0.3.1/preproc/h2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/preproc/m1_fewshot_trial_counts.py` & `falcon_challenge-0.3.1/preproc/m1_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/preproc/m1_reachgrasp_preprocv2.py` & `falcon_challenge-0.3.1/preproc/m1_reachgrasp_preprocv2.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/preproc/m2_fewshot_trial_counts.py` & `falcon_challenge-0.3.1/preproc/m2_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/preproc/m2_preproc.py` & `falcon_challenge-0.3.1/preproc/m2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/preproc/merge_answers.py` & `falcon_challenge-0.3.1/preproc/merge_answers.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/preproc/nwb_create_utils.py` & `falcon_challenge-0.3.1/preproc/nwb_create_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/preproc/zip_data.py` & `falcon_challenge-0.3.1/preproc/zip_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.9/setup.py` & `falcon_challenge-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falcon_challenge',
-    version='0.2.9',
+    version='0.3.1',
 
     url='https://github.com/snel-repo/stability-benchmark',
     author='Joel Ye',
     author_email='joelye9@gmail.com',
 
     packages=find_packages(exclude=['data_demos', 'data']),
     install_requires=[
```

