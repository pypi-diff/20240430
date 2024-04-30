# Comparing `tmp/fse_baro-0.1.6.tar.gz` & `tmp/fse_baro-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fse_baro-0.1.6.tar", last modified: Mon Apr 29 13:01:10 2024, max compression
+gzip compressed data, was "fse_baro-0.1.7.tar", last modified: Tue Apr 30 02:22:09 2024, max compression
```

## Comparing `fse_baro-0.1.6.tar` & `fse_baro-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.723485 fse_baro-0.1.6/.circleci/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 13:01:05.000000 fse_baro-0.1.6/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.723485 fse_baro-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-29 13:01:05.000000 fse_baro-0.1.6/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 13:01:05.000000 fse_baro-0.1.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-29 13:01:05.000000 fse_baro-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 13:01:05.000000 fse_baro-0.1.6/ENHANCEMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-29 13:01:05.000000 fse_baro-0.1.6/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-29 13:01:05.000000 fse_baro-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 13:01:10.727485 fse_baro-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-29 13:01:05.000000 fse_baro-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-29 13:01:05.000000 fse_baro-0.1.6/REQUIREMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-29 13:01:05.000000 fse_baro-0.1.6/STATUS.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/baro/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 13:01:05.000000 fse_baro-0.1.6/baro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-29 13:01:05.000000 fse_baro-0.1.6/baro/_bocpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-29 13:01:05.000000 fse_baro-0.1.6/baro/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-29 13:01:05.000000 fse_baro-0.1.6/baro/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-29 13:01:05.000000 fse_baro-0.1.6/baro/root_cause_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-29 13:01:05.000000 fse_baro-0.1.6/baro/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-29 13:01:05.000000 fse_baro-0.1.6/docs/running_time_and_instrumentation_cost.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/fse_baro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 13:01:10.000000 fse_baro-0.1.6/fse_baro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-29 13:01:10.000000 fse_baro-0.1.6/fse_baro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:01:10.000000 fse_baro-0.1.6/fse_baro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 13:01:10.000000 fse_baro-0.1.6/fse_baro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 13:01:10.000000 fse_baro-0.1.6/fse_baro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-29 13:01:05.000000 fse_baro-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:01:10.727485 fse_baro-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-29 13:01:05.000000 fse_baro-0.1.6/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-29 13:01:05.000000 fse_baro-0.1.6/tutorials/reproduce_multivariate_bocpd.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-29 13:01:05.000000 fse_baro-0.1.6/tutorials/reproducibility.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.390118 fse_baro-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-30 02:22:04.000000 fse_baro-0.1.7/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.382117 fse_baro-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-30 02:22:04.000000 fse_baro-0.1.7/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-30 02:22:04.000000 fse_baro-0.1.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-30 02:22:04.000000 fse_baro-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 02:22:04.000000 fse_baro-0.1.7/ENHANCEMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-30 02:22:04.000000 fse_baro-0.1.7/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-30 02:22:04.000000 fse_baro-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-30 02:22:09.386118 fse_baro-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-30 02:22:04.000000 fse_baro-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 02:22:04.000000 fse_baro-0.1.7/REQUIREMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-30 02:22:04.000000 fse_baro-0.1.7/STATUS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/baro/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 02:22:04.000000 fse_baro-0.1.7/baro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-30 02:22:04.000000 fse_baro-0.1.7/baro/_bocpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-30 02:22:04.000000 fse_baro-0.1.7/baro/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-30 02:22:04.000000 fse_baro-0.1.7/baro/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-30 02:22:04.000000 fse_baro-0.1.7/baro/root_cause_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-30 02:22:04.000000 fse_baro-0.1.7/baro/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-30 02:22:04.000000 fse_baro-0.1.7/docs/running_time_and_instrumentation_cost.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/fse_baro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-30 02:22:09.000000 fse_baro-0.1.7/fse_baro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-30 02:22:09.000000 fse_baro-0.1.7/fse_baro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 02:22:09.000000 fse_baro-0.1.7/fse_baro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 02:22:09.000000 fse_baro-0.1.7/fse_baro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 02:22:09.000000 fse_baro-0.1.7/fse_baro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-30 02:22:04.000000 fse_baro-0.1.7/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-30 02:22:04.000000 fse_baro-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 02:22:09.390118 fse_baro-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-30 02:22:04.000000 fse_baro-0.1.7/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-30 02:22:04.000000 fse_baro-0.1.7/tutorials/reproduce_multivariate_bocpd.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-30 02:22:04.000000 fse_baro-0.1.7/tutorials/reproducibility.ipynb
```

### Comparing `fse_baro-0.1.6/.github/workflows/build-and-test.yml` & `fse_baro-0.1.7/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.6/.github/workflows/python-publish.yml` & `fse_baro-0.1.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.6/.gitignore` & `fse_baro-0.1.7/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -196,7 +196,8 @@
 data/fse-*
 data/sock-shop-2
 .ar
 data
 .vscode
 env
 env*
+*.zip
```

### Comparing `fse_baro-0.1.6/INSTALL.md` & `fse_baro-0.1.7/INSTALL.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.6/LICENSE` & `fse_baro-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.6/REQUIREMENTS.md` & `fse_baro-0.1.7/REQUIREMENTS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.6/STATUS.md` & `fse_baro-0.1.7/STATUS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.6/baro/_bocpd.py` & `fse_baro-0.1.7/baro/_bocpd.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.6/baro/anomaly_detection.py` & `fse_baro-0.1.7/baro/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.6/baro/root_cause_analysis.py` & `fse_baro-0.1.7/baro/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.6/baro/utility.py` & `fse_baro-0.1.7/baro/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import glob 
 import shutil
 import requests
 import json
 import zipfile
-from os.path import join, basename, dirname
+from os.path import join, basename, dirname, exists
 
 import numpy as np
 from tqdm import tqdm
 import pandas as pd
 import matplotlib.pyplot as plt
 
 
@@ -151,15 +151,15 @@
             ref.write(data)
 
     progress_bar.close()
     if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
         print("ERROR, something went wrong")
 
 
-def read_data(data_path):
+def read_data(data_path, strip=True):
     """Read csv data for root cause analysis."""    
     data = pd.read_csv(data_path)
     data_dir = os.path.dirname(data_path)
 
     ############# PREPROCESSING ###############
     if "time.1" in data:
         data = data.drop(columns=["time.1"])
@@ -174,25 +174,34 @@
         columns={
             c: c.replace("_latency-90", "_latency")
             for c in data.columns
             if c.endswith("_latency-90")
         }
     )
 
-    # cut the data into 10 mins
-    data_length = 300
-    with open(join(data_dir, "inject_time.txt")) as f:
-        inject_time = int(f.readlines()[0].strip())
-    normal_df = data[data["time"] < inject_time].tail(data_length)
-    anomal_df = data[data["time"] >= inject_time].head(data_length)
-    data = pd.concat([normal_df, anomal_df], ignore_index=True)    
+    if strip is True and exists(join(data_dir, "inject_time.txt")):
+        # cut the data into 10 mins
+        data_length = 300
+        with open(join(data_dir, "inject_time.txt")) as f:
+            inject_time = int(f.readlines()[0].strip())
+        normal_df = data[data["time"] < inject_time].tail(data_length)
+        anomal_df = data[data["time"] >= inject_time].head(data_length)
+        data = pd.concat([normal_df, anomal_df], ignore_index=True)    
     return data
 
 def to_service_ranks(ranks):
     """Convert fine-grained ranking to service ranks"""
     _service_ranks = [r.split("_")[0] for r in ranks]
     service_ranks = []
     # remove duplicates
     for s in _service_ranks:
         if s not in service_ranks:
             service_ranks.append(s)
-    return service_ranks
+    return service_ranks
+
+
+def find_cps(maxes):
+    cps = []
+    for i in range(1, len(maxes)):
+        if abs(maxes[i] - maxes[i-1]) > 1:
+            cps.append((i, abs(maxes[i] - maxes[i-1])))
+    return cps
```

### Comparing `fse_baro-0.1.6/docs/running_time_and_instrumentation_cost.md` & `fse_baro-0.1.7/docs/running_time_and_instrumentation_cost.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.6/fse_baro.egg-info/SOURCES.txt` & `fse_baro-0.1.7/fse_baro.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitignore
 ENHANCEMENTS.md
 INSTALL.md
 LICENSE
 README.md
 REQUIREMENTS.md
 STATUS.md
+main.py
 pyproject.toml
 .circleci/config.yml
 .github/workflows/build-and-test.yml
 .github/workflows/python-publish.yml
 baro/__init__.py
 baro/_bocpd.py
 baro/anomaly_detection.py
```

### Comparing `fse_baro-0.1.6/pyproject.toml` & `fse_baro-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.6/tests/test.py` & `fse_baro-0.1.7/tests/test.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.6/tutorials/reproduce_multivariate_bocpd.ipynb` & `fse_baro-0.1.7/tutorials/reproduce_multivariate_bocpd.ipynb`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.6/tutorials/reproducibility.ipynb` & `fse_baro-0.1.7/tutorials/reproducibility.ipynb`

 * *Files identical despite different names*

