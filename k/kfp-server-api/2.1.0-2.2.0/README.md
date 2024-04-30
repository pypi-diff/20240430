# Comparing `tmp/kfp-server-api-2.1.0.tar.gz` & `tmp/kfp-server-api-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-server-api-2.1.0.tar", last modified: Mon Mar 25 20:38:35 2024, max compression
+gzip compressed data, was "kfp-server-api-2.2.0.tar", last modified: Tue Apr 30 21:26:00 2024, max compression
```

## Comparing `kfp-server-api-2.1.0.tar` & `kfp-server-api-2.2.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 chesu    (630462) primarygroup (89939)        0 2024-03-25 20:38:35.004035 kfp-server-api-2.1.0/
--rw-r-----   0 chesu    (630462) primarygroup (89939)    11357 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/LICENSE
--rw-r--r--   0 chesu    (630462) primarygroup (89939)      444 2024-03-25 20:38:35.004035 kfp-server-api-2.1.0/PKG-INFO
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    14706 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/README.md
-drwxr-xr-x   0 chesu    (630462) primarygroup (89939)        0 2024-03-25 20:38:34.908029 kfp-server-api-2.1.0/kfp_server_api/
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5024 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/__init__.py
-drwxr-xr-x   0 chesu    (630462) primarygroup (89939)        0 2024-03-25 20:38:34.916030 kfp-server-api-2.1.0/kfp_server_api/api/
--rw-r--r--   0 chesu    (630462) primarygroup (89939)      738 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/api/__init__.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     6318 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/api/auth_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    36994 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/api/experiment_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5454 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/api/healthz_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    64610 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/api/pipeline_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    14031 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/api/pipeline_upload_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    38033 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/api/recurring_run_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    12076 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/api/report_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    55691 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/api/run_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     7277 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/api/visualization_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    26250 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/api_client.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    13302 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/configuration.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3795 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/exceptions.py
-drwxr-xr-x   0 chesu    (630462) primarygroup (89939)        0 2024-03-25 20:38:34.960032 kfp-server-api-2.1.0/kfp_server_api/models/
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3937 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/models/__init__.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2926 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/kfp_server_api/models/authorize_request_resources.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2939 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/kfp_server_api/models/authorize_request_verb.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5603 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/kfp_server_api/models/googlerpc_status.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     4512 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/kfp_server_api/models/pipeline_task_detail_child_task.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3379 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/kfp_server_api/models/predicate_int_values.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3387 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/kfp_server_api/models/predicate_long_values.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3403 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/kfp_server_api/models/predicate_string_values.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     7241 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/kfp_server_api/models/protobuf_any.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2831 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/kfp_server_api/models/protobuf_null_value.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2908 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/kfp_server_api/models/recurring_run_mode.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5206 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/models/runtime_error.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3623 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_artifact_list.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     4594 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_create_pipeline_and_version_request.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     4999 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_cron_schedule.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     8164 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_experiment.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2999 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_experiment_storage_state.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3616 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_filter.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3616 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_get_healthz_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5673 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_list_experiments_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5922 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_list_pipeline_versions_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5687 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_list_pipelines_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5803 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_list_recurring_runs_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5361 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_list_runs_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5544 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_periodic_schedule.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     8024 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_pipeline.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    17041 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_pipeline_task_detail.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     8131 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_pipeline_task_executor_detail.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    11389 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_pipeline_version.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     4853 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_pipeline_version_reference.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    10093 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_predicate.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3250 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_predicate_operation.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3903 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_read_artifact_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    19695 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_recurring_run.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2956 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_recurring_run_status.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    18975 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_run.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5847 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_run_details.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2971 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_run_storage_state.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     4566 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_runtime_config.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3157 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_runtime_state.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     4949 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_runtime_status.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     4447 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_trigger.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3547 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_url.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     7294 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_visualization.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2961 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_visualization_type.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    12327 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/kfp_server_api/rest.py
-drwxr-xr-x   0 chesu    (630462) primarygroup (89939)        0 2024-03-25 20:38:34.912029 kfp-server-api-2.1.0/kfp_server_api.egg-info/
--rw-r--r--   0 chesu    (630462) primarygroup (89939)      444 2024-03-25 20:38:34.000000 kfp-server-api-2.1.0/kfp_server_api.egg-info/PKG-INFO
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     4985 2024-03-25 20:38:34.000000 kfp-server-api-2.1.0/kfp_server_api.egg-info/SOURCES.txt
--rw-r--r--   0 chesu    (630462) primarygroup (89939)        1 2024-03-25 20:38:34.000000 kfp-server-api-2.1.0/kfp_server_api.egg-info/dependency_links.txt
--rw-r--r--   0 chesu    (630462) primarygroup (89939)       48 2024-03-25 20:38:34.000000 kfp-server-api-2.1.0/kfp_server_api.egg-info/requires.txt
--rw-r--r--   0 chesu    (630462) primarygroup (89939)       15 2024-03-25 20:38:34.000000 kfp-server-api-2.1.0/kfp_server_api.egg-info/top_level.txt
--rw-r--r--   0 chesu    (630462) primarygroup (89939)       69 2024-03-25 20:38:35.004035 kfp-server-api-2.1.0/setup.cfg
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1190 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/setup.py
-drwxr-xr-x   0 chesu    (630462) primarygroup (89939)        0 2024-03-25 20:38:35.000035 kfp-server-api-2.1.0/test/
--rw-r--r--   0 chesu    (630462) primarygroup (89939)      875 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/test/test_auth_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1511 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/test/test_authorize_request_resources.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1456 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/test/test_authorize_request_verb.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2302 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/test/test_experiment_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1660 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/test/test_googlerpc_status.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)      943 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/test/test_healthz_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3012 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/test/test_pipeline_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1600 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/test/test_pipeline_task_detail_child_task.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1043 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_pipeline_upload_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1506 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/test/test_predicate_int_values.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1518 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/test/test_predicate_long_values.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1540 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/test/test_predicate_string_values.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1419 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/test/test_protobuf_any.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1423 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/test/test_protobuf_null_value.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1412 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/test/test_recurring_run_mode.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2354 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/test/test_recurring_run_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1057 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/test/test_report_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2632 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/test/test_run_service_api.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1657 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/test/test_runtime_error.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1524 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/test/test_v2beta1_artifact_list.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3479 2023-08-17 21:44:56.000000 kfp-server-api-2.1.0/test/test_v2beta1_create_pipeline_and_version_request.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1686 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_cron_schedule.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1734 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_experiment.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1557 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_experiment_storage_state.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2288 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_filter.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1547 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_get_healthz_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2140 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_list_experiments_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2868 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_list_pipeline_versions_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2478 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_list_pipelines_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     4554 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_list_recurring_runs_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     6835 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_list_runs_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1741 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_periodic_schedule.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2022 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_pipeline.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     4402 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_pipeline_task_detail.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1863 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_pipeline_task_executor_detail.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2357 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_pipeline_version.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1657 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_pipeline_version_reference.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2265 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_predicate.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1511 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_predicate_operation.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1565 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_read_artifact_response.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3876 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_recurring_run.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1513 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_recurring_run_status.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     6934 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_run.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     4315 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_run_details.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1480 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_run_storage_state.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1580 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_runtime_config.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1445 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_runtime_state.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1991 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_runtime_status.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2119 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_trigger.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1379 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_url.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1613 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_visualization.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1500 2023-08-17 21:44:57.000000 kfp-server-api-2.1.0/test/test_v2beta1_visualization_type.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)      975 2024-03-25 17:57:09.000000 kfp-server-api-2.1.0/test/test_visualization_service_api.py
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2024-04-30 21:26:00.164387 kfp-server-api-2.2.0/
+-rw-r-----   0 chesu    (630462) primarygroup (89939)    11357 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/LICENSE
+-rw-r-----   0 chesu    (630462) primarygroup (89939)      444 2024-04-30 21:26:00.164387 kfp-server-api-2.2.0/PKG-INFO
+-rw-r-----   0 chesu    (630462) primarygroup (89939)    14706 2024-04-30 21:25:33.000000 kfp-server-api-2.2.0/README.md
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2024-04-30 21:26:00.128384 kfp-server-api-2.2.0/kfp_server_api/
+-rw-r-----   0 chesu    (630462) primarygroup (89939)     5024 2024-04-30 21:25:33.000000 kfp-server-api-2.2.0/kfp_server_api/__init__.py
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2024-04-30 21:26:00.136385 kfp-server-api-2.2.0/kfp_server_api/api/
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      738 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/api/__init__.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     6318 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/kfp_server_api/api/auth_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    36994 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/kfp_server_api/api/experiment_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5454 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/kfp_server_api/api/healthz_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    64610 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/kfp_server_api/api/pipeline_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    14031 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/api/pipeline_upload_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    38033 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/kfp_server_api/api/recurring_run_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    12076 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/kfp_server_api/api/report_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    55691 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/kfp_server_api/api/run_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     7277 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/kfp_server_api/api/visualization_service_api.py
+-rw-r-----   0 chesu    (630462) primarygroup (89939)    26250 2024-04-30 21:25:33.000000 kfp-server-api-2.2.0/kfp_server_api/api_client.py
+-rw-r-----   0 chesu    (630462) primarygroup (89939)    13302 2024-04-30 21:25:33.000000 kfp-server-api-2.2.0/kfp_server_api/configuration.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3795 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/exceptions.py
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2024-04-30 21:26:00.144385 kfp-server-api-2.2.0/kfp_server_api/models/
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3937 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/kfp_server_api/models/__init__.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2926 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/kfp_server_api/models/authorize_request_resources.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2939 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/kfp_server_api/models/authorize_request_verb.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5603 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/kfp_server_api/models/googlerpc_status.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4512 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/kfp_server_api/models/pipeline_task_detail_child_task.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3379 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/kfp_server_api/models/predicate_int_values.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3387 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/kfp_server_api/models/predicate_long_values.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3403 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/kfp_server_api/models/predicate_string_values.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     7241 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/kfp_server_api/models/protobuf_any.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2831 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/kfp_server_api/models/protobuf_null_value.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2908 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/kfp_server_api/models/recurring_run_mode.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5206 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/kfp_server_api/models/runtime_error.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3623 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_artifact_list.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4594 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_create_pipeline_and_version_request.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4999 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_cron_schedule.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     8164 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_experiment.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2999 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_experiment_storage_state.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3616 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_filter.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3616 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_get_healthz_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5673 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_list_experiments_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5922 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_list_pipeline_versions_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5687 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_list_pipelines_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5803 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_list_recurring_runs_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5361 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_list_runs_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5544 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_periodic_schedule.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     8024 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_pipeline.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    17041 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_pipeline_task_detail.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     8131 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_pipeline_task_executor_detail.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    11389 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_pipeline_version.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4853 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_pipeline_version_reference.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    10093 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_predicate.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3250 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_predicate_operation.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3903 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_read_artifact_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    19695 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_recurring_run.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2956 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_recurring_run_status.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    18975 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_run.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     5847 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_run_details.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2971 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_run_storage_state.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4566 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_runtime_config.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3157 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_runtime_state.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4949 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_runtime_status.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4447 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_trigger.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3547 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_url.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     7294 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_visualization.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2961 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_visualization_type.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)    12327 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/kfp_server_api/rest.py
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2024-04-30 21:26:00.132384 kfp-server-api-2.2.0/kfp_server_api.egg-info/
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      444 2024-04-30 21:25:59.000000 kfp-server-api-2.2.0/kfp_server_api.egg-info/PKG-INFO
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4985 2024-04-30 21:25:59.000000 kfp-server-api-2.2.0/kfp_server_api.egg-info/SOURCES.txt
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)        1 2024-04-30 21:25:59.000000 kfp-server-api-2.2.0/kfp_server_api.egg-info/dependency_links.txt
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)       48 2024-04-30 21:25:59.000000 kfp-server-api-2.2.0/kfp_server_api.egg-info/requires.txt
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)       15 2024-04-30 21:25:59.000000 kfp-server-api-2.2.0/kfp_server_api.egg-info/top_level.txt
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)       69 2024-04-30 21:26:00.164387 kfp-server-api-2.2.0/setup.cfg
+-rw-r-----   0 chesu    (630462) primarygroup (89939)     1190 2024-04-30 21:25:33.000000 kfp-server-api-2.2.0/setup.py
+drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2024-04-30 21:26:00.164387 kfp-server-api-2.2.0/test/
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      875 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/test/test_auth_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1511 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/test/test_authorize_request_resources.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1456 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/test/test_authorize_request_verb.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2302 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/test/test_experiment_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1660 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/test/test_googlerpc_status.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      943 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/test/test_healthz_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3012 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/test/test_pipeline_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1600 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/test/test_pipeline_task_detail_child_task.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1043 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_pipeline_upload_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1506 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/test/test_predicate_int_values.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1518 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/test/test_predicate_long_values.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1540 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/test/test_predicate_string_values.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1419 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/test/test_protobuf_any.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1423 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/test/test_protobuf_null_value.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1412 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/test/test_recurring_run_mode.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2354 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/test/test_recurring_run_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1057 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/test/test_report_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2632 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/test/test_run_service_api.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1657 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/test/test_runtime_error.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1524 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/test/test_v2beta1_artifact_list.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3479 2023-08-17 21:44:56.000000 kfp-server-api-2.2.0/test/test_v2beta1_create_pipeline_and_version_request.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1686 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_cron_schedule.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1734 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_experiment.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1557 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_experiment_storage_state.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2288 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_filter.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1547 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_get_healthz_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2140 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_list_experiments_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2868 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_list_pipeline_versions_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2478 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_list_pipelines_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4554 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_list_recurring_runs_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     6835 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_list_runs_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1741 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_periodic_schedule.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2022 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_pipeline.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4402 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_pipeline_task_detail.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1863 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_pipeline_task_executor_detail.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2357 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_pipeline_version.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1657 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_pipeline_version_reference.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2265 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_predicate.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1511 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_predicate_operation.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1565 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_read_artifact_response.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     3876 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_recurring_run.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1513 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_recurring_run_status.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     6934 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_run.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     4315 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_run_details.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1480 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_run_storage_state.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1580 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_runtime_config.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1445 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_runtime_state.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1991 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_runtime_status.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     2119 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_trigger.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1379 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_url.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1613 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_visualization.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)     1500 2023-08-17 21:44:57.000000 kfp-server-api-2.2.0/test/test_v2beta1_visualization_type.py
+-rw-r--r--   0 chesu    (630462) primarygroup (89939)      975 2024-03-25 17:57:09.000000 kfp-server-api-2.2.0/test/test_visualization_service_api.py
```

### Comparing `kfp-server-api-2.1.0/LICENSE` & `kfp-server-api-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/README.md` & `kfp-server-api-2.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # kfp-server-api
 This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.1.0
-- Package version: 2.1.0
+- API version: 2.2.0
+- Package version: 2.2.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.google.com](https://www.google.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `kfp-server-api-2.1.0/kfp_server_api/__init__.py` & `kfp-server-api-2.2.0/kfp_server_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 
 # import apis into sdk package
 from kfp_server_api.api.auth_service_api import AuthServiceApi
 from kfp_server_api.api.experiment_service_api import ExperimentServiceApi
 from kfp_server_api.api.healthz_service_api import HealthzServiceApi
 from kfp_server_api.api.pipeline_service_api import PipelineServiceApi
 from kfp_server_api.api.pipeline_upload_service_api import PipelineUploadServiceApi
```

### Comparing `kfp-server-api-2.1.0/kfp_server_api/api/__init__.py` & `kfp-server-api-2.2.0/kfp_server_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/api/auth_service_api.py` & `kfp-server-api-2.2.0/kfp_server_api/api/auth_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/api/experiment_service_api.py` & `kfp-server-api-2.2.0/kfp_server_api/api/experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/api/healthz_service_api.py` & `kfp-server-api-2.2.0/kfp_server_api/api/healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/api/pipeline_service_api.py` & `kfp-server-api-2.2.0/kfp_server_api/api/pipeline_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/api/pipeline_upload_service_api.py` & `kfp-server-api-2.2.0/kfp_server_api/api/pipeline_upload_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/api/recurring_run_service_api.py` & `kfp-server-api-2.2.0/kfp_server_api/api/recurring_run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/api/report_service_api.py` & `kfp-server-api-2.2.0/kfp_server_api/api/report_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/api/run_service_api.py` & `kfp-server-api-2.2.0/kfp_server_api/api/run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/api/visualization_service_api.py` & `kfp-server-api-2.2.0/kfp_server_api/api/visualization_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/api_client.py` & `kfp-server-api-2.2.0/kfp_server_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.1.0/python'
+        self.user_agent = 'OpenAPI-Generator/2.2.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kfp-server-api-2.1.0/kfp_server_api/configuration.py` & `kfp-server-api-2.2.0/kfp_server_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,16 +347,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.1.0\n"\
-               "SDK Package Version: 2.1.0".\
+               "Version of the API: 2.2.0\n"\
+               "SDK Package Version: 2.2.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `kfp-server-api-2.1.0/kfp_server_api/exceptions.py` & `kfp-server-api-2.2.0/kfp_server_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/__init__.py` & `kfp-server-api-2.2.0/kfp_server_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/authorize_request_resources.py` & `kfp-server-api-2.2.0/kfp_server_api/models/authorize_request_resources.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/authorize_request_verb.py` & `kfp-server-api-2.2.0/kfp_server_api/models/authorize_request_verb.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/googlerpc_status.py` & `kfp-server-api-2.2.0/kfp_server_api/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/pipeline_task_detail_child_task.py` & `kfp-server-api-2.2.0/kfp_server_api/models/pipeline_task_detail_child_task.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/predicate_int_values.py` & `kfp-server-api-2.2.0/kfp_server_api/models/predicate_int_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/predicate_long_values.py` & `kfp-server-api-2.2.0/kfp_server_api/models/predicate_long_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/predicate_string_values.py` & `kfp-server-api-2.2.0/kfp_server_api/models/predicate_string_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/protobuf_any.py` & `kfp-server-api-2.2.0/kfp_server_api/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/protobuf_null_value.py` & `kfp-server-api-2.2.0/kfp_server_api/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/recurring_run_mode.py` & `kfp-server-api-2.2.0/kfp_server_api/models/recurring_run_mode.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/runtime_error.py` & `kfp-server-api-2.2.0/kfp_server_api/models/runtime_error.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_artifact_list.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_artifact_list.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_create_pipeline_and_version_request.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_create_pipeline_and_version_request.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_cron_schedule.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_cron_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_experiment.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_experiment_storage_state.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_filter.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_filter.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_get_healthz_response.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_get_healthz_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_list_experiments_response.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_list_pipeline_versions_response.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_list_pipeline_versions_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_list_pipelines_response.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_list_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_list_recurring_runs_response.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_list_recurring_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_list_runs_response.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_list_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_periodic_schedule.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_pipeline.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_pipeline_task_detail.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_pipeline_task_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_pipeline_task_executor_detail.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_pipeline_task_executor_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_pipeline_version.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_pipeline_version.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_pipeline_version_reference.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_pipeline_version_reference.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_predicate.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_predicate.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_predicate_operation.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_predicate_operation.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_read_artifact_response.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_read_artifact_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_recurring_run.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_recurring_run.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_recurring_run_status.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_recurring_run_status.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_run.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_run.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_run_details.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_run_details.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_run_storage_state.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_run_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_runtime_config.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_runtime_config.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_runtime_state.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_runtime_state.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_runtime_status.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_runtime_status.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_trigger.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_trigger.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_url.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_url.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_visualization.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_visualization.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/models/v2beta1_visualization_type.py` & `kfp-server-api-2.2.0/kfp_server_api/models/v2beta1_visualization_type.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api/rest.py` & `kfp-server-api-2.2.0/kfp_server_api/rest.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/kfp_server_api.egg-info/SOURCES.txt` & `kfp-server-api-2.2.0/kfp_server_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/setup.py` & `kfp-server-api-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "kfp-server-api"
-VERSION = "2.1.0"
+VERSION = "2.2.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `kfp-server-api-2.1.0/test/test_auth_service_api.py` & `kfp-server-api-2.2.0/test/test_auth_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_authorize_request_resources.py` & `kfp-server-api-2.2.0/test/test_authorize_request_resources.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_authorize_request_verb.py` & `kfp-server-api-2.2.0/test/test_authorize_request_verb.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_experiment_service_api.py` & `kfp-server-api-2.2.0/test/test_experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_googlerpc_status.py` & `kfp-server-api-2.2.0/test/test_googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_healthz_service_api.py` & `kfp-server-api-2.2.0/test/test_healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_pipeline_service_api.py` & `kfp-server-api-2.2.0/test/test_pipeline_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_pipeline_task_detail_child_task.py` & `kfp-server-api-2.2.0/test/test_pipeline_task_detail_child_task.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_pipeline_upload_service_api.py` & `kfp-server-api-2.2.0/test/test_pipeline_upload_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_predicate_int_values.py` & `kfp-server-api-2.2.0/test/test_predicate_int_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_predicate_long_values.py` & `kfp-server-api-2.2.0/test/test_predicate_long_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_predicate_string_values.py` & `kfp-server-api-2.2.0/test/test_predicate_string_values.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_protobuf_any.py` & `kfp-server-api-2.2.0/test/test_protobuf_any.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_protobuf_null_value.py` & `kfp-server-api-2.2.0/test/test_protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_recurring_run_mode.py` & `kfp-server-api-2.2.0/test/test_recurring_run_mode.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_recurring_run_service_api.py` & `kfp-server-api-2.2.0/test/test_recurring_run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_report_service_api.py` & `kfp-server-api-2.2.0/test/test_report_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_run_service_api.py` & `kfp-server-api-2.2.0/test/test_run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_runtime_error.py` & `kfp-server-api-2.2.0/test/test_runtime_error.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_artifact_list.py` & `kfp-server-api-2.2.0/test/test_v2beta1_artifact_list.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_create_pipeline_and_version_request.py` & `kfp-server-api-2.2.0/test/test_v2beta1_create_pipeline_and_version_request.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_cron_schedule.py` & `kfp-server-api-2.2.0/test/test_v2beta1_cron_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_experiment.py` & `kfp-server-api-2.2.0/test/test_v2beta1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_experiment_storage_state.py` & `kfp-server-api-2.2.0/test/test_v2beta1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_filter.py` & `kfp-server-api-2.2.0/test/test_v2beta1_filter.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_get_healthz_response.py` & `kfp-server-api-2.2.0/test/test_v2beta1_get_healthz_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_list_experiments_response.py` & `kfp-server-api-2.2.0/test/test_v2beta1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_list_pipeline_versions_response.py` & `kfp-server-api-2.2.0/test/test_v2beta1_list_pipeline_versions_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_list_pipelines_response.py` & `kfp-server-api-2.2.0/test/test_v2beta1_list_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_list_recurring_runs_response.py` & `kfp-server-api-2.2.0/test/test_v2beta1_list_recurring_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_list_runs_response.py` & `kfp-server-api-2.2.0/test/test_v2beta1_list_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_periodic_schedule.py` & `kfp-server-api-2.2.0/test/test_v2beta1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_pipeline.py` & `kfp-server-api-2.2.0/test/test_v2beta1_pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_pipeline_task_detail.py` & `kfp-server-api-2.2.0/test/test_v2beta1_pipeline_task_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_pipeline_task_executor_detail.py` & `kfp-server-api-2.2.0/test/test_v2beta1_pipeline_task_executor_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_pipeline_version.py` & `kfp-server-api-2.2.0/test/test_v2beta1_pipeline_version.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_pipeline_version_reference.py` & `kfp-server-api-2.2.0/test/test_v2beta1_pipeline_version_reference.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_predicate.py` & `kfp-server-api-2.2.0/test/test_v2beta1_predicate.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_predicate_operation.py` & `kfp-server-api-2.2.0/test/test_v2beta1_predicate_operation.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_read_artifact_response.py` & `kfp-server-api-2.2.0/test/test_v2beta1_read_artifact_response.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_recurring_run.py` & `kfp-server-api-2.2.0/test/test_v2beta1_recurring_run.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_recurring_run_status.py` & `kfp-server-api-2.2.0/test/test_v2beta1_recurring_run_status.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_run.py` & `kfp-server-api-2.2.0/test/test_v2beta1_run.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_run_details.py` & `kfp-server-api-2.2.0/test/test_v2beta1_run_details.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_run_storage_state.py` & `kfp-server-api-2.2.0/test/test_v2beta1_run_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_runtime_config.py` & `kfp-server-api-2.2.0/test/test_v2beta1_runtime_config.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_runtime_state.py` & `kfp-server-api-2.2.0/test/test_v2beta1_runtime_state.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_runtime_status.py` & `kfp-server-api-2.2.0/test/test_v2beta1_runtime_status.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_trigger.py` & `kfp-server-api-2.2.0/test/test_v2beta1_trigger.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_url.py` & `kfp-server-api-2.2.0/test/test_v2beta1_url.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_visualization.py` & `kfp-server-api-2.2.0/test/test_v2beta1_visualization.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_v2beta1_visualization_type.py` & `kfp-server-api-2.2.0/test/test_v2beta1_visualization_type.py`

 * *Files identical despite different names*

### Comparing `kfp-server-api-2.1.0/test/test_visualization_service_api.py` & `kfp-server-api-2.2.0/test/test_visualization_service_api.py`

 * *Files identical despite different names*

