# Comparing `tmp/fse_baro-0.1.8.tar.gz` & `tmp/fse_baro-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fse_baro-0.1.8.tar", last modified: Tue Apr 30 03:32:43 2024, max compression
+gzip compressed data, was "fse_baro-0.1.9.tar", last modified: Tue Apr 30 14:18:15 2024, max compression
```

## Comparing `fse_baro-0.1.8.tar` & `fse_baro-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.866862 fse_baro-0.1.8/.circleci/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-30 03:32:38.000000 fse_baro-0.1.8/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.866862 fse_baro-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-30 03:32:38.000000 fse_baro-0.1.8/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-30 03:32:38.000000 fse_baro-0.1.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-30 03:32:38.000000 fse_baro-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 03:32:38.000000 fse_baro-0.1.8/ENHANCEMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-30 03:32:38.000000 fse_baro-0.1.8/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-30 03:32:38.000000 fse_baro-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-30 03:32:43.870862 fse_baro-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-04-30 03:32:38.000000 fse_baro-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 03:32:38.000000 fse_baro-0.1.8/REQUIREMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-30 03:32:38.000000 fse_baro-0.1.8/STATUS.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/baro/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 03:32:38.000000 fse_baro-0.1.8/baro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-30 03:32:38.000000 fse_baro-0.1.8/baro/_bocpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-30 03:32:38.000000 fse_baro-0.1.8/baro/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-30 03:32:38.000000 fse_baro-0.1.8/baro/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-30 03:32:38.000000 fse_baro-0.1.8/baro/root_cause_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-30 03:32:38.000000 fse_baro-0.1.8/baro/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-30 03:32:38.000000 fse_baro-0.1.8/docs/running_time_and_instrumentation_cost.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/fse_baro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-30 03:32:43.000000 fse_baro-0.1.8/fse_baro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-30 03:32:43.000000 fse_baro-0.1.8/fse_baro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 03:32:43.000000 fse_baro-0.1.8/fse_baro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 03:32:43.000000 fse_baro-0.1.8/fse_baro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 03:32:43.000000 fse_baro-0.1.8/fse_baro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-30 03:32:38.000000 fse_baro-0.1.8/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-30 03:32:38.000000 fse_baro-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 03:32:43.870862 fse_baro-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-30 03:32:38.000000 fse_baro-0.1.8/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-30 03:32:38.000000 fse_baro-0.1.8/tutorials/reproduce_multivariate_bocpd.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-30 03:32:38.000000 fse_baro-0.1.8/tutorials/reproducibility.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:18:15.156154 fse_baro-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:18:15.148153 fse_baro-0.1.9/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-30 14:18:06.000000 fse_baro-0.1.9/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:18:15.148153 fse_baro-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:18:15.148153 fse_baro-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-30 14:18:06.000000 fse_baro-0.1.9/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-30 14:18:06.000000 fse_baro-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-30 14:18:06.000000 fse_baro-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 14:18:06.000000 fse_baro-0.1.9/ENHANCEMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-30 14:18:06.000000 fse_baro-0.1.9/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-30 14:18:06.000000 fse_baro-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-04-30 14:18:15.156154 fse_baro-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-04-30 14:18:06.000000 fse_baro-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-30 14:18:06.000000 fse_baro-0.1.9/REQUIREMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-30 14:18:06.000000 fse_baro-0.1.9/STATUS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:18:15.152153 fse_baro-0.1.9/baro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:18:06.000000 fse_baro-0.1.9/baro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-30 14:18:06.000000 fse_baro-0.1.9/baro/_bocpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-30 14:18:06.000000 fse_baro-0.1.9/baro/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-04-30 14:18:06.000000 fse_baro-0.1.9/baro/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-30 14:18:06.000000 fse_baro-0.1.9/baro/root_cause_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-30 14:18:06.000000 fse_baro-0.1.9/baro/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:18:15.152153 fse_baro-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)  1260165 2024-04-30 14:18:06.000000 fse_baro-0.1.9/docs/fse_baro_supplementary_material.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-30 14:18:06.000000 fse_baro-0.1.9/docs/running_time_and_instrumentation_cost.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:18:15.156154 fse_baro-0.1.9/fse_baro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-04-30 14:18:15.000000 fse_baro-0.1.9/fse_baro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-30 14:18:15.000000 fse_baro-0.1.9/fse_baro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:18:15.000000 fse_baro-0.1.9/fse_baro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 14:18:15.000000 fse_baro-0.1.9/fse_baro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 14:18:15.000000 fse_baro-0.1.9/fse_baro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-30 14:18:06.000000 fse_baro-0.1.9/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-30 14:18:06.000000 fse_baro-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:18:15.156154 fse_baro-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:18:15.152153 fse_baro-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-30 14:18:06.000000 fse_baro-0.1.9/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:18:15.156154 fse_baro-0.1.9/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)   961218 2024-04-30 14:18:06.000000 fse_baro-0.1.9/tutorials/how-to-use-baro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-30 14:18:06.000000 fse_baro-0.1.9/tutorials/reproduce_multivariate_bocpd.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-30 14:18:06.000000 fse_baro-0.1.9/tutorials/reproducibility.ipynb
```

### Comparing `fse_baro-0.1.8/.circleci/config.yml` & `fse_baro-0.1.9/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.8/.github/workflows/build-and-test.yml` & `fse_baro-0.1.9/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.8/.github/workflows/python-publish.yml` & `fse_baro-0.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.8/.gitignore` & `fse_baro-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.8/LICENSE` & `fse_baro-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.8/REQUIREMENTS.md` & `fse_baro-0.1.9/REQUIREMENTS.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ## Operating System & Hardware
-We recommend using machines equipped with at least 8 cores and 16GB RAM with **Ubuntu 20.04** or **Ubuntu 22.04** to stably reproduce the experimental results in our paper.  
+We recommend using machines equipped with at least 8 cores, 16GB RAM, and ~10GB available disk space with **Ubuntu 20.04** or **Ubuntu 22.04** to stably reproduce the experimental results in our paper.  
 
 ## Software
 
 - We develop BARO using Python 3.10.
 - We encourage user to create a virtual environment to use BARO (e.g., `python3.10 -m venv env`).
 - BARO could be installed using pip. (e.g., `pip install fse-baro`).
-- BARO requires "numpy", "pandas", "scikit-learn" packages. The dependencies are described in the [pyproject.toml](pyproject.toml) file.
+- BARO requires the following packages: "numpy", "pandas", "scikit-learn", "pytest", "tqdm", "requests", and "matplotlib". These dependencies are described in the [pyproject.toml](pyproject.toml) file.  We adhere to [PEP 735](https://peps.python.org/pep-0735/) for storing package requirements in the `pyproject.toml` file rather than the `requirements.txt` file.
+
```

### Comparing `fse_baro-0.1.8/baro/_bocpd.py` & `fse_baro-0.1.9/baro/_bocpd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# The code is shamelessly copied and developed from 
+# Acknowledgement: The code is copied and developed from 
 # https://github.com/hildensia/bayesian_changepoint_detection/tree/master/bayesian_changepoint_detection
+
 from abc import ABC, abstractmethod
 
 import numpy as np
 import scipy.stats as ss
 from itertools import islice
 from numpy.linalg import inv
 from functools import partial
```

### Comparing `fse_baro-0.1.8/baro/reproducibility.py` & `fse_baro-0.1.9/baro/reproducibility.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,14 +22,22 @@
 )
 from baro._bocpd import online_changepoint_detection, partial, constant_hazard, MultivariateT
 from baro.anomaly_detection import bocpd
 from baro.root_cause_analysis import robust_scorer
 
 
 def reproduce_baro(dataset=None, fault=None):
+    """Reproduce BARO results for the given dataset and fault type.
+    
+    Parameters:
+    - dataset : str, optional
+        The dataset to reproduce results for. Supported values are "fse-ob" (Online Boutique), "fse-ss" (Sock Shop), and "fse-tt" (Train Ticket).
+    - fault : str, optional
+        The type of fault to consider. Supported values are "cpu", "mem", "delay", "loss", or "all" (for all fault types). Default is None.
+    """
     assert dataset in ["fse-ob", "fse-ss", "fse-tt"], f"{dataset} is not supported!"
     assert fault in [None, "all", "cpu", "mem", "delay", "loss"], f"{fault} is not supported!"
     if fault is None:
         fault = "all"
     
     if not os.path.exists(f"data/{dataset}"):
         if dataset == "fse-ob":
@@ -86,14 +94,22 @@
     print(f"Dataset   : {dataset}")
     print(f"Fault type: {fault}")
     print(f"Avg@5 Acc : {avg5_accuracy:.2f}")
     print()
     
 
 def reproduce_bocpd(dataset=None, saved=False):
+    """Reproduce Multivariate BOCPD results for the given dataset.
+    
+    Parameters:
+    - dataset : str, optional
+        The dataset to reproduce results for. Supported values are "fse-ob" (Online Boutique), "fse-ss" (Sock Shop), and "fse-tt" (Train Ticket).
+    - saved : bool, optional
+        If True, load precomputed results. If False, run BOCPD algorithm again. Default is False.
+    """
     assert dataset in ["fse-ob", "fse-ss", "fse-tt"], f"{dataset} is not supported!"
     
     if not os.path.exists(f"data/{dataset}"):
         if dataset == "fse-ob":
             download_online_boutique_dataset()
         elif dataset == "fse-ss":
             download_sock_shop_dataset()
@@ -163,8 +179,83 @@
     precision = tp / (tp + fp)
     recall = tp / (tp + fn)
     f1 = 2 * precision * recall / (precision + recall)
     print("====== Reproduce BOCPD =====")
     print(f"Dataset: {dataset}")
     print(f"Precision: {precision:.2f}")
     print(f"Recall   : {recall:.2f}")
-    print(f"F1       : {f1:.2f}")
+    print(f"F1       : {f1:.2f}")
+    
+    
+    
+def reproduce_rq4(dataset=None, eval_metric=None):
+    """Reproduce RQ4 results for the given dataset and evaluation metric.
+    
+    Parameters:
+    - dataset : str, optional
+        The dataset to reproduce results for. Supported values are "fse-ob" (Online Boutique), "fse-ss" (Sock Shop), and "fse-tt" (Train Ticket).
+    - eval_metric : str, optional
+        The evaluation metric to use. Supported values are "top1", "top3", "avg5", or None (default, which equals to "avg5").
+    """
+    assert dataset in ["fse-ob", "fse-ss", "fse-tt"], f"{dataset} is not supported!"
+    assert eval_metric in [None, "top1", "top3", "avg5"], f"{eval_metric} is not supported!"
+    
+    if eval_metric is None:
+        eval_metric = "avg5"
+    
+    if not os.path.exists(f"data/{dataset}"):
+        if dataset == "fse-ob":
+            download_online_boutique_dataset()
+        elif dataset == "fse-ss":
+            download_sock_shop_dataset()
+        elif dataset == "fse-tt":
+            download_train_ticket_dataset()
+    
+    data_paths = list(glob.glob(f"./data/{dataset}/**/simple_data.csv", recursive=True))
+    
+    scores = []
+    for t_bias in tqdm(range(-40, 40, 2), desc="Running"):
+        top1_cnt, top2_cnt, top3_cnt, top4_cnt, top5_cnt, total_cnt = 0, 0, 0, 0, 0, 0
+
+        for data_path in data_paths:
+            # read data
+            data = read_data(data_path)
+            data_dir = os.path.dirname(data_path)
+            service, metric = basename(dirname(dirname(data_path))).split("_")
+
+            ############# READ INJECT TIME ###############
+            with open(join(data_dir, "inject_time.txt")) as f:
+                inject_time = int(f.readlines()[0].strip()) + t_bias
+
+            ############# ROOT CAUSE ANALYSIS ###############
+            ranks = robust_scorer(data, inject_time=inject_time)["ranks"]
+            service_ranks = to_service_ranks(ranks)
+
+            ############## EVALUATION ###############
+            if service in service_ranks[:1]:
+                top1_cnt += 1
+            if service in service_ranks[:2]:
+                top2_cnt += 1
+            if service in service_ranks[:3]:
+                top3_cnt += 1
+            if service in service_ranks[:4]:
+                top4_cnt += 1
+            if service in service_ranks[:5]:
+                top5_cnt += 1
+            total_cnt += 1
+
+        ############## EVALUATION ###############
+        top1_accuracy = top1_cnt / total_cnt
+        top2_accuracy = top2_cnt / total_cnt
+        top3_accuracy = top3_cnt / total_cnt
+        top4_accuracy = top4_cnt / total_cnt
+        top5_accuracy = top5_cnt / total_cnt
+        avg5_accuracy = (top1_accuracy + top2_accuracy + top3_accuracy + top4_accuracy + top5_accuracy) / 5
+        
+        if eval_metric == "top1":
+            scores.append(top1_accuracy)
+        elif eval_metric == "top3":
+            scores.append(top3_accuracy)
+        elif eval_metric == "avg5":
+            scores.append(avg5_accuracy)    
+            
+    print([round(s, 2) for s in scores])
```

### Comparing `fse_baro-0.1.8/baro/utility.py` & `fse_baro-0.1.9/baro/utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,87 +9,85 @@
 import numpy as np
 from tqdm import tqdm
 import pandas as pd
 import matplotlib.pyplot as plt
 
 
 def download_online_boutique_dataset(local_path=None):
-    """
-    Download the Online Boutique dataset from Zenodo.
-    """
+    """Download the Online Boutique dataset from Zenodo."""
     if local_path == None:
         local_path = "data"
     if not os.path.exists(local_path):
         os.makedirs(local_path)
     if os.path.exists(join(local_path, "fse-ob")):
         return
     download_data("https://zenodo.org/records/11046533/files/fse-ob.zip?download=1", "fse-ob.zip")
     with zipfile.ZipFile("fse-ob.zip", 'r') as file:
         file.extractall(local_path)
     os.remove("fse-ob.zip")
 
 
 def download_sock_shop_dataset(local_path=None):
-    """
-    Download the Sock Shop dataset from Zenodo. 
-    """
+    """Download the Sock Shop dataset from Zenodo."""
     if local_path == None:
         local_path = "data"
     if not os.path.exists(local_path):
         os.makedirs(local_path)
     if os.path.exists(join(local_path, "fse-ss")):
         return   
     download_data("https://zenodo.org/records/11046533/files/fse-ss.zip?download=1", "fse-ss.zip")
     with zipfile.ZipFile("fse-ss.zip", 'r') as file:
         file.extractall(local_path)
     os.remove("fse-ss.zip")
 
 
 def download_train_ticket_dataset(local_path=None):
-    """
-    Download the Train Ticket dataset from Zenodo. 
-    """
+    """Download the Train Ticket dataset from Zenodo."""
     if local_path == None:
         local_path = "data"
     if not os.path.exists(local_path):
         os.makedirs(local_path)
     if os.path.exists(join(local_path, "fse-tt")):
         return
     download_data("https://zenodo.org/records/11046533/files/fse-tt.zip?download=1", "fse-tt.zip")
     with zipfile.ZipFile("fse-tt.zip", 'r') as file:
         file.extractall(local_path)
     os.remove("fse-tt.zip")
     
 
 def load_json(filename: str):
+    """Load data from a JSON file."""
     with open(filename) as f:
         data = json.load(f)
     return data
               
               
 def drop_constant(df: pd.DataFrame):
+    """Drop constant columns from the DataFrame."""
     return df.loc[:, (df != df.iloc[0]).any()]
 
 
 def drop_near_constant(df: pd.DataFrame, threshold: float = 0.1):
+    """Drop columns with near-constant values from the DataFrame."""
     return df.loc[:, (df != df.iloc[0]).mean() > threshold]
 
 
 def drop_time(df: pd.DataFrame):
+    """Drop time-related columns from the DataFrame."""
     if "time" in df:
         df = df.drop(columns=["time"])
     if "Time" in df:
         df = df.drop(columns=["Time"])
     if "timestamp" in df:
         df = df.drop(columns=["timestamp"])
     return df
 
 
 def visualize_metrics(data: pd.DataFrame, filename=None, figsize=None):
-    """Visualize the metrics."""
+    """Visualize metrics from the DataFrame."""
     if figsize is None:
         figsize = (25, 25)
 
     data = drop_time(data)
     services = []
     metrics = []
     for c in data.columns:
@@ -124,15 +122,15 @@
         plt.savefig(filename)
 
     # close the figure
     plt.close(fig)
 
 
 def download_data(remote_url=None, local_path=None):
-    """Download sample metrics data""" 
+    """Download data from a remote URL."""
     if remote_url is None:
         remote_url = "https://github.com/phamquiluan/baro/releases/download/0.0.4/simple_data.csv"
     if local_path is None:
         local_path = "data.csv"
 
     response = requests.get(remote_url, stream=True)
     total_size_in_bytes = int(response.headers.get("content-length", 0))
@@ -152,15 +150,15 @@
 
     progress_bar.close()
     if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
         print("ERROR, something went wrong")
 
 
 def read_data(data_path, strip=True):
-    """Read csv data for root cause analysis."""    
+    """Read CSV data for root cause analysis."""
     data = pd.read_csv(data_path)
     data_dir = os.path.dirname(data_path)
 
     ############# PREPROCESSING ###############
     if "time.1" in data:
         data = data.drop(columns=["time.1"])
     data = data.replace([np.inf, -np.inf], np.nan)
@@ -185,15 +183,15 @@
             inject_time = int(f.readlines()[0].strip())
         normal_df = data[data["time"] < inject_time].tail(data_length)
         anomal_df = data[data["time"] >= inject_time].head(data_length)
         data = pd.concat([normal_df, anomal_df], ignore_index=True)    
     return data
 
 def to_service_ranks(ranks):
-    """Convert fine-grained ranking to service ranks"""
+    """Convert fine-grained ranking to service ranks."""
     _service_ranks = [r.split("_")[0] for r in ranks]
     service_ranks = []
     # remove duplicates
     for s in _service_ranks:
         if s not in service_ranks:
             service_ranks.append(s)
     return service_ranks
@@ -202,12 +200,13 @@
 def select_latency_and_error(data):
     """Select latency and error columns, retain `time` col"""
     latency_cols = [c for c in data.columns if "latency" in c]
     error_cols = [c for c in data.columns if "error" in c]
     return data[["time"] + latency_cols + error_cols]    
 
 def find_cps(maxes):
+    """Find change points given a `maxes` array."""
     cps = []
     for i in range(1, len(maxes)):
         if abs(maxes[i] - maxes[i-1]) > 1:
             cps.append((i, abs(maxes[i] - maxes[i-1])))
     return cps
```

### Comparing `fse_baro-0.1.8/docs/running_time_and_instrumentation_cost.md` & `fse_baro-0.1.9/docs/running_time_and_instrumentation_cost.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.8/main.py` & `fse_baro-0.1.9/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,49 @@
-from argparse import ArgumentParser
-from baro.reproducibility import reproduce_baro, reproduce_bocpd
+from argparse import ArgumentParser, RawTextHelpFormatter
+from baro.reproducibility import reproduce_baro, reproduce_bocpd, reproduce_rq4
 
+# Define dataset mappings
 DATASET_MAPS = {
     "OnlineBoutique": "fse-ob",
     "SockShop": "fse-ss",
     "TrainTicket": "fse-tt"
 }
 
-parser = ArgumentParser()
-parser.add_argument("--anomaly-detection", action="store_true")
-parser.add_argument("--saved", action="store_true")
-parser.add_argument("--dataset", type=str, default=None)
-parser.add_argument("--fault-type", type=str, default=None)
+# Define command-line arguments
+parser = ArgumentParser(formatter_class=RawTextHelpFormatter)
+parser.add_argument("--anomaly-detection", action="store_true",
+    help="Reproduce anomaly detection results."
+)
+parser.add_argument("--saved", action="store_true",
+    help="Use saved anomaly detection results to reproduce the\n"
+         "presented results without rerunning anomaly detection."
+)
+parser.add_argument("--dataset", type=str, default=None,
+    help="Choose a dataset to analyze. Options:\n"
+         "['OnlineBoutique', 'SockShop', and 'TrainTicket']."
+)
+parser.add_argument("--fault-type", type=str, default=None,
+    help="Specify the fault type for root cause analysis.\n"
+         "Options: ['cpu', 'mem', 'delay', 'loss', and 'all'].\n"
+         "If 'all' is selected, the program will run the root\n"
+         "cause analysis for all fault types."
+)
+parser.add_argument("--rq4", action="store_true",
+    help="Reproduce RQ4 results.")
+parser.add_argument("--eval-metric", type=str, default="avg5",
+    help="Evaluation metric for RQ4. Options: ['top1', 'top3',\n"
+        "'avg5']. Default: 'avg5'.")
 
 args = parser.parse_args()
 if args.dataset not in DATASET_MAPS:
     print(f"Dataset {args.dataset} is not supported! Valid datasets are {list(DATASET_MAPS.keys())}")
     exit(0)
 if args.fault_type not in [None, "all", "cpu", "mem", "delay", "loss"]:
     print(f"Fault type {args.fault_type} is not supported! Valid fault types are [None, 'all', 'cpu', 'mem', 'delay', 'loss']")
     exit(0)
 
-if not args.anomaly_detection:
-    reproduce_baro(dataset=DATASET_MAPS[args.dataset], fault=args.fault_type)
+if args.anomaly_detection:
+    reproduce_bocpd(dataset=DATASET_MAPS[args.dataset], saved=args.saved)
+elif args.rq4:
+    reproduce_rq4(dataset=DATASET_MAPS[args.dataset], eval_metric=args.eval_metric)
 else:
-    reproduce_bocpd(dataset=DATASET_MAPS[args.dataset], saved=args.saved)
+    reproduce_baro(dataset=DATASET_MAPS[args.dataset], fault=args.fault_type)
```

### Comparing `fse_baro-0.1.8/pyproject.toml` & `fse_baro-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.8/tests/test.py` & `fse_baro-0.1.9/tests/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     # make df from time_col and latency
     df = pd.DataFrame({'time': time_col, 'latency': latency})
     
     anomalies = bocpd(df)
     assert abs(anomalies[0] - 100) < 10, anomalies
 
 def test_baro():
+    """Test BARO end-to-end"""
     local_path = tempfile.NamedTemporaryFile().name
     download_data(local_path=local_path)
     df = pd.read_csv(local_path)
     df = df[60:660].reset_index(drop=True)
 
     # select latency and error rate
     time_col = pd.Series(range(df.shape[0])) # df["time"]
```

### Comparing `fse_baro-0.1.8/tutorials/reproduce_multivariate_bocpd.ipynb` & `fse_baro-0.1.9/tutorials/reproduce_multivariate_bocpd.ipynb`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.8/tutorials/reproducibility.ipynb` & `fse_baro-0.1.9/tutorials/reproducibility.ipynb`

 * *Files identical despite different names*

