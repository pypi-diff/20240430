# Comparing `tmp/fse_baro-0.1.5.tar.gz` & `tmp/fse_baro-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fse_baro-0.1.5.tar", last modified: Mon Apr 29 12:53:23 2024, max compression
+gzip compressed data, was "fse_baro-0.1.6.tar", last modified: Mon Apr 29 13:01:10 2024, max compression
```

## Comparing `fse_baro-0.1.5.tar` & `fse_baro-0.1.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.887968 fse_baro-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.883968 fse_baro-0.1.5/.circleci/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 12:53:15.000000 fse_baro-0.1.5/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.879968 fse_baro-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.883968 fse_baro-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-29 12:53:15.000000 fse_baro-0.1.5/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 12:53:15.000000 fse_baro-0.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-29 12:53:15.000000 fse_baro-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 12:53:15.000000 fse_baro-0.1.5/ENHANCEMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-29 12:53:15.000000 fse_baro-0.1.5/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-29 12:53:15.000000 fse_baro-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 12:53:23.887968 fse_baro-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-29 12:53:15.000000 fse_baro-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-29 12:53:15.000000 fse_baro-0.1.5/REQUIREMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-29 12:53:15.000000 fse_baro-0.1.5/STATUS.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.883968 fse_baro-0.1.5/baro/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 12:53:15.000000 fse_baro-0.1.5/baro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-29 12:53:15.000000 fse_baro-0.1.5/baro/_bocpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-29 12:53:15.000000 fse_baro-0.1.5/baro/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-29 12:53:15.000000 fse_baro-0.1.5/baro/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-29 12:53:15.000000 fse_baro-0.1.5/baro/root_cause_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-29 12:53:15.000000 fse_baro-0.1.5/baro/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.883968 fse_baro-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-29 12:53:15.000000 fse_baro-0.1.5/docs/running_time_and_instrumentation_cost.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.887968 fse_baro-0.1.5/fse_baro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 12:53:23.000000 fse_baro-0.1.5/fse_baro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-29 12:53:23.000000 fse_baro-0.1.5/fse_baro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:53:23.000000 fse_baro-0.1.5/fse_baro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 12:53:23.000000 fse_baro-0.1.5/fse_baro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 12:53:23.000000 fse_baro-0.1.5/fse_baro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-29 12:53:15.000000 fse_baro-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:53:23.887968 fse_baro-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.887968 fse_baro-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-29 12:53:15.000000 fse_baro-0.1.5/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.887968 fse_baro-0.1.5/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-29 12:53:15.000000 fse_baro-0.1.5/tutorials/reproduce_multivariate_bocpd.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-29 12:53:15.000000 fse_baro-0.1.5/tutorials/reproducibility.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.723485 fse_baro-0.1.6/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 13:01:05.000000 fse_baro-0.1.6/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.723485 fse_baro-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-29 13:01:05.000000 fse_baro-0.1.6/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 13:01:05.000000 fse_baro-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-29 13:01:05.000000 fse_baro-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 13:01:05.000000 fse_baro-0.1.6/ENHANCEMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-29 13:01:05.000000 fse_baro-0.1.6/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-29 13:01:05.000000 fse_baro-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 13:01:10.727485 fse_baro-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-29 13:01:05.000000 fse_baro-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-29 13:01:05.000000 fse_baro-0.1.6/REQUIREMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-29 13:01:05.000000 fse_baro-0.1.6/STATUS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/baro/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 13:01:05.000000 fse_baro-0.1.6/baro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-29 13:01:05.000000 fse_baro-0.1.6/baro/_bocpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-29 13:01:05.000000 fse_baro-0.1.6/baro/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-29 13:01:05.000000 fse_baro-0.1.6/baro/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-29 13:01:05.000000 fse_baro-0.1.6/baro/root_cause_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-29 13:01:05.000000 fse_baro-0.1.6/baro/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-29 13:01:05.000000 fse_baro-0.1.6/docs/running_time_and_instrumentation_cost.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/fse_baro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 13:01:10.000000 fse_baro-0.1.6/fse_baro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-29 13:01:10.000000 fse_baro-0.1.6/fse_baro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:01:10.000000 fse_baro-0.1.6/fse_baro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 13:01:10.000000 fse_baro-0.1.6/fse_baro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 13:01:10.000000 fse_baro-0.1.6/fse_baro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-29 13:01:05.000000 fse_baro-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:01:10.727485 fse_baro-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-29 13:01:05.000000 fse_baro-0.1.6/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:01:10.727485 fse_baro-0.1.6/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-29 13:01:05.000000 fse_baro-0.1.6/tutorials/reproduce_multivariate_bocpd.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-29 13:01:05.000000 fse_baro-0.1.6/tutorials/reproducibility.ipynb
```

### Comparing `fse_baro-0.1.5/.circleci/config.yml` & `fse_baro-0.1.6/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/.github/workflows/build-and-test.yml` & `fse_baro-0.1.6/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/.github/workflows/python-publish.yml` & `fse_baro-0.1.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/.gitignore` & `fse_baro-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/INSTALL.md` & `fse_baro-0.1.6/INSTALL.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/LICENSE` & `fse_baro-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/PKG-INFO` & `fse_baro-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.1.5
+Version: 0.1.6
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fse_baro-0.1.5/README.md` & `fse_baro-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/REQUIREMENTS.md` & `fse_baro-0.1.6/REQUIREMENTS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/STATUS.md` & `fse_baro-0.1.6/STATUS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/baro/_bocpd.py` & `fse_baro-0.1.6/baro/_bocpd.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/baro/anomaly_detection.py` & `fse_baro-0.1.6/baro/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/baro/reproducibility.py` & `fse_baro-0.1.6/baro/reproducibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,8 +77,9 @@
     top4_accuracy = top4_cnt / total_cnt
     top5_accuracy = top5_cnt / total_cnt
     avg5_accuracy = (top1_accuracy + top2_accuracy + top3_accuracy + top4_accuracy + top5_accuracy) / 5
 
     print("====== Reproduce BARO =====")
     print(f"Dataset   : {dataset}")
     print(f"Fault type: {fault}")
-    print(f"Avg@5 Acc : {avg5_accuracy:.2f}")
+    print(f"Avg@5 Acc : {avg5_accuracy:.2f}")
+    print()
```

### Comparing `fse_baro-0.1.5/baro/root_cause_analysis.py` & `fse_baro-0.1.6/baro/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/baro/utility.py` & `fse_baro-0.1.6/baro/utility.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/docs/running_time_and_instrumentation_cost.md` & `fse_baro-0.1.6/docs/running_time_and_instrumentation_cost.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/fse_baro.egg-info/PKG-INFO` & `fse_baro-0.1.6/fse_baro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.1.5
+Version: 0.1.6
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fse_baro-0.1.5/fse_baro.egg-info/SOURCES.txt` & `fse_baro-0.1.6/fse_baro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/pyproject.toml` & `fse_baro-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/tests/test.py` & `fse_baro-0.1.6/tests/test.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/tutorials/reproduce_multivariate_bocpd.ipynb` & `fse_baro-0.1.6/tutorials/reproduce_multivariate_bocpd.ipynb`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.5/tutorials/reproducibility.ipynb` & `fse_baro-0.1.6/tutorials/reproducibility.ipynb`

 * *Files identical despite different names*

