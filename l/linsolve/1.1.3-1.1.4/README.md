# Comparing `tmp/linsolve-1.1.3.tar.gz` & `tmp/linsolve-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linsolve-1.1.3.tar", last modified: Wed Dec  6 09:47:48 2023, max compression
+gzip compressed data, was "linsolve-1.1.4.tar", last modified: Tue Apr 30 16:59:01 2024, max compression
```

## Comparing `linsolve-1.1.3.tar` & `linsolve-1.1.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 09:47:48.040355 linsolve-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-06 09:47:39.000000 linsolve-1.1.3/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-12-06 09:47:39.000000 linsolve-1.1.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-12-06 09:47:39.000000 linsolve-1.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 09:47:48.036355 linsolve-1.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-12-06 09:47:39.000000 linsolve-1.1.3/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2023-12-06 09:47:39.000000 linsolve-1.1.3/.github/labels.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2023-12-06 09:47:39.000000 linsolve-1.1.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 09:47:48.036355 linsolve-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-12-06 09:47:39.000000 linsolve-1.1.3/.github/workflows/auto-merge-deps.yml
--rw-r--r--   0 runner    (1001) docker     (127)      515 2023-12-06 09:47:39.000000 linsolve-1.1.3/.github/workflows/check-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-12-06 09:47:39.000000 linsolve-1.1.3/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-12-06 09:47:39.000000 linsolve-1.1.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2023-12-06 09:47:39.000000 linsolve-1.1.3/.github/workflows/run_tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-12-06 09:47:39.000000 linsolve-1.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2023-12-06 09:47:39.000000 linsolve-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-12-06 09:47:39.000000 linsolve-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2023-12-06 09:47:48.040355 linsolve-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2023-12-06 09:47:39.000000 linsolve-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 09:47:48.036355 linsolve-1.1.3/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2023-12-06 09:47:39.000000 linsolve-1.1.3/ci/test_environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 09:47:48.036355 linsolve-1.1.3/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)    72241 2023-12-06 09:47:39.000000 linsolve-1.1.3/imgs/linear_model.png
--rw-r--r--   0 runner    (1001) docker     (127)    16889 2023-12-06 09:47:39.000000 linsolve-1.1.3/imgs/points.png
--rw-r--r--   0 runner    (1001) docker     (127)    16058 2023-12-06 09:47:39.000000 linsolve-1.1.3/linsolve_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-12-06 09:47:39.000000 linsolve-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 09:47:48.040355 linsolve-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 09:47:48.032355 linsolve-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 09:47:48.036355 linsolve-1.1.3/src/linsolve/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-06 09:47:39.000000 linsolve-1.1.3/src/linsolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-06 09:47:47.000000 linsolve-1.1.3/src/linsolve/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    46255 2023-12-06 09:47:39.000000 linsolve-1.1.3/src/linsolve/linsolve.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-12-06 09:47:39.000000 linsolve-1.1.3/src/linsolve/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 09:47:48.040355 linsolve-1.1.3/src/linsolve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2023-12-06 09:47:48.000000 linsolve-1.1.3/src/linsolve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-12-06 09:47:48.000000 linsolve-1.1.3/src/linsolve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 09:47:48.000000 linsolve-1.1.3/src/linsolve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-06 09:47:48.000000 linsolve-1.1.3/src/linsolve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-06 09:47:48.000000 linsolve-1.1.3/src/linsolve.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 09:47:48.040355 linsolve-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2023-12-06 09:47:39.000000 linsolve-1.1.3/tests/benchmark_A_large_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2023-12-06 09:47:39.000000 linsolve-1.1.3/tests/benchmark_A_large_shared_sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-12-06 09:47:39.000000 linsolve-1.1.3/tests/benchmark_A_small_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2023-12-06 09:47:39.000000 linsolve-1.1.3/tests/benchmark_A_small_shared_sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-06 09:47:39.000000 linsolve-1.1.3/tests/benchmark_A_small_unique.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2023-12-06 09:47:39.000000 linsolve-1.1.3/tests/benchmark_A_small_unique_sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    29318 2023-12-06 09:47:39.000000 linsolve-1.1.3/tests/test_linsolve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:01.364317 linsolve-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 16:58:56.000000 linsolve-1.1.4/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-30 16:58:56.000000 linsolve-1.1.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-30 16:58:56.000000 linsolve-1.1.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:01.360317 linsolve-1.1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 16:58:56.000000 linsolve-1.1.4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-30 16:58:56.000000 linsolve-1.1.4/.github/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-30 16:58:56.000000 linsolve-1.1.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:01.360317 linsolve-1.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-30 16:58:56.000000 linsolve-1.1.4/.github/workflows/auto-merge-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-30 16:58:56.000000 linsolve-1.1.4/.github/workflows/check-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-30 16:58:56.000000 linsolve-1.1.4/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-30 16:58:56.000000 linsolve-1.1.4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-30 16:58:56.000000 linsolve-1.1.4/.github/workflows/run_tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-30 16:58:56.000000 linsolve-1.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-30 16:58:56.000000 linsolve-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-30 16:58:56.000000 linsolve-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-30 16:59:01.364317 linsolve-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-30 16:58:56.000000 linsolve-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:01.360317 linsolve-1.1.4/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-30 16:58:56.000000 linsolve-1.1.4/ci/test_environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:01.364317 linsolve-1.1.4/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)    72241 2024-04-30 16:58:56.000000 linsolve-1.1.4/imgs/linear_model.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-30 16:58:56.000000 linsolve-1.1.4/imgs/points.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-04-30 16:58:56.000000 linsolve-1.1.4/linsolve_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-30 16:58:56.000000 linsolve-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 16:59:01.364317 linsolve-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:01.360317 linsolve-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:01.364317 linsolve-1.1.4/src/linsolve/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 16:58:56.000000 linsolve-1.1.4/src/linsolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 16:59:01.000000 linsolve-1.1.4/src/linsolve/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46069 2024-04-30 16:58:56.000000 linsolve-1.1.4/src/linsolve/linsolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-30 16:58:56.000000 linsolve-1.1.4/src/linsolve/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:01.364317 linsolve-1.1.4/src/linsolve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-30 16:59:01.000000 linsolve-1.1.4/src/linsolve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-30 16:59:01.000000 linsolve-1.1.4/src/linsolve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:59:01.000000 linsolve-1.1.4/src/linsolve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-30 16:59:01.000000 linsolve-1.1.4/src/linsolve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 16:59:01.000000 linsolve-1.1.4/src/linsolve.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:01.364317 linsolve-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-30 16:58:56.000000 linsolve-1.1.4/tests/benchmark_A_large_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-30 16:58:56.000000 linsolve-1.1.4/tests/benchmark_A_large_shared_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 16:58:56.000000 linsolve-1.1.4/tests/benchmark_A_small_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-30 16:58:56.000000 linsolve-1.1.4/tests/benchmark_A_small_shared_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-30 16:58:56.000000 linsolve-1.1.4/tests/benchmark_A_small_unique.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-30 16:58:56.000000 linsolve-1.1.4/tests/benchmark_A_small_unique_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29318 2024-04-30 16:58:56.000000 linsolve-1.1.4/tests/test_linsolve.py
```

### Comparing `linsolve-1.1.3/.flake8` & `linsolve-1.1.4/.flake8`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/.github/labels.yml` & `linsolve-1.1.4/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/.github/release-drafter.yml` & `linsolve-1.1.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/.github/workflows/check-build.yml` & `linsolve-1.1.4/.github/workflows/check-build.yml`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/.github/workflows/publish.yaml` & `linsolve-1.1.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/.github/workflows/run_tests.yaml` & `linsolve-1.1.4/.github/workflows/run_tests.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
       run:
         shell: bash -l {0}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python-version: [3.8, 3.9, '3.10']
+        python-version: [3.9, '3.10', '3.11', '3.12']
     env:
       OS: ${{ matrix.os }}
       PYTHON: ${{ matrix.python-version }}
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `linsolve-1.1.3/.pre-commit-config.yaml` & `linsolve-1.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/LICENSE` & `linsolve-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/PKG-INFO` & `linsolve-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linsolve
-Version: 1.1.3
+Version: 1.1.4
 Summary: high-level tools for linearizing and solving systems of equations
 Author: HERA Team
 License: MIT License
         
         Copyright (c) 2017 Hydrogen Epoch of Reionization Array (HERA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,18 +27,18 @@
         
 Project-URL: Repository, https://github.com/HERA-Team/linsolve
 Keywords: linear equations,optimal estimation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.23
 Requires-Dist: scipy
 Provides-Extra: test
```

### Comparing `linsolve-1.1.3/README.md` & `linsolve-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/imgs/linear_model.png` & `linsolve-1.1.4/imgs/linear_model.png`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/imgs/points.png` & `linsolve-1.1.4/imgs/points.png`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/linsolve_example.ipynb` & `linsolve-1.1.4/linsolve_example.ipynb`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/pyproject.toml` & `linsolve-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 keywords=[
     "linear equations",
     "optimal estimation"
 ]
 dynamic = ["version"]
```

### Comparing `linsolve-1.1.3/src/linsolve/linsolve.py` & `linsolve-1.1.4/src/linsolve/linsolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,29 +32,23 @@
 from functools import reduce
 
 import numpy as np
 import scipy.linalg
 import scipy.sparse.linalg
 from scipy.sparse import csc_matrix
 
-# Monkey patch for backward compatibility:
-# ast.Num deprecated in Python 3.8. Make it an alias for ast.Constant
-# if it gets removed.
-if not hasattr(ast, "Num"):
-    ast.Num = ast.Constant
-
 
 def ast_getterms(n):
     """Convert an AST parse tree into a list of terms.
 
     E.g. 'a*x1+b*x2' -> [[a,x1],[b,x2]]
     """
     if type(n) is ast.Name:
         return [[n.id]]
-    elif type(n) is ast.Constant or type(n) is ast.Num:
+    elif type(n) is ast.Constant or type(n) is ast.Constant:
         return [[n.n]]
     elif type(n) is ast.Expression:
         return ast_getterms(n.body)
     elif type(n) is ast.UnaryOp:
         assert type(n.op) is ast.USub
         return [[-1] + ast_getterms(n.operand)[0]]
     elif type(n) is ast.BinOp:
@@ -879,16 +873,17 @@
             dict that maps equation strings from data to real weights to apply to each
             equation. Weights are treated as 1/sigma^2. All equations in the data must
             have a weight if wgts is not the default, {}, which means all 1.0s.
         sparse : bool
             If True, represents A matrix sparsely (though AtA, Aty end up dense)
             May be faster for certain systems of equations.
         build_solver : bool
-            Advanced users can turn this off to save memory when using only LinProductSolver
-            infrastructure but not solve() or solve_iteratively(), as in omnical.
+            Advanced users can turn this off to save memory when using only
+            LinProductSolver infrastructure but not solve() or solve_iteratively(), as
+            in omnical.
         **kwargs: keyword arguments of constants (python variables in keys of data that
             are not to be solved for)
         """
         # XXX make this something hard to collide with
         # see https://github.com/HERA-Team/linsolve/issues/17
         self.prepend = "d"
         self.data, self.sparse, self.keys = data, sparse, list(data.keys())
@@ -898,17 +893,19 @@
         self.sols_kwargs.update(sol0)
         self.all_terms, self.taylors, self.taylor_keys = self.gen_taylors()
         if build_solver:
             self.build_solver(sol0)
             self.dtype = self.ls.dtype
         else:
             self.sol0 = sol0
-            self.dtype = infer_dtype(list(self.data.values())
-                                     + list(self.sol0.values())
-                                     + list(self.wgts.values()))
+            self.dtype = infer_dtype(
+                list(self.data.values())
+                + list(self.sol0.values())
+                + list(self.wgts.values())
+            )
 
     def gen_taylors(self, keys=None):
         """Perform Taylor expansion, and map eq. keys to taylor expansion keys."""
         if keys is None:
             keys = self.keys
         all_terms = [ast_getterms(ast.parse(k, mode="eval")) for k in keys]
         taylors, taylor_keys = [], {}
```

### Comparing `linsolve-1.1.3/src/linsolve.egg-info/PKG-INFO` & `linsolve-1.1.4/src/linsolve.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linsolve
-Version: 1.1.3
+Version: 1.1.4
 Summary: high-level tools for linearizing and solving systems of equations
 Author: HERA Team
 License: MIT License
         
         Copyright (c) 2017 Hydrogen Epoch of Reionization Array (HERA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,18 +27,18 @@
         
 Project-URL: Repository, https://github.com/HERA-Team/linsolve
 Keywords: linear equations,optimal estimation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.23
 Requires-Dist: scipy
 Provides-Extra: test
```

### Comparing `linsolve-1.1.3/src/linsolve.egg-info/SOURCES.txt` & `linsolve-1.1.4/src/linsolve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/tests/benchmark_A_large_shared.py` & `linsolve-1.1.4/tests/benchmark_A_large_shared.py`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/tests/benchmark_A_large_shared_sparse.py` & `linsolve-1.1.4/tests/benchmark_A_large_shared_sparse.py`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/tests/benchmark_A_small_shared.py` & `linsolve-1.1.4/tests/benchmark_A_small_shared.py`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/tests/benchmark_A_small_shared_sparse.py` & `linsolve-1.1.4/tests/benchmark_A_small_shared_sparse.py`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/tests/benchmark_A_small_unique.py` & `linsolve-1.1.4/tests/benchmark_A_small_unique.py`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/tests/benchmark_A_small_unique_sparse.py` & `linsolve-1.1.4/tests/benchmark_A_small_unique_sparse.py`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.3/tests/test_linsolve.py` & `linsolve-1.1.4/tests/test_linsolve.py`

 * *Files identical despite different names*

