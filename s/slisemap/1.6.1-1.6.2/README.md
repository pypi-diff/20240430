# Comparing `tmp/slisemap-1.6.1.tar.gz` & `tmp/slisemap-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slisemap-1.6.1.tar", last modified: Tue Feb 20 13:03:56 2024, max compression
+gzip compressed data, was "slisemap-1.6.2.tar", last modified: Tue Apr 30 09:09:29 2024, max compression
```

## Comparing `slisemap-1.6.1.tar` & `slisemap-1.6.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:03:56.305507 slisemap-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-20 13:03:48.000000 slisemap-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-02-20 13:03:56.305507 slisemap-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-02-20 13:03:48.000000 slisemap-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-20 13:03:48.000000 slisemap-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 13:03:56.305507 slisemap-1.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:03:56.301507 slisemap-1.6.1/slisemap/
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-02-20 13:03:48.000000 slisemap-1.6.1/slisemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12357 2024-02-20 13:03:48.000000 slisemap-1.6.1/slisemap/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8734 2024-02-20 13:03:48.000000 slisemap-1.6.1/slisemap/escape.py
--rw-r--r--   0 runner    (1001) docker     (127)    13588 2024-02-20 13:03:48.000000 slisemap-1.6.1/slisemap/local_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-20 13:03:48.000000 slisemap-1.6.1/slisemap/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-02-20 13:03:48.000000 slisemap-1.6.1/slisemap/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19086 2024-02-20 13:03:48.000000 slisemap-1.6.1/slisemap/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    50277 2024-02-20 13:03:48.000000 slisemap-1.6.1/slisemap/slipmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    67672 2024-02-20 13:03:48.000000 slisemap-1.6.1/slisemap/slisemap.py
--rw-r--r--   0 runner    (1001) docker     (127)    21561 2024-02-20 13:03:48.000000 slisemap-1.6.1/slisemap/tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-02-20 13:03:48.000000 slisemap-1.6.1/slisemap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:03:56.301507 slisemap-1.6.1/slisemap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-02-20 13:03:56.000000 slisemap-1.6.1/slisemap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-20 13:03:56.000000 slisemap-1.6.1/slisemap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 13:03:56.000000 slisemap-1.6.1/slisemap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-20 13:03:56.000000 slisemap-1.6.1/slisemap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-20 13:03:56.000000 slisemap-1.6.1/slisemap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:03:56.301507 slisemap-1.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-02-20 13:03:48.000000 slisemap-1.6.1/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-02-20 13:03:48.000000 slisemap-1.6.1/tests/test_escape.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-02-20 13:03:48.000000 slisemap-1.6.1/tests/test_local_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-02-20 13:03:48.000000 slisemap-1.6.1/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-02-20 13:03:48.000000 slisemap-1.6.1/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-02-20 13:03:48.000000 slisemap-1.6.1/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-02-20 13:03:48.000000 slisemap-1.6.1/tests/test_slipmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-02-20 13:03:48.000000 slisemap-1.6.1/tests/test_slisemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-20 13:03:48.000000 slisemap-1.6.1/tests/test_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-02-20 13:03:48.000000 slisemap-1.6.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:09:29.537478 slisemap-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-30 09:09:25.000000 slisemap-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-30 09:09:29.537478 slisemap-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-30 09:09:25.000000 slisemap-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-30 09:09:25.000000 slisemap-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:09:29.537478 slisemap-1.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:09:29.533478 slisemap-1.6.2/slisemap/
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-30 09:09:25.000000 slisemap-1.6.2/slisemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12357 2024-04-30 09:09:25.000000 slisemap-1.6.2/slisemap/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8734 2024-04-30 09:09:25.000000 slisemap-1.6.2/slisemap/escape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13588 2024-04-30 09:09:25.000000 slisemap-1.6.2/slisemap/local_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-30 09:09:25.000000 slisemap-1.6.2/slisemap/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-04-30 09:09:25.000000 slisemap-1.6.2/slisemap/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19086 2024-04-30 09:09:25.000000 slisemap-1.6.2/slisemap/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50277 2024-04-30 09:09:25.000000 slisemap-1.6.2/slisemap/slipmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67672 2024-04-30 09:09:25.000000 slisemap-1.6.2/slisemap/slisemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21561 2024-04-30 09:09:25.000000 slisemap-1.6.2/slisemap/tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-04-30 09:09:25.000000 slisemap-1.6.2/slisemap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:09:29.537478 slisemap-1.6.2/slisemap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-30 09:09:29.000000 slisemap-1.6.2/slisemap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-30 09:09:29.000000 slisemap-1.6.2/slisemap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:09:29.000000 slisemap-1.6.2/slisemap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 09:09:29.000000 slisemap-1.6.2/slisemap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 09:09:29.000000 slisemap-1.6.2/slisemap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:09:29.537478 slisemap-1.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-30 09:09:25.000000 slisemap-1.6.2/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-30 09:09:25.000000 slisemap-1.6.2/tests/test_escape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-30 09:09:25.000000 slisemap-1.6.2/tests/test_local_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-30 09:09:25.000000 slisemap-1.6.2/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-30 09:09:25.000000 slisemap-1.6.2/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-30 09:09:25.000000 slisemap-1.6.2/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-30 09:09:25.000000 slisemap-1.6.2/tests/test_slipmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-30 09:09:25.000000 slisemap-1.6.2/tests/test_slisemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-30 09:09:25.000000 slisemap-1.6.2/tests/test_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-30 09:09:25.000000 slisemap-1.6.2/tests/test_utils.py
```

### Comparing `slisemap-1.6.1/LICENSE` & `slisemap-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/PKG-INFO` & `slisemap-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: slisemap
-Version: 1.6.1
+Version: 1.6.2
 Summary: SLISEMAP: Combine local explanations with supervised dimensionality reduction
-Author: Jarmo Mäkelä
+Author: Lauri Seppäläinen, Jarmo Mäkelä
 Author-email: Anton Björklund <anton.bjorklund@helsinki.fi>, Kai Puolamäki <kai.puolamaki@helsinki.fi>
 License: MIT License
         
         Copyright (c) 2024 Anton Björklund, Jarmo Mäkelä, and Kai Puolamäki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -70,28 +70,28 @@
 *This library also includes the faster SLIPMAP variant, that uses "prototypes" to speed up
 the calculations (linear time and memory complexity instead of quadratic).
 SLIPMAP is largely compatible with SLISEMAP, just change the class name (`Slisemap` to `Slipmap`, see example below).*
 
 
 ## Citations
 
-The full SLISEMAP paper ([arXiv](https://arxiv.org/abs/2201.04455) and [supplements](https://github.com/edahelsinki/slisemap/tree/slisemap_experiments)):
+The new SLIPMAP paper ([supplements](https://github.com/edahelsinki/slisemap/tree/slipmap_experiments) and [slides](https://github.com/edahelsinki/slisemap/blob/data/slides/slipmap_slides.pdf)):
+> *Björklund, A., Seppäläinen, L., & Puolamäki, K. (2024).*  
+> **SLIPMAP: Fast and Robust Manifold Visualisation for Explainable AI**  
+> Advances in Intelligent Data Analysis XXII, IDA 2024, pp. 223-235. Lecture Notes in Computer Science, vol 14642. DOI: [10.1007/978-3-031-58553-1_18](https://doi.org/10.1007/978-3-031-58553-1_18)  
+
+The full SLISEMAP paper ([arXiv](https://arxiv.org/abs/2201.04455), [supplements](https://github.com/edahelsinki/slisemap/tree/slisemap_experiments), and [slides](https://github.com/edahelsinki/slisemap/blob/data/slides/slisemap_slides.pdf)):
 > *Björklund, A., Mäkelä, J., & Puolamäki, K. (2023).*  
 > **SLISEMAP: Supervised dimensionality reduction through local explanations.**  
 > Machine Learning 112, 1-43. DOI: [10.1007/s10994-022-06261-1](https://doi.org/10.1007/s10994-022-06261-1)  
 
-The short demo paper ([video](https://youtu.be/zvcFYItwRlQ) and [slides](https://github.com/edahelsinki/slisemap/blob/main/examples/demo_presentation.pdf)):
+The short demo paper ([video](https://youtu.be/zvcFYItwRlQ) and [slides](https://github.com/edahelsinki/slisemap/blob/data/slides/demo_slides.pdf)):
 > *Björklund, A., Mäkelä, J., & Puolamäki, K. (2023).*  
 > **SLISEMAP: Combining Supervised Dimensionality Reduction with Local Explanations.**  
-> Machine Learning and Knowledge Discovery in Databases. ECML PKDD 2022. Lecture Notes in Computer Science, vol 13718. DOI: [10.1007/978-3-031-26422-1_41](https://doi.org/10.1007/978-3-031-26422-1_41).
-
-The new SLIPMAP paper ([supplements](https://github.com/edahelsinki/slisemap/tree/slipmap_experiments)):
-> *Björklund, A., Seppäläinen, L., & Puolamäki, K. (2024).*  
-> **SLIPMAP: Fast and Robust Manifold Visualisation for Explainable AI**  
-> To appear in: Advances in Intelligent Data Analysis XXII. IDA 2024. Lecture Notes in Computer Science.  
+> Machine Learning and Knowledge Discovery in Databases, ECML PKDD 2022. Lecture Notes in Computer Science, vol 13718. DOI: [10.1007/978-3-031-26422-1_41](https://doi.org/10.1007/978-3-031-26422-1_41).
 
 
 ## Installation
 
 To install the package just run:
 
 ```sh
```

### Comparing `slisemap-1.6.1/README.md` & `slisemap-1.6.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 *This library also includes the faster SLIPMAP variant, that uses "prototypes" to speed up
 the calculations (linear time and memory complexity instead of quadratic).
 SLIPMAP is largely compatible with SLISEMAP, just change the class name (`Slisemap` to `Slipmap`, see example below).*
 
 
 ## Citations
 
-The full SLISEMAP paper ([arXiv](https://arxiv.org/abs/2201.04455) and [supplements](https://github.com/edahelsinki/slisemap/tree/slisemap_experiments)):
+The new SLIPMAP paper ([supplements](https://github.com/edahelsinki/slisemap/tree/slipmap_experiments) and [slides](https://github.com/edahelsinki/slisemap/blob/data/slides/slipmap_slides.pdf)):
+> *Björklund, A., Seppäläinen, L., & Puolamäki, K. (2024).*  
+> **SLIPMAP: Fast and Robust Manifold Visualisation for Explainable AI**  
+> Advances in Intelligent Data Analysis XXII, IDA 2024, pp. 223-235. Lecture Notes in Computer Science, vol 14642. DOI: [10.1007/978-3-031-58553-1_18](https://doi.org/10.1007/978-3-031-58553-1_18)  
+
+The full SLISEMAP paper ([arXiv](https://arxiv.org/abs/2201.04455), [supplements](https://github.com/edahelsinki/slisemap/tree/slisemap_experiments), and [slides](https://github.com/edahelsinki/slisemap/blob/data/slides/slisemap_slides.pdf)):
 > *Björklund, A., Mäkelä, J., & Puolamäki, K. (2023).*  
 > **SLISEMAP: Supervised dimensionality reduction through local explanations.**  
 > Machine Learning 112, 1-43. DOI: [10.1007/s10994-022-06261-1](https://doi.org/10.1007/s10994-022-06261-1)  
 
-The short demo paper ([video](https://youtu.be/zvcFYItwRlQ) and [slides](https://github.com/edahelsinki/slisemap/blob/main/examples/demo_presentation.pdf)):
+The short demo paper ([video](https://youtu.be/zvcFYItwRlQ) and [slides](https://github.com/edahelsinki/slisemap/blob/data/slides/demo_slides.pdf)):
 > *Björklund, A., Mäkelä, J., & Puolamäki, K. (2023).*  
 > **SLISEMAP: Combining Supervised Dimensionality Reduction with Local Explanations.**  
-> Machine Learning and Knowledge Discovery in Databases. ECML PKDD 2022. Lecture Notes in Computer Science, vol 13718. DOI: [10.1007/978-3-031-26422-1_41](https://doi.org/10.1007/978-3-031-26422-1_41).
-
-The new SLIPMAP paper ([supplements](https://github.com/edahelsinki/slisemap/tree/slipmap_experiments)):
-> *Björklund, A., Seppäläinen, L., & Puolamäki, K. (2024).*  
-> **SLIPMAP: Fast and Robust Manifold Visualisation for Explainable AI**  
-> To appear in: Advances in Intelligent Data Analysis XXII. IDA 2024. Lecture Notes in Computer Science.  
+> Machine Learning and Knowledge Discovery in Databases, ECML PKDD 2022. Lecture Notes in Computer Science, vol 13718. DOI: [10.1007/978-3-031-26422-1_41](https://doi.org/10.1007/978-3-031-26422-1_41).
 
 
 ## Installation
 
 To install the package just run:
 
 ```sh
```

### Comparing `slisemap-1.6.1/pyproject.toml` & `slisemap-1.6.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slisemap"
-version = "1.6.1"
+version = "1.6.2"
 authors = [
     { name = "Anton Björklund", email = "anton.bjorklund@helsinki.fi" },
-    { name = "Jarmo Mäkelä" },
     { name = "Kai Puolamäki", email = "kai.puolamaki@helsinki.fi" },
+    { name = "Lauri Seppäläinen" },
+    { name = "Jarmo Mäkelä" },
 ]
 description = "SLISEMAP: Combine local explanations with supervised dimensionality reduction"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "Explainable AI",
     "Local explanation",
```

### Comparing `slisemap-1.6.1/slisemap/__init__.py` & `slisemap-1.6.2/slisemap/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,42 +12,43 @@
 For more information see the the [repository](https://github.com/edahelsinki/slisemap),
 the [documentation](https://edahelsinki.github.io/slisemap/slisemap), or the
 [paper](https://doi.org/10.1007/s10994-022-06261-1).
 
 This module also includes the faster SLIPMAP variant, that uses "prototypes" to speed up
 the calculations (linear time and memory complexity instead of quadratic).
 SLIPMAP is largely compatible with SLISEMAP, just change the class name (`Slisemap` to `Slipmap`).
-For more information, see the sources above and the [paper](TODO).
+For more information, see the sources above and the [paper](https://doi.org/10.1007/978-3-031-58553-1_18).
 
 Documentation
 -------------
 
 - [Slisemap][slisemap.slisemap.Slisemap]
 - [Slipmap][slisemap.slipmap.Slipmap]
 
 
 Citations
 ---------
-> Björklund, A., Mäkelä, J. & Puolamäki, K. (2023).
-> SLISEMAP: Supervised dimensionality reduction through local explanations.
-> Machine Learning 112, 1-43. DOI: 10.1007/s10994-022-06261-1.
-
-> Björklund, A., Seppäläinen, L., & Puolamäki, K. (2024).
-> SLIPMAP: Fast and Robust Manifold Visualisation for Explainable AI
-> To appear in: Advances in Intelligent Data Analysis XXII. IDA 2024. Lecture Notes in Computer Science.
+> Björklund, A., Mäkelä, J. & Puolamäki, K. (2023).  
+> SLISEMAP: Supervised dimensionality reduction through local explanations.  
+> Machine Learning 112, 1-43. DOI: 10.1007/s10994-022-06261-1.  
+
+> Björklund, A., Seppäläinen, L., & Puolamäki, K. (2024).  
+> SLIPMAP: Fast and Robust Manifold Visualisation for Explainable AI  
+> Advances in Intelligent Data Analysis XXII, pp. 223-235, LNCS 14642.  
+> DOI: 10.1007/978-3-031-58553-1_18.  
 
 
 Example Usage
 -------------
 
     from slisemap import Slipmap
     import numpy as np
 
     X = np.array([[0.1,0.5,0.7], [0.8,0.9,1], [0.8,0.5,0.3], [0.1,0.2,0.3], [1,2,5], [2,3,4], [2,0,1]])
     y = np.array([1, 2, 3, 4, 1.5, 1.8, 1.7])
     sm = Slipmap(X, y, radius=2.0, lasso=1e-4, ridge=2e-4)
     sm.optimise()
     sm.plot()
-"""  # noqa: D205
+"""  # noqa: D205, W291
 
 from slisemap.slipmap import Slipmap  # noqa: F401
 from slisemap.slisemap import Slisemap  # noqa: F401
```

### Comparing `slisemap-1.6.1/slisemap/diagnostics.py` & `slisemap-1.6.2/slisemap/diagnostics.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/slisemap/escape.py` & `slisemap-1.6.2/slisemap/escape.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/slisemap/local_models.py` & `slisemap-1.6.2/slisemap/local_models.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/slisemap/metrics.py` & `slisemap-1.6.2/slisemap/metrics.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/slisemap/plot.py` & `slisemap-1.6.2/slisemap/plot.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/slisemap/slipmap.py` & `slisemap-1.6.2/slisemap/slipmap.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/slisemap/slisemap.py` & `slisemap-1.6.2/slisemap/slisemap.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/slisemap/tuning.py` & `slisemap-1.6.2/slisemap/tuning.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/slisemap/utils.py` & `slisemap-1.6.2/slisemap/utils.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/slisemap.egg-info/PKG-INFO` & `slisemap-1.6.2/slisemap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: slisemap
-Version: 1.6.1
+Version: 1.6.2
 Summary: SLISEMAP: Combine local explanations with supervised dimensionality reduction
-Author: Jarmo Mäkelä
+Author: Lauri Seppäläinen, Jarmo Mäkelä
 Author-email: Anton Björklund <anton.bjorklund@helsinki.fi>, Kai Puolamäki <kai.puolamaki@helsinki.fi>
 License: MIT License
         
         Copyright (c) 2024 Anton Björklund, Jarmo Mäkelä, and Kai Puolamäki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -70,28 +70,28 @@
 *This library also includes the faster SLIPMAP variant, that uses "prototypes" to speed up
 the calculations (linear time and memory complexity instead of quadratic).
 SLIPMAP is largely compatible with SLISEMAP, just change the class name (`Slisemap` to `Slipmap`, see example below).*
 
 
 ## Citations
 
-The full SLISEMAP paper ([arXiv](https://arxiv.org/abs/2201.04455) and [supplements](https://github.com/edahelsinki/slisemap/tree/slisemap_experiments)):
+The new SLIPMAP paper ([supplements](https://github.com/edahelsinki/slisemap/tree/slipmap_experiments) and [slides](https://github.com/edahelsinki/slisemap/blob/data/slides/slipmap_slides.pdf)):
+> *Björklund, A., Seppäläinen, L., & Puolamäki, K. (2024).*  
+> **SLIPMAP: Fast and Robust Manifold Visualisation for Explainable AI**  
+> Advances in Intelligent Data Analysis XXII, IDA 2024, pp. 223-235. Lecture Notes in Computer Science, vol 14642. DOI: [10.1007/978-3-031-58553-1_18](https://doi.org/10.1007/978-3-031-58553-1_18)  
+
+The full SLISEMAP paper ([arXiv](https://arxiv.org/abs/2201.04455), [supplements](https://github.com/edahelsinki/slisemap/tree/slisemap_experiments), and [slides](https://github.com/edahelsinki/slisemap/blob/data/slides/slisemap_slides.pdf)):
 > *Björklund, A., Mäkelä, J., & Puolamäki, K. (2023).*  
 > **SLISEMAP: Supervised dimensionality reduction through local explanations.**  
 > Machine Learning 112, 1-43. DOI: [10.1007/s10994-022-06261-1](https://doi.org/10.1007/s10994-022-06261-1)  
 
-The short demo paper ([video](https://youtu.be/zvcFYItwRlQ) and [slides](https://github.com/edahelsinki/slisemap/blob/main/examples/demo_presentation.pdf)):
+The short demo paper ([video](https://youtu.be/zvcFYItwRlQ) and [slides](https://github.com/edahelsinki/slisemap/blob/data/slides/demo_slides.pdf)):
 > *Björklund, A., Mäkelä, J., & Puolamäki, K. (2023).*  
 > **SLISEMAP: Combining Supervised Dimensionality Reduction with Local Explanations.**  
-> Machine Learning and Knowledge Discovery in Databases. ECML PKDD 2022. Lecture Notes in Computer Science, vol 13718. DOI: [10.1007/978-3-031-26422-1_41](https://doi.org/10.1007/978-3-031-26422-1_41).
-
-The new SLIPMAP paper ([supplements](https://github.com/edahelsinki/slisemap/tree/slipmap_experiments)):
-> *Björklund, A., Seppäläinen, L., & Puolamäki, K. (2024).*  
-> **SLIPMAP: Fast and Robust Manifold Visualisation for Explainable AI**  
-> To appear in: Advances in Intelligent Data Analysis XXII. IDA 2024. Lecture Notes in Computer Science.  
+> Machine Learning and Knowledge Discovery in Databases, ECML PKDD 2022. Lecture Notes in Computer Science, vol 13718. DOI: [10.1007/978-3-031-26422-1_41](https://doi.org/10.1007/978-3-031-26422-1_41).
 
 
 ## Installation
 
 To install the package just run:
 
 ```sh
```

### Comparing `slisemap-1.6.1/slisemap.egg-info/SOURCES.txt` & `slisemap-1.6.2/slisemap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/tests/test_diagnostics.py` & `slisemap-1.6.2/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/tests/test_escape.py` & `slisemap-1.6.2/tests/test_escape.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/tests/test_local_models.py` & `slisemap-1.6.2/tests/test_local_models.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/tests/test_metrics.py` & `slisemap-1.6.2/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/tests/test_plot.py` & `slisemap-1.6.2/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/tests/test_save.py` & `slisemap-1.6.2/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/tests/test_slipmap.py` & `slisemap-1.6.2/tests/test_slipmap.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/tests/test_slisemap.py` & `slisemap-1.6.2/tests/test_slisemap.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/tests/test_tuning.py` & `slisemap-1.6.2/tests/test_tuning.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.6.1/tests/test_utils.py` & `slisemap-1.6.2/tests/test_utils.py`

 * *Files identical despite different names*

