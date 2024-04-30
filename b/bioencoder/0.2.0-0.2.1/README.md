# Comparing `tmp/bioencoder-0.2.0.tar.gz` & `tmp/bioencoder-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioencoder-0.2.0.tar", last modified: Thu Apr 18 21:46:07 2024, max compression
+gzip compressed data, was "bioencoder-0.2.1.tar", last modified: Tue Apr 30 21:06:19 2024, max compression
```

## Comparing `bioencoder-0.2.0.tar` & `bioencoder-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 21:46:07.549732 bioencoder-0.2.0/
--rw-rw-rw-   0        0        0     1126 2024-03-28 22:06:00.000000 bioencoder-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     6178 2024-04-18 21:46:07.548730 bioencoder-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5283 2024-04-18 21:24:57.000000 bioencoder-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 21:46:07.273192 bioencoder-0.2.0/bioencoder/
--rw-rw-rw-   0        0        0      532 2024-03-28 22:17:18.000000 bioencoder-0.2.0/bioencoder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 21:46:07.385000 bioencoder-0.2.0/bioencoder/core/
--rw-rw-rw-   0        0        0      205 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/__init__.py
--rw-rw-rw-   0        0        0     2218 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/augmentations.py
--rw-rw-rw-   0        0        0      213 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/backbones.py
--rw-rw-rw-   0        0        0     2072 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/datasets.py
--rw-rw-rw-   0        0        0     6357 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/losses.py
--rw-rw-rw-   0        0        0     4594 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/core/models.py
--rw-rw-rw-   0        0        0      281 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/optimizers.py
--rw-rw-rw-   0        0        0      368 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/schedulers.py
--rw-rw-rw-   0        0        0    21555 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-18 21:46:07.493074 bioencoder-0.2.0/bioencoder/scripts/
--rw-rw-rw-   0        0        0      188 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/scripts/__init__.py
--rw-rw-rw-   0        0        0     4561 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/archive.py
--rw-rw-rw-   0        0        0     2971 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/configure.py
--rw-rw-rw-   0        0        0     5195 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/interactive_plots.py
--rw-rw-rw-   0        0        0     4891 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/lr_finder.py
--rw-rw-rw-   0        0        0     5941 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/model_explorer.py
--rw-rw-rw-   0        0        0      732 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/scripts/model_explorer_wrapper.py
--rw-rw-rw-   0        0        0    11228 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/split_dataset.py
--rw-rw-rw-   0        0        0     4338 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/swa.py
--rw-rw-rw-   0        0        0    13758 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/train.py
-drwxrwxrwx   0        0        0        0 2024-04-18 21:46:07.544704 bioencoder-0.2.0/bioencoder/vis/
--rw-rw-rw-   0        0        0       70 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/vis/__init__.py
--rw-rw-rw-   0        0        0    11283 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/vis/classes.py
--rw-rw-rw-   0        0        0     9856 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/vis/helpers.py
--rw-rw-rw-   0        0        0     6720 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/vis/methods.py
--rw-rw-rw-   0        0        0    14028 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/vis/methods_backup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 21:46:07.547218 bioencoder-0.2.0/bioencoder.egg-info/
--rw-rw-rw-   0        0        0     6178 2024-04-18 21:46:07.000000 bioencoder-0.2.0/bioencoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1008 2024-04-18 21:46:07.000000 bioencoder-0.2.0/bioencoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 21:46:07.000000 bioencoder-0.2.0/bioencoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      432 2024-04-18 21:46:07.000000 bioencoder-0.2.0/bioencoder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      212 2024-04-18 21:46:07.000000 bioencoder-0.2.0/bioencoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       45 2024-04-18 21:46:07.000000 bioencoder-0.2.0/bioencoder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1159 2024-04-18 21:44:09.000000 bioencoder-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      227 2024-03-11 21:33:49.000000 bioencoder-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 21:46:07.549732 bioencoder-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 21:06:19.036723 bioencoder-0.2.1/
+-rw-rw-rw-   0        0        0     1126 2024-03-28 22:06:00.000000 bioencoder-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     6296 2024-04-30 21:06:19.035723 bioencoder-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5401 2024-04-30 21:01:37.000000 bioencoder-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 21:06:18.828169 bioencoder-0.2.1/bioencoder/
+-rw-rw-rw-   0        0        0      532 2024-03-28 22:17:18.000000 bioencoder-0.2.1/bioencoder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 21:06:18.921994 bioencoder-0.2.1/bioencoder/core/
+-rw-rw-rw-   0        0        0      205 2024-03-11 21:33:49.000000 bioencoder-0.2.1/bioencoder/core/__init__.py
+-rw-rw-rw-   0        0        0     2218 2024-03-11 21:33:49.000000 bioencoder-0.2.1/bioencoder/core/augmentations.py
+-rw-rw-rw-   0        0        0      213 2024-03-11 21:33:49.000000 bioencoder-0.2.1/bioencoder/core/backbones.py
+-rw-rw-rw-   0        0        0     2072 2024-03-11 21:33:49.000000 bioencoder-0.2.1/bioencoder/core/datasets.py
+-rw-rw-rw-   0        0        0     6357 2024-03-11 21:33:49.000000 bioencoder-0.2.1/bioencoder/core/losses.py
+-rw-rw-rw-   0        0        0     4594 2024-04-18 21:43:24.000000 bioencoder-0.2.1/bioencoder/core/models.py
+-rw-rw-rw-   0        0        0      281 2024-03-11 21:33:49.000000 bioencoder-0.2.1/bioencoder/core/optimizers.py
+-rw-rw-rw-   0        0        0      368 2024-03-11 21:33:49.000000 bioencoder-0.2.1/bioencoder/core/schedulers.py
+-rw-rw-rw-   0        0        0    21555 2024-04-18 21:43:24.000000 bioencoder-0.2.1/bioencoder/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 21:06:18.995122 bioencoder-0.2.1/bioencoder/scripts/
+-rw-rw-rw-   0        0        0      188 2024-03-11 21:33:49.000000 bioencoder-0.2.1/bioencoder/scripts/__init__.py
+-rw-rw-rw-   0        0        0     4561 2024-04-18 21:43:24.000000 bioencoder-0.2.1/bioencoder/scripts/archive.py
+-rw-rw-rw-   0        0        0     2971 2024-04-18 21:43:24.000000 bioencoder-0.2.1/bioencoder/scripts/configure.py
+-rw-rw-rw-   0        0        0     5487 2024-04-30 21:01:37.000000 bioencoder-0.2.1/bioencoder/scripts/interactive_plots.py
+-rw-rw-rw-   0        0        0     4891 2024-04-18 21:43:24.000000 bioencoder-0.2.1/bioencoder/scripts/lr_finder.py
+-rw-rw-rw-   0        0        0     5941 2024-04-18 21:43:24.000000 bioencoder-0.2.1/bioencoder/scripts/model_explorer.py
+-rw-rw-rw-   0        0        0      732 2024-03-11 21:33:49.000000 bioencoder-0.2.1/bioencoder/scripts/model_explorer_wrapper.py
+-rw-rw-rw-   0        0        0    11228 2024-04-18 21:43:24.000000 bioencoder-0.2.1/bioencoder/scripts/split_dataset.py
+-rw-rw-rw-   0        0        0     4338 2024-04-18 21:43:24.000000 bioencoder-0.2.1/bioencoder/scripts/swa.py
+-rw-rw-rw-   0        0        0    13758 2024-04-18 21:43:24.000000 bioencoder-0.2.1/bioencoder/scripts/train.py
+drwxrwxrwx   0        0        0        0 2024-04-30 21:06:19.033717 bioencoder-0.2.1/bioencoder/vis/
+-rw-rw-rw-   0        0        0       70 2024-03-11 21:33:49.000000 bioencoder-0.2.1/bioencoder/vis/__init__.py
+-rw-rw-rw-   0        0        0    11283 2024-03-11 21:33:49.000000 bioencoder-0.2.1/bioencoder/vis/classes.py
+-rw-rw-rw-   0        0        0     9811 2024-04-30 21:01:37.000000 bioencoder-0.2.1/bioencoder/vis/helpers.py
+-rw-rw-rw-   0        0        0     6720 2024-03-11 21:33:49.000000 bioencoder-0.2.1/bioencoder/vis/methods.py
+-rw-rw-rw-   0        0        0    14028 2024-03-11 21:33:49.000000 bioencoder-0.2.1/bioencoder/vis/methods_backup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 21:06:19.034725 bioencoder-0.2.1/bioencoder.egg-info/
+-rw-rw-rw-   0        0        0     6296 2024-04-30 21:06:18.000000 bioencoder-0.2.1/bioencoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1008 2024-04-30 21:06:18.000000 bioencoder-0.2.1/bioencoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 21:06:18.000000 bioencoder-0.2.1/bioencoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      432 2024-04-30 21:06:18.000000 bioencoder-0.2.1/bioencoder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      212 2024-04-30 21:06:18.000000 bioencoder-0.2.1/bioencoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       45 2024-04-30 21:06:18.000000 bioencoder-0.2.1/bioencoder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1159 2024-04-30 21:03:44.000000 bioencoder-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      227 2024-03-11 21:33:49.000000 bioencoder-0.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 21:06:19.036723 bioencoder-0.2.1/setup.cfg
```

### Comparing `bioencoder-0.2.0/LICENSE` & `bioencoder-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/PKG-INFO` & `bioencoder-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioencoder
-Version: 0.2.0
+Version: 0.2.1
 Summary: A metric learning toolkit
 Author-email: Arthur Porto <agporto@gmail.com>, Moritz Lürig <moritz.luerig@gmail.com>
 Project-URL: Homepage, https://github.com/agporto/BioEncoder
 Project-URL: Bug Tracker, https://github.com/agporto/BioEncoder/issues
 Keywords: metric learning,biology
 Requires-Python: ==3.9.*
 Description-Content-Type: text/markdown
@@ -29,14 +29,16 @@
     <p><img src="https://github.com/agporto/BioEncoder/raw/main/assets/bioencoder_logo.png" width="300"></p>
 </div>
 
 # BioEncoder
 
 BioEncoder is a tool box for image classification and trait discovery in organismal biology. It relies on image classification models trained using metric learning to learn species trait data  (i.e., features) from images. This implementation is based on [SupCon](https://github.com/ivanpanshin/SupCon-Framework) and [timm-vis](https://github.com/novice03/timm-vis). 
 
+Preprint on BioRxiv: [https://doi.org/10.1101/2024.04.03.587987]( https://doi.org/10.1101/2024.04.03.587987)
+
 ## Features
 - Taxon-agnostic dataloaders (making it applicable to any dataset - not just biological ones)
 - Support of [timm models](https://github.com/rwightman/pytorch-image-models), and [pytorch-optimizer](https://github.com/jettify/pytorch-optimizer)
 - Access to state-of-the-art metric losses, such as [Supcon](https://arxiv.org/abs/2004.11362) and  [Sub-center ArcFace](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123560715.pdf).
 - [Exponential Moving Average](https://github.com/fadel/pytorch_ema) for stable training, and Stochastic Moving Average for better generalization and performance.
 - [LRFinder](https://github.com/davidtvs/pytorch-lr-finder) for the second stage of the training.
 - Easy customization of hyperparameters, including augmentations, through `YAML` configs (check the [config-templates](config-templates) folder for examples)
@@ -65,15 +67,15 @@
 
 ```python
 ## use "overwrite=True to redo a step
 
 import bioencoder
 
 ## global setup
-bioencoder.configure(root_dir=r"bioencoder_wd", run_name="v1")
+bioencoder.configure(root_dir=r"~/bioencoder_wd", run_name="v1")
 
 ## split dataset
 bioencoder.split_dataset(image_dir=r"~/Downloads/damselflies-aligned-trai_val", max_ratio=6, random_seed=42)
 
 ## train stage 1
 bioencoder.train(config_path=r"bioencoder_configs/train_stage1.yml")
 bioencoder.swa(config_path=r"bioencoder_configs/swa_stage1.yml")
@@ -94,15 +96,15 @@
 
 ```
 4\. Alternatively, you can directly use the command line interface: 
 
 ```python
 ## use the flag "--overwrite" to redo a step
 
-bioencoder_configure --root-dir bioencoder_wd --run-name v1
+bioencoder_configure --root-dir "~/bioencoder_wd" --run-name v1
 bioencoder_split_dataset --image-dir "~/Downloads/damselflies-aligned-trai_val" --max-ratio 6 --random-seed 42
 bioencoder_train --config-path "bioencoder_configs/train_stage1.yml"
 bioencoder_swa --config-path "bioencoder_configs/swa_stage1.yml"
 bioencoder_interactive_plots --config-path "bioencoder_configs/plot_stage1.yml"
 bioencoder_model_explorer --config-path "bioencoder_configs/explore_stage1.yml"
 bioencoder_lr_finder --config-path "bioencoder_configs/lr_finder.yml"
 bioencoder_train --config-path "bioencoder_configs/train_stage2.yml"
```

### Comparing `bioencoder-0.2.0/README.md` & `bioencoder-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,16 @@
     <p><img src="https://github.com/agporto/BioEncoder/raw/main/assets/bioencoder_logo.png" width="300"></p>
 </div>
 
 # BioEncoder
 
 BioEncoder is a tool box for image classification and trait discovery in organismal biology. It relies on image classification models trained using metric learning to learn species trait data  (i.e., features) from images. This implementation is based on [SupCon](https://github.com/ivanpanshin/SupCon-Framework) and [timm-vis](https://github.com/novice03/timm-vis). 
 
+Preprint on BioRxiv: [https://doi.org/10.1101/2024.04.03.587987]( https://doi.org/10.1101/2024.04.03.587987)
+
 ## Features
 - Taxon-agnostic dataloaders (making it applicable to any dataset - not just biological ones)
 - Support of [timm models](https://github.com/rwightman/pytorch-image-models), and [pytorch-optimizer](https://github.com/jettify/pytorch-optimizer)
 - Access to state-of-the-art metric losses, such as [Supcon](https://arxiv.org/abs/2004.11362) and  [Sub-center ArcFace](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123560715.pdf).
 - [Exponential Moving Average](https://github.com/fadel/pytorch_ema) for stable training, and Stochastic Moving Average for better generalization and performance.
 - [LRFinder](https://github.com/davidtvs/pytorch-lr-finder) for the second stage of the training.
 - Easy customization of hyperparameters, including augmentations, through `YAML` configs (check the [config-templates](config-templates) folder for examples)
@@ -38,15 +40,15 @@
 
 ```python
 ## use "overwrite=True to redo a step
 
 import bioencoder
 
 ## global setup
-bioencoder.configure(root_dir=r"bioencoder_wd", run_name="v1")
+bioencoder.configure(root_dir=r"~/bioencoder_wd", run_name="v1")
 
 ## split dataset
 bioencoder.split_dataset(image_dir=r"~/Downloads/damselflies-aligned-trai_val", max_ratio=6, random_seed=42)
 
 ## train stage 1
 bioencoder.train(config_path=r"bioencoder_configs/train_stage1.yml")
 bioencoder.swa(config_path=r"bioencoder_configs/swa_stage1.yml")
@@ -67,15 +69,15 @@
 
 ```
 4\. Alternatively, you can directly use the command line interface: 
 
 ```python
 ## use the flag "--overwrite" to redo a step
 
-bioencoder_configure --root-dir bioencoder_wd --run-name v1
+bioencoder_configure --root-dir "~/bioencoder_wd" --run-name v1
 bioencoder_split_dataset --image-dir "~/Downloads/damselflies-aligned-trai_val" --max-ratio 6 --random-seed 42
 bioencoder_train --config-path "bioencoder_configs/train_stage1.yml"
 bioencoder_swa --config-path "bioencoder_configs/swa_stage1.yml"
 bioencoder_interactive_plots --config-path "bioencoder_configs/plot_stage1.yml"
 bioencoder_model_explorer --config-path "bioencoder_configs/explore_stage1.yml"
 bioencoder_lr_finder --config-path "bioencoder_configs/lr_finder.yml"
 bioencoder_train --config-path "bioencoder_configs/train_stage2.yml"
```

### Comparing `bioencoder-0.2.0/bioencoder/__init__.py` & `bioencoder-0.2.1/bioencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/core/augmentations.py` & `bioencoder-0.2.1/bioencoder/core/augmentations.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/core/datasets.py` & `bioencoder-0.2.1/bioencoder/core/datasets.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/core/losses.py` & `bioencoder-0.2.1/bioencoder/core/losses.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/core/models.py` & `bioencoder-0.2.1/bioencoder/core/models.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/core/utils.py` & `bioencoder-0.2.1/bioencoder/core/utils.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/scripts/archive.py` & `bioencoder-0.2.1/bioencoder/scripts/archive.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/scripts/configure.py` & `bioencoder-0.2.1/bioencoder/scripts/configure.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/scripts/interactive_plots.py` & `bioencoder-0.2.1/bioencoder/scripts/interactive_plots.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import argparse
 import yaml
+import numpy as np
 import pandas as pd
 import torch
 
 from pathlib import Path
 
 from bioencoder.core import utils
 from bioencoder.vis import helpers
@@ -53,32 +54,24 @@
     run_name = config.run_name
     
     ## load config
     hyperparams = utils.load_yaml(config_path)
     
     ## parse config
     backbone = hyperparams["model"]["backbone"]
-    stage = hyperparams["model"]["stage"]
+    num_classes = hyperparams["model"].get("num_classes", None)
+    checkpoint = hyperparams["model"].get("checkpoint", "swa")
+    stage = hyperparams["model"].get("stage", "first")
     batch_sizes = {
         "train_batch_size": hyperparams["dataloaders"]["train_batch_size"],
         "valid_batch_size": hyperparams["dataloaders"]["valid_batch_size"],
     }
     num_workers = hyperparams["dataloaders"]["num_workers"]
-    color_classes = hyperparams.get("color_classes")
-
-    ## manage second stage
-    if stage == "second":
-        num_classes = hyperparams["model"]["num_classes"]
-    else:
-        num_classes = None
-
-    ## set cuda device
-    cuda_device = kwargs.get("cuda_device",0)
-    torch.cuda.set_device(cuda_device)
-    print(f"Using CUDA device {cuda_device}")
+    color_classes = hyperparams.get("color_classes", None)
+    color_map = hyperparams.get("color_map", "jet")
 
     ## init scaler
     scaler = torch.cuda.amp.GradScaler()
     
     ## set up dirs
     data_dir = os.path.join(root_dir,"data",  run_name)
     plot_dir = os.path.join(root_dir, "plots")
@@ -86,40 +79,41 @@
     
     ## plot path
     plot_path = os.path.join(plot_dir, f"{run_name}.html")
     if not overwrite and not kwargs.get("ret_embeddings"):
         assert not os.path.isfile(plot_path), f"File exists: {plot_path}"
     
     ## load weights
-    ckpt_pretrained = os.path.join(config.root_dir, "weights", run_name, stage, "swa")
+    print(f"Checkpoint: using {checkpoint} of {stage} stage")
+    ckpt_pretrained = os.path.join(config.root_dir, "weights", run_name, stage, checkpoint)
 
     ## set random seed
     utils.set_seed()
 
+    ## extract embeddings
     transforms = utils.build_transforms(hyperparams)
     loaders = utils.build_loaders(
         data_dir, transforms, batch_sizes, num_workers, second_stage=(stage == "second")
     )
     model = utils.build_model(
         backbone,
         second_stage=(stage == "second"),
         num_classes=num_classes,
         ckpt_pretrained=ckpt_pretrained,
-        cuda_device=cuda_device,
     ).cuda()
     model.use_projection_head(False)
     model.eval()
-
     embeddings_train, labels_train = utils.compute_embeddings(
         loaders["valid_loader"], model, scaler
     )
     
-
+    ## load dataset
     paths_train = [item[0] for item in loaders["valid_loader"].dataset.imgs]
     
+    ## return embeddings without plotting
     if kwargs.get("ret_embeddings"):
         
         df = pd.DataFrame([os.path.basename(item) for item in paths_train], columns=["image_name"])
         df["class"] = [
             os.path.basename(os.path.dirname(item[0])) for item in loaders["valid_loader"].dataset.imgs
         ]
         return pd.concat([df, pd.DataFrame(embeddings_train)], axis=1)
@@ -133,15 +127,19 @@
         os.path.join("..", "..", item) for item in paths_train
     ]
     df["class"] = labels_train
     df["class_str"] = [
         os.path.basename(os.path.dirname(item[0])) for item in loaders["valid_loader"].dataset.imgs
     ]
     
-    helpers.bokeh_plot(df, out_path=plot_path, color_classes=color_classes)
+    ## check if color matches n classes
+    if color_classes:
+        assert len(np.unique(labels_train)) == len(color_classes), f"Number of classes is {len(np.unique(labels_train))}, but you only provided {len(color_classes)} colors"
+    
+    helpers.bokeh_plot(df, out_path=plot_path, color_map=color_map, color_classes=color_classes)
     
     
 def cli():
 
     parser = argparse.ArgumentParser()
     parser.add_argument( "--config-path",type=str, help="Path to the YAML configuration file to create interactive plots.")
     parser.add_argument("--overwrite", action='store_true', help="Overwrite existing files without asking.")
```

### Comparing `bioencoder-0.2.0/bioencoder/scripts/lr_finder.py` & `bioencoder-0.2.1/bioencoder/scripts/lr_finder.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/scripts/model_explorer.py` & `bioencoder-0.2.1/bioencoder/scripts/model_explorer.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/scripts/model_explorer_wrapper.py` & `bioencoder-0.2.1/bioencoder/scripts/model_explorer_wrapper.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/scripts/split_dataset.py` & `bioencoder-0.2.1/bioencoder/scripts/split_dataset.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/scripts/swa.py` & `bioencoder-0.2.1/bioencoder/scripts/swa.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/scripts/train.py` & `bioencoder-0.2.1/bioencoder/scripts/train.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/vis/classes.py` & `bioencoder-0.2.1/bioencoder/vis/classes.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/vis/helpers.py` & `bioencoder-0.2.1/bioencoder/vis/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,15 +230,15 @@
     pca_obj = decomposition.PCA(n_components=2)
     pca = pca_obj.fit_transform(norm_data)
     tsne = manifold.TSNE(learning_rate='auto', init='pca').fit_transform(norm_data)
     names = ['PC1', 'PC2', 'tSNE-0', 'tSNE-1']
     return np.hstack((pca, tsne)), names, pca_obj
 
 
-def bokeh_plot(df, out_path='plot.html', **kwargs):
+def bokeh_plot(df, out_path='plot.html', color_map="jet", color_classes=None, **kwargs):
     """
     Plot a scatter plot of the PCA and t-SNE dimensions of the data using bokeh.
 
     Parameters:
     df (pandas.DataFrame): The dataframe containing the data to plot. The dataframe must have
                            two columns: 'paths' (the file paths of the images) and 'class' (the
                            class labels of the images).
@@ -268,22 +268,21 @@
             </div>
         </div>
               """
     filenames = df['paths']
     df['image_files'] = filenames
     
     ## color management
-    color_classes = kwargs.get("color_classes")
-    if not color_classes.__class__.__name__ == "NoneType":
+    if color_classes:
         df_col = pd.DataFrame.from_dict(color_classes.items())
         df_col.columns = ["class_str","color"]
         df = df.merge(df_col)
     else:
         num_classes = len(df['class'].unique())
-        cmap=plt.cm.get_cmap("jet", num_classes)
+        cmap=plt.cm.get_cmap(color_map, num_classes)
         colors_raw = cmap((df['class']), bytes=True)
         colors_str = ['#%02x%02x%02x' % tuple(c[:3]) for c in colors_raw]
         df['color'] = colors_str
         
     source = ColumnDataSource(df)
     bplot.output_file(out_path)
     hover0 = HoverTool(tooltips=tooltip)
```

### Comparing `bioencoder-0.2.0/bioencoder/vis/methods.py` & `bioencoder-0.2.1/bioencoder/vis/methods.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder/vis/methods_backup.py` & `bioencoder-0.2.1/bioencoder/vis/methods_backup.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/bioencoder.egg-info/PKG-INFO` & `bioencoder-0.2.1/bioencoder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioencoder
-Version: 0.2.0
+Version: 0.2.1
 Summary: A metric learning toolkit
 Author-email: Arthur Porto <agporto@gmail.com>, Moritz Lürig <moritz.luerig@gmail.com>
 Project-URL: Homepage, https://github.com/agporto/BioEncoder
 Project-URL: Bug Tracker, https://github.com/agporto/BioEncoder/issues
 Keywords: metric learning,biology
 Requires-Python: ==3.9.*
 Description-Content-Type: text/markdown
@@ -29,14 +29,16 @@
     <p><img src="https://github.com/agporto/BioEncoder/raw/main/assets/bioencoder_logo.png" width="300"></p>
 </div>
 
 # BioEncoder
 
 BioEncoder is a tool box for image classification and trait discovery in organismal biology. It relies on image classification models trained using metric learning to learn species trait data  (i.e., features) from images. This implementation is based on [SupCon](https://github.com/ivanpanshin/SupCon-Framework) and [timm-vis](https://github.com/novice03/timm-vis). 
 
+Preprint on BioRxiv: [https://doi.org/10.1101/2024.04.03.587987]( https://doi.org/10.1101/2024.04.03.587987)
+
 ## Features
 - Taxon-agnostic dataloaders (making it applicable to any dataset - not just biological ones)
 - Support of [timm models](https://github.com/rwightman/pytorch-image-models), and [pytorch-optimizer](https://github.com/jettify/pytorch-optimizer)
 - Access to state-of-the-art metric losses, such as [Supcon](https://arxiv.org/abs/2004.11362) and  [Sub-center ArcFace](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123560715.pdf).
 - [Exponential Moving Average](https://github.com/fadel/pytorch_ema) for stable training, and Stochastic Moving Average for better generalization and performance.
 - [LRFinder](https://github.com/davidtvs/pytorch-lr-finder) for the second stage of the training.
 - Easy customization of hyperparameters, including augmentations, through `YAML` configs (check the [config-templates](config-templates) folder for examples)
@@ -65,15 +67,15 @@
 
 ```python
 ## use "overwrite=True to redo a step
 
 import bioencoder
 
 ## global setup
-bioencoder.configure(root_dir=r"bioencoder_wd", run_name="v1")
+bioencoder.configure(root_dir=r"~/bioencoder_wd", run_name="v1")
 
 ## split dataset
 bioencoder.split_dataset(image_dir=r"~/Downloads/damselflies-aligned-trai_val", max_ratio=6, random_seed=42)
 
 ## train stage 1
 bioencoder.train(config_path=r"bioencoder_configs/train_stage1.yml")
 bioencoder.swa(config_path=r"bioencoder_configs/swa_stage1.yml")
@@ -94,15 +96,15 @@
 
 ```
 4\. Alternatively, you can directly use the command line interface: 
 
 ```python
 ## use the flag "--overwrite" to redo a step
 
-bioencoder_configure --root-dir bioencoder_wd --run-name v1
+bioencoder_configure --root-dir "~/bioencoder_wd" --run-name v1
 bioencoder_split_dataset --image-dir "~/Downloads/damselflies-aligned-trai_val" --max-ratio 6 --random-seed 42
 bioencoder_train --config-path "bioencoder_configs/train_stage1.yml"
 bioencoder_swa --config-path "bioencoder_configs/swa_stage1.yml"
 bioencoder_interactive_plots --config-path "bioencoder_configs/plot_stage1.yml"
 bioencoder_model_explorer --config-path "bioencoder_configs/explore_stage1.yml"
 bioencoder_lr_finder --config-path "bioencoder_configs/lr_finder.yml"
 bioencoder_train --config-path "bioencoder_configs/train_stage2.yml"
```

### Comparing `bioencoder-0.2.0/bioencoder.egg-info/SOURCES.txt` & `bioencoder-0.2.1/bioencoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioencoder-0.2.0/pyproject.toml` & `bioencoder-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 	{name = "Moritz Lürig", email = "moritz.luerig@gmail.com"},
 	]
 description = "A metric learning toolkit"
 readme = "README.md"
 requires-python = "==3.9.*"
 keywords = ["metric learning", "biology"]
 dynamic = ["dependencies"]
-version = "0.2.0"
+version = "0.2.1"
 
 [project.urls]
 "Homepage" = "https://github.com/agporto/BioEncoder"
 "Bug Tracker" = "https://github.com/agporto/BioEncoder/issues"
 
 [project.scripts]
 bioencoder_configure = "bioencoder.scripts.configure:cli"
```

