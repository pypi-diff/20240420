# Comparing `tmp/flwr_nightly-1.9.0.dev20240417.tar.gz` & `tmp/flwr_nightly-1.9.0.dev20240418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.9.0.dev20240417.tar", max compression
+gzip compressed data, was "flwr_nightly-1.9.0.dev20240418.tar", max compression
```

## Comparing `flwr_nightly-1.9.0.dev20240417.tar` & `flwr_nightly-1.9.0.dev20240418.tar`

### file list

```diff
@@ -1,208 +1,210 @@
--rw-r--r--   0        0        0    11358 2024-04-17 23:05:25.511498 flwr_nightly-1.9.0.dev20240417/LICENSE
--rw-r--r--   0        0        0    12916 2024-04-17 23:05:25.511498 flwr_nightly-1.9.0.dev20240417/README.md
--rw-r--r--   0        0        0     5836 2024-04-17 23:05:39.379692 flwr_nightly-1.9.0.dev20240417/pyproject.toml
--rw-r--r--   0        0        0      937 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     4696 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/config_utils.py
--rw-r--r--   0        0        0     2215 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0      789 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     5240 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0      668 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0      521 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1173 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0       48 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      248 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      594 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0       48 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     3684 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0      489 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      558 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      537 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0      789 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2331 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     4153 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1187 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    26193 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8636 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8717 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     8560 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0     2404 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/heartbeat.py
--rw-r--r--   0        0        0      719 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5397 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2623 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     4918 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-04-17 23:05:25.927503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    14482 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     1006 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     2424 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2273 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     6096 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    12385 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4849 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     3016 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    13798 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    11707 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     3546 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7782 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3207 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     5016 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     5018 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     9161 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0    10605 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2811 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-04-17 23:05:25.931503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1785 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    24302 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     5271 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3496 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     7344 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      820 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0    10106 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0     4586 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/driver/grpc_driver.py
--rw-r--r--   0        0        0     5121 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5592 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17664 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4402 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17458 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12904 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4761 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11818 2024-04-17 23:05:25.935503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3387 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      731 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3473 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     7621 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6375 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    12454 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0     9586 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    23985 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     6058 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0     2207 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/state/utils.py
--rw-r--r--   0        0        0      913 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    12547 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29038 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1400 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    13904 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    19367 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    15685 2024-04-17 23:05:25.939503 flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15260 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240417/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-18 23:05:56.600567 flwr_nightly-1.9.0.dev20240418/LICENSE
+-rw-r--r--   0        0        0    12916 2024-04-18 23:05:56.600567 flwr_nightly-1.9.0.dev20240418/README.md
+-rw-r--r--   0        0        0     5836 2024-04-18 23:06:14.592406 flwr_nightly-1.9.0.dev20240418/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     4696 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/config_utils.py
+-rw-r--r--   0        0        0     2215 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0      789 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     5380 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0     3078 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/.gitignore.tpl
+-rw-r--r--   0        0        0      668 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0      521 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1173 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0       48 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      248 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      594 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0       48 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     3684 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0      489 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      558 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      537 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0      789 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2331 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     4153 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1187 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    26193 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8717 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     8560 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2404 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5397 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2623 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     4918 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    14456 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     1006 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2273 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     6096 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    12385 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4849 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     4553 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    13798 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11707 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     3546 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7782 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3207 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     5016 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5018 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     9161 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0    10605 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2811 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1785 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    24302 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     5271 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3496 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     7344 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      820 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     5090 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/abc_driver.py
+-rw-r--r--   0        0        0    10106 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0     4586 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     5121 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5592 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17664 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17458 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12904 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4780 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11818 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3387 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      731 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3473 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     7621 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6375 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12454 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0    10083 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    24580 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     6762 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    12547 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1400 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    13904 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15685 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15260 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240418/PKG-INFO
```

### Comparing `flwr_nightly-1.9.0.dev20240417/LICENSE` & `flwr_nightly-1.9.0.dev20240418/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/README.md` & `flwr_nightly-1.9.0.dev20240418/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/pyproject.toml` & `flwr_nightly-1.9.0.dev20240418/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.9.0.dev20240417"
+version = "1.9.0.dev20240418"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
```

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/app.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/config_utils.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/example.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/new.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,17 @@
         return tpl_file.read()
 
 
 def render_template(template: str, data: Dict[str, str]) -> str:
     """Render template."""
     tpl_file = load_template(template)
     tpl = Template(tpl_file)
-    result = tpl.substitute(data)
-    return result
+    if ".gitignore" not in template:
+        return tpl.substitute(data)
+    return tpl.template
 
 
 def create_file(file_path: str, content: str) -> None:
     """Create file including all nessecary directories and write content into file."""
     os.makedirs(os.path.dirname(file_path), exist_ok=True)
     with open(file_path, "w", encoding="utf-8") as f:
         f.write(content)
@@ -123,23 +124,27 @@
     # Set project directory path
     cwd = os.getcwd()
     pnl = project_name.lower()
     project_dir = os.path.join(cwd, pnl)
 
     # List of files to render
     files = {
+        ".gitignore": {"template": "app/.gitignore.tpl"},
         "README.md": {"template": "app/README.md.tpl"},
         "pyproject.toml": {"template": f"app/pyproject.{framework_str}.toml.tpl"},
         f"{pnl}/__init__.py": {"template": "app/code/__init__.py.tpl"},
         f"{pnl}/server.py": {"template": f"app/code/server.{framework_str}.py.tpl"},
         f"{pnl}/client.py": {"template": f"app/code/client.{framework_str}.py.tpl"},
     }
 
-    # In case framework is MlFramework.PYTORCH generate additionally the task.py file
-    if framework_str == MlFramework.PYTORCH.value.lower():
+    # Depending on the framework, generate task.py file
+    frameworks_with_tasks = [
+        MlFramework.PYTORCH.value.lower(),
+    ]
+    if framework_str in frameworks_with_tasks:
         files[f"{pnl}/task.py"] = {"template": f"app/code/task.{framework_str}.py.tpl"}
 
     context = {"project_name": project_name}
 
     for file_path, value in files.items():
         render_and_create(
             file_path=os.path.join(project_dir, file_path),
```

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/run/run.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/cli/utils.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/app.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/client.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/client_app.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/client_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/heartbeat.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/heartbeat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/localdp_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/node_state.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/rest_client/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,22 +169,22 @@
         # Check status code and headers
         if res.status_code != 200:
             return
         if "content-type" not in res.headers:
             log(
                 WARN,
                 "[Node] POST /%s: missing header `Content-Type`",
-                PATH_PULL_TASK_INS,
+                PATH_PING,
             )
             return
         if res.headers["content-type"] != "application/protobuf":
             log(
                 WARN,
                 "[Node] POST /%s: header `Content-Type` has wrong value",
-                PATH_PULL_TASK_INS,
+                PATH_PING,
             )
             return
 
         # Deserialize ProtoBuf from bytes
         ping_res = PingResponse()
         ping_res.ParseFromString(res.content)
 
@@ -219,22 +219,22 @@
         # Check status code and headers
         if res.status_code != 200:
             return
         if "content-type" not in res.headers:
             log(
                 WARN,
                 "[Node] POST /%s: missing header `Content-Type`",
-                PATH_PULL_TASK_INS,
+                PATH_CREATE_NODE,
             )
             return
         if res.headers["content-type"] != "application/protobuf":
             log(
                 WARN,
                 "[Node] POST /%s: header `Content-Type` has wrong value",
-                PATH_PULL_TASK_INS,
+                PATH_CREATE_NODE,
             )
             return
 
         # Deserialize ProtoBuf from bytes
         create_node_response_proto = CreateNodeResponse()
         create_node_response_proto.ParseFromString(res.content)
 
@@ -273,22 +273,22 @@
         # Check status code and headers
         if res.status_code != 200:
             return
         if "content-type" not in res.headers:
             log(
                 WARN,
                 "[Node] POST /%s: missing header `Content-Type`",
-                PATH_PULL_TASK_INS,
+                PATH_DELETE_NODE,
             )
             return
         if res.headers["content-type"] != "application/protobuf":
             log(
                 WARN,
                 "[Node] POST /%s: header `Content-Type` has wrong value",
-                PATH_PULL_TASK_INS,
+                PATH_DELETE_NODE,
             )
 
         # Cleanup
         node = None
 
     def receive() -> Optional[Message]:
         """Receive next task from server."""
```

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/client/typing.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/address.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/constant.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/context.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/date.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/dp.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/grpc.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/logger.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/message.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/message.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/parameter.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/recordset.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,68 +12,107 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """RecordSet."""
 
 
 from dataclasses import dataclass
-from typing import Callable, Dict, Optional, Type, TypeVar
+from typing import Dict, Optional, cast
 
 from .configsrecord import ConfigsRecord
 from .metricsrecord import MetricsRecord
 from .parametersrecord import ParametersRecord
 from .typeddict import TypedDict
 
-T = TypeVar("T")
 
+class RecordSetData:
+    """Inner data container for the RecordSet class."""
 
-@dataclass
-class RecordSet:
-    """RecordSet stores groups of parameters, metrics and configs."""
-
-    _parameters_records: TypedDict[str, ParametersRecord]
-    _metrics_records: TypedDict[str, MetricsRecord]
-    _configs_records: TypedDict[str, ConfigsRecord]
+    parameters_records: TypedDict[str, ParametersRecord]
+    metrics_records: TypedDict[str, MetricsRecord]
+    configs_records: TypedDict[str, ConfigsRecord]
 
     def __init__(
         self,
         parameters_records: Optional[Dict[str, ParametersRecord]] = None,
         metrics_records: Optional[Dict[str, MetricsRecord]] = None,
         configs_records: Optional[Dict[str, ConfigsRecord]] = None,
     ) -> None:
-        def _get_check_fn(__t: Type[T]) -> Callable[[T], None]:
-            def _check_fn(__v: T) -> None:
-                if not isinstance(__v, __t):
-                    raise TypeError(f"Expected `{__t}`, but `{type(__v)}` was passed.")
-
-            return _check_fn
-
-        self._parameters_records = TypedDict[str, ParametersRecord](
-            _get_check_fn(str), _get_check_fn(ParametersRecord)
+        self.parameters_records = TypedDict[str, ParametersRecord](
+            self._check_fn_str, self._check_fn_params
         )
-        self._metrics_records = TypedDict[str, MetricsRecord](
-            _get_check_fn(str), _get_check_fn(MetricsRecord)
+        self.metrics_records = TypedDict[str, MetricsRecord](
+            self._check_fn_str, self._check_fn_metrics
         )
-        self._configs_records = TypedDict[str, ConfigsRecord](
-            _get_check_fn(str), _get_check_fn(ConfigsRecord)
+        self.configs_records = TypedDict[str, ConfigsRecord](
+            self._check_fn_str, self._check_fn_configs
         )
         if parameters_records is not None:
-            self._parameters_records.update(parameters_records)
+            self.parameters_records.update(parameters_records)
         if metrics_records is not None:
-            self._metrics_records.update(metrics_records)
+            self.metrics_records.update(metrics_records)
         if configs_records is not None:
-            self._configs_records.update(configs_records)
+            self.configs_records.update(configs_records)
+
+    def _check_fn_str(self, key: str) -> None:
+        if not isinstance(key, str):
+            raise TypeError(
+                f"Expected `{str.__name__}`, but "
+                f"received `{type(key).__name__}` for the key."
+            )
+
+    def _check_fn_params(self, record: ParametersRecord) -> None:
+        if not isinstance(record, ParametersRecord):
+            raise TypeError(
+                f"Expected `{ParametersRecord.__name__}`, but "
+                f"received `{type(record).__name__}` for the value."
+            )
+
+    def _check_fn_metrics(self, record: MetricsRecord) -> None:
+        if not isinstance(record, MetricsRecord):
+            raise TypeError(
+                f"Expected `{MetricsRecord.__name__}`, but "
+                f"received `{type(record).__name__}` for the value."
+            )
+
+    def _check_fn_configs(self, record: ConfigsRecord) -> None:
+        if not isinstance(record, ConfigsRecord):
+            raise TypeError(
+                f"Expected `{ConfigsRecord.__name__}`, but "
+                f"received `{type(record).__name__}` for the value."
+            )
+
+
+@dataclass
+class RecordSet:
+    """RecordSet stores groups of parameters, metrics and configs."""
+
+    def __init__(
+        self,
+        parameters_records: Optional[Dict[str, ParametersRecord]] = None,
+        metrics_records: Optional[Dict[str, MetricsRecord]] = None,
+        configs_records: Optional[Dict[str, ConfigsRecord]] = None,
+    ) -> None:
+        data = RecordSetData(
+            parameters_records=parameters_records,
+            metrics_records=metrics_records,
+            configs_records=configs_records,
+        )
+        setattr(self, "_data", data)  # noqa
 
     @property
     def parameters_records(self) -> TypedDict[str, ParametersRecord]:
         """Dictionary holding ParametersRecord instances."""
-        return self._parameters_records
+        data = cast(RecordSetData, getattr(self, "_data"))  # noqa
+        return data.parameters_records
 
     @property
     def metrics_records(self) -> TypedDict[str, MetricsRecord]:
         """Dictionary holding MetricsRecord instances."""
-        return self._metrics_records
+        data = cast(RecordSetData, getattr(self, "_data"))  # noqa
+        return data.metrics_records
 
     @property
     def configs_records(self) -> TypedDict[str, ConfigsRecord]:
         """Dictionary holding ConfigsRecord instances."""
-        return self._configs_records
+        data = cast(RecordSetData, getattr(self, "_data"))  # noqa
+        return data.configs_records
```

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/recordset_compat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/retry_invoker.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/serde.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/typing.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/common/version.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/app.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/compat/app.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/app_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/criterion.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/driver/grpc_driver.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/grpc_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/history.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/run_serverapp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/server.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/server_app.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/server_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/server_config.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def CreateRun(
         self, request: CreateRunRequest, context: grpc.ServicerContext
     ) -> CreateRunResponse:
         """Create run ID."""
         log(INFO, "DriverServicer.CreateRun")
         state: State = self.state_factory.state()
-        run_id = state.create_run()
+        run_id = state.create_run("None/None", "None")
         return CreateRunResponse(run_id=run_id)
 
     def PushTaskIns(
         self, request: PushTaskInsRequest, context: grpc.ServicerContext
     ) -> PushTaskInsResponse:
         """Push a set of TaskIns."""
         log(DEBUG, "DriverServicer.PushTaskIns")
```

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 
 class InMemoryState(State):
     """In-memory State implementation."""
 
     def __init__(self) -> None:
         # Map node_id to (online_until, ping_interval)
         self.node_ids: Dict[int, Tuple[float, float]] = {}
-        self.run_ids: Set[int] = set()
+        # Map run_id to (fab_id, fab_version)
+        self.run_ids: Dict[int, Tuple[str, str]] = {}
         self.task_ins_store: Dict[UUID, TaskIns] = {}
         self.task_res_store: Dict[UUID, TaskRes] = {}
         self.lock = threading.Lock()
 
     def store_task_ins(self, task_ins: TaskIns) -> Optional[UUID]:
         """Store one TaskIns."""
         # Validate task
@@ -234,26 +235,34 @@
             current_time = time.time()
             return {
                 node_id
                 for node_id, (online_until, _) in self.node_ids.items()
                 if online_until > current_time
             }
 
-    def create_run(self) -> int:
-        """Create one run."""
+    def create_run(self, fab_id: str, fab_version: str) -> int:
+        """Create a new run for the specified `fab_id` and `fab_version`."""
         # Sample a random int64 as run_id
         with self.lock:
             run_id: int = int.from_bytes(os.urandom(8), "little", signed=True)
 
             if run_id not in self.run_ids:
-                self.run_ids.add(run_id)
+                self.run_ids[run_id] = (fab_id, fab_version)
                 return run_id
         log(ERROR, "Unexpected run creation failure.")
         return 0
 
+    def get_run(self, run_id: int) -> Tuple[int, str, str]:
+        """Retrieve information about the run with the specified `run_id`."""
+        with self.lock:
+            if run_id not in self.run_ids:
+                log(ERROR, "`run_id` is invalid")
+                return 0, "", ""
+            return run_id, *self.run_ids[run_id]
+
     def acknowledge_ping(self, node_id: int, ping_interval: float) -> bool:
         """Acknowledge a ping received from a node, serving as a heartbeat."""
         with self.lock:
             if node_id in self.node_ids:
                 self.node_ids[node_id] = (time.time() + ping_interval, ping_interval)
                 return True
         return False
```

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,17 @@
 
 SQL_CREATE_INDEX_ONLINE_UNTIL = """
 CREATE INDEX IF NOT EXISTS idx_online_until ON node (online_until);
 """
 
 SQL_CREATE_TABLE_RUN = """
 CREATE TABLE IF NOT EXISTS run(
-    run_id INTEGER UNIQUE
+    run_id          INTEGER UNIQUE,
+    fab_id          TEXT,
+    fab_version     TEXT
 );
 """
 
 SQL_CREATE_TABLE_TASK_INS = """
 CREATE TABLE IF NOT EXISTS task_ins(
     task_id                 TEXT UNIQUE,
     group_id                TEXT,
@@ -554,29 +556,39 @@
 
         # Get nodes
         query = "SELECT node_id FROM node WHERE online_until > ?;"
         rows = self.query(query, (time.time(),))
         result: Set[int] = {row["node_id"] for row in rows}
         return result
 
-    def create_run(self) -> int:
-        """Create one run and store it in state."""
+    def create_run(self, fab_id: str, fab_version: str) -> int:
+        """Create a new run for the specified `fab_id` and `fab_version`."""
         # Sample a random int64 as run_id
         run_id: int = int.from_bytes(os.urandom(8), "little", signed=True)
 
         # Check conflicts
         query = "SELECT COUNT(*) FROM run WHERE run_id = ?;"
         # If run_id does not exist
         if self.query(query, (run_id,))[0]["COUNT(*)"] == 0:
-            query = "INSERT INTO run VALUES(:run_id);"
-            self.query(query, {"run_id": run_id})
+            query = "INSERT INTO run (run_id, fab_id, fab_version) VALUES (?, ?, ?);"
+            self.query(query, (run_id, fab_id, fab_version))
             return run_id
         log(ERROR, "Unexpected run creation failure.")
         return 0
 
+    def get_run(self, run_id: int) -> Tuple[int, str, str]:
+        """Retrieve information about the run with the specified `run_id`."""
+        query = "SELECT * FROM run WHERE run_id = ?;"
+        try:
+            row = self.query(query, (run_id,))[0]
+            return run_id, row["fab_id"], row["fab_version"]
+        except sqlite3.IntegrityError:
+            log(ERROR, "`run_id` does not exist.")
+            return 0, "", ""
+
     def acknowledge_ping(self, node_id: int, ping_interval: float) -> bool:
         """Acknowledge a ping received from a node, serving as a heartbeat."""
         # Update `online_until` and `ping_interval` for the given `node_id`
         query = "UPDATE node SET online_until = ?, ping_interval = ? WHERE node_id = ?;"
         try:
             self.query(query, (time.time() + ping_interval, ping_interval, node_id))
             return True
```

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/state.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Abstract base class State."""
 
 
 import abc
-from typing import List, Optional, Set
+from typing import List, Optional, Set, Tuple
 from uuid import UUID
 
 from flwr.proto.task_pb2 import TaskIns, TaskRes  # pylint: disable=E0611
 
 
 class State(abc.ABC):
     """Abstract State."""
@@ -146,16 +146,34 @@
         Constraints
         -----------
         If the provided `run_id` does not exist or has no matching nodes,
         an empty `Set` MUST be returned.
         """
 
     @abc.abstractmethod
-    def create_run(self) -> int:
-        """Create one run."""
+    def create_run(self, fab_id: str, fab_version: str) -> int:
+        """Create a new run for the specified `fab_id` and `fab_version`."""
+
+    @abc.abstractmethod
+    def get_run(self, run_id: int) -> Tuple[int, str, str]:
+        """Retrieve information about the run with the specified `run_id`.
+
+        Parameters
+        ----------
+        run_id : int
+            The identifier of the run.
+
+        Returns
+        -------
+        Tuple[int, str, str]
+            A tuple containing three elements:
+            - `run_id`: The identifier of the run, same as the specified `run_id`.
+            - `fab_id`: The identifier of the FAB used in the specified run.
+            - `fab_version`: The version of the FAB used in the specified run.
+        """
 
     @abc.abstractmethod
     def acknowledge_ping(self, node_id: int, ping_interval: float) -> bool:
         """Acknowledge a ping received from a node, serving as a heartbeat.
 
         Parameters
         ----------
```

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/superlink/state/utils.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/typing.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/default_workflows.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/app.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/run_simulation.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240417/PKG-INFO` & `flwr_nightly-1.9.0.dev20240418/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.9.0.dev20240417
+Version: 1.9.0.dev20240418
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
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240417 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240418 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

