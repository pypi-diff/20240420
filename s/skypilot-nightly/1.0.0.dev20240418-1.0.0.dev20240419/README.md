# Comparing `tmp/skypilot_nightly-1.0.0.dev20240418.tar.gz` & `tmp/skypilot_nightly-1.0.0.dev20240419.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot_nightly-1.0.0.dev20240418.tar", last modified: Thu Apr 18 10:39:10 2024, max compression
+gzip compressed data, was "skypilot_nightly-1.0.0.dev20240419.tar", last modified: Fri Apr 19 10:38:01 2024, max compression
```

## Comparing `skypilot_nightly-1.0.0.dev20240418.tar` & `skypilot_nightly-1.0.0.dev20240419.tar`

### file list

```diff
@@ -1,335 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.806936 skypilot_nightly-1.0.0.dev20240418/
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-18 10:39:10.806936 skypilot_nightly-1.0.0.dev20240418/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 10:39:10.806936 skypilot_nightly-1.0.0.dev20240418/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-18 10:39:07.000000 skypilot_nightly-1.0.0.dev20240418/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.738936 skypilot_nightly-1.0.0.dev20240418/sky/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-18 10:39:10.000000 skypilot_nightly-1.0.0.dev20240418/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.742936 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/adaptors/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    21410 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.742936 skypilot_nightly-1.0.0.dev20240418/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)   118820 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   221923 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.742936 skypilot_nightly-1.0.0.dev20240418/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.742936 skypilot_nightly-1.0.0.dev20240418/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (127)   186846 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.746936 skypilot_nightly-1.0.0.dev20240418/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43129 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    30940 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/cloud_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    46892 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16680 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/paperspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.750936 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/cudo_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.750936 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/fluidstack_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/kubernetes_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/paperspace_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/runpod_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/vsphere_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.754936 skypilot_nightly-1.0.0.dev20240418/sky/clouds/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/utils/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/utils/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/utils/oci_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/utils/scp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/clouds/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.754936 skypilot_nightly-1.0.0.dev20240418/sky/data/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   119221 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24916 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    54049 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.754936 skypilot_nightly-1.0.0.dev20240418/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.758936 skypilot_nightly-1.0.0.dev20240418/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36603 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/aws/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.758936 skypilot_nightly-1.0.0.dev20240418/sky/provision/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/azure/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.758936 skypilot_nightly-1.0.0.dev20240418/sky/provision/cudo/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/cudo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/cudo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/cudo/cudo_machine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/cudo/cudo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/cudo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/docker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.758936 skypilot_nightly-1.0.0.dev20240418/sky/provision/fluidstack/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/fluidstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/fluidstack/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/fluidstack/fluidstack_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14870 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/fluidstack/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.758936 skypilot_nightly-1.0.0.dev20240418/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22258 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/instance_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.762936 skypilot_nightly-1.0.0.dev20240418/sky/provision/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    32523 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/kubernetes/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/kubernetes/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/kubernetes/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    53819 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.762936 skypilot_nightly-1.0.0.dev20240418/sky/provision/paperspace/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/paperspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/paperspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/paperspace/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/paperspace/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/paperspace/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25255 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.762936 skypilot_nightly-1.0.0.dev20240418/sky/provision/runpod/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/runpod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/runpod/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/runpod/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/runpod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.762936 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.766936 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/cls_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/cls_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/metadata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/service_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/ssl_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/vapiconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/vim_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24476 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/vsphere_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    60100 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.766936 skypilot_nightly-1.0.0.dev20240418/sky/serve/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30137 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/serve/autoscalers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/serve/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/serve/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/serve/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/serve/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/serve/load_balancing_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    55738 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/serve/replica_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/serve/serve_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    36837 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/serve/serve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/serve/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/serve/service_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.770936 skypilot_nightly-1.0.0.dev20240418/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-18 10:39:07.000000 skypilot_nightly-1.0.0.dev20240418/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.770936 skypilot_nightly-1.0.0.dev20240418/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    35113 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18788 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/log_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/log_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.770936 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.774936 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/azure/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.774936 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.774936 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.774936 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.774936 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/scp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.778936 skypilot_nightly-1.0.0.dev20240418/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.778936 skypilot_nightly-1.0.0.dev20240418/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    25830 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/spot/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/spot/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.778936 skypilot_nightly-1.0.0.dev20240418/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.778936 skypilot_nightly-1.0.0.dev20240418/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.778936 skypilot_nightly-1.0.0.dev20240418/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    22487 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    31559 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    46443 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.782936 skypilot_nightly-1.0.0.dev20240418/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/cudo-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/fluidstack-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/kubernetes-ingress.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/kubernetes-loadbalancer.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/kubernetes-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/kubernetes-ssh-jump.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/paperspace-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/runpod-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/sky-serve-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/spot-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/templates/vsphere-ray.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.782936 skypilot_nightly-1.0.0.dev20240418/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.786936 skypilot_nightly-1.0.0.dev20240418/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.786936 skypilot_nightly-1.0.0.dev20240418/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/cluster_yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/command_runner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22349 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25413 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/controller_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/env_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.790936 skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9667 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/create_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/delete_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/generate_kind_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/gpu_labeler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/resources_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20387 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.794936 skypilot_nightly-1.0.0.dev20240418/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-18 10:39:10.000000 skypilot_nightly-1.0.0.dev20240418/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9162 2024-04-18 10:39:10.000000 skypilot_nightly-1.0.0.dev20240418/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:39:10.000000 skypilot_nightly-1.0.0.dev20240418/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 10:39:10.000000 skypilot_nightly-1.0.0.dev20240418/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-18 10:39:10.000000 skypilot_nightly-1.0.0.dev20240418/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-18 10:39:10.000000 skypilot_nightly-1.0.0.dev20240418/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:10.794936 skypilot_nightly-1.0.0.dev20240418/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_serve_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)   211236 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_spot_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_wheels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-18 10:39:00.000000 skypilot_nightly-1.0.0.dev20240418/tests/test_yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.687680 skypilot_nightly-1.0.0.dev20240419/
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-19 10:38:01.687680 skypilot_nightly-1.0.0.dev20240419/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:38:01.687680 skypilot_nightly-1.0.0.dev20240419/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-19 10:37:58.000000 skypilot_nightly-1.0.0.dev20240419/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.623679 skypilot_nightly-1.0.0.dev20240419/sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-19 10:38:01.000000 skypilot_nightly-1.0.0.dev20240419/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.623679 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/adaptors/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21410 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.627679 skypilot_nightly-1.0.0.dev20240419/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118820 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   221923 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.627679 skypilot_nightly-1.0.0.dev20240419/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.627679 skypilot_nightly-1.0.0.dev20240419/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)   186846 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.631679 skypilot_nightly-1.0.0.dev20240419/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43129 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/cloud_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46901 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16680 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/paperspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.631679 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/cudo_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.635680 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/fluidstack_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/kubernetes_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/paperspace_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/runpod_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/vsphere_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.635680 skypilot_nightly-1.0.0.dev20240419/sky/clouds/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/utils/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/utils/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/utils/oci_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/utils/scp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/clouds/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.635680 skypilot_nightly-1.0.0.dev20240419/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119221 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24916 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54049 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.639680 skypilot_nightly-1.0.0.dev20240419/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.639680 skypilot_nightly-1.0.0.dev20240419/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36603 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/aws/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.639680 skypilot_nightly-1.0.0.dev20240419/sky/provision/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/azure/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.639680 skypilot_nightly-1.0.0.dev20240419/sky/provision/cudo/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/cudo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/cudo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/cudo/cudo_machine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/cudo/cudo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/cudo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/docker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.643679 skypilot_nightly-1.0.0.dev20240419/sky/provision/fluidstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/fluidstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/fluidstack/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/fluidstack/fluidstack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14870 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/fluidstack/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.643679 skypilot_nightly-1.0.0.dev20240419/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22258 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/instance_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.643679 skypilot_nightly-1.0.0.dev20240419/sky/provision/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32523 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/kubernetes/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/kubernetes/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/kubernetes/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53819 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.643679 skypilot_nightly-1.0.0.dev20240419/sky/provision/paperspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/paperspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/paperspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/paperspace/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/paperspace/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/paperspace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25255 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.647680 skypilot_nightly-1.0.0.dev20240419/sky/provision/runpod/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/runpod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/runpod/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/runpod/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/runpod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.647680 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.647680 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/cls_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/cls_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/metadata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/service_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/ssl_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/vapiconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/vim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24476 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/vsphere_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60100 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.651680 skypilot_nightly-1.0.0.dev20240419/sky/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30137 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/serve/autoscalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/serve/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/serve/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/serve/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/serve/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/serve/load_balancing_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55738 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/serve/replica_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/serve/serve_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36837 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/serve/serve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/serve/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/serve/service_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.651680 skypilot_nightly-1.0.0.dev20240419/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-19 10:37:58.000000 skypilot_nightly-1.0.0.dev20240419/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.655680 skypilot_nightly-1.0.0.dev20240419/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35113 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18788 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/log_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/log_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.655680 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.655680 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/azure/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.655680 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.655680 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.659680 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.659680 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/scp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.659680 skypilot_nightly-1.0.0.dev20240419/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.659680 skypilot_nightly-1.0.0.dev20240419/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25830 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/spot/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/spot/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.663680 skypilot_nightly-1.0.0.dev20240419/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.663680 skypilot_nightly-1.0.0.dev20240419/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.663680 skypilot_nightly-1.0.0.dev20240419/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22487 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31559 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46443 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.667680 skypilot_nightly-1.0.0.dev20240419/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/cudo-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/fluidstack-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/kubernetes-ingress.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/kubernetes-loadbalancer.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/kubernetes-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/kubernetes-ssh-jump.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/paperspace-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/runpod-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/sky-serve-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/spot-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/templates/vsphere-ray.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.667680 skypilot_nightly-1.0.0.dev20240419/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.671680 skypilot_nightly-1.0.0.dev20240419/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.671680 skypilot_nightly-1.0.0.dev20240419/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/cluster_yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/command_runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22349 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25413 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/controller_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/env_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.671680 skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9667 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/create_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/delete_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/generate_kind_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/gpu_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/resources_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20387 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.675680 skypilot_nightly-1.0.0.dev20240419/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-19 10:38:01.000000 skypilot_nightly-1.0.0.dev20240419/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9162 2024-04-19 10:38:01.000000 skypilot_nightly-1.0.0.dev20240419/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:38:01.000000 skypilot_nightly-1.0.0.dev20240419/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 10:38:01.000000 skypilot_nightly-1.0.0.dev20240419/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-19 10:38:01.000000 skypilot_nightly-1.0.0.dev20240419/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 10:38:01.000000 skypilot_nightly-1.0.0.dev20240419/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:38:01.675680 skypilot_nightly-1.0.0.dev20240419/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_serve_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)   211236 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_spot_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_wheels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-19 10:37:56.000000 skypilot_nightly-1.0.0.dev20240419/tests/test_yaml_parser.py
```

### Comparing `skypilot_nightly-1.0.0.dev20240418/LICENSE` & `skypilot_nightly-1.0.0.dev20240419/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240419/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240419/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240418
+Version: 1.0.0.dev20240419
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240418/README.md` & `skypilot_nightly-1.0.0.dev20240419/README.md`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/pyproject.toml` & `skypilot_nightly-1.0.0.dev20240419/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/setup.py` & `skypilot_nightly-1.0.0.dev20240419/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The SkyPilot package."""
 import os
 import subprocess
 from typing import Optional
 import urllib.request
 
 # Replaced with the current commit when building the wheels.
-_SKYPILOT_COMMIT_SHA = '20493fb61601ce00d612073ebad4706bbccdf487'
+_SKYPILOT_COMMIT_SHA = 'cade827c538aeade90584aa18c3a3d5a34033b09'
 
 
 def _get_git_commit():
     if 'SKYPILOT_COMMIT_SHA' not in _SKYPILOT_COMMIT_SHA:
         # This is a release build, so we don't need to get the commit hash from
         # git, as it's already been set.
         return _SKYPILOT_COMMIT_SHA
@@ -31,15 +31,15 @@
             commit_hash += '-dirty'
         return commit_hash
     except Exception:  # pylint: disable=broad-except
         return _SKYPILOT_COMMIT_SHA
 
 
 __commit__ = _get_git_commit()
-__version__ = '1.0.0.dev20240418'
+__version__ = '1.0.0.dev20240419'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 
 # ---------------------- Proxy Configuration ---------------------- #
 def _set_http_proxy_env_vars() -> None:
     urllib_proxies = dict(urllib.request.getproxies())
```

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/adaptors/aws.py` & `skypilot_nightly-1.0.0.dev20240419/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/adaptors/azure.py` & `skypilot_nightly-1.0.0.dev20240419/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/adaptors/cloudflare.py` & `skypilot_nightly-1.0.0.dev20240419/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/adaptors/common.py` & `skypilot_nightly-1.0.0.dev20240419/sky/adaptors/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/adaptors/gcp.py` & `skypilot_nightly-1.0.0.dev20240419/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/adaptors/ibm.py` & `skypilot_nightly-1.0.0.dev20240419/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/adaptors/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240419/sky/adaptors/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/adaptors/oci.py` & `skypilot_nightly-1.0.0.dev20240419/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/adaptors/vsphere.py` & `skypilot_nightly-1.0.0.dev20240419/sky/adaptors/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/authentication.py` & `skypilot_nightly-1.0.0.dev20240419/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/backends/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/backends/backend.py` & `skypilot_nightly-1.0.0.dev20240419/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/backends/backend_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/backends/cloud_vm_ray_backend.py` & `skypilot_nightly-1.0.0.dev20240419/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/backends/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/backends/local_docker_backend.py` & `skypilot_nightly-1.0.0.dev20240419/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot_nightly-1.0.0.dev20240419/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/backends/wheel_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/benchmark/benchmark_state.py` & `skypilot_nightly-1.0.0.dev20240419/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/benchmark/benchmark_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/check.py` & `skypilot_nightly-1.0.0.dev20240419/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/cli.py` & `skypilot_nightly-1.0.0.dev20240419/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/cloud_stores.py` & `skypilot_nightly-1.0.0.dev20240419/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/aws.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/azure.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,15 +290,16 @@
         acc_count = None
         if acc_dict is not None:
             custom_resources = json.dumps(acc_dict, separators=(',', ':'))
             acc_count = str(sum(acc_dict.values()))
         else:
             custom_resources = None
 
-        if resources.image_id is None:
+        if (resources.image_id is None or
+                resources.extract_docker_image() is not None):
             # pylint: disable=import-outside-toplevel
             from sky.clouds.service_catalog import azure_catalog
             gen_version = azure_catalog.get_gen_version_from_instance_type(
                 r.instance_type)
             image_id = self._get_default_image_tag(gen_version, r.instance_type)
         else:
             if None in resources.image_id:
```

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/cloud.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/cloud_registry.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/cloud_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/cudo.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/fluidstack.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/gcp.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/gcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,16 +457,16 @@
                     # versions of CUDA as noted below.
                     # CUDA driver version 470.57.02, CUDA Library 11.4
                     image_id = 'skypilot:k80-debian-10'
                 else:
                     # CUDA driver version 535.86.10, CUDA Library 12.2
                     image_id = 'skypilot:gpu-debian-11'
 
-        if resources.image_id is not None and resources.extract_docker_image(
-        ) is None:
+        if (resources.image_id is not None and
+                resources.extract_docker_image() is None):
             if None in resources.image_id:
                 image_id = resources.image_id[None]
             else:
                 assert region_name in resources.image_id, resources.image_id
                 image_id = resources.image_id[region_name]
         if image_id.startswith('skypilot:'):
             image_id = service_catalog.get_image_id_from_tag(image_id,
```

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/ibm.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/oci.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/paperspace.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/paperspace.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/runpod.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/runpod.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/scp.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/aws_catalog.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/azure_catalog.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/common.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/config.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/cudo_catalog.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/cudo_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/fluidstack_catalog.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/fluidstack_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/kubernetes_catalog.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/kubernetes_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/oci_catalog.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/paperspace_catalog.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/paperspace_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/runpod_catalog.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/runpod_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/scp_catalog.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/service_catalog/vsphere_catalog.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/service_catalog/vsphere_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/utils/gcp_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/utils/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/utils/lambda_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/utils/oci_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/utils/oci_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/utils/scp_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/utils/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/clouds/vsphere.py` & `skypilot_nightly-1.0.0.dev20240419/sky/clouds/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/core.py` & `skypilot_nightly-1.0.0.dev20240419/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/dag.py` & `skypilot_nightly-1.0.0.dev20240419/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/data/data_transfer.py` & `skypilot_nightly-1.0.0.dev20240419/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/data/data_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/data/mounting_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/data/storage.py` & `skypilot_nightly-1.0.0.dev20240419/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/data/storage_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/exceptions.py` & `skypilot_nightly-1.0.0.dev20240419/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/execution.py` & `skypilot_nightly-1.0.0.dev20240419/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/global_user_state.py` & `skypilot_nightly-1.0.0.dev20240419/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/optimizer.py` & `skypilot_nightly-1.0.0.dev20240419/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/aws/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/aws/config.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/aws/instance.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/aws/utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/azure/instance.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/azure/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/common.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/cudo/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/cudo/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/cudo/cudo_machine_type.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/cudo/cudo_machine_type.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/cudo/cudo_wrapper.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/cudo/cudo_wrapper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/cudo/instance.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/cudo/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/fluidstack/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/fluidstack/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/fluidstack/fluidstack_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/fluidstack/fluidstack_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/fluidstack/instance.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/fluidstack/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/gcp/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/gcp/config.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/gcp/constants.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/gcp/instance.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/gcp/instance_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/instance_setup.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/instance_setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/kubernetes/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/kubernetes/config.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/kubernetes/instance.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/kubernetes/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/kubernetes/network.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/kubernetes/network.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/kubernetes/network_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/kubernetes/network_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/kubernetes/utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/logging.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/paperspace/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/paperspace/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/paperspace/config.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/paperspace/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/paperspace/constants.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/paperspace/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/paperspace/instance.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/paperspace/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/paperspace/utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/paperspace/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/provisioner.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/provisioner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/runpod/instance.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/runpod/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/runpod/utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/runpod/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/cls_api_client.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/cls_api_client.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/cls_api_helper.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/cls_api_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/service_manager.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/service_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/service_manager_factory.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/service_manager_factory.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/ssl_helper.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/ssl_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/vapiconnect.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/vapiconnect.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/common/vim_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/common/vim_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/instance.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/provision/vsphere/vsphere_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/provision/vsphere/vsphere_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/resources.py` & `skypilot_nightly-1.0.0.dev20240419/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/serve/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/serve/autoscalers.py` & `skypilot_nightly-1.0.0.dev20240419/sky/serve/autoscalers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/serve/constants.py` & `skypilot_nightly-1.0.0.dev20240419/sky/serve/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/serve/controller.py` & `skypilot_nightly-1.0.0.dev20240419/sky/serve/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/serve/core.py` & `skypilot_nightly-1.0.0.dev20240419/sky/serve/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/serve/load_balancer.py` & `skypilot_nightly-1.0.0.dev20240419/sky/serve/load_balancer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/serve/load_balancing_policies.py` & `skypilot_nightly-1.0.0.dev20240419/sky/serve/load_balancing_policies.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/serve/replica_managers.py` & `skypilot_nightly-1.0.0.dev20240419/sky/serve/replica_managers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/serve/serve_state.py` & `skypilot_nightly-1.0.0.dev20240419/sky/serve/serve_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/serve/serve_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/serve/service.py` & `skypilot_nightly-1.0.0.dev20240419/sky/serve/service.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/serve/service_spec.py` & `skypilot_nightly-1.0.0.dev20240419/sky/serve/service_spec.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/setup_files/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240419/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/setup_files/setup.py` & `skypilot_nightly-1.0.0.dev20240419/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/sky_logging.py` & `skypilot_nightly-1.0.0.dev20240419/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/LICENSE` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/attempt_skylet.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/autostop_lib.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/configs.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/constants.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/events.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/job_lib.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/log_lib.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/log_lib.pyi` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/log_lib.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/azure/azure-config-template.json` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/azure/config.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/azure/node_provider.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/command_runner.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/ibm/node_provider.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/ibm/utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/oci/node_provider.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/oci/query_helper.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/scp/config.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/providers/scp/node_provider.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/ray_patches/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/ray_patches/worker.py.patch` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/skylet.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skylet/subprocess_daemon.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/skypilot_config.py` & `skypilot_nightly-1.0.0.dev20240419/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/spot/__init__.py` & `skypilot_nightly-1.0.0.dev20240419/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/spot/constants.py` & `skypilot_nightly-1.0.0.dev20240419/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/spot/controller.py` & `skypilot_nightly-1.0.0.dev20240419/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/spot/core.py` & `skypilot_nightly-1.0.0.dev20240419/sky/spot/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/spot/dashboard/dashboard.py` & `skypilot_nightly-1.0.0.dev20240419/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/spot/dashboard/static/favicon.ico` & `skypilot_nightly-1.0.0.dev20240419/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/spot/dashboard/templates/index.html` & `skypilot_nightly-1.0.0.dev20240419/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/spot/recovery_strategy.py` & `skypilot_nightly-1.0.0.dev20240419/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/spot/spot_state.py` & `skypilot_nightly-1.0.0.dev20240419/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/spot/spot_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/status_lib.py` & `skypilot_nightly-1.0.0.dev20240419/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/task.py` & `skypilot_nightly-1.0.0.dev20240419/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/aws-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/azure-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/cudo-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/cudo-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/fluidstack-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/fluidstack-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/gcp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/ibm-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/kubernetes-ingress.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/kubernetes-ingress.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/kubernetes-port-forward-proxy-command.sh.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/kubernetes-port-forward-proxy-command.sh.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/kubernetes-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/kubernetes-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/kubernetes-ssh-jump.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/kubernetes-ssh-jump.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/lambda-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/local-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/oci-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/paperspace-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/paperspace-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/runpod-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/runpod-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/scp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/sky-serve-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/sky-serve-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/spot-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/templates/vsphere-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240419/sky/templates/vsphere-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/usage/constants.py` & `skypilot_nightly-1.0.0.dev20240419/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/usage/usage_lib.py` & `skypilot_nightly-1.0.0.dev20240419/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/accelerator_registry.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/cli_utils/status_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/cluster_yaml_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/cluster_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/command_runner.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/command_runner.pyi` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/command_runner.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/common_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/controller_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/controller_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/dag_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/db_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/env_options.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/create_cluster.sh` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/delete_cluster.sh` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/delete_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/generate_kind_config.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/generate_kind_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/gpu_labeler.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/gpu_labeler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/kubernetes_enums.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/kubernetes_enums.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/log_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/resources_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/resources_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/rich_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/schemas.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/subprocess_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/timeline.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/ux_utils.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/sky/utils/validator.py` & `skypilot_nightly-1.0.0.dev20240419/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/skypilot_nightly.egg-info/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240419/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240418
+Version: 1.0.0.dev20240419
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240418/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot_nightly-1.0.0.dev20240419/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/skypilot_nightly.egg-info/requires.txt` & `skypilot_nightly-1.0.0.dev20240419/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/tests/test_cli.py` & `skypilot_nightly-1.0.0.dev20240419/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/tests/test_config.py` & `skypilot_nightly-1.0.0.dev20240419/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/tests/test_jobs.py` & `skypilot_nightly-1.0.0.dev20240419/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/tests/test_list_accelerators.py` & `skypilot_nightly-1.0.0.dev20240419/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/tests/test_optimizer_dryruns.py` & `skypilot_nightly-1.0.0.dev20240419/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/tests/test_optimizer_random_dag.py` & `skypilot_nightly-1.0.0.dev20240419/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/tests/test_serve_autoscaler.py` & `skypilot_nightly-1.0.0.dev20240419/tests/test_serve_autoscaler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/tests/test_smoke.py` & `skypilot_nightly-1.0.0.dev20240419/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/tests/test_spot_serve.py` & `skypilot_nightly-1.0.0.dev20240419/tests/test_spot_serve.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/tests/test_storage.py` & `skypilot_nightly-1.0.0.dev20240419/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/tests/test_wheels.py` & `skypilot_nightly-1.0.0.dev20240419/tests/test_wheels.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240418/tests/test_yaml_parser.py` & `skypilot_nightly-1.0.0.dev20240419/tests/test_yaml_parser.py`

 * *Files identical despite different names*

