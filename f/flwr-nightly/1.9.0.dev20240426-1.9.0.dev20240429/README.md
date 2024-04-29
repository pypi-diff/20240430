# Comparing `tmp/flwr_nightly-1.9.0.dev20240426.tar.gz` & `tmp/flwr_nightly-1.9.0.dev20240429.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.9.0.dev20240426.tar", max compression
+gzip compressed data, was "flwr_nightly-1.9.0.dev20240429.tar", max compression
```

## Comparing `flwr_nightly-1.9.0.dev20240426.tar` & `flwr_nightly-1.9.0.dev20240429.tar`

### file list

```diff
@@ -1,215 +1,216 @@
--rw-r--r--   0        0        0    11358 2024-04-26 23:05:32.112046 flwr_nightly-1.9.0.dev20240426/LICENSE
--rw-r--r--   0        0        0    12916 2024-04-26 23:05:32.112046 flwr_nightly-1.9.0.dev20240426/README.md
--rw-r--r--   0        0        0     5776 2024-04-26 23:05:44.383988 flwr_nightly-1.9.0.dev20240426/pyproject.toml
--rw-r--r--   0        0        0      937 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     4899 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/config_utils.py
--rw-r--r--   0        0        0     2215 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0      789 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     5989 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0     3078 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/.gitignore.tpl
--rw-r--r--   0        0        0      667 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0      521 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1172 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0     2801 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
--rw-r--r--   0        0        0     1911 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      248 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      593 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0      341 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
--rw-r--r--   0        0        0      371 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     3684 2024-04-26 23:05:32.528044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0      521 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      590 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      570 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
--rw-r--r--   0        0        0      569 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0      789 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2334 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     4119 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1262 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    24670 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8636 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8993 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     4761 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/grpc_rere_client/client_interceptor.py
--rw-r--r--   0        0        0     9597 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0     2404 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/heartbeat.py
--rw-r--r--   0        0        0      719 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5397 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2623 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     4918 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    11520 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0      793 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/supernode/__init__.py
--rw-r--r--   0        0        0     3861 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/supernode/app.py
--rw-r--r--   0        0        0     1006 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     2424 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2460 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     6096 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    12385 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-04-26 23:05:32.532044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4849 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     4553 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    13798 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    11707 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     4173 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7865 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3207 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     5016 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     5018 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     9161 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0    10605 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2811 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1785 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    24199 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     5287 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3468 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     5444 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      862 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     5090 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0    11832 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/driver/grpc_driver.py
--rw-r--r--   0        0        0     5121 2024-04-26 23:05:32.536044 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5972 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17664 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4402 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17458 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12904 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4796 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11818 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3387 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      731 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3622 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     7621 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6375 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    12454 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0    11651 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    27167 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     7709 2024-04-26 23:05:32.540043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0     2207 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/state/utils.py
--rw-r--r--   0        0        0      913 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    12547 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29038 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1400 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    13904 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    19367 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    15694 2024-04-26 23:05:32.544043 flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15260 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240426/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-29 23:05:13.919324 flwr_nightly-1.9.0.dev20240429/LICENSE
+-rw-r--r--   0        0        0    12916 2024-04-29 23:05:13.919324 flwr_nightly-1.9.0.dev20240429/README.md
+-rw-r--r--   0        0        0     5776 2024-04-29 23:05:30.539412 flwr_nightly-1.9.0.dev20240429/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     4899 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/config_utils.py
+-rw-r--r--   0        0        0     2215 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0      789 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     5989 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0     3078 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/.gitignore.tpl
+-rw-r--r--   0        0        0      667 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0      521 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1172 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0     2801 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
+-rw-r--r--   0        0        0     1911 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      248 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      593 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0      341 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
+-rw-r--r--   0        0        0      371 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     3684 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0      521 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      590 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      570 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
+-rw-r--r--   0        0        0      569 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0      789 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2334 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     4119 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1268 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    22313 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-04-29 23:05:14.335326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8993 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     4761 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_rere_client/client_interceptor.py
+-rw-r--r--   0        0        0     9597 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2404 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5397 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2623 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     4918 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    11520 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0      865 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/supernode/__init__.py
+-rw-r--r--   0        0        0     9052 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/supernode/app.py
+-rw-r--r--   0        0        0     1006 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2460 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     6096 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    12385 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4849 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     4553 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    13798 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11707 2024-04-29 23:05:14.339326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     4707 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7865 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3207 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     5016 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5018 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     9161 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0    10605 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2811 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1785 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    28282 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     5287 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3468 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     5444 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      862 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     5090 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0    11832 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     5121 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5972 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17664 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-04-29 23:05:14.343326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17458 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12904 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4796 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11932 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3387 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0     5799 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py
+-rw-r--r--   0        0        0      731 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3622 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     7621 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6375 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12454 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0    11651 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    27167 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     7709 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-04-29 23:05:14.347326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    12547 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1400 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    13904 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15694 2024-04-29 23:05:14.351326 flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15260 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240429/PKG-INFO
```

### Comparing `flwr_nightly-1.9.0.dev20240426/LICENSE` & `flwr_nightly-1.9.0.dev20240429/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/README.md` & `flwr_nightly-1.9.0.dev20240429/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/pyproject.toml` & `flwr_nightly-1.9.0.dev20240429/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.9.0.dev20240426"
+version = "1.9.0.dev20240429"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
```

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/app.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/config_utils.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/example.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/new.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/.gitignore.tpl` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/.gitignore.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/run/run.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/cli/utils.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/cli/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower client."""
 
 
-from .app import run_client_app as run_client_app
 from .app import start_client as start_client
 from .app import start_numpy_client as start_numpy_client
 from .client import Client as Client
 from .client_app import ClientApp as ClientApp
 from .numpy_client import NumPyClient as NumPyClient
+from .supernode import run_client_app as run_client_app
 from .supernode import run_supernode as run_supernode
 from .typing import ClientFn as ClientFn
 
 __all__ = [
     "Client",
     "ClientApp",
     "ClientFn",
```

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/app.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower client app."""
 
-import argparse
 import sys
 import time
 from logging import DEBUG, ERROR, INFO, WARN
-from pathlib import Path
 from typing import Callable, ContextManager, Optional, Tuple, Type, Union
 
+from cryptography.hazmat.primitives.asymmetric import ec
 from grpc import RpcError
 
 from flwr.client.client import Client
 from flwr.client.client_app import ClientApp, LoadClientAppError
 from flwr.client.typing import ClientFn
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH, EventType, Message, event
 from flwr.common.address import parse_address
@@ -32,113 +31,23 @@
     MISSING_EXTRA_REST,
     TRANSPORT_TYPE_GRPC_BIDI,
     TRANSPORT_TYPE_GRPC_RERE,
     TRANSPORT_TYPE_REST,
     TRANSPORT_TYPES,
     ErrorCode,
 )
-from flwr.common.exit_handlers import register_exit_handlers
 from flwr.common.logger import log, warn_deprecated_feature
 from flwr.common.message import Error
-from flwr.common.object_ref import load_app, validate
 from flwr.common.retry_invoker import RetryInvoker, exponential
 
 from .grpc_client.connection import grpc_connection
 from .grpc_rere_client.connection import grpc_request_response
 from .message_handler.message_handler import handle_control_message
 from .node_state import NodeState
 from .numpy_client import NumPyClient
-from .supernode.app import parse_args_run_client_app
-
-
-def run_client_app() -> None:
-    """Run Flower client app."""
-    log(INFO, "Long-running Flower client starting")
-
-    event(EventType.RUN_CLIENT_APP_ENTER)
-
-    args = _parse_args_run_client_app().parse_args()
-
-    # Obtain certificates
-    if args.insecure:
-        if args.root_certificates is not None:
-            sys.exit(
-                "Conflicting options: The '--insecure' flag disables HTTPS, "
-                "but '--root-certificates' was also specified. Please remove "
-                "the '--root-certificates' option when running in insecure mode, "
-                "or omit '--insecure' to use HTTPS."
-            )
-        log(
-            WARN,
-            "Option `--insecure` was set. "
-            "Starting insecure HTTP client connected to %s.",
-            args.server,
-        )
-        root_certificates = None
-    else:
-        # Load the certificates if provided, or load the system certificates
-        cert_path = args.root_certificates
-        if cert_path is None:
-            root_certificates = None
-        else:
-            root_certificates = Path(cert_path).read_bytes()
-        log(
-            DEBUG,
-            "Starting secure HTTPS client connected to %s "
-            "with the following certificates: %s.",
-            args.server,
-            cert_path,
-        )
-
-    log(
-        DEBUG,
-        "Flower will load ClientApp `%s`",
-        getattr(args, "client-app"),
-    )
-
-    client_app_dir = args.dir
-    if client_app_dir is not None:
-        sys.path.insert(0, client_app_dir)
-
-    app_ref: str = getattr(args, "client-app")
-    valid, error_msg = validate(app_ref)
-    if not valid and error_msg:
-        raise LoadClientAppError(error_msg) from None
-
-    def _load() -> ClientApp:
-        client_app = load_app(app_ref, LoadClientAppError)
-
-        if not isinstance(client_app, ClientApp):
-            raise LoadClientAppError(
-                f"Attribute {app_ref} is not of type {ClientApp}",
-            ) from None
-
-        return client_app
-
-    _start_client_internal(
-        server_address=args.server,
-        load_client_app_fn=_load,
-        transport="rest" if args.rest else "grpc-rere",
-        root_certificates=root_certificates,
-        insecure=args.insecure,
-        max_retries=args.max_retries,
-        max_wait_time=args.max_wait_time,
-    )
-    register_exit_handlers(event_type=EventType.RUN_CLIENT_APP_LEAVE)
-
-
-def _parse_args_run_client_app() -> argparse.ArgumentParser:
-    """Parse flower-client-app command line arguments."""
-    parser = argparse.ArgumentParser(
-        description="Start a Flower client app",
-    )
-
-    parse_args_run_client_app(parser=parser)
-
-    return parser
 
 
 def _check_actionable_client(
     client: Optional[Client], client_fn: Optional[ClientFn]
 ) -> None:
     if client_fn is None and client is None:
         raise ValueError(
@@ -161,14 +70,17 @@
     server_address: str,
     client_fn: Optional[ClientFn] = None,
     client: Optional[Client] = None,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[Union[bytes, str]] = None,
     insecure: Optional[bool] = None,
     transport: Optional[str] = None,
+    authentication_keys: Optional[
+        Tuple[ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey]
+    ] = None,
     max_retries: Optional[int] = None,
     max_wait_time: Optional[float] = None,
 ) -> None:
     """Start a Flower client node which connects to a Flower server.
 
     Parameters
     ----------
@@ -245,14 +157,15 @@
         load_client_app_fn=None,
         client_fn=client_fn,
         client=client,
         grpc_max_message_length=grpc_max_message_length,
         root_certificates=root_certificates,
         insecure=insecure,
         transport=transport,
+        authentication_keys=authentication_keys,
         max_retries=max_retries,
         max_wait_time=max_wait_time,
     )
     event(EventType.START_CLIENT_LEAVE)
 
 
 # pylint: disable=import-outside-toplevel
@@ -265,14 +178,17 @@
     load_client_app_fn: Optional[Callable[[], ClientApp]] = None,
     client_fn: Optional[ClientFn] = None,
     client: Optional[Client] = None,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[Union[bytes, str]] = None,
     insecure: Optional[bool] = None,
     transport: Optional[str] = None,
+    authentication_keys: Optional[
+        Tuple[ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey]
+    ] = None,
     max_retries: Optional[int] = None,
     max_wait_time: Optional[float] = None,
 ) -> None:
     """Start a Flower client node which connects to a Flower server.
 
     Parameters
     ----------
@@ -389,14 +305,15 @@
         sleep_duration: int = 0
         with connection(
             address,
             insecure,
             retry_invoker,
             grpc_max_message_length,
             root_certificates,
+            authentication_keys,
         ) as conn:
             # pylint: disable-next=W0612
             receive, send, create_node, delete_node, get_run = conn
 
             # Register node
             if create_node is not None:
                 create_node()  # pylint: disable=not-callable
@@ -602,15 +519,22 @@
         insecure=insecure,
         transport=transport,
     )
 
 
 def _init_connection(transport: Optional[str], server_address: str) -> Tuple[
     Callable[
-        [str, bool, RetryInvoker, int, Union[bytes, str, None]],
+        [
+            str,
+            bool,
+            RetryInvoker,
+            int,
+            Union[bytes, str, None],
+            Optional[Tuple[ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey]],
+        ],
         ContextManager[
             Tuple[
                 Callable[[], Optional[Message]],
                 Callable[[Message], None],
                 Optional[Callable[[], None]],
                 Optional[Callable[[], None]],
                 Optional[Callable[[int], Tuple[str, str]]],
```

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/client.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/client_app.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/client_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/grpc_rere_client/client_interceptor.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_rere_client/client_interceptor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/heartbeat.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/heartbeat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/localdp_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/node_state.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/supernode/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower SuperNode."""
-
-
-from .app import run_supernode as run_supernode
-
-__all__ = [
-    "run_supernode",
-]
+"""Flower SuperLink."""
```

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/client/typing.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/address.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/constant.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/context.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/date.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/dp.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/grpc.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/logger.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/message.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/message.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/parameter.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/recordset.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/recordset_compat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/retry_invoker.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files 18% similar despite different names*

```diff
@@ -113,7 +113,22 @@
     computed_hmac = hmac.HMAC(key, hashes.SHA256())
     computed_hmac.update(message)
     try:
         computed_hmac.verify(hmac_value)
         return True
     except InvalidSignature:
         return False
+
+
+def ssh_types_to_elliptic_curve(
+    private_key: serialization.SSHPrivateKeyTypes,
+    public_key: serialization.SSHPublicKeyTypes,
+) -> Tuple[ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey]:
+    """Cast SSH key types to elliptic curve."""
+    if isinstance(private_key, ec.EllipticCurvePrivateKey) and isinstance(
+        public_key, ec.EllipticCurvePublicKey
+    ):
+        return (private_key, public_key)
+
+    raise TypeError(
+        "The provided key is not an EllipticCurvePrivateKey or EllipticCurvePublicKey"
+    )
```

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/serde.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/typing.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/common/version.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/app.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,34 +12,44 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower server app."""
 
 import argparse
 import asyncio
+import csv
 import importlib.util
 import sys
 import threading
 from logging import ERROR, INFO, WARN
 from os.path import isfile
 from pathlib import Path
-from typing import List, Optional, Tuple
+from typing import List, Optional, Sequence, Set, Tuple
 
 import grpc
+from cryptography.hazmat.primitives.asymmetric import ec
+from cryptography.hazmat.primitives.serialization import (
+    load_ssh_private_key,
+    load_ssh_public_key,
+)
 
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH, EventType, event
 from flwr.common.address import parse_address
 from flwr.common.constant import (
     MISSING_EXTRA_REST,
     TRANSPORT_TYPE_GRPC_RERE,
     TRANSPORT_TYPE_REST,
     TRANSPORT_TYPE_VCE,
 )
 from flwr.common.exit_handlers import register_exit_handlers
 from flwr.common.logger import log
+from flwr.common.secure_aggregation.crypto.symmetric_encryption import (
+    public_key_to_bytes,
+    ssh_types_to_elliptic_curve,
+)
 from flwr.proto.fleet_pb2_grpc import (  # pylint: disable=E0611
     add_FleetServicer_to_server,
 )
 
 from .client_manager import ClientManager
 from .history import History
 from .server import Server, init_defaults, run_fl
@@ -47,14 +57,15 @@
 from .strategy import Strategy
 from .superlink.driver.driver_grpc import run_driver_api_grpc
 from .superlink.fleet.grpc_bidi.grpc_server import (
     generic_create_grpc_server,
     start_grpc_server,
 )
 from .superlink.fleet.grpc_rere.fleet_servicer import FleetServicer
+from .superlink.fleet.grpc_rere.server_interceptor import AuthenticateServerInterceptor
 from .superlink.fleet.vce import start_vce
 from .superlink.state import StateFactory
 
 ADDRESS_DRIVER_API = "0.0.0.0:9091"
 ADDRESS_FLEET_API_GRPC_RERE = "0.0.0.0:9092"
 ADDRESS_FLEET_API_GRPC_BIDI = "[::]:8080"  # IPv6 to keep start_server compatible
 ADDRESS_FLEET_API_REST = "0.0.0.0:9093"
@@ -350,18 +361,36 @@
     elif args.fleet_api_type == TRANSPORT_TYPE_GRPC_RERE:
         address_arg = args.grpc_rere_fleet_api_address
         parsed_address = parse_address(address_arg)
         if not parsed_address:
             sys.exit(f"Fleet IP address ({address_arg}) cannot be parsed.")
         host, port, is_v6 = parsed_address
         address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
+
+        maybe_keys = _try_setup_client_authentication(args, certificates)
+        interceptors: Optional[Sequence[grpc.ServerInterceptor]] = None
+        if maybe_keys is not None:
+            (
+                client_public_keys,
+                server_private_key,
+                server_public_key,
+            ) = maybe_keys
+            interceptors = [
+                AuthenticateServerInterceptor(
+                    client_public_keys,
+                    server_private_key,
+                    server_public_key,
+                )
+            ]
+
         fleet_server = _run_fleet_api_grpc_rere(
             address=address,
             state_factory=state_factory,
             certificates=certificates,
+            interceptors=interceptors,
         )
         grpc_servers.append(fleet_server)
     elif args.fleet_api_type == TRANSPORT_TYPE_VCE:
         f_stop = asyncio.Event()  # Does nothing
         _run_fleet_api_vce(
             num_supernodes=args.num_supernodes,
             client_app_attr=args.client_app,
@@ -386,14 +415,78 @@
         if bckg_threads:
             for thread in bckg_threads:
                 if not thread.is_alive():
                     sys.exit(1)
         driver_server.wait_for_termination(timeout=1)
 
 
+def _try_setup_client_authentication(
+    args: argparse.Namespace,
+    certificates: Optional[Tuple[bytes, bytes, bytes]],
+) -> Optional[Tuple[Set[bytes], ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey]]:
+    if not args.require_client_authentication:
+        return None
+
+    if certificates is None:
+        sys.exit(
+            "Client authentication only works over secure connections. "
+            "Please provide certificate paths using '--certificates' when "
+            "enabling '--require-client-authentication'."
+        )
+
+    client_keys_file_path = Path(args.require_client_authentication[0])
+    if not client_keys_file_path.exists():
+        sys.exit(
+            "The provided path to the client public keys CSV file does not exist: "
+            f"{client_keys_file_path}. "
+            "Please provide the CSV file path containing known client public keys "
+            "to '--require-client-authentication'."
+        )
+
+    client_public_keys: Set[bytes] = set()
+    ssh_private_key = load_ssh_private_key(
+        Path(args.require_client_authentication[1]).read_bytes(),
+        None,
+    )
+    ssh_public_key = load_ssh_public_key(
+        Path(args.require_client_authentication[2]).read_bytes()
+    )
+
+    try:
+        server_private_key, server_public_key = ssh_types_to_elliptic_curve(
+            ssh_private_key, ssh_public_key
+        )
+    except TypeError:
+        sys.exit(
+            "The file paths provided could not be read as a private and public "
+            "key pair. Client authentication requires an elliptic curve public and "
+            "private key pair. Please provide the file paths containing elliptic "
+            "curve private and public keys to '--require-client-authentication'."
+        )
+
+    with open(client_keys_file_path, newline="", encoding="utf-8") as csvfile:
+        reader = csv.reader(csvfile)
+        for row in reader:
+            for element in row:
+                public_key = load_ssh_public_key(element.encode())
+                if isinstance(public_key, ec.EllipticCurvePublicKey):
+                    client_public_keys.add(public_key_to_bytes(public_key))
+                else:
+                    sys.exit(
+                        "Error: Unable to parse the public keys in the .csv "
+                        "file. Please ensure that the .csv file contains valid "
+                        "SSH public keys and try again."
+                    )
+        return (
+            client_public_keys,
+            server_private_key,
+            server_public_key,
+        )
+
+
 def _try_obtain_certificates(
     args: argparse.Namespace,
 ) -> Optional[Tuple[bytes, bytes, bytes]]:
     # Obtain certificates
     if args.insecure:
         log(WARN, "Option `--insecure` was set. Starting insecure HTTP server.")
         certificates = None
@@ -413,26 +506,28 @@
     return certificates
 
 
 def _run_fleet_api_grpc_rere(
     address: str,
     state_factory: StateFactory,
     certificates: Optional[Tuple[bytes, bytes, bytes]],
+    interceptors: Optional[Sequence[grpc.ServerInterceptor]] = None,
 ) -> grpc.Server:
     """Run Fleet API (gRPC, request-response)."""
     # Create Fleet API gRPC server
     fleet_servicer = FleetServicer(
         state_factory=state_factory,
     )
     fleet_add_servicer_to_server_fn = add_FleetServicer_to_server
     fleet_grpc_server = generic_create_grpc_server(
         servicer_and_add_fn=(fleet_servicer, fleet_add_servicer_to_server_fn),
         server_address=address,
         max_message_length=GRPC_MAX_MESSAGE_LENGTH,
         certificates=certificates,
+        interceptors=interceptors,
     )
 
     log(INFO, "Flower ECE: Starting Fleet API (gRPC-rere) on %s", address)
     fleet_grpc_server.start()
 
     return fleet_grpc_server
 
@@ -602,14 +697,23 @@
         help="A string representing the path to the database "
         "file that will be opened. Note that passing ':memory:' "
         "will open a connection to a database that is in RAM, "
         "instead of on disk. If nothing is provided, "
         "Flower will just create a state in memory.",
         default=DATABASE,
     )
+    parser.add_argument(
+        "--require-client-authentication",
+        nargs=3,
+        metavar=("CLIENT_KEYS", "SERVER_PRIVATE_KEY", "SERVER_PUBLIC_KEY"),
+        type=str,
+        help="Provide three file paths: (1) a .csv file containing a list of "
+        "known client public keys for authentication, (2) the server's private "
+        "key file, and (3) the server's public key file.",
+    )
 
 
 def _add_args_driver_api(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "--driver-api-address",
         help="Driver API (gRPC) server address (IPv4, IPv6, or a domain name)",
         default=ADDRESS_DRIVER_API,
```

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/compat/app.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/app_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/criterion.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/driver/grpc_driver.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/driver/grpc_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/history.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/run_serverapp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/server.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/server_app.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/server_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/server_config.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Copyright 2024 Flower Labs GmbH. All Rights Reserved.
+# Copyright 2020 Flower Labs GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower SuperLink."""
+"""Ray-based Flower ClientProxy implementation."""
```

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 """Implements utility function to create a gRPC server."""
 
 
 import concurrent.futures
 import sys
 from logging import ERROR
-from typing import Any, Callable, Optional, Tuple, Union
+from typing import Any, Callable, Optional, Sequence, Tuple, Union
 
 import grpc
 
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH
 from flwr.common.logger import log
 from flwr.proto.transport_pb2_grpc import (  # pylint: disable=E0611
     add_FlowerServiceServicer_to_server,
@@ -158,14 +158,15 @@
         Tuple[DriverServicer, AddServicerToServerFn],
     ],
     server_address: str,
     max_concurrent_workers: int = 1000,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     keepalive_time_ms: int = 210000,
     certificates: Optional[Tuple[bytes, bytes, bytes]] = None,
+    interceptors: Optional[Sequence[grpc.ServerInterceptor]] = None,
 ) -> grpc.Server:
     """Create a gRPC server with a single servicer.
 
     Parameters
     ----------
     servicer_and_add_fn : Tuple
         A tuple holding a servicer implementation and a matching
@@ -245,14 +246,15 @@
 
     server = grpc.server(
         concurrent.futures.ThreadPoolExecutor(max_workers=max_concurrent_workers),
         # Set the maximum number of concurrent RPCs this server will service before
         # returning RESOURCE_EXHAUSTED status, or None to indicate no limit.
         maximum_concurrent_rpcs=max_concurrent_workers,
         options=options,
+        interceptors=interceptors,
     )
     add_servicer_to_server_fn(servicer, server)
 
     if certificates is not None:
         if not valid_certificates(certificates):
             sys.exit(1)
```

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/superlink/state/utils.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/superlink/state/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/typing.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/default_workflows.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/app.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/client/supernode/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,24 @@
-# Copyright 2020 Flower Labs GmbH. All Rights Reserved.
+# Copyright 2024 Flower Labs GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Ray-based Flower ClientProxy implementation."""
+"""Flower SuperNode."""
+
+
+from .app import run_client_app as run_client_app
+from .app import run_supernode as run_supernode
+
+__all__ = [
+    "run_client_app",
+    "run_supernode",
+]
```

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.9.0.dev20240429/src/py/flwr/simulation/run_simulation.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240426/PKG-INFO` & `flwr_nightly-1.9.0.dev20240429/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.9.0.dev20240426
+Version: 1.9.0.dev20240429
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.ai
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.ai
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240426 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240429 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

