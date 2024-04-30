# Comparing `tmp/python-iArt-1.0.4.tar.gz` & `tmp/python-iArt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-iArt-1.0.4.tar", last modified: Sat Apr 27 21:59:34 2024, max compression
+gzip compressed data, was "python-iArt-1.1.0.tar", last modified: Tue Apr 30 04:56:14 2024, max compression
```

## Comparing `python-iArt-1.0.4.tar` & `python-iArt-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-27 21:59:34.750051 python-iArt-1.0.4/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-27 21:59:34.749695 python-iArt-1.0.4/PKG-INFO
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     3930 2024-04-09 03:41:46.000000 python-iArt-1.0.4/README.md
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-27 21:59:34.746838 python-iArt-1.0.4/iArt/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       48 2024-04-09 03:34:10.000000 python-iArt-1.0.4/iArt/__init__.py
--rw-r--r--   0 jiaweizhang   (501) staff       (20)    18837 2024-04-27 21:57:37.000000 python-iArt-1.0.4/iArt/iArt.py
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-27 21:59:34.749070 python-iArt-1.0.4/python_iArt.egg-info/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-27 21:59:34.000000 python-iArt-1.0.4/python_iArt.egg-info/PKG-INFO
--rw-r--r--   0 jiaweizhang   (501) staff       (20)      222 2024-04-27 21:59:34.000000 python-iArt-1.0.4/python_iArt.egg-info/SOURCES.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)        1 2024-04-27 21:59:34.000000 python-iArt-1.0.4/python_iArt.egg-info/dependency_links.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       66 2024-04-27 21:59:34.000000 python-iArt-1.0.4/python_iArt.egg-info/requires.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)        5 2024-04-27 21:59:34.000000 python-iArt-1.0.4/python_iArt.egg-info/top_level.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       38 2024-04-27 21:59:34.750201 python-iArt-1.0.4/setup.cfg
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     1059 2024-04-27 21:58:54.000000 python-iArt-1.0.4/setup.py
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-30 04:56:14.582780 python-iArt-1.1.0/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-30 04:56:14.582526 python-iArt-1.1.0/PKG-INFO
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     3930 2024-04-09 03:41:46.000000 python-iArt-1.1.0/README.md
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-30 04:56:14.580594 python-iArt-1.1.0/iArt/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       48 2024-04-09 03:34:10.000000 python-iArt-1.1.0/iArt/__init__.py
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)    18075 2024-04-30 04:55:09.000000 python-iArt-1.1.0/iArt/iArt.py
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-30 04:56:14.582113 python-iArt-1.1.0/python_iArt.egg-info/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-30 04:56:14.000000 python-iArt-1.1.0/python_iArt.egg-info/PKG-INFO
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)      222 2024-04-30 04:56:14.000000 python-iArt-1.1.0/python_iArt.egg-info/SOURCES.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)        1 2024-04-30 04:56:14.000000 python-iArt-1.1.0/python_iArt.egg-info/dependency_links.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       66 2024-04-30 04:56:14.000000 python-iArt-1.1.0/python_iArt.egg-info/requires.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)        5 2024-04-30 04:56:14.000000 python-iArt-1.1.0/python_iArt.egg-info/top_level.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       38 2024-04-30 04:56:14.582896 python-iArt-1.1.0/setup.cfg
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     1059 2024-04-30 04:55:27.000000 python-iArt-1.1.0/setup.py
```

### Comparing `python-iArt-1.0.4/PKG-INFO` & `python-iArt-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iArt
-Version: 1.0.4
+Version: 1.1.0
 Summary: iArt: A Generalized Framework for Imputation-Assisted Randomization Tests
 Home-page: https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py
 Author: Siyu Heng, Jiawei Zhang, and Yang Feng
 Author-email: siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu
 License: UNKNOWN
 Description: # iArt: Imputation-Assisted Randomization Tests
```

### Comparing `python-iArt-1.0.4/README.md` & `python-iArt-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `python-iArt-1.0.4/iArt/iArt.py` & `python-iArt-1.1.0/iArt/iArt.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     
     if covariate_adjustment == 0:
         return Y_head
     
     # suppress the warnings
     warnings.filterwarnings('ignore', category=ConvergenceWarning)
 
-    if covariate_adjustment == 'linear':
+    if covariate_adjustment == 1:
         warnings.filterwarnings(action='ignore', category=DataConversionWarning)
         # use linear regression to adjust the predicted Y values based on X
         Y_head_adjusted = np.zeros_like(Y_head)
         for i in range(lenY):
             # Extract the current target predictions
             Y_current = Y_head[:, i]
 
@@ -64,30 +64,30 @@
 
             # Predict and adjust for the current target
             Y_current_adjusted = lm.predict(X)
             Y_head_adjusted[:, i] = Y_current - Y_current_adjusted
 
         return Y_head_adjusted
     
-    if covariate_adjustment == 'xgboost':
+    if covariate_adjustment == 2:
         warnings.filterwarnings(action='ignore', category=DataConversionWarning)
         # use xgboost to adjust the predicted Y values based on X
         Y_head_adjusted = np.zeros_like(Y_head)
         for i in range(lenY):
             # Extract the current target predictions
             Y_current = Y_head[:, i]
 
             xg = xgb.XGBRegressor()
             xg.fit(X, Y_current)
             Y_current_adjusted = xg.predict(X)
             Y_head_adjusted[:, i] = Y_current - Y_current_adjusted
 
         return Y_head_adjusted
     
-    if covariate_adjustment == 'lightgbm':
+    if covariate_adjustment == 3:
         warnings.filterwarnings(action='ignore', category=DataConversionWarning)
         # use lightgbm to adjust the predicted Y values based on X
         Y_head_adjusted = np.zeros_like(Y_head)
         for i in range(lenY):
             # Extract the current target predictions
             Y_current = Y_head[:, i]
 
@@ -159,17 +159,17 @@
 
     # Create a Z_sim template for each unique value in S
     Z_sim_templates = []
     unique_strata = np.unique(S)
     for stratum in unique_strata:
         strata_indices = np.where(S == stratum)[0]
         strata_Z = Z_sorted[strata_indices]
-        p = np.mean(strata_Z)
+        n = int(np.sum(strata_Z))
         strata_size = len(strata_indices)
-        Z_sim_template = [0.0] * int(strata_size * (1 - p)) + [1.0] * (strata_size -int(strata_size * (1 - p)) )
+        Z_sim_template = [0.0] * (strata_size - n) + [1.0] * n
         Z_sim_templates.append(Z_sim_template)
     return Z_sim_templates
 
 def getZsim(Z_sim_templates):
     """ 
     Shuffle each Z_sim template and concatenate them into a single permutated Z_sim array 
     """
@@ -214,15 +214,15 @@
     Y = df.iloc[:, Z.shape[1] + X.shape[1]:Z.shape[1] + X.shape[1] + Y.shape[1]].values.reshape(-1, Y.shape[1])
     S = df.iloc[:, Z.shape[1] + X.shape[1] + Y.shape[1]:Z.shape[1] + X.shape[1] + Y.shape[1] + S.shape[1]].values.reshape(-1, 1)
 
     M = np.isnan(Y).reshape(-1, Y.shape[1])
     return Z, X, Y, S, M
 
 
-def check_param(*,Z, X, Y, S, G, L,randomization_design,threshold_covariate_median_imputation, verbose, covariate_adjustment,alpha,alternative,random_state):
+def check_param(*,Z, X, Y, S, G, L,mode, verbose, covariate_adjustment,alpha,alternative,random_state):
     """
     Check the validity of the input parameters
     """
 
     # check the dimension of Z, X, Y, S
     if Z.shape[0] != X.shape[0] or Z.shape[0] != Y.shape[0] or Z.shape[0] != S.shape[0]:
         raise ValueError("Z, X, Y, S must have the same number of rows")
@@ -251,33 +251,29 @@
     if not (0 < alpha <= 1):
         raise ValueError("alpha must be greater than 0 and less than or equal to 1")
     
     # Check G: Cannot be None
     if G is None:
         raise ValueError("G cannot be None")
     
-    # Check threshold_covariate_imputation: must be a float between 0 and 1
-    if not (0 <= threshold_covariate_median_imputation <= 1):
-        raise ValueError("threshold_covariate_median_imputation must be a float between 0 and 1")
-    
     # Check covariate_adjustment: must be True or False
-    if covariate_adjustment not in [0, 'linear', 'lightgbm', 'xgboost']:
-        raise ValueError("covariate_adjustment must be 0, linear, lightgbm, or xgboost")
+    if covariate_adjustment not in [0, 1, 2, 3]:
+        raise ValueError("covariate_adjustment must be one of 0, 1, 2, 3")
 
     # Check alternative: must be one of "greater", "less" or "two-sided" 
     if alternative not in ["greater", "less", "two-sided"]:
         raise ValueError("alternative must be one of greater, less or two-sided")
     
     # Check random_state: must be an integer greater than 0 or None
     if random_state != None and (not isinstance(random_state, int) or random_state < 0):
         raise ValueError("random_state must be an integer >= 0 or None")
     
-    # Check randomization_design: must be one of "strata" or "cluster"
-    if randomization_design not in ["strata", "cluster"]:
-        raise ValueError("randomization_design must be one of strata or cluster")
+    # Check mode: must be one of "strata" or "cluster"
+    if mode not in ["strata", "cluster"]:
+        raise ValueError("mode must be one of strata or cluster")
     
     
 def choosemodel(G):
     """ 
     Choose the imputation model based on the input parameter G.
     If G is a string, choose the imputation model based on the string.
     If G is a function, return the function.
@@ -342,50 +338,50 @@
         if len(columns_to_impute)>0:
             print(f"Missing Rate After Imputation for X: {missing_rate_after * 100}")
             print(f"Columns Imputed for X: {imputed_columns}")
         print(f"Columns Not Imputed for X: {not_imputed_columns}")
     
     return X
 
-def test(*,Z, X, Y, G='iterative+linear', S=None,L = 10000,threshold_covariate_median_imputation = 0.1, randomization_design = 'strata',verbose = False, covariate_adjustment = 0, random_state=None, alternative = "greater", alpha = 0.05):
+def test(*,Z, X, Y, G='linear', S=None,L = 10000,threshholdForX = 0.2, mode = 'strata',verbose = False, covariate_adjustment = 0, random_state=None, alternative = "greater", alpha = 0.05):
     """Imputation-Assisted Randomization Tests (iArt) for testing 
     the null hypothesis that the treatment has no effect on the outcome.
 
     Parameters
     ----------
     Z : array_like
         Z is the array of observed treatment indicators
 
     X, Y : array_like
         X is 2D array of observed covariates, Y is 2D array of observed outcomes,
     
     S : array_like, default: None
         S is the array of observed strata indicators
         
-    threshold_covariate_median_imputation : float, default: 0.1
-        The threshhold for missing covariate to be imputed with median in advance for performance improvement
+    threshholdForX : float, default: 0.1
+        The threshhold for missing outcome to be imputed in advance in covariate X
 
-    G : str or function, default: 'iterative+linear'
+    G : str or function, default: 'linear'
         A string for the eight available choice or a function that takes 
         (Z, M, Y_k) as input and returns the imputed complete values 
 
     L : int, default: 10000
         The number of Monte Carlo simulations 
 
-    randomization_design : {'strata','cluster'}, default: 'strata'
-        A string indicating the randomization design
+    mode : {'strata','cluster'}, default: 'strata'
+        A string indicating the randomization mode
 
     verbose : bool, default: False
         A boolean indicating whether to print training start and end 
 
     covarite_adjustment : int, default: 0
         if 0, covariate adjustment is not used
-        if linear, linear covariate adjustment is used
-        if xgboost, xgboost covariate adjustment is used
-        if lightgbm, lightgbm covariate adjustment is used
+        if 1, ridge covariate adjustment is used
+        if 2, xgboost covariate adjustment is used
+        if 3, lightgbm covariate adjustment is used
 
     random_state : {None, int, `numpy.random.Generator`,`numpy.random.RandomState`}, default: None
         If `seed` is None (or `np.random`), the `numpy.random.RandomState`
         singleton is used.
         If `seed` is an int, a new ``RandomState`` instance is used,
         seeded with `seed`.
         If `seed` is already a ``Generator`` or ``RandomState`` instance then
@@ -405,18 +401,18 @@
     reject : array_like
         A boolean indicating whether the null hypothesis is rejected for each outcome
     """
     start_time = time.time()
 
     # preprocess the variable
     Z, X, Y, S, M = preprocess(Z, X, Y, S)
-    X = transformX(X,threshold_covariate_median_imputation,verbose)
+    X = transformX(X,threshholdForX,verbose)
 
     # Check the validity of the input parameters
-    check_param(Z=Z, X=X, Y=Y, S=S, G=G, L=L,threshold_covariate_median_imputation = threshold_covariate_median_imputation, randomization_design=randomization_design, verbose=verbose, covariate_adjustment=covariate_adjustment, alpha=alpha, alternative=alternative, random_state=random_state)
+    check_param(Z=Z, X=X, Y=Y, S=S, G=G, L=L, mode=mode, verbose=verbose, covariate_adjustment=covariate_adjustment, alpha=alpha, alternative=alternative, random_state=random_state)
     
     # Set random seed
     np.random.seed(random_state)
 
     # choose the imputation model
     G_model = choosemodel(G)
 
@@ -436,26 +432,26 @@
             print("Covariate adjustment is not used")
         print("prediction Wilcoxon rank-sum test statistics:"+str(t_obs))
         #print wheather covariate adjustment is used
         print("=========================================================")
 
     # re-impute the missing values and calculate the observed test statistics in part 2
     t_sim = [ [] for _ in range(L)]
-    if randomization_design == 'strata':
+    if mode == 'strata':
         Z_sim_templates = getZsimTemplates(Z, S)
     else:
         p = 0.5
         cluster_indices = np.unique(S)
         num_clusters = len(cluster_indices)
         cluster_sim_template = np.array([0.0] * int(num_clusters * p) + [1.0] * (num_clusters - int(num_clusters * p)))
 
     for l in range(L):
         
         # simulate treatment indicators
-        if randomization_design == 'strata':
+        if mode == 'strata':
             Z_sim = getZsim(Z_sim_templates)
         else:
             cluster_sim = cluster_sim_template.copy()
             np.random.shuffle(cluster_sim)
             Z_sim = []
             for s in S.flatten():
                 Z_sim.append(cluster_sim[int(s) - 1])
```

### Comparing `python-iArt-1.0.4/python_iArt.egg-info/PKG-INFO` & `python-iArt-1.1.0/python_iArt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iArt
-Version: 1.0.4
+Version: 1.1.0
 Summary: iArt: A Generalized Framework for Imputation-Assisted Randomization Tests
 Home-page: https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py
 Author: Siyu Heng, Jiawei Zhang, and Yang Feng
 Author-email: siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu
 License: UNKNOWN
 Description: # iArt: Imputation-Assisted Randomization Tests
```

### Comparing `python-iArt-1.0.4/setup.py` & `python-iArt-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="python-iArt",
-    version="1.0.4",
+    version="1.1.0",
     author="Siyu Heng, Jiawei Zhang, and Yang Feng",
     author_email="siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu",
     description="iArt: A Generalized Framework for Imputation-Assisted Randomization Tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py",
     packages=find_packages(),
```

