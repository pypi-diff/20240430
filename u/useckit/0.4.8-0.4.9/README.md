# Comparing `tmp/useckit-0.4.8.tar.gz` & `tmp/useckit-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "useckit-0.4.8.tar", last modified: Wed Jan 17 15:51:55 2024, max compression
+gzip compressed data, was "useckit-0.4.9.tar", last modified: Wed Jan 17 16:00:55 2024, max compression
```

## Comparing `useckit-0.4.8.tar` & `useckit-0.4.9.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.261711 useckit-0.4.8/
--rw-rw-rw-   0        0        0    35821 2021-01-21 13:00:25.000000 useckit-0.4.8/LICENSE
--rw-rw-rw-   0        0        0     1131 2024-01-17 15:51:55.260710 useckit-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-10-10 01:41:38.000000 useckit-0.4.8/README.md
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.093455 useckit-0.4.8/examples/
--rw-rw-rw-   0        0        0    22292 2024-01-17 14:17:18.000000 useckit-0.4.8/examples/useckit-high-level.ipynb
--rw-rw-rw-   0        0        0    11699 2023-05-06 09:26:39.000000 useckit-0.4.8/examples/useckit-low-level.ipynb
--rw-rw-rw-   0        0        0       42 2024-01-17 15:51:55.261711 useckit-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1116 2024-01-17 15:51:52.000000 useckit-0.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.097456 useckit-0.4.8/useckit/
--rw-rw-rw-   0        0        0    11197 2024-01-17 14:37:56.000000 useckit-0.4.8/useckit/Evaluators.py
--rw-rw-rw-   0        0        0      531 2023-01-16 21:07:19.000000 useckit-0.4.8/useckit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.116456 useckit-0.4.8/useckit/evaluation/
--rw-rw-rw-   0        0        0        0 2023-01-12 19:58:05.000000 useckit-0.4.8/useckit/evaluation/__init__.py
--rw-rw-rw-   0        0        0     3040 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/evaluation/identification.py
--rw-rw-rw-   0        0        0      937 2023-01-12 20:29:18.000000 useckit-0.4.8/useckit/evaluation/identification_with_reject.py
--rw-rw-rw-   0        0        0     4831 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/evaluation/verification.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.120596 useckit-0.4.8/useckit/paradigms/
--rw-rw-rw-   0        0        0        0 2023-01-12 20:29:18.000000 useckit-0.4.8/useckit/paradigms/__init__.py
--rw-rw-rw-   0        0        0     9790 2024-01-17 14:27:52.000000 useckit-0.4.8/useckit/paradigms/_paradigm_base.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.125805 useckit-0.4.8/useckit/paradigms/anomaly_detection/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/__init__.py
--rw-rw-rw-   0        0        0     2323 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/anomaly_paradigm.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.142711 useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/__init__.py
--rw-rw-rw-   0        0        0     2012 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/_fixed_false_negative_thresholding_method.py
--rw-rw-rw-   0        0        0      690 2023-01-12 19:58:05.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/anomaly_evaluation_method_base.py
--rw-rw-rw-   0        0        0     1687 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/identification.py
--rw-rw-rw-   0        0        0     2848 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/identification_with_reject.py
--rw-rw-rw-   0        0        0     3693 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/legacy_identification_with_reject.py
--rw-rw-rw-   0        0        0     2418 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/verification.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.156532 useckit-0.4.8/useckit/paradigms/anomaly_detection/prediction_models/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/prediction_models/__init__.py
--rw-rw-rw-   0        0        0     1389 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/prediction_models/anomaly_prediction_model_base.py
--rw-rw-rw-   0        0        0     8667 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/prediction_models/auto_encoder_keras_prediction_model.py
--rw-rw-rw-   0        0        0     1342 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/prediction_models/keras_model_descriptions.py
--rw-rw-rw-   0        0        0     3231 2024-01-17 14:17:18.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/prediction_models/scikit_anomaly_prediction_model.py
--rw-rw-rw-   0        0        0      587 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/anomaly_detection/prediction_models/scikit_model_descriptions.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.160530 useckit-0.4.8/useckit/paradigms/distance_learning/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.8/useckit/paradigms/distance_learning/__init__.py
--rw-rw-rw-   0        0        0     2338 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/distance_learning/distance_paradigm.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.180947 useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/__init__.py
--rw-rw-rw-   0        0        0     3076 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/_equal_error_thresholding_method.py
--rw-rw-rw-   0        0        0     4081 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/_sample_broadcasting.py
--rw-rw-rw-   0        0        0      623 2023-01-12 19:58:05.000000 useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/distance_evaluation_method_base.py
--rw-rw-rw-   0        0        0     4388 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/identification.py
--rw-rw-rw-   0        0        0     5181 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/identification_with_reject.py
--rw-rw-rw-   0        0        0     1078 2023-01-12 19:58:05.000000 useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/pairwise_accuracy_eval.py
--rw-rw-rw-   0        0        0     7752 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/verification.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.184874 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.190054 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/
--rw-rw-rw-   0        0        0        0 2023-01-12 19:58:05.000000 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/__init__.py
--rw-rw-rw-   0        0        0     5872 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_keras_prediction_model.py
--rw-rw-rw-   0        0        0     1674 2023-01-12 20:29:18.000000 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_model_description.py
--rw-rw-rw-   0        0        0      489 2023-01-12 19:58:05.000000 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/distance_prediction_model_base.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.200096 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/
--rw-rw-rw-   0        0        0        0 2023-01-12 19:59:01.000000 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/__init__.py
--rw-rw-rw-   0        0        0     5171 2023-01-12 20:29:18.000000 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/offline_triplet_keras_prediction_model.py
--rw-rw-rw-   0        0        0     4035 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triple_tower_model.py
--rw-rw-rw-   0        0        0      682 2023-01-12 19:59:01.000000 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triplet_distance_layer.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.204095 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/
--rw-rw-rw-   0        0        0        0 2023-01-12 19:59:01.000000 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/__init__.py
--rw-rw-rw-   0        0        0     5218 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/online_triplet_keras_prediction_model.py
--rw-rw-rw-   0        0        0     1959 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/scikit_distance_model.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.209096 useckit-0.4.8/useckit/paradigms/time_series_classification/
--rw-rw-rw-   0        0        0        0 2022-09-27 11:27:44.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.217095 useckit-0.4.8/useckit/paradigms/time_series_classification/evaluation_methods/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/evaluation_methods/__init__.py
--rw-rw-rw-   0        0        0     1444 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/evaluation_methods/identification.py
--rw-rw-rw-   0        0        0     1733 2023-01-12 20:29:18.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/evaluation_methods/legacy_identification.py
--rw-rw-rw-   0        0        0      396 2023-01-12 20:29:18.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/evaluation_methods/tsc_evaluation_method_base.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.237050 useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/
--rw-rw-rw-   0        0        0        0 2022-09-27 11:27:44.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/__init__.py
--rw-rw-rw-   0        0        0     4675 2023-01-12 20:29:18.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/classification_keras_prediction_model.py
--rw-rw-rw-   0        0        0     1597 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/classification_scikit_prediction_model.py
--rw-rw-rw-   0        0        0     1512 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/classification_xgboost_prediction_model.py
--rw-rw-rw-   0        0        0     5217 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/inception.py
--rw-rw-rw-   0        0        0     9420 2023-01-12 19:58:05.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/keras_model_descriptions.py
--rw-rw-rw-   0        0        0     3589 2023-01-19 23:13:48.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/mcdcnn.py
--rw-rw-rw-   0        0        0    23759 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/mcnn.py
--rw-rw-rw-   0        0        0    11621 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/tlenet.py
--rw-rw-rw-   0        0        0     1616 2023-01-12 20:29:18.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/tsc_prediction_model_base.py
--rw-rw-rw-   0        0        0    12771 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/twiesn.py
--rw-rw-rw-   0        0        0     2815 2024-01-17 14:37:56.000000 useckit-0.4.8/useckit/paradigms/time_series_classification/tsc_paradigm.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.246051 useckit-0.4.8/useckit/tests/
--rw-rw-rw-   0        0        0        0 2021-02-10 15:30:41.000000 useckit-0.4.8/useckit/tests/__init__.py
--rw-rw-rw-   0        0        0     4312 2023-06-02 09:26:04.000000 useckit-0.4.8/useckit/tests/test_dataset.py
--rw-rw-rw-   0        0        0     5328 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/tests/test_evaluations.py
--rw-rw-rw-   0        0        0     4084 2024-01-17 14:17:18.000000 useckit-0.4.8/useckit/tests/test_model_save_load.py
--rw-rw-rw-   0        0        0    11092 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/tests/test_models.py
--rw-rw-rw-   0        0        0     3061 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.257713 useckit-0.4.8/useckit/util/
--rw-rw-rw-   0        0        0        0 2022-09-27 11:27:44.000000 useckit-0.4.8/useckit/util/__init__.py
--rw-rw-rw-   0        0        0    13985 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/util/dataset.py
--rw-rw-rw-   0        0        0     9142 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/util/dataset_windowsliced.py
--rw-rw-rw-   0        0        0    10255 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/util/plotting.py
--rw-rw-rw-   0        0        0    25370 2023-04-12 08:55:25.000000 useckit-0.4.8/useckit/util/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-17 15:51:55.108511 useckit-0.4.8/useckit.egg-info/
--rw-rw-rw-   0        0        0     1131 2024-01-17 15:51:54.000000 useckit-0.4.8/useckit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5278 2024-01-17 15:51:54.000000 useckit-0.4.8/useckit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-17 15:51:54.000000 useckit-0.4.8/useckit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2024-01-17 15:51:54.000000 useckit-0.4.8/useckit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-01-17 15:51:54.000000 useckit-0.4.8/useckit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.817314 useckit-0.4.9/
+-rw-rw-rw-   0        0        0    35821 2021-01-21 13:00:25.000000 useckit-0.4.9/LICENSE
+-rw-rw-rw-   0        0        0     1131 2024-01-17 16:00:55.815311 useckit-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-10-10 01:41:38.000000 useckit-0.4.9/README.md
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.668313 useckit-0.4.9/examples/
+-rw-rw-rw-   0        0        0    22292 2024-01-17 14:17:18.000000 useckit-0.4.9/examples/useckit-high-level.ipynb
+-rw-rw-rw-   0        0        0    11699 2023-05-06 09:26:39.000000 useckit-0.4.9/examples/useckit-low-level.ipynb
+-rw-rw-rw-   0        0        0       42 2024-01-17 16:00:55.817314 useckit-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1116 2024-01-17 16:00:22.000000 useckit-0.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.672384 useckit-0.4.9/useckit/
+-rw-rw-rw-   0        0        0    11197 2024-01-17 14:37:56.000000 useckit-0.4.9/useckit/Evaluators.py
+-rw-rw-rw-   0        0        0      531 2023-01-16 21:07:19.000000 useckit-0.4.9/useckit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.690310 useckit-0.4.9/useckit/evaluation/
+-rw-rw-rw-   0        0        0        0 2023-01-12 19:58:05.000000 useckit-0.4.9/useckit/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     3040 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/evaluation/identification.py
+-rw-rw-rw-   0        0        0      937 2023-01-12 20:29:18.000000 useckit-0.4.9/useckit/evaluation/identification_with_reject.py
+-rw-rw-rw-   0        0        0     4831 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/evaluation/verification.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.694511 useckit-0.4.9/useckit/paradigms/
+-rw-rw-rw-   0        0        0        0 2023-01-12 20:29:18.000000 useckit-0.4.9/useckit/paradigms/__init__.py
+-rw-rw-rw-   0        0        0     9794 2024-01-17 16:00:14.000000 useckit-0.4.9/useckit/paradigms/_paradigm_base.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.699310 useckit-0.4.9/useckit/paradigms/anomaly_detection/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/__init__.py
+-rw-rw-rw-   0        0        0     2323 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/anomaly_paradigm.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.712348 useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/__init__.py
+-rw-rw-rw-   0        0        0     2012 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/_fixed_false_negative_thresholding_method.py
+-rw-rw-rw-   0        0        0      690 2023-01-12 19:58:05.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/anomaly_evaluation_method_base.py
+-rw-rw-rw-   0        0        0     1687 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/identification.py
+-rw-rw-rw-   0        0        0     2848 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/identification_with_reject.py
+-rw-rw-rw-   0        0        0     3693 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/legacy_identification_with_reject.py
+-rw-rw-rw-   0        0        0     2418 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/verification.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.722312 useckit-0.4.9/useckit/paradigms/anomaly_detection/prediction_models/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/prediction_models/__init__.py
+-rw-rw-rw-   0        0        0     1389 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/prediction_models/anomaly_prediction_model_base.py
+-rw-rw-rw-   0        0        0     8667 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/prediction_models/auto_encoder_keras_prediction_model.py
+-rw-rw-rw-   0        0        0     1342 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/prediction_models/keras_model_descriptions.py
+-rw-rw-rw-   0        0        0     3231 2024-01-17 14:17:18.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/prediction_models/scikit_anomaly_prediction_model.py
+-rw-rw-rw-   0        0        0      587 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/anomaly_detection/prediction_models/scikit_model_descriptions.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.725313 useckit-0.4.9/useckit/paradigms/distance_learning/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.9/useckit/paradigms/distance_learning/__init__.py
+-rw-rw-rw-   0        0        0     2338 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/distance_learning/distance_paradigm.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.739316 useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/__init__.py
+-rw-rw-rw-   0        0        0     3076 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/_equal_error_thresholding_method.py
+-rw-rw-rw-   0        0        0     4081 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/_sample_broadcasting.py
+-rw-rw-rw-   0        0        0      623 2023-01-12 19:58:05.000000 useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/distance_evaluation_method_base.py
+-rw-rw-rw-   0        0        0     4388 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/identification.py
+-rw-rw-rw-   0        0        0     5181 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/identification_with_reject.py
+-rw-rw-rw-   0        0        0     1078 2023-01-12 19:58:05.000000 useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/pairwise_accuracy_eval.py
+-rw-rw-rw-   0        0        0     7752 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/verification.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.744318 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.748308 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/
+-rw-rw-rw-   0        0        0        0 2023-01-12 19:58:05.000000 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/__init__.py
+-rw-rw-rw-   0        0        0     5872 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_keras_prediction_model.py
+-rw-rw-rw-   0        0        0     1674 2023-01-12 20:29:18.000000 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_model_description.py
+-rw-rw-rw-   0        0        0      489 2023-01-12 19:58:05.000000 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/distance_prediction_model_base.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.755313 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/
+-rw-rw-rw-   0        0        0        0 2023-01-12 19:59:01.000000 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/__init__.py
+-rw-rw-rw-   0        0        0     5171 2023-01-12 20:29:18.000000 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/offline_triplet_keras_prediction_model.py
+-rw-rw-rw-   0        0        0     4035 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triple_tower_model.py
+-rw-rw-rw-   0        0        0      682 2023-01-12 19:59:01.000000 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triplet_distance_layer.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.758309 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/
+-rw-rw-rw-   0        0        0        0 2023-01-12 19:59:01.000000 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/__init__.py
+-rw-rw-rw-   0        0        0     5218 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/online_triplet_keras_prediction_model.py
+-rw-rw-rw-   0        0        0     1959 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/scikit_distance_model.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.764978 useckit-0.4.9/useckit/paradigms/time_series_classification/
+-rw-rw-rw-   0        0        0        0 2022-09-27 11:27:44.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.775315 useckit-0.4.9/useckit/paradigms/time_series_classification/evaluation_methods/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/evaluation_methods/__init__.py
+-rw-rw-rw-   0        0        0     1444 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/evaluation_methods/identification.py
+-rw-rw-rw-   0        0        0     1733 2023-01-12 20:29:18.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/evaluation_methods/legacy_identification.py
+-rw-rw-rw-   0        0        0      396 2023-01-12 20:29:18.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/evaluation_methods/tsc_evaluation_method_base.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.796312 useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/
+-rw-rw-rw-   0        0        0        0 2022-09-27 11:27:44.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/__init__.py
+-rw-rw-rw-   0        0        0     4675 2023-01-12 20:29:18.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/classification_keras_prediction_model.py
+-rw-rw-rw-   0        0        0     1597 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/classification_scikit_prediction_model.py
+-rw-rw-rw-   0        0        0     1512 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/classification_xgboost_prediction_model.py
+-rw-rw-rw-   0        0        0     5217 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/inception.py
+-rw-rw-rw-   0        0        0     9420 2023-01-12 19:58:05.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/keras_model_descriptions.py
+-rw-rw-rw-   0        0        0     3589 2023-01-19 23:13:48.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/mcdcnn.py
+-rw-rw-rw-   0        0        0    23759 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/mcnn.py
+-rw-rw-rw-   0        0        0    11621 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/tlenet.py
+-rw-rw-rw-   0        0        0     1616 2023-01-12 20:29:18.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/tsc_prediction_model_base.py
+-rw-rw-rw-   0        0        0    12771 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/twiesn.py
+-rw-rw-rw-   0        0        0     2815 2024-01-17 14:37:56.000000 useckit-0.4.9/useckit/paradigms/time_series_classification/tsc_paradigm.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.806581 useckit-0.4.9/useckit/tests/
+-rw-rw-rw-   0        0        0        0 2021-02-10 15:30:41.000000 useckit-0.4.9/useckit/tests/__init__.py
+-rw-rw-rw-   0        0        0     4312 2023-06-02 09:26:04.000000 useckit-0.4.9/useckit/tests/test_dataset.py
+-rw-rw-rw-   0        0        0     5328 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/tests/test_evaluations.py
+-rw-rw-rw-   0        0        0     4084 2024-01-17 14:17:18.000000 useckit-0.4.9/useckit/tests/test_model_save_load.py
+-rw-rw-rw-   0        0        0    11092 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/tests/test_models.py
+-rw-rw-rw-   0        0        0     3061 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.814319 useckit-0.4.9/useckit/util/
+-rw-rw-rw-   0        0        0        0 2022-09-27 11:27:44.000000 useckit-0.4.9/useckit/util/__init__.py
+-rw-rw-rw-   0        0        0    13985 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/util/dataset.py
+-rw-rw-rw-   0        0        0     9142 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/util/dataset_windowsliced.py
+-rw-rw-rw-   0        0        0    10255 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/util/plotting.py
+-rw-rw-rw-   0        0        0    25370 2023-04-12 08:55:25.000000 useckit-0.4.9/useckit/util/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-17 16:00:55.683315 useckit-0.4.9/useckit.egg-info/
+-rw-rw-rw-   0        0        0     1131 2024-01-17 16:00:55.000000 useckit-0.4.9/useckit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5278 2024-01-17 16:00:55.000000 useckit-0.4.9/useckit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-17 16:00:55.000000 useckit-0.4.9/useckit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2024-01-17 16:00:55.000000 useckit-0.4.9/useckit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-01-17 16:00:55.000000 useckit-0.4.9/useckit.egg-info/top_level.txt
```

### Comparing `useckit-0.4.8/LICENSE` & `useckit-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/PKG-INFO` & `useckit-0.4.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useckit
-Version: 0.4.8
+Version: 0.4.9
 Home-page: https://blindforreview.com
 Author: BlindForReview.com
 Author-email: mail@blindforreview.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `useckit-0.4.8/examples/useckit-high-level.ipynb` & `useckit-0.4.9/examples/useckit-high-level.ipynb`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/examples/useckit-low-level.ipynb` & `useckit-0.4.9/examples/useckit-low-level.ipynb`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/setup.py` & `useckit-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="useckit",
-    version="0.4.8",
+    version="0.4.9",
     author="BlindForReview.com",
     author_email="mail@blindforreview.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://blindforreview.com",
     packages=setuptools.find_packages(include=['useckit', 'useckit.*']),
```

### Comparing `useckit-0.4.8/useckit/Evaluators.py` & `useckit-0.4.9/useckit/Evaluators.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/__init__.py` & `useckit-0.4.9/useckit/__init__.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/evaluation/identification.py` & `useckit-0.4.9/useckit/evaluation/identification.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/evaluation/identification_with_reject.py` & `useckit-0.4.9/useckit/evaluation/identification_with_reject.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/evaluation/verification.py` & `useckit-0.4.9/useckit/evaluation/verification.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/_paradigm_base.py` & `useckit-0.4.9/useckit/paradigms/_paradigm_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,18 +126,18 @@
                 try:
                     self.name += '_' + type(prediction_model).__name__
                 except Exception:
                     pass  # append nothing
         self.output_dir = os.path.join(self.output_dir, self.name)
         os.makedirs(self.output_dir, exist_ok=True)
         ParadigmBase._experiment_number += 1
-        if len(os.listdir(self.output_dir)) != 0:
-            raise AttributeError(
-                "Please choose a unique name for your experiment or delete/move previous results, " +
-                "if you want to refrain from naming them by hand")
+        #if len(os.listdir(self.output_dir)) != 0:
+        #    raise AttributeError(
+        #        "Please choose a unique name for your experiment or delete/move previous results, " +
+        #        "if you want to refrain from naming them by hand")
 
     def _propagate_output_dir_to_model_evaluation(self, prediction_model: PredictionModelBase,
                                                   evaluation_methods: [EvaluationMethodBase]):
         self.prediction_model = prediction_model
         prediction_model.merge_paradigm_output_folder(self.output_dir)
         if isinstance(evaluation_methods, EvaluationMethodBase):
             evaluation_methods = [evaluation_methods]
```

### Comparing `useckit-0.4.8/useckit/paradigms/anomaly_detection/anomaly_paradigm.py` & `useckit-0.4.9/useckit/paradigms/anomaly_detection/anomaly_paradigm.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/_fixed_false_negative_thresholding_method.py` & `useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/_fixed_false_negative_thresholding_method.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/anomaly_evaluation_method_base.py` & `useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/anomaly_evaluation_method_base.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/identification.py` & `useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/identification.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/identification_with_reject.py` & `useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/identification_with_reject.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/legacy_identification_with_reject.py` & `useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/legacy_identification_with_reject.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/anomaly_detection/evaluation_methods/verification.py` & `useckit-0.4.9/useckit/paradigms/anomaly_detection/evaluation_methods/verification.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/anomaly_detection/prediction_models/anomaly_prediction_model_base.py` & `useckit-0.4.9/useckit/paradigms/anomaly_detection/prediction_models/anomaly_prediction_model_base.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/anomaly_detection/prediction_models/auto_encoder_keras_prediction_model.py` & `useckit-0.4.9/useckit/paradigms/anomaly_detection/prediction_models/auto_encoder_keras_prediction_model.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/anomaly_detection/prediction_models/keras_model_descriptions.py` & `useckit-0.4.9/useckit/paradigms/anomaly_detection/prediction_models/keras_model_descriptions.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/anomaly_detection/prediction_models/scikit_anomaly_prediction_model.py` & `useckit-0.4.9/useckit/paradigms/anomaly_detection/prediction_models/scikit_anomaly_prediction_model.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/anomaly_detection/prediction_models/scikit_model_descriptions.py` & `useckit-0.4.9/useckit/paradigms/anomaly_detection/prediction_models/scikit_model_descriptions.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/distance_paradigm.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/distance_paradigm.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/_equal_error_thresholding_method.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/_equal_error_thresholding_method.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/_sample_broadcasting.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/_sample_broadcasting.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/distance_evaluation_method_base.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/distance_evaluation_method_base.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/identification.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/identification.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/identification_with_reject.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/identification_with_reject.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/pairwise_accuracy_eval.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/pairwise_accuracy_eval.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/evaluation_methods/verification.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/evaluation_methods/verification.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_keras_prediction_model.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_keras_prediction_model.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_model_description.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_model_description.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/offline_triplet_keras_prediction_model.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/offline_triplet_keras_prediction_model.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triple_tower_model.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triple_tower_model.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triplet_distance_layer.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triplet_distance_layer.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/online_triplet_keras_prediction_model.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/online_triplet_keras_prediction_model.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/distance_learning/prediction_models/scikit_distance_model.py` & `useckit-0.4.9/useckit/paradigms/distance_learning/prediction_models/scikit_distance_model.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/time_series_classification/evaluation_methods/identification.py` & `useckit-0.4.9/useckit/paradigms/time_series_classification/evaluation_methods/identification.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/time_series_classification/evaluation_methods/legacy_identification.py` & `useckit-0.4.9/useckit/paradigms/time_series_classification/evaluation_methods/legacy_identification.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/classification_keras_prediction_model.py` & `useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/classification_keras_prediction_model.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/classification_scikit_prediction_model.py` & `useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/classification_scikit_prediction_model.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/classification_xgboost_prediction_model.py` & `useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/classification_xgboost_prediction_model.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/inception.py` & `useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/inception.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/keras_model_descriptions.py` & `useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/keras_model_descriptions.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/mcdcnn.py` & `useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/mcdcnn.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/mcnn.py` & `useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/mcnn.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/tlenet.py` & `useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/tlenet.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/tsc_prediction_model_base.py` & `useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/tsc_prediction_model_base.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/time_series_classification/prediction_models/twiesn.py` & `useckit-0.4.9/useckit/paradigms/time_series_classification/prediction_models/twiesn.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/paradigms/time_series_classification/tsc_paradigm.py` & `useckit-0.4.9/useckit/paradigms/time_series_classification/tsc_paradigm.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/tests/test_dataset.py` & `useckit-0.4.9/useckit/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/tests/test_evaluations.py` & `useckit-0.4.9/useckit/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/tests/test_model_save_load.py` & `useckit-0.4.9/useckit/tests/test_model_save_load.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/tests/test_models.py` & `useckit-0.4.9/useckit/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/tests/test_utils.py` & `useckit-0.4.9/useckit/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/util/dataset.py` & `useckit-0.4.9/useckit/util/dataset.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/util/dataset_windowsliced.py` & `useckit-0.4.9/useckit/util/dataset_windowsliced.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/util/plotting.py` & `useckit-0.4.9/useckit/util/plotting.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit/util/utils.py` & `useckit-0.4.9/useckit/util/utils.py`

 * *Files identical despite different names*

### Comparing `useckit-0.4.8/useckit.egg-info/PKG-INFO` & `useckit-0.4.9/useckit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useckit
-Version: 0.4.8
+Version: 0.4.9
 Home-page: https://blindforreview.com
 Author: BlindForReview.com
 Author-email: mail@blindforreview.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `useckit-0.4.8/useckit.egg-info/SOURCES.txt` & `useckit-0.4.9/useckit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

