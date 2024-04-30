# Comparing `tmp/epimodel_sensitivity_test-0.1.6.tar.gz` & `tmp/epimodel_sensitivity_test-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epimodel_sensitivity_test-0.1.6.tar", last modified: Mon Apr 29 08:17:56 2024, max compression
+gzip compressed data, was "epimodel_sensitivity_test-0.1.7.tar", last modified: Tue Apr 30 16:59:44 2024, max compression
```

## Comparing `epimodel_sensitivity_test-0.1.6.tar` & `epimodel_sensitivity_test-0.1.7.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.683814 epimodel_sensitivity_test-0.1.6/
--rw-rw-rw-   0        0        0     2153 2024-04-29 08:17:56.683814 epimodel_sensitivity_test-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1698 2024-04-05 10:47:20.000000 epimodel_sensitivity_test-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.277536 epimodel_sensitivity_test-0.1.6/data/
--rw-rw-rw-   0        0        0     6144 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.6/data/age_distribution.xls
--rw-rw-rw-   0        0        0    26112 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.6/data/contact_matrices.xls
--rw-rw-rw-   0        0        0     3079 2024-04-28 22:03:14.000000 epimodel_sensitivity_test-0.1.6/data/model_parameters.json
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.293163 epimodel_sensitivity_test-0.1.6/epimodel_sensitivity_test.egg-info/
--rw-rw-rw-   0        0        0     2153 2024-04-29 08:17:56.000000 epimodel_sensitivity_test-0.1.6/epimodel_sensitivity_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2423 2024-04-29 08:17:56.000000 epimodel_sensitivity_test-0.1.6/epimodel_sensitivity_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 08:17:56.000000 epimodel_sensitivity_test-0.1.6/epimodel_sensitivity_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-29 08:17:56.000000 epimodel_sensitivity_test-0.1.6/epimodel_sensitivity_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 08:17:56.000000 epimodel_sensitivity_test-0.1.6/epimodel_sensitivity_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.308791 epimodel_sensitivity_test-0.1.6/examples/
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.340041 epimodel_sensitivity_test-0.1.6/examples/SEIHR_2_age_groups/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/examples/SEIHR_2_age_groups/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.355668 epimodel_sensitivity_test-0.1.6/examples/SEIHR_2_age_groups/configs/
--rw-rw-rw-   0        0        0      845 2024-04-28 16:22:42.000000 epimodel_sensitivity_test-0.1.6/examples/SEIHR_2_age_groups/configs/model_struct.json
--rw-rw-rw-   0        0        0      619 2024-04-08 14:26:10.000000 epimodel_sensitivity_test-0.1.6/examples/SEIHR_2_age_groups/configs/sampling_config.json
--rw-rw-rw-   0        0        0      963 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.6/examples/SEIHR_2_age_groups/seihr_2_ag_main.py
--rw-rw-rw-   0        0        0     1694 2024-04-27 18:48:18.000000 epimodel_sensitivity_test-0.1.6/examples/SEIHR_2_age_groups/simulation_seihr.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.402546 epimodel_sensitivity_test-0.1.6/examples/SEIR_no_age_groups/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/examples/SEIR_no_age_groups/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.418173 epimodel_sensitivity_test-0.1.6/examples/SEIR_no_age_groups/configs/
--rw-rw-rw-   0        0        0      548 2024-04-28 12:23:52.000000 epimodel_sensitivity_test-0.1.6/examples/SEIR_no_age_groups/configs/model_struct.json
--rw-rw-rw-   0        0        0      371 2024-04-28 10:08:14.000000 epimodel_sensitivity_test-0.1.6/examples/SEIR_no_age_groups/configs/sampling_config.json
--rw-rw-rw-   0        0        0      344 2024-04-12 11:39:01.000000 epimodel_sensitivity_test-0.1.6/examples/SEIR_no_age_groups/model_seir.py
--rw-rw-rw-   0        0        0      332 2024-04-08 13:30:52.000000 epimodel_sensitivity_test-0.1.6/examples/SEIR_no_age_groups/sampler_seir.py
--rw-rw-rw-   0        0        0      714 2024-04-28 22:01:07.000000 epimodel_sensitivity_test-0.1.6/examples/SEIR_no_age_groups/seir_no_ag_main.py
--rw-rw-rw-   0        0        0     1542 2024-04-12 10:17:04.000000 epimodel_sensitivity_test-0.1.6/examples/SEIR_no_age_groups/simulation_seir.py
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.449422 epimodel_sensitivity_test-0.1.6/examples/contact_sensitivity/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/examples/contact_sensitivity/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.465049 epimodel_sensitivity_test-0.1.6/examples/contact_sensitivity/configs/
--rw-rw-rw-   0        0        0     1966 2024-04-28 12:45:38.000000 epimodel_sensitivity_test-0.1.6/examples/contact_sensitivity/configs/model_struct.json
--rw-rw-rw-   0        0        0      428 2024-04-05 22:30:36.000000 epimodel_sensitivity_test-0.1.6/examples/contact_sensitivity/configs/sampling_config.json
--rw-rw-rw-   0        0        0      406 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/examples/contact_sensitivity/contact_main.py
--rw-rw-rw-   0        0        0      572 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.6/examples/contact_sensitivity/sampler_contact.py
--rw-rw-rw-   0        0        0     3148 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.6/examples/contact_sensitivity/sensitivity_model_contact.py
--rw-rw-rw-   0        0        0     3820 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.6/examples/contact_sensitivity/simulation_contact.py
--rw-rw-rw-   0        0        0      398 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.6/examples/test.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.480684 epimodel_sensitivity_test-0.1.6/examples/utils/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/examples/utils/__init__.py
--rw-rw-rw-   0        0        0     3456 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/examples/utils/dataloader_16_ag.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.527555 epimodel_sensitivity_test-0.1.6/examples/vaccinated_sensitivity/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/examples/vaccinated_sensitivity/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.543189 epimodel_sensitivity_test-0.1.6/examples/vaccinated_sensitivity/configs/
--rw-rw-rw-   0        0        0     1574 2024-04-28 12:20:37.000000 epimodel_sensitivity_test-0.1.6/examples/vaccinated_sensitivity/configs/model_struct.json
--rw-rw-rw-   0        0        0      414 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/examples/vaccinated_sensitivity/configs/sampling_config.json
--rw-rw-rw-   0        0        0     2771 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/examples/vaccinated_sensitivity/sampler_vaccinated.py
--rw-rw-rw-   0        0        0     1112 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py
--rw-rw-rw-   0        0        0     3666 2024-04-08 20:55:46.000000 epimodel_sensitivity_test-0.1.6/examples/vaccinated_sensitivity/simulation_vacc.py
--rw-rw-rw-   0        0        0      428 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/examples/vaccinated_sensitivity/vaccinated_main.py
--rw-rw-rw-   0        0        0       42 2024-04-29 08:17:56.683814 epimodel_sensitivity_test-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1244 2024-04-29 08:17:51.000000 epimodel_sensitivity_test-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.574433 epimodel_sensitivity_test-0.1.6/src/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.6/src/__init__.py
--rw-rw-rw-   0        0        0      517 2024-04-29 08:05:11.000000 epimodel_sensitivity_test-0.1.6/src/dataloader.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.605686 epimodel_sensitivity_test-0.1.6/src/model/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.6/src/model/__init__.py
--rw-rw-rw-   0        0        0     1205 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/src/model/epidemic_model.py
--rw-rw-rw-   0        0        0    10445 2024-04-28 12:30:58.000000 epimodel_sensitivity_test-0.1.6/src/model/matrix_generator.py
--rw-rw-rw-   0        0        0     4134 2024-04-28 15:52:31.000000 epimodel_sensitivity_test-0.1.6/src/model/model_base.py
--rw-rw-rw-   0        0        0     4715 2024-04-28 12:20:37.000000 epimodel_sensitivity_test-0.1.6/src/model/r0.py
--rw-rw-rw-   0        0        0     8110 2024-04-28 16:26:24.000000 epimodel_sensitivity_test-0.1.6/src/plotter.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.636935 epimodel_sensitivity_test-0.1.6/src/sensitivity/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.6/src/sensitivity/__init__.py
--rw-rw-rw-   0        0        0     1137 2024-04-04 14:22:44.000000 epimodel_sensitivity_test-0.1.6/src/sensitivity/prcc.py
--rw-rw-rw-   0        0        0     4593 2024-04-08 14:28:40.000000 epimodel_sensitivity_test-0.1.6/src/sensitivity/sampler_base.py
--rw-rw-rw-   0        0        0     4874 2024-04-28 12:24:21.000000 epimodel_sensitivity_test-0.1.6/src/sensitivity/sensitivity_model_base.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.668190 epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/__init__.py
--rw-rw-rw-   0        0        0     1479 2024-04-08 13:26:57.000000 epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/output_generator.py
--rw-rw-rw-   0        0        0     1608 2024-04-08 14:34:22.000000 epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/r0calculator.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:17:56.683814 epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/sol_based/
--rw-rw-rw-   0        0        0        0 2024-04-07 15:24:44.000000 epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/sol_based/__init__.py
--rw-rw-rw-   0        0        0      908 2024-04-28 11:42:55.000000 epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/sol_based/final_size_calc.py
--rw-rw-rw-   0        0        0      923 2024-04-07 15:33:11.000000 epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/sol_based/peak_calc.py
--rw-rw-rw-   0        0        0     3373 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/sol_based/target_calc_base.py
--rw-rw-rw-   0        0        0     8511 2024-04-28 15:52:59.000000 epimodel_sensitivity_test-0.1.6/src/simulation_base.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.586039 epimodel_sensitivity_test-0.1.7/
+-rw-rw-rw-   0        0        0     2153 2024-04-30 16:59:44.585039 epimodel_sensitivity_test-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1698 2024-04-05 10:47:20.000000 epimodel_sensitivity_test-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.441342 epimodel_sensitivity_test-0.1.7/data/
+-rw-rw-rw-   0        0        0     6144 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.7/data/age_distribution.xls
+-rw-rw-rw-   0        0        0    26112 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.7/data/contact_matrices.xls
+-rw-rw-rw-   0        0        0     3079 2024-04-28 22:03:14.000000 epimodel_sensitivity_test-0.1.7/data/model_parameters.json
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.465349 epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/
+-rw-rw-rw-   0        0        0     2153 2024-04-30 16:59:44.000000 epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2423 2024-04-30 16:59:44.000000 epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 16:59:44.000000 epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-30 16:59:44.000000 epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 16:59:44.000000 epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.468349 epimodel_sensitivity_test-0.1.7/examples/
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.474351 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.479353 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/configs/
+-rw-rw-rw-   0        0        0      840 2024-04-30 14:35:58.000000 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/configs/model_struct.json
+-rw-rw-rw-   0        0        0      569 2024-04-30 14:26:59.000000 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/configs/sampling_config.json
+-rw-rw-rw-   0        0        0     1003 2024-04-30 14:43:33.000000 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/seihr_2_ag_main.py
+-rw-rw-rw-   0        0        0     1694 2024-04-27 18:48:18.000000 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/simulation_seihr.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.491365 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.496357 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/configs/
+-rw-rw-rw-   0        0        0      543 2024-04-30 14:35:58.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/configs/model_struct.json
+-rw-rw-rw-   0        0        0      372 2024-04-30 14:17:47.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/configs/sampling_config.json
+-rw-rw-rw-   0        0        0      344 2024-04-12 11:39:01.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/model_seir.py
+-rw-rw-rw-   0        0        0      332 2024-04-08 13:30:52.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/sampler_seir.py
+-rw-rw-rw-   0        0        0      739 2024-04-30 14:11:55.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/seir_no_ag_main.py
+-rw-rw-rw-   0        0        0     1187 2024-04-30 14:15:47.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/simulation_seir.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.506488 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.511541 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/configs/
+-rw-rw-rw-   0        0        0     1961 2024-04-30 14:35:59.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/configs/model_struct.json
+-rw-rw-rw-   0        0        0      428 2024-04-05 22:30:36.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/configs/sampling_config.json
+-rw-rw-rw-   0        0        0      452 2024-04-30 14:08:09.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/contact_main.py
+-rw-rw-rw-   0        0        0      572 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/sampler_contact.py
+-rw-rw-rw-   0        0        0     3159 2024-04-30 14:37:54.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/sensitivity_model_contact.py
+-rw-rw-rw-   0        0        0     3820 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/simulation_contact.py
+-rw-rw-rw-   0        0        0      398 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.7/examples/test.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.515605 epimodel_sensitivity_test-0.1.7/examples/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/utils/__init__.py
+-rw-rw-rw-   0        0        0     3456 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/utils/dataloader_16_ag.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.528936 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.535029 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/configs/
+-rw-rw-rw-   0        0        0     1569 2024-04-30 14:35:58.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/configs/model_struct.json
+-rw-rw-rw-   0        0        0      414 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/configs/sampling_config.json
+-rw-rw-rw-   0        0        0     2771 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/sampler_vaccinated.py
+-rw-rw-rw-   0        0        0     1112 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py
+-rw-rw-rw-   0        0        0     3666 2024-04-08 20:55:46.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/simulation_vacc.py
+-rw-rw-rw-   0        0        0      439 2024-04-30 13:55:41.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/vaccinated_main.py
+-rw-rw-rw-   0        0        0       42 2024-04-30 16:59:44.586039 epimodel_sensitivity_test-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1244 2024-04-30 16:59:34.000000 epimodel_sensitivity_test-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.544028 epimodel_sensitivity_test-0.1.7/src/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.7/src/__init__.py
+-rw-rw-rw-   0        0        0      517 2024-04-29 08:05:11.000000 epimodel_sensitivity_test-0.1.7/src/dataloader.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.556032 epimodel_sensitivity_test-0.1.7/src/model/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.7/src/model/__init__.py
+-rw-rw-rw-   0        0        0     1239 2024-04-30 14:32:48.000000 epimodel_sensitivity_test-0.1.7/src/model/epidemic_model.py
+-rw-rw-rw-   0        0        0    10445 2024-04-28 12:30:58.000000 epimodel_sensitivity_test-0.1.7/src/model/matrix_generator.py
+-rw-rw-rw-   0        0        0     4466 2024-04-30 14:32:48.000000 epimodel_sensitivity_test-0.1.7/src/model/model_base.py
+-rw-rw-rw-   0        0        0     4742 2024-04-30 14:32:48.000000 epimodel_sensitivity_test-0.1.7/src/model/r0.py
+-rw-rw-rw-   0        0        0     8110 2024-04-28 16:26:24.000000 epimodel_sensitivity_test-0.1.7/src/plotter.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.566035 epimodel_sensitivity_test-0.1.7/src/sensitivity/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/__init__.py
+-rw-rw-rw-   0        0        0     1137 2024-04-04 14:22:44.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/prcc.py
+-rw-rw-rw-   0        0        0     4661 2024-04-30 14:26:59.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/sampler_base.py
+-rw-rw-rw-   0        0        0     4988 2024-04-30 14:32:48.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/sensitivity_model_base.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.573035 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/__init__.py
+-rw-rw-rw-   0        0        0     1479 2024-04-08 13:26:57.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/output_generator.py
+-rw-rw-rw-   0        0        0     1606 2024-04-30 14:36:56.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/r0calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.582039 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/
+-rw-rw-rw-   0        0        0        0 2024-04-07 15:24:44.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/__init__.py
+-rw-rw-rw-   0        0        0      908 2024-04-28 11:42:55.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/final_size_calc.py
+-rw-rw-rw-   0        0        0      923 2024-04-07 15:33:11.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/peak_calc.py
+-rw-rw-rw-   0        0        0     3373 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/target_calc_base.py
+-rw-rw-rw-   0        0        0     8430 2024-04-30 14:36:31.000000 epimodel_sensitivity_test-0.1.7/src/simulation_base.py
```

### Comparing `epimodel_sensitivity_test-0.1.6/PKG-INFO` & `epimodel_sensitivity_test-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epimodel_sensitivity_test
-Version: 0.1.6
+Version: 0.1.7
 Summary: Efficient sensitivity analysis and evaluation of epidemiological models
 Home-page: https://github.com/KKol21/epimodel_sensitivity
 Author: Kolos Kovács
 Author-email: kovkol21@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `epimodel_sensitivity_test-0.1.6/README.md` & `epimodel_sensitivity_test-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/data/age_distribution.xls` & `epimodel_sensitivity_test-0.1.7/data/age_distribution.xls`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/data/contact_matrices.xls` & `epimodel_sensitivity_test-0.1.7/data/contact_matrices.xls`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/data/model_parameters.json` & `epimodel_sensitivity_test-0.1.7/data/model_parameters.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/epimodel_sensitivity_test.egg-info/PKG-INFO` & `epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epimodel-sensitivity-test
-Version: 0.1.6
+Version: 0.1.7
 Summary: Efficient sensitivity analysis and evaluation of epidemiological models
 Home-page: https://github.com/KKol21/epimodel_sensitivity
 Author: Kolos Kovács
 Author-email: kovkol21@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `epimodel_sensitivity_test-0.1.6/epimodel_sensitivity_test.egg-info/SOURCES.txt` & `epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/examples/SEIHR_2_age_groups/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/configs/model_struct.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('state_data', OrderedDict([('s', OrderedDict([('type', "*

 * *            "'susceptible')])), ('e', OrderedDict([('type', 'infected')])), ('i', "*

 * *            "OrderedDict([('type', 'infected')])), ('h', OrderedDict([('n_substates', 1)])), ('r', "*

 * *            "OrderedDict([('type', 'recovered')]))])), ('trans_data', [OrderedDict([('source', "*

 * *            "'i'), ('target', 'r'), ('param', 'gamma')]), OrderedDict([('source', 'e'), ('target', "*

 * *            "'i'), ('param', 'alpha'), ('dist […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "states": {
+    "state_data": {
         "e": {
             "type": "infected"
         },
         "h": {
             "n_substates": 1
         },
         "i": {
@@ -12,15 +12,24 @@
         "r": {
             "type": "recovered"
         },
         "s": {
             "type": "susceptible"
         }
     },
-    "transition": [
+    "tms_rules": [
+        {
+            "actors-params": {
+                "i": null
+            },
+            "source": "s",
+            "target": "e"
+        }
+    ],
+    "trans_data": [
         {
             "param": "gamma",
             "source": "i",
             "target": "r"
         },
         {
             "distr": [
@@ -39,18 +48,9 @@
             "target": "h"
         },
         {
             "param": "gamma",
             "source": "h",
             "target": "r"
         }
-    ],
-    "transmission_rules": [
-        {
-            "actors-params": {
-                "i": null
-            },
-            "source": "s",
-            "target": "e"
-        }
     ]
 }
```

### Comparing `epimodel_sensitivity_test-0.1.6/examples/SEIHR_2_age_groups/seihr_2_ag_main.py` & `epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/seihr_2_ag_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,24 +11,25 @@
               "alpha": 0.3,
               "eta": [0.5, 0.5]}
     for key, value in params.items():
         params[key] = torch.tensor(value)
     contact_data = torch.tensor([[1, 2],
                                  [0.5, 1]])
 
-    age_data = torch.tensor([[1E5,
-                              2E5]])
+    age_data = torch.tensor([1E5,
+                             2E5])
 
     data = SimpleNamespace(**{"params": params,
                               "cm": contact_data,
                               "age_data": age_data,
-                              "n_age": len(age_data[0]),
+                              "n_age": len(age_data),
                               "device": "cpu"})
 
     sim = SimulationSEIHR(data)
+    sim.model.visualize_transmission_graph()
     sim.run_sampling()
     sim.calculate_all_prcc()
     sim.calculate_all_p_values()
     sim.plot_all_prcc()
 
 
 if __name__ == "__main__":
```

### Comparing `epimodel_sensitivity_test-0.1.6/examples/SEIHR_2_age_groups/simulation_seihr.py` & `epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/simulation_seihr.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/examples/SEIR_no_age_groups/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/configs/model_struct.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('state_data', OrderedDict([('s', OrderedDict([('type', "*

 * *            "'susceptible')])), ('e', OrderedDict([('type', 'infected')])), ('i', "*

 * *            "OrderedDict([('type', 'infected')])), ('r', OrderedDict([('type', 'recovered')]))])), "*

 * *            "('trans_data', [OrderedDict([('source', 'i'), ('target', 'r'), ('param', 'gamma')]), "*

 * *            "OrderedDict([('source', 'e'), ('target', 'i'), ('param', 'alpha')])]), ('tms_rules', "*

 * *            "[OrderedDict([('source', 's'), […]*

```diff
@@ -1,37 +1,37 @@
 {
-    "states": {
+    "state_data": {
         "e": {
             "type": "infected"
         },
         "i": {
             "type": "infected"
         },
         "r": {
             "type": "recovered"
         },
         "s": {
             "type": "susceptible"
         }
     },
-    "transition": [
+    "tms_rules": [
+        {
+            "actors-params": {
+                "i": null
+            },
+            "source": "s",
+            "target": "e"
+        }
+    ],
+    "trans_data": [
         {
             "param": "gamma",
             "source": "i",
             "target": "r"
         },
         {
             "param": "alpha",
             "source": "e",
             "target": "i"
         }
-    ],
-    "transmission_rules": [
-        {
-            "actors-params": {
-                "i": null
-            },
-            "source": "s",
-            "target": "e"
-        }
     ]
 }
```

### Comparing `epimodel_sensitivity_test-0.1.6/examples/SEIR_no_age_groups/seir_no_ag_main.py` & `epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/seir_no_ag_main.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 import torch
 
 from examples.SEIR_no_age_groups.simulation_seir import SimulationSEIR
 
 
 def main():
-    params = {"gamma": 0.2, "beta": 0.2, "alpha": 0.3}
-    contact_data = torch.tensor([[1]])
-    age_data = torch.tensor([[10000]])
+    params = {"gamma": 0.2, "alpha": 0.3}
+    contact_data = torch.tensor(1)
+    age_data = torch.tensor(10000)
     data = SimpleNamespace(**{"params": params,
                               "cm": contact_data,
                               "age_data": age_data,
                               "n_age": 1,
                               "device": "cpu"})
 
     sim = SimulationSEIR(data)
+    sim.model.visualize_transmission_graph()
     sim.run_sampling()
     sim.calculate_all_prcc()
     sim.calculate_all_p_values()
     sim.plot_all_prcc()
 
 
 if __name__ == "__main__":
```

### Comparing `epimodel_sensitivity_test-0.1.6/examples/SEIR_no_age_groups/simulation_seir.py` & `epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/simulation_seir.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import os
 
-import torch
-
 from examples.SEIR_no_age_groups.model_seir import SEIRModel
 from examples.SEIR_no_age_groups.sampler_seir import SamplerSEIR
 from src.dataloader import PROJECT_PATH
 from src.simulation_base import SimulationBase
 
 
 class SimulationSEIR(SimulationBase):
@@ -16,23 +14,15 @@
         self.folder_name = os.path.join(self.folder_name, "sens_data_SEIR_no_ag")
 
         # Initalize model
         self.model = SEIRModel(sim_obj=self)
 
     def run_sampling(self):
         for variable_params in self.variable_param_combinations:
-            susc = self.tensorize(param=variable_params["susc"])
-            self.params.update({"susc": susc})
             base_r0 = variable_params["r0"]
             beta = self.get_beta_from_r0(base_r0)
             self.params["beta"] = beta
 
             self.model.initialize_matrices()
 
             param_generator = SamplerSEIR(sim_obj=self, variable_params=variable_params)
             param_generator.run()
-
-    def tensorize(self, param):
-        if isinstance(param, dict):
-            return torch.Tensor(list(param.values())[0], device=self.device)
-        else:
-            return torch.Tensor(param, device=self.device)
```

### Comparing `epimodel_sensitivity_test-0.1.6/examples/contact_sensitivity/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/configs/model_struct.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('state_data', OrderedDict([('s', OrderedDict([('type', "*

 * *            "'susceptible')])), ('l', OrderedDict([('type', 'infected'), ('n_substates', 2)])), "*

 * *            "('ip', OrderedDict([('type', 'infected')])), ('ia', OrderedDict([('type', "*

 * *            "'infected'), ('n_substates', 3)])), ('is', OrderedDict([('type', 'infected'), "*

 * *            "('n_substates', 3)])), ('ic', OrderedDict()), ('icr', OrderedDict()), ('h', "*

 * *            "OrderedDict()), ('r', OrderedDict([('type',  […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "states": {
+    "state_data": {
         "d": {
             "type": "dead"
         },
         "h": {},
         "ia": {
             "n_substates": 3,
             "type": "infected"
@@ -24,15 +24,26 @@
         "r": {
             "type": "recovered"
         },
         "s": {
             "type": "susceptible"
         }
     },
-    "transition": [
+    "tms_rules": [
+        {
+            "actors-params": {
+                "ia": "inf_a",
+                "ip": null,
+                "is": null
+            },
+            "source": "s",
+            "target": "l"
+        }
+    ],
+    "trans_data": [
         {
             "param": "alpha_l",
             "source": "l",
             "target": "ip"
         },
         {
             "distr": [
@@ -103,20 +114,9 @@
             "distr": [
                 "mu_"
             ],
             "param": "gamma_c",
             "source": "ic",
             "target": "icr"
         }
-    ],
-    "transmission_rules": [
-        {
-            "actors-params": {
-                "ia": "inf_a",
-                "ip": null,
-                "is": null
-            },
-            "source": "s",
-            "target": "l"
-        }
     ]
 }
```

### Comparing `epimodel_sensitivity_test-0.1.6/examples/contact_sensitivity/sampler_contact.py` & `epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/sampler_contact.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/examples/contact_sensitivity/sensitivity_model_contact.py` & `epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/sensitivity_model_contact.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         T = torch.zeros((cm_samples.size(0), self.s_mtx, self.s_mtx)).to(self.device)
         for idx, (beta, cm) in enumerate(zip(cm_samples, betas)):
             self.matrix_generator.ps.update({"beta": beta})
             T[idx, :, :] = self.matrix_generator.get_T(cm=cm)
         return T
 
     def _get_betas_from_contacts(self, cm_samples: torch.Tensor):
-        r0gen = R0Generator(data=self.data, **self.sim_obj.model_struct)
+        r0gen = R0Generator(data=self.data, model_struct=self.sim_obj.model_struct)
         betas = [self.base_r0 / r0gen.get_eig_val(contact_mtx=cm,
                                                   susceptibles=self.sim_obj.susceptibles.flatten(),
                                                   population=self.sim_obj.population)
                  for cm in cm_samples]
         return torch.tensor(betas, device=self.device)
 
     def get_contacts_from_lhs(self, lhs_table: np.ndarray):
```

### Comparing `epimodel_sensitivity_test-0.1.6/examples/contact_sensitivity/simulation_contact.py` & `epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/simulation_contact.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/examples/utils/dataloader_16_ag.py` & `epimodel_sensitivity_test-0.1.7/examples/utils/dataloader_16_ag.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/examples/vaccinated_sensitivity/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/configs/model_struct.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('state_data', OrderedDict([('s', OrderedDict([('type', "*

 * *            "'susceptible')])), ('e', OrderedDict([('type', 'infected'), ('n_substates', 3)])), "*

 * *            "('i', OrderedDict([('type', 'infected'), ('n_substates', 5)])), ('ic', "*

 * *            "OrderedDict()), ('icr', OrderedDict()), ('h', OrderedDict()), ('r', "*

 * *            "OrderedDict([('type', 'recovered')])), ('d', OrderedDict([('type', 'dead')])), ('v', "*

 * *            "OrderedDict([('type', 'recovered')]))])), ('tms_ […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "states": {
+    "state_data": {
         "d": {
             "type": "dead"
         },
         "e": {
             "n_substates": 3,
             "type": "infected"
         },
@@ -20,15 +20,24 @@
         "s": {
             "type": "susceptible"
         },
         "v": {
             "type": "recovered"
         }
     },
-    "transition": [
+    "tms_rules": [
+        {
+            "actors-params": {
+                "i": null
+            },
+            "source": "s",
+            "target": "e"
+        }
+    ],
+    "trans_data": [
         {
             "distr": [
                 "h_"
             ],
             "param": "gamma",
             "source": "i",
             "target": "r"
@@ -83,18 +92,9 @@
             "target": "icr"
         },
         {
             "param": "alpha",
             "source": "e",
             "target": "i"
         }
-    ],
-    "transmission_rules": [
-        {
-            "actors-params": {
-                "i": null
-            },
-            "source": "s",
-            "target": "e"
-        }
     ]
 }
```

### Comparing `epimodel_sensitivity_test-0.1.6/examples/vaccinated_sensitivity/sampler_vaccinated.py` & `epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/sampler_vaccinated.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py` & `epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/examples/vaccinated_sensitivity/simulation_vacc.py` & `epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/simulation_vacc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/setup.py` & `epimodel_sensitivity_test-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='epimodel_sensitivity_test',
-    version='0.1.6',
+    version='0.1.7',
     author='Kolos Kovács',
     author_email='kovkol21@gmail.com',
     description='Efficient sensitivity analysis and evaluation of epidemiological models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/KKol21/epimodel_sensitivity',
     packages=find_packages(),
```

### Comparing `epimodel_sensitivity_test-0.1.6/src/dataloader.py` & `epimodel_sensitivity_test-0.1.7/src/dataloader.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/src/model/epidemic_model.py` & `epimodel_sensitivity_test-0.1.7/src/model/epidemic_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import torch
 
 from src.model.model_base import EpidemicModelBase
 
 
 class EpidemicModel(EpidemicModelBase):
     def __init__(self, data, model_struct):
-        super().__init__(data, **model_struct)
+        super().__init__(data, model_struct)
 
     def get_solution(self, y0, t_eval, **kwargs):
-        return self.get_sol_from_ode(y0=y0,
-                                     t_eval=t_eval,
+        return self.get_sol_from_ode(y0=torch.atleast_2d(y0),
+                                     t_eval=torch.atleast_2d(t_eval),
                                      odefun=self.get_ode())
 
     def get_ode(self):
         if self.is_vaccinated:
             v_div = torch.ones(self.n_eq).to(self.device)
             div_idx = self.idx('s_0') + self.idx('v_0')
```

### Comparing `epimodel_sensitivity_test-0.1.6/src/model/matrix_generator.py` & `epimodel_sensitivity_test-0.1.7/src/model/matrix_generator.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/src/model/model_base.py` & `epimodel_sensitivity_test-0.1.7/src/model/model_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from abc import ABC, abstractmethod
 
 import torch
 import torchode as to
 
 
 class EpidemicModelBase(ABC):
-    def __init__(self, data, state_data, trans_data, tms_rules):
+    def __init__(self, data, model_struct):
         """
         Initialises Abstract base class for epidemic models.
 
         This class provides the base functionality for epidemic models. It contains methods to initialize the model,
         retrieve initial values, and obtain the model solutution
 
         Returns:
             None
         """
         self.data = data
-        self.state_data = state_data
-        self.trans_data = trans_data
-        self.tms_rules = tms_rules
+        self.state_data = model_struct["state_data"]
+        self.trans_data = model_struct["trans_data"]
+        self.tms_rules = model_struct["tms_rules"]
 
         self.n_age = data.n_age
         self.population = data.age_data.flatten()
         self.compartments = self.get_compartments()
         self.n_comp = len(self.compartments)
         self.ps = data.params
         self.device = data.device
@@ -45,14 +45,20 @@
         self.A = mtx_gen.get_A()
         self.T = mtx_gen.get_T()
         self.B = mtx_gen.get_B()
         if self.is_vaccinated:
             self.V_1 = mtx_gen.get_V_1()
             self.V_2 = mtx_gen.get_V_2()
 
+    def visualize_transmission_graph(self):
+        from src.plotter import visualize_transmission_graph
+        visualize_transmission_graph(state_data=self.state_data,
+                                     trans_data=self.trans_data,
+                                     tms_rules=self.tms_rules)
+
     @abstractmethod
     def get_solution(self, y0, t_eval, **kwargs):
         pass
 
     def get_sol_from_ode(self, y0, t_eval, odefun):
         term = to.ODETerm(odefun)
         step_method = to.Euler(term=term)
```

### Comparing `epimodel_sensitivity_test-0.1.6/src/model/r0.py` & `epimodel_sensitivity_test-0.1.7/src/model/r0.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import torch
 
 from src.model.matrix_generator import generate_transition_matrix, get_susc_mul, get_inf_mul, get_distr_mul
 from src.model.model_base import get_substates
 
 
 class R0Generator:
-    def __init__(self, data, state_data, trans_data, tms_rules):
+    def __init__(self, data, model_struct):
         self.data = data
         self.device = data.device
-        self.state_data = state_data
-        self.trans_data = trans_data
-        self.tms_rules = tms_rules
+        self.state_data = model_struct["state_data"]
+        self.trans_data = model_struct["trans_data"]
+        self.tms_rules = model_struct["tms_rules"]
 
         self.inf_states = self.get_infected_states()
         self.n_comp = len(self.inf_states)
         self.n_age = data.n_age
         self.n_states = len(self.inf_states)
         self.params = data.params
         self.i = {self.inf_states[index]: index for index in torch.arange(0, self.n_states)}
```

### Comparing `epimodel_sensitivity_test-0.1.6/src/plotter.py` & `epimodel_sensitivity_test-0.1.7/src/plotter.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/src/sensitivity/prcc.py` & `epimodel_sensitivity_test-0.1.7/src/sensitivity/prcc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/src/sensitivity/sampler_base.py` & `epimodel_sensitivity_test-0.1.7/src/sensitivity/sampler_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,16 @@
             bounds[:, idx] = param_bounds
         return bounds.T
 
     def _get_sim_output(self, lhs_table: np.ndarray):
         print(f"\n Simulation for {self.n_samples} samples ({self.sim_obj.get_filename(self.variable_params)})")
         print(f"Batch size: {self.batch_size}\n")
 
-        output_generator = OutputGenerator(self.sim_obj, self.variable_params)
+        output_generator = OutputGenerator(sim_obj=self.sim_obj,
+                                           variable_params=self.variable_params)
         sim_outputs = output_generator.get_output(lhs_table=lhs_table)
 
         time.sleep(0.3)
 
         # Save samples, target values
         filename = self.sim_obj.get_filename(self.variable_params)
         self.save_output(output=lhs_table, output_name='lhs', filename=filename)
```

### Comparing `epimodel_sensitivity_test-0.1.6/src/sensitivity/sensitivity_model_base.py` & `epimodel_sensitivity_test-0.1.7/src/sensitivity/sensitivity_model_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 def get_lhs_dict(params: list, lhs_table: torch.Tensor, params_col_idx: dict) -> dict:
     return {param: lhs_table[:, params_col_idx[param]] for param in params}
 
 
 class SensitivityModelBase(EpidemicModelBase, ABC):
     def __init__(self, sim_obj):
-        super().__init__(data=sim_obj.data, **sim_obj.model_struct)
+        super().__init__(data=sim_obj.data, model_struct=sim_obj.model_struct)
         self.sim_obj = sim_obj
         self.test = sim_obj.test
         self.sim_state = None
 
     def get_basic_ode(self):
         A_mul = self.get_mul_method(self.A)
         T_mul = self.get_mul_method(self.T)
@@ -66,21 +66,23 @@
 
         return mul_by_2d if len(tensor.size()) < 3 else mul_by_3d
 
     def get_matrix_from_lhs(self, lhs_dict: dict, matrix_name: str):
         n_eq = self.n_eq
         n_samples = next(iter(lhs_dict.values())).shape[0]
         mtx = torch.zeros((n_samples, n_eq, n_eq)).to(self.device)
+        ps_original = self.matrix_generator.ps.copy()
         for idx in range(n_samples):
             # Select idx. value from lhs table for each parameter
             row_dict = {key: value[idx] if len(value.size()) < 2 else value[idx, :]
                         for key, value in lhs_dict.items()}
             self.matrix_generator.ps.update(row_dict)
 
             mtx[idx, :, :] = self.matrix_generator.generate_matrix(matrix_name)
+        self.matrix_generator.ps = ps_original
         return mtx
 
     def get_initial_values(self):
         return self.get_initial_values_from_dict(self.sim_obj.init_vals)
 
     def generate_3D_matrices(self, samples: torch.Tensor):
         spb = self.sim_obj.sampled_params_boundaries
```

### Comparing `epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/output_generator.py` & `epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/output_generator.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/r0calculator.py` & `epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/r0calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         sim_obj = self.sim_obj
         n_samples = lhs_table.shape[0]
         spb = sim_obj.sampled_params_boundaries
         if spb is None:
             raise ValueError("Sampled parameters boundaries not specified, automatic R0 generation isn't possible")
         pci = get_params_col_idx(sampled_params_boundaries=spb)
         lhs_dict = get_lhs_dict(params=spb.keys(), lhs_table=lhs_table, params_col_idx=pci)
-        r0gen = R0Generator(sim_obj.data, **sim_obj.model_struct)
+        r0gen = R0Generator(sim_obj.data, sim_obj.model_struct)
         r0s = []
         print(f"Calculating R0 for {n_samples} samples")
         for idx in tqdm(range(n_samples)):
             # Select idx. value from lhs table for each parameter
             row_dict = {key: value[idx] if len(value.size()) < 2 else value[idx, :]
                         for key, value in lhs_dict.items()}
             r0gen.params.update(row_dict)
```

### Comparing `epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/sol_based/final_size_calc.py` & `epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/final_size_calc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/sol_based/peak_calc.py` & `epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/peak_calc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/src/sensitivity/target_calc/sol_based/target_calc_base.py` & `epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/target_calc_base.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.6/src/simulation_base.py` & `epimodel_sensitivity_test-0.1.7/src/simulation_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import itertools
 import json
 import os
 from abc import ABC, abstractmethod
 
 import numpy as np
 from scipy import stats as ss
+from torch import atleast_2d
 
 from src.dataloader import PROJECT_PATH
 from src.model.r0 import R0Generator
 from src.plotter import generate_tornado_plot
 from src.sensitivity.prcc import get_prcc_values
 
 
@@ -23,35 +24,33 @@
         self.data = data
         self.device = data.device
         self.model = None
 
         self._load_simulation_data()
         self._load_config(config_path)
         self._load_model_structure(model_struct_path)
-        from src.plotter import visualize_transmission_graph
-        visualize_transmission_graph(**self.model_struct)
 
     @property
     def susceptibles(self):
         return self.model.get_initial_values()[self.model.idx("s_0")]
 
     def _load_simulation_data(self):
         self.params = self.data.params
-        self.n_age = self.data.n_age
-        self.cm = self.data.cm
+        self.cm = atleast_2d(self.data.cm)
         self.population = self.data.age_data.flatten()
+        self.n_age = len(self.population)
         self.folder_name = os.path.join(PROJECT_PATH, "sens_data")
 
     def _load_model_structure(self, model_struct_path):
         with open(model_struct_path) as f:
             model_structure = json.load(f)
 
-        self.state_data = model_structure["states"]
-        self.trans_data = model_structure["transition"]
-        self.tms_rules = model_structure["transmission_rules"]
+        self.state_data = model_structure["state_data"]
+        self.trans_data = model_structure["trans_data"]
+        self.tms_rules = model_structure["tms_rules"]
 
         self.model_struct = {
             "state_data": self.state_data,
             "trans_data": self.trans_data,
             "tms_rules": self.tms_rules,
         }
 
@@ -113,15 +112,15 @@
         if isinstance(variable_params[key], dict):
             subkey = next(iter(variable_params[key]))
             return f"{key}-{subkey}"
         else:
             return f"{key}-{variable_params[key]}"
 
     def get_beta_from_r0(self, base_r0):
-        r0generator = R0Generator(self.data, **self.model_struct)
+        r0generator = R0Generator(self.data, self.model_struct)
         if isinstance(base_r0, tuple):
             base_r0 = base_r0[0]
         return base_r0 / r0generator.get_eig_val(contact_mtx=self.cm,
                                                  susceptibles=self.susceptibles.reshape(1, -1),
                                                  population=self.population)
 
     def calculate_prcc(self, filename: str, target: str) -> None:
```

