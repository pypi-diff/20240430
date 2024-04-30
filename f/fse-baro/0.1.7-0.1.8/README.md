# Comparing `tmp/fse_baro-0.1.7.tar.gz` & `tmp/fse_baro-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fse_baro-0.1.7.tar", last modified: Tue Apr 30 02:22:09 2024, max compression
+gzip compressed data, was "fse_baro-0.1.8.tar", last modified: Tue Apr 30 03:32:43 2024, max compression
```

## Comparing `fse_baro-0.1.7.tar` & `fse_baro-0.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.390118 fse_baro-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/.circleci/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-30 02:22:04.000000 fse_baro-0.1.7/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.382117 fse_baro-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-30 02:22:04.000000 fse_baro-0.1.7/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-30 02:22:04.000000 fse_baro-0.1.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-30 02:22:04.000000 fse_baro-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 02:22:04.000000 fse_baro-0.1.7/ENHANCEMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-30 02:22:04.000000 fse_baro-0.1.7/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-30 02:22:04.000000 fse_baro-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-30 02:22:09.386118 fse_baro-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-30 02:22:04.000000 fse_baro-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 02:22:04.000000 fse_baro-0.1.7/REQUIREMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-30 02:22:04.000000 fse_baro-0.1.7/STATUS.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/baro/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 02:22:04.000000 fse_baro-0.1.7/baro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-30 02:22:04.000000 fse_baro-0.1.7/baro/_bocpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-30 02:22:04.000000 fse_baro-0.1.7/baro/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-30 02:22:04.000000 fse_baro-0.1.7/baro/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-30 02:22:04.000000 fse_baro-0.1.7/baro/root_cause_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-30 02:22:04.000000 fse_baro-0.1.7/baro/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-30 02:22:04.000000 fse_baro-0.1.7/docs/running_time_and_instrumentation_cost.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/fse_baro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-30 02:22:09.000000 fse_baro-0.1.7/fse_baro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-30 02:22:09.000000 fse_baro-0.1.7/fse_baro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 02:22:09.000000 fse_baro-0.1.7/fse_baro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 02:22:09.000000 fse_baro-0.1.7/fse_baro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 02:22:09.000000 fse_baro-0.1.7/fse_baro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-30 02:22:04.000000 fse_baro-0.1.7/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-30 02:22:04.000000 fse_baro-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 02:22:09.390118 fse_baro-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-30 02:22:04.000000 fse_baro-0.1.7/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:22:09.386118 fse_baro-0.1.7/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-30 02:22:04.000000 fse_baro-0.1.7/tutorials/reproduce_multivariate_bocpd.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-30 02:22:04.000000 fse_baro-0.1.7/tutorials/reproducibility.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.866862 fse_baro-0.1.8/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-30 03:32:38.000000 fse_baro-0.1.8/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.866862 fse_baro-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-30 03:32:38.000000 fse_baro-0.1.8/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-30 03:32:38.000000 fse_baro-0.1.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-30 03:32:38.000000 fse_baro-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 03:32:38.000000 fse_baro-0.1.8/ENHANCEMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-30 03:32:38.000000 fse_baro-0.1.8/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-30 03:32:38.000000 fse_baro-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-30 03:32:43.870862 fse_baro-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-04-30 03:32:38.000000 fse_baro-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 03:32:38.000000 fse_baro-0.1.8/REQUIREMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-30 03:32:38.000000 fse_baro-0.1.8/STATUS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/baro/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 03:32:38.000000 fse_baro-0.1.8/baro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-30 03:32:38.000000 fse_baro-0.1.8/baro/_bocpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-30 03:32:38.000000 fse_baro-0.1.8/baro/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-30 03:32:38.000000 fse_baro-0.1.8/baro/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-30 03:32:38.000000 fse_baro-0.1.8/baro/root_cause_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-30 03:32:38.000000 fse_baro-0.1.8/baro/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-30 03:32:38.000000 fse_baro-0.1.8/docs/running_time_and_instrumentation_cost.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/fse_baro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-30 03:32:43.000000 fse_baro-0.1.8/fse_baro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-30 03:32:43.000000 fse_baro-0.1.8/fse_baro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 03:32:43.000000 fse_baro-0.1.8/fse_baro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 03:32:43.000000 fse_baro-0.1.8/fse_baro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 03:32:43.000000 fse_baro-0.1.8/fse_baro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-30 03:32:38.000000 fse_baro-0.1.8/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-30 03:32:38.000000 fse_baro-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 03:32:43.870862 fse_baro-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-30 03:32:38.000000 fse_baro-0.1.8/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:32:43.870862 fse_baro-0.1.8/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-30 03:32:38.000000 fse_baro-0.1.8/tutorials/reproduce_multivariate_bocpd.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-30 03:32:38.000000 fse_baro-0.1.8/tutorials/reproducibility.ipynb
```

### Comparing `fse_baro-0.1.7/.circleci/config.yml` & `fse_baro-0.1.8/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/.github/workflows/build-and-test.yml` & `fse_baro-0.1.8/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/.github/workflows/python-publish.yml` & `fse_baro-0.1.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/.gitignore` & `fse_baro-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/INSTALL.md` & `fse_baro-0.1.8/INSTALL.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/LICENSE` & `fse_baro-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/PKG-INFO` & `fse_baro-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.1.7
+Version: 0.1.8
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -76,28 +76,47 @@
 ### Sample Python commands to use BARO
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
 
 BARO consists of two modules, namely MultivariateBOCPD (implemented in `baro.anomaly_detection.bocpd`) and RobustScorer (implemented in `baro.root_cause_analysis.robust_scorer`). We expose these two functions for users/researchers to reuse them more conveniently. The sample commands to run BARO are presented as follows,
 
 ```python
-import pandas as pd 
+# You can put the code here to a file named test.py
 from baro.anomaly_detection import bocpd
 from baro.root_cause_analysis import robust_scorer
 from baro.utility import download_data, read_data
 
 # download a sample data to data.csv
 download_data()
 
-# read data, perform anomaly detection and rca using bocpd and robust_scorer
+# read data from data.csv
 data = read_data("data.csv")
-anomalies = bocpd(data)
-root_causes = robust_scorer(data, anomalies=anomalies)
-print(root_causes)
+
+# perform anomaly detection 
+anomalies = bocpd(data) 
+print("Anomalies are detected at timestep:", anomalies[0])
+
+# perform root cause analysis
+root_causes = robust_scorer(data, anomalies=anomalies)["ranks"]
+
+# print the top 5 root causes
+print("Top 5 root causes:", root_causes[:5])
+```
+
+<details>
+<summary>Expected output after running the above code (it takes around 1 minute)</summary>
+
 ```
+$ python test.py
+Downloading data.csv..: 100%|████████████████████████████████| 570k/570k [00:00<00:00, 17.1MiB/s]
+Anomalies are detected at timestep: 243
+Top 5 root causes: ['checkoutservice_latency', 'cartservice_mem', 'cartservice_latency', 'cartservice_cpu', 'main_mem']
+```
+</details>
+
 
 ## Reproducibility
 
 As presented in Table 3, BARO achieves Avg@5 of 0.91, 0.96, 0.95, 0.62, and 0.86 for CPU, MEM, DELAY, LOSS, and ALL fault types on the Online Boutique dataset. To reproduce the RCA performance of our BARO as presented in the Table 3. You can run the following commands:
 
 **Reproduce RCA performance on the Online Boutique dataset, fault type CPU**
```

### Comparing `fse_baro-0.1.7/README.md` & `fse_baro-0.1.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -37,28 +37,47 @@
 ### Sample Python commands to use BARO
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
 
 BARO consists of two modules, namely MultivariateBOCPD (implemented in `baro.anomaly_detection.bocpd`) and RobustScorer (implemented in `baro.root_cause_analysis.robust_scorer`). We expose these two functions for users/researchers to reuse them more conveniently. The sample commands to run BARO are presented as follows,
 
 ```python
-import pandas as pd 
+# You can put the code here to a file named test.py
 from baro.anomaly_detection import bocpd
 from baro.root_cause_analysis import robust_scorer
 from baro.utility import download_data, read_data
 
 # download a sample data to data.csv
 download_data()
 
-# read data, perform anomaly detection and rca using bocpd and robust_scorer
+# read data from data.csv
 data = read_data("data.csv")
-anomalies = bocpd(data)
-root_causes = robust_scorer(data, anomalies=anomalies)
-print(root_causes)
+
+# perform anomaly detection 
+anomalies = bocpd(data) 
+print("Anomalies are detected at timestep:", anomalies[0])
+
+# perform root cause analysis
+root_causes = robust_scorer(data, anomalies=anomalies)["ranks"]
+
+# print the top 5 root causes
+print("Top 5 root causes:", root_causes[:5])
+```
+
+<details>
+<summary>Expected output after running the above code (it takes around 1 minute)</summary>
+
 ```
+$ python test.py
+Downloading data.csv..: 100%|████████████████████████████████| 570k/570k [00:00<00:00, 17.1MiB/s]
+Anomalies are detected at timestep: 243
+Top 5 root causes: ['checkoutservice_latency', 'cartservice_mem', 'cartservice_latency', 'cartservice_cpu', 'main_mem']
+```
+</details>
+
 
 ## Reproducibility
 
 As presented in Table 3, BARO achieves Avg@5 of 0.91, 0.96, 0.95, 0.62, and 0.86 for CPU, MEM, DELAY, LOSS, and ALL fault types on the Online Boutique dataset. To reproduce the RCA performance of our BARO as presented in the Table 3. You can run the following commands:
 
 **Reproduce RCA performance on the Online Boutique dataset, fault type CPU**
```

### Comparing `fse_baro-0.1.7/REQUIREMENTS.md` & `fse_baro-0.1.8/REQUIREMENTS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/STATUS.md` & `fse_baro-0.1.8/STATUS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/baro/_bocpd.py` & `fse_baro-0.1.8/baro/_bocpd.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/baro/anomaly_detection.py` & `fse_baro-0.1.8/baro/anomaly_detection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import warnings
 warnings.filterwarnings("ignore")
 import pandas 
 import numpy as np
+from baro.utility import drop_constant, find_cps
 
 def nsigma(data, k=3, startsfrom=100):
     """For each time series (column) in the data,
     detect anomalies using the n-sigma rule.
     Return the timestamps of the anomalies.
     """
     anomalies = []
@@ -46,32 +47,38 @@
     return merged_anomalies, anomalies
 
 
 def bocpd(data):
     from functools import partial
     from baro._bocpd import online_changepoint_detection, constant_hazard, MultivariateT
     data = data.copy()
-    time_col = data['time']
-    data.drop(columns=['time'], inplace=True)
+    
+    # select latency and error metrics from microservices
+    selected_cols = []
+    for c in data.columns:
+        if 'queue-master' in c or 'rabbitmq_' in c: continue
+        if "latency" in c or "latency-50" in c or "_error" in c:
+            selected_cols.append(c)
+    data = data[selected_cols]
+
+    # handle na
+    data = drop_constant(data)
+    data = data.fillna(method="ffill")
+    data = data.fillna(0)
     for c in data.columns:
         data[c] = (data[c] - np.min(data[c])) / (np.max(data[c]) - np.min(data[c]))
-    data = data.ffill()
+    data = data.fillna(method="ffill")
     data = data.fillna(0)
+        
     data = data.to_numpy()
 
     R, maxes = online_changepoint_detection(
         data,
         partial(constant_hazard, 50),
         MultivariateT(dims=data.shape[1])
     )
-    Nw = 10
-    anomalies, merged_anomalies = find_anomalies(data=R[Nw,Nw:-1].tolist(), time_col=time_col)
-    return anomalies
-    
-
-def anomaly_detector(data, method="nsigma"):
-    # assert data is dataframe
-    assert isinstance(data, pandas.DataFrame)
-
-    # retain all `latency` and `error` columns
-    data = data[['latency', 'error']]
+    cps = find_cps(maxes)
+    anomalies = [p[0] for p in cps]
+    # anomalies, merged_anomalies = find_anomalies(data=R[Nw,Nw:-1].tolist(), time_col=time_col)
     
+    return anomalies
+
```

### Comparing `fse_baro-0.1.7/baro/reproducibility.py` & `fse_baro-0.1.8/baro/reproducibility.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/baro/root_cause_analysis.py` & `fse_baro-0.1.8/baro/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/baro/utility.py` & `fse_baro-0.1.8/baro/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,13 +195,19 @@
     # remove duplicates
     for s in _service_ranks:
         if s not in service_ranks:
             service_ranks.append(s)
     return service_ranks
 
 
+def select_latency_and_error(data):
+    """Select latency and error columns, retain `time` col"""
+    latency_cols = [c for c in data.columns if "latency" in c]
+    error_cols = [c for c in data.columns if "error" in c]
+    return data[["time"] + latency_cols + error_cols]    
+
 def find_cps(maxes):
     cps = []
     for i in range(1, len(maxes)):
         if abs(maxes[i] - maxes[i-1]) > 1:
             cps.append((i, abs(maxes[i] - maxes[i-1])))
     return cps
```

### Comparing `fse_baro-0.1.7/docs/running_time_and_instrumentation_cost.md` & `fse_baro-0.1.8/docs/running_time_and_instrumentation_cost.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/fse_baro.egg-info/PKG-INFO` & `fse_baro-0.1.8/fse_baro.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.1.7
+Version: 0.1.8
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -76,28 +76,47 @@
 ### Sample Python commands to use BARO
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
 
 BARO consists of two modules, namely MultivariateBOCPD (implemented in `baro.anomaly_detection.bocpd`) and RobustScorer (implemented in `baro.root_cause_analysis.robust_scorer`). We expose these two functions for users/researchers to reuse them more conveniently. The sample commands to run BARO are presented as follows,
 
 ```python
-import pandas as pd 
+# You can put the code here to a file named test.py
 from baro.anomaly_detection import bocpd
 from baro.root_cause_analysis import robust_scorer
 from baro.utility import download_data, read_data
 
 # download a sample data to data.csv
 download_data()
 
-# read data, perform anomaly detection and rca using bocpd and robust_scorer
+# read data from data.csv
 data = read_data("data.csv")
-anomalies = bocpd(data)
-root_causes = robust_scorer(data, anomalies=anomalies)
-print(root_causes)
+
+# perform anomaly detection 
+anomalies = bocpd(data) 
+print("Anomalies are detected at timestep:", anomalies[0])
+
+# perform root cause analysis
+root_causes = robust_scorer(data, anomalies=anomalies)["ranks"]
+
+# print the top 5 root causes
+print("Top 5 root causes:", root_causes[:5])
+```
+
+<details>
+<summary>Expected output after running the above code (it takes around 1 minute)</summary>
+
 ```
+$ python test.py
+Downloading data.csv..: 100%|████████████████████████████████| 570k/570k [00:00<00:00, 17.1MiB/s]
+Anomalies are detected at timestep: 243
+Top 5 root causes: ['checkoutservice_latency', 'cartservice_mem', 'cartservice_latency', 'cartservice_cpu', 'main_mem']
+```
+</details>
+
 
 ## Reproducibility
 
 As presented in Table 3, BARO achieves Avg@5 of 0.91, 0.96, 0.95, 0.62, and 0.86 for CPU, MEM, DELAY, LOSS, and ALL fault types on the Online Boutique dataset. To reproduce the RCA performance of our BARO as presented in the Table 3. You can run the following commands:
 
 **Reproduce RCA performance on the Online Boutique dataset, fault type CPU**
```

### Comparing `fse_baro-0.1.7/fse_baro.egg-info/SOURCES.txt` & `fse_baro-0.1.8/fse_baro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/main.py` & `fse_baro-0.1.8/main.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/pyproject.toml` & `fse_baro-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/tests/test.py` & `fse_baro-0.1.8/tests/test.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/tutorials/reproduce_multivariate_bocpd.ipynb` & `fse_baro-0.1.8/tutorials/reproduce_multivariate_bocpd.ipynb`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.7/tutorials/reproducibility.ipynb` & `fse_baro-0.1.8/tutorials/reproducibility.ipynb`

 * *Files identical despite different names*

