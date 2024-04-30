# Comparing `tmp/depp_test-0.3.8.tar.gz` & `tmp/depp_test-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depp_test-0.3.8.tar", last modified: Tue Jan  9 17:10:59 2024, max compression
+gzip compressed data, was "depp_test-0.3.9.tar", last modified: Tue Jan  9 21:06:08 2024, max compression
```

## Comparing `depp_test-0.3.8.tar` & `depp_test-0.3.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2024-01-09 17:10:59.968822 depp_test-0.3.8/
--rw-r--r--   0 yueyu      (501) staff       (20)     1067 2022-03-31 05:54:54.000000 depp_test-0.3.8/LICENSE
--rw-r--r--   0 yueyu      (501) staff       (20)      449 2024-01-09 17:10:59.968662 depp_test-0.3.8/PKG-INFO
--rw-r--r--   0 yueyu      (501) staff       (20)     9392 2022-08-16 00:49:49.000000 depp_test-0.3.8/README.md
--rw-r--r--   0 yueyu      (501) staff       (20)     1941 2023-04-27 23:37:10.000000 depp_test-0.3.8/agg_dist.py
--rw-r--r--   0 yueyu      (501) staff       (20)      577 2023-04-27 23:37:10.000000 depp_test-0.3.8/comb_json.py
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2024-01-09 17:10:59.966758 depp_test-0.3.8/depp/
--rw-r--r--   0 yueyu      (501) staff       (20)     5765 2024-01-04 18:06:29.000000 depp_test-0.3.8/depp/Agg_model.py
--rw-r--r--   0 yueyu      (501) staff       (20)     4909 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/Agg_model_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5935 2022-03-31 06:34:25.000000 depp_test-0.3.8/depp/Model_new.py
--rw-r--r--   0 yueyu      (501) staff       (20)     8681 2024-01-04 18:00:11.000000 depp_test-0.3.8/depp/Model_pl.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5542 2022-03-31 06:34:25.000000 depp_test-0.3.8/depp/Model_pl.split.py
--rw-r--r--   0 yueyu      (501) staff       (20)    11301 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/Model_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)        0 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/__init__.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1605 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/assign_cluster_by_placement.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5019 2023-11-29 20:58:50.000000 depp_test-0.3.8/depp/combine_similar_seq.py
--rw-r--r--   0 yueyu      (501) staff       (20)      526 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/count_gapped_ratio.py
--rw-r--r--   0 yueyu      (501) staff       (20)    12673 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/data.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2431 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/data.split.py
--rw-r--r--   0 yueyu      (501) staff       (20)     4009 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/data_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1730 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/default_config.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2433 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/depp_distance.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2063 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/depp_distance_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1645 2022-03-31 06:34:25.000000 depp_test-0.3.8/depp/distance_correction.py
--rw-r--r--   0 yueyu      (501) staff       (20)      766 2023-04-27 23:36:52.000000 depp_test-0.3.8/depp/filter_by_entropy_gap.sh
--rw-r--r--   0 yueyu      (501) staff       (20)      782 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/get_names_by_entropy_gap.py
--rw-r--r--   0 yueyu      (501) staff       (20)      873 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/get_tree_dist.py
--rw-r--r--   0 yueyu      (501) staff       (20)      576 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/grep_jplace.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1008 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/grep_seq.py
--rw-r--r--   0 yueyu      (501) staff       (20)      909 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/grep_seq_group.py
--rw-r--r--   0 yueyu      (501) staff       (20)      743 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/select_placement.py
--rw-------   0 yueyu      (501) staff       (20)      895 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/select_species_by_distance.py
--rw-r--r--   0 yueyu      (501) staff       (20)      366 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/set_bl_one.py
--rw-r--r--   0 yueyu      (501) staff       (20)     7731 2023-04-27 23:36:57.000000 depp_test-0.3.8/depp/submodule.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1578 2023-11-03 19:56:54.000000 depp_test-0.3.8/depp/test_scripts.py
--rw-r--r--   0 yueyu      (501) staff       (20)    37938 2024-01-04 18:03:17.000000 depp_test-0.3.8/depp/utils.py
--rw-r--r--   0 yueyu      (501) staff       (20)     4245 2023-11-29 00:27:08.000000 depp_test-0.3.8/depp-place-rRNA-one-type.sh
--rw-r--r--   0 yueyu      (501) staff       (20)     6663 2024-01-09 17:10:17.000000 depp_test-0.3.8/depp-place-rRNA.sh
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2024-01-09 17:10:59.968467 depp_test-0.3.8/depp_test.egg-info/
--rw-r--r--   0 yueyu      (501) staff       (20)      449 2024-01-09 17:10:59.000000 depp_test-0.3.8/depp_test.egg-info/PKG-INFO
--rw-r--r--   0 yueyu      (501) staff       (20)     1060 2024-01-09 17:10:59.000000 depp_test-0.3.8/depp_test.egg-info/SOURCES.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        1 2024-01-09 17:10:59.000000 depp_test-0.3.8/depp_test.egg-info/dependency_links.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        1 2022-03-31 15:15:32.000000 depp_test-0.3.8/depp_test.egg-info/not-zip-safe
--rw-r--r--   0 yueyu      (501) staff       (20)      155 2024-01-09 17:10:59.000000 depp_test-0.3.8/depp_test.egg-info/requires.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        5 2024-01-09 17:10:59.000000 depp_test-0.3.8/depp_test.egg-info/top_level.txt
--rw-r--r--   0 yueyu      (501) staff       (20)     1149 2023-04-27 23:37:10.000000 depp_test-0.3.8/merge_json.py
--rwxr-xr-x   0 yueyu      (501) staff       (20)      912 2023-04-27 23:37:14.000000 depp_test-0.3.8/run_upp.sh
--rw-r--r--   0 yueyu      (501) staff       (20)     2339 2023-04-27 23:37:10.000000 depp_test-0.3.8/seq_sep.py
--rw-r--r--   0 yueyu      (501) staff       (20)       38 2024-01-09 17:10:59.968869 depp_test-0.3.8/setup.cfg
--rw-r--r--   0 yueyu      (501) staff       (20)     2009 2024-01-09 17:10:31.000000 depp_test-0.3.8/setup.py
--rw-r--r--   0 yueyu      (501) staff       (20)     6976 2023-11-06 06:04:49.000000 depp_test-0.3.8/train_cluster_depp.sh
--rw-r--r--   0 yueyu      (501) staff       (20)     4773 2023-04-27 23:37:10.000000 depp_test-0.3.8/train_depp.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5033 2023-04-27 23:37:10.000000 depp_test-0.3.8/train_depp_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5173 2023-04-27 23:37:14.000000 depp_test-0.3.8/wol_placement.sh
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2024-01-09 21:06:08.100739 depp_test-0.3.9/
+-rw-r--r--   0 yueyu      (501) staff       (20)     1067 2022-03-31 05:54:54.000000 depp_test-0.3.9/LICENSE
+-rw-r--r--   0 yueyu      (501) staff       (20)      449 2024-01-09 21:06:08.100490 depp_test-0.3.9/PKG-INFO
+-rw-r--r--   0 yueyu      (501) staff       (20)     9392 2022-08-16 00:49:49.000000 depp_test-0.3.9/README.md
+-rw-r--r--   0 yueyu      (501) staff       (20)     1941 2023-04-27 23:37:10.000000 depp_test-0.3.9/agg_dist.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      577 2023-04-27 23:37:10.000000 depp_test-0.3.9/comb_json.py
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2024-01-09 21:06:08.098698 depp_test-0.3.9/depp/
+-rw-r--r--   0 yueyu      (501) staff       (20)     5765 2024-01-04 18:06:29.000000 depp_test-0.3.9/depp/Agg_model.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     4909 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/Agg_model_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5935 2022-03-31 06:34:25.000000 depp_test-0.3.9/depp/Model_new.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     8681 2024-01-04 18:00:11.000000 depp_test-0.3.9/depp/Model_pl.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5542 2022-03-31 06:34:25.000000 depp_test-0.3.9/depp/Model_pl.split.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    11301 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/Model_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)        0 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/__init__.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1605 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/assign_cluster_by_placement.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5019 2023-11-29 20:58:50.000000 depp_test-0.3.9/depp/combine_similar_seq.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      526 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/count_gapped_ratio.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    12673 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/data.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2431 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/data.split.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     4009 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/data_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1730 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/default_config.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2433 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/depp_distance.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2063 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/depp_distance_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1645 2022-03-31 06:34:25.000000 depp_test-0.3.9/depp/distance_correction.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      766 2023-04-27 23:36:52.000000 depp_test-0.3.9/depp/filter_by_entropy_gap.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)      782 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/get_names_by_entropy_gap.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      873 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/get_tree_dist.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      576 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/grep_jplace.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1008 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/grep_seq.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      909 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/grep_seq_group.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      743 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/select_placement.py
+-rw-------   0 yueyu      (501) staff       (20)      895 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/select_species_by_distance.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      366 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/set_bl_one.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     7731 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/submodule.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1578 2023-11-03 19:56:54.000000 depp_test-0.3.9/depp/test_scripts.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    37938 2024-01-04 18:03:17.000000 depp_test-0.3.9/depp/utils.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     4245 2023-11-29 00:27:08.000000 depp_test-0.3.9/depp-place-rRNA-one-type.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     6648 2024-01-09 21:05:22.000000 depp_test-0.3.9/depp-place-rRNA.sh
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2024-01-09 21:06:08.099827 depp_test-0.3.9/depp_test.egg-info/
+-rw-r--r--   0 yueyu      (501) staff       (20)      449 2024-01-09 21:06:07.000000 depp_test-0.3.9/depp_test.egg-info/PKG-INFO
+-rw-r--r--   0 yueyu      (501) staff       (20)     1060 2024-01-09 21:06:08.000000 depp_test-0.3.9/depp_test.egg-info/SOURCES.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        1 2024-01-09 21:06:07.000000 depp_test-0.3.9/depp_test.egg-info/dependency_links.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        1 2022-03-31 15:15:32.000000 depp_test-0.3.9/depp_test.egg-info/not-zip-safe
+-rw-r--r--   0 yueyu      (501) staff       (20)      155 2024-01-09 21:06:07.000000 depp_test-0.3.9/depp_test.egg-info/requires.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        5 2024-01-09 21:06:07.000000 depp_test-0.3.9/depp_test.egg-info/top_level.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)     1149 2023-04-27 23:37:10.000000 depp_test-0.3.9/merge_json.py
+-rwxr-xr-x   0 yueyu      (501) staff       (20)      912 2023-04-27 23:37:14.000000 depp_test-0.3.9/run_upp.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     2339 2023-04-27 23:37:10.000000 depp_test-0.3.9/seq_sep.py
+-rw-r--r--   0 yueyu      (501) staff       (20)       38 2024-01-09 21:06:08.100801 depp_test-0.3.9/setup.cfg
+-rw-r--r--   0 yueyu      (501) staff       (20)     2009 2024-01-09 21:05:48.000000 depp_test-0.3.9/setup.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     6976 2023-11-06 06:04:49.000000 depp_test-0.3.9/train_cluster_depp.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     4773 2023-04-27 23:37:10.000000 depp_test-0.3.9/train_depp.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5033 2023-04-27 23:37:10.000000 depp_test-0.3.9/train_depp_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5173 2023-04-27 23:37:14.000000 depp_test-0.3.9/wol_placement.sh
```

### Comparing `depp_test-0.3.8/LICENSE` & `depp_test-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/README.md` & `depp_test-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/agg_dist.py` & `depp_test-0.3.9/agg_dist.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/comb_json.py` & `depp_test-0.3.9/comb_json.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/Agg_model.py` & `depp_test-0.3.9/depp/Agg_model.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/Agg_model_recon.py` & `depp_test-0.3.9/depp/Agg_model_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/Model_new.py` & `depp_test-0.3.9/depp/Model_new.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/Model_pl.py` & `depp_test-0.3.9/depp/Model_pl.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/Model_pl.split.py` & `depp_test-0.3.9/depp/Model_pl.split.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/Model_recon.py` & `depp_test-0.3.9/depp/Model_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/assign_cluster_by_placement.py` & `depp_test-0.3.9/depp/assign_cluster_by_placement.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/combine_similar_seq.py` & `depp_test-0.3.9/depp/combine_similar_seq.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/count_gapped_ratio.py` & `depp_test-0.3.9/depp/count_gapped_ratio.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/data.py` & `depp_test-0.3.9/depp/data.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/data.split.py` & `depp_test-0.3.9/depp/data.split.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/data_recon.py` & `depp_test-0.3.9/depp/data_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/default_config.py` & `depp_test-0.3.9/depp/default_config.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/depp_distance.py` & `depp_test-0.3.9/depp/depp_distance.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/depp_distance_recon.py` & `depp_test-0.3.9/depp/depp_distance_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/distance_correction.py` & `depp_test-0.3.9/depp/distance_correction.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/filter_by_entropy_gap.sh` & `depp_test-0.3.9/depp/filter_by_entropy_gap.sh`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/get_names_by_entropy_gap.py` & `depp_test-0.3.9/depp/get_names_by_entropy_gap.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/get_tree_dist.py` & `depp_test-0.3.9/depp/get_tree_dist.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/grep_jplace.py` & `depp_test-0.3.9/depp/grep_jplace.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/grep_seq.py` & `depp_test-0.3.9/depp/grep_seq.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/grep_seq_group.py` & `depp_test-0.3.9/depp/grep_seq_group.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/select_placement.py` & `depp_test-0.3.9/depp/select_placement.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/select_species_by_distance.py` & `depp_test-0.3.9/depp/select_species_by_distance.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/submodule.py` & `depp_test-0.3.9/depp/submodule.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/test_scripts.py` & `depp_test-0.3.9/depp/test_scripts.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp/utils.py` & `depp_test-0.3.9/depp/utils.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp-place-rRNA-one-type.sh` & `depp_test-0.3.9/depp-place-rRNA-one-type.sh`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/depp-place-rRNA.sh` & `depp_test-0.3.9/depp-place-rRNA.sh`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     # align sequences
     echo "aligning the sequences..."
 
     # split query sequences into multiple files (/tmp directory)
     for i in ${tmpdir}/query_seq/*.fa;
     do
-      upptmpdir=`mktemp -d -t 'upp-tmp-XXXXXXXXXX'`
+      upptmpdir=`mktemp -d -t 'upp'`
       # check if the directory is created
       if [[ ! "$tmpdir" || ! -d "$tmpdir" ]]; then
         echo "Could not create temp dir"
         exit 1
       fi
       j="${i##*/}"
       dt="${j%.*}"
```

### Comparing `depp_test-0.3.8/depp_test.egg-info/SOURCES.txt` & `depp_test-0.3.9/depp_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/merge_json.py` & `depp_test-0.3.9/merge_json.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/run_upp.sh` & `depp_test-0.3.9/run_upp.sh`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/seq_sep.py` & `depp_test-0.3.9/seq_sep.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/setup.py` & `depp_test-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
 	name='depp_test',    # This is the name of your PyPI-package.
-        version='0.3.8',    # Update the version number for new releases
+        version='0.3.9',    # Update the version number for new releases
         scripts=['train_depp.py',
                  'depp/depp_distance.py',
                  'agg_dist.py',
                  'wol_placement.sh',
                  'run_upp.sh',
                  'merge_json.py',
                  'train_depp_recon.py',
```

### Comparing `depp_test-0.3.8/train_cluster_depp.sh` & `depp_test-0.3.9/train_cluster_depp.sh`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/train_depp.py` & `depp_test-0.3.9/train_depp.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/train_depp_recon.py` & `depp_test-0.3.9/train_depp_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.8/wol_placement.sh` & `depp_test-0.3.9/wol_placement.sh`

 * *Files identical despite different names*

