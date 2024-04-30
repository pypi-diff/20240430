# Comparing `tmp/fiddler-client-3.1.0.dev2.tar.gz` & `tmp/fiddler-client-3.1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-client-3.1.0.dev2.tar", last modified: Fri Apr 19 12:21:13 2024, max compression
+gzip compressed data, was "fiddler-client-3.1.0.dev3.tar", last modified: Tue Apr 30 14:58:00 2024, max compression
```

## Comparing `fiddler-client-3.1.0.dev2.tar` & `fiddler-client-3.1.0.dev3.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.158824 fiddler-client-3.1.0.dev2/
--rw-r--r--   0 runner    (1001) runner    (1001)      559 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/LICENSE.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       42 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) runner    (1001)     1549 2024-04-19 12:21:13.158824 fiddler-client-3.1.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      855 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/PUBLIC.md
--rw-r--r--   0 runner    (1001) runner    (1001)     2165 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.138823 fiddler-client-3.1.0.dev2/fiddler/
--rw-r--r--   0 runner    (1001) runner    (1001)       11 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/VERSION
--rw-r--r--   0 runner    (1001) runner    (1001)     3757 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      217 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/configs.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5677 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/connection.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.138823 fiddler-client-3.1.0.dev2/fiddler/constants/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)      400 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/common.py
--rw-r--r--   0 runner    (1001) runner    (1001)      126 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)      114 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1706 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)      278 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      214 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1820 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/decorators.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.148823 fiddler-client-3.1.0.dev2/fiddler/entities/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3564 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11569 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2106 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7907 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6568 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/custom_expression.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4399 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4291 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5220 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18613 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5520 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/model_artifact.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3769 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1074 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4631 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3077 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/surrogate.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1243 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/user.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3798 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)    20250 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2221 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/exceptions.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.148823 fiddler-client-3.1.0.dev2/fiddler/libs/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6027 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/libs/http_client.py
--rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/libs/json_encoder.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15995 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/libs/semver.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.148823 fiddler-client-3.1.0.dev2/fiddler/packtools/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4637 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7941 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15799 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10467 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/packtools/template_model.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.148823 fiddler-client-3.1.0.dev2/fiddler/schemas/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      668 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1222 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)      189 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)      844 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/custom_expression.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5531 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/custom_features.py
--rw-r--r--   0 runner    (1001) runner    (1001)      657 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)      409 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1325 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/filter_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)      354 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1405 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1128 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1914 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/model_schema.py
--rw-r--r--   0 runner    (1001) runner    (1001)      941 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/model_spec.py
--rw-r--r--   0 runner    (1001) runner    (1001)      691 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/model_task_params.py
--rw-r--r--   0 runner    (1001) runner    (1001)      281 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)      379 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1166 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      500 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/server_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/user.py
--rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)      739 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/xai_params.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.148823 fiddler-client-3.1.0.dev2/fiddler/tests/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.158824 fiddler-client-3.1.0.dev2/fiddler/tests/apis/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3118 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11231 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7494 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8208 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_custom_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4636 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5134 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_events.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4501 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_files.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5089 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_generate_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1891 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2517 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_mixin.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18346 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5635 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model_artifact.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2441 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4443 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model_surrogate.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6015 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7804 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_segment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6440 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)    28590 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)      840 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/conftest.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/constants.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1865 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/test_connection.py
--rw-r--r--   0 runner    (1001) runner    (1001)      783 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/test_json_encoder.py
--rw-r--r--   0 runner    (1001) runner    (1001)      312 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/test_logger.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3333 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/test_utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)      335 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/utils.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.158824 fiddler-client-3.1.0.dev2/fiddler/utils/
--rw-r--r--   0 runner    (1001) runner    (1001)       53 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2908 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/utils/helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/utils/logger.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2203 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/utils/model_generator.py
--rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/utils/validations.py
--rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/utils/version.py
--rw-r--r--   0 runner    (1001) runner    (1001)      140 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/version.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.158824 fiddler-client-3.1.0.dev2/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     1549 2024-04-19 12:21:13.000000 fiddler-client-3.1.0.dev2/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     3321 2024-04-19 12:21:13.000000 fiddler-client-3.1.0.dev2/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-19 12:21:13.000000 fiddler-client-3.1.0.dev2/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-04-19 12:21:13.000000 fiddler-client-3.1.0.dev2/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-04-19 12:21:13.000000 fiddler-client-3.1.0.dev2/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-19 12:21:13.158824 fiddler-client-3.1.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.413544 fiddler-client-3.1.0.dev3/
+-rw-r--r--   0 runner    (1001) runner    (1001)      559 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       42 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) runner    (1001)     1589 2024-04-30 14:58:00.413544 fiddler-client-3.1.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      855 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/PUBLIC.md
+-rw-r--r--   0 runner    (1001) runner    (1001)     2165 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.393543 fiddler-client-3.1.0.dev3/fiddler/
+-rw-r--r--   0 runner    (1001) runner    (1001)       11 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/VERSION
+-rw-r--r--   0 runner    (1001) runner    (1001)     3824 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      217 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/configs.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5677 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/connection.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.393543 fiddler-client-3.1.0.dev3/fiddler/constants/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      400 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/common.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      126 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      114 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1706 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      278 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      214 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1820 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/decorators.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.393543 fiddler-client-3.1.0.dev3/fiddler/entities/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3564 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11800 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2106 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7907 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6568 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/custom_expression.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4399 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5383 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5220 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    19206 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5520 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/model_artifact.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3769 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1074 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4631 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3077 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/surrogate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1243 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4514 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    20250 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2221 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/exceptions.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.393543 fiddler-client-3.1.0.dev3/fiddler/libs/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6027 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/libs/http_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/libs/json_encoder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15995 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/libs/semver.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.393543 fiddler-client-3.1.0.dev3/fiddler/packtools/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4637 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7941 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15799 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10467 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/packtools/template_model.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.403543 fiddler-client-3.1.0.dev3/fiddler/schemas/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      668 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1328 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      189 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      953 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/custom_expression.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5531 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/custom_features.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      657 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      409 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1325 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/filter_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      354 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1405 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1128 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1914 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/model_schema.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      941 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/model_spec.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      691 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/model_task_params.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      281 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      379 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1166 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      500 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/server_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      739 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/xai_params.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.403543 fiddler-client-3.1.0.dev3/fiddler/tests/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.403543 fiddler-client-3.1.0.dev3/fiddler/tests/apis/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3118 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11593 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7494 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8208 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_custom_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4636 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5134 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4501 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_files.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5089 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_generate_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1891 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2517 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_mixin.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18551 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5635 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model_artifact.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2441 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4443 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model_surrogate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6015 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7804 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_segment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8099 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    28590 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      840 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/conftest.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/constants.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1865 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      783 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/test_json_encoder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      312 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3333 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      335 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.413544 fiddler-client-3.1.0.dev3/fiddler/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)       53 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2908 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/utils/helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/utils/logger.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2203 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/utils/model_generator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/utils/validations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/utils/version.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      140 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/version.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.413544 fiddler-client-3.1.0.dev3/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1589 2024-04-30 14:58:00.000000 fiddler-client-3.1.0.dev3/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     3321 2024-04-30 14:58:00.000000 fiddler-client-3.1.0.dev3/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-30 14:58:00.000000 fiddler-client-3.1.0.dev3/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)      162 2024-04-30 14:58:00.000000 fiddler-client-3.1.0.dev3/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-04-30 14:58:00.000000 fiddler-client-3.1.0.dev3/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-30 14:58:00.413544 fiddler-client-3.1.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)     1138 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/setup.py
```

### Comparing `fiddler-client-3.1.0.dev2/LICENSE.txt` & `fiddler-client-3.1.0.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/PKG-INFO` & `fiddler-client-3.1.0.dev3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 3.1.0.dev2
+Version: 3.1.0.dev3
 Summary: Python client for Fiddler Platform
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8.0
@@ -16,14 +16,15 @@
 Requires-Dist: pandas>=1.2.5
 Requires-Dist: pydantic<2,>=1.9.0
 Requires-Dist: deprecated==1.2.13
 Requires-Dist: tqdm
 Requires-Dist: simplejson>=3.17.0
 Requires-Dist: pyarrow>=7.0.0
 Requires-Dist: pyyaml
+Requires-Dist: typing-extensions<=4.5.0
 
 Fiddler Client
 =============
 
 Python client for interacting with Fiddler. Provides a user-friendly interface to our REST API and enables event
 publishing for use with our monitoring features.
```

### Comparing `fiddler-client-3.1.0.dev2/PUBLIC.md` & `fiddler-client-3.1.0.dev3/PUBLIC.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/README.md` & `fiddler-client-3.1.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/__init__.py` & `fiddler-client-3.1.0.dev3/fiddler/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 from fiddler.schemas.xai import (  # noqa
     DatasetDataSource,
     EventIdDataSource,
     RowDataSource,
     SqlSliceQueryDataSource,
 )
 from fiddler.schemas.xai_params import XaiParams  # noqa
+from fiddler.utils.helpers import group_by  # noqa
 from fiddler.utils.logger import set_logging  # noqa
 from fiddler.version import __version__  # noqa
 
 # Global connection object
 conn: Connection | None = None
 
 
@@ -137,8 +138,9 @@
     'Unsupported',
     'HttpError',
     'ConnTimeout',
     'ConnError',
     'ApiError',
     # Utilities
     'set_logging',
+    'group_by',
 ]
```

### Comparing `fiddler-client-3.1.0.dev2/fiddler/connection.py` & `fiddler-client-3.1.0.dev3/fiddler/connection.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/constants/alert_rule.py` & `fiddler-client-3.1.0.dev3/fiddler/constants/alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/constants/model.py` & `fiddler-client-3.1.0.dev3/fiddler/constants/model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/decorators.py` & `fiddler-client-3.1.0.dev3/fiddler/decorators.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/alert_record.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/alert_rule.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/alert_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         compare_to: CompareTo | str,
         condition: AlertCondition | str,
         bin_size: BinSize | str,
         critical_threshold: float,
         warning_threshold: float | None = None,
         columns: list[str] | None = None,
         baseline_id: UUID | str | None = None,
+        segment_id: UUID | str | None = None,
         compare_bin_delta: int | None = None,
     ) -> None:
         """Construct a alert rule instance."""
         self.name = name
         self.model_id = model_id
         self.metric_id = metric_id
         self.columns = columns
@@ -45,14 +46,15 @@
         self.priority = priority
         self.compare_to = compare_to
         self.compare_bin_delta = compare_bin_delta
         self.warning_threshold = warning_threshold
         self.critical_threshold = critical_threshold
         self.condition = condition
         self.bin_size = bin_size
+        self.segment_id = segment_id
 
         self.id: UUID | None = None
         self.project_id: UUID | None = None
 
         self.created_at: datetime | None = None
         self.updated_at: datetime | None = None
 
@@ -80,15 +82,16 @@
             priority=resp_obj.priority,
             compare_to=resp_obj.compare_to,
             condition=resp_obj.condition,
             bin_size=resp_obj.bin_size,
             critical_threshold=resp_obj.critical_threshold,
             warning_threshold=resp_obj.warning_threshold,
             columns=resp_obj.columns,
-            baseline_id=resp_obj.baseline_id,
+            baseline_id=resp_obj.baseline.id if resp_obj.baseline else None,
+            segment_id=resp_obj.segment.id if resp_obj.segment else None,
             compare_bin_delta=resp_obj.compare_bin_delta,
         )
 
         # Add remaining fields
         fields = [
             'id',
             'created_at',
@@ -206,14 +209,15 @@
             'model_name': model.name,
             'project_name': model.project.name,
             'metric_id': self.metric_id,
             'priority': self.priority,
             'compare_to': self.compare_to,
             'condition': self.condition,
             'bin_size': self.bin_size,
+            'segment_id': self.segment_id,
             'critical_threshold': self.critical_threshold,
             'warning_threshold': self.warning_threshold,
             'feature_names': self.columns,
             'compare_bin_delta': self.compare_bin_delta,
             'notifications': self._get_notifications_dict(),
         }
         if self.baseline_id:
```

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/base.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/base.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/baseline.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/custom_expression.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/custom_expression.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/dataset.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/events.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/events.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import annotations
 
 import tempfile
 from pathlib import Path
-from typing import Any
+from typing import Any, Callable
 from uuid import UUID
 
 import pandas as pd
 from requests import Response
 from tqdm import tqdm
 
 from fiddler.configs import STREAM_EVENT_LIMIT
 from fiddler.connection import ConnectionMixin
 from fiddler.decorators import handle_api_error
 from fiddler.entities.file import File
 from fiddler.entities.job import Job
 from fiddler.schemas.dataset import EnvType
 from fiddler.schemas.events import EventsSource, FileSource
 from fiddler.schemas.job import JobCompactResp
+from fiddler.utils.logger import get_logger
+
+logger = get_logger(__name__)
 
 
 class EventPublisher(ConnectionMixin):
     STREAM_LIMIT = STREAM_EVENT_LIMIT
 
     def __init__(self, model_id: UUID) -> None:
         """
@@ -47,48 +50,80 @@
             list[dict]: list of event dicts EnvType.PRE_PRODUCTION is not supported
         :param environment: Either EnvType.PRE_PRODUCTION or EnvType.PRODUCTION
         :param dataset_name: Name of the dataset. Not supported for EnvType.PRODUCTION
         :param update: flag indicating if the events are updates to previously published rows
 
         :return: list[UUID] for list of dicts source and Job object for file path or dataframe source.
         """
+
+        publish_method = self._get_publish_method(source=source)
+
+        return publish_method(
+            source=source,
+            environment=environment,
+            dataset_name=dataset_name,
+            update=update,
+        )
+
+    def _get_publish_method(
+        self, source: list[dict[str, Any]] | str | Path | pd.DataFrame
+    ) -> Callable:
         if isinstance(source, (str, Path)):
-            return self._publish_file(
-                source=source,
-                environment=environment,
-                dataset_name=dataset_name,
-                update=update,
-            )
+            return self._publish_file
 
         if isinstance(source, pd.DataFrame):
-            with tempfile.NamedTemporaryFile(suffix='.csv') as temp_file:
-                source.to_csv(temp_file.name, index=False)
+            return self._publish_df
+
+        if isinstance(source, list):
+            return self._publish_stream
+
+        raise ValueError(f'Unsupported source - {type(source)}')
+
+    def _publish_df(
+        self,
+        source: pd.DataFrame,
+        environment: EnvType,
+        dataset_name: str | None = None,
+        update: bool = False,
+    ) -> Job:
+        with tempfile.NamedTemporaryFile(suffix='.parquet') as temp_file:
+            try:
+                source.to_parquet(temp_file.name, index=False)
                 return self._publish_file(
                     source=temp_file.name,
                     environment=environment,
                     dataset_name=dataset_name,
                     update=update,
                 )
-
-        elif isinstance(source, list):
-            return self._publish_stream(source=source, update=update)
-
-        raise ValueError(f'Unsupported source - {type(source)}')
+            except Exception:
+                logger.warning(
+                    'Failed to convert input dataframe to parquet format. Retrying as a CSV file.'
+                )
+        with tempfile.NamedTemporaryFile(suffix='.csv') as temp_file:
+            source.to_csv(temp_file.name, index=False)
+            return self._publish_file(
+                source=temp_file.name,
+                environment=environment,
+                dataset_name=dataset_name,
+                update=update,
+            )
 
     def _publish_stream(
         self,
         source: list[dict[str, Any]],
+        environment: EnvType = EnvType.PRODUCTION,
+        dataset_name: str | None = None,
         update: bool = False,
     ) -> list[UUID]:
         event_ids = []
         for i in tqdm(range(0, len(source), self.STREAM_LIMIT)):
             response = self._publish_call(
                 source=EventsSource(events=source[i : i + self.STREAM_LIMIT]),
-                environment=EnvType.PRODUCTION,
-                dataset_name=None,
+                environment=environment,
+                dataset_name=dataset_name,
                 update=update,
             )
             event_ids.extend(response.json()['data']['event_ids'])
 
         return event_ids
 
     def _publish_file(
```

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/file.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/file.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/job.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/job.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/model.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import builtins
-import copy
 import typing
 from dataclasses import dataclass
 from datetime import datetime
 from functools import cached_property
 from pathlib import Path
 from typing import Any, Iterator
 from uuid import UUID
@@ -29,21 +28,25 @@
 from fiddler.schemas.model import ModelResp
 from fiddler.schemas.model_deployment import DeploymentParams
 from fiddler.schemas.model_schema import ModelSchema
 from fiddler.schemas.model_spec import ModelSpec
 from fiddler.schemas.model_task_params import ModelTaskParams
 from fiddler.schemas.xai_params import XaiParams
 from fiddler.utils.helpers import raise_not_found
+from fiddler.utils.logger import get_logger
 from fiddler.utils.model_generator import ModelGenerator
 
 if typing.TYPE_CHECKING:
     from fiddler.entities.baseline import Baseline
     from fiddler.entities.dataset import Dataset
 
 
+logger = get_logger(__name__)
+
+
 class Model(
     BaseEntity,
     CreatedByMixin,
     ProjectCompactMixin,
     UpdatedByMixin,
     XaiMixin,
 ):  # pylint: disable=too-many-ancestors
@@ -303,33 +306,43 @@
             _filter.add_rule(
                 QueryRule(field='name', operator=OperatorType.EQUAL, value=name)
             )
 
         params = {'filter': _filter.json()}
 
         for model in cls._paginate(url=cls._get_url(), params=params):
-            yield ModelCompact(id=model['id'], name=model['name'])
+            yield ModelCompact(
+                id=model['id'], name=model['name'], version=model['version']
+            )
 
     def duplicate(self, version: str | None = None) -> Model:
         """
         Duplicate the model instance with the given version name.
 
         This call will not save the model on server. After making changes to the model
         instance call .create() to add the model version to Fiddler Platform.
 
         :param version: Version name for the new instance
         :return: Model instance
         """
-        self_copy = copy.deepcopy(self)
-        self_copy.id = None
-
-        if version:
-            self_copy.version = version
-
-        return self_copy
+        return Model(
+            name=self.name,
+            project_id=self.project_id,
+            schema=self.schema,
+            spec=self.spec,
+            version=version if version else self.version,
+            input_type=self.input_type,
+            task=self.task,
+            task_params=self.task_params,
+            description=self.description,
+            event_id_col=self.event_id_col,
+            event_ts_col=self.event_ts_col,
+            event_ts_format=self.event_ts_format,
+            xai_params=self.xai_params,
+        )
 
     @property
     def datasets(self) -> Iterator[Dataset]:
         """Fetch all the datasets of this model"""
         from fiddler.entities.dataset import (  # pylint: disable=import-outside-toplevel
             Dataset,
         )
@@ -452,15 +465,15 @@
         :param dataset_name: Name of the dataset. Not supported for EnvType.PRODUCTION
         :param update: flag indicating if the events are updates to previously
             published rows
 
         :return: list[UUID] for list of dicts or dataframe source and Job object for
             file path source.
         """
-
+        logger.info('Model[%s/%s] - Publishing events', self.name, self.version)
         return self._event_publisher.publish(
             source=source,
             environment=environment,
             dataset_name=dataset_name,
             update=update,
         )
```

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/model_artifact.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/model_artifact.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/model_deployment.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/organization.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/organization.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/project.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/surrogate.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/surrogate.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/user.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/user.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/webhook.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/webhook.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 from datetime import datetime
 from typing import Any, Iterator
 from uuid import UUID
 
 from fiddler.decorators import handle_api_error
 from fiddler.entities.base import BaseEntity
+from fiddler.schemas.filter_query import OperatorType, QueryCondition, QueryRule
 from fiddler.schemas.webhook import WebhookProvider, WebhookResp
+from fiddler.utils.helpers import raise_not_found
 
 
 class Webhook(BaseEntity):
     def __init__(self, name: str, url: str, provider: WebhookProvider | str) -> None:
         """
         Construct a webhook instance
 
@@ -79,14 +81,30 @@
         :returns: `Webhook` object
         """
         response = cls._client().get(url=cls._get_url(id_))
         return cls._from_response(response=response)
 
     @classmethod
     @handle_api_error
+    def from_name(cls, name: str) -> Webhook:
+        """Get the webhook instance using webhook name"""
+        _filter = QueryCondition(
+            rules=[QueryRule(field='name', operator=OperatorType.EQUAL, value=name)]
+        )
+
+        response = cls._client().get(
+            url=cls._get_url(), params={'filter': _filter.json()}
+        )
+        if response.json()['data']['total'] == 0:
+            raise_not_found('Webhook not found for the given identifier')
+
+        return cls._from_dict(data=response.json()['data']['items'][0])
+
+    @classmethod
+    @handle_api_error
     def list(cls) -> Iterator[Webhook]:
         """Get a list of all webhooks in the organization"""
         for webhook in cls._paginate(url=cls._get_url()):
             yield cls._from_dict(data=webhook)
 
     @handle_api_error
     def create(self) -> Webhook:
```

### Comparing `fiddler-client-3.1.0.dev2/fiddler/entities/xai.py` & `fiddler-client-3.1.0.dev3/fiddler/entities/xai.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/exceptions.py` & `fiddler-client-3.1.0.dev3/fiddler/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/libs/http_client.py` & `fiddler-client-3.1.0.dev3/fiddler/libs/http_client.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/libs/json_encoder.py` & `fiddler-client-3.1.0.dev3/fiddler/libs/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/libs/semver.py` & `fiddler-client-3.1.0.dev3/fiddler/libs/semver.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/packtools/gem.py` & `fiddler-client-3.1.0.dev3/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/packtools/keras_ig_helpers.py` & `fiddler-client-3.1.0.dev3/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/packtools/project_attributions_helpers.py` & `fiddler-client-3.1.0.dev3/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/packtools/template_model.py` & `fiddler-client-3.1.0.dev3/fiddler/packtools/template_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/alert_record.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/alert_rule.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/alert_rule.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 from uuid import UUID
 
 from pydantic import Field
 
 from fiddler.constants.alert_rule import AlertCondition, BinSize, CompareTo, Priority
 from fiddler.schemas.base import BaseModel
 from fiddler.schemas.baseline import BaselineCompactResp
+from fiddler.schemas.custom_expression import SegmentCompactResp
 from fiddler.schemas.model import ModelCompactResp
 from fiddler.schemas.project import ProjectCompactResp
 
 
 class AlertRuleResp(BaseModel):
     id: UUID = Field(alias='uuid')
     name: str
     model: ModelCompactResp
     project: ProjectCompactResp
     baseline: Optional[BaselineCompactResp]
+    segment: Optional[SegmentCompactResp]
     priority: Union[str, Priority]
     compare_to: Union[str, CompareTo]
     metric_id: Union[str, UUID]
     critical_threshold: float
     condition: Union[str, AlertCondition]
     bin_size: Union[str, BinSize]
-    columns: Optional[List[str]]
-    baseline_id: Optional[UUID]
+    columns: Optional[List[str]] = Field(alias='feature_names')
     compare_bin_delta: Optional[int]
     warning_threshold: Optional[float]
 
     created_at: datetime
     updated_at: datetime = Field(alias='last_updated')
```

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/baseline.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/custom_expression.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/custom_expression.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,7 +25,14 @@
 
 class CustomMetricResp(CustomExpressionResp):
     """Custom metric response object"""
 
 
 class SegmentResp(CustomExpressionResp):
     """Segment response object"""
+
+
+class SegmentCompactResp(BaseModel):
+    """Segment compact response object"""
+
+    id: UUID
+    name: str
```

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/custom_features.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/custom_features.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/dataset.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/filter_query.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/filter_query.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/model.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/model_deployment.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/model_schema.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/model_schema.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/model_spec.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/model_spec.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/model_task_params.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/model_task_params.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/response.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/response.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/schemas/xai.py` & `fiddler-client-3.1.0.dev3/fiddler/schemas/xai.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_alert_record.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_alert_rule.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_alert_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,62 +24,69 @@
     PROJECT_NAME,
     URL,
 )
 from fiddler.utils.logger import set_logging
 
 API_RESPONSE_200 = {
     'data': {
-        'feature_names': ['age'],
-        'id': 620,
-        'created_at': '2023-11-28T08:04:12.651937+00:00',
+        'id': 794,
         'organization_name': 'mainbuild',
-        'compare_period': None,
-        'time_bucket': 3600000,
-        'alert_type': 'data_integrity',
-        'metric_display_name': 'Missing Value Violation',
-        'enable_notification': True,
-        'last_updated': '2023-11-28T08:04:12.653346+00:00',
-        'alert_type_display_name': 'Data Integrity',
-        'critical_threshold': 0.0,
+        'project_name': PROJECT_NAME,
+        'model_id': 285,
+        'name': 'test_rule',
+        'metric': 'jsd',
+        'metric_id': 'jsd',
+        'metric_display_name': 'Jensen-Shannon Distance',
+        'alert_type': 'drift',
+        'alert_type_display_name': 'Data Drift',
+        'priority': 'MEDIUM',
         'baseline_name': BASELINE_NAME,
-        'baseline': {
-            'id': BASELINE_ID,
-            'name': BASELINE_NAME,
-        },
+        'feature_names': ['creditscore'],
+        'time_bucket': 3600000,
+        'category': None,
+        'bin_size': 'Hour',
+        'compare_to': 'raw_value',
         'condition': 'greater',
-        'uuid': ALERT_RULE_ID,
-        'segment': None,
-        'warning_threshold': None,
-        'name': 'Age Missing 1 Hr',
-        'model_name': MODEL_NAME,
-        'model': {
-            'id': MODEL_ID,
-            'name': MODEL_NAME,
-        },
+        'compare_period': None,
+        'warning_threshold': 1.0,
+        'critical_threshold': 2.3,
         'is_active': True,
         'created_by': 'admin@fiddler.ai',
-        'bin_size': 'Hour',
-        'category': None,
-        'project_name': PROJECT_NAME,
-        'project': {
-            'id': PROJECT_ID,
-            'name': PROJECT_NAME,
+        'created_at': '2024-04-23T10:34:14.321895+00:00',
+        'last_updated': '2024-04-23T10:34:14.323554+00:00',
+        'model_name': 'bank_churn',
+        'enable_notification': True,
+        'segment': {
+            'id': '1c9b551a-808b-4ef0-b67b-e788eaf1e6de',
+            'organization_name': 'mainbuild',
+            'project_name': 'nick_test_project_11',
+            'model_name': 'bank_churn',
+            'name': 'xyzab',
+            'definition': 'Age > 10',
+            'description': 'meh',
+            'created_at': '2024-04-23T10:31:52.181550+00:00',
+            'created_by': {
+                'id': 1,
+                'full_name': 'Fiddler Administrator',
+                'email': 'admin@fiddler.ai',
+            },
         },
-        'metric': 'null_violation_count',
-        'metric_id': 'null_violation_count',
-        'compare_to': 'raw_value',
-        'priority': 'HIGH',
+        'project': {'id': PROJECT_ID, 'name': PROJECT_NAME},
+        'model': {'id': MODEL_ID, 'name': MODEL_NAME, 'version': 'v1'},
+        'baseline': {'id': BASELINE_ID, 'name': BASELINE_NAME},
+        'compare_bin_delta': None,
+        'uuid': ALERT_RULE_ID,
         'notifications': {
-            'emails': {'alert_config_uuid': ALERT_RULE_ID, 'email': 'admin@fiddler.ai'},
             'pagerduty': {
-                'severity': '',
                 'alert_config_uuid': ALERT_RULE_ID,
                 'service': '',
+                'severity': '',
             },
-            'webhooks': [{'uuid': 'e20bf4cc-d2cf-4540-baef-d96913b14f1b'}],
+            'emails': {'email': ''},
+            'webhooks': [],
         },
     },
     'api_version': '2.0',
     'kind': 'NORMAL',
 }
 
 API_RESPONSE_404 = {
```

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_baseline.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_custom_metric.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_custom_metric.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_dataset.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_events.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_events.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_files.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_files.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_generate_model.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_generate_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_job.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_job.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_mixin.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -467,14 +467,15 @@
         url=f'{URL}/v3/models',
         json=LIST_API_RESPONSE,
         match=[matchers.query_param_matcher(params)],
     )
     models = Model.list(project_id=PROJECT_ID)
     for model in models:
         assert isinstance(model, ModelCompact)
+        assert model.version is not None
 
 
 @responses.activate
 def test_model_list_with_name() -> None:
     params = {
         'filter': '{"condition": "AND", "rules": [{"field": "project_id", "operator": "equal", "value": "1531bfd9-2ca2-4a7b-bb5a-136c8da09ca1"}, {"field": "name", "operator": "equal", "value": "bank_churn"}]}',
         'limit': 50,
@@ -650,18 +651,24 @@
     responses.get(
         url=f'{URL}/v3/models/{MODEL_ID}',
         json=API_RESPONSE_200,
     )
     model = Model.get(id_=MODEL_ID)
 
     assert model.id == UUID(MODEL_ID)
+    assert model._event_publisher.model_id == model.id
 
     # Without version parameter
     model_copy = model.duplicate()
+
     assert model_copy.id is None
     assert model_copy.version == model.version
 
+    with pytest.raises(AssertionError):
+        # since id is None
+        _ = model_copy._event_publisher
+
     # With version parameter
     new_version = 'v2'
     model_copy = model.duplicate(version=new_version)
     assert model_copy.id is None
     assert model_copy.version == new_version
```

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model_artifact.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model_artifact.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model_deployment.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model_surrogate.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model_surrogate.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_project.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_segment.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_segment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_webhook.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_webhook.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,14 +44,37 @@
             }
         ],
     },
     'api_version': '2.0',
     'kind': 'ERROR',
 }
 
+API_RESPONSE_FROM_NAME = {
+    'data': {
+        'page_size': 100,
+        'total': 1,
+        'item_count': 1,
+        'page_count': 1,
+        'page_index': 1,
+        'offset': 0,
+        'items': [
+            {
+                'id': 1,
+                'uuid': WEBHOOK_ID,
+                'name': WEBHOOK_NAME,
+                'url': WEBHOOK_URL,
+                'provider': WEBHOOK_PROVIDER,
+                'created_at': '2024-04-30T13:38:08.408013+00:00',
+                'updated_at': '2024-04-30T13:38:08.408013+00:00',
+                'organization_name': ORG_NAME,
+            }
+        ],
+    }
+}
+
 LIST_API_RESPONSE = {
     'data': {
         'page_size': 100,
         'total': 2,
         'item_count': 2,
         'page_count': 1,
         'page_index': 1,
@@ -121,14 +144,48 @@
     )
 
     with pytest.raises(NotFound):
         Webhook.get(id_=webhook_id)
 
 
 @responses.activate
+def test_webhook_from_name_success() -> None:
+    params = {
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "test_webhook_config_name"}]}'
+    }
+    responses.get(
+        url=f'{URL}/v2/webhooks',
+        json=API_RESPONSE_FROM_NAME,
+        match=[responses.matchers.query_param_matcher(params)],
+    )
+    webhook = Webhook.from_name(name=WEBHOOK_NAME)
+    assert isinstance(webhook, Webhook)
+
+
+@responses.activate
+def test_webhook_from_name_not_found() -> None:
+    resp = API_RESPONSE_FROM_NAME.copy()
+    resp['data']['total'] = 0
+    resp['data']['item_count'] = 0
+    resp['data']['items'] = []
+
+    params = {
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "test_webhook_config_name"}]}'
+    }
+    responses.get(
+        url=f'{URL}/v2/webhooks',
+        json=resp,
+        match=[responses.matchers.query_param_matcher(params)],
+    )
+
+    with pytest.raises(NotFound):
+        Webhook.from_name(name=WEBHOOK_NAME)
+
+
+@responses.activate
 def test_webhook_list_success() -> None:
     responses.get(
         url=f'{URL}/v2/webhooks',
         json=LIST_API_RESPONSE,
     )
     for webhook in Webhook.list():
         assert isinstance(webhook, Webhook)
```

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_xai.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_xai.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/conftest.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/constants.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/constants.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/test_connection.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/test_json_encoder.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/tests/test_utils.py` & `fiddler-client-3.1.0.dev3/fiddler/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/utils/helpers.py` & `fiddler-client-3.1.0.dev3/fiddler/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/utils/logger.py` & `fiddler-client-3.1.0.dev3/fiddler/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/utils/model_generator.py` & `fiddler-client-3.1.0.dev3/fiddler/utils/model_generator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler/utils/version.py` & `fiddler-client-3.1.0.dev3/fiddler/utils/version.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/fiddler_client.egg-info/PKG-INFO` & `fiddler-client-3.1.0.dev3/fiddler_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 3.1.0.dev2
+Version: 3.1.0.dev3
 Summary: Python client for Fiddler Platform
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8.0
@@ -16,14 +16,15 @@
 Requires-Dist: pandas>=1.2.5
 Requires-Dist: pydantic<2,>=1.9.0
 Requires-Dist: deprecated==1.2.13
 Requires-Dist: tqdm
 Requires-Dist: simplejson>=3.17.0
 Requires-Dist: pyarrow>=7.0.0
 Requires-Dist: pyyaml
+Requires-Dist: typing-extensions<=4.5.0
 
 Fiddler Client
 =============
 
 Python client for interacting with Fiddler. Provides a user-friendly interface to our REST API and enables event
 publishing for use with our monitoring features.
```

### Comparing `fiddler-client-3.1.0.dev2/fiddler_client.egg-info/SOURCES.txt` & `fiddler-client-3.1.0.dev3/fiddler_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev2/setup.py` & `fiddler-client-3.1.0.dev3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         'pandas>=1.2.5',
         'pydantic>=1.9.0,<2',
         'deprecated==1.2.13',
         'tqdm',
         'simplejson>=3.17.0',
         'pyarrow>=7.0.0',
         'pyyaml',
+        'typing-extensions<=4.5.0',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
     ],
     python_requires='>3.8.0',
```

