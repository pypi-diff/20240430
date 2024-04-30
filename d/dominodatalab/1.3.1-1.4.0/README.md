# Comparing `tmp/dominodatalab-1.3.1.tar.gz` & `tmp/dominodatalab-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dominodatalab-1.3.1.tar", last modified: Fri Apr 19 13:15:35 2024, max compression
+gzip compressed data, was "dominodatalab-1.4.0.tar", last modified: Tue Apr 30 14:03:10 2024, max compression
```

## Comparing `dominodatalab-1.3.1.tar` & `dominodatalab-1.4.0.tar`

### file list

```diff
@@ -1,102 +1,104 @@
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:35.022921 dominodatalab-1.3.1/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    11358 2022-06-06 14:00:07.000000 dominodatalab-1.3.1/LICENSE.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)       14 2022-06-21 20:35:17.000000 dominodatalab-1.3.1/MANIFEST.in
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    24348 2024-04-19 13:15:35.021533 dominodatalab-1.3.1/PKG-INFO
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    22833 2024-04-19 12:58:12.000000 dominodatalab-1.3.1/README.md
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.766755 dominodatalab-1.3.1/domino/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      105 2022-06-21 20:35:17.000000 dominodatalab-1.3.1/domino/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9576 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_custom_metrics.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.767623 dominodatalab-1.3.1/domino/_impl/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)        0 2022-10-18 20:07:39.000000 dominodatalab-1.3.1/domino/_impl/__init__.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.779576 dominodatalab-1.3.1/domino/_impl/custommetrics/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      821 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    58419 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/api_client.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.857266 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      214 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      972 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/path_to_api.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.863336 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/paths/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      253 2022-10-18 20:07:39.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/paths/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      137 2022-10-18 20:07:39.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/paths/api_metric_alerts_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      137 2022-10-18 20:07:39.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/paths/api_metric_values_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      184 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/paths/api_metric_values_v1_model_monitoring_id_metric.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      383 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/tag_to_api.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.865630 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/tags/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      336 2022-10-18 20:07:39.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/tags/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      750 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/tags/custom_metrics_api.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15937 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/configuration.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4416 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/exceptions.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.909076 dominodatalab-1.3.1/domino/_impl/custommetrics/model/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      360 2022-10-18 20:07:39.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3798 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/failure_envelope_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3798 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/failure_envelope_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2463 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/invalid_body_envelope_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2463 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/invalid_body_envelope_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3801 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metadata_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3801 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metadata_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4856 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_alert_request_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4888 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_alert_request_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2871 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_tag_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2871 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_tag_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4529 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_value_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4561 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_value_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4054 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_values_envelope_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4118 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_values_envelope_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     5730 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_value_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     5762 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_value_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3557 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3589 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4848 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/target_range_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4449 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/target_range_v1.pyi
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.964660 dominodatalab-1.3.1/domino/_impl/custommetrics/models/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1236 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/models/__init__.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.966859 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      508 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/__init__.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.972200 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      351 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15351 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15120 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.pyi
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.977750 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      351 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15377 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1/post.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15146 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1/post.pyi
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.996467 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      405 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    16879 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    16648 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    10493 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/rest.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    96843 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/schemas.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)       22 2024-04-19 12:46:23.000000 dominodatalab-1.3.1/domino/_version.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.999103 dominodatalab-1.3.1/domino/airflow/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      259 2022-06-21 20:35:17.000000 dominodatalab-1.3.1/domino/airflow/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    11462 2023-01-05 19:13:36.000000 dominodatalab-1.3.1/domino/airflow/_operator.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3612 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/authentication.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1513 2023-01-18 14:15:18.000000 dominodatalab-1.3.1/domino/constants.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      723 2022-07-27 14:46:07.000000 dominodatalab-1.3.1/domino/data_sources.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9038 2024-01-19 15:58:01.000000 dominodatalab-1.3.1/domino/datasets.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    54359 2024-04-19 12:44:33.000000 dominodatalab-1.3.1/domino/domino.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1626 2022-07-06 17:07:45.000000 dominodatalab-1.3.1/domino/exceptions.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2426 2022-08-22 21:15:27.000000 dominodatalab-1.3.1/domino/helpers.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3408 2024-04-18 11:57:59.000000 dominodatalab-1.3.1/domino/http_request_manager.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9454 2024-01-19 15:58:01.000000 dominodatalab-1.3.1/domino/routes.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      787 2022-06-21 20:35:17.000000 dominodatalab-1.3.1/domino/training_sets.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:35.017349 dominodatalab-1.3.1/dominodatalab.egg-info/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    24348 2024-04-19 13:15:34.000000 dominodatalab-1.3.1/dominodatalab.egg-info/PKG-INFO
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3540 2024-04-19 13:15:34.000000 dominodatalab-1.3.1/dominodatalab.egg-info/SOURCES.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)        1 2024-04-19 13:15:34.000000 dominodatalab-1.3.1/dominodatalab.egg-info/dependency_links.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      424 2024-04-19 13:15:34.000000 dominodatalab-1.3.1/dominodatalab.egg-info/requires.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)        7 2024-04-19 13:15:34.000000 dominodatalab-1.3.1/dominodatalab.egg-info/top_level.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      879 2024-04-19 13:15:10.000000 dominodatalab-1.3.1/requirements.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)       38 2024-04-19 13:15:35.023150 dominodatalab-1.3.1/setup.cfg
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2184 2024-04-18 11:57:59.000000 dominodatalab-1.3.1/setup.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:35.015797 dominodatalab-1.3.1/tests/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9921 2024-04-18 11:57:59.000000 dominodatalab-1.3.1/tests/test_basic_auth.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      675 2022-08-22 21:15:27.000000 dominodatalab-1.3.1/tests/test_data_sources.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     5183 2024-04-19 12:44:33.000000 dominodatalab-1.3.1/tests/test_datasets.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1492 2024-04-18 11:57:59.000000 dominodatalab-1.3.1/tests/test_domino.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2015 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/tests/test_environments.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9142 2024-04-19 12:44:33.000000 dominodatalab-1.3.1/tests/test_jobs.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1969 2022-06-21 20:35:17.000000 dominodatalab-1.3.1/tests/test_models.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      505 2022-08-22 21:15:27.000000 dominodatalab-1.3.1/tests/test_no_data_sources.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2280 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/tests/test_operator.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9614 2023-12-14 22:20:12.000000 dominodatalab-1.3.1/tests/test_projects.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3472 2024-04-19 12:44:33.000000 dominodatalab-1.3.1/tests/test_spark_operator.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.223392 dominodatalab-1.4.0/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    11358 2022-06-06 14:00:07.000000 dominodatalab-1.4.0/LICENSE.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)       14 2022-06-21 20:35:17.000000 dominodatalab-1.4.0/MANIFEST.in
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    30459 2024-04-30 14:03:10.221122 dominodatalab-1.4.0/PKG-INFO
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    28944 2024-04-30 12:48:57.000000 dominodatalab-1.4.0/README.md
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.014395 dominodatalab-1.4.0/domino/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      105 2022-06-21 20:35:17.000000 dominodatalab-1.4.0/domino/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9576 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_custom_metrics.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.016384 dominodatalab-1.4.0/domino/_impl/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)        0 2022-10-18 20:07:39.000000 dominodatalab-1.4.0/domino/_impl/__init__.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.033306 dominodatalab-1.4.0/domino/_impl/custommetrics/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      821 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    58419 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/api_client.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.044702 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      214 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      972 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/path_to_api.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.052424 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/paths/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      253 2022-10-18 20:07:39.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/paths/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      137 2022-10-18 20:07:39.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/paths/api_metric_alerts_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      137 2022-10-18 20:07:39.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/paths/api_metric_values_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      184 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/paths/api_metric_values_v1_model_monitoring_id_metric.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      383 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/tag_to_api.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.056223 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/tags/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      336 2022-10-18 20:07:39.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/tags/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      750 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/tags/custom_metrics_api.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15937 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/configuration.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4416 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/exceptions.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.100222 dominodatalab-1.4.0/domino/_impl/custommetrics/model/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      360 2022-10-18 20:07:39.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3798 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/failure_envelope_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3798 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/failure_envelope_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2463 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/invalid_body_envelope_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2463 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/invalid_body_envelope_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3801 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metadata_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3801 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metadata_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4856 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_alert_request_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4888 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_alert_request_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2871 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_tag_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2871 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_tag_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4529 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_value_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4561 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_value_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4054 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_values_envelope_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4118 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_values_envelope_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     5730 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_value_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     5762 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_value_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3557 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3589 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4848 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/target_range_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4449 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/target_range_v1.pyi
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.102229 dominodatalab-1.4.0/domino/_impl/custommetrics/models/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1236 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/models/__init__.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.104818 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      508 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/__init__.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.109647 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      351 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15351 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15120 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.pyi
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.114092 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      351 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15377 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1/post.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15146 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1/post.pyi
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.145291 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      405 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    16879 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    16648 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    10493 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/rest.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    96843 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/schemas.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)       22 2024-04-30 12:33:26.000000 dominodatalab-1.4.0/domino/_version.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.164659 dominodatalab-1.4.0/domino/airflow/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      259 2022-06-21 20:35:17.000000 dominodatalab-1.4.0/domino/airflow/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    11462 2023-01-05 19:13:36.000000 dominodatalab-1.4.0/domino/airflow/_operator.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3612 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/authentication.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1513 2024-04-24 12:43:48.000000 dominodatalab-1.4.0/domino/constants.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      723 2022-07-27 14:46:07.000000 dominodatalab-1.4.0/domino/data_sources.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9038 2024-01-19 15:58:01.000000 dominodatalab-1.4.0/domino/datasets.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    69419 2024-04-30 12:15:28.000000 dominodatalab-1.4.0/domino/domino.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      437 2024-04-30 12:15:28.000000 dominodatalab-1.4.0/domino/domino_enums.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1626 2022-07-06 17:07:45.000000 dominodatalab-1.4.0/domino/exceptions.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2426 2022-08-22 21:15:27.000000 dominodatalab-1.4.0/domino/helpers.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3408 2024-04-29 13:03:50.000000 dominodatalab-1.4.0/domino/http_request_manager.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    10594 2024-04-30 12:15:28.000000 dominodatalab-1.4.0/domino/routes.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      787 2022-06-21 20:35:17.000000 dominodatalab-1.4.0/domino/training_sets.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.214326 dominodatalab-1.4.0/dominodatalab.egg-info/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    30459 2024-04-30 14:03:09.000000 dominodatalab-1.4.0/dominodatalab.egg-info/PKG-INFO
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3584 2024-04-30 14:03:09.000000 dominodatalab-1.4.0/dominodatalab.egg-info/SOURCES.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)        1 2024-04-30 14:03:09.000000 dominodatalab-1.4.0/dominodatalab.egg-info/dependency_links.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      424 2024-04-30 14:03:09.000000 dominodatalab-1.4.0/dominodatalab.egg-info/requires.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)        7 2024-04-30 14:03:09.000000 dominodatalab-1.4.0/dominodatalab.egg-info/top_level.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      879 2024-04-30 14:02:11.000000 dominodatalab-1.4.0/requirements.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)       38 2024-04-30 14:03:10.223650 dominodatalab-1.4.0/setup.cfg
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2184 2024-04-19 14:44:50.000000 dominodatalab-1.4.0/setup.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.212525 dominodatalab-1.4.0/tests/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9973 2024-04-30 12:15:28.000000 dominodatalab-1.4.0/tests/test_basic_auth.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      675 2022-08-22 21:15:27.000000 dominodatalab-1.4.0/tests/test_data_sources.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     5183 2024-04-19 12:44:33.000000 dominodatalab-1.4.0/tests/test_datasets.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1321 2024-04-30 12:15:28.000000 dominodatalab-1.4.0/tests/test_domino.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2015 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/tests/test_environments.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9013 2024-04-30 12:15:28.000000 dominodatalab-1.4.0/tests/test_finops.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9142 2024-04-19 12:44:33.000000 dominodatalab-1.4.0/tests/test_jobs.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1969 2022-06-21 20:35:17.000000 dominodatalab-1.4.0/tests/test_models.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      505 2022-08-22 21:15:27.000000 dominodatalab-1.4.0/tests/test_no_data_sources.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2280 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/tests/test_operator.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9614 2023-12-14 22:20:12.000000 dominodatalab-1.4.0/tests/test_projects.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3472 2024-04-19 12:44:33.000000 dominodatalab-1.4.0/tests/test_spark_operator.py
```

### Comparing `dominodatalab-1.3.1/LICENSE.txt` & `dominodatalab-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/PKG-INFO` & `dominodatalab-1.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dominodatalab
-Version: 1.3.1
+Version: 1.4.0
 Summary: Python bindings for the Domino API
 Home-page: https://github.com/dominodatalab/python-domino
-Download-URL: https://github.com/dominodatalab/python-domino/archive/release-1.3.1.zip
+Download-URL: https://github.com/dominodatalab/python-domino/archive/release-1.4.0.zip
 Author: Domino Data Lab
 Author-email: support@dominodatalab.com
 License: Apache Software License (Apache 2.0)
 Keywords: Domino Data Lab,API
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -43,28 +43,29 @@
 See this documentation for details about the APIs:
 
 -   [Latest public Domino
     APIs](https://docs.dominodatalab.com/en/latest/api_guide/8c929e/domino-public-apis/)
 
 -   [Legacy APIs](https://dominodatalab.github.io/api-docs/)
 
-The latest released version of `python-domino` is `1.3.1`.
+The latest released version of `python-domino` is `1.4.0`.
 
 # Version compatibility matrix
 
 The `python-domino` library is compatible with different versions of
 Domino:
 
 | Domino Versions |                                    Python-Domino                                    |
 |-----------------|:-----------------------------------------------------------------------------------:|
 | 3.6.x or lower  |      [0.3.5](https://github.com/dominodatalab/python-domino/archive/0.3.5.zip)       |
 | 4.1.0 or higher | [1.0.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/1.0.0.zip) or Higher |
 | 5.3.0 or higher | [1.2.0]https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.0.zip) or Higher |
 | 5.5.0 or higher | [1.2.2](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.2.zip) or Higher |
 | 5.10.0 or higher | [1.3.1](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.3.1.zip) or Higher |
+| 5.11.0 or higher | [1.4.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.4.0.zip) or Higher |
 
 # Development
 
 The current `python-domino` is based on Python 3.9, which is therefore recommended for development. `Pipenv` is also recommended to manage the dependencies.
 
 To use the Python binding in a Domino workbook session, include `dominodatalab` in your project's requirements.txt file.
 This makes the Python binding available for each new workbook session (or batch run) started within the project.
@@ -143,20 +144,212 @@
     
     Default Retry is set to 4 
     Determines the number of attempts for the request session in case of a ConnectionError
     Get more info on request max timeout/error durations based on Retry and backoff factors [here](https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry)
 
 # Methods
 
+# Budgets and Billing Tags
+
+See
+[`example_budget_manager.py`](https://github.com/dominodatalab/python-domino/blob/release-1.4.0/examples/example_budget_manager.py)
+for example code.
+
+### budget_defaults_list()
+
+Get a list of the available default budgets with the assigned (if any) limits
+Requires Admin permission
+
+### budget_defaults_update(budget_label, budget_limit)
+
+Update default budgets by BudgetLabel
+Requires Admin roles
+
+-   *budget_label:* (required) label of budget to be updated ex: `BillingTag`, `Organization`
+
+-   *budget_limit:* (required) new budget quota to assign to default label
+
+### budget_overrides_list()
+
+Get a list of the available budgets overrides with the assigned limits.
+Requires Admin permission
+
+### budget_override_create(budget_label, budget_id, budget_limit)
+
+Create Budget overrides based on BudgetLabels, ie BillingTags, Organization, or Projects
+the object id is used as budget ids
+Requires Admin roles
+
+-   *budget_label:* label of budget to be updated
+
+-   *budget_id:* id of project or organization to be used as new budget override id.
+
+-   *budget_limit:* budget quota to assign to override
+
+### budget_override_update(budget_label, budget_id, budget_limit)
+
+Update Budget overrides based on BudgetLabel and budget id
+Requires Admin roles
+
+-   *budget_label:* label of budget to be updated
+
+-   *budget_id:* id of budget override to be updated.
+
+-   *budget_limit:* new budget quota to assign to override
+
+### budget_override_delete(budget_id)
+
+Delete an existing budget override
+Requires Admin roles
+
+-   *budget_id:* id of budget override to be deleted.
+
+### budget_alerts_settings()
+
+Get the current budget alerts settings
+Requires Admin permission
+
+### budget_alerts_settings_update(alerts_enabled, notify_org_owner)
+
+Update the current budget alerts settings to enable/disable budget notifications
+and whether to notify org owners on projects notifications
+Requires Admin permission
+
+-   *alerts_enabled:* whether to enable or disable notifications.
+
+-   *notify_org_owner:* whether to notify organizations owners on projects reaching threshold.
+
+### budget_alerts_targets_update(targets)
+
+Update the current budget alerts settings with additional email targets per budget label
+Requires Admin permission
+
+-   *targets:* dictionary of budget labels and list of email addresses
+
+### billing_tags_list_active()
+
+Get a list of active billing tags
+Requires Admin permission
+
+### billing_tags_create(tags_list)
+
+Create a list of active billing tags
+Requires Admin permission
+
+-   *tags_list:* list of billing tags names to be created
+
+### active_billing_tag_by_name(name)
+
+Get detailed info on active or archived billing tag
+Requires Admin permission
+
+-   *name:* name of existing billing tag
+
+### billing_tag_archive(name)
+
+Archive an active billing tag
+Requires Admin permission
+
+-   *name:* name of existing billing tag to archive
+
+### billing_tag_settings()
+
+Get the current billing tag settings
+Requires Admin permission
+
+### billing_tag_settings_mode()
+
+Get the current billing tag settings mode
+Requires Admin permission
+
+### billing_tag_settings_mode_update(mode)
+
+Update the current billing tag settings mode
+Requires Admin permission
+
+-   *mode:* new mode to set the billing tag settings (see BillingTagSettingMode)
+
+### project_billing_tag(project_id)
+
+Get a billing tag assigned to a particular project by project id
+Requires Admin permission
+
+-   *project_id:* id of the project to find assigned billing tag
+
+###  project_billing_tag_update(billing_tag, project_id)
+
+Update project's billing tag with new billing tag.
+Requires Admin permission
+
+-   *billing_tag:* billing tag to assign to a project
+
+-   *project_id:* id of the project to assign a billing tag
+
+### project_billing_tag_reset(project_id)
+
+Remove a billing tag from a specified project
+Requires Admin permission
+
+-   *project_id:* id of the project to reset billing tag field
+
+### projects_by_billing_tag( billing_tag, offset, page_size, name_filter, sort_by, sort_order, missing_tag_only=False)
+
+Remove a billing tag from a specified project
+Requires Admin permission
+
+-   *billing_tag:* billing tag string to filter projects by
+
+-   *offset:* The index of the start of the page, where checkpointProjectId is index 0.
+If the offset is negative the project it points to will be the end of the page.
+-   *page_size:* The number of records to return per page.
+
+-   *name_filter:* matches projects by name substring
+
+-   *sort_by:* (Optional) field to sort the projects on
+
+-   *sort_order:* (Optional) Whether to sort in asc or desc order
+
+-   *missing_tag_only:* (Optional) determine whether to only return projects with missing tag
+
+### project_billing_tag_bulk_update(projects_tag)
+
+Update project's billing tags in bulk
+Requires Admin permission
+
+-   *projects_tag:* dictionary of project_id and billing_tags
+
+
 ## Projects
 
 See
 [`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/example_projects_usage.py)
 for example code.
 
+### project_create_v4(project_name, owner_id, owner_username, description, collaborators, tags, billing_tag, visibility=PUBLIC)
+
+Newer version of projects creation using the v4 endpoints which allows more optional fields.
+
+-   *project_name:* (required) The name of the project.
+
+-   *owner_id:* (Optional) user id of the owner of the new project to be created (must be admin to create projects for other users)
+  owner_id or owner_username can be used, both are not needed (Defaults to current owner_username)
+
+-   *owner_username:* (Optional) username of the owner of the new project to be created (must be admin to create projects for other users)
+  owner_id or owner_username can be used, both are not needed (Defaults to current owner_username)
+
+-   *description:* (Optional) description of the project
+
+-   *collaborators:* (Optional) list of collaborators to be added to the project
+
+-   *tags:* (Optional) list of tags to add to project
+
+-   *billing_tag:* (Optional unless billingTag settings mode is Required) active billing tag to be added to projects for governance
+
+-   *visibility:* (Optional) (Defaults to Public) project visibility 
+
 ### project_create(project_name, owner_username=None)
 
 Create a new project with given project name.
 
 -   *project_name:* The name of the project.
 
 -   *owner_username:* (Optional) The owner username for the project.
```

### Comparing `dominodatalab-1.3.1/README.md` & `dominodatalab-1.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 See this documentation for details about the APIs:
 
 -   [Latest public Domino
     APIs](https://docs.dominodatalab.com/en/latest/api_guide/8c929e/domino-public-apis/)
 
 -   [Legacy APIs](https://dominodatalab.github.io/api-docs/)
 
-The latest released version of `python-domino` is `1.3.1`.
+The latest released version of `python-domino` is `1.4.0`.
 
 # Version compatibility matrix
 
 The `python-domino` library is compatible with different versions of
 Domino:
 
 | Domino Versions |                                    Python-Domino                                    |
 |-----------------|:-----------------------------------------------------------------------------------:|
 | 3.6.x or lower  |      [0.3.5](https://github.com/dominodatalab/python-domino/archive/0.3.5.zip)       |
 | 4.1.0 or higher | [1.0.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/1.0.0.zip) or Higher |
 | 5.3.0 or higher | [1.2.0]https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.0.zip) or Higher |
 | 5.5.0 or higher | [1.2.2](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.2.zip) or Higher |
 | 5.10.0 or higher | [1.3.1](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.3.1.zip) or Higher |
+| 5.11.0 or higher | [1.4.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.4.0.zip) or Higher |
 
 # Development
 
 The current `python-domino` is based on Python 3.9, which is therefore recommended for development. `Pipenv` is also recommended to manage the dependencies.
 
 To use the Python binding in a Domino workbook session, include `dominodatalab` in your project's requirements.txt file.
 This makes the Python binding available for each new workbook session (or batch run) started within the project.
@@ -103,20 +104,212 @@
     
     Default Retry is set to 4 
     Determines the number of attempts for the request session in case of a ConnectionError
     Get more info on request max timeout/error durations based on Retry and backoff factors [here](https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry)
 
 # Methods
 
+# Budgets and Billing Tags
+
+See
+[`example_budget_manager.py`](https://github.com/dominodatalab/python-domino/blob/release-1.4.0/examples/example_budget_manager.py)
+for example code.
+
+### budget_defaults_list()
+
+Get a list of the available default budgets with the assigned (if any) limits
+Requires Admin permission
+
+### budget_defaults_update(budget_label, budget_limit)
+
+Update default budgets by BudgetLabel
+Requires Admin roles
+
+-   *budget_label:* (required) label of budget to be updated ex: `BillingTag`, `Organization`
+
+-   *budget_limit:* (required) new budget quota to assign to default label
+
+### budget_overrides_list()
+
+Get a list of the available budgets overrides with the assigned limits.
+Requires Admin permission
+
+### budget_override_create(budget_label, budget_id, budget_limit)
+
+Create Budget overrides based on BudgetLabels, ie BillingTags, Organization, or Projects
+the object id is used as budget ids
+Requires Admin roles
+
+-   *budget_label:* label of budget to be updated
+
+-   *budget_id:* id of project or organization to be used as new budget override id.
+
+-   *budget_limit:* budget quota to assign to override
+
+### budget_override_update(budget_label, budget_id, budget_limit)
+
+Update Budget overrides based on BudgetLabel and budget id
+Requires Admin roles
+
+-   *budget_label:* label of budget to be updated
+
+-   *budget_id:* id of budget override to be updated.
+
+-   *budget_limit:* new budget quota to assign to override
+
+### budget_override_delete(budget_id)
+
+Delete an existing budget override
+Requires Admin roles
+
+-   *budget_id:* id of budget override to be deleted.
+
+### budget_alerts_settings()
+
+Get the current budget alerts settings
+Requires Admin permission
+
+### budget_alerts_settings_update(alerts_enabled, notify_org_owner)
+
+Update the current budget alerts settings to enable/disable budget notifications
+and whether to notify org owners on projects notifications
+Requires Admin permission
+
+-   *alerts_enabled:* whether to enable or disable notifications.
+
+-   *notify_org_owner:* whether to notify organizations owners on projects reaching threshold.
+
+### budget_alerts_targets_update(targets)
+
+Update the current budget alerts settings with additional email targets per budget label
+Requires Admin permission
+
+-   *targets:* dictionary of budget labels and list of email addresses
+
+### billing_tags_list_active()
+
+Get a list of active billing tags
+Requires Admin permission
+
+### billing_tags_create(tags_list)
+
+Create a list of active billing tags
+Requires Admin permission
+
+-   *tags_list:* list of billing tags names to be created
+
+### active_billing_tag_by_name(name)
+
+Get detailed info on active or archived billing tag
+Requires Admin permission
+
+-   *name:* name of existing billing tag
+
+### billing_tag_archive(name)
+
+Archive an active billing tag
+Requires Admin permission
+
+-   *name:* name of existing billing tag to archive
+
+### billing_tag_settings()
+
+Get the current billing tag settings
+Requires Admin permission
+
+### billing_tag_settings_mode()
+
+Get the current billing tag settings mode
+Requires Admin permission
+
+### billing_tag_settings_mode_update(mode)
+
+Update the current billing tag settings mode
+Requires Admin permission
+
+-   *mode:* new mode to set the billing tag settings (see BillingTagSettingMode)
+
+### project_billing_tag(project_id)
+
+Get a billing tag assigned to a particular project by project id
+Requires Admin permission
+
+-   *project_id:* id of the project to find assigned billing tag
+
+###  project_billing_tag_update(billing_tag, project_id)
+
+Update project's billing tag with new billing tag.
+Requires Admin permission
+
+-   *billing_tag:* billing tag to assign to a project
+
+-   *project_id:* id of the project to assign a billing tag
+
+### project_billing_tag_reset(project_id)
+
+Remove a billing tag from a specified project
+Requires Admin permission
+
+-   *project_id:* id of the project to reset billing tag field
+
+### projects_by_billing_tag( billing_tag, offset, page_size, name_filter, sort_by, sort_order, missing_tag_only=False)
+
+Remove a billing tag from a specified project
+Requires Admin permission
+
+-   *billing_tag:* billing tag string to filter projects by
+
+-   *offset:* The index of the start of the page, where checkpointProjectId is index 0.
+If the offset is negative the project it points to will be the end of the page.
+-   *page_size:* The number of records to return per page.
+
+-   *name_filter:* matches projects by name substring
+
+-   *sort_by:* (Optional) field to sort the projects on
+
+-   *sort_order:* (Optional) Whether to sort in asc or desc order
+
+-   *missing_tag_only:* (Optional) determine whether to only return projects with missing tag
+
+### project_billing_tag_bulk_update(projects_tag)
+
+Update project's billing tags in bulk
+Requires Admin permission
+
+-   *projects_tag:* dictionary of project_id and billing_tags
+
+
 ## Projects
 
 See
 [`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/example_projects_usage.py)
 for example code.
 
+### project_create_v4(project_name, owner_id, owner_username, description, collaborators, tags, billing_tag, visibility=PUBLIC)
+
+Newer version of projects creation using the v4 endpoints which allows more optional fields.
+
+-   *project_name:* (required) The name of the project.
+
+-   *owner_id:* (Optional) user id of the owner of the new project to be created (must be admin to create projects for other users)
+  owner_id or owner_username can be used, both are not needed (Defaults to current owner_username)
+
+-   *owner_username:* (Optional) username of the owner of the new project to be created (must be admin to create projects for other users)
+  owner_id or owner_username can be used, both are not needed (Defaults to current owner_username)
+
+-   *description:* (Optional) description of the project
+
+-   *collaborators:* (Optional) list of collaborators to be added to the project
+
+-   *tags:* (Optional) list of tags to add to project
+
+-   *billing_tag:* (Optional unless billingTag settings mode is Required) active billing tag to be added to projects for governance
+
+-   *visibility:* (Optional) (Defaults to Public) project visibility 
+
 ### project_create(project_name, owner_username=None)
 
 Create a new project with given project name.
 
 -   *project_name:* The name of the project.
 
 -   *owner_username:* (Optional) The owner username for the project.
```

### Comparing `dominodatalab-1.3.1/domino/_custom_metrics.py` & `dominodatalab-1.4.0/domino/_custom_metrics.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/__init__.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/api_client.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/api_client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/apis/path_to_api.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/apis/tags/custom_metrics_api.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/apis/tags/custom_metrics_api.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/configuration.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/configuration.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/exceptions.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/exceptions.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/failure_envelope_v1.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/failure_envelope_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/failure_envelope_v1.pyi` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/failure_envelope_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/invalid_body_envelope_v1.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/invalid_body_envelope_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/invalid_body_envelope_v1.pyi` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/invalid_body_envelope_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metadata_v1.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metadata_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metadata_v1.pyi` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metadata_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_alert_request_v1.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_alert_request_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_alert_request_v1.pyi` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_alert_request_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_tag_v1.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_tag_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_tag_v1.pyi` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_tag_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_value_v1.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_value_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_value_v1.pyi` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_value_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_values_envelope_v1.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_values_envelope_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_values_envelope_v1.pyi` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_values_envelope_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_value_v1.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_value_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_value_v1.pyi` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_value_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.pyi` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/target_range_v1.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/target_range_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/model/target_range_v1.pyi` & `dominodatalab-1.4.0/domino/_impl/custommetrics/model/target_range_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/models/__init__.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.pyi` & `dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1/post.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1/post.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1/post.pyi` & `dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1/post.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.pyi` & `dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/rest.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/rest.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/_impl/custommetrics/schemas.py` & `dominodatalab-1.4.0/domino/_impl/custommetrics/schemas.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/airflow/_operator.py` & `dominodatalab-1.4.0/domino/airflow/_operator.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/authentication.py` & `dominodatalab-1.4.0/domino/authentication.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/constants.py` & `dominodatalab-1.4.0/domino/constants.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/data_sources.py` & `dominodatalab-1.4.0/domino/data_sources.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/datasets.py` & `dominodatalab-1.4.0/domino/datasets.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/domino.py` & `dominodatalab-1.4.0/domino/domino.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import functools
+import json
 import logging
 import os
 from packaging import version
 import re
 import time
 from typing import List, Optional, Tuple
 import warnings
@@ -10,14 +11,15 @@
 import polling2
 import requests
 from bs4 import BeautifulSoup
 
 from domino import exceptions, helpers, datasets
 from domino._version import __version__
 from domino.authentication import get_auth_by_type
+from domino.domino_enums import BillingTagSettingMode, BudgetLabel, BudgetType, ProjectVisibility
 from domino.constants import (
     CLUSTER_TYPE_MIN_SUPPORT,
     DOMINO_HOST_KEY_NAME,
     DOMINO_LOG_LEVEL_KEY_NAME,
     MINIMUM_EXTERNAL_VOLUME_MOUNTS_SUPPORT_DOMINO_VERSION,
     MINIMUM_ON_DEMAND_SPARK_CLUSTER_SUPPORT_DOMINO_VERSION,
     MINIMUM_SUPPORTED_DOMINO_VERSION,
@@ -38,28 +40,27 @@
         assert _host, (
             "Host must be supplied as a parameter or through the "
             f"{DOMINO_HOST_KEY_NAME} environment variable."
         )
         host = helpers.clean_host_url(_host)
 
         try:
-            owner_username, project_name = project.split("/")
-            self._routes = _Routes(host, owner_username, project_name)
+            self._owner_username, self._project_name = project.split("/")
+            self._routes = _Routes(host, self._owner_username, self._project_name)
         except ValueError:
             self._logger.error(
                 f"Project {project} must be given in the form username/projectname"
             )
             raise
 
         # This call sets self.request_manager
         self.authenticate(api_key, auth_token, domino_token_file, api_proxy)
 
         # Get version
-        self._version = "5.10.0"
-        # self._version = self.deployment_version().get("version")
+        self._version = self.deployment_version().get("version")
         assert self.requires_at_least(MINIMUM_SUPPORTED_DOMINO_VERSION)
 
         self._logger.debug(
             f"Domino deployment {host} is running version {self._version}"
         )
 
         # Check version compatibility
@@ -730,28 +731,60 @@
         response = self.request_manager.post(url, json=request)
         return response
 
     def deployment_version(self):
         url = self._routes.deployment_version()
         return self._get(url)
 
+    def project_create_v4(
+        self,
+        project_name: str,
+        owner_id: Optional[str] = None,
+        owner_username: Optional[str] = None,
+        description: Optional[str] = "",
+        collaborators: Optional[list] = None,
+        tags: Optional[list] = None,
+        billing_tag: Optional[str] = None,
+        visibility: Optional[ProjectVisibility] = ProjectVisibility.PUBLIC,
+    ):
+        owner = (
+            owner_id if owner_id else self.get_user_id(owner_username) if owner_username
+            else self.get_user_id(self._owner_username)
+        )
+        data = {
+            "name": project_name,
+            "visibility": visibility.value,
+            "ownerId": owner,
+            "description": description,
+            "collaborators": collaborators if collaborators is not None else [],
+            "tags": {"tagNames": tags if tags is not None else []},
+        }
+
+        if billing_tag:
+            data.update({"billingTag": {"tag": billing_tag}})
+
+        url = self._routes.project_v4()
+        payload = json.dumps(data)
+        response = self.request_manager.post(url, data=payload, headers={'Content-Type': 'application/json'})
+        return response.json()
+
     def project_create(self, project_name, owner_username=None):
         url = self._routes.project_create()
         data = {"projectName": project_name, "ownerOverrideUsername": owner_username}
         response = self.request_manager.post(
             url, data=data, headers=self._csrf_no_check_header
         )
         return response
 
     def project_archive(self, project_name):
         """Delete the project with the given name"""
         all_owned_projects = self.projects_list(show_completed=True)
         for p in all_owned_projects:
             if p["name"] == project_name:
-                url = self._routes.project_archive(project_id=p["id"])
+                url = self._routes.project_v4(project_id=p["id"])
                 self.request_manager.delete(url)
                 break
         else:
             raise exceptions.ProjectNotFoundException(project_name)
 
     def projects_list(self, relationship="Owned", show_completed=False):
         url = self._routes.projects_list()
@@ -767,15 +800,15 @@
             "showCompleted": str(show_completed).lower(),
         }
         response = self.request_manager.get(url, params=query)
         return response.json()
 
     def tags_list(self, project_id=None):
         project_id = project_id if project_id else self.project_id
-        url = self._routes.tags_list(project_id)
+        url = self._routes.project_v4(project_id)
         return self._get(url)["tags"]
 
     def tag_details(self, tag_id):
         url = self._routes.tag_details(tag_id)
         return self._get(url)
 
     def tags_add(self, tags: list, project_id=None):
@@ -1103,15 +1136,14 @@
             target_relative_path=target_relative_path
         ) as uploader:
             path = uploader.upload()
             self.log.info(f"Uploading chunks for file or directory `{path}` to dataset {dataset_id} completed. "
                           f"Now attempting to end upload session.")
             return path
 
-
     def model_version_export(
         self,
         model_id,
         model_version_id,
         registry_host,
         registry_username,
         registry_password,
@@ -1191,25 +1223,365 @@
                 text = BeautifulSoup(line, "html.parser").text
 
                 if "text-danger" in line:
                     self.log.warning(text)
                 else:
                     self.log.info(text)
 
+    def budget_defaults_list(self) -> list:
+        """
+        Get a list of the available default budgets with the assigned (if any) limits
+        Requires Admin permission
+
+        :return: Returns a list of default budgets with details
+        """
+        url = self._routes.budgets_default()
+        return self.request_manager.get(url).json()
+
+    def budget_defaults_update(self, budget_label: BudgetLabel, budget_limit: float) -> dict:
+        """
+        Update default budgets limits (or quota) by BudgetLabel
+        Requires Admin permission
+
+        :param budget_label: label of budget to be updated ex: `BillingTag`, `Organization`
+        :param budget_limit: new budget quota to assign to default label
+
+        :return: Returns the updated budget with the newly assigned limit.
+        """
+        url = self._routes.budgets_default(budget_label.value)
+        updated_budget = {"budgetLabel": budget_label.value, "budgetType": "Default", "limit": budget_limit,
+                          "window": "monthly"}
+        data = json.dumps(updated_budget)
+        return self.request_manager.put(url, data=data, headers={"Content-Type": "application/json"}).json()
+
+    def budget_overrides_list(self):
+        """
+        Get a list of the available budgets overrides with the assigned limits.
+        Requires Admin permission
+
+        :return: Returns a list of budgets overrides with details
+        """
+        url = self._routes.budget_overrides()
+        return self.request_manager.get(url).json()
+
+    def budget_override_create(self, budget_label: BudgetLabel, budget_id: str, budget_limit: float) -> dict:
+        """
+        Create Budget overrides based on BudgetLabels, ie BillingTags, Organization, or Projects
+        the object id is used as budget ids
+        Requires Admin roles
+
+        :param budget_label: label of budget to be updated
+        :param budget_id: id of project or organization to be used as new budget override id.
+        :param budget_limit: budget quota to assign to override
+
+        :return: Returns the newly created budget override
+        """
+        url = self._routes.budget_overrides()
+        new_budget: dict = self._generate_budget(budget_label, budget_id, budget_limit)
+        data = json.dumps(new_budget)
+        return self.request_manager.post(url, data=data, headers={"Content-Type": "application/json"}).json()
+
+    def budget_override_update(self, budget_label: BudgetLabel, budget_id: str, budget_limit: float) -> dict:
+        """
+        Update Budget overrides based on BudgetLabel and budget id
+        Requires Admin roles
+
+        :param budget_label: label of budget to be updated
+        :param budget_id: id of budget override to be updated.
+        :param budget_limit: new budget quota to assign to override
+
+        :return: Returns the updated budget override
+        """
+        url = self._routes.budget_overrides(budget_id)
+        new_budget: dict = self._generate_budget(budget_label, budget_id, budget_limit)
+        data = json.dumps(new_budget)
+        return self.request_manager.put(url, data=data, headers={"Content-Type": "application/json"}).json()
+
+    def budget_override_delete(self, budget_id: str) -> list:
+        """
+        Delete an existing budget override
+        Requires Admin roles
+
+        :param budget_id: id of budget override to be deleted.
+
+        :return: Returns list of messages confirming the budget override deletion
+        """
+        url = self._routes.budget_overrides(budget_id)
+        return self.request_manager.delete(url).json()
+
+    def budget_alerts_settings(self) -> dict:
+        """
+        Get the current budget alerts settings
+        Requires Admin permission
+
+        :return: Returns the current budget alert setting
+        """
+        url = self._routes.budget_settings()
+        return self.request_manager.get(url).json()
+
+    def budget_alerts_settings_update(
+        self,
+        alerts_enabled: Optional[bool] = None,
+        notify_org_owner: Optional[bool] = None
+    ) -> dict:
+        """
+        Update the current budget alerts settings to enable/disable budget notifications
+        and whether to notify org owners on projects notifications
+        Requires Admin permission
+
+        :param alerts_enabled: whether to enable or disable notifications.
+        :param notify_org_owner: whether to notify organizations owners on projects reaching threshold.
+
+        :return: Returns the updated budget alert setting
+        """
+        current_settings = self.budget_alerts_settings()
+
+        optional_fields = {
+            "alertsEnabled": alerts_enabled,
+            "notifyOrgOwner": notify_org_owner
+        }
+
+        updated_settings = self._update_if_set(current_settings, optional_fields)
+
+        payload = json.dumps(updated_settings)
+        url = self._routes.budget_settings()
+        return self.request_manager.put(url, data=payload).json()
+
+    def budget_alerts_targets_update(self, targets: dict[BudgetLabel, list]) -> dict:
+        """
+        Update the current budget alerts settings with additional email targets per budget label
+        Requires Admin permission
+
+        :param targets: dictionary of budget labels and list of email addresses
+
+        :return: Returns the updated budget alert setting
+        """
+
+        budget_settings = self.budget_alerts_settings()
+
+        current_targets = budget_settings["alertTargets"]
+
+        updated_targets = []
+
+        for target in current_targets:
+            if target["label"] in targets:
+                updated_targets.append({"label": target["label"], "emails": targets[target["label"]]})
+            else:
+                updated_targets.append(target)
+
+        budget_settings["alertTargets"] = updated_targets
+
+        payload = json.dumps(budget_settings)
+        url = self._routes.budget_settings()
+        return self.request_manager.put(url, data=payload).json()
+
+    def billing_tags_list_active(self) -> dict:
+        """
+        Get a list of active billing tags
+        Requires Admin permission
+
+        :return: Returns a dictionary containing the list active billing tags
+        """
+        self.requires_at_least("5.11.0")
+        url = self._routes.billing_tags()
+        return self.request_manager.get(url).json()
+
+    def billing_tags_create(self, tags_list: list) -> dict:
+        """
+        Create a list of active billing tags
+        Requires Admin permission
+
+        :param tags_list: list of billing tags names to be created
+
+        :return: Returns a dictionary containing the list newly created billing tags
+        """
+        self.requires_at_least("5.11.0")
+        url = self._routes.billing_tags()
+        payload = json.dumps({"billingTags": tags_list})
+        return self.request_manager.post(url, data=payload, headers={"Content-Type": "application/json"}).json()
+
+    def active_billing_tag_by_name(self, name: str) -> dict:
+        """
+        Get detailed info on active or archived billing tag
+        Requires Admin permission
+
+        :param name: name of existing billing tag
+
+        :return: Returns a dictionary containing the list newly created billing tags
+        """
+        url = self._routes.billing_tags(name)
+        return self.request_manager.get(url).json()
+
+    def billing_tag_archive(self, name: str) -> dict:
+        """
+        Archive an active billing tag
+        Requires Admin permission
+
+        :param name: name of existing billing tag to archive
+
+        :return: Returns a dictionary containing the updated billing tag
+        """
+        url = self._routes.billing_tags(name)
+        return self.request_manager.delete(url).json()
+
+    def billing_tag_settings(self) -> dict:
+        """
+        Get the current billing tag settings
+        Requires Admin permission
+
+        :return: Returns the current billing tag settings
+        """
+        url = self._routes.billing_tags_settings()
+        return self.request_manager.get(url).json()
+
+    def billing_tag_settings_mode(self) -> dict:
+        """
+        Get the current billing tag settings mode
+        Requires Admin permission
+
+        :return: Returns the current billing tag settings mode
+        """
+        url = self._routes.billing_tags_settings(mode_only=True)
+        return self.request_manager.get(url).json()
+
+    def billing_tag_settings_mode_update(self, mode: BillingTagSettingMode) -> dict[str, BillingTagSettingMode]:
+        """
+        Update the current billing tag settings mode
+        Requires Admin permission
+
+        :param mode: new mode to set the billing tag settings (see BillingTagSettingMode)
+
+        :return: Returns the updated billing tag settings mode
+        """
+        url = self._routes.billing_tags_settings(mode_only=True)
+        payload = json.dumps({"mode": mode.value})
+        return self.request_manager.put(url, data=payload, headers={"Content-Type": "application/json"}).json()
+
+    def project_billing_tag(self, project_id: Optional[str] = None) -> Optional[dict]:
+        """
+        Get a billing tag assigned to a particular project by project id
+        Requires Admin permission
+
+        :param project_id: id of the project to find assigned billing tag
+
+        :return: Returns the billing tag if assigned or None
+        """
+        url = self._routes.project_billing_tag(project_id if project_id else self.project_id)
+        return self.request_manager.get(url).json()
+
+    def project_billing_tag_update(self, billing_tag: str, project_id: Optional[str] = None) -> dict:
+        """
+        Update project's billing tag with new billing tag.
+        Requires Admin permission
+
+        :param billing_tag: billing tag to assign to a project
+        :param project_id: id of the project to assign a billing tag
+
+        :return: Returns the project details including the new billing tag
+        """
+        url = self._routes.project_billing_tag(project_id if project_id else self.project_id)
+        data = {
+            "tag": billing_tag
+        }
+        return self.request_manager.post(url, data=json.dumps(data)).json()
+
+    def project_billing_tag_reset(self, project_id: Optional[str] = None) -> dict:
+        """
+        Remove a billing tag from a specified project
+        Requires Admin permission
+
+        :param project_id: id of the project to reset billing tag field
+
+        :return: Returns the project details
+        """
+        url = self._routes.project_billing_tag(project_id if project_id else self.project_id)
+        return self.request_manager.delete(url).json()
+
+    def projects_by_billing_tag(
+        self,
+        billing_tag: Optional[str] = None,
+        offset: Optional[int] = 0,
+        page_size: Optional[int] = 10,
+        name_filter: Optional[str] = None,
+        sort_by: Optional[str] = None,
+        sort_order: Optional[str] = None,
+        missing_tag_only: bool = False,
+    ) -> dict:
+        """
+        Remove a billing tag from a specified project
+        Requires Admin permission
+
+        :param billing_tag: billing tag string to filter projects by
+        :param offset: The index of the start of the page, where checkpointProjectId is index 0.
+                        If the offset is negative the project it points to will be the end of the page.
+        :param page_size: The number of record to return per page.
+        :param name_filter: matches projects by name substring
+        :param sort_by: (Optional) field to sort the projects on
+        :param sort_order: (Optional) Whether to sort in asc or desc order
+        :param missing_tag_only: (Optional) determine whether to only return projects with missing tag
+
+        :return: Returns a dictionary containing a page with the projects matching the query based on the page_size,
+                 and to total count of projects aching the query
+        """
+
+        parameters = {
+            "offset": offset,
+            "pageSize": page_size,
+            "missingBillingTagOnly": str(missing_tag_only).lower()
+        }
+
+        optional_params = {
+            "billingTag": billing_tag,
+            "nameFilter": name_filter,
+            "sortBy": sort_by,
+            "sortOrder": sort_order,
+        }
+
+        updated_params = self._update_if_set(parameters, optional_params)
+
+        url = self._routes.projects_billing_tags()
+
+        return self.request_manager.get(url, params=updated_params).json()
+
+    def project_billing_tag_bulk_update(self, projects_tag: dict[str, str]) -> dict:
+        """
+        Update project's billing tags in bulk
+        Requires Admin permission
+
+        :param projects_tag: dictionary of project_id and billing_tags
+
+        :return: Returns the updated projects detail summary
+        """
+        value_list = []
+        for key, value in projects_tag.items():
+            value_list.append(
+                {
+                    "projectId": key,
+                    "billingTag": {
+                        "tag": value
+                    }
+                }
+            )
+
+        data = {
+            "projectsBillingTags": value_list
+        }
+
+        url = self._routes.projects_billing_tags()
+        return self.request_manager.post(url, data=json.dumps(data)).json()
 
     _CUSTOM_METRICS_USE_GEN = True
 
     def custom_metrics_client(self) -> _CustomMetricsClientBase:
         self.requires_at_least("5.3.1")
         if self._CUSTOM_METRICS_USE_GEN:
             return _CustomMetricsClientGen(self, self._routes)
         else:
             return _CustomMetricsClient(self, self._routes)
 
-
     # Validation methods
     def _useable_environments_list(self):
         self.log.debug("Getting list of useable environment")
         useable_environment_list_url = self._routes.useable_environments_list(
             self.project_id
         )
         return self.request_manager.get(useable_environment_list_url).json()[
@@ -1310,14 +1682,31 @@
         except KeyError:
             raise Exception(
                 "Information value is formatted incorrectly."
                 + f" Allowed units: {', '.join(accepted_units.keys())}"
                 + " Example: { 'unit': 'GiB', 'value': 5 }"
             )
 
+    @staticmethod
+    def _generate_budget(budget_label: BudgetLabel, budget_id: str, budget_limit: float) -> dict:
+        return {
+            "limit": budget_limit,
+            "labelId": budget_id,
+            "window": "monthly",
+            "budgetLabel": budget_label.value,
+            "budgetType": BudgetType.OVERRIDE.value
+        }
+
+    @staticmethod
+    def _update_if_set(update_dict: dict, new_dict: dict) -> dict:
+        for key, value in new_dict.items():
+            if value is not None:
+                update_dict[key] = value
+        return update_dict
+
     def requires_at_least(self, at_least_version):
         if version.parse(at_least_version) > version.parse(self._version):
             raise Exception(
                 f"You need at least version {at_least_version} but your deployment seems to be running {self._version}"
             )
         return True
```

### Comparing `dominodatalab-1.3.1/domino/exceptions.py` & `dominodatalab-1.4.0/domino/exceptions.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/helpers.py` & `dominodatalab-1.4.0/domino/helpers.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/http_request_manager.py` & `dominodatalab-1.4.0/domino/http_request_manager.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/domino/routes.py` & `dominodatalab-1.4.0/domino/routes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import warnings
 
 from urllib.parse import quote
 
+from typing import Optional
+
 
 class _Routes:
     def __init__(self, host, owner_username, project_name):
         self.host = host
         self._owner_username = owner_username
         self._project_name = project_name
 
@@ -32,24 +34,20 @@
     def _build_models_v4_url(self):
         return self.host + "/v4/models"
 
     # Project URLs
     def project_create(self):
         return self.host + "/project"
 
-    def project_archive(self, project_id):
-        return f"{self.host}/v4/projects/{project_id}"
+    def project_v4(self, project_id: Optional[str] = None) -> str:
+        return self.host + "/v4/projects" + (f"/{project_id}" if project_id else "")
 
     def projects_list(self):
         return f"{self.host}/v4/gateway/projects"
 
-    # tags URLs
-    def tags_list(self, project_id):
-        return f"{self.host}/v4/projects/{project_id}"
-
     def tag_details(self, tag_id):
         return f"{self.host}/projectTags/{tag_id}"
 
     def tags_add(self, project_id):
         return f"{self.host}/v4/projects/{project_id}/tags"
 
     def tags_remove(self, project_id, tag_id):
@@ -287,9 +285,35 @@
     def find_project_by_owner_name_and_project_name_url(self):
         return (
             f"{self.host}/v4/gateway/projects/findProjectByOwnerAndName"
             f"?ownerName={self._owner_username}&projectName={self._project_name}"
         )
 
     # User URLs
-    def users_get(self):
+    def users_get(self) -> str:
         return self.host + "/v4/users"
+
+    # Budgets and Billing Tags
+    def budget_settings(self) -> str:
+        return self.host + "/v4/cost/budgets/global/alertsSettings"
+
+    def budgets_default(self, budget_label: Optional[str] = None) -> str:
+        label = f"/{budget_label}" if budget_label else ""
+        return self.host + f"/v4/cost/budgets/defaults{label}"
+
+    def budget_overrides(self, override_id: Optional[str] = None) -> str:
+        override = f"/{override_id}" if override_id else ""
+        return self.host + f"/v4/cost/budgets/overrides{override}"
+
+    def billing_tags_settings(self, mode_only: Optional[bool] = False) -> str:
+        mode_str = "/mode" if mode_only else ""
+        return self.host + "/v4/cost/billingtagSettings" + mode_str
+
+    def billing_tags(self, name: Optional[str] = None) -> str:
+        optional_name = f"/{name}" if name else ""
+        return self.host + "/v4/cost/billingtags" + optional_name
+
+    def project_billing_tag(self, project_id: Optional[str] = None) -> str:
+        return self.host + f"/v4/projects/{project_id}/billingtag"
+
+    def projects_billing_tags(self):
+        return self.host + "/v4/projects/billingtags/projects"
```

### Comparing `dominodatalab-1.3.1/domino/training_sets.py` & `dominodatalab-1.4.0/domino/training_sets.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/dominodatalab.egg-info/PKG-INFO` & `dominodatalab-1.4.0/dominodatalab.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dominodatalab
-Version: 1.3.1
+Version: 1.4.0
 Summary: Python bindings for the Domino API
 Home-page: https://github.com/dominodatalab/python-domino
-Download-URL: https://github.com/dominodatalab/python-domino/archive/release-1.3.1.zip
+Download-URL: https://github.com/dominodatalab/python-domino/archive/release-1.4.0.zip
 Author: Domino Data Lab
 Author-email: support@dominodatalab.com
 License: Apache Software License (Apache 2.0)
 Keywords: Domino Data Lab,API
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -43,28 +43,29 @@
 See this documentation for details about the APIs:
 
 -   [Latest public Domino
     APIs](https://docs.dominodatalab.com/en/latest/api_guide/8c929e/domino-public-apis/)
 
 -   [Legacy APIs](https://dominodatalab.github.io/api-docs/)
 
-The latest released version of `python-domino` is `1.3.1`.
+The latest released version of `python-domino` is `1.4.0`.
 
 # Version compatibility matrix
 
 The `python-domino` library is compatible with different versions of
 Domino:
 
 | Domino Versions |                                    Python-Domino                                    |
 |-----------------|:-----------------------------------------------------------------------------------:|
 | 3.6.x or lower  |      [0.3.5](https://github.com/dominodatalab/python-domino/archive/0.3.5.zip)       |
 | 4.1.0 or higher | [1.0.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/1.0.0.zip) or Higher |
 | 5.3.0 or higher | [1.2.0]https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.0.zip) or Higher |
 | 5.5.0 or higher | [1.2.2](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.2.zip) or Higher |
 | 5.10.0 or higher | [1.3.1](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.3.1.zip) or Higher |
+| 5.11.0 or higher | [1.4.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.4.0.zip) or Higher |
 
 # Development
 
 The current `python-domino` is based on Python 3.9, which is therefore recommended for development. `Pipenv` is also recommended to manage the dependencies.
 
 To use the Python binding in a Domino workbook session, include `dominodatalab` in your project's requirements.txt file.
 This makes the Python binding available for each new workbook session (or batch run) started within the project.
@@ -143,20 +144,212 @@
     
     Default Retry is set to 4 
     Determines the number of attempts for the request session in case of a ConnectionError
     Get more info on request max timeout/error durations based on Retry and backoff factors [here](https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry)
 
 # Methods
 
+# Budgets and Billing Tags
+
+See
+[`example_budget_manager.py`](https://github.com/dominodatalab/python-domino/blob/release-1.4.0/examples/example_budget_manager.py)
+for example code.
+
+### budget_defaults_list()
+
+Get a list of the available default budgets with the assigned (if any) limits
+Requires Admin permission
+
+### budget_defaults_update(budget_label, budget_limit)
+
+Update default budgets by BudgetLabel
+Requires Admin roles
+
+-   *budget_label:* (required) label of budget to be updated ex: `BillingTag`, `Organization`
+
+-   *budget_limit:* (required) new budget quota to assign to default label
+
+### budget_overrides_list()
+
+Get a list of the available budgets overrides with the assigned limits.
+Requires Admin permission
+
+### budget_override_create(budget_label, budget_id, budget_limit)
+
+Create Budget overrides based on BudgetLabels, ie BillingTags, Organization, or Projects
+the object id is used as budget ids
+Requires Admin roles
+
+-   *budget_label:* label of budget to be updated
+
+-   *budget_id:* id of project or organization to be used as new budget override id.
+
+-   *budget_limit:* budget quota to assign to override
+
+### budget_override_update(budget_label, budget_id, budget_limit)
+
+Update Budget overrides based on BudgetLabel and budget id
+Requires Admin roles
+
+-   *budget_label:* label of budget to be updated
+
+-   *budget_id:* id of budget override to be updated.
+
+-   *budget_limit:* new budget quota to assign to override
+
+### budget_override_delete(budget_id)
+
+Delete an existing budget override
+Requires Admin roles
+
+-   *budget_id:* id of budget override to be deleted.
+
+### budget_alerts_settings()
+
+Get the current budget alerts settings
+Requires Admin permission
+
+### budget_alerts_settings_update(alerts_enabled, notify_org_owner)
+
+Update the current budget alerts settings to enable/disable budget notifications
+and whether to notify org owners on projects notifications
+Requires Admin permission
+
+-   *alerts_enabled:* whether to enable or disable notifications.
+
+-   *notify_org_owner:* whether to notify organizations owners on projects reaching threshold.
+
+### budget_alerts_targets_update(targets)
+
+Update the current budget alerts settings with additional email targets per budget label
+Requires Admin permission
+
+-   *targets:* dictionary of budget labels and list of email addresses
+
+### billing_tags_list_active()
+
+Get a list of active billing tags
+Requires Admin permission
+
+### billing_tags_create(tags_list)
+
+Create a list of active billing tags
+Requires Admin permission
+
+-   *tags_list:* list of billing tags names to be created
+
+### active_billing_tag_by_name(name)
+
+Get detailed info on active or archived billing tag
+Requires Admin permission
+
+-   *name:* name of existing billing tag
+
+### billing_tag_archive(name)
+
+Archive an active billing tag
+Requires Admin permission
+
+-   *name:* name of existing billing tag to archive
+
+### billing_tag_settings()
+
+Get the current billing tag settings
+Requires Admin permission
+
+### billing_tag_settings_mode()
+
+Get the current billing tag settings mode
+Requires Admin permission
+
+### billing_tag_settings_mode_update(mode)
+
+Update the current billing tag settings mode
+Requires Admin permission
+
+-   *mode:* new mode to set the billing tag settings (see BillingTagSettingMode)
+
+### project_billing_tag(project_id)
+
+Get a billing tag assigned to a particular project by project id
+Requires Admin permission
+
+-   *project_id:* id of the project to find assigned billing tag
+
+###  project_billing_tag_update(billing_tag, project_id)
+
+Update project's billing tag with new billing tag.
+Requires Admin permission
+
+-   *billing_tag:* billing tag to assign to a project
+
+-   *project_id:* id of the project to assign a billing tag
+
+### project_billing_tag_reset(project_id)
+
+Remove a billing tag from a specified project
+Requires Admin permission
+
+-   *project_id:* id of the project to reset billing tag field
+
+### projects_by_billing_tag( billing_tag, offset, page_size, name_filter, sort_by, sort_order, missing_tag_only=False)
+
+Remove a billing tag from a specified project
+Requires Admin permission
+
+-   *billing_tag:* billing tag string to filter projects by
+
+-   *offset:* The index of the start of the page, where checkpointProjectId is index 0.
+If the offset is negative the project it points to will be the end of the page.
+-   *page_size:* The number of records to return per page.
+
+-   *name_filter:* matches projects by name substring
+
+-   *sort_by:* (Optional) field to sort the projects on
+
+-   *sort_order:* (Optional) Whether to sort in asc or desc order
+
+-   *missing_tag_only:* (Optional) determine whether to only return projects with missing tag
+
+### project_billing_tag_bulk_update(projects_tag)
+
+Update project's billing tags in bulk
+Requires Admin permission
+
+-   *projects_tag:* dictionary of project_id and billing_tags
+
+
 ## Projects
 
 See
 [`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/example_projects_usage.py)
 for example code.
 
+### project_create_v4(project_name, owner_id, owner_username, description, collaborators, tags, billing_tag, visibility=PUBLIC)
+
+Newer version of projects creation using the v4 endpoints which allows more optional fields.
+
+-   *project_name:* (required) The name of the project.
+
+-   *owner_id:* (Optional) user id of the owner of the new project to be created (must be admin to create projects for other users)
+  owner_id or owner_username can be used, both are not needed (Defaults to current owner_username)
+
+-   *owner_username:* (Optional) username of the owner of the new project to be created (must be admin to create projects for other users)
+  owner_id or owner_username can be used, both are not needed (Defaults to current owner_username)
+
+-   *description:* (Optional) description of the project
+
+-   *collaborators:* (Optional) list of collaborators to be added to the project
+
+-   *tags:* (Optional) list of tags to add to project
+
+-   *billing_tag:* (Optional unless billingTag settings mode is Required) active billing tag to be added to projects for governance
+
+-   *visibility:* (Optional) (Defaults to Public) project visibility 
+
 ### project_create(project_name, owner_username=None)
 
 Create a new project with given project name.
 
 -   *project_name:* The name of the project.
 
 -   *owner_username:* (Optional) The owner username for the project.
```

### Comparing `dominodatalab-1.3.1/dominodatalab.egg-info/SOURCES.txt` & `dominodatalab-1.4.0/dominodatalab.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 domino/_custom_metrics.py
 domino/_version.py
 domino/authentication.py
 domino/constants.py
 domino/data_sources.py
 domino/datasets.py
 domino/domino.py
+domino/domino_enums.py
 domino/exceptions.py
 domino/helpers.py
 domino/http_request_manager.py
 domino/routes.py
 domino/training_sets.py
 domino/_impl/__init__.py
 domino/_impl/custommetrics/__init__.py
@@ -72,13 +73,14 @@
 dominodatalab.egg-info/requires.txt
 dominodatalab.egg-info/top_level.txt
 tests/test_basic_auth.py
 tests/test_data_sources.py
 tests/test_datasets.py
 tests/test_domino.py
 tests/test_environments.py
+tests/test_finops.py
 tests/test_jobs.py
 tests/test_models.py
 tests/test_no_data_sources.py
 tests/test_operator.py
 tests/test_projects.py
 tests/test_spark_operator.py
```

### Comparing `dominodatalab-1.3.1/requirements.txt` & `dominodatalab-1.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/setup.py` & `dominodatalab-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/tests/test_basic_auth.py` & `dominodatalab-1.4.0/tests/test_basic_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,29 +86,29 @@
 
     d = Domino(host=dummy_host, project="anyuser/quick-start", api_key=dummy_api_key)
     assert isinstance(
         d.request_manager.auth, requests.auth.HTTPBasicAuth
     ), "Authentication using API key should be of type requests.auth.HTTPBasicAuth"
 
 
-@pytest.mark.usefixtures("mock_domino_version_response", "clear_token_file_from_env")
+@pytest.mark.usefixtures("mock_domino_version_response", "clear_token_file_from_env", "mock_proxy_response")
 def test_object_creation_with_api_proxy():
     """
     Confirm that the expected auth type is used when using api proxy.
     """
     dummy_host = "http://domino.somefakecompany.com"
     dummy_api_proxy = "localhost:1234"
 
     d = Domino(host=dummy_host, project="anyuser/quick-start", api_proxy=dummy_api_proxy)
     assert isinstance(
         d.request_manager.auth, domino.authentication.ProxyAuth
     ), "Authentication using API proxy should be of type domino.authentication.ProxyAuth"
     assert d.request_manager.auth.api_proxy == "http://localhost:1234"
 
-@pytest.mark.usefixtures("mock_domino_version_response", "clear_token_file_from_env")
+@pytest.mark.usefixtures("mock_domino_version_response", "clear_token_file_from_env", "mock_proxy_response_https")
 def test_object_creation_with_api_proxy_with_scheme():
     """
     Confirm that the expected auth type is used when using api proxy.
     """
     dummy_host = "http://domino.somefakecompany.com"
     dummy_api_proxy = "https://localhost:1234"
```

### Comparing `dominodatalab-1.3.1/tests/test_data_sources.py` & `dominodatalab-1.4.0/tests/test_data_sources.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/tests/test_datasets.py` & `dominodatalab-1.4.0/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/tests/test_domino.py` & `dominodatalab-1.4.0/tests/test_domino.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 import os
 import pytest
 import time
-from requests.auth import AuthBase
 
 from domino import Domino
 from domino.http_request_manager import _HttpRequestManager
 
 os.environ["DOMINO_MAX_RETRIES"] = "3"
 
-class TestAuth(AuthBase):
-     def __init__(self, *args, **kwargs):
-         super(TestAuth, self).__init__(*args, **kwargs)
-         self.header = None
-
 
 def test_versioning(requests_mock, dummy_hostname):
     """validates domino version checking is correct"""
 
     # Mock a typical response from the jobs status API endpoint (GET)
     requests_mock.get(f"{dummy_hostname}/version", json={"version": "5.10.0"})
 
@@ -24,16 +18,16 @@
 
     dep_version = dom.deployment_version().get("version")
     assert dep_version == "5.10.0"
     assert dom.requires_at_least("5.3.0")
     with pytest.raises(Exception):
         dom.requires_at_least("5.11.0")
 
-def test_request_session():
-     request_manager = _HttpRequestManager(auth=TestAuth())
+def test_request_session(test_auth_base):
+     request_manager = _HttpRequestManager(auth=test_auth_base)
      start_time = time.time()
      try:
          response = request_manager.request_session.get(
              'https://localhost:9999' # ConnectionError
          )
      except Exception as ex:
          print('It failed :(', ex.__class__.__name__)
```

### Comparing `dominodatalab-1.3.1/tests/test_environments.py` & `dominodatalab-1.4.0/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/tests/test_jobs.py` & `dominodatalab-1.4.0/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/tests/test_models.py` & `dominodatalab-1.4.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/tests/test_operator.py` & `dominodatalab-1.4.0/tests/test_operator.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/tests/test_projects.py` & `dominodatalab-1.4.0/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.1/tests/test_spark_operator.py` & `dominodatalab-1.4.0/tests/test_spark_operator.py`

 * *Files identical despite different names*

