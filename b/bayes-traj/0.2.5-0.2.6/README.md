# Comparing `tmp/bayes_traj-0.2.5.tar.gz` & `tmp/bayes_traj-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayes_traj-0.2.5.tar", last modified: Wed Jan 10 16:22:28 2024, max compression
+gzip compressed data, was "bayes_traj-0.2.6.tar", last modified: Tue Apr 30 15:00:31 2024, max compression
```

## Comparing `bayes_traj-0.2.5.tar` & `bayes_traj-0.2.6.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 jr555      (501) staff       (20)        0 2024-01-10 16:22:28.874733 bayes_traj-0.2.5/
--rw-r--r--   0 jr555      (501) staff       (20)     1335 2024-01-10 16:22:28.874306 bayes_traj-0.2.5/PKG-INFO
--rw-r--r--   0 jr555      (501) staff       (20)      871 2024-01-10 15:55:44.000000 bayes_traj-0.2.5/README.md
-drwxr-xr-x   0 jr555      (501) staff       (20)        0 2024-01-10 16:22:28.867210 bayes_traj-0.2.5/bayes_traj/
--rw-r--r--   0 jr555      (501) staff       (20)        0 2022-02-23 21:23:12.000000 bayes_traj-0.2.5/bayes_traj/__init__.py
--rw-r--r--   0 jr555      (501) staff       (20)     3295 2023-08-24 22:46:37.000000 bayes_traj-0.2.5/bayes_traj/assign_trajectory.py
--rw-r--r--   0 jr555      (501) staff       (20)    14911 2024-01-10 16:20:52.000000 bayes_traj-0.2.5/bayes_traj/bayes_traj_main.py
--rw-r--r--   0 jr555      (501) staff       (20)    18664 2022-09-20 14:17:03.000000 bayes_traj-0.2.5/bayes_traj/bayes_traj_main_alpha.py
--rw-r--r--   0 jr555      (501) staff       (20)     1851 2022-02-23 21:23:12.000000 bayes_traj-0.2.5/bayes_traj/bayes_traj_refiner.py
--rw-r--r--   0 jr555      (501) staff       (20)    10657 2023-08-22 22:12:17.000000 bayes_traj-0.2.5/bayes_traj/fit_stats.py
--rw-r--r--   0 jr555      (501) staff       (20)     5900 2022-02-23 21:23:12.000000 bayes_traj-0.2.5/bayes_traj/generate_generic_data.py
--rw-r--r--   0 jr555      (501) staff       (20)    27894 2023-08-23 15:40:20.000000 bayes_traj-0.2.5/bayes_traj/generate_prior.py
--rw-r--r--   0 jr555      (501) staff       (20)     1959 2022-02-23 21:23:12.000000 bayes_traj-0.2.5/bayes_traj/get_constraints_graph.py
--rw-r--r--   0 jr555      (501) staff       (20)     1442 2022-02-23 21:23:12.000000 bayes_traj-0.2.5/bayes_traj/get_longitudinal_constraints_graph.py
--rw-r--r--   0 jr555      (501) staff       (20)    73911 2024-01-10 00:34:36.000000 bayes_traj-0.2.5/bayes_traj/mult_dp_regression.py
--rw-r--r--   0 jr555      (501) staff       (20)     8638 2024-01-10 15:55:44.000000 bayes_traj-0.2.5/bayes_traj/mult_pyro.py
--rw-r--r--   0 jr555      (501) staff       (20)     3587 2022-02-23 21:23:12.000000 bayes_traj-0.2.5/bayes_traj/prior_from_model.py
--rw-r--r--   0 jr555      (501) staff       (20)    12025 2022-02-23 21:23:12.000000 bayes_traj-0.2.5/bayes_traj/psis.py
--rw-r--r--   0 jr555      (501) staff       (20)     7562 2023-12-22 17:27:37.000000 bayes_traj-0.2.5/bayes_traj/summarize_traj_model.py
-drwxr-xr-x   0 jr555      (501) staff       (20)        0 2024-01-10 16:22:28.873661 bayes_traj-0.2.5/bayes_traj/tests/
--rw-r--r--   0 jr555      (501) staff       (20)        0 2022-02-23 21:23:12.000000 bayes_traj-0.2.5/bayes_traj/tests/__init__.py
--rw-r--r--   0 jr555      (501) staff       (20)     9696 2023-08-23 15:31:10.000000 bayes_traj-0.2.5/bayes_traj/tests/test_fit_stats.py
--rw-r--r--   0 jr555      (501) staff       (20)    25841 2023-08-23 15:10:43.000000 bayes_traj-0.2.5/bayes_traj/tests/test_generate_prior.py
--rw-r--r--   0 jr555      (501) staff       (20)    23163 2023-08-23 15:23:47.000000 bayes_traj-0.2.5/bayes_traj/tests/test_mult_dp_regression.py
--rw-r--r--   0 jr555      (501) staff       (20)     1226 2024-01-10 15:55:44.000000 bayes_traj-0.2.5/bayes_traj/tests/test_mult_pyro.py
--rw-r--r--   0 jr555      (501) staff       (20)      800 2022-02-23 21:23:12.000000 bayes_traj-0.2.5/bayes_traj/tests/test_utils.py
--rw-r--r--   0 jr555      (501) staff       (20)     1387 2022-03-03 20:13:24.000000 bayes_traj-0.2.5/bayes_traj/update_model.py
--rw-r--r--   0 jr555      (501) staff       (20)     4897 2022-02-23 21:23:12.000000 bayes_traj-0.2.5/bayes_traj/utils.py
--rw-r--r--   0 jr555      (501) staff       (20)     6445 2024-01-10 15:54:52.000000 bayes_traj-0.2.5/bayes_traj/viz_data_prior_draws.py
--rw-r--r--   0 jr555      (501) staff       (20)     4577 2022-07-12 16:26:27.000000 bayes_traj-0.2.5/bayes_traj/viz_gamma_dists.py
--rw-r--r--   0 jr555      (501) staff       (20)     6321 2023-09-12 18:45:55.000000 bayes_traj-0.2.5/bayes_traj/viz_model_trajs.py
-drwxr-xr-x   0 jr555      (501) staff       (20)        0 2024-01-10 16:22:28.870350 bayes_traj-0.2.5/bayes_traj.egg-info/
--rw-r--r--   0 jr555      (501) staff       (20)     1335 2024-01-10 16:22:28.000000 bayes_traj-0.2.5/bayes_traj.egg-info/PKG-INFO
--rw-r--r--   0 jr555      (501) staff       (20)     1050 2024-01-10 16:22:28.000000 bayes_traj-0.2.5/bayes_traj.egg-info/SOURCES.txt
--rw-r--r--   0 jr555      (501) staff       (20)        1 2024-01-10 16:22:28.000000 bayes_traj-0.2.5/bayes_traj.egg-info/dependency_links.txt
--rw-r--r--   0 jr555      (501) staff       (20)      496 2024-01-10 16:22:28.000000 bayes_traj-0.2.5/bayes_traj.egg-info/entry_points.txt
--rw-r--r--   0 jr555      (501) staff       (20)      159 2024-01-10 16:22:28.000000 bayes_traj-0.2.5/bayes_traj.egg-info/requires.txt
--rw-r--r--   0 jr555      (501) staff       (20)       11 2024-01-10 16:22:28.000000 bayes_traj-0.2.5/bayes_traj.egg-info/top_level.txt
--rw-r--r--   0 jr555      (501) staff       (20)       38 2024-01-10 16:22:28.874891 bayes_traj-0.2.5/setup.cfg
--rw-r--r--   0 jr555      (501) staff       (20)     2742 2024-01-10 16:21:16.000000 bayes_traj-0.2.5/setup.py
+drwxr-xr-x   0 jr555      (501) staff       (20)        0 2024-04-30 15:00:31.501925 bayes_traj-0.2.6/
+-rw-r--r--   0 jr555      (501) staff       (20)     1335 2024-04-30 15:00:31.502171 bayes_traj-0.2.6/PKG-INFO
+-rw-r--r--   0 jr555      (501) staff       (20)      871 2024-04-11 14:59:23.000000 bayes_traj-0.2.6/README.md
+drwxr-xr-x   0 jr555      (501) staff       (20)        0 2024-04-30 15:00:31.495072 bayes_traj-0.2.6/bayes_traj/
+-rw-r--r--   0 jr555      (501) staff       (20)        0 2022-02-23 21:23:12.000000 bayes_traj-0.2.6/bayes_traj/__init__.py
+-rw-r--r--   0 jr555      (501) staff       (20)     3293 2024-04-26 20:29:12.000000 bayes_traj-0.2.6/bayes_traj/assign_trajectory.py
+-rw-r--r--   0 jr555      (501) staff       (20)    15744 2024-04-26 20:29:12.000000 bayes_traj-0.2.6/bayes_traj/bayes_traj_main.py
+-rw-r--r--   0 jr555      (501) staff       (20)    18664 2022-09-20 14:17:03.000000 bayes_traj-0.2.6/bayes_traj/bayes_traj_main_alpha.py
+-rw-r--r--   0 jr555      (501) staff       (20)     1851 2022-02-23 21:23:12.000000 bayes_traj-0.2.6/bayes_traj/bayes_traj_refiner.py
+-rw-r--r--   0 jr555      (501) staff       (20)    10657 2024-04-11 14:59:23.000000 bayes_traj-0.2.6/bayes_traj/fit_stats.py
+-rw-r--r--   0 jr555      (501) staff       (20)     6059 2024-04-26 20:29:12.000000 bayes_traj-0.2.6/bayes_traj/generate_generic_data.py
+-rw-r--r--   0 jr555      (501) staff       (20)    36432 2024-04-26 20:29:12.000000 bayes_traj-0.2.6/bayes_traj/generate_prior.py
+-rw-r--r--   0 jr555      (501) staff       (20)     1959 2022-02-23 21:23:12.000000 bayes_traj-0.2.6/bayes_traj/get_constraints_graph.py
+-rw-r--r--   0 jr555      (501) staff       (20)     1442 2022-02-23 21:23:12.000000 bayes_traj-0.2.6/bayes_traj/get_longitudinal_constraints_graph.py
+-rw-r--r--   0 jr555      (501) staff       (20)    74012 2024-04-26 20:29:12.000000 bayes_traj-0.2.6/bayes_traj/mult_dp_regression.py
+-rw-r--r--   0 jr555      (501) staff       (20)    21129 2024-04-26 20:29:12.000000 bayes_traj-0.2.6/bayes_traj/mult_pyro.py
+-rw-r--r--   0 jr555      (501) staff       (20)     3587 2022-02-23 21:23:12.000000 bayes_traj-0.2.6/bayes_traj/prior_from_model.py
+-rw-r--r--   0 jr555      (501) staff       (20)    12025 2022-02-23 21:23:12.000000 bayes_traj-0.2.6/bayes_traj/psis.py
+-rw-r--r--   0 jr555      (501) staff       (20)     4828 2024-04-26 20:29:12.000000 bayes_traj-0.2.6/bayes_traj/pyro_helper.py
+-rw-r--r--   0 jr555      (501) staff       (20)     7562 2024-04-11 14:59:23.000000 bayes_traj-0.2.6/bayes_traj/summarize_traj_model.py
+drwxr-xr-x   0 jr555      (501) staff       (20)        0 2024-04-30 15:00:31.501088 bayes_traj-0.2.6/bayes_traj/tests/
+-rw-r--r--   0 jr555      (501) staff       (20)        0 2022-02-23 21:23:12.000000 bayes_traj-0.2.6/bayes_traj/tests/__init__.py
+-rw-r--r--   0 jr555      (501) staff       (20)     9696 2024-04-26 15:29:31.000000 bayes_traj-0.2.6/bayes_traj/tests/test_fit_stats.py
+-rw-r--r--   0 jr555      (501) staff       (20)    25911 2024-04-26 20:29:12.000000 bayes_traj-0.2.6/bayes_traj/tests/test_generate_prior.py
+-rw-r--r--   0 jr555      (501) staff       (20)    23163 2024-04-11 14:59:23.000000 bayes_traj-0.2.6/bayes_traj/tests/test_mult_dp_regression.py
+-rw-r--r--   0 jr555      (501) staff       (20)     3155 2024-04-26 20:29:12.000000 bayes_traj-0.2.6/bayes_traj/tests/test_mult_pyro.py
+-rw-r--r--   0 jr555      (501) staff       (20)      800 2022-02-23 21:23:12.000000 bayes_traj-0.2.6/bayes_traj/tests/test_utils.py
+-rw-r--r--   0 jr555      (501) staff       (20)     1387 2022-03-03 20:13:24.000000 bayes_traj-0.2.6/bayes_traj/update_model.py
+-rw-r--r--   0 jr555      (501) staff       (20)     4897 2022-02-23 21:23:12.000000 bayes_traj-0.2.6/bayes_traj/utils.py
+-rw-r--r--   0 jr555      (501) staff       (20)     6445 2024-01-10 15:54:52.000000 bayes_traj-0.2.6/bayes_traj/viz_data_prior_draws.py
+-rw-r--r--   0 jr555      (501) staff       (20)     4577 2022-07-12 16:26:27.000000 bayes_traj-0.2.6/bayes_traj/viz_gamma_dists.py
+-rw-r--r--   0 jr555      (501) staff       (20)     6321 2024-04-11 14:59:23.000000 bayes_traj-0.2.6/bayes_traj/viz_model_trajs.py
+drwxr-xr-x   0 jr555      (501) staff       (20)        0 2024-04-30 15:00:31.497499 bayes_traj-0.2.6/bayes_traj.egg-info/
+-rw-r--r--   0 jr555      (501) staff       (20)     1335 2024-04-30 15:00:31.000000 bayes_traj-0.2.6/bayes_traj.egg-info/PKG-INFO
+-rw-r--r--   0 jr555      (501) staff       (20)     1086 2024-04-30 15:00:31.000000 bayes_traj-0.2.6/bayes_traj.egg-info/SOURCES.txt
+-rw-r--r--   0 jr555      (501) staff       (20)        1 2024-04-30 15:00:31.000000 bayes_traj-0.2.6/bayes_traj.egg-info/dependency_links.txt
+-rw-r--r--   0 jr555      (501) staff       (20)      496 2024-04-30 15:00:31.000000 bayes_traj-0.2.6/bayes_traj.egg-info/entry_points.txt
+-rw-r--r--   0 jr555      (501) staff       (20)      193 2024-04-30 15:00:31.000000 bayes_traj-0.2.6/bayes_traj.egg-info/requires.txt
+-rw-r--r--   0 jr555      (501) staff       (20)       11 2024-04-30 15:00:31.000000 bayes_traj-0.2.6/bayes_traj.egg-info/top_level.txt
+-rw-r--r--   0 jr555      (501) staff       (20)       69 2024-04-30 15:00:31.502839 bayes_traj-0.2.6/setup.cfg
+-rw-r--r--   0 jr555      (501) staff       (20)     2810 2024-04-30 14:59:33.000000 bayes_traj-0.2.6/setup.py
```

### Comparing `bayes_traj-0.2.5/PKG-INFO` & `bayes_traj-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayes_traj
-Version: 0.2.5
+Version: 0.2.6
 Summary: bayes_traj
 Home-page: https://github.com/acil-bwh/bayes_traj
 Author: James Ross
 Author-email: jross@bwh.harvard.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `bayes_traj-0.2.5/README.md` & `bayes_traj-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/assign_trajectory.py` & `bayes_traj-0.2.6/bayes_traj/assign_trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 def main():
     """
     """
     desc = """Assigns individuals to trajectory subgroups using their data 
     contained the input csv file and a trajectory model. The individuals can be 
     different from those used to train the model. However, it is assumed that 
-    the predictor names and target names  match."""
+    the predictor names and target names match."""
 
     args = ArgumentParser(desc)
     args.add_argument('--in_csv', help='Input csv data file. Individuals in \
         this file will be assigned to the best trajectory', required=True,
         type=str)
     args.add_argument('--groupby', help='Subject identifier column name in the \
-        input data file to use for grouping. ', required=False, type=str,
+        input data file to use for grouping.', required=False, type=str,
         default=None)    
     args.add_argument('--model', help='Pickled trajectory model to use for \
         assigning data instances to trajectories', type=str, required=True)
     args.add_argument('--out_csv', help='Output csv file with data instances \
         assigned to trajectories. The output csv file will be identical to the \
         input csv file, but it will additionally have a traj column indicating \
         the trajectory number with the highest assigmnet probability. It will \
```

### Comparing `bayes_traj-0.2.5/bayes_traj/bayes_traj_main.py` & `bayes_traj-0.2.6/bayes_traj/bayes_traj_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 #!/usr/bin/env python
 
 from argparse import ArgumentParser
 import pandas as pd
 import numpy as np
 from bayes_traj.mult_dp_regression import MultDPRegression
+from bayes_traj.mult_pyro import MultPyro
 from bayes_traj.prior_from_model import prior_from_model
 from bayes_traj.utils import *
 from bayes_traj.fit_stats import compute_waic2
+import torch
+import pyro
+from bayes_traj.pyro_helper import *
 from provenance_tools.write_provenance_data import write_provenance_data
-import pdb, pickle, sys, warnings
+import pickle, sys, warnings
+
+torch.set_default_dtype(torch.double) # TODO -- may not be desirable to set this globally
 
 def main():
     """
     """
     np.set_printoptions(precision = 1, suppress = True, threshold=1e6,
                         linewidth=300)
 
@@ -241,17 +247,32 @@
                    w_mu=prior_data['w_mu'],
                    w_var=prior_data['w_var'],
                    lambda_a=prior_data['lambda_a'],
                    lambda_b=prior_data['lambda_b'],
                    weights_only=op.weights_only,
                    num_init_trajs=op.num_init_trajs)
         else:
-            raise NotImplementedError("Pyro not yet implemented")
+            restructured_data = get_restructured_data(df, preds, targets, op.groupby)
+            model = MultPyro(
+                alpha0=torch.full((K,), 100.0, dtype=torch.double),
+                w_mu0=torch.from_numpy(prior_data['w_mu0'].T).double(),
+                w_var0=torch.from_numpy(prior_data['w_var0'].T).double(),
+                lambda_a0=torch.from_numpy(prior_data['lambda_a0']).double(),
+                lambda_b0=torch.from_numpy(prior_data['lambda_b0']).double(),
+                **restructured_data
+            )
+
+            model.fit(num_steps=iters)
+
+            if op.out_model is not None:
+                torch.save(model, op.out_model)
 
-        if r == 0:
+        if op.use_pyro:
+            pass
+        elif r == 0:
             if op.out_model is not None:
                 print("Saving model...")
                 pickle.dump({'MultDPRegression': mm}, open(op.out_model, 'wb'))
 
                 print("Saving model provenance info...")
                 provenance_desc = """ """
                 write_provenance_data(op.out_model, generator_args=op,
```

### Comparing `bayes_traj-0.2.5/bayes_traj/bayes_traj_main_alpha.py` & `bayes_traj-0.2.6/bayes_traj/bayes_traj_main_alpha.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/bayes_traj_refiner.py` & `bayes_traj-0.2.6/bayes_traj/bayes_traj_refiner.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/fit_stats.py` & `bayes_traj-0.2.6/bayes_traj/fit_stats.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/generate_generic_data.py` & `bayes_traj-0.2.6/bayes_traj/generate_generic_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
         dest='visit_span', type=float, default=None)
     parser.add_argument('--max_age', help='No subject age will be above this amount',
         dest='max_age', type=float, default=95)
     parser.add_argument('--num_visits', help='Number of longitudinal visits \
         per individual. Note that the actual number for an individual may be less \
         than this if the generated age for a visit is greater than max_age',
         dest='num_visits', type=int, default=1)
+    parser.add_argument('--cohort', help='Name of cohort to be stored in the \
+        cohort column', type=str, default='A')    
     parser.add_argument('--out_file', help='Output data file name. Columns \
         include: intercept, x, x^2, y, id, data_names, traj.', default=None)
     
     op = parser.parse_args()
     
     enrollment_min = int(op.enrollment.split(',')[0])
     enrollment_max = int(op.enrollment.split(',')[1])
@@ -124,15 +126,16 @@
                             df_out[ids]['y{}'.format(d+1)].values, edgecolor='k',
                             color=cmap(tt), alpha=0.5,
                             label='Traj {} (N={})'.format(tt+1, num_in_traj))
                 axs.set_xlabel('Age')
                 axs.set_ylabel('y{}'.format(d+1))
                 axs.legend()
     plt.show()
-    
+
+    df_out['cohort'] = op.cohort
     if op.out_file is not None:
         print("Writing to file...")
         df_out.to_csv(op.out_file, index=False)
         write_provenance_data(op.out_file, generator_args=op,
                               module_name='bayes_traj')
     
     print("DONE.")
```

### Comparing `bayes_traj-0.2.5/bayes_traj/generate_prior.py` & `bayes_traj-0.2.6/bayes_traj/generate_prior.py`

 * *Files 14% similar despite different names*

```diff
@@ -245,15 +245,15 @@
                 res_tmp.HC0_se.values[i]**2
 
         gamma_mean = 1/np.var(res_tmp.resid.values)
         gamma_var = 0.005 # Heuristic
 
         self.prior_info_['lambda_b'][target][traj] = gamma_mean/gamma_var
         self.prior_info_['lambda_a'][target][traj] = gamma_mean**2/gamma_var
-
+        
     def traj_prior_info_from_model(self, target, traj):
         """This function will retrieve prior information (w_mu, w_var, 
         lambda_a, lambda_b) for a specific trajectory based on a previously fit
         model. Assumes that the model predictors and the predictors for which 
         to compute priors are the same. Also assumes that 'target' is in the
         model.
 
@@ -265,14 +265,17 @@
         traj : int
             Prior information will be retrieved for those data instances 
             belonging to this trajectory.    
         """
         assert self.mm_ is not None, \
             "Trying to set prior info from model, but no model specified"
 
+        assert set(self.prior_info_['w_mu0'][target].keys()) == \
+            set(self.mm_.predictor_names_), "Predictor name mismatch"
+        
         target_index = \
             np.where(np.array(self.mm_.target_names_) == target)[0][0]
 
         self.prior_info_['lambda_a'][target][traj] = \
             self.mm_.lambda_a_[target_index][traj]
         self.prior_info_['lambda_b'][target][traj] = \
             self.mm_.lambda_b_[target_index][traj]
@@ -282,15 +285,15 @@
                 np.where(np.array(self.mm_.predictor_names_) == m)[0][0]
 
             self.prior_info_['w_mu'][m][target][traj] = \
                 self.mm_.w_mu_[pred_index, target_index, traj]
             self.prior_info_['w_var'][m][target][traj] = \
                 self.mm_.w_var_[pred_index, target_index, traj]            
         
-    def prior_info_from_df(self, target):
+    def prior_info_from_df_gaussians(self, target):
         """Computes w_mu0, w_var0, lambda_a0, lambda_b0
 
         Parameters
         ----------
         target : string
             Name of target variable for which to compute prior information
         """
@@ -459,18 +462,227 @@
                                 self.traj_prior_info_from_df(tt, kk)
             else:
                 # No model, but we have data. Because we have no model, we also
                 # won't have df_traj_data_, so we won't be able to get per-traj
                 # information
                 self.prior_info_from_df(tt)
 
+    def prior_info_from_df_binary(self, target):
+        """
+        """
+        self.prior_info_['lambda_b0'][target] = None
+        self.prior_info_['lambda_a0'][target] = None
+     
+        res_tmp = sm.Logit(self.df_data_[target], self.df_data_[self.preds_],
+                           missing='drop').fit()
+    
+        samples = np.random.multivariate_normal(res_tmp.params.values,
+            res_tmp.cov_params().values, 10000)
+
+        for (i, m) in enumerate(self.preds_):
+            self.prior_info_['w_mu0'][target][m] = np.mean(samples, 0)[i]
+            self.prior_info_['w_var0'][target][m] = np.var(samples, 0)[i]
+
+    def prior_info_from_df(self, target):
+        """
+        """
+        nonnan_ids = ~np.isnan(self.df_data_[target].values)
+        if set(self.df_data_[target].values[nonnan_ids]).issubset({1.0, 0.0}):
+            self.prior_info_from_df_binary(target)
+        else:
+            self.prior_info_from_df_gaussians(target)
+
+            
+
 #-------------------------               
 # END OF CLASS DEFINITION
 #-------------------------        
-    
+
+
+#def prior_info_from_df_traj(df_traj, target_name, preds, prior_info,
+#                            traj_ids=None):
+#    """ Takes in a dataframe in which each data instance has a trajectory 
+#    assignment, and from this dataframe and specified target name and 
+#    predictors, estimates information for the prior. 
+#
+#    Parameters
+#    ----------
+#    df_traj : pandas dataframe
+#        Must have as columns 'target_name' and 'preds'. Must also have a 'traj' 
+#        column as well as columns called 'traj_x', where 'x' is an integer
+#        indicating a trajectory number. These columns contain the probability 
+#        that the data instance belongs to that trajectory.
+#
+#    target_name : str
+#        Name of the target variable
+#
+#    preds : list of strings
+#        The predictor names
+#
+#    prior_info : dict
+#        Prior data structure that will be updated by this function
+#
+#    traj_ids : array of ints, optional
+#        Subset of trajectories to use for informing prior setting. It may be 
+#        desirable to use a subset in case some trajectories have been deemed to
+#        be spurios or unstable
+#    """
+#    prior_info['alpha'] = traj_ids.shape[0]/np.log10(df_traj.shape[0])
+#        
+#    nonnan_ids = ~np.isnan(df_traj[target_name].values)
+#    if set(df_traj[target_name].values[nonnan_ids]).issubset({1.0, 0.0}):
+#        prior_info_from_df_traj_binary(df_traj, target_name, preds,
+#                                       prior_info, traj_ids)
+#    else:
+#        prior_info_from_df_traj_gaussian(df_traj, target_name, preds,
+#                                         prior_info, traj_ids)
+#        
+#-def prior_info_from_df_traj_gaussian(df_traj, target_name, preds, prior_info,
+#                                     traj_ids=None):
+#    """ Takes in a dataframe in which each data instance has a trajectory 
+#    assignment, and from this dataframe and specified target name and 
+#    predictors, estimates information for the prior. Estimates are made by 
+#    performing OLS regression within each trajectory subgroup and tallying
+#    regression coefficients and residuals.
+#
+#    Parameters
+#    ----------
+#    df_traj : pandas dataframe
+#        Must have as columns 'target_name' and 'preds'. Must also have a 'traj' 
+#        column as well as columns called 'traj_x', where 'x' is an integer
+#        indicating a trajectory number. These columns contain the probability 
+#        that the data instance belongs to that trajectory.
+#
+#    target_name : str
+#        Name of the target variable
+#
+#    preds : list of strings
+#        The predictor names
+#
+#    prior_info : dict
+#        Prior data structure that will be updated by this function
+#
+#    traj_ids : array of ints, optional
+#        Subset of trajectories to use for informing prior setting. It may be 
+#        desirable to use a subset in case some trajectories have been deemed to
+#        be spurios or unstable
+#    """    
+#    if traj_ids is None:
+#        traj_ids = np.array(list(set(df_traj.traj.values)))
+#
+#    traj_col_names = []
+#    for i in traj_ids:
+#        traj_col_names.append('traj_{}'.format(i))
+#
+#    traj_probs = np.sum(df_traj[traj_col_names].values, 0)/\
+#        np.sum(df_traj[traj_col_names].values)
+#    
+#    num_traj_samples = np.random.multinomial(10000, traj_probs)    
+#
+#    samples = np.zeros([10000, len(preds)])
+#    prev = 0
+#    resids = np.zeros(df_traj.shape[0])
+#    for (i, t) in enumerate(traj_ids):
+#        ids = (df_traj.traj.values == t) & \
+#            ~np.isnan(df_traj[target_name].values)
+#        res_tmp = sm.OLS(df_traj[ids][target_name], df_traj[ids][preds],
+#                         missing='drop').fit()
+#        
+#        samples[prev:np.cumsum(num_traj_samples)[i], :] = \
+#            np.random.multivariate_normal(res_tmp.params.values,
+#                                          np.diag(res_tmp.HC0_se.values**2),
+#                                          num_traj_samples[i])
+#        prev = np.cumsum(num_traj_samples)[i]
+#        resids[ids] = res_tmp.resid.values
+#
+#    for (i, m) in enumerate(preds):
+#        prior_info['w_mu0'][target_name][m] = np.mean(samples, 0)[i]
+#        prior_info['w_var0'][target_name][m] = np.var(samples, 0)[i]
+#
+#    sel_ids = np.zeros(df_traj.shape[0], dtype=bool)
+#    sel_ids[0:int(df_traj.shape[0]/2.)] = True
+#
+#    prec_vec = []
+#    for i in range(100):
+#        sel_ids = np.random.permutation(sel_ids)
+#        prec_vec.append(1./np.var(resids[sel_ids]))
+#
+#    gamma_mean = np.mean(prec_vec)
+#    gamma_var = np.var(prec_vec)
+#
+#    prior_info['lambda_b0'][target_name] = gamma_mean/gamma_var
+#    prior_info['lambda_a0'][target_name] = gamma_mean**2/gamma_var
+#
+#def prior_info_from_df_traj_binary(df_traj, target_name, preds, prior_info,
+#                                   traj_ids=None):
+#    """ Takes in a dataframe in which each data instance has a trajectory 
+#    assignment, and from this dataframe and specified target name and 
+#    predictors, estimates information for the prior. Estimates are made by 
+#    performing logistic regression within each trajectory subgroup and tallying
+#    regression coefficients and residuals.
+#
+#    Parameters
+#    ----------
+#    df_traj : pandas dataframe
+#        Must have as columns 'target_name' and 'preds'. Must also have a 'traj' 
+#        column as well as columns called 'traj_x', where 'x' is an integer
+#        indicating a trajectory number. These columns contain the probability 
+#        that the data instance belongs to that trajectory.
+#
+#    target_name : str
+#        Name of the target variable
+#
+#    preds : list of strings
+#        The predictor names
+#
+#    prior_info : dict
+#        Prior data structure that will be updated by this function
+#
+#    traj_ids : array of ints, optional
+#        Subset of trajectories to use for informing prior setting. It may be 
+#        desirable to use a subset in case some trajectories have been deemed to
+#        be spurios or unstable
+#    """        
+#    prior_info['lambda_b0'][target_name] = None
+#    prior_info['lambda_a0'][target_name] = None
+#    
+#    if traj_ids is None:
+#        traj_ids = np.array(list(set(df_traj.traj.values)))
+#
+#    traj_col_names = []
+#    for i in traj_ids:
+#        traj_col_names.append('traj_{}'.format(i))
+#            
+#    traj_probs = np.sum(df_traj[traj_col_names].values, 0)/\
+#        np.sum(df_traj[traj_col_names].values)
+#    
+#    num_traj_samples = np.random.multinomial(10000, traj_probs)    
+#
+#    samples = np.zeros([10000, len(preds)])
+#    prev = 0
+#    for (i, t) in enumerate(traj_ids):
+#        ids = (df_traj.traj.values == t) & \
+#            ~np.isnan(df_traj[target_name].values)
+#        res_tmp = sm.Logit(df_traj[ids][target_name], df_traj[ids][preds],
+#                         missing='drop').fit()
+#        
+#        samples[prev:np.cumsum(num_traj_samples)[i], :] = \
+#            np.random.multivariate_normal(res_tmp.params.values,
+#                                          res_tmp.cov_params().values,
+#                                          num_traj_samples[i])
+#        prev = np.cumsum(num_traj_samples)[i]
+#
+#    for (i, m) in enumerate(preds):
+#        prior_info['w_mu0'][target_name][m] = np.mean(samples, 0)[i]
+#        prior_info['w_var0'][target_name][m] = np.var(samples, 0)[i]
+
+
+
+#-------------------------------------------------------------------------------
+
 def main():        
     desc = """Generates a pickled file containing Bayesian trajectory prior 
     information"""
     
     parser = ArgumentParser(description=desc)
     parser.add_argument('--preds', help='Comma-separated list of predictor names',
         dest='preds', type=str, default=None)
```

### Comparing `bayes_traj-0.2.5/bayes_traj/get_constraints_graph.py` & `bayes_traj-0.2.6/bayes_traj/get_constraints_graph.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/get_longitudinal_constraints_graph.py` & `bayes_traj-0.2.6/bayes_traj/get_longitudinal_constraints_graph.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/mult_dp_regression.py` & `bayes_traj-0.2.6/bayes_traj/mult_dp_regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1295,18 +1295,20 @@
             else:
                 scale_factor = self.N_
             self.lambda_a_ = \
                 (scale_factor*torch.ones([self.D_, self.K_])).double()
             self.lambda_b_ = \
                 (scale_factor*torch.ones([self.D_, self.K_])).double()
             for d in range(self.D_):
-                scale = 1./self.lambda_b0_[d]
-                shape = self.lambda_a0_[d]                                
-                self.lambda_a_[d, :] = self.lambda_a_[d, :]*(\
-                    torch.distributions.Gamma(shape, scale).sample((self.K_,)))
+                if self.target_type_[d] == 'gaussian':
+                    scale = 1./self.lambda_b0_[d]
+                    shape = self.lambda_a0_[d]                                
+                    self.lambda_a_[d, :] = self.lambda_a_[d, :]*(\
+                        torch.distributions.Gamma(shape, scale).\
+                            sample((self.K_,)))
 
         if torch.isnan(torch.sum(self.lambda_a_)):
             for dd in range(self.D_):
                 for kk in range(self.K_):
                     if torch.isnan(self.lambda_a_[dd, kk]):
                         self.lambda_b_[dd, kk] = 1
                         scale = 1./self.lambda_b0_[dd]
```

### Comparing `bayes_traj-0.2.5/bayes_traj/prior_from_model.py` & `bayes_traj-0.2.6/bayes_traj/prior_from_model.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/psis.py` & `bayes_traj-0.2.6/bayes_traj/psis.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/summarize_traj_model.py` & `bayes_traj-0.2.6/bayes_traj/summarize_traj_model.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/tests/test_fit_stats.py` & `bayes_traj-0.2.6/bayes_traj/tests/test_fit_stats.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/tests/test_generate_prior.py` & `bayes_traj-0.2.6/bayes_traj/tests/test_generate_prior.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,25 @@
     mm = pickle.load(open(model_file_name, 'rb'))['MultDPRegression']
     
     targets = ['y']
     preds = ['intercept', 'age']
     pg = PriorGenerator(targets, preds)
     pg.set_model(mm)
     pg.prior_info_from_model('y')
-
-    assert np.isclose(pg.prior_info_['w_mu0']['y']['intercept'], 7.810441593), \
+    assert np.isclose(pg.prior_info_['w_mu0']['y']['intercept'], 7.73326866724), \
         "w_mu0 not as expected"
-    assert np.isclose(pg.prior_info_['w_mu0']['y']['age'], -1.48068743758711), \
+    assert np.isclose(pg.prior_info_['w_mu0']['y']['age'], -1.47391042070), \
         "w_mu0 not as expected"
-    assert np.isclose(pg.prior_info_['w_var0']['y']['intercept'], 0.51800801), \
+    assert np.isclose(pg.prior_info_['w_var0']['y']['intercept'], 0.46760358415383), \
         "w_var0 not as expected"    
-    assert np.isclose(pg.prior_info_['w_var0']['y']['age'], 0.04260915525159), \
+    assert np.isclose(pg.prior_info_['w_var0']['y']['age'], 0.0439302696606), \
         "w_var0 not as expected"
-    assert np.isclose(pg.prior_info_['lambda_a0']['y'], 207.87669370617036), \
+    assert np.isclose(pg.prior_info_['lambda_a0']['y'], 17.7068686687), \
         "lambda_a0 not as expected"
-    assert np.isclose(pg.prior_info_['lambda_b0']['y'], 67.86146951205156), \
+    assert np.isclose(pg.prior_info_['lambda_b0']['y'], 24.0246304888), \
         "lambda_b0 not as expected"
     
 def test_prior_info_from_df():
     """
     """
     data_file_name = os.path.split(os.path.realpath(__file__))[0] + \
         '/../resources/data/trajectory_data_1.csv'
@@ -94,15 +93,15 @@
     #---------------------------------------------------------------------------
     # Evaluate prior for trajectory 5
     #---------------------------------------------------------------------------
     intercept_co = 10
     age_co = -1
     resid_std = 2
 
-    traj = 5
+    traj = 1
     pg.traj_prior_info_from_df('y', traj)
 
     mu = pg.prior_info_['w_mu']['intercept']['y'][traj]
     sig = np.sqrt(pg.prior_info_['w_var']['intercept']['y'][traj])
 
     assert mu - 2*sig <= intercept_co and mu + 2*sig >= intercept_co, \
         "Intercept prior not as expected for trajectory 5"
@@ -119,15 +118,15 @@
     prec_high = prec_mean + 2*np.sqrt(prec_var)
     prec_low= prec_mean - 2*np.sqrt(prec_var)
 
     std_high = np.sqrt(1/prec_low)
     std_low = np.sqrt(1/prec_high)
 
     assert resid_std >= std_low and resid_std <= std_high, \
-        "Prior over residual precision not as expected for trajectory 5"
+        "Prior over residual precision not as expected for trajectory 1"
 
     #---------------------------------------------------------------------------
     # Evaluate prior for trajectory 3
     #---------------------------------------------------------------------------
     intercept_co = 6
     age_co = -2
     resid_std = 1
@@ -170,15 +169,15 @@
     preds = ['intercept', 'age']
     pg = PriorGenerator(targets, preds)
     pg.set_model(mm)
 
     for tt in np.where(mm.sig_trajs_)[0]:
         pg.traj_prior_info_from_model('y', tt)
 
-    for tt in [3, 5]:
+    for tt in [1, 3]:
         assert pg.prior_info_['w_mu']['intercept']['y'][tt] == \
             mm.w_mu_[0, 0, tt], \
             "Intercept prior not as expected for trajectory 1"
         assert pg.prior_info_['w_mu']['age']['y'][tt] == mm.w_mu_[1, 0, tt], \
             "Age prior not as expected for trajectory 1"
         assert pg.prior_info_['lambda_a']['y'][tt] == mm.lambda_a_[0, tt], \
             "Gamma prior not as expected for trajectory 1"
@@ -243,28 +242,28 @@
     targets = ['y']
     preds = ['intercept', 'age']
     pg = PriorGenerator(targets, preds)
     pg.set_model(mm)    
     pg.set_data(df, 'id')
     pg.compute_prior_info()
 
-    assert np.isclose(pg.prior_info_['w_mu0']['y']['intercept'], 7.810441593), \
+    assert np.isclose(pg.prior_info_['w_mu0']['y']['intercept'], 7.733268667), \
         "w_mu0 not as expected"
-    assert np.isclose(pg.prior_info_['w_mu0']['y']['age'], -1.48068743758711), \
+    assert np.isclose(pg.prior_info_['w_mu0']['y']['age'], -1.473910420702446), \
         "w_mu0 not as expected"
-    assert np.isclose(pg.prior_info_['w_var0']['y']['intercept'], 0.51800801), \
+    assert np.isclose(pg.prior_info_['w_var0']['y']['intercept'], 0.46760358415383946), \
         "w_var0 not as expected"    
-    assert np.isclose(pg.prior_info_['w_var0']['y']['age'], 0.04260915525159), \
+    assert np.isclose(pg.prior_info_['w_var0']['y']['age'], 0.043930269660685), \
         "w_var0 not as expected"
-    assert np.isclose(pg.prior_info_['lambda_a0']['y'], 207.87669370617036), \
+    assert np.isclose(pg.prior_info_['lambda_a0']['y'], 17.70686866876), \
         "lambda_a0 not as expected"
-    assert np.isclose(pg.prior_info_['lambda_b0']['y'], 67.86146951205156), \
+    assert np.isclose(pg.prior_info_['lambda_b0']['y'], 24.0246304888103), \
         "lambda_b0 not as expected"
 
-    for tt in [3, 5]:
+    for tt in [1, 3]:
         assert pg.prior_info_['w_mu']['intercept']['y'][tt] == \
             mm.w_mu_[0, 0, tt], \
             "Intercept prior not as expected for trajectory 1"
         assert pg.prior_info_['w_mu']['age']['y'][tt] == mm.w_mu_[1, 0, tt], \
             "Age prior not as expected for trajectory 1"
         assert pg.prior_info_['lambda_a']['y'][tt] == mm.lambda_a_[0, tt], \
             "Gamma prior not as expected for trajectory 1"
@@ -286,28 +285,28 @@
     targets = ['y']
     preds = ['intercept', 'age']
     pg = PriorGenerator(targets, preds)
     pg.set_model(mm)
     pg.set_data(df, 'id')
     pg.compute_prior_info()
 
-    assert np.isclose(pg.prior_info_['w_mu0']['y']['intercept'], 7.810441593), \
+    assert np.isclose(pg.prior_info_['w_mu0']['y']['intercept'], 7.733268667), \
         "w_mu0 not as expected"
-    assert np.isclose(pg.prior_info_['w_mu0']['y']['age'], -1.48068743758711), \
+    assert np.isclose(pg.prior_info_['w_mu0']['y']['age'], -1.473910420702446), \
         "w_mu0 not as expected"
-    assert np.isclose(pg.prior_info_['w_var0']['y']['intercept'], 0.51800801), \
+    assert np.isclose(pg.prior_info_['w_var0']['y']['intercept'], 0.46760358415383946), \
         "w_var0 not as expected"    
-    assert np.isclose(pg.prior_info_['w_var0']['y']['age'], 0.04260915525159), \
+    assert np.isclose(pg.prior_info_['w_var0']['y']['age'], 0.043930269660685), \
         "w_var0 not as expected"
-    assert np.isclose(pg.prior_info_['lambda_a0']['y'], 207.87669370617036), \
+    assert np.isclose(pg.prior_info_['lambda_a0']['y'], 17.70686866876), \
         "lambda_a0 not as expected"
-    assert np.isclose(pg.prior_info_['lambda_b0']['y'], 67.86146951205156), \
+    assert np.isclose(pg.prior_info_['lambda_b0']['y'], 24.0246304888103), \
         "lambda_b0 not as expected"
 
-    for tt in [3, 5]:
+    for tt in [1, 3]:
         assert pg.prior_info_['w_mu']['intercept']['y'][tt] == \
             mm.w_mu_[0, 0, tt], \
             "Intercept prior not as expected for trajectory 1"
         assert pg.prior_info_['w_mu']['age']['y'][tt] == mm.w_mu_[1, 0, tt], \
             "Age prior not as expected for trajectory 1"
         assert pg.prior_info_['lambda_a']['y'][tt] == mm.lambda_a_[0, tt], \
             "Gamma prior not as expected for trajectory 1"
@@ -330,28 +329,28 @@
     targets = ['y', 'y2']
     preds = ['intercept', 'age']
     pg = PriorGenerator(targets, preds)
     pg.set_model(mm)
     pg.set_data(df, 'id')
     pg.compute_prior_info()
 
-    assert np.isclose(pg.prior_info_['w_mu0']['y']['intercept'], 7.810441593), \
+    assert np.isclose(pg.prior_info_['w_mu0']['y']['intercept'], 7.733268667), \
         "w_mu0 not as expected"
-    assert np.isclose(pg.prior_info_['w_mu0']['y']['age'], -1.48068743758711), \
+    assert np.isclose(pg.prior_info_['w_mu0']['y']['age'], -1.473910420702446), \
         "w_mu0 not as expected"
-    assert np.isclose(pg.prior_info_['w_var0']['y']['intercept'], 0.51800801), \
+    assert np.isclose(pg.prior_info_['w_var0']['y']['intercept'], 0.46760358415383946), \
         "w_var0 not as expected"    
-    assert np.isclose(pg.prior_info_['w_var0']['y']['age'], 0.04260915525159), \
+    assert np.isclose(pg.prior_info_['w_var0']['y']['age'], 0.043930269660685), \
         "w_var0 not as expected"
-    assert np.isclose(pg.prior_info_['lambda_a0']['y'], 207.87669370617036), \
+    assert np.isclose(pg.prior_info_['lambda_a0']['y'], 17.70686866876), \
         "lambda_a0 not as expected"
-    assert np.isclose(pg.prior_info_['lambda_b0']['y'], 67.86146951205156), \
+    assert np.isclose(pg.prior_info_['lambda_b0']['y'], 24.0246304888103), \
         "lambda_b0 not as expected"
 
-    for tt in [3, 5]:
+    for tt in [1, 3]:
         assert pg.prior_info_['w_mu']['intercept']['y'][tt] == \
             mm.w_mu_[0, 0, tt], \
             "Intercept prior not as expected for trajectory 1"
         assert pg.prior_info_['w_mu']['age']['y'][tt] == mm.w_mu_[1, 0, tt], \
             "Age prior not as expected for trajectory 1"
         assert pg.prior_info_['lambda_a']['y'][tt] == mm.lambda_a_[0, tt], \
             "Gamma prior not as expected for trajectory 1"
@@ -367,28 +366,28 @@
     assert np.isclose(pg.prior_info_['w_mu0']['y2']['age'], -1.3658064249792), \
         "w_mu0 not as expected"
     assert np.isclose(pg.prior_info_['lambda_a0']['y2'], 14.399999999999999), \
         "lambda_a0 not as expected"
     assert np.isclose(pg.prior_info_['lambda_b0']['y2'], 356.5218504085522), \
         "lambda_b0 nost as expected"
 
-    for tt in [3, 5]:
+    for tt in [1, 3]:
         assert np.isclose(mm.w_mu_[0, 0, tt] + 10, \
-            pg.prior_info_['w_mu']['intercept']['y2'][tt], atol=0.05), \
+            pg.prior_info_['w_mu']['intercept']['y2'][tt], atol=0.2), \
             "Intercept prior not as expected"
         assert np.isclose(pg.prior_info_['w_mu']['age']['y2'][tt],  \
-            mm.w_mu_[1, 0, tt], atol=0.01), \
+            mm.w_mu_[1, 0, tt], atol=0.02), \
             "Age prior not as expected"
 
     assert np.isclose(np.sqrt(pg.prior_info_['lambda_b']['y2'][3]/\
         pg.prior_info_['lambda_a']['y2'][3]), 1, atol=0.001), \
         "Gamma prior not as expected for trajectory 3"
-    assert np.isclose(np.sqrt(pg.prior_info_['lambda_b']['y2'][5]/\
-        pg.prior_info_['lambda_a']['y2'][5]), 2, atol=0.03), \
-        "Gamma prior not as expected for trajectory 5"
+    assert np.isclose(np.sqrt(pg.prior_info_['lambda_b']['y2'][1]/\
+        pg.prior_info_['lambda_a']['y2'][1]), 2, atol=0.03), \
+        "Gamma prior not as expected for trajectory 1"
     
 def test_compute_prior_info_5():
     """Model and data, different preds, new target
     """
     model_file_name = os.path.split(os.path.realpath(__file__))[0] + \
         '/../resources/models/model_1.p'
     data_file_name = os.path.split(os.path.realpath(__file__))[0] + \
@@ -405,15 +404,14 @@
     pg.set_model(mm)
     pg.set_data(df, 'id')
     pg.compute_prior_info()
 
     # The following values are from a prior that -- upon visual inspection of
     # random draws -- appears reasonable. This test, then, should be considered
     # a regression test as opposed to a test of "correct" values
-    
     prior_info_gt = \
         {'w_mu0': {'y': {'intercept': 8.102185344934247,
                          'age': -1.7021817743184755,
                          'age^2': 0.018416334689522876},
                    'y2': {'intercept': 18.10218534493426,
                           'age': -1.7021817743184746,
                           'age^2': 0.01841633468952318}},
@@ -438,15 +436,16 @@
                    'age^2': {'y': np.array([9.82818683e-06, 5.18071486e-05]),
                              'y2': np.array([9.82818683e-06, 5.18071486e-05])}},
          'lambda_a': {'y': np.array([203.50423622, 11.95284849]),
                       'y2': np.array([203.50423622, 11.95284849])},
          'lambda_b': {'y': np.array([201.74450982, 48.8934525]),
                       'y2': np.array([201.74450982, 48.8934525])},
          'v_a': np.array([51., 51.]),
-         'v_b': np.array([50.74102343, 0.74102343]),
+         #'v_b': np.array([50.74102343, 0.74102343]),
+         'v_b': np.array([0.74102343, 50.74102343]),         
          'traj_probs': np.array([0.5, 0.5]),
          'alpha': 0.5}
 
     assert pg.prior_info_['w_mu0']['y']['intercept'] == \
         prior_info_gt['w_mu0']['y']['intercept'], "Error in prior"
     assert pg.prior_info_['w_mu0']['y']['age'] == \
         prior_info_gt['w_mu0']['y']['age'], "Error in prior"
@@ -509,55 +508,56 @@
         prior_info_gt['lambda_a']['y2'][0]), "Error in prior"
     assert np.isclose(pg.prior_info_['lambda_b']['y'][3], \
         prior_info_gt['lambda_b']['y'][0]), "Error in prior"
     assert np.isclose(pg.prior_info_['lambda_b']['y2'][3], \
         prior_info_gt['lambda_b']['y2'][0]), "Error in prior"
     assert np.isclose(pg.prior_info_['v_a'][3], \
         prior_info_gt['v_a'][0]), "Error in prior"
+
     assert np.isclose(pg.prior_info_['v_b'][3], \
         prior_info_gt['v_b'][0]), "Error in prior"
     assert np.isclose(pg.prior_info_['traj_probs'][3], \
         prior_info_gt['traj_probs'][0]), "Error in prior"
 
-    assert np.isclose(pg.prior_info_['w_mu']['intercept']['y'][5], \
+    assert np.isclose(pg.prior_info_['w_mu']['intercept']['y'][1], \
         prior_info_gt['w_mu']['intercept']['y'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['w_mu']['intercept']['y2'][5], \
+    assert np.isclose(pg.prior_info_['w_mu']['intercept']['y2'][1], \
         prior_info_gt['w_mu']['intercept']['y2'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['w_mu']['age']['y'][5], \
+    assert np.isclose(pg.prior_info_['w_mu']['age']['y'][1], \
         prior_info_gt['w_mu']['age']['y'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['w_mu']['age']['y2'][5], \
+    assert np.isclose(pg.prior_info_['w_mu']['age']['y2'][1], \
         prior_info_gt['w_mu']['age']['y2'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['w_mu']['age^2']['y'][5], \
+    assert np.isclose(pg.prior_info_['w_mu']['age^2']['y'][1], \
         prior_info_gt['w_mu']['age^2']['y'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['w_mu']['age^2']['y2'][5], \
+    assert np.isclose(pg.prior_info_['w_mu']['age^2']['y2'][1], \
         prior_info_gt['w_mu']['age^2']['y2'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['w_var']['intercept']['y'][5], \
+    assert np.isclose(pg.prior_info_['w_var']['intercept']['y'][1], \
         prior_info_gt['w_var']['intercept']['y'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['w_var']['intercept']['y2'][5], \
+    assert np.isclose(pg.prior_info_['w_var']['intercept']['y2'][1], \
         prior_info_gt['w_var']['intercept']['y2'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['w_var']['age']['y'][5], \
+    assert np.isclose(pg.prior_info_['w_var']['age']['y'][1], \
         prior_info_gt['w_var']['age']['y'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['w_var']['age']['y2'][5], \
+    assert np.isclose(pg.prior_info_['w_var']['age']['y2'][1], \
         prior_info_gt['w_var']['age']['y2'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['w_var']['age^2']['y'][5], \
+    assert np.isclose(pg.prior_info_['w_var']['age^2']['y'][1], \
         prior_info_gt['w_var']['age^2']['y'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['w_var']['age^2']['y2'][5], \
+    assert np.isclose(pg.prior_info_['w_var']['age^2']['y2'][1], \
         prior_info_gt['w_var']['age^2']['y2'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['lambda_a']['y'][5], \
+    assert np.isclose(pg.prior_info_['lambda_a']['y'][1], \
         prior_info_gt['lambda_a']['y'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['lambda_a']['y2'][5], \
+    assert np.isclose(pg.prior_info_['lambda_a']['y2'][1], \
         prior_info_gt['lambda_a']['y2'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['lambda_b']['y'][5], \
+    assert np.isclose(pg.prior_info_['lambda_b']['y'][1], \
         prior_info_gt['lambda_b']['y'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['lambda_b']['y2'][5], \
+    assert np.isclose(pg.prior_info_['lambda_b']['y2'][1], \
         prior_info_gt['lambda_b']['y2'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['v_a'][5], \
+    assert np.isclose(pg.prior_info_['v_a'][1], \
         prior_info_gt['v_a'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['v_b'][5], \
+    assert np.isclose(pg.prior_info_['v_b'][1], \
         prior_info_gt['v_b'][1]), "Error in prior"
-    assert np.isclose(pg.prior_info_['traj_probs'][5], \
+    assert np.isclose(pg.prior_info_['traj_probs'][1], \
         prior_info_gt['traj_probs'][1]), "Error in prior"
     
     assert pg.prior_info_['alpha'] == prior_info_gt['alpha'], "Error in prior"
```

### Comparing `bayes_traj-0.2.5/bayes_traj/tests/test_mult_dp_regression.py` & `bayes_traj-0.2.6/bayes_traj/tests/test_mult_dp_regression.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/tests/test_utils.py` & `bayes_traj-0.2.6/bayes_traj/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/update_model.py` & `bayes_traj-0.2.6/bayes_traj/update_model.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/utils.py` & `bayes_traj-0.2.6/bayes_traj/utils.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/viz_data_prior_draws.py` & `bayes_traj-0.2.6/bayes_traj/viz_data_prior_draws.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/viz_gamma_dists.py` & `bayes_traj-0.2.6/bayes_traj/viz_gamma_dists.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj/viz_model_trajs.py` & `bayes_traj-0.2.6/bayes_traj/viz_model_trajs.py`

 * *Files identical despite different names*

### Comparing `bayes_traj-0.2.5/bayes_traj.egg-info/PKG-INFO` & `bayes_traj-0.2.6/bayes_traj.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayes-traj
-Version: 0.2.5
+Version: 0.2.6
 Summary: bayes_traj
 Home-page: https://github.com/acil-bwh/bayes_traj
 Author: James Ross
 Author-email: jross@bwh.harvard.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `bayes_traj-0.2.5/bayes_traj.egg-info/SOURCES.txt` & `bayes_traj-0.2.6/bayes_traj.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.md
+setup.cfg
 setup.py
 bayes_traj/__init__.py
 bayes_traj/assign_trajectory.py
 bayes_traj/bayes_traj_main.py
 bayes_traj/bayes_traj_main_alpha.py
 bayes_traj/bayes_traj_refiner.py
 bayes_traj/fit_stats.py
@@ -10,14 +11,15 @@
 bayes_traj/generate_prior.py
 bayes_traj/get_constraints_graph.py
 bayes_traj/get_longitudinal_constraints_graph.py
 bayes_traj/mult_dp_regression.py
 bayes_traj/mult_pyro.py
 bayes_traj/prior_from_model.py
 bayes_traj/psis.py
+bayes_traj/pyro_helper.py
 bayes_traj/summarize_traj_model.py
 bayes_traj/update_model.py
 bayes_traj/utils.py
 bayes_traj/viz_data_prior_draws.py
 bayes_traj/viz_gamma_dists.py
 bayes_traj/viz_model_trajs.py
 bayes_traj.egg-info/PKG-INFO
```

### Comparing `bayes_traj-0.2.5/setup.py` & `bayes_traj-0.2.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #                                  'bin/*'])
 
 packages = find_packages()
 packages.append('bayes_traj')
 
 setup(
     name='bayes_traj',
-    version='0.2.5',
+    version='0.2.6',
     description='bayes_traj',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/acil-bwh/bayes_traj',
     author='James Ross',
     author_email='jross@bwh.harvard.edu',
 
@@ -42,23 +42,25 @@
                                         'summarize_traj_model = bayes_traj.summarize_traj_model:main',
                                         'assign_trajectory = bayes_traj.assign_trajectory:main',
                                         'update_model = bayes_traj.update_model:main',                                        
                                         'generate_prior = bayes_traj.generate_prior:main']},
     
     install_requires=[
         'provenance-tools >= 0.0.5',
-        'pandas < 2.0.0',
-        'numpy >= 1.19.1',
+        'pandas < 2.2.2',
+        'numpy >= 1.26.4',
         'matplotlib >= 3.3.1',
         'scipy >= 1.5.2',
         'argparse >= 1.1',
         'statsmodels >= 0.11.1',
         'torch >= 2.0.1',
         'pyro-ppl >= 1.8.5',
         'pytest >= 7.0.0',
+        'numexpr >= 2.10.0',
+        'bottleneck >= 1.3.8',        
     ],
     
     
     ### Other stuff ...
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

