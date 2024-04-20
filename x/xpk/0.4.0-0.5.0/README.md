# Comparing `tmp/xpk-0.4.0.tar.gz` & `tmp/xpk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpk-0.4.0.tar", last modified: Wed Apr 17 21:29:30 2024, max compression
+gzip compressed data, was "xpk-0.5.0.tar", last modified: Sat Apr 20 01:25:49 2024, max compression
```

## Comparing `xpk-0.4.0.tar` & `xpk-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-x---   0 sjsurbhi (1142443) primarygroup (89939)        0 2024-04-17 21:29:30.540634 xpk-0.4.0/
--rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)    11358 2024-04-17 21:29:16.000000 xpk-0.4.0/LICENSE
--rw-r--r--   0 sjsurbhi (1142443) primarygroup (89939)    44328 2024-04-17 21:29:30.540634 xpk-0.4.0/PKG-INFO
--rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)    43614 2024-04-17 21:29:16.000000 xpk-0.4.0/README.md
--rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)     1767 2024-04-17 21:29:16.000000 xpk-0.4.0/pyproject.toml
--rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)       38 2024-04-17 21:29:30.540634 xpk-0.4.0/setup.cfg
-drwxr-x---   0 sjsurbhi (1142443) primarygroup (89939)        0 2024-04-17 21:29:30.540634 xpk-0.4.0/xpk.egg-info/
--rw-r--r--   0 sjsurbhi (1142443) primarygroup (89939)    44328 2024-04-17 21:29:30.000000 xpk-0.4.0/xpk.egg-info/PKG-INFO
--rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)      203 2024-04-17 21:29:30.000000 xpk-0.4.0/xpk.egg-info/SOURCES.txt
--rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)        1 2024-04-17 21:29:30.000000 xpk-0.4.0/xpk.egg-info/dependency_links.txt
--rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)       33 2024-04-17 21:29:30.000000 xpk-0.4.0/xpk.egg-info/entry_points.txt
--rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)       76 2024-04-17 21:29:30.000000 xpk-0.4.0/xpk.egg-info/requires.txt
--rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)        4 2024-04-17 21:29:30.000000 xpk-0.4.0/xpk.egg-info/top_level.txt
--rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)   215487 2024-04-17 21:29:16.000000 xpk-0.4.0/xpk.py
+drwxr-x---   0 sjsurbhi (1142443) primarygroup (89939)        0 2024-04-20 01:25:49.547335 xpk-0.5.0/
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)    11358 2024-04-17 21:29:16.000000 xpk-0.5.0/LICENSE
+-rw-r--r--   0 sjsurbhi (1142443) primarygroup (89939)    44137 2024-04-20 01:25:49.547335 xpk-0.5.0/PKG-INFO
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)    43423 2024-04-20 00:54:25.000000 xpk-0.5.0/README.md
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)     1767 2024-04-17 21:29:16.000000 xpk-0.5.0/pyproject.toml
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)       38 2024-04-20 01:25:49.547335 xpk-0.5.0/setup.cfg
+drwxr-x---   0 sjsurbhi (1142443) primarygroup (89939)        0 2024-04-20 01:25:49.547335 xpk-0.5.0/xpk.egg-info/
+-rw-r--r--   0 sjsurbhi (1142443) primarygroup (89939)    44137 2024-04-20 01:25:49.000000 xpk-0.5.0/xpk.egg-info/PKG-INFO
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)      203 2024-04-20 01:25:49.000000 xpk-0.5.0/xpk.egg-info/SOURCES.txt
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)        1 2024-04-20 01:25:49.000000 xpk-0.5.0/xpk.egg-info/dependency_links.txt
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)       33 2024-04-20 01:25:49.000000 xpk-0.5.0/xpk.egg-info/entry_points.txt
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)       76 2024-04-20 01:25:49.000000 xpk-0.5.0/xpk.egg-info/requires.txt
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)        4 2024-04-20 01:25:49.000000 xpk-0.5.0/xpk.egg-info/top_level.txt
+-rw-r-----   0 sjsurbhi (1142443) primarygroup (89939)   217498 2024-04-20 01:25:36.000000 xpk-0.5.0/xpk.py
```

### Comparing `xpk-0.4.0/LICENSE` & `xpk-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xpk-0.4.0/PKG-INFO` & `xpk-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: xpk
-Version: 0.4.0
-Summary: xpk helps Cloud developers to orchestrate training jobs on accelerators on GKE.
-Author-email: Cloud TPU Team <cloud-tpu-eng@google.com>
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/google/xpk
-Project-URL: Bug Tracker, https://github.com/google/xpk/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: cloud-accelerator-diagnostics
-Provides-Extra: dev
-Requires-Dist: pyink==24.3.0; extra == "dev"
-Requires-Dist: pylint>=2.6.0; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-
 <!--
  Copyright 2023 Google LLC
 
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at
 
@@ -135,22 +116,14 @@
 # gcloud config:
 gcloud config set project $PROJECT_ID
 gcloud config set compute/zone $ZONE
 # xpk arguments
 xpk .. --zone $ZONE --project $PROJECT_ID
 ```
 
-`Cluster Create` command will create a project-specific Service Account. Note that only one service 
-account will be created per project. This service account will be attached to the node pools instead of default 
-[Compute Engine Service Account](https://cloud.google.com/compute/docs/access/service-accounts#default_service_account). 
-All the required permissions will be assigned to this service account by XPK. Make sure you have 
-[Service Account Admin](https://cloud.google.com/iam/docs/understanding-roles#iam.serviceAccountAdmin) and 
-[Project IAM Admin](https://cloud.google.com/iam/docs/understanding-roles#resourcemanager.projectIamAdmin) 
-roles assigned to your user account.
-
 The cluster created is a regional cluster to enable the GKE control plane across
 all zones.
 
 *   Cluster Create (provision reserved capacity):
 
     ```shell
     # Find your reservations
@@ -222,15 +195,17 @@
     python3 xpk.py cluster create --force \
     --cluster xpk-test --tpu-type=v5litepod-16 \
     --num-slices=6  --reservation=$RESERVATION_ID
 
     ```
 
 ### Create Vertex AI Tensorboard
-*Note: This feature is available in XPK >= 0.4.0. Enable [Vertex AI API](https://cloud.google.com/vertex-ai/docs/start/cloud-environment#enable_vertexai_apis) in your Google Cloud console to use this feature.*
+*Note: This feature is available in XPK >= 0.4.0. Enable [Vertex AI API](https://cloud.google.com/vertex-ai/docs/start/cloud-environment#enable_vertexai_apis) in your Google Cloud console to use this feature. Make sure you have
+[Vertex AI Administrator](https://cloud.google.com/vertex-ai/docs/general/access-control#aiplatform.admin) role
+assigned to your user account.*
 
 Vertex AI Tensorboard is a fully managed version of open-source Tensorboard. To learn more about Vertex AI Tensorboard, visit [this](https://cloud.google.com/vertex-ai/docs/experiments/tensorboard-introduction). Note that Vertex AI Tensorboard is only available in [these](https://cloud.google.com/vertex-ai/docs/general/locations#available-regions) regions.
 
 You can create a Vertex AI Tensorboard for your cluster with `Cluster Create` command. XPK will create a single Vertex AI Tensorboard instance per cluster.
 
 * Create Vertex AI Tensorboard in default region with default Tensorboard name:
 
@@ -382,15 +357,17 @@
   ```shell
   python3 xpk.py workload create \
   --workload xpk-test-medium-workload --command "echo goodbye" --cluster \
   xpk-test --tpu-type=v5litepod-16 --priority=medium
   ```
 
 ### Create Vertex AI Experiment to upload data to Vertex AI Tensorboard
-*Note: This feature is available in XPK >= 0.4.0. Enable [Vertex AI API](https://cloud.google.com/vertex-ai/docs/start/cloud-environment#enable_vertexai_apis) in your Google Cloud console to use this feature.*
+*Note: This feature is available in XPK >= 0.4.0. Enable [Vertex AI API](https://cloud.google.com/vertex-ai/docs/start/cloud-environment#enable_vertexai_apis) in your Google Cloud console to use this feature. Make sure you have
+[Vertex AI Administrator](https://cloud.google.com/vertex-ai/docs/general/access-control#aiplatform.admin) role
+assigned to your user account and to the [Compute Engine Service account](https://cloud.google.com/compute/docs/access/service-accounts#default_service_account) attached to the node pools in the cluster.*
 
 Vertex AI Experiment is a tool that helps to track and analyze an experiment run on Vertex AI Tensorboard. To learn more about Vertex AI Experiments, visit [this](https://cloud.google.com/vertex-ai/docs/experiments/intro-vertex-ai-experiments).
 
 XPK will create a Vertex AI Experiment in `workload create` command and attach the Vertex AI Tensorboard created for the cluster during `cluster create`. If there is a cluster created before this feature is released, there will be no Vertex AI Tensorboard created for the cluster and `workload create` will fail. Re-run `cluster create` to create a Vertex AI Tensorboard and then run `workload create` again to schedule your workload.
 
 * Create Vertex AI Experiment with default Experiment name:
```

### Comparing `xpk-0.4.0/README.md` & `xpk-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: xpk
+Version: 0.5.0
+Summary: xpk helps Cloud developers to orchestrate training jobs on accelerators on GKE.
+Author-email: Cloud TPU Team <cloud-tpu-eng@google.com>
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/google/xpk
+Project-URL: Bug Tracker, https://github.com/google/xpk/issues
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cloud-accelerator-diagnostics
+Provides-Extra: dev
+Requires-Dist: pyink==24.3.0; extra == "dev"
+Requires-Dist: pylint>=2.6.0; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+
 <!--
  Copyright 2023 Google LLC
 
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at
 
@@ -116,22 +135,14 @@
 # gcloud config:
 gcloud config set project $PROJECT_ID
 gcloud config set compute/zone $ZONE
 # xpk arguments
 xpk .. --zone $ZONE --project $PROJECT_ID
 ```
 
-`Cluster Create` command will create a project-specific Service Account. Note that only one service 
-account will be created per project. This service account will be attached to the node pools instead of default 
-[Compute Engine Service Account](https://cloud.google.com/compute/docs/access/service-accounts#default_service_account). 
-All the required permissions will be assigned to this service account by XPK. Make sure you have 
-[Service Account Admin](https://cloud.google.com/iam/docs/understanding-roles#iam.serviceAccountAdmin) and 
-[Project IAM Admin](https://cloud.google.com/iam/docs/understanding-roles#resourcemanager.projectIamAdmin) 
-roles assigned to your user account.
-
 The cluster created is a regional cluster to enable the GKE control plane across
 all zones.
 
 *   Cluster Create (provision reserved capacity):
 
     ```shell
     # Find your reservations
@@ -203,15 +214,17 @@
     python3 xpk.py cluster create --force \
     --cluster xpk-test --tpu-type=v5litepod-16 \
     --num-slices=6  --reservation=$RESERVATION_ID
 
     ```
 
 ### Create Vertex AI Tensorboard
-*Note: This feature is available in XPK >= 0.4.0. Enable [Vertex AI API](https://cloud.google.com/vertex-ai/docs/start/cloud-environment#enable_vertexai_apis) in your Google Cloud console to use this feature.*
+*Note: This feature is available in XPK >= 0.4.0. Enable [Vertex AI API](https://cloud.google.com/vertex-ai/docs/start/cloud-environment#enable_vertexai_apis) in your Google Cloud console to use this feature. Make sure you have
+[Vertex AI Administrator](https://cloud.google.com/vertex-ai/docs/general/access-control#aiplatform.admin) role
+assigned to your user account.*
 
 Vertex AI Tensorboard is a fully managed version of open-source Tensorboard. To learn more about Vertex AI Tensorboard, visit [this](https://cloud.google.com/vertex-ai/docs/experiments/tensorboard-introduction). Note that Vertex AI Tensorboard is only available in [these](https://cloud.google.com/vertex-ai/docs/general/locations#available-regions) regions.
 
 You can create a Vertex AI Tensorboard for your cluster with `Cluster Create` command. XPK will create a single Vertex AI Tensorboard instance per cluster.
 
 * Create Vertex AI Tensorboard in default region with default Tensorboard name:
 
@@ -363,15 +376,17 @@
   ```shell
   python3 xpk.py workload create \
   --workload xpk-test-medium-workload --command "echo goodbye" --cluster \
   xpk-test --tpu-type=v5litepod-16 --priority=medium
   ```
 
 ### Create Vertex AI Experiment to upload data to Vertex AI Tensorboard
-*Note: This feature is available in XPK >= 0.4.0. Enable [Vertex AI API](https://cloud.google.com/vertex-ai/docs/start/cloud-environment#enable_vertexai_apis) in your Google Cloud console to use this feature.*
+*Note: This feature is available in XPK >= 0.4.0. Enable [Vertex AI API](https://cloud.google.com/vertex-ai/docs/start/cloud-environment#enable_vertexai_apis) in your Google Cloud console to use this feature. Make sure you have
+[Vertex AI Administrator](https://cloud.google.com/vertex-ai/docs/general/access-control#aiplatform.admin) role
+assigned to your user account and to the [Compute Engine Service account](https://cloud.google.com/compute/docs/access/service-accounts#default_service_account) attached to the node pools in the cluster.*
 
 Vertex AI Experiment is a tool that helps to track and analyze an experiment run on Vertex AI Tensorboard. To learn more about Vertex AI Experiments, visit [this](https://cloud.google.com/vertex-ai/docs/experiments/intro-vertex-ai-experiments).
 
 XPK will create a Vertex AI Experiment in `workload create` command and attach the Vertex AI Tensorboard created for the cluster during `cluster create`. If there is a cluster created before this feature is released, there will be no Vertex AI Tensorboard created for the cluster and `workload create` will fail. Re-run `cluster create` to create a Vertex AI Tensorboard and then run `workload create` again to schedule your workload.
 
 * Create Vertex AI Experiment with default Experiment name:
```

### Comparing `xpk-0.4.0/pyproject.toml` & `xpk-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xpk-0.4.0/xpk.egg-info/PKG-INFO` & `xpk-0.5.0/xpk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpk
-Version: 0.4.0
+Version: 0.5.0
 Summary: xpk helps Cloud developers to orchestrate training jobs on accelerators on GKE.
 Author-email: Cloud TPU Team <cloud-tpu-eng@google.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/google/xpk
 Project-URL: Bug Tracker, https://github.com/google/xpk/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -135,22 +135,14 @@
 # gcloud config:
 gcloud config set project $PROJECT_ID
 gcloud config set compute/zone $ZONE
 # xpk arguments
 xpk .. --zone $ZONE --project $PROJECT_ID
 ```
 
-`Cluster Create` command will create a project-specific Service Account. Note that only one service 
-account will be created per project. This service account will be attached to the node pools instead of default 
-[Compute Engine Service Account](https://cloud.google.com/compute/docs/access/service-accounts#default_service_account). 
-All the required permissions will be assigned to this service account by XPK. Make sure you have 
-[Service Account Admin](https://cloud.google.com/iam/docs/understanding-roles#iam.serviceAccountAdmin) and 
-[Project IAM Admin](https://cloud.google.com/iam/docs/understanding-roles#resourcemanager.projectIamAdmin) 
-roles assigned to your user account.
-
 The cluster created is a regional cluster to enable the GKE control plane across
 all zones.
 
 *   Cluster Create (provision reserved capacity):
 
     ```shell
     # Find your reservations
@@ -222,15 +214,17 @@
     python3 xpk.py cluster create --force \
     --cluster xpk-test --tpu-type=v5litepod-16 \
     --num-slices=6  --reservation=$RESERVATION_ID
 
     ```
 
 ### Create Vertex AI Tensorboard
-*Note: This feature is available in XPK >= 0.4.0. Enable [Vertex AI API](https://cloud.google.com/vertex-ai/docs/start/cloud-environment#enable_vertexai_apis) in your Google Cloud console to use this feature.*
+*Note: This feature is available in XPK >= 0.4.0. Enable [Vertex AI API](https://cloud.google.com/vertex-ai/docs/start/cloud-environment#enable_vertexai_apis) in your Google Cloud console to use this feature. Make sure you have
+[Vertex AI Administrator](https://cloud.google.com/vertex-ai/docs/general/access-control#aiplatform.admin) role
+assigned to your user account.*
 
 Vertex AI Tensorboard is a fully managed version of open-source Tensorboard. To learn more about Vertex AI Tensorboard, visit [this](https://cloud.google.com/vertex-ai/docs/experiments/tensorboard-introduction). Note that Vertex AI Tensorboard is only available in [these](https://cloud.google.com/vertex-ai/docs/general/locations#available-regions) regions.
 
 You can create a Vertex AI Tensorboard for your cluster with `Cluster Create` command. XPK will create a single Vertex AI Tensorboard instance per cluster.
 
 * Create Vertex AI Tensorboard in default region with default Tensorboard name:
 
@@ -382,15 +376,17 @@
   ```shell
   python3 xpk.py workload create \
   --workload xpk-test-medium-workload --command "echo goodbye" --cluster \
   xpk-test --tpu-type=v5litepod-16 --priority=medium
   ```
 
 ### Create Vertex AI Experiment to upload data to Vertex AI Tensorboard
-*Note: This feature is available in XPK >= 0.4.0. Enable [Vertex AI API](https://cloud.google.com/vertex-ai/docs/start/cloud-environment#enable_vertexai_apis) in your Google Cloud console to use this feature.*
+*Note: This feature is available in XPK >= 0.4.0. Enable [Vertex AI API](https://cloud.google.com/vertex-ai/docs/start/cloud-environment#enable_vertexai_apis) in your Google Cloud console to use this feature. Make sure you have
+[Vertex AI Administrator](https://cloud.google.com/vertex-ai/docs/general/access-control#aiplatform.admin) role
+assigned to your user account and to the [Compute Engine Service account](https://cloud.google.com/compute/docs/access/service-accounts#default_service_account) attached to the node pools in the cluster.*
 
 Vertex AI Experiment is a tool that helps to track and analyze an experiment run on Vertex AI Tensorboard. To learn more about Vertex AI Experiments, visit [this](https://cloud.google.com/vertex-ai/docs/experiments/intro-vertex-ai-experiments).
 
 XPK will create a Vertex AI Experiment in `workload create` command and attach the Vertex AI Tensorboard created for the cluster during `cluster create`. If there is a cluster created before this feature is released, there will be no Vertex AI Tensorboard created for the cluster and `workload create` will fail. Re-run `cluster create` to create a Vertex AI Tensorboard and then run `workload create` again to schedule your workload.
 
 * Create Vertex AI Experiment with default Experiment name:
```

### Comparing `xpk-0.4.0/xpk.py` & `xpk-0.5.0/xpk.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,16 @@
   )
 
 
 ################### Internally used constants ##############
 
 default_docker_image = 'python:3.10'
 default_script_dir = os.getcwd()
-default_gke_version = '1.29.1-gke.1589017'
 # This is the version for XPK PyPI package
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 xpk_current_version = __version__
 
 h100_device_type = 'h100-80gb-8'
 
 _AUTOPROVISIONING_CONFIG_VALUE = 'AUTOPROVISION'
 _AUTOPROVISIONING_CONFIG_MINIMUM_KEY = 'minimum_chips'
 _AUTOPROVISIONING_CONFIG_MAXIMUM_KEY = 'maximum_chips'
@@ -81,18 +80,15 @@
 _CAPACITY_TYPE_CONFIG_KEY = 'capacity_type'
 _RESERVATION_CONFIG_KEY = 'reservation_id'
 _CLUSTER_QUEUE_NAME = 'cluster-queue'
 _LOCAL_QUEUE_NAME = 'multislice-queue'
 _DEFAULT_POOL_NAME = 'default-pool'
 _CLUSTER_RESOURCES_CONFIGMAP = 'resources-configmap'
 _CLUSTER_METADATA_CONFIGMAP = 'metadata-configmap'
-_XPK_SERVICE_ACCOUNT = 'xpk-sa'
-# Set to True to attach a service account to cluster & node pools
-_SERVICE_ACCOUNT_FEATURE_FLAG = xpk_current_version >= '0.4.0'
-_VERTEX_TENSORBOARD_FEATURE_FLAG = _SERVICE_ACCOUNT_FEATURE_FLAG
+_VERTEX_TENSORBOARD_FEATURE_FLAG = xpk_current_version >= '0.4.0'
 _DEFAULT_VERTEX_TENSORBOARD_NAME = 'tb-instance'
 
 
 class CapacityType(enum.Enum):
   ON_DEMAND = 'on_demand'
   RESERVATION = 'reservation'
   SPOT = 'spot'
@@ -260,19 +256,20 @@
     template:
       metadata:
         annotations:
           alpha.jobset.sigs.k8s.io/exclusive-topology: cloud.google.com/gke-nodepool
         labels:
           xpk.google.com/workload: {args.workload}
       spec:
-        backoffLimit: 0
+        backoffLimit: 4
         completions: {system.vms_per_slice}
         parallelism: {system.vms_per_slice}
         template:
           spec:
+            terminationGracePeriodSeconds: {args.termination_grace_period_seconds}
             containers:
             - args:
               {pathways_worker_args}
               image: {args.server_image}
               imagePullPolicy: Always
               name: pathways-worker
               ports:
@@ -607,15 +604,14 @@
 autoprovisioning_config_file = """
 management:
   autoRepair: true
   autoUpgrade: true
 autoprovisioningLocations:
   {zones}
 {resource_limits}
-{service_account}
 """
 
 autoprovisioning_resource_limits = """
 resourceLimits:
 - resourceType: 'cpu'
   {cpu_limits}
 - resourceType: 'memory'
@@ -625,24 +621,14 @@
 
 autoprovisioning_custom_resource_type = """
 - resourceType: {resource_type}
   minimum: {minimum}
   maximum: {maximum}
 """
 
-# Add IAM roles to attach to service account used by node pools in the cluster
-IAMRoles = {
-    'Kubernetes Engine Admin': 'roles/container.admin',
-    'Artifact Registry Writer': 'roles/artifactregistry.writer',
-    'Monitoring Admin': 'roles/monitoring.admin',
-    'Logging Admin': 'roles/logging.admin',
-    'Storage Admin': 'roles/storage.admin',
-    'Vertex AI Administrator': 'roles/aiplatform.admin',
-}
-
 
 AcceleratorType = {'TPU': 1, 'GPU': 2, 'CPU': 3}
 
 
 @dataclass
 class AutoprovisioningConfig:
   config_filename: str
@@ -1887,14 +1873,22 @@
     ),
 }
 """ If you modify UserFacingNameToSystemCharacteristics you should also modify
 the corresponding Map in MaxText/accelerator_to_spec_map.py """
 # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 
+PathwaysExpectedInstancesMap = {
+    'v5p': 'v5',
+    'v5litepod': 'v5e',
+    'v4': 'v4',
+    'v3': 'v3',
+}
+
+
 def chunks(lst, n):
   """Return a list of n-sized chunks from lst.
 
   Args:
     lst: input list to get chunks from.
     n: size of each chunk.
 
@@ -2158,25 +2152,32 @@
   with open(file=file.name, mode='a', encoding='utf=8') as f:
     f.write(payload)
     f.flush()
   return file
 
 
 def run_command_for_value(
-    command, task, global_args, dry_run_return_val='0', print_timer=False
+    command,
+    task,
+    global_args,
+    dry_run_return_val='0',
+    print_timer=False,
+    hide_error=False,
 ) -> tuple[int, str]:
   """Runs the command and returns the error code and stdout.
 
   Prints errors and associated user-facing information
 
   Args:
     command: user provided command to run.
     task: user provided task name for running the command.
     global_args: user provided arguments for running the command.
     dry_run_return_val: return value of this command for dry run.
+    print_timer: print out the time the command is running.
+    hide_error: hide the error from the command output upon success.
 
   Returns:
     tuple[int, str]
     int: return_code, default is 0
     str: return_val, default is '0'
   """
   if global_args.dry_run:
@@ -2212,15 +2213,15 @@
         f'Task: `{task}` is implemented by `{command}`, hiding output unless'
         ' there is an error.'
     )
     try:
       output = subprocess.check_output(
           command,
           shell=True,
-          stderr=subprocess.STDOUT,
+          stderr=subprocess.STDOUT if not hide_error else None,
       )
     except subprocess.CalledProcessError as e:
       xpk_print(f'Task {task} failed with {e.returncode}')
       xpk_print('*' * 80)
       xpk_print(e.output)
       xpk_print('*' * 80)
       return e.returncode, str(e.output, 'UTF-8')
@@ -2393,150 +2394,14 @@
   Returns:
      The region name.
   """
   zone_terms = zone.split('-')
   return zone_terms[0] + '-' + zone_terms[1]
 
 
-def get_service_account_name(args) -> str:
-  """Get the name for the service account.
-  Args:
-    args: user provided arguments.
-
-  Returns:
-    the name of the service account.
-  """
-  return f'{args.project}-{_XPK_SERVICE_ACCOUNT}@{args.project}.iam.gserviceaccount.com'
-
-
-def check_if_service_account_exists(args) -> bool:
-  """Check if a service account with the given name exists in the project.
-
-  Args:
-    args: user provided arguments for running the command.
-
-  Returns:
-    True if service account exist, False otherwise.
-  """
-  service_account_name = get_service_account_name(args)
-  command = f'gcloud iam service-accounts describe {service_account_name}'
-  return_code = run_command_with_updates(
-      command, 'Service Account Describe', args, verbose=False
-  )
-  if return_code != 0:
-    xpk_print(
-        'Service Account Describe did not find the service account'
-        f' {service_account_name}.'
-    )
-    return False
-  return True
-
-
-def create_service_account(args) -> int:
-  """Creates a service account in the project.
-
-  Args:
-    args: user provided arguments for running the command.
-
-  Returns:
-    0 if successful and 1 otherwise.
-  """
-  command = (
-      'gcloud iam service-accounts create'
-      f' {args.project}-{_XPK_SERVICE_ACCOUNT}     --description="Service'
-      ' Account for XPK"    '
-      f' --display-name="{args.project}-{_XPK_SERVICE_ACCOUNT}"'
-  )
-  return_code = run_command_with_updates(
-      command, 'Service Account Create', args
-  )
-  if return_code != 0:
-    xpk_print(f'Service Account Create request returned ERROR {return_code}')
-    xpk_print(
-        'Make sure you have Service Account Admin Role attached to your user.'
-    )
-    return 1
-  return 0
-
-
-def get_existing_roles_in_service_account(args) -> set:
-  """
-  Args:
-    args: user provided arguments for running the command.
-
-  Returns:
-    set of IAM roles already attached to the service account.
-  """
-  roles = set()
-  service_account_name = get_service_account_name(args)
-  command = (
-      f'gcloud projects get-iam-policy {args.project}'
-      f' --filter="bindings.members:{service_account_name}"'
-      ' --flatten="bindings[].members" --format="table(bindings.role)"'
-  )
-  return_code, return_value = run_command_for_value(
-      command, 'Get IAM Roles For Service Account', args
-  )
-  if return_code != 0:
-    xpk_print(
-        'Get IAM Roles For Service Account request returned ERROR'
-        f' {return_code}'
-    )
-  else:
-    return_value = return_value.strip()
-    roles = set(return_value.split('\n'))
-    """Format of return_value is:
-          ROLE
-          roles/storage.admin
-          roles/logging.admin
-      removing `ROLE` from the list
-    """
-    if 'ROLE' in roles:
-      roles.remove('ROLE')
-  return roles
-
-
-def add_roles_to_service_account(args) -> int:
-  """Add IAM roles to service account.
-
-  Args:
-    args: user provided arguments for running the command.
-
-  Returns:
-    0 if successful and 1 otherwise.
-  """
-  service_account_name = get_service_account_name(args)
-  existing_roles = get_existing_roles_in_service_account(args)
-  xpk_print(f'IAM roles already attached to service account: {existing_roles}')
-
-  for name, role in IAMRoles.items():
-    if role in existing_roles:
-      continue
-
-    xpk_print(f'Adding {name} role to service account: {service_account_name}.')
-    command = (
-        f'gcloud projects add-iam-policy-binding {args.project}      '
-        f' --member="serviceAccount:{service_account_name}"      '
-        f' --role="{role}"       --condition=None'
-    )
-    return_code = run_command_with_updates(
-        command, 'Add IAM Role to Service Account', args, verbose=False
-    )
-    if return_code != 0:
-      xpk_print(
-          'Add IAM Role to Service Account request returned ERROR'
-          f' {return_code}'
-      )
-      xpk_print(
-          'Make sure you have Project IAM Admin Role attached to your user.'
-      )
-      return 1
-  return 0
-
-
 def get_total_chips_requested_from_args(
     args, system: SystemCharacteristics
 ) -> int:
   """Return the total chips requested based on user args.
 
   Args:
     args: user provided arguments for running the command.
@@ -2627,24 +2492,15 @@
 
   resource_limits = autoprovisioning_resource_limits.format(
       cpu_limits=cpu_limits,
       memory_limits=memory_limits,
       custom_resource_type=custom_resource_string,
   )
 
-  # Default service_account is the project's default service account.
-  service_account = ''
-  if _SERVICE_ACCOUNT_FEATURE_FLAG:
-    service_account_name = get_service_account_name(args)
-    service_account_exists = check_if_service_account_exists(args)
-    if service_account_exists:
-      service_account = f'serviceAccount: {service_account_name}'
-
   yml_string = autoprovisioning_config_file.format(
-      service_account=service_account,
       resource_limits=resource_limits,
       zones=f'- {args.zone}',
   )
   autoprovisioning_config = AutoprovisioningConfig(
       config_filename=write_temporary_file(yml_string).name,
       minimum_chips=minimum,
       maximum_chips=maximum,
@@ -2739,19 +2595,20 @@
         'Update node pools with autoprovisioning support returned ERROR:'
         f' {max_return_code}'
     )
     return None, max_return_code
   return autoprovisioning_config, return_code
 
 
-def run_gke_cluster_create_command(args) -> int:
+def run_gke_cluster_create_command(args, gke_control_plane_version: str) -> int:
   """Run the Create GKE Cluster request.
 
   Args:
     args: user provided arguments for running the command.
+    gke_control_plane_version: version used if creating the cluster.
 
   Returns:
     0 if successful and 1 otherwise.
   """
   # cluster_cpu_machine_type is soon to be deprecated!
   machine_type = args.default_pool_cpu_machine_type
   if args.cluster_cpu_machine_type != '':
@@ -2768,33 +2625,22 @@
   # benefit from a larger initial `--num-nodes`. After the cluster is created,
   # the auto-scaler can reduce/increase the nodes based on the load.
   command = (
       'gcloud beta container clusters create'
       f' {args.cluster} --project={args.project}'
       f' --region={zone_to_region(args.zone)}'
       f' --node-locations={args.zone}'
-      f' --cluster-version={args.gke_version}'
+      f' --cluster-version={gke_control_plane_version}'
       f' --machine-type={machine_type}'
       ' --enable-autoscaling'
       ' --total-min-nodes 1 --total-max-nodes 1000'
       f' --num-nodes {args.default_pool_cpu_num_nodes}'
       f' {args.custom_cluster_arguments}'
   )
 
-  if _SERVICE_ACCOUNT_FEATURE_FLAG:
-    service_account_name = get_service_account_name(args)
-    service_account_exists = check_if_service_account_exists(args)
-    if service_account_exists:
-      command += f' --service-account={service_account_name}'
-    else:
-      xpk_print(
-          f'Service Account: {service_account_name} does not exist in the'
-          ' project. Will attach the default service account to the cluster.'
-      )
-
   device_type = args.tpu_type if args.tpu_type else args.device_type
   if device_type == h100_device_type:
     command += (
         ' --enable-dataplane-v2 --enable-ip-alias'
         ' --enable-multi-networking --no-enable-autoupgrade'
     )
   else:
@@ -3372,32 +3218,33 @@
   if return_code != 0:
     xpk_print(f'Find if Cluster Exists returned ERROR {return_code}')
     return [], return_code
   cluster_names = [x.split(' ')[0] for x in raw_cluster_output.splitlines()]
   return cluster_names, 0
 
 
-def create_cluster_if_necessary(args) -> int:
+def create_cluster_if_necessary(args, gke_control_plane_version: str) -> int:
   """Creates cluster if not present in the project.
 
   Args:
     args: user provided arguments for running the command.
+    gke_control_plane_version: version used if creating the cluster.
 
   Returns:
     0 if successful and 1 otherwise.
   """
   all_clusters, return_code = get_all_clusters_programmatic(args)
   if return_code > 0:
     xpk_print('Listing all clusters failed!')
     return 1
   if args.cluster in all_clusters:
-    xpk_print('Skipping cluster creation since it already exists')
+    xpk_print('Skipping cluster creation since it already exists.')
     return 0
   else:
-    return run_gke_cluster_create_command(args)
+    return run_gke_cluster_create_command(args, gke_control_plane_version)
 
 
 def get_all_nodepools_programmatic(args) -> tuple[list[str], int]:
   """Gets all the nodepools associated with the cluster / project / region.
 
   Args:
     args: user provided arguments for running the command.
@@ -3495,20 +3342,23 @@
   Returns:
     True if user enter y or yes at the prompt, False otherwise.
   """
   user_input = input(input_msg)
   return user_input in ('y', 'yes')
 
 
-def run_gke_node_pool_create_command(args, system) -> int:
+def run_gke_node_pool_create_command(
+    args, system, gke_node_pool_version
+) -> int:
   """Run the Create GKE Node Pool request.
 
   Args:
     args: user provided arguments for running the command.
     system: System characteristics based on device type/topology.
+    gke_node_pool_version: GKE version to use to create node pools.
 
   Returns:
     0 if successful and 1 otherwise.
   """
   device_type = args.tpu_type if args.tpu_type else args.device_type
   xpk_print(
       f'Creating {args.num_slices} node pool or pools of {device_type}\n'
@@ -3570,18 +3420,20 @@
         f' --machine-type={system.gce_machine_type}'
         f' --host-maintenance-interval={args.host_maintenance_interval}'
         f' {capacity_args}'
         ' --enable-gvnic'
         f' {args.custom_nodepool_arguments}'
     )
     if system.accelerator_type == AcceleratorType['TPU']:
-      command += f' --node-version={args.gke_version}'
+      command += f' --node-version={gke_node_pool_version}'
       command += f' --num-nodes={system.vms_per_slice}'
       command += ' --placement-type=COMPACT  --max-pods-per-node 15'
-      command += ' --scopes=storage-full,gke-default'
+      command += (
+          ' --scopes=storage-full,gke-default,"https://www.googleapis.com/auth/cloud-platform"'
+      )
       command += f' --tpu-topology={system.topology}'
       command += f' {args.custom_tpu_nodepool_arguments}'
     elif system.accelerator_type == AcceleratorType['GPU']:
       subnet_prefix = f'{args.cluster}-{zone_to_region(args.zone)}'
       command += f' --num-nodes={args.num_nodes}'
       command += (
           ' --accelerator'
@@ -3597,38 +3449,27 @@
           ' --no-enable-autoupgrade '
           ' --scopes="https://www.googleapis.com/auth/cloud-platform"'
       )
     elif system.accelerator_type == AcceleratorType['CPU']:
       command += f' --num-nodes={system.vms_per_slice}'
       command += ' --scopes=storage-full,gke-default'
 
-    if _SERVICE_ACCOUNT_FEATURE_FLAG:
-      service_account_name = get_service_account_name(args)
-      service_account_exists = check_if_service_account_exists(args)
-      if service_account_exists:
-        command += f' --service-account={service_account_name}'
-      else:
-        xpk_print(
-            f'Service Account: {service_account_name} does not exist in the'
-            ' project. Will attach the default service account to the node'
-            ' pools.'
-        )
     task = f'NodepoolCreate-{node_pool_name}'
     commands.append(command)
     task_names.append(task)
 
   desired_pw_cpu_node_pools = ['cpu-user-np', 'cpu-rm-np', 'cpu-proxy-np']
   if args.enable_pathways:
     # Pathways needs CPU nodepools in addition to TPU nodepools
     for node_pool_name in desired_pw_cpu_node_pools:
       if node_pool_name in existing_node_pool_names:
         continue
       command = (
           'gcloud beta container node-pools create'
-          f' {node_pool_name} --node-version={args.gke_version}'
+          f' {node_pool_name} --node-version={gke_node_pool_version}'
           f' --cluster={args.cluster}'
           f' --project={args.project} --node-locations={args.zone}'
           f' --region={zone_to_region(args.zone)}'
           ' --num-nodes=1'
           f' --machine-type={args.pathways_gce_machine_type}'
           ' --scopes=storage-full,gke-default'
           ' --enable-autoscaling --min-nodes=1 --max-nodes=20'
@@ -4056,14 +3897,192 @@
         f'Install NCCL Plugin On Cluster request returned ERROR {return_code}'
     )
     return 1
 
   return 0
 
 
+@dataclass
+class GkeServerConfig:
+  """Stores the valid gke versions based on gcloud recommendations."""
+
+  default_rapid_gke_version: str
+  valid_master_versions: set[str]
+  valid_node_versions: set[str]
+
+
+def get_gke_server_config(args) -> tuple[int, GkeServerConfig | None]:
+  """Determine the GKE versions supported by gcloud currently.
+
+  Args:
+    args: user provided arguments for running the command.
+
+  Returns:
+    Tuple of
+    int: 0 if successful and 1 otherwise.
+    GkeServerConfig: stores valid gke version to use in node pool and cluster.
+  """
+  base_command = (
+      'gcloud container get-server-config'
+      f' --project={args.project} --region={zone_to_region(args.zone)}'
+  )
+  default_rapid_gke_version_cmd = (
+      base_command
+      + ' --flatten="channels" --filter="channels.channel=RAPID"'
+      ' --format="value(channels.defaultVersion)"'
+  )
+  valid_master_versions_cmd = (
+      base_command
+      + ' --flatten="channels" --format="value(validMasterVersions)"'
+  )
+  valid_node_versions_cmd = (
+      base_command + ' --flatten="channels" --format="value(validNodeVersions)"'
+  )
+  base_command_description = 'Determine server supported GKE versions for'
+
+  server_config_commands_and_descriptions = [
+      (
+          default_rapid_gke_version_cmd,
+          base_command_description + 'default rapid gke version',
+      ),
+      (
+          valid_master_versions_cmd,
+          base_command_description + 'valid master versions',
+      ),
+      (
+          valid_node_versions_cmd,
+          base_command_description + 'valid node versions',
+      ),
+  ]
+  command_outputs = []
+
+  for command, command_description in server_config_commands_and_descriptions:
+    return_code, cmd_output = run_command_for_value(
+        command,
+        command_description,
+        args,
+        hide_error=True,
+    )
+    if return_code != 0:
+      xpk_print(f'Unable to get server config for {command_description}.')
+      return return_code, None
+    command_outputs.append(cmd_output)
+
+  return 0, GkeServerConfig(
+      default_rapid_gke_version=command_outputs[0].strip(),
+      valid_master_versions=set(command_outputs[1].split(';')),
+      valid_node_versions=set(command_outputs[2].split(';')),
+  )
+
+
+def get_gke_control_plane_version(
+    args, gke_server_config: GkeServerConfig
+) -> tuple[int, str | None]:
+  """Determine gke control plane version for cluster creation.
+
+  Args:
+    args: user provided arguments for running the command.
+    gke_server_config: holds valid gke versions and recommended default version.
+
+  Returns:
+    Tuple of
+    int: 0 if successful and 1 otherwise.
+    str: gke control plane version to use.
+  """
+
+  # Override with user provide gke version if specified.
+  if args.gke_version is not None:
+    master_gke_version = args.gke_version
+  else:
+    master_gke_version = gke_server_config.default_rapid_gke_version
+
+  is_valid_master_version = (
+      master_gke_version in gke_server_config.valid_master_versions
+  )
+  is_valid_node_version = (
+      master_gke_version in gke_server_config.valid_node_versions
+  )
+
+  if not is_valid_master_version or not is_valid_node_version:
+    xpk_print(
+        f'Planned GKE Version: {master_gke_version}\n Valid Master'
+        f' Versions:\n{gke_server_config.valid_master_versions}\nValid Node'
+        f' Versions:\n{gke_server_config.valid_node_versions}\nRecommended GKE'
+        f' Version: {gke_server_config.default_rapid_gke_version}'
+    )
+    xpk_print(
+        f'Error: Planned GKE Version {master_gke_version} is not valid.'
+        f'Checks failed: Is Master Valid: {is_valid_master_version}'
+        f'\nIs Valid Node Version: {is_valid_node_version}'
+    )
+    xpk_print(
+        'Please select a gke version from the above list using --gke-version=x'
+        ' argument or rely on the default gke version:'
+        f' {gke_server_config.default_rapid_gke_version}'
+    )
+    return 1, None
+
+  return 0, master_gke_version
+
+
+def get_gke_node_pool_version(
+    args, gke_server_config: GkeServerConfig
+) -> tuple[int, str | None]:
+  """Determine the gke node pool version for the node pool.
+
+  Args:
+    args: user provided arguments for running the command.
+    gke_server_config: holds valid gke versions and recommended default version.
+
+  Returns:
+    Tuple of
+    int: 0 if successful and 1 otherwise.
+    str: gke control plane version to use.
+  """
+
+  # By default use the current gke master version for creating node pools.
+  command_description = 'Determine current gke master version'
+  command = (
+      f'gcloud beta container clusters describe {args.cluster}'
+      f' --region {zone_to_region(args.zone)} --project {args.project}'
+      ' --format="value(currentMasterVersion)"'
+  )
+
+  return_code, current_gke_master_version = run_command_for_value(
+      command, command_description, args
+  )
+  if return_code != 0:
+    xpk_print(
+        f'Unable to get server config for command: {command_description}.'
+    )
+    return return_code, None
+
+  # Override with user provide gke version if specified.
+  if args.gke_version is not None:
+    node_pool_gke_version = args.gke_version
+  else:
+    node_pool_gke_version = current_gke_master_version.strip()
+
+  is_supported_node_pool_version = (
+      node_pool_gke_version in gke_server_config.valid_node_versions
+  )
+  # In rare cases, user's provided gke version may be invalid, but gke will return an error if so.
+  # An example scenario is if the user provided gke version is greater than the master version.
+  if not is_supported_node_pool_version:
+    xpk_print(
+        f'Planned node pool version {node_pool_gke_version} is not supported in'
+        ' valid node_pool_gke_versions'
+        f' {gke_server_config.valid_node_versions}Please adjust the gke version'
+        ' using --gke-version=x or remove the arg and depend on xpk default of'
+        f' {current_gke_master_version}'
+    )
+    return 1, None
+  return 0, node_pool_gke_version
+
+
 ################### Subcommand Functions ###################
 def default_subcommand_function(
     _args,
 ) -> int:  # args is unused, so pylint: disable=invalid-name
   """Default subcommand function.
 
   Args:
@@ -4093,34 +4112,27 @@
   if return_code > 0:
     xpk_print('Fetching system characteristics failed!')
     xpk_exit(return_code)
 
   xpk_print(f'Starting cluster create for cluster {args.cluster}:', flush=True)
   add_zone_and_project(args)
 
-  if _SERVICE_ACCOUNT_FEATURE_FLAG:
-    service_account_name = get_service_account_name(args)
-    service_account_exists = check_if_service_account_exists(args)
-    if service_account_exists:
-      xpk_print(
-          f'Service Account: {service_account_name} already exist in the'
-          ' project. Will not create a new service account.'
-      )
-    else:
-      # create a service account in the project
-      create_service_account_code = create_service_account(args)
-      if create_service_account_code != 0:
-        xpk_exit(create_service_account_code)
-
-    # add IAM roles to the service account
-    add_roles_to_service_account_code = add_roles_to_service_account(args)
-    if add_roles_to_service_account_code != 0:
-      xpk_exit(add_roles_to_service_account_code)
+  return_code, gke_server_config = get_gke_server_config(args)
+  if return_code != 0:
+    xpk_exit(return_code)
 
-  create_cluster_command_code = create_cluster_if_necessary(args)
+  return_code, gke_control_plane_version = get_gke_control_plane_version(
+      args, gke_server_config
+  )
+  if return_code != 0:
+    xpk_exit(return_code)
+
+  create_cluster_command_code = create_cluster_if_necessary(
+      args, gke_control_plane_version
+  )
   if create_cluster_command_code != 0:
     xpk_exit(create_cluster_command_code)
 
   set_cluster_command_code = set_cluster_command(args)
   if set_cluster_command_code != 0:
     xpk_exit(set_cluster_command_code)
 
@@ -4140,16 +4152,24 @@
       xpk_exit(set_up_cluster_network_code)
 
     xpk_print('Creating Network Config for cluster')
     create_cluster_network_config_code = create_cluster_network_config(args)
     if create_cluster_network_config_code != 0:
       xpk_exit(create_cluster_network_config_code)
 
+  # Check the control plane version of the cluster and determine the node pool
+  # version to use.
+  return_code, gke_node_pool_version = get_gke_node_pool_version(
+      args, gke_server_config
+  )
+  if return_code != 0:
+    xpk_exit(return_code)
+
   run_gke_node_pool_create_command_code = run_gke_node_pool_create_command(
-      args, system
+      args, system, gke_node_pool_version
   )
   if run_gke_node_pool_create_command_code != 0:
     xpk_exit(run_gke_node_pool_create_command_code)
 
   xpk_print(
       'Enabling the jobset API on our cluster, to be deprecated when Jobset is'
       ' globally available'
@@ -4814,36 +4834,79 @@
     return gpu_volume_yaml
 
   regular_volume_mount_yaml = """- mountPath: /dev/shm
                   name: dshm-2"""
   return regular_volume_mount_yaml
 
 
-def get_pathways_rm_args(args) -> str:
+def get_pathways_rm_args(args, system: SystemCharacteristics) -> str:
   """Arguments for the Pathways resource manager.
   Args:
     args: user provided arguments for running the command.
 
   Returns:
     str: yaml containing arguments for the Pathways resource manager.
   """
   yaml = """- --alsologtostderr
               - --pathways_server_port=38677
               - --pathways_server_provides_devices=false
               - --pathways_device_type=NONE
               - --pathways_persistent_compilation_cache=false
               - --pathways_compilation_mode=compile_at_worker
               - --pathways_tmp_dir_pattern={args.pathways_gcs_location}
-              - --pathways_resource_manager_expected_num_worker_jobs={args.num_slices}"""
+              - --pathways_expected_instances={expected_instances}"""
   if args.use_pathways:
-    return yaml.format(args=args)
+    return yaml.format(
+        args=args,
+        expected_instances=compute_pathways_expected_instances(args, system),
+    )
   else:
     return ''
 
 
+def compute_pathways_expected_instances(
+    args, system: SystemCharacteristics
+) -> str:
+  """Computes the expected instances from the system characteristics.
+  Args:
+    args: user provided args.
+    system: system characteristics.
+
+  Returns:
+    str: formatted string representing the expected instances (eg:
+    "tpuv4:2x2x2,tpuv4:2x2x2" for 2 slices of v4-16).
+  """
+  expected_instances = ','.join([
+      f'tpu{get_pathways_expected_tpu_type(system.device_type)}:{system.topology}'
+      for _ in range(args.num_slices)
+  ])
+
+  xpk_print(f'Pathways expected instances are: {expected_instances}')
+  return expected_instances
+
+
+def get_pathways_expected_tpu_type(device_type: str) -> str:
+  """Returns the device type expected by Pathways
+  Args:
+    device_type: the system characteristic device type
+
+  Returns:
+    str: the device type expected by pathways.
+  """
+  raw_type = device_type.split('-')[0].lower()
+  pathways_expected_instance = PathwaysExpectedInstancesMap[raw_type]
+  if not pathways_expected_instance:
+    xpk_print(
+        f'Passed in device_type {device_type} is incorrect. Please pass in a'
+        ' valid device type'
+    )
+    xpk_exit(1)
+  return pathways_expected_instance
+
+
 def get_pathways_worker_args(args) -> str:
   """Arguments for the Pathways workers.
   Args:
     args: user provided arguments for running the command.
 
   Returns:
     str: yaml containing arguments for the Pathways workers.
@@ -5512,15 +5575,15 @@
         args=args,
         system=system,
         container=container,
         accelerator_label=create_accelerator_label(
             system.accelerator_type, system
         ),
         machine_label=create_machine_label(system.accelerator_type, system),
-        pathways_rm_args=get_pathways_rm_args(args),
+        pathways_rm_args=get_pathways_rm_args(args, system),
         pathways_worker_args=get_pathways_worker_args(args),
         pathways_proxy_args=get_pathways_proxy_args(args),
         resource_type=resource_type,
         local_queue_name=_LOCAL_QUEUE_NAME,
         autoprovisioning_args=autoprovisioning_args,
     )
   else:
@@ -5757,14 +5820,15 @@
 
   return_code, return_value = run_command_for_value(
       command,
       f'List Jobs with filter-by-status={args.filter_by_status}'
       f' with filter-by-jobs={args.filter_by_job}',
       args,
   )
+
   return return_code, return_value
 
 
 def wait_for_job_completion(args) -> int:
   """Function to wait for job completion.
 
   Args:
@@ -5865,15 +5929,15 @@
     args.filter_by_job = args.wait_for_job_completion
 
   return_code, return_value = get_workload_list(args)
 
   if return_code != 0:
     xpk_print(f'List Job request returned ERROR {return_code}')
     xpk_exit(return_code)
-  xpk_print(return_value)
+  xpk_print(f'Workload List Output:\n{return_value}')
   xpk_exit(0)
 
 
 def inspector_run_command_helper(
     args, command, command_description, file
 ) -> int:
   """Runs a command for xpk inspector, and build the output file.
@@ -6376,18 +6440,18 @@
     choices=['AS_NEEDED', 'PERIODIC'],
     default='AS_NEEDED',
     help='The maintenance policy of the cluster and respective clusters.',
 )
 cluster_create_optional_arguments.add_argument(
     '--gke-version',
     type=str,
-    default=default_gke_version,
     help=(
-        'The GKE version of the cluster and respective clusters. The default is'
-        f' "{default_gke_version}".'
+        'The GKE version of the cluster and respective clusters. The'
+        ' default is'
+        ' determined dynamically based on RAPID channel recommended version.'
     ),
 )
 cluster_create_optional_arguments.add_argument(
     '--num-slices',
     type=int,
     default=1,
     help='The number of slices to run the job on, defaults to 1.',
```

