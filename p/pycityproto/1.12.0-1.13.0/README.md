# Comparing `tmp/pycityproto-1.12.0.tar.gz` & `tmp/pycityproto-1.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycityproto-1.12.0.tar", last modified: Tue Mar 26 07:17:01 2024, max compression
+gzip compressed data, was "pycityproto-1.13.0.tar", last modified: Sat Apr 20 04:11:02 2024, max compression
```

## Comparing `pycityproto-1.12.0.tar` & `pycityproto-1.13.0.tar`

### file list

```diff
@@ -1,375 +1,375 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.101506 pycityproto-1.12.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-26 07:16:55.000000 pycityproto-1.12.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-03-26 07:17:01.101506 pycityproto-1.12.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-03-26 07:16:55.000000 pycityproto-1.12.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.045506 pycityproto-1.12.0/pycityproto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.045506 pycityproto-1.12.0/pycityproto/city/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.045506 pycityproto-1.12.0/pycityproto/city/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/agent/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.049506 pycityproto-1.12.0/pycityproto/city/agent/v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/agent/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/agent/v2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/agent/v2/agent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/agent/v2/agent_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/agent/v2/agent_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/agent/v2/agent_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/agent/v2/agent_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/agent/v2/agent_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/agent/v2/motion_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/agent/v2/motion_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/agent/v2/motion_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.049506 pycityproto-1.12.0/pycityproto/city/clock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/clock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/clock/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.049506 pycityproto-1.12.0/pycityproto/city/clock/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/clock/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/clock/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/clock/v1/clock_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/clock/v1/clock_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/clock/v1/clock_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.049506 pycityproto-1.12.0/pycityproto/city/cognition/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.049506 pycityproto-1.12.0/pycityproto/city/cognition/input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/input/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.053506 pycityproto-1.12.0/pycityproto/city/cognition/input/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/input/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/input/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/input/v1/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/input/v1/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/input/v1/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/input/v1/input_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/input/v1/input_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/input/v1/input_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/input/v1/input_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/input/v1/input_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/input/v1/input_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.053506 pycityproto-1.12.0/pycityproto/city/cognition/output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/output/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.053506 pycityproto-1.12.0/pycityproto/city/cognition/output/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/output/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/output/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/output/v1/output_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/output/v1/output_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/output/v1/output_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/output/v1/output_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/output/v1/output_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/cognition/output/v1/output_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.053506 pycityproto-1.12.0/pycityproto/city/comm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.053506 pycityproto-1.12.0/pycityproto/city/comm/input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/input/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.057506 pycityproto-1.12.0/pycityproto/city/comm/input/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/input/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/input/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/input/v1/comm_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/input/v1/comm_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/input/v1/comm_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.057506 pycityproto-1.12.0/pycityproto/city/comm/interaction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.057506 pycityproto-1.12.0/pycityproto/city/comm/interaction/aoi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/aoi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/aoi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.057506 pycityproto-1.12.0/pycityproto/city/comm/interaction/aoi/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/aoi/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/aoi/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/aoi/v1/aoi_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/aoi/v1/aoi_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/aoi/v1/aoi_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.057506 pycityproto-1.12.0/pycityproto/city/comm/interaction/demand/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/demand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/demand/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.057506 pycityproto-1.12.0/pycityproto/city/comm/interaction/demand/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/demand/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/demand/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/demand/v1/demand_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/demand/v1/demand_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/demand/v1/demand_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.057506 pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.061506 pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/gateway_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/gateway_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/gateway_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/gateway_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/gateway_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/gateway_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.061506 pycityproto-1.12.0/pycityproto/city/comm/output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/output/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.061506 pycityproto-1.12.0/pycityproto/city/comm/output/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/output/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/output/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/output/v1/output_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/output/v1/output_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/output/v1/output_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/output/v1/output_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/output/v1/output_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/comm/output/v1/output_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.061506 pycityproto-1.12.0/pycityproto/city/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/config/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.065506 pycityproto-1.12.0/pycityproto/city/config/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/config/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/config/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/config/v1/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/config/v1/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/config/v1/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.065506 pycityproto-1.12.0/pycityproto/city/economy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/economy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/economy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.065506 pycityproto-1.12.0/pycityproto/city/economy/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/economy/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/economy/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/economy/v1/economy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/economy/v1/economy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/economy/v1/economy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/economy/v1/org_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/economy/v1/org_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/economy/v1/org_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/economy/v1/person_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/economy/v1/person_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/economy/v1/person_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.065506 pycityproto-1.12.0/pycityproto/city/elec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.065506 pycityproto-1.12.0/pycityproto/city/elec/input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/input/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.069506 pycityproto-1.12.0/pycityproto/city/elec/input/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/input/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/input/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/input/v1/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/input/v1/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/input/v1/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/input/v1/input_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/input/v1/input_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/input/v1/input_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/input/v1/input_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/input/v1/input_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/input/v1/input_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.069506 pycityproto-1.12.0/pycityproto/city/elec/interaction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/interaction/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.069506 pycityproto-1.12.0/pycityproto/city/elec/interaction/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/interaction/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/interaction/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/interaction/v1/elec_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/interaction/v1/elec_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/interaction/v1/elec_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.069506 pycityproto-1.12.0/pycityproto/city/elec/output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/output/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.073506 pycityproto-1.12.0/pycityproto/city/elec/output/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/output/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/output/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/output/v1/output_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/output/v1/output_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/output/v1/output_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/output/v1/output_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/output/v1/output_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/elec/output/v1/output_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.073506 pycityproto-1.12.0/pycityproto/city/event/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.073506 pycityproto-1.12.0/pycityproto/city/event/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v1/event_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v1/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v1/event_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v1/event_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v1/event_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v1/event_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.073506 pycityproto-1.12.0/pycityproto/city/event/v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v2/event_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v2/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v2/event_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v2/event_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v2/event_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/event/v2/event_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.073506 pycityproto-1.12.0/pycityproto/city/geo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/geo/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.077506 pycityproto-1.12.0/pycityproto/city/geo/v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/geo/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/geo/v2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/geo/v2/geo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/geo/v2/geo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/geo/v2/geo_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.077506 pycityproto-1.12.0/pycityproto/city/map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.081506 pycityproto-1.12.0/pycityproto/city/map/v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/aoi_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/aoi_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/aoi_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/lane_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/lane_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/lane_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/light_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/light_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/light_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/map_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14037 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/map_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/road_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/road_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/road_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/traffic_light_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/traffic_light_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/map/v2/traffic_light_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.081506 pycityproto-1.12.0/pycityproto/city/person/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/person/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/person/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.081506 pycityproto-1.12.0/pycityproto/city/person/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/person/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/person/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/person/v1/motion_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/person/v1/motion_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/person/v1/motion_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/person/v1/person_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/person/v1/person_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/person/v1/person_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/person/v1/person_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/person/v1/person_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/person/v1/person_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.081506 pycityproto-1.12.0/pycityproto/city/ping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/ping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/ping/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.085506 pycityproto-1.12.0/pycityproto/city/ping/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/ping/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/ping/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/ping/v1/ping_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/ping/v1/ping_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/ping/v1/ping_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.085506 pycityproto-1.12.0/pycityproto/city/routing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/routing/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.085506 pycityproto-1.12.0/pycityproto/city/routing/v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/routing/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/routing/v2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/routing/v2/cost_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/routing/v2/cost_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/routing/v2/cost_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/routing/v2/routing_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/routing/v2/routing_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/routing/v2/routing_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/routing/v2/routing_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/routing/v2/routing_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/routing/v2/routing_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.085506 pycityproto-1.12.0/pycityproto/city/social/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/social/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/social/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.089506 pycityproto-1.12.0/pycityproto/city/social/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/social/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/social/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/social/v1/message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/social/v1/message_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/social/v1/message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/social/v1/social_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/social/v1/social_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/social/v1/social_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.089506 pycityproto-1.12.0/pycityproto/city/streetview/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/streetview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/streetview/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.089506 pycityproto-1.12.0/pycityproto/city/streetview/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/streetview/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/streetview/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/streetview/v1/streetview_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/streetview/v1/streetview_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/streetview/v1/streetview_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.089506 pycityproto-1.12.0/pycityproto/city/sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/sync/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.089506 pycityproto-1.12.0/pycityproto/city/sync/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/sync/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/sync/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/sync/v1/sync_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/sync/v1/sync_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/sync/v1/sync_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.089506 pycityproto-1.12.0/pycityproto/city/trip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/trip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/trip/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.093506 pycityproto-1.12.0/pycityproto/city/trip/v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/trip/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/trip/v2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/trip/v2/trip_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/trip/v2/trip_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/trip/v2/trip_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.093506 pycityproto-1.12.0/pycityproto/city/wargame/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/wargame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/wargame/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.093506 pycityproto-1.12.0/pycityproto/city/wargame/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/wargame/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/wargame/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/wargame/v1/wargame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/wargame/v1/wargame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/wargame/v1/wargame_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/wargame/v1/wargame_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/wargame/v1/wargame_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/wargame/v1/wargame_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.093506 pycityproto-1.12.0/pycityproto/city/water/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.093506 pycityproto-1.12.0/pycityproto/city/water/input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/input/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.097506 pycityproto-1.12.0/pycityproto/city/water/input/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/input/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/input/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/input/v1/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/input/v1/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/input/v1/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/input/v1/input_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/input/v1/input_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/input/v1/input_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/input/v1/water_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/input/v1/water_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/input/v1/water_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.097506 pycityproto-1.12.0/pycityproto/city/water/interaction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/interaction/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.097506 pycityproto-1.12.0/pycityproto/city/water/interaction/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/interaction/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/interaction/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/interaction/v1/water_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/interaction/v1/water_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/interaction/v1/water_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.097506 pycityproto-1.12.0/pycityproto/city/water/output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/output/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.097506 pycityproto-1.12.0/pycityproto/city/water/output/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/output/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/output/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/output/v1/output_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/output/v1/output_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/output/v1/output_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/output/v1/output_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/output/v1/output_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pycityproto/city/water/output/v1/output_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 07:17:01.101506 pycityproto-1.12.0/pycityproto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-03-26 07:17:01.000000 pycityproto-1.12.0/pycityproto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13937 2024-03-26 07:17:01.000000 pycityproto-1.12.0/pycityproto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 07:17:01.000000 pycityproto-1.12.0/pycityproto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-26 07:17:01.000000 pycityproto-1.12.0/pycityproto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-26 07:17:01.000000 pycityproto-1.12.0/pycityproto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-26 07:16:55.000000 pycityproto-1.12.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 07:17:01.101506 pycityproto-1.12.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.893347 pycityproto-1.13.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-20 04:10:54.000000 pycityproto-1.13.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-20 04:11:02.893347 pycityproto-1.13.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-20 04:10:54.000000 pycityproto-1.13.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.845347 pycityproto-1.13.0/pycityproto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.849347 pycityproto-1.13.0/pycityproto/city/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.849347 pycityproto-1.13.0/pycityproto/city/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/agent/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.849347 pycityproto-1.13.0/pycityproto/city/agent/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/agent/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/agent/v2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/agent/v2/agent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/agent/v2/agent_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/agent/v2/agent_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/agent/v2/agent_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/agent/v2/agent_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/agent/v2/agent_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/agent/v2/motion_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/agent/v2/motion_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/agent/v2/motion_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.849347 pycityproto-1.13.0/pycityproto/city/clock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/clock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/clock/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.853347 pycityproto-1.13.0/pycityproto/city/clock/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/clock/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/clock/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/clock/v1/clock_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/clock/v1/clock_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/clock/v1/clock_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.853347 pycityproto-1.13.0/pycityproto/city/cognition/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.853347 pycityproto-1.13.0/pycityproto/city/cognition/input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/input/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.853347 pycityproto-1.13.0/pycityproto/city/cognition/input/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/input/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/input/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/input/v1/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/input/v1/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/input/v1/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/input/v1/input_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/input/v1/input_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/input/v1/input_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/input/v1/input_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/input/v1/input_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/input/v1/input_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.853347 pycityproto-1.13.0/pycityproto/city/cognition/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/output/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.857347 pycityproto-1.13.0/pycityproto/city/cognition/output/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/output/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/output/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/output/v1/output_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/output/v1/output_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/output/v1/output_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/output/v1/output_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/output/v1/output_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/cognition/output/v1/output_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.857347 pycityproto-1.13.0/pycityproto/city/comm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.857347 pycityproto-1.13.0/pycityproto/city/comm/input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/input/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.857347 pycityproto-1.13.0/pycityproto/city/comm/input/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/input/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/input/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/input/v1/comm_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/input/v1/comm_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/input/v1/comm_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.857347 pycityproto-1.13.0/pycityproto/city/comm/interaction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.857347 pycityproto-1.13.0/pycityproto/city/comm/interaction/aoi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/aoi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/aoi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.857347 pycityproto-1.13.0/pycityproto/city/comm/interaction/aoi/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/aoi/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/aoi/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/aoi/v1/aoi_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/aoi/v1/aoi_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/aoi/v1/aoi_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.857347 pycityproto-1.13.0/pycityproto/city/comm/interaction/demand/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/demand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/demand/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.861347 pycityproto-1.13.0/pycityproto/city/comm/interaction/demand/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/demand/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/demand/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/demand/v1/demand_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/demand/v1/demand_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/demand/v1/demand_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.861347 pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.861347 pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/gateway_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/gateway_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/gateway_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/gateway_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/gateway_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/gateway_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.861347 pycityproto-1.13.0/pycityproto/city/comm/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/output/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.861347 pycityproto-1.13.0/pycityproto/city/comm/output/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/output/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/output/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/output/v1/output_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/output/v1/output_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/output/v1/output_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/output/v1/output_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/output/v1/output_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/comm/output/v1/output_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.865347 pycityproto-1.13.0/pycityproto/city/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/config/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.865347 pycityproto-1.13.0/pycityproto/city/config/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/config/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/config/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/config/v1/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/config/v1/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/config/v1/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.865347 pycityproto-1.13.0/pycityproto/city/economy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/economy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/economy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.865347 pycityproto-1.13.0/pycityproto/city/economy/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/economy/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/economy/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/economy/v1/economy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/economy/v1/economy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/economy/v1/economy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/economy/v1/org_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/economy/v1/org_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/economy/v1/org_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/economy/v1/person_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/economy/v1/person_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/economy/v1/person_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.865347 pycityproto-1.13.0/pycityproto/city/elec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.865347 pycityproto-1.13.0/pycityproto/city/elec/input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/input/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.869347 pycityproto-1.13.0/pycityproto/city/elec/input/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/input/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/input/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/input/v1/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/input/v1/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/input/v1/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/input/v1/input_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/input/v1/input_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/input/v1/input_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/input/v1/input_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/input/v1/input_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/input/v1/input_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.869347 pycityproto-1.13.0/pycityproto/city/elec/interaction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/interaction/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.869347 pycityproto-1.13.0/pycityproto/city/elec/interaction/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/interaction/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/interaction/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/interaction/v1/elec_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/interaction/v1/elec_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/interaction/v1/elec_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.869347 pycityproto-1.13.0/pycityproto/city/elec/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/output/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.869347 pycityproto-1.13.0/pycityproto/city/elec/output/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/output/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/output/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/output/v1/output_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/output/v1/output_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/output/v1/output_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/output/v1/output_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/output/v1/output_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/elec/output/v1/output_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.873347 pycityproto-1.13.0/pycityproto/city/event/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.873347 pycityproto-1.13.0/pycityproto/city/event/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v1/event_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v1/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v1/event_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v1/event_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v1/event_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v1/event_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.873347 pycityproto-1.13.0/pycityproto/city/event/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v2/event_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v2/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v2/event_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v2/event_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v2/event_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/event/v2/event_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.873347 pycityproto-1.13.0/pycityproto/city/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/geo/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.873347 pycityproto-1.13.0/pycityproto/city/geo/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/geo/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/geo/v2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/geo/v2/geo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/geo/v2/geo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/geo/v2/geo_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.873347 pycityproto-1.13.0/pycityproto/city/map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.877347 pycityproto-1.13.0/pycityproto/city/map/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/aoi_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/aoi_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/aoi_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/lane_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/lane_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/lane_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/light_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/light_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/light_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/map_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14037 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/map_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/road_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/road_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/road_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/traffic_light_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/traffic_light_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/map/v2/traffic_light_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.877347 pycityproto-1.13.0/pycityproto/city/person/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/person/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/person/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.881347 pycityproto-1.13.0/pycityproto/city/person/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/person/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/person/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/person/v1/motion_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/person/v1/motion_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/person/v1/motion_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/person/v1/person_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/person/v1/person_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/person/v1/person_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/person/v1/person_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/person/v1/person_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/person/v1/person_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.881347 pycityproto-1.13.0/pycityproto/city/ping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/ping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/ping/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.881347 pycityproto-1.13.0/pycityproto/city/ping/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/ping/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/ping/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/ping/v1/ping_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/ping/v1/ping_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/ping/v1/ping_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.881347 pycityproto-1.13.0/pycityproto/city/routing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/routing/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.881347 pycityproto-1.13.0/pycityproto/city/routing/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/routing/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/routing/v2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/routing/v2/cost_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/routing/v2/cost_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/routing/v2/cost_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/routing/v2/routing_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/routing/v2/routing_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/routing/v2/routing_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/routing/v2/routing_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/routing/v2/routing_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/routing/v2/routing_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.885347 pycityproto-1.13.0/pycityproto/city/social/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/social/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/social/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.885347 pycityproto-1.13.0/pycityproto/city/social/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/social/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/social/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/social/v1/message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/social/v1/message_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/social/v1/message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/social/v1/social_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/social/v1/social_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/social/v1/social_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.885347 pycityproto-1.13.0/pycityproto/city/streetview/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/streetview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/streetview/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.885347 pycityproto-1.13.0/pycityproto/city/streetview/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/streetview/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/streetview/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/streetview/v1/streetview_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/streetview/v1/streetview_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/streetview/v1/streetview_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.885347 pycityproto-1.13.0/pycityproto/city/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/sync/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.885347 pycityproto-1.13.0/pycityproto/city/sync/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/sync/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/sync/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/sync/v1/sync_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/sync/v1/sync_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/sync/v1/sync_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.885347 pycityproto-1.13.0/pycityproto/city/trip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/trip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/trip/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.889347 pycityproto-1.13.0/pycityproto/city/trip/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/trip/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/trip/v2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/trip/v2/trip_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/trip/v2/trip_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/trip/v2/trip_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.889347 pycityproto-1.13.0/pycityproto/city/wargame/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/wargame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/wargame/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.889347 pycityproto-1.13.0/pycityproto/city/wargame/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/wargame/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/wargame/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/wargame/v1/wargame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/wargame/v1/wargame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/wargame/v1/wargame_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/wargame/v1/wargame_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/wargame/v1/wargame_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/wargame/v1/wargame_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.889347 pycityproto-1.13.0/pycityproto/city/water/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.889347 pycityproto-1.13.0/pycityproto/city/water/input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/input/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.893347 pycityproto-1.13.0/pycityproto/city/water/input/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/input/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/input/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/input/v1/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/input/v1/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/input/v1/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/input/v1/input_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/input/v1/input_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/input/v1/input_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/input/v1/water_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/input/v1/water_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/input/v1/water_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.893347 pycityproto-1.13.0/pycityproto/city/water/interaction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/interaction/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.893347 pycityproto-1.13.0/pycityproto/city/water/interaction/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/interaction/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/interaction/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/interaction/v1/water_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/interaction/v1/water_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/interaction/v1/water_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.893347 pycityproto-1.13.0/pycityproto/city/water/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/output/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.893347 pycityproto-1.13.0/pycityproto/city/water/output/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/output/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/output/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/output/v1/output_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/output/v1/output_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/output/v1/output_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/output/v1/output_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/output/v1/output_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pycityproto/city/water/output/v1/output_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:11:02.893347 pycityproto-1.13.0/pycityproto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-20 04:11:02.000000 pycityproto-1.13.0/pycityproto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13937 2024-04-20 04:11:02.000000 pycityproto-1.13.0/pycityproto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 04:11:02.000000 pycityproto-1.13.0/pycityproto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 04:11:02.000000 pycityproto-1.13.0/pycityproto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 04:11:02.000000 pycityproto-1.13.0/pycityproto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-20 04:10:54.000000 pycityproto-1.13.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 04:11:02.893347 pycityproto-1.13.0/setup.cfg
```

### Comparing `pycityproto-1.12.0/LICENSE` & `pycityproto-1.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/PKG-INFO` & `pycityproto-1.13.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityproto
-Version: 1.12.0
+Version: 1.13.0
 Summary: City Proto Generated Python SDK
 Author-email: Jun Zhang <zhangjun990222@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycityproto-1.12.0/README.md` & `pycityproto-1.13.0/README.md`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/agent/v2/agent_pb2.py` & `pycityproto-1.13.0/pycityproto/city/agent/v2/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/agent/v2/agent_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/agent/v2/agent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/agent/v2/agent_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/agent/v2/agent_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/agent/v2/agent_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/agent/v2/agent_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/agent/v2/agent_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/agent/v2/agent_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/agent/v2/motion_pb2.py` & `pycityproto-1.13.0/pycityproto/city/agent/v2/motion_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/agent/v2/motion_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/agent/v2/motion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/clock/v1/clock_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/clock/v1/clock_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/clock/v1/clock_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/clock/v1/clock_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/cognition/input/v1/config_pb2.py` & `pycityproto-1.13.0/pycityproto/city/cognition/input/v1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/cognition/input/v1/config_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/cognition/input/v1/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/cognition/input/v1/input_pb2.py` & `pycityproto-1.13.0/pycityproto/city/cognition/input/v1/input_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/cognition/input/v1/input_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/cognition/input/v1/input_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/cognition/input/v1/input_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/cognition/input/v1/input_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/cognition/input/v1/input_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/cognition/input/v1/input_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/cognition/input/v1/input_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/cognition/input/v1/input_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/cognition/output/v1/output_pb2.py` & `pycityproto-1.13.0/pycityproto/city/cognition/output/v1/output_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/cognition/output/v1/output_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/cognition/output/v1/output_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/cognition/output/v1/output_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/cognition/output/v1/output_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/cognition/output/v1/output_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/cognition/output/v1/output_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/cognition/output/v1/output_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/cognition/output/v1/output_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/input/v1/comm_pb2.py` & `pycityproto-1.13.0/pycityproto/city/comm/input/v1/comm_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/input/v1/comm_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/comm/input/v1/comm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/interaction/aoi/v1/aoi_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/comm/interaction/aoi/v1/aoi_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/interaction/aoi/v1/aoi_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/comm/interaction/aoi/v1/aoi_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/interaction/aoi/v1/aoi_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/comm/interaction/aoi/v1/aoi_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/interaction/demand/v1/demand_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/comm/interaction/demand/v1/demand_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/interaction/demand/v1/demand_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/comm/interaction/demand/v1/demand_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/interaction/demand/v1/demand_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/comm/interaction/demand/v1/demand_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/gateway_pb2.py` & `pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/gateway_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/gateway_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/gateway_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/gateway_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/gateway_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/gateway_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/gateway_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/interaction/gateway/v1/gateway_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/comm/interaction/gateway/v1/gateway_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/output/v1/output_pb2.py` & `pycityproto-1.13.0/pycityproto/city/comm/output/v1/output_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/output/v1/output_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/comm/output/v1/output_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/output/v1/output_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/comm/output/v1/output_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/output/v1/output_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/comm/output/v1/output_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/comm/output/v1/output_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/comm/output/v1/output_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/config/v1/config_pb2.py` & `pycityproto-1.13.0/pycityproto/city/config/v1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/config/v1/config_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/config/v1/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/economy/v1/economy_pb2.py` & `pycityproto-1.13.0/pycityproto/city/economy/v1/economy_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/economy/v1/economy_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/economy/v1/economy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/economy/v1/org_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/economy/v1/org_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/economy/v1/org_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/economy/v1/org_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/economy/v1/org_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/economy/v1/org_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/economy/v1/person_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/economy/v1/person_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/economy/v1/person_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/economy/v1/person_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/economy/v1/person_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/economy/v1/person_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/input/v1/config_pb2.py` & `pycityproto-1.13.0/pycityproto/city/elec/input/v1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/input/v1/config_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/elec/input/v1/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/input/v1/input_pb2.py` & `pycityproto-1.13.0/pycityproto/city/elec/input/v1/input_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/input/v1/input_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/elec/input/v1/input_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/input/v1/input_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/elec/input/v1/input_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/input/v1/input_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/elec/input/v1/input_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/input/v1/input_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/elec/input/v1/input_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/interaction/v1/elec_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/elec/interaction/v1/elec_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/interaction/v1/elec_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/elec/interaction/v1/elec_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/interaction/v1/elec_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/elec/interaction/v1/elec_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/output/v1/output_pb2.py` & `pycityproto-1.13.0/pycityproto/city/elec/output/v1/output_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/output/v1/output_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/elec/output/v1/output_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/output/v1/output_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/elec/output/v1/output_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/output/v1/output_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/elec/output/v1/output_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/elec/output/v1/output_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/elec/output/v1/output_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/event/v1/event_pb2.py` & `pycityproto-1.13.0/pycityproto/city/event/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/event/v1/event_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/event/v1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/event/v1/event_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/event/v1/event_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/event/v1/event_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/event/v1/event_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/event/v1/event_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/event/v1/event_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/event/v2/event_pb2.py` & `pycityproto-1.13.0/pycityproto/city/event/v2/event_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/event/v2/event_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/event/v2/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/event/v2/event_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/event/v2/event_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/event/v2/event_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/event/v2/event_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/event/v2/event_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/event/v2/event_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/geo/v2/geo_pb2.py` & `pycityproto-1.13.0/pycityproto/city/geo/v2/geo_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/geo/v2/geo_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/geo/v2/geo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/aoi_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/map/v2/aoi_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/aoi_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/map/v2/aoi_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/aoi_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/map/v2/aoi_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/lane_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/map/v2/lane_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/lane_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/map/v2/lane_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/lane_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/map/v2/lane_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/light_pb2.py` & `pycityproto-1.13.0/pycityproto/city/map/v2/light_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/light_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/map/v2/light_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/map_pb2.py` & `pycityproto-1.13.0/pycityproto/city/map/v2/map_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/map_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/map/v2/map_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/road_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/map/v2/road_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/road_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/map/v2/road_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/road_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/map/v2/road_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/traffic_light_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/map/v2/traffic_light_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/traffic_light_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/map/v2/traffic_light_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/map/v2/traffic_light_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/map/v2/traffic_light_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/person/v1/motion_pb2.py` & `pycityproto-1.13.0/pycityproto/city/person/v1/motion_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/person/v1/motion_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/person/v1/motion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/person/v1/person_pb2.py` & `pycityproto-1.13.0/pycityproto/city/person/v1/person_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,38 +2,40 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 _sym_db = _symbol_database.Default()
 from ....city.geo.v2 import geo_pb2 as city_dot_geo_dot_v2_dot_geo__pb2
 from ....city.trip.v2 import trip_pb2 as city_dot_trip_dot_v2_dot_trip__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bcity/person/v1/person.proto\x12\x0ecity.person.v1\x1a\x15city/geo/v2/geo.proto\x1a\x17city/trip/v2/trip.proto"\xae\x02\n\x0fPersonAttribute\x12\x16\n\x06length\x18\x02 \x01(\x01R\x06length\x12\x14\n\x05width\x18\x03 \x01(\x01R\x05width\x12\x1b\n\tmax_speed\x18\x04 \x01(\x01R\x08maxSpeed\x12)\n\x10max_acceleration\x18\x05 \x01(\x01R\x0fmaxAcceleration\x128\n\x18max_braking_acceleration\x18\x06 \x01(\x01R\x16maxBrakingAcceleration\x12-\n\x12usual_acceleration\x18\x07 \x01(\x01R\x11usualAcceleration\x12<\n\x1ausual_braking_acceleration\x18\x08 \x01(\x01R\x18usualBrakingAcceleration"Y\n\x10VehicleAttribute\x12,\n\x12lane_change_length\x18\x01 \x01(\x01R\x10laneChangeLength\x12\x17\n\x07min_gap\x18\x02 \x01(\x01R\x06minGap"C\n\x0cBusAttribute\x12\x17\n\x07line_id\x18\x01 \x01(\x05R\x06lineId\x12\x1a\n\x08capacity\x18\x02 \x01(\x05R\x08capacity"\x0f\n\rBikeAttribute"\xc9\x01\n\rPersonProfile\x12\x10\n\x03age\x18\x01 \x01(\x05R\x03age\x127\n\teducation\x18\x02 \x01(\x0e2\x19.city.person.v1.EducationR\teducation\x12.\n\x06gender\x18\x03 \x01(\x0e2\x16.city.person.v1.GenderR\x06gender\x12=\n\x0bconsumption\x18\x04 \x01(\x0e2\x1b.city.person.v1.ConsumptionR\x0bconsumption"\x9b\x05\n\x06Person\x12\x0e\n\x02id\x18\x01 \x01(\x05R\x02id\x12=\n\tattribute\x18\x02 \x01(\x0b2\x1f.city.person.v1.PersonAttributeR\tattribute\x12)\n\x04home\x18\x03 \x01(\x0b2\x15.city.geo.v2.PositionR\x04home\x124\n\tschedules\x18\x04 \x03(\x0b2\x16.city.trip.v2.ScheduleR\tschedules\x12R\n\x11vehicle_attribute\x18\x07 \x01(\x0b2 .city.person.v1.VehicleAttributeH\x00R\x10vehicleAttribute\x88\x01\x01\x12F\n\rbus_attribute\x18\x08 \x01(\x0b2\x1c.city.person.v1.BusAttributeH\x01R\x0cbusAttribute\x88\x01\x01\x12I\n\x0ebike_attribute\x18\t \x01(\x0b2\x1d.city.person.v1.BikeAttributeH\x02R\rbikeAttribute\x88\x01\x01\x12:\n\x06labels\x18\n \x03(\x0b2".city.person.v1.Person.LabelsEntryR\x06labels\x12<\n\x07profile\x18\x0b \x01(\x0b2\x1d.city.person.v1.PersonProfileH\x03R\x07profile\x88\x01\x01\x1a9\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x028\x01B\x14\n\x12_vehicle_attributeB\x10\n\x0e_bus_attributeB\x11\n\x0f_bike_attributeB\n\n\x08_profile";\n\x07Persons\x120\n\x07persons\x18\x01 \x03(\x0b2\x16.city.person.v1.PersonR\x07persons*\xdc\x01\n\tEducation\x12\x19\n\x15EDUCATION_UNSPECIFIED\x10\x00\x12\x14\n\x10EDUCATION_DOCTOR\x10\x01\x12\x14\n\x10EDUCATION_MASTER\x10\x02\x12\x16\n\x12EDUCATION_BACHELOR\x10\x03\x12\x19\n\x15EDUCATION_HIGH_SCHOOL\x10\x04\x12 \n\x1cEDUCATION_JUNIOR_HIGH_SCHOOL\x10\x05\x12\x1c\n\x18EDUCATION_PRIMARY_SCHOOL\x10\x06\x12\x15\n\x11EDUCATION_COLLEGE\x10\x07*D\n\x06Gender\x12\x16\n\x12GENDER_UNSPECIFIED\x10\x00\x12\x0f\n\x0bGENDER_MALE\x10\x01\x12\x11\n\rGENDER_FEMALE\x10\x02*\xae\x01\n\x0bConsumption\x12\x1b\n\x17CONSUMPTION_UNSPECIFIED\x10\x00\x12\x13\n\x0fCONSUMPTION_LOW\x10\x01\x12\x1e\n\x1aCONSUMPTION_RELATIVELY_LOW\x10\x02\x12\x16\n\x12CONSUMPTION_MEDIUM\x10\x03\x12\x1f\n\x1bCONSUMPTION_RELATIVELY_HIGH\x10\x04\x12\x14\n\x10CONSUMPTION_HIGH\x10\x05B\xb1\x01\n\x12com.city.person.v1B\x0bPersonProtoP\x01Z4git.fiblab.net/sim/protos/go/city/person/v1;personv1\xa2\x02\x03CPX\xaa\x02\x0eCity.Person.V1\xca\x02\x0eCity\\Person\\V1\xe2\x02\x1aCity\\Person\\V1\\GPBMetadata\xea\x02\x10City::Person::V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bcity/person/v1/person.proto\x12\x0ecity.person.v1\x1a\x15city/geo/v2/geo.proto\x1a\x17city/trip/v2/trip.proto"\xae\x02\n\x0fPersonAttribute\x12\x16\n\x06length\x18\x02 \x01(\x01R\x06length\x12\x14\n\x05width\x18\x03 \x01(\x01R\x05width\x12\x1b\n\tmax_speed\x18\x04 \x01(\x01R\x08maxSpeed\x12)\n\x10max_acceleration\x18\x05 \x01(\x01R\x0fmaxAcceleration\x128\n\x18max_braking_acceleration\x18\x06 \x01(\x01R\x16maxBrakingAcceleration\x12-\n\x12usual_acceleration\x18\x07 \x01(\x01R\x11usualAcceleration\x12<\n\x1ausual_braking_acceleration\x18\x08 \x01(\x01R\x18usualBrakingAcceleration"~\n\x10VehicleAttribute\x12,\n\x12lane_change_length\x18\x01 \x01(\x01R\x10laneChangeLength\x12\x17\n\x07min_gap\x18\x02 \x01(\x01R\x06minGap\x12\x19\n\x05model\x18\x03 \x01(\tH\x00R\x05model\x88\x01\x01B\x08\n\x06_model"C\n\x0cBusAttribute\x12\x17\n\x07line_id\x18\x01 \x01(\x05R\x06lineId\x12\x1a\n\x08capacity\x18\x02 \x01(\x05R\x08capacity"+\n\x13PedestrianAttribute\x12\x14\n\x05speed\x18\x01 \x01(\x01R\x05speed"%\n\rBikeAttribute\x12\x14\n\x05speed\x18\x01 \x01(\x01R\x05speed"\xc9\x01\n\rPersonProfile\x12\x10\n\x03age\x18\x01 \x01(\x05R\x03age\x127\n\teducation\x18\x02 \x01(\x0e2\x19.city.person.v1.EducationR\teducation\x12.\n\x06gender\x18\x03 \x01(\x0e2\x16.city.person.v1.GenderR\x06gender\x12=\n\x0bconsumption\x18\x04 \x01(\x0e2\x1b.city.person.v1.ConsumptionR\x0bconsumption"\x91\x06\n\x06Person\x12\x0e\n\x02id\x18\x01 \x01(\x05R\x02id\x12=\n\tattribute\x18\x02 \x01(\x0b2\x1f.city.person.v1.PersonAttributeR\tattribute\x12)\n\x04home\x18\x03 \x01(\x0b2\x15.city.geo.v2.PositionR\x04home\x124\n\tschedules\x18\x04 \x03(\x0b2\x16.city.trip.v2.ScheduleR\tschedules\x12R\n\x11vehicle_attribute\x18\x07 \x01(\x0b2 .city.person.v1.VehicleAttributeH\x00R\x10vehicleAttribute\x88\x01\x01\x12F\n\rbus_attribute\x18\x08 \x01(\x0b2\x1c.city.person.v1.BusAttributeH\x01R\x0cbusAttribute\x88\x01\x01\x12[\n\x14pedestrian_attribute\x18\x0c \x01(\x0b2#.city.person.v1.PedestrianAttributeH\x02R\x13pedestrianAttribute\x88\x01\x01\x12I\n\x0ebike_attribute\x18\t \x01(\x0b2\x1d.city.person.v1.BikeAttributeH\x03R\rbikeAttribute\x88\x01\x01\x12:\n\x06labels\x18\n \x03(\x0b2".city.person.v1.Person.LabelsEntryR\x06labels\x12<\n\x07profile\x18\x0b \x01(\x0b2\x1d.city.person.v1.PersonProfileH\x04R\x07profile\x88\x01\x01\x1a9\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x028\x01B\x14\n\x12_vehicle_attributeB\x10\n\x0e_bus_attributeB\x17\n\x15_pedestrian_attributeB\x11\n\x0f_bike_attributeB\n\n\x08_profile";\n\x07Persons\x120\n\x07persons\x18\x01 \x03(\x0b2\x16.city.person.v1.PersonR\x07persons*\xdc\x01\n\tEducation\x12\x19\n\x15EDUCATION_UNSPECIFIED\x10\x00\x12\x14\n\x10EDUCATION_DOCTOR\x10\x01\x12\x14\n\x10EDUCATION_MASTER\x10\x02\x12\x16\n\x12EDUCATION_BACHELOR\x10\x03\x12\x19\n\x15EDUCATION_HIGH_SCHOOL\x10\x04\x12 \n\x1cEDUCATION_JUNIOR_HIGH_SCHOOL\x10\x05\x12\x1c\n\x18EDUCATION_PRIMARY_SCHOOL\x10\x06\x12\x15\n\x11EDUCATION_COLLEGE\x10\x07*D\n\x06Gender\x12\x16\n\x12GENDER_UNSPECIFIED\x10\x00\x12\x0f\n\x0bGENDER_MALE\x10\x01\x12\x11\n\rGENDER_FEMALE\x10\x02*\xae\x01\n\x0bConsumption\x12\x1b\n\x17CONSUMPTION_UNSPECIFIED\x10\x00\x12\x13\n\x0fCONSUMPTION_LOW\x10\x01\x12\x1e\n\x1aCONSUMPTION_RELATIVELY_LOW\x10\x02\x12\x16\n\x12CONSUMPTION_MEDIUM\x10\x03\x12\x1f\n\x1bCONSUMPTION_RELATIVELY_HIGH\x10\x04\x12\x14\n\x10CONSUMPTION_HIGH\x10\x05B\xb1\x01\n\x12com.city.person.v1B\x0bPersonProtoP\x01Z4git.fiblab.net/sim/protos/go/city/person/v1;personv1\xa2\x02\x03CPX\xaa\x02\x0eCity.Person.V1\xca\x02\x0eCity\\Person\\V1\xe2\x02\x1aCity\\Person\\V1\\GPBMetadata\xea\x02\x10City::Person::V1b\x06proto3')
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'city.person.v1.person_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     _globals['DESCRIPTOR']._options = None
     _globals['DESCRIPTOR']._serialized_options = b'\n\x12com.city.person.v1B\x0bPersonProtoP\x01Z4git.fiblab.net/sim/protos/go/city/person/v1;personv1\xa2\x02\x03CPX\xaa\x02\x0eCity.Person.V1\xca\x02\x0eCity\\Person\\V1\xe2\x02\x1aCity\\Person\\V1\\GPBMetadata\xea\x02\x10City::Person::V1'
     _globals['_PERSON_LABELSENTRY']._options = None
     _globals['_PERSON_LABELSENTRY']._serialized_options = b'8\x01'
-    _globals['_EDUCATION']._serialized_start = 1513
-    _globals['_EDUCATION']._serialized_end = 1733
-    _globals['_GENDER']._serialized_start = 1735
-    _globals['_GENDER']._serialized_end = 1803
-    _globals['_CONSUMPTION']._serialized_start = 1806
-    _globals['_CONSUMPTION']._serialized_end = 1980
+    _globals['_EDUCATION']._serialized_start = 1735
+    _globals['_EDUCATION']._serialized_end = 1955
+    _globals['_GENDER']._serialized_start = 1957
+    _globals['_GENDER']._serialized_end = 2025
+    _globals['_CONSUMPTION']._serialized_start = 2028
+    _globals['_CONSUMPTION']._serialized_end = 2202
     _globals['_PERSONATTRIBUTE']._serialized_start = 96
     _globals['_PERSONATTRIBUTE']._serialized_end = 398
     _globals['_VEHICLEATTRIBUTE']._serialized_start = 400
-    _globals['_VEHICLEATTRIBUTE']._serialized_end = 489
-    _globals['_BUSATTRIBUTE']._serialized_start = 491
-    _globals['_BUSATTRIBUTE']._serialized_end = 558
-    _globals['_BIKEATTRIBUTE']._serialized_start = 560
-    _globals['_BIKEATTRIBUTE']._serialized_end = 575
-    _globals['_PERSONPROFILE']._serialized_start = 578
-    _globals['_PERSONPROFILE']._serialized_end = 779
-    _globals['_PERSON']._serialized_start = 782
-    _globals['_PERSON']._serialized_end = 1449
-    _globals['_PERSON_LABELSENTRY']._serialized_start = 1321
-    _globals['_PERSON_LABELSENTRY']._serialized_end = 1378
-    _globals['_PERSONS']._serialized_start = 1451
-    _globals['_PERSONS']._serialized_end = 1510
+    _globals['_VEHICLEATTRIBUTE']._serialized_end = 526
+    _globals['_BUSATTRIBUTE']._serialized_start = 528
+    _globals['_BUSATTRIBUTE']._serialized_end = 595
+    _globals['_PEDESTRIANATTRIBUTE']._serialized_start = 597
+    _globals['_PEDESTRIANATTRIBUTE']._serialized_end = 640
+    _globals['_BIKEATTRIBUTE']._serialized_start = 642
+    _globals['_BIKEATTRIBUTE']._serialized_end = 679
+    _globals['_PERSONPROFILE']._serialized_start = 682
+    _globals['_PERSONPROFILE']._serialized_end = 883
+    _globals['_PERSON']._serialized_start = 886
+    _globals['_PERSON']._serialized_end = 1671
+    _globals['_PERSON_LABELSENTRY']._serialized_start = 1518
+    _globals['_PERSON_LABELSENTRY']._serialized_end = 1575
+    _globals['_PERSONS']._serialized_start = 1673
+    _globals['_PERSONS']._serialized_end = 1732
```

### Comparing `pycityproto-1.12.0/pycityproto/city/person/v1/person_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/person/v1/person_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -67,37 +67,49 @@
     usual_acceleration: float
     usual_braking_acceleration: float
 
     def __init__(self, length: _Optional[float]=..., width: _Optional[float]=..., max_speed: _Optional[float]=..., max_acceleration: _Optional[float]=..., max_braking_acceleration: _Optional[float]=..., usual_acceleration: _Optional[float]=..., usual_braking_acceleration: _Optional[float]=...) -> None:
         ...
 
 class VehicleAttribute(_message.Message):
-    __slots__ = ['lane_change_length', 'min_gap']
+    __slots__ = ['lane_change_length', 'min_gap', 'model']
     LANE_CHANGE_LENGTH_FIELD_NUMBER: _ClassVar[int]
     MIN_GAP_FIELD_NUMBER: _ClassVar[int]
+    MODEL_FIELD_NUMBER: _ClassVar[int]
     lane_change_length: float
     min_gap: float
+    model: str
 
-    def __init__(self, lane_change_length: _Optional[float]=..., min_gap: _Optional[float]=...) -> None:
+    def __init__(self, lane_change_length: _Optional[float]=..., min_gap: _Optional[float]=..., model: _Optional[str]=...) -> None:
         ...
 
 class BusAttribute(_message.Message):
     __slots__ = ['line_id', 'capacity']
     LINE_ID_FIELD_NUMBER: _ClassVar[int]
     CAPACITY_FIELD_NUMBER: _ClassVar[int]
     line_id: int
     capacity: int
 
     def __init__(self, line_id: _Optional[int]=..., capacity: _Optional[int]=...) -> None:
         ...
 
+class PedestrianAttribute(_message.Message):
+    __slots__ = ['speed']
+    SPEED_FIELD_NUMBER: _ClassVar[int]
+    speed: float
+
+    def __init__(self, speed: _Optional[float]=...) -> None:
+        ...
+
 class BikeAttribute(_message.Message):
-    __slots__ = []
+    __slots__ = ['speed']
+    SPEED_FIELD_NUMBER: _ClassVar[int]
+    speed: float
 
-    def __init__(self) -> None:
+    def __init__(self, speed: _Optional[float]=...) -> None:
         ...
 
 class PersonProfile(_message.Message):
     __slots__ = ['age', 'education', 'gender', 'consumption']
     AGE_FIELD_NUMBER: _ClassVar[int]
     EDUCATION_FIELD_NUMBER: _ClassVar[int]
     GENDER_FIELD_NUMBER: _ClassVar[int]
@@ -107,15 +119,15 @@
     gender: Gender
     consumption: Consumption
 
     def __init__(self, age: _Optional[int]=..., education: _Optional[_Union[Education, str]]=..., gender: _Optional[_Union[Gender, str]]=..., consumption: _Optional[_Union[Consumption, str]]=...) -> None:
         ...
 
 class Person(_message.Message):
-    __slots__ = ['id', 'attribute', 'home', 'schedules', 'vehicle_attribute', 'bus_attribute', 'bike_attribute', 'labels', 'profile']
+    __slots__ = ['id', 'attribute', 'home', 'schedules', 'vehicle_attribute', 'bus_attribute', 'pedestrian_attribute', 'bike_attribute', 'labels', 'profile']
 
     class LabelsEntry(_message.Message):
         __slots__ = ['key', 'value']
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
@@ -124,28 +136,30 @@
             ...
     ID_FIELD_NUMBER: _ClassVar[int]
     ATTRIBUTE_FIELD_NUMBER: _ClassVar[int]
     HOME_FIELD_NUMBER: _ClassVar[int]
     SCHEDULES_FIELD_NUMBER: _ClassVar[int]
     VEHICLE_ATTRIBUTE_FIELD_NUMBER: _ClassVar[int]
     BUS_ATTRIBUTE_FIELD_NUMBER: _ClassVar[int]
+    PEDESTRIAN_ATTRIBUTE_FIELD_NUMBER: _ClassVar[int]
     BIKE_ATTRIBUTE_FIELD_NUMBER: _ClassVar[int]
     LABELS_FIELD_NUMBER: _ClassVar[int]
     PROFILE_FIELD_NUMBER: _ClassVar[int]
     id: int
     attribute: PersonAttribute
     home: _geo_pb2.Position
     schedules: _containers.RepeatedCompositeFieldContainer[_trip_pb2.Schedule]
     vehicle_attribute: VehicleAttribute
     bus_attribute: BusAttribute
+    pedestrian_attribute: PedestrianAttribute
     bike_attribute: BikeAttribute
     labels: _containers.ScalarMap[str, str]
     profile: PersonProfile
 
-    def __init__(self, id: _Optional[int]=..., attribute: _Optional[_Union[PersonAttribute, _Mapping]]=..., home: _Optional[_Union[_geo_pb2.Position, _Mapping]]=..., schedules: _Optional[_Iterable[_Union[_trip_pb2.Schedule, _Mapping]]]=..., vehicle_attribute: _Optional[_Union[VehicleAttribute, _Mapping]]=..., bus_attribute: _Optional[_Union[BusAttribute, _Mapping]]=..., bike_attribute: _Optional[_Union[BikeAttribute, _Mapping]]=..., labels: _Optional[_Mapping[str, str]]=..., profile: _Optional[_Union[PersonProfile, _Mapping]]=...) -> None:
+    def __init__(self, id: _Optional[int]=..., attribute: _Optional[_Union[PersonAttribute, _Mapping]]=..., home: _Optional[_Union[_geo_pb2.Position, _Mapping]]=..., schedules: _Optional[_Iterable[_Union[_trip_pb2.Schedule, _Mapping]]]=..., vehicle_attribute: _Optional[_Union[VehicleAttribute, _Mapping]]=..., bus_attribute: _Optional[_Union[BusAttribute, _Mapping]]=..., pedestrian_attribute: _Optional[_Union[PedestrianAttribute, _Mapping]]=..., bike_attribute: _Optional[_Union[BikeAttribute, _Mapping]]=..., labels: _Optional[_Mapping[str, str]]=..., profile: _Optional[_Union[PersonProfile, _Mapping]]=...) -> None:
         ...
 
 class Persons(_message.Message):
     __slots__ = ['persons']
     PERSONS_FIELD_NUMBER: _ClassVar[int]
     persons: _containers.RepeatedCompositeFieldContainer[Person]
```

### Comparing `pycityproto-1.12.0/pycityproto/city/person/v1/person_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/person/v1/person_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/person/v1/person_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/person/v1/person_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/person/v1/person_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/person/v1/person_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/ping/v1/ping_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/ping/v1/ping_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/ping/v1/ping_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/ping/v1/ping_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/routing/v2/cost_pb2.py` & `pycityproto-1.13.0/pycityproto/city/routing/v2/cost_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/routing/v2/cost_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/routing/v2/cost_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/routing/v2/routing_pb2.py` & `pycityproto-1.13.0/pycityproto/city/routing/v2/routing_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/routing/v2/routing_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/routing/v2/routing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/routing/v2/routing_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/routing/v2/routing_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/routing/v2/routing_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/routing/v2/routing_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/routing/v2/routing_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/routing/v2/routing_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/social/v1/message_pb2.py` & `pycityproto-1.13.0/pycityproto/city/social/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/social/v1/message_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/social/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/social/v1/social_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/social/v1/social_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/social/v1/social_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/social/v1/social_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/social/v1/social_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/social/v1/social_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/streetview/v1/streetview_pb2.py` & `pycityproto-1.13.0/pycityproto/city/streetview/v1/streetview_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/streetview/v1/streetview_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/streetview/v1/streetview_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/sync/v1/sync_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/sync/v1/sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/sync/v1/sync_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/sync/v1/sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/sync/v1/sync_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/sync/v1/sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/trip/v2/trip_pb2.py` & `pycityproto-1.13.0/pycityproto/city/trip/v2/trip_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/trip/v2/trip_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/trip/v2/trip_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/wargame/v1/wargame_pb2.py` & `pycityproto-1.13.0/pycityproto/city/wargame/v1/wargame_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/wargame/v1/wargame_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/wargame/v1/wargame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/wargame/v1/wargame_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/wargame/v1/wargame_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/wargame/v1/wargame_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/wargame/v1/wargame_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/wargame/v1/wargame_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/wargame/v1/wargame_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/input/v1/config_pb2.py` & `pycityproto-1.13.0/pycityproto/city/water/input/v1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/input/v1/config_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/water/input/v1/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/input/v1/input_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/water/input/v1/input_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/input/v1/input_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/water/input/v1/input_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/input/v1/input_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/water/input/v1/input_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/input/v1/water_pb2.py` & `pycityproto-1.13.0/pycityproto/city/water/input/v1/water_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/input/v1/water_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/water/input/v1/water_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/interaction/v1/water_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/water/interaction/v1/water_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/interaction/v1/water_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/water/interaction/v1/water_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/interaction/v1/water_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/water/interaction/v1/water_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/output/v1/output_pb2.py` & `pycityproto-1.13.0/pycityproto/city/water/output/v1/output_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/output/v1/output_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/water/output/v1/output_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/output/v1/output_service_pb2.py` & `pycityproto-1.13.0/pycityproto/city/water/output/v1/output_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/output/v1/output_service_pb2.pyi` & `pycityproto-1.13.0/pycityproto/city/water/output/v1/output_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto/city/water/output/v1/output_service_pb2_grpc.py` & `pycityproto-1.13.0/pycityproto/city/water/output/v1/output_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pycityproto.egg-info/PKG-INFO` & `pycityproto-1.13.0/pycityproto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityproto
-Version: 1.12.0
+Version: 1.13.0
 Summary: City Proto Generated Python SDK
 Author-email: Jun Zhang <zhangjun990222@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycityproto-1.12.0/pycityproto.egg-info/SOURCES.txt` & `pycityproto-1.13.0/pycityproto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycityproto-1.12.0/pyproject.toml` & `pycityproto-1.13.0/pyproject.toml`

 * *Files identical despite different names*

