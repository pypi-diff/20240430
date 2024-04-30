# Comparing `tmp/pcpfm-1.0.7.tar.gz` & `tmp/pcpfm-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcpfm-1.0.7.tar", last modified: Fri Feb 23 19:20:20 2024, max compression
+gzip compressed data, was "pcpfm-1.0.9.tar", last modified: Wed Feb 28 19:45:28 2024, max compression
```

## Comparing `pcpfm-1.0.7.tar` & `pcpfm-1.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        0 2024-02-23 19:20:20.854153 pcpfm-1.0.7/
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     1166 2024-02-21 16:47:58.000000 pcpfm-1.0.7/LICENSE
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      295 2024-02-21 16:47:58.000000 pcpfm-1.0.7/MANIFEST.in
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    29296 2024-02-23 19:20:20.853508 pcpfm-1.0.7/PKG-INFO
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    27927 2024-02-21 16:47:58.000000 pcpfm-1.0.7/README.md
-drwxr-xr-x   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        0 2024-02-23 19:20:20.817632 pcpfm-1.0.7/pcpfm/
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    10149 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/Acquisition.py
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    30669 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/EmpCpds.py
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    32713 2024-02-21 21:38:48.000000 pcpfm-1.0.7/pcpfm/Experiment.py
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    75629 2024-02-22 16:08:09.000000 pcpfm-1.0.7/pcpfm/FeatureTable.py
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     5741 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/MSnSpectrum.py
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    18487 2024-02-21 22:19:33.000000 pcpfm-1.0.7/pcpfm/Report.py
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)       22 2024-02-23 19:19:17.000000 pcpfm-1.0.7/pcpfm/__init__.py
-drwxr-xr-x   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        0 2024-02-23 19:20:20.827398 pcpfm-1.0.7/pcpfm/annotation_sources/
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      336 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/annotation_sources/README.md
-drwxr-xr-x   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        0 2024-02-23 19:20:20.852270 pcpfm-1.0.7/pcpfm/default_configs/
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        0 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/default_configs/__init__.py
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     3955 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/default_configs/default.json
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      263 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/default_configs/default_adducts_neg_feature.json
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      123 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/default_configs/default_adducts_neg_khipu.json
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      184 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/default_configs/default_adducts_pos_feature.json
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)       95 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/default_configs/default_adducts_pos_khipu.json
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      145 2024-02-21 17:35:18.000000 pcpfm-1.0.7/pcpfm/default_configs/default_auto_drop.json
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        7 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/default_configs/default_charges.json
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      885 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/default_configs/default_experiment_params.json
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      500 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/default_configs/default_extended_adducts.json
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      118 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/default_configs/default_isotopes.json
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     1505 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/default_configs/default_preprocessing.json
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     2243 2024-02-21 17:04:20.000000 pcpfm-1.0.7/pcpfm/default_configs/default_report.json
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     4085 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/default_parameters.py
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    41672 2024-02-21 21:33:14.000000 pcpfm-1.0.7/pcpfm/main.py
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    12557 2024-02-21 16:47:58.000000 pcpfm-1.0.7/pcpfm/utils.py
-drwxr-xr-x   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        0 2024-02-23 19:20:20.852906 pcpfm-1.0.7/pcpfm.egg-info/
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    29296 2024-02-23 19:20:20.000000 pcpfm-1.0.7/pcpfm.egg-info/PKG-INFO
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     1071 2024-02-23 19:20:20.000000 pcpfm-1.0.7/pcpfm.egg-info/SOURCES.txt
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        1 2024-02-23 19:20:20.000000 pcpfm-1.0.7/pcpfm.egg-info/dependency_links.txt
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)       41 2024-02-23 19:20:20.000000 pcpfm-1.0.7/pcpfm.egg-info/entry_points.txt
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      216 2024-02-23 19:20:20.000000 pcpfm-1.0.7/pcpfm.egg-info/requires.txt
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        6 2024-02-23 19:20:20.000000 pcpfm-1.0.7/pcpfm.egg-info/top_level.txt
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      216 2024-02-21 16:47:58.000000 pcpfm-1.0.7/requirements.txt
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)       38 2024-02-23 19:20:20.854219 pcpfm-1.0.7/setup.cfg
--rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     1388 2024-02-21 16:47:58.000000 pcpfm-1.0.7/setup.py
+drwxr-xr-x   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        0 2024-02-28 19:45:28.285299 pcpfm-1.0.9/
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     1166 2024-02-21 16:47:58.000000 pcpfm-1.0.9/LICENSE
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      295 2024-02-21 16:47:58.000000 pcpfm-1.0.9/MANIFEST.in
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    29296 2024-02-28 19:45:28.284720 pcpfm-1.0.9/PKG-INFO
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    27927 2024-02-21 16:47:58.000000 pcpfm-1.0.9/README.md
+drwxr-xr-x   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        0 2024-02-28 19:45:28.252827 pcpfm-1.0.9/pcpfm/
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    10149 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/Acquisition.py
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    30669 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/EmpCpds.py
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    32713 2024-02-21 21:38:48.000000 pcpfm-1.0.9/pcpfm/Experiment.py
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    75815 2024-02-28 19:35:04.000000 pcpfm-1.0.9/pcpfm/FeatureTable.py
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     5741 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/MSnSpectrum.py
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    18487 2024-02-21 22:19:33.000000 pcpfm-1.0.9/pcpfm/Report.py
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)       22 2024-02-28 19:35:48.000000 pcpfm-1.0.9/pcpfm/__init__.py
+drwxr-xr-x   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        0 2024-02-28 19:45:28.261304 pcpfm-1.0.9/pcpfm/annotation_sources/
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      336 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/annotation_sources/README.md
+drwxr-xr-x   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        0 2024-02-28 19:45:28.283307 pcpfm-1.0.9/pcpfm/default_configs/
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        0 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/default_configs/__init__.py
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     3955 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/default_configs/default.json
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      263 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/default_configs/default_adducts_neg_feature.json
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      123 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/default_configs/default_adducts_neg_khipu.json
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      184 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/default_configs/default_adducts_pos_feature.json
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)       95 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/default_configs/default_adducts_pos_khipu.json
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      145 2024-02-21 17:35:18.000000 pcpfm-1.0.9/pcpfm/default_configs/default_auto_drop.json
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        7 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/default_configs/default_charges.json
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      885 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/default_configs/default_experiment_params.json
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      500 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/default_configs/default_extended_adducts.json
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      118 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/default_configs/default_isotopes.json
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     1505 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/default_configs/default_preprocessing.json
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     2243 2024-02-21 17:04:20.000000 pcpfm-1.0.9/pcpfm/default_configs/default_report.json
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     4085 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/default_parameters.py
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    41672 2024-02-21 21:33:14.000000 pcpfm-1.0.9/pcpfm/main.py
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    12557 2024-02-21 16:47:58.000000 pcpfm-1.0.9/pcpfm/utils.py
+drwxr-xr-x   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        0 2024-02-28 19:45:28.284027 pcpfm-1.0.9/pcpfm.egg-info/
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)    29296 2024-02-28 19:45:28.000000 pcpfm-1.0.9/pcpfm.egg-info/PKG-INFO
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     1071 2024-02-28 19:45:28.000000 pcpfm-1.0.9/pcpfm.egg-info/SOURCES.txt
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        1 2024-02-28 19:45:28.000000 pcpfm-1.0.9/pcpfm.egg-info/dependency_links.txt
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)       41 2024-02-28 19:45:28.000000 pcpfm-1.0.9/pcpfm.egg-info/entry_points.txt
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      216 2024-02-28 19:45:28.000000 pcpfm-1.0.9/pcpfm.egg-info/requires.txt
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)        6 2024-02-28 19:45:28.000000 pcpfm-1.0.9/pcpfm.egg-info/top_level.txt
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)      216 2024-02-21 16:47:58.000000 pcpfm-1.0.9/requirements.txt
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)       38 2024-02-28 19:45:28.285367 pcpfm-1.0.9/setup.cfg
+-rw-r--r--   0 mitchjo  (935526437) JAX\Domain Users (1088672553)     1388 2024-02-21 16:47:58.000000 pcpfm-1.0.9/setup.py
```

### Comparing `pcpfm-1.0.7/LICENSE` & `pcpfm-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/PKG-INFO` & `pcpfm-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcpfm
-Version: 1.0.7
+Version: 1.0.9
 Summary: LC-MS metabolomics data processing pipeline
 Home-page: https://github.com/jmmitc06/PythonCentricPipelineForMetabolomics
 Author: Joshua Mitchell
 Author-email: joshua.mitchell@jax.org
 License: MIT
 Keywords: metabolomics bioinformatics mass spectrometry
 Classifier: Intended Audience :: Developers
```

### Comparing `pcpfm-1.0.7/README.md` & `pcpfm-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/pcpfm/Acquisition.py` & `pcpfm-1.0.9/pcpfm/Acquisition.py`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/pcpfm/EmpCpds.py` & `pcpfm-1.0.9/pcpfm/EmpCpds.py`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/pcpfm/Experiment.py` & `pcpfm-1.0.9/pcpfm/Experiment.py`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/pcpfm/FeatureTable.py` & `pcpfm-1.0.9/pcpfm/FeatureTable.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,18 +214,19 @@
         :return: the feature table for the moniker
         :rtype: FeatureTable
         """
 
         df = pd.read_csv(experiment.feature_tables[moniker], sep="\t")
         mzml_to_name = {}
         for acquisition in experiment.acquisitions:
-            mzml_to_name[os.path.basename(acquisition.mzml_filepath).rstrip('.mzML')] = acquisition.name
-        df.rename(mzml_to_name, inplace=True)
+            if os.path.basename(acquisition.mzml_filepath).rstrip('.mzML') in df.columns:
+                mzml_to_name[os.path.basename(acquisition.mzml_filepath).rstrip('.mzML')] = acquisition.name
+        renamed = df.rename(columns=mzml_to_name)
         return FeatureTable(
-            df,
+            renamed,
             experiment,
             moniker,
         )
 
     def make_nonnegative(self, fill_value=1):
         """
         This replaces all NaN and 0 values in the feature table with the specified fill_value
@@ -1248,16 +1249,18 @@
                     for qaqc_result in result:
                         qcqa_results = self.experiment.qcqa_results[self.moniker]
                         qcqa_results[qaqc_result["Type"]] = qaqc_result
                         self.experiment.qcqa_results[self.moniker][qaqc_result["Type"]] = qaqc_result
                 else:
                     print("No method found for " + field)
             qaqc_results_for_field = self.experiment.qcqa_results[self.moniker].get(field, None)
+            print(qaqc_results_for_field)
             if qaqc_results_for_field:
                 for sample, value in qaqc_results_for_field["Result"].items():
+                    print(sample, value)
                     if not min_value < float(value) < max_value:
                         if qaqc_filter[field]["Action"] == "Keep":
                             pass
                         elif qaqc_filter[field]["Action"] == "Drop":
                             to_drop.append(sample)
             else:
                 print("No qaqc results found for " + field)
```

### Comparing `pcpfm-1.0.7/pcpfm/MSnSpectrum.py` & `pcpfm-1.0.9/pcpfm/MSnSpectrum.py`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/pcpfm/Report.py` & `pcpfm-1.0.9/pcpfm/Report.py`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/pcpfm/default_configs/default.json` & `pcpfm-1.0.9/pcpfm/default_configs/default.json`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/pcpfm/default_configs/default_experiment_params.json` & `pcpfm-1.0.9/pcpfm/default_configs/default_experiment_params.json`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/pcpfm/default_configs/default_preprocessing.json` & `pcpfm-1.0.9/pcpfm/default_configs/default_preprocessing.json`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/pcpfm/default_configs/default_report.json` & `pcpfm-1.0.9/pcpfm/default_configs/default_report.json`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/pcpfm/default_parameters.py` & `pcpfm-1.0.9/pcpfm/default_parameters.py`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/pcpfm/main.py` & `pcpfm-1.0.9/pcpfm/main.py`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/pcpfm/utils.py` & `pcpfm-1.0.9/pcpfm/utils.py`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/pcpfm.egg-info/PKG-INFO` & `pcpfm-1.0.9/pcpfm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcpfm
-Version: 1.0.7
+Version: 1.0.9
 Summary: LC-MS metabolomics data processing pipeline
 Home-page: https://github.com/jmmitc06/PythonCentricPipelineForMetabolomics
 Author: Joshua Mitchell
 Author-email: joshua.mitchell@jax.org
 License: MIT
 Keywords: metabolomics bioinformatics mass spectrometry
 Classifier: Intended Audience :: Developers
```

### Comparing `pcpfm-1.0.7/pcpfm.egg-info/SOURCES.txt` & `pcpfm-1.0.9/pcpfm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcpfm-1.0.7/setup.py` & `pcpfm-1.0.9/setup.py`

 * *Files identical despite different names*

