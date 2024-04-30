# Comparing `tmp/instill_sdk-0.8.1rc0.tar.gz` & `tmp/instill_sdk-0.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instill_sdk-0.8.1rc0.tar", max compression
+gzip compressed data, was "instill_sdk-0.9.0rc0.tar", max compression
```

## Comparing `instill_sdk-0.8.1rc0.tar` & `instill_sdk-0.9.0rc0.tar`

### file list

```diff
@@ -1,548 +1,548 @@
--rw-r--r--   0        0        0     1072 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/LICENSE.md
--rw-r--r--   0        0        0    13232 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/README.md
--rw-r--r--   0        0        0      392 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/__init__.py
--rw-r--r--   0        0        0      329 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/__main__.py
--rw-r--r--   0        0        0      203 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/clients/__init__.py
--rw-r--r--   0        0        0     1635 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/clients/base.py
--rw-r--r--   0        0        0     2430 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/clients/client.py
--rw-r--r--   0        0        0       34 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/clients/constant.py
--rw-r--r--   0        0        0     1886 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/clients/instance.py
--rw-r--r--   0        0        0    26690 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/clients/mgmt.py
--rw-r--r--   0        0        0    16584 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/clients/model.py
--rw-r--r--   0        0        0    67548 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/clients/pipeline.py
--rw-r--r--   0        0        0     1681 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/configuration/__init__.py
--rw-r--r--   0        0        0      315 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/.dockerignore
--rw-r--r--   0        0        0      377 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/Dockerfile
--rw-r--r--   0        0        0      624 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/__init__.py
--rw-r--r--   0        0        0     3613 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/build.py
--rw-r--r--   0        0        0     2919 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/const.py
--rw-r--r--   0        0        0      253 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/errors.py
--rw-r--r--   0        0        0        1 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/protobufs/__init__.py
--rw-r--r--   0        0        0    12634 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/protobufs/parse.py
--rw-r--r--   0        0        0     3424 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/protobufs/ray_pb2.py
--rw-r--r--   0        0        0     4376 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/protobufs/ray_pb2.pyi
--rw-r--r--   0        0        0     3974 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/protobufs/ray_pb2_grpc.py
--rw-r--r--   0        0        0     1355 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/push.py
--rw-r--r--   0        0        0     6261 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/ray_config.py
--rw-r--r--   0        0        0    29040 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/ray_io.py
--rw-r--r--   0        0        0      678 2024-04-29 19:11:04.712280 instill_sdk-0.8.1rc0/instill/helpers/utils.py
--rw-r--r--   0        0        0       44 2024-04-29 19:11:24.104190 instill_sdk-0.8.1rc0/instill/protogen/.git
--rw-r--r--   0        0        0       32 2024-04-29 19:11:24.112190 instill_sdk-0.8.1rc0/instill/protogen/.github/CODEOWNERS
--rw-r--r--   0        0        0     2015 2024-04-29 19:11:24.112190 instill_sdk-0.8.1rc0/instill/protogen/.github/workflows/releases.yml
--rw-r--r--   0        0        0     1899 2024-04-29 19:11:24.112190 instill_sdk-0.8.1rc0/instill/protogen/CHANGELOG.md
--rw-r--r--   0        0        0    11346 2024-04-29 19:11:24.112190 instill_sdk-0.8.1rc0/instill/protogen/LICENSE
--rw-r--r--   0        0        0      326 2024-04-29 19:11:24.112190 instill_sdk-0.8.1rc0/instill/protogen/README.md
--rw-r--r--   0        0        0     3447 2024-04-29 19:11:24.112190 instill_sdk-0.8.1rc0/instill/protogen/artifact/artifact/v1alpha/artifact_pb2.py
--rw-r--r--   0        0        0     4562 2024-04-29 19:11:24.112190 instill_sdk-0.8.1rc0/instill/protogen/artifact/artifact/v1alpha/artifact_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.112190 instill_sdk-0.8.1rc0/instill/protogen/artifact/artifact/v1alpha/artifact_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.112190 instill_sdk-0.8.1rc0/instill/protogen/artifact/artifact/v1alpha/artifact_pb2_grpc.pyi
--rw-r--r--   0        0        0     3643 2024-04-29 19:11:24.112190 instill_sdk-0.8.1rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2.py
--rw-r--r--   0        0        0      165 2024-04-29 19:11:24.112190 instill_sdk-0.8.1rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2.pyi
--rw-r--r--   0        0        0     4951 2024-04-29 19:11:24.112190 instill_sdk-0.8.1rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2_grpc.py
--rw-r--r--   0        0        0     3374 2024-04-29 19:11:24.112190 instill_sdk-0.8.1rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2732 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/common/healthcheck/v1beta/healthcheck_pb2.py
--rw-r--r--   0        0        0     3210 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/common/healthcheck/v1beta/healthcheck_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/common/healthcheck/v1beta/healthcheck_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/common/healthcheck/v1beta/healthcheck_pb2_grpc.pyi
--rw-r--r--   0        0        0     2198 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/common/task/v1alpha/task_pb2.py
--rw-r--r--   0        0        0     4161 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/common/task/v1alpha/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/common/task/v1alpha/task_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/common/task/v1alpha/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    36390 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/metric/v1beta/metric_pb2.py
--rw-r--r--   0        0        0    52449 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/metric/v1beta/metric_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/metric/v1beta/metric_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/metric/v1beta/metric_pb2_grpc.pyi
--rw-r--r--   0        0        0     5818 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/metric/v1beta/metric_service_pb2.py
--rw-r--r--   0        0        0      407 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/metric/v1beta/metric_service_pb2.pyi
--rw-r--r--   0        0        0    43978 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/metric/v1beta/metric_service_pb2_grpc.py
--rw-r--r--   0        0        0    23247 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/metric/v1beta/metric_service_pb2_grpc.pyi
--rw-r--r--   0        0        0    18869 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/metric_pb2.py
--rw-r--r--   0        0        0    34273 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/metric_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/metric_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/metric_pb2_grpc.pyi
--rw-r--r--   0        0        0    58540 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_pb2.py
--rw-r--r--   0        0        0   112455 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.116190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_pb2_grpc.pyi
--rw-r--r--   0        0        0     6038 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2.py
--rw-r--r--   0        0        0      165 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2.pyi
--rw-r--r--   0        0        0    16129 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2_grpc.py
--rw-r--r--   0        0        0     9488 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2_grpc.pyi
--rw-r--r--   0        0        0    22092 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2.py
--rw-r--r--   0        0        0      165 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2.pyi
--rw-r--r--   0        0        0    72729 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2_grpc.py
--rw-r--r--   0        0        0    41689 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2_grpc.pyi
--rw-r--r--   0        0        0    23834 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/usage/v1beta/usage_pb2.py
--rw-r--r--   0        0        0    31770 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/usage/v1beta/usage_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/usage/v1beta/usage_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/usage/v1beta/usage_pb2_grpc.pyi
--rw-r--r--   0        0        0     3896 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/usage/v1beta/usage_service_pb2.py
--rw-r--r--   0        0        0      165 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/usage/v1beta/usage_service_pb2.pyi
--rw-r--r--   0        0        0     8313 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/usage/v1beta/usage_service_pb2_grpc.py
--rw-r--r--   0        0        0     5498 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/core/usage/v1beta/usage_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     7452 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/controller/v1alpha/controller_pb2.py
--rw-r--r--   0        0        0    11007 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/controller/v1alpha/controller_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/controller/v1alpha/controller_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/controller/v1alpha/controller_pb2_grpc.pyi
--rw-r--r--   0        0        0     4850 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2.py
--rw-r--r--   0        0        0      165 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2.pyi
--rw-r--r--   0        0        0    10707 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2_grpc.py
--rw-r--r--   0        0        0     6913 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3718 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/common_pb2.py
--rw-r--r--   0        0        0     5998 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/common_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/common_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/common_pb2_grpc.pyi
--rw-r--r--   0        0        0     8044 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_definition_pb2.py
--rw-r--r--   0        0        0    11160 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_definition_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_definition_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_definition_pb2_grpc.pyi
--rw-r--r--   0        0        0    60155 2024-04-29 19:11:24.120190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_pb2.py
--rw-r--r--   0        0        0   104082 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_pb2_grpc.pyi
--rw-r--r--   0        0        0     4749 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2.py
--rw-r--r--   0        0        0      165 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2.pyi
--rw-r--r--   0        0        0    10398 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2_grpc.py
--rw-r--r--   0        0        0     6144 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2_grpc.pyi
--rw-r--r--   0        0        0    20411 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2.py
--rw-r--r--   0        0        0      165 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2.pyi
--rw-r--r--   0        0        0    76760 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2_grpc.py
--rw-r--r--   0        0        0    54158 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3246 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_classification_pb2.py
--rw-r--r--   0        0        0     3180 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_classification_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_classification_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_classification_pb2_grpc.pyi
--rw-r--r--   0        0        0     3948 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_detection_pb2.py
--rw-r--r--   0        0        0     4253 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_detection_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_detection_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_detection_pb2_grpc.pyi
--rw-r--r--   0        0        0     4000 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_image_to_image_pb2.py
--rw-r--r--   0        0        0     4601 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_image_to_image_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_image_to_image_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_image_to_image_pb2_grpc.pyi
--rw-r--r--   0        0        0     4474 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_instance_segmentation_pb2.py
--rw-r--r--   0        0        0     4651 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_instance_segmentation_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_instance_segmentation_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_instance_segmentation_pb2_grpc.pyi
--rw-r--r--   0        0        0     4575 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_keypoint_pb2.py
--rw-r--r--   0        0        0     5208 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_keypoint_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_keypoint_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_keypoint_pb2_grpc.pyi
--rw-r--r--   0        0        0     3715 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_ocr_pb2.py
--rw-r--r--   0        0        0     4122 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_ocr_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_ocr_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_ocr_pb2_grpc.pyi
--rw-r--r--   0        0        0     3796 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_semantic_segmentation_pb2.py
--rw-r--r--   0        0        0     4121 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_semantic_segmentation_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_semantic_segmentation_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_semantic_segmentation_pb2_grpc.pyi
--rw-r--r--   0        0        0     5005 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_generation_chat_pb2.py
--rw-r--r--   0        0        0     5034 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_generation_chat_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_generation_chat_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_generation_chat_pb2_grpc.pyi
--rw-r--r--   0        0        0     4878 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_generation_pb2.py
--rw-r--r--   0        0        0     4992 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_generation_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_generation_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_generation_pb2_grpc.pyi
--rw-r--r--   0        0        0     3945 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_to_image_pb2.py
--rw-r--r--   0        0        0     4375 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_to_image_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_to_image_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_to_image_pb2_grpc.pyi
--rw-r--r--   0        0        0     2411 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_unspecified_pb2.py
--rw-r--r--   0        0        0     1928 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_unspecified_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_unspecified_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_unspecified_pb2_grpc.pyi
--rw-r--r--   0        0        0     5154 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_visual_question_answering_pb2.py
--rw-r--r--   0        0        0     5106 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_visual_question_answering_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_visual_question_answering_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_visual_question_answering_pb2_grpc.pyi
--rw-r--r--   0        0        0      203 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/release-please/config.json
--rw-r--r--   0        0        0       25 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/release-please/manifest.json
--rw-r--r--   0        0        0     4929 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/common_pb2.py
--rw-r--r--   0        0        0     9979 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/common_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/common_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/common_pb2_grpc.pyi
--rw-r--r--   0        0        0    12501 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/connector_definition_pb2.py
--rw-r--r--   0        0        0    18407 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/connector_definition_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/connector_definition_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.124190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/connector_definition_pb2_grpc.pyi
--rw-r--r--   0        0        0    38171 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/connector_pb2.py
--rw-r--r--   0        0        0    66085 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/connector_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/connector_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/connector_pb2_grpc.pyi
--rw-r--r--   0        0        0    10846 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/operator_definition_pb2.py
--rw-r--r--   0        0        0    15372 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/operator_definition_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/operator_definition_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/operator_definition_pb2_grpc.pyi
--rw-r--r--   0        0        0    75773 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_pb2.py
--rw-r--r--   0        0        0   133670 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_pb2_grpc.pyi
--rw-r--r--   0        0        0     7107 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2.py
--rw-r--r--   0        0        0      165 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2.pyi
--rw-r--r--   0        0        0    17769 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2_grpc.py
--rw-r--r--   0        0        0    11549 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2_grpc.pyi
--rw-r--r--   0        0        0    42219 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2.py
--rw-r--r--   0        0        0      165 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2.pyi
--rw-r--r--   0        0        0   159316 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2_grpc.py
--rw-r--r--   0        0        0   116394 2024-04-29 19:11:24.128190 instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     1441 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/__init__.py
--rw-r--r--   0        0        0     2738 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/connector.py
--rw-r--r--   0        0        0     7653 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/connector_ai.py
--rw-r--r--   0        0        0    57773 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/connector_airbyte.py
--rw-r--r--   0        0        0     1249 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/connector_blockchain.py
--rw-r--r--   0        0        0     7811 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/connector_data.py
--rw-r--r--   0        0        0      159 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/const.py
--rw-r--r--   0        0        0      119 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/errors.py
--rw-r--r--   0        0        0     4584 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/model.py
--rw-r--r--   0        0        0     1678 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/operator.py
--rw-r--r--   0        0        0     3031 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/pipeline.py
--rw-r--r--   0        0        0      305 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/recipe.py
--rw-r--r--   0        0        0      522 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/resource.py
--rw-r--r--   0        0        0        0 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/__init__.py
--rw-r--r--   0        0        0      447 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/airbyte/OAuth2.py
--rw-r--r--   0        0        0    61711 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/airbyte/__init__.py
--rw-r--r--   0        0        0      242 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/airbyte_task_write_destination_input.py
--rw-r--r--   0        0        0      199 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/airbyte_task_write_destination_output.py
--rw-r--r--   0        0        0      190 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/base64_task_decode_input.py
--rw-r--r--   0        0        0      192 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/base64_task_decode_output.py
--rw-r--r--   0        0        0      190 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/base64_task_encode_input.py
--rw-r--r--   0        0        0      192 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/base64_task_encode_output.py
--rw-r--r--   0        0        0      266 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/bigquery.py
--rw-r--r--   0        0        0      232 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/bigquery_task_insert_input.py
--rw-r--r--   0        0        0      196 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/bigquery_task_insert_output.py
--rw-r--r--   0        0        0      163 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/end_task_end_input.py
--rw-r--r--   0        0        0      321 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/end_task_end_metadata.py
--rw-r--r--   0        0        0      181 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/end_task_end_output.py
--rw-r--r--   0        0        0      247 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/googlecloudstorage.py
--rw-r--r--   0        0        0      223 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/googlecloudstorage_task_upload_input.py
--rw-r--r--   0        0        0      393 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/googlecloudstorage_task_upload_output.py
--rw-r--r--   0        0        0      229 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/googlesearch.py
--rw-r--r--   0        0        0      347 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/googlesearch_task_search_input.py
--rw-r--r--   0        0        0      389 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/googlesearch_task_search_output.py
--rw-r--r--   0        0        0     2111 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/helper.py
--rw-r--r--   0        0        0      258 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface.py
--rw-r--r--   0        0        0      270 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_audio_classification_input.py
--rw-r--r--   0        0        0      304 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_audio_classification_output.py
--rw-r--r--   0        0        0      899 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_conversational_input.py
--rw-r--r--   0        0        0      397 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_conversational_output.py
--rw-r--r--   0        0        0      405 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_fill_mask_input.py
--rw-r--r--   0        0        0      410 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_fill_mask_output.py
--rw-r--r--   0        0        0      270 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_image_classification_input.py
--rw-r--r--   0        0        0      304 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_image_classification_output.py
--rw-r--r--   0        0        0      268 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_image_segmentation_input.py
--rw-r--r--   0        0        0      321 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_image_segmentation_output.py
--rw-r--r--   0        0        0      263 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_image_to_text_input.py
--rw-r--r--   0        0        0      204 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_image_to_text_output.py
--rw-r--r--   0        0        0      266 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_object_detection_input.py
--rw-r--r--   0        0        0      403 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_object_detection_output.py
--rw-r--r--   0        0        0      479 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_question_answering_input.py
--rw-r--r--   0        0        0      336 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_question_answering_output.py
--rw-r--r--   0        0        0      501 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_sentence_similarity_input.py
--rw-r--r--   0        0        0      244 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_sentence_similarity_output.py
--rw-r--r--   0        0        0      268 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_speech_recognition_input.py
--rw-r--r--   0        0        0      209 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_speech_recognition_output.py
--rw-r--r--   0        0        0      747 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_summarization_input.py
--rw-r--r--   0        0        0      212 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_summarization_output.py
--rw-r--r--   0        0        0      502 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_table_question_answering_input.py
--rw-r--r--   0        0        0      376 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_table_question_answering_output.py
--rw-r--r--   0        0        0      415 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_text_classification_input.py
--rw-r--r--   0        0        0      305 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_text_classification_output.py
--rw-r--r--   0        0        0      845 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_text_generation_input.py
--rw-r--r--   0        0        0      216 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_text_generation_output.py
--rw-r--r--   0        0        0      680 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_text_to_image_input.py
--rw-r--r--   0        0        0      205 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_text_to_image_output.py
--rw-r--r--   0        0        0      538 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_token_classification_input.py
--rw-r--r--   0        0        0      450 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_token_classification_output.py
--rw-r--r--   0        0        0      407 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_translation_input.py
--rw-r--r--   0        0        0      214 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_translation_output.py
--rw-r--r--   0        0        0      555 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_zero_shot_classification_input.py
--rw-r--r--   0        0        0      316 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_zero_shot_classification_output.py
--rw-r--r--   0        0        0      303 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/image_task_draw_classification_input.py
--rw-r--r--   0        0        0      205 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/image_task_draw_classification_output.py
--rw-r--r--   0        0        0      485 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/image_task_draw_detection_input.py
--rw-r--r--   0        0        0      200 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/image_task_draw_detection_output.py
--rw-r--r--   0        0        0      510 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/image_task_draw_instance_segmentation_input.py
--rw-r--r--   0        0        0      212 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/image_task_draw_instance_segmentation_output.py
--rw-r--r--   0        0        0      566 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/image_task_draw_keypoint_input.py
--rw-r--r--   0        0        0      199 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/image_task_draw_keypoint_output.py
--rw-r--r--   0        0        0      475 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/image_task_draw_ocr_input.py
--rw-r--r--   0        0        0      194 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/image_task_draw_ocr_output.py
--rw-r--r--   0        0        0      364 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/image_task_draw_semantic_segmentation_input.py
--rw-r--r--   0        0        0      212 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/image_task_draw_semantic_segmentation_output.py
--rw-r--r--   0        0        0      502 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill.py
--rw-r--r--   0        0        0      227 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_classification_input.py
--rw-r--r--   0        0        0      221 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_classification_output.py
--rw-r--r--   0        0        0      222 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_detection_input.py
--rw-r--r--   0        0        0      421 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_detection_output.py
--rw-r--r--   0        0        0      465 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_image_to_image_input.py
--rw-r--r--   0        0        0      233 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_image_to_image_output.py
--rw-r--r--   0        0        0      234 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_instance_segmentation_input.py
--rw-r--r--   0        0        0      446 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_instance_segmentation_output.py
--rw-r--r--   0        0        0      221 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_keypoint_input.py
--rw-r--r--   0        0        0      502 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_keypoint_output.py
--rw-r--r--   0        0        0      216 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_ocr_input.py
--rw-r--r--   0        0        0      411 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_ocr_output.py
--rw-r--r--   0        0        0      234 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_semantic_segmentation_input.py
--rw-r--r--   0        0        0      300 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_semantic_segmentation_output.py
--rw-r--r--   0        0        0      953 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_text_generation_chat_input.py
--rw-r--r--   0        0        0      207 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_text_generation_chat_output.py
--rw-r--r--   0        0        0      948 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_text_generation_input.py
--rw-r--r--   0        0        0      202 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_text_generation_output.py
--rw-r--r--   0        0        0      444 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_text_to_image_input.py
--rw-r--r--   0        0        0      232 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_text_to_image_output.py
--rw-r--r--   0        0        0      941 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_visual_question_answering_input.py
--rw-r--r--   0        0        0      212 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_visual_question_answering_output.py
--rw-r--r--   0        0        0      231 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/json_task_marshal_input.py
--rw-r--r--   0        0        0      193 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/json_task_marshal_output.py
--rw-r--r--   0        0        0      193 2024-04-29 19:11:04.716280 instill_sdk-0.8.1rc0/instill/resources/schema/json_task_unmarshal_input.py
--rw-r--r--   0        0        0      235 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/json_task_unmarshal_output.py
--rw-r--r--   0        0        0   266195 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/airbyte_definitions.json
--rw-r--r--   0        0        0      425 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/airbyte_task_write_destination_input.json
--rw-r--r--   0        0        0       68 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/airbyte_task_write_destination_output.json
--rw-r--r--   0        0        0      638 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/airbyte_tasks.json
--rw-r--r--   0        0        0      402 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/base64_definitions.json
--rw-r--r--   0        0        0      353 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/base64_task_decode_input.json
--rw-r--r--   0        0        0      278 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/base64_task_decode_output.json
--rw-r--r--   0        0        0      344 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/base64_task_encode_input.json
--rw-r--r--   0        0        0      278 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/base64_task_encode_output.json
--rw-r--r--   0        0        0     1552 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/base64_tasks.json
--rw-r--r--   0        0        0      850 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/bigquery_definitions.json
--rw-r--r--   0        0        0      416 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/bigquery_task_insert_input.json
--rw-r--r--   0        0        0      226 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/bigquery_task_insert_output.json
--rw-r--r--   0        0        0      786 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/bigquery_tasks.json
--rw-r--r--   0        0        0    13691 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/component.json
--rw-r--r--   0        0        0      369 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/end_definitions.json
--rw-r--r--   0        0        0      347 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/end_task_end_input.json
--rw-r--r--   0        0        0      230 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/end_task_end_metadata.json
--rw-r--r--   0        0        0      120 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/end_task_end_output.json
--rw-r--r--   0        0        0      801 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/end_tasks.json
--rw-r--r--   0        0        0      595 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlecloudstorage_definitions.json
--rw-r--r--   0        0        0      502 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlecloudstorage_task_upload_input.json
--rw-r--r--   0        0        0      953 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlecloudstorage_task_upload_output.json
--rw-r--r--   0        0        0     1665 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlecloudstorage_tasks.json
--rw-r--r--   0        0        0     1112 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlesearch_definitions.json
--rw-r--r--   0        0        0     1212 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlesearch_task_search_input.json
--rw-r--r--   0        0        0     1298 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlesearch_task_search_output.json
--rw-r--r--   0        0        0     3954 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlesearch_tasks.json
--rw-r--r--   0        0        0     1019 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_definitions.json
--rw-r--r--   0        0        0      435 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_audio_classification_input.json
--rw-r--r--   0        0        0      555 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_audio_classification_output.json
--rw-r--r--   0        0        0     5048 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_conversational_input.json
--rw-r--r--   0        0        0     1062 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_conversational_output.json
--rw-r--r--   0        0        0     1611 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_fill_mask_input.json
--rw-r--r--   0        0        0      838 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_fill_mask_output.json
--rw-r--r--   0        0        0      435 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_image_classification_input.json
--rw-r--r--   0        0        0      555 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_image_classification_output.json
--rw-r--r--   0        0        0      435 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_image_segmentation_input.json
--rw-r--r--   0        0        0      779 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_image_segmentation_output.json
--rw-r--r--   0        0        0      435 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_image_to_text_input.json
--rw-r--r--   0        0        0      199 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_image_to_text_output.json
--rw-r--r--   0        0        0      435 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_object_detection_input.json
--rw-r--r--   0        0        0     1155 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_object_detection_output.json
--rw-r--r--   0        0        0     1984 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_question_answering_input.json
--rw-r--r--   0        0        0      770 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_question_answering_output.json
--rw-r--r--   0        0        0     2271 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_sentence_similarity_input.json
--rw-r--r--   0        0        0      282 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_sentence_similarity_output.json
--rw-r--r--   0        0        0      435 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_speech_recognition_input.json
--rw-r--r--   0        0        0      269 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_speech_recognition_output.json
--rw-r--r--   0        0        0     3893 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_summarization_input.json
--rw-r--r--   0        0        0      270 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_summarization_output.json
--rw-r--r--   0        0        0     2073 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_table_question_answering_input.json
--rw-r--r--   0        0        0      815 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_table_question_answering_output.json
--rw-r--r--   0        0        0     1611 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_text_classification_input.json
--rw-r--r--   0        0        0      548 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_text_classification_output.json
--rw-r--r--   0        0        0     4860 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_text_generation_input.json
--rw-r--r--   0        0        0      268 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_text_generation_output.json
--rw-r--r--   0        0        0     2719 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_text_to_image_input.json
--rw-r--r--   0        0        0      180 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_text_to_image_output.json
--rw-r--r--   0        0        0     2681 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_token_classification_input.json
--rw-r--r--   0        0        0     1095 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_token_classification_output.json
--rw-r--r--   0        0        0     1611 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_translation_input.json
--rw-r--r--   0        0        0      280 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_translation_output.json
--rw-r--r--   0        0        0     2550 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_zero_shot_classification_input.json
--rw-r--r--   0        0        0      668 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_zero_shot_classification_output.json
--rw-r--r--   0        0        0    57232 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_tasks.json
--rw-r--r--   0        0        0      528 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_definitions.json
--rw-r--r--   0        0        0      811 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_classification_input.json
--rw-r--r--   0        0        0      268 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_classification_output.json
--rw-r--r--   0        0        0     1937 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_detection_input.json
--rw-r--r--   0        0        0      268 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_detection_output.json
--rw-r--r--   0        0        0     2107 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_instance_segmentation_input.json
--rw-r--r--   0        0        0      268 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_instance_segmentation_output.json
--rw-r--r--   0        0        0     2427 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_keypoint_input.json
--rw-r--r--   0        0        0      268 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_keypoint_output.json
--rw-r--r--   0        0        0     1866 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_ocr_input.json
--rw-r--r--   0        0        0      268 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_ocr_output.json
--rw-r--r--   0        0        0     1131 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_semantic_segmentation_input.json
--rw-r--r--   0        0        0      268 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_semantic_segmentation_output.json
--rw-r--r--   0        0        0    13511 2024-04-29 19:11:04.720280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_tasks.json
--rw-r--r--   0        0        0     1048 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_definitions.json
--rw-r--r--   0        0        0      569 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_classification_input.json
--rw-r--r--   0        0        0      402 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_classification_output.json
--rw-r--r--   0        0        0      569 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_detection_input.json
--rw-r--r--   0        0        0     1528 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_detection_output.json
--rw-r--r--   0        0        0     1794 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_image_to_image_input.json
--rw-r--r--   0        0        0      291 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_image_to_image_output.json
--rw-r--r--   0        0        0      569 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_instance_segmentation_input.json
--rw-r--r--   0        0        0     1698 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_instance_segmentation_output.json
--rw-r--r--   0        0        0      569 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_keypoint_input.json
--rw-r--r--   0        0        0     2018 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_keypoint_output.json
--rw-r--r--   0        0        0      569 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_ocr_input.json
--rw-r--r--   0        0        0     1457 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_ocr_output.json
--rw-r--r--   0        0        0      569 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_semantic_segmentation_input.json
--rw-r--r--   0        0        0      722 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_semantic_segmentation_output.json
--rw-r--r--   0        0        0     1593 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_text_generation_chat_$ref.json
--rw-r--r--   0        0        0     4140 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_text_generation_chat_input.json
--rw-r--r--   0        0        0      278 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_text_generation_chat_output.json
--rw-r--r--   0        0        0     4140 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_text_generation_input.json
--rw-r--r--   0        0        0      278 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_text_generation_output.json
--rw-r--r--   0        0        0     1590 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_text_to_image_input.json
--rw-r--r--   0        0        0      291 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_text_to_image_output.json
--rw-r--r--   0        0        0     1593 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_visual_question_answering_$ref.json
--rw-r--r--   0        0        0     4172 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_visual_question_answering_input.json
--rw-r--r--   0        0        0      278 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_visual_question_answering_output.json
--rw-r--r--   0        0        0    33462 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_tasks.json
--rw-r--r--   0        0        0      374 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/json_definitions.json
--rw-r--r--   0        0        0      405 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/json_task_marshal_input.json
--rw-r--r--   0        0        0      284 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/json_task_marshal_output.json
--rw-r--r--   0        0        0      363 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/json_task_unmarshal_input.json
--rw-r--r--   0        0        0      321 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/json_task_unmarshal_output.json
--rw-r--r--   0        0        0     1700 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/json_tasks.json
--rw-r--r--   0        0        0      517 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/numbers_definitions.json
--rw-r--r--   0        0        0     3333 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/numbers_task_commit_input.json
--rw-r--r--   0        0        0      328 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/numbers_task_commit_output.json
--rw-r--r--   0        0        0     3202 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/numbers_task_register_input.json
--rw-r--r--   0        0        0      328 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/numbers_task_register_output.json
--rw-r--r--   0        0        0     3856 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/numbers_tasks.json
--rw-r--r--   0        0        0   378387 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai.json
--rw-r--r--   0        0        0      624 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_definitions.json
--rw-r--r--   0        0        0     1332 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_speech_recognition_input.json
--rw-r--r--   0        0        0      114 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_speech_recognition_output.json
--rw-r--r--   0        0        0      640 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_text_embeddings_input.json
--rw-r--r--   0        0        0      214 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_text_embeddings_output.json
--rw-r--r--   0        0        0     6290 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_text_generation_input.json
--rw-r--r--   0        0        0      251 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_text_generation_output.json
--rw-r--r--   0        0        0     1744 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_text_to_image_input.json
--rw-r--r--   0        0        0      505 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_text_to_image_output.json
--rw-r--r--   0        0        0     1013 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_text_to_speech_input.json
--rw-r--r--   0        0        0      207 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_text_to_speech_output.json
--rw-r--r--   0        0        0    14866 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_tasks.json
--rw-r--r--   0        0        0      663 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/pinecone_definitions.json
--rw-r--r--   0        0        0     2278 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/pinecone_task_query_input.json
--rw-r--r--   0        0        0     1109 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/pinecone_task_query_output.json
--rw-r--r--   0        0        0     1069 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/pinecone_task_upsert_input.json
--rw-r--r--   0        0        0      257 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/pinecone_task_upsert_output.json
--rw-r--r--   0        0        0     5398 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/pinecone_tasks.json
--rw-r--r--   0        0        0     2844 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_definitions.json
--rw-r--r--   0        0        0      972 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_task_chat_history_retrieve_input.json
--rw-r--r--   0        0        0     1151 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_task_chat_history_retrieve_output.json
--rw-r--r--   0        0        0      912 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_task_chat_message_write_input.json
--rw-r--r--   0        0        0     1204 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_task_chat_message_write_multi_modal_input.json
--rw-r--r--   0        0        0      231 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_task_chat_message_write_multi_modal_output.json
--rw-r--r--   0        0        0      231 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_task_chat_message_write_output.json
--rw-r--r--   0        0        0     5410 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_tasks.json
--rw-r--r--   0        0        0     2236 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_definitions.json
--rw-r--r--   0        0        0      928 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_delete_input.json
--rw-r--r--   0        0        0      633 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_delete_output.json
--rw-r--r--   0        0        0      615 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_get_input.json
--rw-r--r--   0        0        0      633 2024-04-29 19:11:04.724280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_get_output.json
--rw-r--r--   0        0        0      615 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_head_input.json
--rw-r--r--   0        0        0      633 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_head_output.json
--rw-r--r--   0        0        0      928 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_options_input.json
--rw-r--r--   0        0        0      633 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_options_output.json
--rw-r--r--   0        0        0      928 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_patch_input.json
--rw-r--r--   0        0        0      633 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_patch_output.json
--rw-r--r--   0        0        0      928 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_post_input.json
--rw-r--r--   0        0        0      633 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_post_output.json
--rw-r--r--   0        0        0      928 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_put_input.json
--rw-r--r--   0        0        0      633 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_put_output.json
--rw-r--r--   0        0        0    14137 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_tasks.json
--rw-r--r--   0        0        0    87757 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/stabilityai.json
--rw-r--r--   0        0        0      421 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/stabilityai_definitions.json
--rw-r--r--   0        0        0     4953 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/stabilityai_task_image_to_image_input.json
--rw-r--r--   0        0        0      585 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/stabilityai_task_image_to_image_output.json
--rw-r--r--   0        0        0     4015 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/stabilityai_task_text_to_image_input.json
--rw-r--r--   0        0        0      585 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/stabilityai_task_text_to_image_output.json
--rw-r--r--   0        0        0    10972 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/stabilityai_tasks.json
--rw-r--r--   0        0        0      379 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/start_definitions.json
--rw-r--r--   0        0        0      118 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/start_task_start_input.json
--rw-r--r--   0        0        0      461 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/start_task_start_metadata.json
--rw-r--r--   0        0        0      120 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/start_task_start_output.json
--rw-r--r--   0        0        0      811 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/start_tasks.json
--rw-r--r--   0        0        0      387 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/text_definitions.json
--rw-r--r--   0        0        0      408 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/text_task_convert_to_text_input.json
--rw-r--r--   0        0        0      783 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/text_task_convert_to_text_output.json
--rw-r--r--   0        0        0     1455 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/text_task_split_by_token_input.json
--rw-r--r--   0        0        0      661 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/text_task_split_by_token_output.json
--rw-r--r--   0        0        0     3743 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/text_tasks.json
--rw-r--r--   0        0        0      178 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/website_definitions.json
--rw-r--r--   0        0        0     1720 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/website_task_scrape_website_input.json
--rw-r--r--   0        0        0     1053 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/website_task_scrape_website_output.json
--rw-r--r--   0        0        0     3987 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/jsons/website_tasks.json
--rw-r--r--   0        0        0      227 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/numbers.py
--rw-r--r--   0        0        0     1383 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/numbers_task_commit_input.py
--rw-r--r--   0        0        0      229 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/numbers_task_commit_output.py
--rw-r--r--   0        0        0     1321 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/numbers_task_register_input.py
--rw-r--r--   0        0        0      231 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/numbers_task_register_output.py
--rw-r--r--   0        0        0      272 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/openai.py
--rw-r--r--   0        0        0      426 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/openai_task_speech_recognition_input.py
--rw-r--r--   0        0        0      204 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/openai_task_speech_recognition_output.py
--rw-r--r--   0        0        0      313 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/openai_task_text_embeddings_input.py
--rw-r--r--   0        0        0      238 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/openai_task_text_embeddings_output.py
--rw-r--r--   0        0        0     1654 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/openai_task_text_generation_input.py
--rw-r--r--   0        0        0      232 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/openai_task_text_generation_output.py
--rw-r--r--   0        0        0      813 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/openai_task_text_to_image_input.py
--rw-r--r--   0        0        0      299 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/openai_task_text_to_image_output.py
--rw-r--r--   0        0        0      703 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/openai_task_text_to_speech_input.py
--rw-r--r--   0        0        0      246 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/openai_task_text_to_speech_output.py
--rw-r--r--   0        0        0      218 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/pinecone.py
--rw-r--r--   0        0        0      496 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/pinecone_task_query_input.py
--rw-r--r--   0        0        0      410 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/pinecone_task_query_output.py
--rw-r--r--   0        0        0      341 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/pinecone_task_upsert_input.py
--rw-r--r--   0        0        0      204 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/pinecone_task_upsert_output.py
--rw-r--r--   0        0        0      718 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/redis.py
--rw-r--r--   0        0        0      320 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/redis_task_chat_history_retrieve_input.py
--rw-r--r--   0        0        0      649 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/redis_task_chat_history_retrieve_output.py
--rw-r--r--   0        0        0      323 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/redis_task_chat_message_write_input.py
--rw-r--r--   0        0        0      604 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/redis_task_chat_message_write_multi_modal_input.py
--rw-r--r--   0        0        0      218 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/redis_task_chat_message_write_multi_modal_output.py
--rw-r--r--   0        0        0      206 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/redis_task_chat_message_write_output.py
--rw-r--r--   0        0        0      684 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi.py
--rw-r--r--   0        0        0      325 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_delete_input.py
--rw-r--r--   0        0        0      281 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_delete_output.py
--rw-r--r--   0        0        0      280 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_get_input.py
--rw-r--r--   0        0        0      278 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_get_output.py
--rw-r--r--   0        0        0      281 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_head_input.py
--rw-r--r--   0        0        0      279 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_head_output.py
--rw-r--r--   0        0        0      326 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_options_input.py
--rw-r--r--   0        0        0      282 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_options_output.py
--rw-r--r--   0        0        0      324 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_patch_input.py
--rw-r--r--   0        0        0      280 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_patch_output.py
--rw-r--r--   0        0        0      323 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_post_input.py
--rw-r--r--   0        0        0      279 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_post_output.py
--rw-r--r--   0        0        0      322 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_put_input.py
--rw-r--r--   0        0        0      278 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/restapi_task_put_output.py
--rw-r--r--   0        0        0      215 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/stabilityai.py
--rw-r--r--   0        0        0     2400 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/stabilityai_task_image_to_image_input.py
--rw-r--r--   0        0        0      260 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/stabilityai_task_image_to_image_output.py
--rw-r--r--   0        0        0     2107 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/stabilityai_task_text_to_image_input.py
--rw-r--r--   0        0        0      259 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/stabilityai_task_text_to_image_output.py
--rw-r--r--   0        0        0      183 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/start_task_start_input.py
--rw-r--r--   0        0        0      459 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/start_task_start_metadata.py
--rw-r--r--   0        0        0      185 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/start_task_start_output.py
--rw-r--r--   0        0        0      196 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/text_task_convert_to_text_input.py
--rw-r--r--   0        0        0      285 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/text_task_convert_to_text_output.py
--rw-r--r--   0        0        0     1734 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/text_task_split_by_token_input.py
--rw-r--r--   0        0        0      275 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/text_task_split_by_token_output.py
--rw-r--r--   0        0        0      199 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/website.py
--rw-r--r--   0        0        0      394 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/website_task_scrape_website_input.py
--rw-r--r--   0        0        0      408 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/resources/schema/website_task_scrape_website_output.py
--rw-r--r--   0        0        0       34 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/tests/__init__.py
--rw-r--r--   0        0        0      267 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/tests/conftest.py
--rw-r--r--   0        0        0     4842 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/tests/test_client.py
--rw-r--r--   0        0        0        0 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/utils/__init__.py
--rw-r--r--   0        0        0      783 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/utils/error_handler.py
--rw-r--r--   0        0        0     2008 2024-04-29 19:11:04.728280 instill_sdk-0.8.1rc0/instill/utils/logger.py
--rw-r--r--   0        0        0     2905 2024-04-29 19:11:21.784201 instill_sdk-0.8.1rc0/pyproject.toml
--rw-r--r--   0        0        0    14712 1970-01-01 00:00:00.000000 instill_sdk-0.8.1rc0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/LICENSE.md
+-rw-r--r--   0        0        0    13232 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/README.md
+-rw-r--r--   0        0        0      392 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/__init__.py
+-rw-r--r--   0        0        0      329 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/__main__.py
+-rw-r--r--   0        0        0      203 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/clients/__init__.py
+-rw-r--r--   0        0        0     1635 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/clients/base.py
+-rw-r--r--   0        0        0     2430 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/clients/client.py
+-rw-r--r--   0        0        0       34 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/clients/constant.py
+-rw-r--r--   0        0        0     1886 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/clients/instance.py
+-rw-r--r--   0        0        0    26690 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/clients/mgmt.py
+-rw-r--r--   0        0        0    16584 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/clients/model.py
+-rw-r--r--   0        0        0    67548 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/clients/pipeline.py
+-rw-r--r--   0        0        0     1681 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/configuration/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/.dockerignore
+-rw-r--r--   0        0        0      489 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/Dockerfile
+-rw-r--r--   0        0        0      624 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/__init__.py
+-rw-r--r--   0        0        0     4511 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/build.py
+-rw-r--r--   0        0        0     2919 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/const.py
+-rw-r--r--   0        0        0      479 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/errors.py
+-rw-r--r--   0        0        0        1 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/protobufs/__init__.py
+-rw-r--r--   0        0        0    12634 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/protobufs/parse.py
+-rw-r--r--   0        0        0     3424 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/protobufs/ray_pb2.py
+-rw-r--r--   0        0        0     4376 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/protobufs/ray_pb2.pyi
+-rw-r--r--   0        0        0     3974 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/protobufs/ray_pb2_grpc.py
+-rw-r--r--   0        0        0     1467 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/push.py
+-rw-r--r--   0        0        0     6261 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/ray_config.py
+-rw-r--r--   0        0        0    29040 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/ray_io.py
+-rw-r--r--   0        0        0      678 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/helpers/utils.py
+-rw-r--r--   0        0        0       44 2024-04-30 10:41:19.080742 instill_sdk-0.9.0rc0/instill/protogen/.git
+-rw-r--r--   0        0        0       32 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/.github/CODEOWNERS
+-rw-r--r--   0        0        0     2015 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/.github/workflows/releases.yml
+-rw-r--r--   0        0        0     1899 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/CHANGELOG.md
+-rw-r--r--   0        0        0    11346 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/LICENSE
+-rw-r--r--   0        0        0      326 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/README.md
+-rw-r--r--   0        0        0     3447 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/artifact/artifact/v1alpha/artifact_pb2.py
+-rw-r--r--   0        0        0     4562 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/artifact/artifact/v1alpha/artifact_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/artifact/artifact/v1alpha/artifact_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/artifact/artifact/v1alpha/artifact_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3643 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2.py
+-rw-r--r--   0        0        0      165 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2.pyi
+-rw-r--r--   0        0        0     4951 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3374 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2732 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/common/healthcheck/v1beta/healthcheck_pb2.py
+-rw-r--r--   0        0        0     3210 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/common/healthcheck/v1beta/healthcheck_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/common/healthcheck/v1beta/healthcheck_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/common/healthcheck/v1beta/healthcheck_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2198 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/common/task/v1alpha/task_pb2.py
+-rw-r--r--   0        0        0     4161 2024-04-30 10:41:19.088743 instill_sdk-0.9.0rc0/instill/protogen/common/task/v1alpha/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/common/task/v1alpha/task_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/common/task/v1alpha/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    36390 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/metric/v1beta/metric_pb2.py
+-rw-r--r--   0        0        0    52449 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/metric/v1beta/metric_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/metric/v1beta/metric_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/metric/v1beta/metric_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5818 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/metric/v1beta/metric_service_pb2.py
+-rw-r--r--   0        0        0      407 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/metric/v1beta/metric_service_pb2.pyi
+-rw-r--r--   0        0        0    43978 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/metric/v1beta/metric_service_pb2_grpc.py
+-rw-r--r--   0        0        0    23247 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/metric/v1beta/metric_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18869 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/metric_pb2.py
+-rw-r--r--   0        0        0    34273 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/metric_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/metric_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/metric_pb2_grpc.pyi
+-rw-r--r--   0        0        0    58540 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_pb2.py
+-rw-r--r--   0        0        0   112455 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6038 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2.py
+-rw-r--r--   0        0        0      165 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2.pyi
+-rw-r--r--   0        0        0    16129 2024-04-30 10:41:19.092743 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9488 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0    22092 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2.py
+-rw-r--r--   0        0        0      165 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2.pyi
+-rw-r--r--   0        0        0    72729 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2_grpc.py
+-rw-r--r--   0        0        0    41689 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0    23834 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/core/usage/v1beta/usage_pb2.py
+-rw-r--r--   0        0        0    31770 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/core/usage/v1beta/usage_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/core/usage/v1beta/usage_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/core/usage/v1beta/usage_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3896 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/core/usage/v1beta/usage_service_pb2.py
+-rw-r--r--   0        0        0      165 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/core/usage/v1beta/usage_service_pb2.pyi
+-rw-r--r--   0        0        0     8313 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/core/usage/v1beta/usage_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5498 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/core/usage/v1beta/usage_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7452 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/controller/v1alpha/controller_pb2.py
+-rw-r--r--   0        0        0    11007 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/controller/v1alpha/controller_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/controller/v1alpha/controller_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/controller/v1alpha/controller_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4850 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2.py
+-rw-r--r--   0        0        0      165 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2.pyi
+-rw-r--r--   0        0        0    10707 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6913 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3718 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/common_pb2.py
+-rw-r--r--   0        0        0     5998 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/common_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/common_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8044 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_definition_pb2.py
+-rw-r--r--   0        0        0    11160 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_definition_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_definition_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_definition_pb2_grpc.pyi
+-rw-r--r--   0        0        0    60155 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_pb2.py
+-rw-r--r--   0        0        0   104082 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4749 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2.py
+-rw-r--r--   0        0        0      165 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2.pyi
+-rw-r--r--   0        0        0    10398 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6144 2024-04-30 10:41:19.096742 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0    20411 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2.py
+-rw-r--r--   0        0        0      165 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2.pyi
+-rw-r--r--   0        0        0    76760 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2_grpc.py
+-rw-r--r--   0        0        0    54158 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3246 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_classification_pb2.py
+-rw-r--r--   0        0        0     3180 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_classification_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_classification_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_classification_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3948 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_detection_pb2.py
+-rw-r--r--   0        0        0     4253 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_detection_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_detection_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_detection_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4000 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_image_to_image_pb2.py
+-rw-r--r--   0        0        0     4601 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_image_to_image_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_image_to_image_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_image_to_image_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4474 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_instance_segmentation_pb2.py
+-rw-r--r--   0        0        0     4651 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_instance_segmentation_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_instance_segmentation_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_instance_segmentation_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4575 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_keypoint_pb2.py
+-rw-r--r--   0        0        0     5208 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_keypoint_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_keypoint_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_keypoint_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3715 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_ocr_pb2.py
+-rw-r--r--   0        0        0     4122 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_ocr_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_ocr_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_ocr_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3796 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_semantic_segmentation_pb2.py
+-rw-r--r--   0        0        0     4121 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_semantic_segmentation_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_semantic_segmentation_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_semantic_segmentation_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5005 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_generation_chat_pb2.py
+-rw-r--r--   0        0        0     5034 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_generation_chat_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_generation_chat_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_generation_chat_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4878 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_generation_pb2.py
+-rw-r--r--   0        0        0     4992 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_generation_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_generation_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_generation_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3945 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_to_image_pb2.py
+-rw-r--r--   0        0        0     4375 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_to_image_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_to_image_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_to_image_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2411 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_unspecified_pb2.py
+-rw-r--r--   0        0        0     1928 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_unspecified_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_unspecified_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_unspecified_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5154 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_visual_question_answering_pb2.py
+-rw-r--r--   0        0        0     5106 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_visual_question_answering_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_visual_question_answering_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_visual_question_answering_pb2_grpc.pyi
+-rw-r--r--   0        0        0      203 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/release-please/config.json
+-rw-r--r--   0        0        0       25 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/release-please/manifest.json
+-rw-r--r--   0        0        0     4929 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/common_pb2.py
+-rw-r--r--   0        0        0     9979 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/common_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/common_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12501 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/connector_definition_pb2.py
+-rw-r--r--   0        0        0    18407 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/connector_definition_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/connector_definition_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/connector_definition_pb2_grpc.pyi
+-rw-r--r--   0        0        0    38171 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/connector_pb2.py
+-rw-r--r--   0        0        0    66085 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/connector_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/connector_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/connector_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10846 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/operator_definition_pb2.py
+-rw-r--r--   0        0        0    15372 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/operator_definition_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/operator_definition_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.100743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/operator_definition_pb2_grpc.pyi
+-rw-r--r--   0        0        0    75773 2024-04-30 10:41:19.104743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_pb2.py
+-rw-r--r--   0        0        0   133670 2024-04-30 10:41:19.104743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:19.104743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-30 10:41:19.104743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7107 2024-04-30 10:41:19.104743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2.py
+-rw-r--r--   0        0        0      165 2024-04-30 10:41:19.104743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2.pyi
+-rw-r--r--   0        0        0    17769 2024-04-30 10:41:19.104743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11549 2024-04-30 10:41:19.104743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0    42219 2024-04-30 10:41:19.104743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2.py
+-rw-r--r--   0        0        0      165 2024-04-30 10:41:19.104743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2.pyi
+-rw-r--r--   0        0        0   159316 2024-04-30 10:41:19.104743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2_grpc.py
+-rw-r--r--   0        0        0   116394 2024-04-30 10:41:19.104743 instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1441 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/__init__.py
+-rw-r--r--   0        0        0     2738 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/connector.py
+-rw-r--r--   0        0        0     7653 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/connector_ai.py
+-rw-r--r--   0        0        0    57773 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/connector_airbyte.py
+-rw-r--r--   0        0        0     1249 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/connector_blockchain.py
+-rw-r--r--   0        0        0     7811 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/connector_data.py
+-rw-r--r--   0        0        0      159 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/const.py
+-rw-r--r--   0        0        0      119 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/errors.py
+-rw-r--r--   0        0        0     4584 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/model.py
+-rw-r--r--   0        0        0     1678 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/operator.py
+-rw-r--r--   0        0        0     3031 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/pipeline.py
+-rw-r--r--   0        0        0      305 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/recipe.py
+-rw-r--r--   0        0        0      522 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/resource.py
+-rw-r--r--   0        0        0        0 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/__init__.py
+-rw-r--r--   0        0        0      447 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/airbyte/OAuth2.py
+-rw-r--r--   0        0        0    61711 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/airbyte/__init__.py
+-rw-r--r--   0        0        0      242 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/airbyte_task_write_destination_input.py
+-rw-r--r--   0        0        0      199 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/airbyte_task_write_destination_output.py
+-rw-r--r--   0        0        0      190 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/base64_task_decode_input.py
+-rw-r--r--   0        0        0      192 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/base64_task_decode_output.py
+-rw-r--r--   0        0        0      190 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/base64_task_encode_input.py
+-rw-r--r--   0        0        0      192 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/base64_task_encode_output.py
+-rw-r--r--   0        0        0      266 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/bigquery.py
+-rw-r--r--   0        0        0      232 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/bigquery_task_insert_input.py
+-rw-r--r--   0        0        0      196 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/bigquery_task_insert_output.py
+-rw-r--r--   0        0        0      163 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/end_task_end_input.py
+-rw-r--r--   0        0        0      321 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/end_task_end_metadata.py
+-rw-r--r--   0        0        0      181 2024-04-30 10:41:00.420548 instill_sdk-0.9.0rc0/instill/resources/schema/end_task_end_output.py
+-rw-r--r--   0        0        0      247 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/googlecloudstorage.py
+-rw-r--r--   0        0        0      223 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/googlecloudstorage_task_upload_input.py
+-rw-r--r--   0        0        0      393 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/googlecloudstorage_task_upload_output.py
+-rw-r--r--   0        0        0      229 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/googlesearch.py
+-rw-r--r--   0        0        0      347 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/googlesearch_task_search_input.py
+-rw-r--r--   0        0        0      389 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/googlesearch_task_search_output.py
+-rw-r--r--   0        0        0     2111 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/helper.py
+-rw-r--r--   0        0        0      258 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface.py
+-rw-r--r--   0        0        0      270 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_audio_classification_input.py
+-rw-r--r--   0        0        0      304 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_audio_classification_output.py
+-rw-r--r--   0        0        0      899 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_conversational_input.py
+-rw-r--r--   0        0        0      397 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_conversational_output.py
+-rw-r--r--   0        0        0      405 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_fill_mask_input.py
+-rw-r--r--   0        0        0      410 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_fill_mask_output.py
+-rw-r--r--   0        0        0      270 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_image_classification_input.py
+-rw-r--r--   0        0        0      304 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_image_classification_output.py
+-rw-r--r--   0        0        0      268 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_image_segmentation_input.py
+-rw-r--r--   0        0        0      321 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_image_segmentation_output.py
+-rw-r--r--   0        0        0      263 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_image_to_text_input.py
+-rw-r--r--   0        0        0      204 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_image_to_text_output.py
+-rw-r--r--   0        0        0      266 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_object_detection_input.py
+-rw-r--r--   0        0        0      403 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_object_detection_output.py
+-rw-r--r--   0        0        0      479 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_question_answering_input.py
+-rw-r--r--   0        0        0      336 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_question_answering_output.py
+-rw-r--r--   0        0        0      501 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_sentence_similarity_input.py
+-rw-r--r--   0        0        0      244 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_sentence_similarity_output.py
+-rw-r--r--   0        0        0      268 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_speech_recognition_input.py
+-rw-r--r--   0        0        0      209 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_speech_recognition_output.py
+-rw-r--r--   0        0        0      747 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_summarization_input.py
+-rw-r--r--   0        0        0      212 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_summarization_output.py
+-rw-r--r--   0        0        0      502 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_table_question_answering_input.py
+-rw-r--r--   0        0        0      376 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_table_question_answering_output.py
+-rw-r--r--   0        0        0      415 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_text_classification_input.py
+-rw-r--r--   0        0        0      305 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_text_classification_output.py
+-rw-r--r--   0        0        0      845 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_text_generation_input.py
+-rw-r--r--   0        0        0      216 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_text_generation_output.py
+-rw-r--r--   0        0        0      680 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_text_to_image_input.py
+-rw-r--r--   0        0        0      205 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_text_to_image_output.py
+-rw-r--r--   0        0        0      538 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_token_classification_input.py
+-rw-r--r--   0        0        0      450 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_token_classification_output.py
+-rw-r--r--   0        0        0      407 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_translation_input.py
+-rw-r--r--   0        0        0      214 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_translation_output.py
+-rw-r--r--   0        0        0      555 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_zero_shot_classification_input.py
+-rw-r--r--   0        0        0      316 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_zero_shot_classification_output.py
+-rw-r--r--   0        0        0      303 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/image_task_draw_classification_input.py
+-rw-r--r--   0        0        0      205 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/image_task_draw_classification_output.py
+-rw-r--r--   0        0        0      485 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/image_task_draw_detection_input.py
+-rw-r--r--   0        0        0      200 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/image_task_draw_detection_output.py
+-rw-r--r--   0        0        0      510 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/image_task_draw_instance_segmentation_input.py
+-rw-r--r--   0        0        0      212 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/image_task_draw_instance_segmentation_output.py
+-rw-r--r--   0        0        0      566 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/image_task_draw_keypoint_input.py
+-rw-r--r--   0        0        0      199 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/image_task_draw_keypoint_output.py
+-rw-r--r--   0        0        0      475 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/image_task_draw_ocr_input.py
+-rw-r--r--   0        0        0      194 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/image_task_draw_ocr_output.py
+-rw-r--r--   0        0        0      364 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/image_task_draw_semantic_segmentation_input.py
+-rw-r--r--   0        0        0      212 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/image_task_draw_semantic_segmentation_output.py
+-rw-r--r--   0        0        0      502 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill.py
+-rw-r--r--   0        0        0      227 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_classification_input.py
+-rw-r--r--   0        0        0      221 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_classification_output.py
+-rw-r--r--   0        0        0      222 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_detection_input.py
+-rw-r--r--   0        0        0      421 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_detection_output.py
+-rw-r--r--   0        0        0      465 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_image_to_image_input.py
+-rw-r--r--   0        0        0      233 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_image_to_image_output.py
+-rw-r--r--   0        0        0      234 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_instance_segmentation_input.py
+-rw-r--r--   0        0        0      446 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_instance_segmentation_output.py
+-rw-r--r--   0        0        0      221 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_keypoint_input.py
+-rw-r--r--   0        0        0      502 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_keypoint_output.py
+-rw-r--r--   0        0        0      216 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_ocr_input.py
+-rw-r--r--   0        0        0      411 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_ocr_output.py
+-rw-r--r--   0        0        0      234 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_semantic_segmentation_input.py
+-rw-r--r--   0        0        0      300 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_semantic_segmentation_output.py
+-rw-r--r--   0        0        0      953 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_text_generation_chat_input.py
+-rw-r--r--   0        0        0      207 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_text_generation_chat_output.py
+-rw-r--r--   0        0        0      948 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_text_generation_input.py
+-rw-r--r--   0        0        0      202 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_text_generation_output.py
+-rw-r--r--   0        0        0      444 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_text_to_image_input.py
+-rw-r--r--   0        0        0      232 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_text_to_image_output.py
+-rw-r--r--   0        0        0      941 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_visual_question_answering_input.py
+-rw-r--r--   0        0        0      212 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_visual_question_answering_output.py
+-rw-r--r--   0        0        0      231 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/json_task_marshal_input.py
+-rw-r--r--   0        0        0      193 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/json_task_marshal_output.py
+-rw-r--r--   0        0        0      193 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/json_task_unmarshal_input.py
+-rw-r--r--   0        0        0      235 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/json_task_unmarshal_output.py
+-rw-r--r--   0        0        0   266195 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/airbyte_definitions.json
+-rw-r--r--   0        0        0      425 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/airbyte_task_write_destination_input.json
+-rw-r--r--   0        0        0       68 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/airbyte_task_write_destination_output.json
+-rw-r--r--   0        0        0      638 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/airbyte_tasks.json
+-rw-r--r--   0        0        0      402 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/base64_definitions.json
+-rw-r--r--   0        0        0      353 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/base64_task_decode_input.json
+-rw-r--r--   0        0        0      278 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/base64_task_decode_output.json
+-rw-r--r--   0        0        0      344 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/base64_task_encode_input.json
+-rw-r--r--   0        0        0      278 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/base64_task_encode_output.json
+-rw-r--r--   0        0        0     1552 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/base64_tasks.json
+-rw-r--r--   0        0        0      850 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/bigquery_definitions.json
+-rw-r--r--   0        0        0      416 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/bigquery_task_insert_input.json
+-rw-r--r--   0        0        0      226 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/bigquery_task_insert_output.json
+-rw-r--r--   0        0        0      786 2024-04-30 10:41:00.424548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/bigquery_tasks.json
+-rw-r--r--   0        0        0    13691 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/component.json
+-rw-r--r--   0        0        0      369 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/end_definitions.json
+-rw-r--r--   0        0        0      347 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/end_task_end_input.json
+-rw-r--r--   0        0        0      230 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/end_task_end_metadata.json
+-rw-r--r--   0        0        0      120 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/end_task_end_output.json
+-rw-r--r--   0        0        0      801 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/end_tasks.json
+-rw-r--r--   0        0        0      595 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlecloudstorage_definitions.json
+-rw-r--r--   0        0        0      502 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlecloudstorage_task_upload_input.json
+-rw-r--r--   0        0        0      953 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlecloudstorage_task_upload_output.json
+-rw-r--r--   0        0        0     1665 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlecloudstorage_tasks.json
+-rw-r--r--   0        0        0     1112 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlesearch_definitions.json
+-rw-r--r--   0        0        0     1212 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlesearch_task_search_input.json
+-rw-r--r--   0        0        0     1298 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlesearch_task_search_output.json
+-rw-r--r--   0        0        0     3954 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlesearch_tasks.json
+-rw-r--r--   0        0        0     1019 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_definitions.json
+-rw-r--r--   0        0        0      435 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_audio_classification_input.json
+-rw-r--r--   0        0        0      555 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_audio_classification_output.json
+-rw-r--r--   0        0        0     5048 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_conversational_input.json
+-rw-r--r--   0        0        0     1062 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_conversational_output.json
+-rw-r--r--   0        0        0     1611 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_fill_mask_input.json
+-rw-r--r--   0        0        0      838 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_fill_mask_output.json
+-rw-r--r--   0        0        0      435 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_image_classification_input.json
+-rw-r--r--   0        0        0      555 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_image_classification_output.json
+-rw-r--r--   0        0        0      435 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_image_segmentation_input.json
+-rw-r--r--   0        0        0      779 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_image_segmentation_output.json
+-rw-r--r--   0        0        0      435 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_image_to_text_input.json
+-rw-r--r--   0        0        0      199 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_image_to_text_output.json
+-rw-r--r--   0        0        0      435 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_object_detection_input.json
+-rw-r--r--   0        0        0     1155 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_object_detection_output.json
+-rw-r--r--   0        0        0     1984 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_question_answering_input.json
+-rw-r--r--   0        0        0      770 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_question_answering_output.json
+-rw-r--r--   0        0        0     2271 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_sentence_similarity_input.json
+-rw-r--r--   0        0        0      282 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_sentence_similarity_output.json
+-rw-r--r--   0        0        0      435 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_speech_recognition_input.json
+-rw-r--r--   0        0        0      269 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_speech_recognition_output.json
+-rw-r--r--   0        0        0     3893 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_summarization_input.json
+-rw-r--r--   0        0        0      270 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_summarization_output.json
+-rw-r--r--   0        0        0     2073 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_table_question_answering_input.json
+-rw-r--r--   0        0        0      815 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_table_question_answering_output.json
+-rw-r--r--   0        0        0     1611 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_text_classification_input.json
+-rw-r--r--   0        0        0      548 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_text_classification_output.json
+-rw-r--r--   0        0        0     4860 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_text_generation_input.json
+-rw-r--r--   0        0        0      268 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_text_generation_output.json
+-rw-r--r--   0        0        0     2719 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_text_to_image_input.json
+-rw-r--r--   0        0        0      180 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_text_to_image_output.json
+-rw-r--r--   0        0        0     2681 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_token_classification_input.json
+-rw-r--r--   0        0        0     1095 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_token_classification_output.json
+-rw-r--r--   0        0        0     1611 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_translation_input.json
+-rw-r--r--   0        0        0      280 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_translation_output.json
+-rw-r--r--   0        0        0     2550 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_zero_shot_classification_input.json
+-rw-r--r--   0        0        0      668 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_zero_shot_classification_output.json
+-rw-r--r--   0        0        0    57232 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_tasks.json
+-rw-r--r--   0        0        0      528 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_definitions.json
+-rw-r--r--   0        0        0      811 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_classification_input.json
+-rw-r--r--   0        0        0      268 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_classification_output.json
+-rw-r--r--   0        0        0     1937 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_detection_input.json
+-rw-r--r--   0        0        0      268 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_detection_output.json
+-rw-r--r--   0        0        0     2107 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_instance_segmentation_input.json
+-rw-r--r--   0        0        0      268 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_instance_segmentation_output.json
+-rw-r--r--   0        0        0     2427 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_keypoint_input.json
+-rw-r--r--   0        0        0      268 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_keypoint_output.json
+-rw-r--r--   0        0        0     1866 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_ocr_input.json
+-rw-r--r--   0        0        0      268 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_ocr_output.json
+-rw-r--r--   0        0        0     1131 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_semantic_segmentation_input.json
+-rw-r--r--   0        0        0      268 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_semantic_segmentation_output.json
+-rw-r--r--   0        0        0    13511 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_tasks.json
+-rw-r--r--   0        0        0     1048 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_definitions.json
+-rw-r--r--   0        0        0      569 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_classification_input.json
+-rw-r--r--   0        0        0      402 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_classification_output.json
+-rw-r--r--   0        0        0      569 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_detection_input.json
+-rw-r--r--   0        0        0     1528 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_detection_output.json
+-rw-r--r--   0        0        0     1794 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_image_to_image_input.json
+-rw-r--r--   0        0        0      291 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_image_to_image_output.json
+-rw-r--r--   0        0        0      569 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_instance_segmentation_input.json
+-rw-r--r--   0        0        0     1698 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_instance_segmentation_output.json
+-rw-r--r--   0        0        0      569 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_keypoint_input.json
+-rw-r--r--   0        0        0     2018 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_keypoint_output.json
+-rw-r--r--   0        0        0      569 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_ocr_input.json
+-rw-r--r--   0        0        0     1457 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_ocr_output.json
+-rw-r--r--   0        0        0      569 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_semantic_segmentation_input.json
+-rw-r--r--   0        0        0      722 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_semantic_segmentation_output.json
+-rw-r--r--   0        0        0     1593 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_text_generation_chat_$ref.json
+-rw-r--r--   0        0        0     4140 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_text_generation_chat_input.json
+-rw-r--r--   0        0        0      278 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_text_generation_chat_output.json
+-rw-r--r--   0        0        0     4140 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_text_generation_input.json
+-rw-r--r--   0        0        0      278 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_text_generation_output.json
+-rw-r--r--   0        0        0     1590 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_text_to_image_input.json
+-rw-r--r--   0        0        0      291 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_text_to_image_output.json
+-rw-r--r--   0        0        0     1593 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_visual_question_answering_$ref.json
+-rw-r--r--   0        0        0     4172 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_visual_question_answering_input.json
+-rw-r--r--   0        0        0      278 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_visual_question_answering_output.json
+-rw-r--r--   0        0        0    33462 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_tasks.json
+-rw-r--r--   0        0        0      374 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/json_definitions.json
+-rw-r--r--   0        0        0      405 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/json_task_marshal_input.json
+-rw-r--r--   0        0        0      284 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/json_task_marshal_output.json
+-rw-r--r--   0        0        0      363 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/json_task_unmarshal_input.json
+-rw-r--r--   0        0        0      321 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/json_task_unmarshal_output.json
+-rw-r--r--   0        0        0     1700 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/json_tasks.json
+-rw-r--r--   0        0        0      517 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/numbers_definitions.json
+-rw-r--r--   0        0        0     3333 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/numbers_task_commit_input.json
+-rw-r--r--   0        0        0      328 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/numbers_task_commit_output.json
+-rw-r--r--   0        0        0     3202 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/numbers_task_register_input.json
+-rw-r--r--   0        0        0      328 2024-04-30 10:41:00.428548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/numbers_task_register_output.json
+-rw-r--r--   0        0        0     3856 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/numbers_tasks.json
+-rw-r--r--   0        0        0   378387 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai.json
+-rw-r--r--   0        0        0      624 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_definitions.json
+-rw-r--r--   0        0        0     1332 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_speech_recognition_input.json
+-rw-r--r--   0        0        0      114 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_speech_recognition_output.json
+-rw-r--r--   0        0        0      640 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_text_embeddings_input.json
+-rw-r--r--   0        0        0      214 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_text_embeddings_output.json
+-rw-r--r--   0        0        0     6290 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_text_generation_input.json
+-rw-r--r--   0        0        0      251 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_text_generation_output.json
+-rw-r--r--   0        0        0     1744 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_text_to_image_input.json
+-rw-r--r--   0        0        0      505 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_text_to_image_output.json
+-rw-r--r--   0        0        0     1013 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_text_to_speech_input.json
+-rw-r--r--   0        0        0      207 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_text_to_speech_output.json
+-rw-r--r--   0        0        0    14866 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_tasks.json
+-rw-r--r--   0        0        0      663 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/pinecone_definitions.json
+-rw-r--r--   0        0        0     2278 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/pinecone_task_query_input.json
+-rw-r--r--   0        0        0     1109 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/pinecone_task_query_output.json
+-rw-r--r--   0        0        0     1069 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/pinecone_task_upsert_input.json
+-rw-r--r--   0        0        0      257 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/pinecone_task_upsert_output.json
+-rw-r--r--   0        0        0     5398 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/pinecone_tasks.json
+-rw-r--r--   0        0        0     2844 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_definitions.json
+-rw-r--r--   0        0        0      972 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_task_chat_history_retrieve_input.json
+-rw-r--r--   0        0        0     1151 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_task_chat_history_retrieve_output.json
+-rw-r--r--   0        0        0      912 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_task_chat_message_write_input.json
+-rw-r--r--   0        0        0     1204 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_task_chat_message_write_multi_modal_input.json
+-rw-r--r--   0        0        0      231 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_task_chat_message_write_multi_modal_output.json
+-rw-r--r--   0        0        0      231 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_task_chat_message_write_output.json
+-rw-r--r--   0        0        0     5410 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_tasks.json
+-rw-r--r--   0        0        0     2236 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_definitions.json
+-rw-r--r--   0        0        0      928 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_delete_input.json
+-rw-r--r--   0        0        0      633 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_delete_output.json
+-rw-r--r--   0        0        0      615 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_get_input.json
+-rw-r--r--   0        0        0      633 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_get_output.json
+-rw-r--r--   0        0        0      615 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_head_input.json
+-rw-r--r--   0        0        0      633 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_head_output.json
+-rw-r--r--   0        0        0      928 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_options_input.json
+-rw-r--r--   0        0        0      633 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_options_output.json
+-rw-r--r--   0        0        0      928 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_patch_input.json
+-rw-r--r--   0        0        0      633 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_patch_output.json
+-rw-r--r--   0        0        0      928 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_post_input.json
+-rw-r--r--   0        0        0      633 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_post_output.json
+-rw-r--r--   0        0        0      928 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_put_input.json
+-rw-r--r--   0        0        0      633 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_put_output.json
+-rw-r--r--   0        0        0    14137 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_tasks.json
+-rw-r--r--   0        0        0    87757 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/stabilityai.json
+-rw-r--r--   0        0        0      421 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/stabilityai_definitions.json
+-rw-r--r--   0        0        0     4953 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/stabilityai_task_image_to_image_input.json
+-rw-r--r--   0        0        0      585 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/stabilityai_task_image_to_image_output.json
+-rw-r--r--   0        0        0     4015 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/stabilityai_task_text_to_image_input.json
+-rw-r--r--   0        0        0      585 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/stabilityai_task_text_to_image_output.json
+-rw-r--r--   0        0        0    10972 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/stabilityai_tasks.json
+-rw-r--r--   0        0        0      379 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/start_definitions.json
+-rw-r--r--   0        0        0      118 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/start_task_start_input.json
+-rw-r--r--   0        0        0      461 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/start_task_start_metadata.json
+-rw-r--r--   0        0        0      120 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/start_task_start_output.json
+-rw-r--r--   0        0        0      811 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/start_tasks.json
+-rw-r--r--   0        0        0      387 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/text_definitions.json
+-rw-r--r--   0        0        0      408 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/text_task_convert_to_text_input.json
+-rw-r--r--   0        0        0      783 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/text_task_convert_to_text_output.json
+-rw-r--r--   0        0        0     1455 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/text_task_split_by_token_input.json
+-rw-r--r--   0        0        0      661 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/text_task_split_by_token_output.json
+-rw-r--r--   0        0        0     3743 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/text_tasks.json
+-rw-r--r--   0        0        0      178 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/website_definitions.json
+-rw-r--r--   0        0        0     1720 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/website_task_scrape_website_input.json
+-rw-r--r--   0        0        0     1053 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/website_task_scrape_website_output.json
+-rw-r--r--   0        0        0     3987 2024-04-30 10:41:00.432548 instill_sdk-0.9.0rc0/instill/resources/schema/jsons/website_tasks.json
+-rw-r--r--   0        0        0      227 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/numbers.py
+-rw-r--r--   0        0        0     1383 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/numbers_task_commit_input.py
+-rw-r--r--   0        0        0      229 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/numbers_task_commit_output.py
+-rw-r--r--   0        0        0     1321 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/numbers_task_register_input.py
+-rw-r--r--   0        0        0      231 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/numbers_task_register_output.py
+-rw-r--r--   0        0        0      272 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/openai.py
+-rw-r--r--   0        0        0      426 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/openai_task_speech_recognition_input.py
+-rw-r--r--   0        0        0      204 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/openai_task_speech_recognition_output.py
+-rw-r--r--   0        0        0      313 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/openai_task_text_embeddings_input.py
+-rw-r--r--   0        0        0      238 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/openai_task_text_embeddings_output.py
+-rw-r--r--   0        0        0     1654 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/openai_task_text_generation_input.py
+-rw-r--r--   0        0        0      232 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/openai_task_text_generation_output.py
+-rw-r--r--   0        0        0      813 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/openai_task_text_to_image_input.py
+-rw-r--r--   0        0        0      299 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/openai_task_text_to_image_output.py
+-rw-r--r--   0        0        0      703 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/openai_task_text_to_speech_input.py
+-rw-r--r--   0        0        0      246 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/openai_task_text_to_speech_output.py
+-rw-r--r--   0        0        0      218 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/pinecone.py
+-rw-r--r--   0        0        0      496 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/pinecone_task_query_input.py
+-rw-r--r--   0        0        0      410 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/pinecone_task_query_output.py
+-rw-r--r--   0        0        0      341 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/pinecone_task_upsert_input.py
+-rw-r--r--   0        0        0      204 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/pinecone_task_upsert_output.py
+-rw-r--r--   0        0        0      718 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/redis.py
+-rw-r--r--   0        0        0      320 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/redis_task_chat_history_retrieve_input.py
+-rw-r--r--   0        0        0      649 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/redis_task_chat_history_retrieve_output.py
+-rw-r--r--   0        0        0      323 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/redis_task_chat_message_write_input.py
+-rw-r--r--   0        0        0      604 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/redis_task_chat_message_write_multi_modal_input.py
+-rw-r--r--   0        0        0      218 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/redis_task_chat_message_write_multi_modal_output.py
+-rw-r--r--   0        0        0      206 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/redis_task_chat_message_write_output.py
+-rw-r--r--   0        0        0      684 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi.py
+-rw-r--r--   0        0        0      325 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_delete_input.py
+-rw-r--r--   0        0        0      281 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_delete_output.py
+-rw-r--r--   0        0        0      280 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_get_input.py
+-rw-r--r--   0        0        0      278 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_get_output.py
+-rw-r--r--   0        0        0      281 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_head_input.py
+-rw-r--r--   0        0        0      279 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_head_output.py
+-rw-r--r--   0        0        0      326 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_options_input.py
+-rw-r--r--   0        0        0      282 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_options_output.py
+-rw-r--r--   0        0        0      324 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_patch_input.py
+-rw-r--r--   0        0        0      280 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_patch_output.py
+-rw-r--r--   0        0        0      323 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_post_input.py
+-rw-r--r--   0        0        0      279 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_post_output.py
+-rw-r--r--   0        0        0      322 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_put_input.py
+-rw-r--r--   0        0        0      278 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/restapi_task_put_output.py
+-rw-r--r--   0        0        0      215 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/stabilityai.py
+-rw-r--r--   0        0        0     2400 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/stabilityai_task_image_to_image_input.py
+-rw-r--r--   0        0        0      260 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/stabilityai_task_image_to_image_output.py
+-rw-r--r--   0        0        0     2107 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/stabilityai_task_text_to_image_input.py
+-rw-r--r--   0        0        0      259 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/stabilityai_task_text_to_image_output.py
+-rw-r--r--   0        0        0      183 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/start_task_start_input.py
+-rw-r--r--   0        0        0      459 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/start_task_start_metadata.py
+-rw-r--r--   0        0        0      185 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/start_task_start_output.py
+-rw-r--r--   0        0        0      196 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/text_task_convert_to_text_input.py
+-rw-r--r--   0        0        0      285 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/text_task_convert_to_text_output.py
+-rw-r--r--   0        0        0     1734 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/text_task_split_by_token_input.py
+-rw-r--r--   0        0        0      275 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/text_task_split_by_token_output.py
+-rw-r--r--   0        0        0      199 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/website.py
+-rw-r--r--   0        0        0      394 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/website_task_scrape_website_input.py
+-rw-r--r--   0        0        0      408 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/resources/schema/website_task_scrape_website_output.py
+-rw-r--r--   0        0        0       34 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/tests/__init__.py
+-rw-r--r--   0        0        0      267 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/tests/conftest.py
+-rw-r--r--   0        0        0     4842 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/tests/test_client.py
+-rw-r--r--   0        0        0        0 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/utils/__init__.py
+-rw-r--r--   0        0        0      783 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/utils/error_handler.py
+-rw-r--r--   0        0        0     2008 2024-04-30 10:41:00.436548 instill_sdk-0.9.0rc0/instill/utils/logger.py
+-rw-r--r--   0        0        0     3018 2024-04-30 10:41:16.968720 instill_sdk-0.9.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    14773 1970-01-01 00:00:00.000000 instill_sdk-0.9.0rc0/PKG-INFO
```

### Comparing `instill_sdk-0.8.1rc0/LICENSE.md` & `instill_sdk-0.9.0rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/README.md` & `instill_sdk-0.9.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/clients/base.py` & `instill_sdk-0.9.0rc0/instill/clients/base.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/clients/client.py` & `instill_sdk-0.9.0rc0/instill/clients/client.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/clients/instance.py` & `instill_sdk-0.9.0rc0/instill/clients/instance.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/clients/mgmt.py` & `instill_sdk-0.9.0rc0/instill/clients/mgmt.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/clients/model.py` & `instill_sdk-0.9.0rc0/instill/clients/model.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/clients/pipeline.py` & `instill_sdk-0.9.0rc0/instill/clients/pipeline.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/configuration/__init__.py` & `instill_sdk-0.9.0rc0/instill/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/helpers/__init__.py` & `instill_sdk-0.9.0rc0/instill/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/helpers/build.py` & `instill_sdk-0.9.0rc0/instill/helpers/build.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,61 +7,82 @@
 import tempfile
 
 import ray
 import yaml
 
 import instill
 from instill.helpers.const import DEFAULT_DEPENDENCIES
+from instill.helpers.errors import ModelConfigException
 from instill.utils.logger import Logger
 
-if __name__ == "__main__":
-    Logger.i("[Instill Builder] Setup docker...")
+
+def config_check_required_fields(c):
+    if "build" not in c or c["build"] is None:
+        raise ModelConfigException("build")
+    if "gpu" not in c["build"] or c["build"]["gpu"] is None:
+        raise ModelConfigException("gpu")
+    if "python_version" not in c["build"] or c["build"]["python_version"] is None:
+        raise ModelConfigException("python_version")
+    if "repo" not in c or c["repo"] is None:
+        raise ModelConfigException("repo")
+
+
+def build_image():
     if platform.machine() in ("i386", "AMD64", "x86_64"):
         default_platform = "amd64"
     else:
         default_platform = platform.machine()
     parser = argparse.ArgumentParser()
     parser.add_argument(
+        "-t",
+        "--tag",
+        help="tag for the model image",
+        default="",
+        required=False,
+    )
+    parser.add_argument(
         "--no-cache",
         help="build the image without cache",
         action="store_true",
         required=False,
     )
     parser.add_argument(
         "--target-arch",
         help="target platform architecture for the model image, default to host",
         default=default_platform,
         choices=["arm64", "amd64"],
         required=False,
     )
 
+    args = parser.parse_args()
     try:
-        args = parser.parse_args()
-
         Logger.i("[Instill Builder] Loading config file...")
         with open("instill.yaml", "r", encoding="utf8") as f:
             Logger.i("[Instill Builder] Parsing config file...")
             config = yaml.safe_load(f)
 
+        config_check_required_fields(config)
+
         build = config["build"]
         repo = config["repo"]
-        tag = (
-            config["tag"]
-            if config["tag"] is not None and config["tag"] != ""
-            else hashlib.sha256().hexdigest()
-        )
+        tag = args.tag if args.tag != "" else hashlib.sha256().hexdigest()
 
         python_version = build["python_version"].replace(".", "")
         ray_version = ray.__version__
         instill_version = instill.__version__
 
         cuda_suffix = "" if not build["gpu"] else "-cu121"
 
+        system_str = ""
+        if "system_packages" in build and not build["system_packages"] is None:
+            for p in build["system_packages"]:
+                system_str += p + " "
+
         packages_str = ""
-        if not build["python_packages"] is None:
+        if "python_packages" in build and not build["python_packages"] is None:
             for p in build["python_packages"]:
                 packages_str += p + " "
         for p in DEFAULT_DEPENDENCIES:
             packages_str += p + " "
         packages_str += f"instill-sdk=={instill_version}"
 
         with tempfile.TemporaryDirectory() as tmpdir:
@@ -86,28 +107,34 @@
                 f"RAY_VERSION={ray_version}",
                 "--build-arg",
                 f"PYTHON_VERSION={python_version}",
                 "--build-arg",
                 f"CUDA_SUFFIX={cuda_suffix}",
                 "--build-arg",
                 f"PACKAGES={packages_str}",
+                "--build-arg",
+                f"SYSTEM_PACKAGES={system_str}",
                 "--platform",
                 f"linux/{args.target_arch}",
                 "-t",
                 f"{repo}:{tag}",
                 tmpdir,
                 "--load",
             ]
             if args.no_cache:
                 command.append("--no-cache")
             subprocess.run(
                 command,
                 check=True,
             )
             Logger.i(f"[Instill Builder] {repo}:{tag} built")
-    except subprocess.CalledProcessError as e:
+    except subprocess.CalledProcessError:
         Logger.e("[Instill Builder] Build failed")
     except Exception as e:
         Logger.e("[Instill Builder] Prepare failed")
         Logger.e(e)
     finally:
         Logger.i("[Instill Builder] Done")
+
+
+if __name__ == "__main__":
+    build_image()
```

### Comparing `instill_sdk-0.8.1rc0/instill/helpers/const.py` & `instill_sdk-0.9.0rc0/instill/helpers/const.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/helpers/protobufs/parse.py` & `instill_sdk-0.9.0rc0/instill/helpers/protobufs/parse.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/helpers/protobufs/ray_pb2.py` & `instill_sdk-0.9.0rc0/instill/helpers/protobufs/ray_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/helpers/protobufs/ray_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/helpers/protobufs/ray_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/helpers/protobufs/ray_pb2_grpc.py` & `instill_sdk-0.9.0rc0/instill/helpers/protobufs/ray_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/helpers/push.py` & `instill_sdk-0.9.0rc0/instill/helpers/push.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 import argparse
 import subprocess
 
 import yaml
 
 from instill.utils.logger import Logger
 
-if __name__ == "__main__":
-    Logger.i("[Instill Builder] Setup docker...")
 
+def push_image():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-u",
         "--url",
         help="image registry url, in the format of host:port, default to docker.io",
         default="docker.io",
         required=False,
     )
+    parser.add_argument(
+        "-t",
+        "--tag",
+        help="tag for the model image",
+        required=True,
+    )
 
     try:
         args = parser.parse_args()
 
         Logger.i("[Instill Builder] Loading config file...")
         with open("instill.yaml", "r", encoding="utf8") as f:
             Logger.i("[Instill Builder] Parsing config file...")
             config = yaml.safe_load(f)
 
         registry = args.url
         repo = config["repo"]
-        tag = config["tag"]
 
         subprocess.run(
-            ["docker", "tag", f"{repo}:{tag}", f"{registry}/{repo}:{tag}"], check=True
+            ["docker", "tag", f"{repo}:{args.tag}", f"{registry}/{repo}:{args.tag}"],
+            check=True,
         )
         Logger.i("[Instill Builder] Pushing model image...")
-        subprocess.run(["docker", "push", f"{registry}/{repo}:{tag}"], check=True)
-        Logger.i(f"[Instill Builder] {registry}/{repo}:{tag} pushed")
-    except subprocess.CalledProcessError as e:
+        subprocess.run(["docker", "push", f"{registry}/{repo}:{args.tag}"], check=True)
+        Logger.i(f"[Instill Builder] {registry}/{repo}:{args.tag} pushed")
+    except subprocess.CalledProcessError:
         Logger.e("[Instill Builder] Push failed")
     except Exception as e:
         Logger.e("[Instill Builder] Prepare failed")
         Logger.e(e)
     finally:
         Logger.i("[Instill Builder] Done")
+
+
+if __name__ == "__main__":
+    push_image()
```

### Comparing `instill_sdk-0.8.1rc0/instill/helpers/ray_config.py` & `instill_sdk-0.9.0rc0/instill/helpers/ray_config.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/helpers/ray_io.py` & `instill_sdk-0.9.0rc0/instill/helpers/ray_io.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/helpers/utils.py` & `instill_sdk-0.9.0rc0/instill/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/.github/workflows/releases.yml` & `instill_sdk-0.9.0rc0/instill/protogen/.github/workflows/releases.yml`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/CHANGELOG.md` & `instill_sdk-0.9.0rc0/instill/protogen/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/LICENSE` & `instill_sdk-0.9.0rc0/instill/protogen/LICENSE`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/artifact/artifact/v1alpha/artifact_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/artifact/artifact/v1alpha/artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/artifact/artifact/v1alpha/artifact_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/artifact/artifact/v1alpha/artifact_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2_grpc.py` & `instill_sdk-0.9.0rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2_grpc.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/artifact/artifact/v1alpha/artifact_public_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/common/healthcheck/v1beta/healthcheck_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/common/healthcheck/v1beta/healthcheck_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/common/healthcheck/v1beta/healthcheck_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/common/healthcheck/v1beta/healthcheck_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/common/task/v1alpha/task_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/common/task/v1alpha/task_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/common/task/v1alpha/task_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/common/task/v1alpha/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/metric/v1beta/metric_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/core/metric/v1beta/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/metric/v1beta/metric_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/core/metric/v1beta/metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/metric/v1beta/metric_service_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/core/metric/v1beta/metric_service_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/metric/v1beta/metric_service_pb2_grpc.py` & `instill_sdk-0.9.0rc0/instill/protogen/core/metric/v1beta/metric_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/metric/v1beta/metric_service_pb2_grpc.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/core/metric/v1beta/metric_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/metric_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/metric_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2_grpc.py` & `instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2_grpc.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_private_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2_grpc.py` & `instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2_grpc.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/core/mgmt/v1beta/mgmt_public_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/usage/v1beta/usage_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/core/usage/v1beta/usage_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/usage/v1beta/usage_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/core/usage/v1beta/usage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/usage/v1beta/usage_service_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/core/usage/v1beta/usage_service_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/usage/v1beta/usage_service_pb2_grpc.py` & `instill_sdk-0.9.0rc0/instill/protogen/core/usage/v1beta/usage_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/core/usage/v1beta/usage_service_pb2_grpc.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/core/usage/v1beta/usage_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/controller/v1alpha/controller_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/controller/v1alpha/controller_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/controller/v1alpha/controller_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/controller/v1alpha/controller_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2_grpc.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2_grpc.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/controller/v1alpha/controller_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/common_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/common_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/common_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_definition_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_definition_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_definition_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2_grpc.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2_grpc.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_private_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2_grpc.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2_grpc.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/model_public_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_classification_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_classification_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_classification_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_classification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_detection_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_detection_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_detection_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_detection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_image_to_image_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_image_to_image_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_image_to_image_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_image_to_image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_instance_segmentation_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_instance_segmentation_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_instance_segmentation_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_instance_segmentation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_keypoint_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_keypoint_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_keypoint_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_keypoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_ocr_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_ocr_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_ocr_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_ocr_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_semantic_segmentation_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_semantic_segmentation_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_semantic_segmentation_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_semantic_segmentation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_generation_chat_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_generation_chat_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_generation_chat_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_generation_chat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_generation_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_generation_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_generation_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_generation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_to_image_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_to_image_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_text_to_image_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_text_to_image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_unspecified_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_unspecified_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_unspecified_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_unspecified_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_visual_question_answering_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_visual_question_answering_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/model/model/v1alpha/task_visual_question_answering_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/model/model/v1alpha/task_visual_question_answering_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/common_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/common_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/common_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/connector_definition_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/connector_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/connector_definition_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/connector_definition_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/connector_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/connector_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/connector_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/connector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/operator_definition_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/operator_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/operator_definition_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/operator_definition_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_pb2.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_pb2.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2_grpc.py` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2_grpc.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_private_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2.py` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2_grpc.py` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2_grpc.pyi` & `instill_sdk-0.9.0rc0/instill/protogen/vdp/pipeline/v1beta/pipeline_public_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/__init__.py` & `instill_sdk-0.9.0rc0/instill/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/connector.py` & `instill_sdk-0.9.0rc0/instill/resources/connector.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/connector_ai.py` & `instill_sdk-0.9.0rc0/instill/resources/connector_ai.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/connector_airbyte.py` & `instill_sdk-0.9.0rc0/instill/resources/connector_airbyte.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/connector_blockchain.py` & `instill_sdk-0.9.0rc0/instill/resources/connector_blockchain.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/connector_data.py` & `instill_sdk-0.9.0rc0/instill/resources/connector_data.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/model.py` & `instill_sdk-0.9.0rc0/instill/resources/model.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/operator.py` & `instill_sdk-0.9.0rc0/instill/resources/operator.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/pipeline.py` & `instill_sdk-0.9.0rc0/instill/resources/pipeline.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/resource.py` & `instill_sdk-0.9.0rc0/instill/resources/resource.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/airbyte/__init__.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/airbyte/__init__.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/helper.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/helper.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_conversational_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_conversational_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_summarization_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_summarization_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_text_generation_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_text_generation_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_text_to_image_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_text_to_image_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_token_classification_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_token_classification_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/huggingface_task_zero_shot_classification_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/huggingface_task_zero_shot_classification_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/image_task_draw_keypoint_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/image_task_draw_keypoint_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_text_generation_chat_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_text_generation_chat_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_text_generation_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_text_generation_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/instill_task_visual_question_answering_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/instill_task_visual_question_answering_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/airbyte_definitions.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/airbyte_definitions.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/airbyte_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/airbyte_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/base64_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/base64_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/bigquery_definitions.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/bigquery_definitions.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/bigquery_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/bigquery_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/component.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/component.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/end_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/end_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlecloudstorage_definitions.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlecloudstorage_definitions.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlecloudstorage_task_upload_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlecloudstorage_task_upload_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlecloudstorage_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlecloudstorage_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlesearch_definitions.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlesearch_definitions.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlesearch_task_search_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlesearch_task_search_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlesearch_task_search_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlesearch_task_search_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/googlesearch_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/googlesearch_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_definitions.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_definitions.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_audio_classification_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_audio_classification_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_conversational_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_conversational_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_conversational_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_conversational_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_fill_mask_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_fill_mask_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_fill_mask_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_fill_mask_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_image_classification_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_image_classification_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_image_segmentation_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_image_segmentation_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_object_detection_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_object_detection_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_question_answering_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_question_answering_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_question_answering_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_question_answering_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_sentence_similarity_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_sentence_similarity_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_summarization_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_summarization_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_table_question_answering_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_table_question_answering_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_table_question_answering_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_table_question_answering_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_text_classification_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_text_classification_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_text_classification_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_text_classification_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_text_generation_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_text_generation_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_text_to_image_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_text_to_image_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_token_classification_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_token_classification_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_token_classification_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_token_classification_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_translation_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_translation_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_zero_shot_classification_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_zero_shot_classification_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_task_zero_shot_classification_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_task_zero_shot_classification_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/huggingface_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/huggingface_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_definitions.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_definitions.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_classification_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_classification_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_detection_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_detection_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_instance_segmentation_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_instance_segmentation_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_keypoint_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_keypoint_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_ocr_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_ocr_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_task_draw_semantic_segmentation_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_task_draw_semantic_segmentation_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/image_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/image_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_definitions.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_definitions.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_classification_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_classification_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_detection_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_detection_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_detection_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_detection_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_image_to_image_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_image_to_image_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_instance_segmentation_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_instance_segmentation_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_instance_segmentation_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_instance_segmentation_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_keypoint_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_keypoint_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_keypoint_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_keypoint_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_ocr_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_ocr_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_ocr_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_ocr_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_semantic_segmentation_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_semantic_segmentation_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_semantic_segmentation_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_semantic_segmentation_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_text_generation_chat_$ref.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_text_generation_chat_$ref.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_text_generation_chat_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_text_generation_chat_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_text_generation_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_text_generation_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_text_to_image_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_text_to_image_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_visual_question_answering_$ref.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_visual_question_answering_$ref.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_task_visual_question_answering_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_task_visual_question_answering_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/instill_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/instill_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/json_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/json_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/numbers_definitions.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/numbers_definitions.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/numbers_task_commit_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/numbers_task_commit_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/numbers_task_register_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/numbers_task_register_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/numbers_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/numbers_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_definitions.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_definitions.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_speech_recognition_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_speech_recognition_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_text_embeddings_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_text_embeddings_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_text_generation_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_text_generation_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_text_to_image_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_text_to_image_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_task_text_to_speech_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_task_text_to_speech_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/openai_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/openai_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/pinecone_definitions.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/pinecone_definitions.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/pinecone_task_query_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/pinecone_task_query_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/pinecone_task_query_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/pinecone_task_query_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/pinecone_task_upsert_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/pinecone_task_upsert_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/pinecone_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/pinecone_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_definitions.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_definitions.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_task_chat_history_retrieve_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_task_chat_history_retrieve_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_task_chat_history_retrieve_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_task_chat_history_retrieve_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_task_chat_message_write_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_task_chat_message_write_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_task_chat_message_write_multi_modal_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_task_chat_message_write_multi_modal_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/redis_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/redis_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_definitions.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_definitions.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_delete_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_delete_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_delete_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_delete_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_get_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_get_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_get_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_get_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_head_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_head_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_head_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_head_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_options_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_options_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_options_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_options_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_patch_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_patch_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_patch_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_patch_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_post_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_post_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_post_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_post_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_put_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_put_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_task_put_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_task_put_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/restapi_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/restapi_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/stabilityai.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/stabilityai.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/stabilityai_task_image_to_image_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/stabilityai_task_image_to_image_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/stabilityai_task_image_to_image_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/stabilityai_task_image_to_image_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/stabilityai_task_text_to_image_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/stabilityai_task_text_to_image_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/stabilityai_task_text_to_image_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/stabilityai_task_text_to_image_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/stabilityai_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/stabilityai_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/start_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/start_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/text_task_convert_to_text_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/text_task_convert_to_text_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/text_task_split_by_token_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/text_task_split_by_token_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/text_task_split_by_token_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/text_task_split_by_token_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/text_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/text_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/website_task_scrape_website_input.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/website_task_scrape_website_input.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/website_task_scrape_website_output.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/website_task_scrape_website_output.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/jsons/website_tasks.json` & `instill_sdk-0.9.0rc0/instill/resources/schema/jsons/website_tasks.json`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/numbers_task_commit_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/numbers_task_commit_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/numbers_task_register_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/numbers_task_register_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/openai_task_text_generation_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/openai_task_text_generation_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/openai_task_text_to_image_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/openai_task_text_to_image_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/openai_task_text_to_speech_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/openai_task_text_to_speech_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/redis.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/redis.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/redis_task_chat_history_retrieve_output.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/redis_task_chat_history_retrieve_output.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/redis_task_chat_message_write_multi_modal_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/redis_task_chat_message_write_multi_modal_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/restapi.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/restapi.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/stabilityai_task_image_to_image_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/stabilityai_task_image_to_image_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/stabilityai_task_text_to_image_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/stabilityai_task_text_to_image_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/resources/schema/text_task_split_by_token_input.py` & `instill_sdk-0.9.0rc0/instill/resources/schema/text_task_split_by_token_input.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/tests/test_client.py` & `instill_sdk-0.9.0rc0/instill/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/utils/error_handler.py` & `instill_sdk-0.9.0rc0/instill/utils/error_handler.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/instill/utils/logger.py` & `instill_sdk-0.9.0rc0/instill/utils/logger.py`

 * *Files identical despite different names*

### Comparing `instill_sdk-0.8.1rc0/pyproject.toml` & `instill_sdk-0.9.0rc0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 
 name = "instill-sdk"
-version = "0.8.1rc0"
+version = "0.9.0rc0"
 description = "python sdk for Instill AI products"
 
 packages = [{ include = "instill" }]
 
 license = "MIT"
 authors = ["instill-ai <drop@instill.tech>"]
 
 readme = "README.md"
 homepage = "https://pypi.org/project/instill-sdk"
 documentation = "https://instill-sdk.readthedocs.io"
 repository = "https://github.com/instill-ai/python-sdk"
 
+maintainers = ["Heiru Wu <heiru.wu@instill.tech>"]
+
 keywords = []
 classifiers = [
   "Development Status :: 1 - Planning",
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
@@ -33,15 +35,15 @@
 types-protobuf = "^4.24.0.1"
 types-pyyaml = "^6.0.12.11"
 google-api-core = "^2.11.1"
 googleapis-common-protos = "^1.60.0"
 protoc-gen-openapiv2 = "^0.0.1"
 pydantic = ">=1.10.13"
 pillow = "^10.1.0"
-ray = {version = "2.9.3", extras = ["serve"]}
+ray = { version = "2.9.3", extras = ["serve"] }
 jsonschema = "^4.20.0"
 
 [tool.poetry.dev-dependencies]
 
 # Formatters
 black = "^24.3"
 tomli = "*"     # missing 'black' dependency
@@ -80,16 +82,16 @@
 datamodel-code-generator = "^0.25.2"
 jsonref = "^1.1.0"
 
 # Publish
 twine = "^4.0.2"
 
 [tool.poetry.scripts]
-
-# python-sdk = "instill.cli:main"
+instill_build = "instill.helpers.build:build_image"
+instill_push = "instill.helpers.push:push_image"
 
 [tool.black]
 
 quiet = true
 exclude = '''
 (
   /(
@@ -114,17 +116,15 @@
 
 [tool.isort]
 
 profile = "black"
 skip_glob = ["**/protogen/*", "**/protobufs/*"]
 
 [tool.mypy]
-exclude = [
-    'instill/resources/schema',
-]
+exclude = ['instill/resources/schema']
 ignore_missing_imports = true
 no_implicit_optional = true
 check_untyped_defs = true
 
 cache_dir = ".cache/mypy/"
 
 [tool.pytest.ini_options]
```

### Comparing `instill_sdk-0.8.1rc0/PKG-INFO` & `instill_sdk-0.9.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: instill-sdk
-Version: 0.8.1rc0
+Version: 0.9.0rc0
 Summary: python sdk for Instill AI products
 Home-page: https://pypi.org/project/instill-sdk
 License: MIT
 Author: instill-ai
 Author-email: drop@instill.tech
+Maintainer: Heiru Wu
+Maintainer-email: heiru.wu@instill.tech
 Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

