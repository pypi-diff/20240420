# Comparing `tmp/botocore-a-la-carte-imagebuilder-1.34.87.tar.gz` & `tmp/botocore-a-la-carte-imagebuilder-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-imagebuilder-1.34.87.tar", last modified: Fri Apr 19 01:00:55 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-imagebuilder-1.34.9.tar", last modified: Thu Dec 28 01:06:46 2023, max compression
```

## Comparing `botocore-a-la-carte-imagebuilder-1.34.87.tar` & `botocore-a-la-carte-imagebuilder-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:55.908603 botocore-a-la-carte-imagebuilder-1.34.87/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-19 01:00:55.000000 botocore-a-la-carte-imagebuilder-1.34.87/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-19 01:00:55.908603 botocore-a-la-carte-imagebuilder-1.34.87/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:55.904603 botocore-a-la-carte-imagebuilder-1.34.87/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:55.908603 botocore-a-la-carte-imagebuilder-1.34.87/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:55.908603 botocore-a-la-carte-imagebuilder-1.34.87/botocore/data/imagebuilder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:55.908603 botocore-a-la-carte-imagebuilder-1.34.87/botocore/data/imagebuilder/2019-12-02/
--rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-04-19 01:00:35.000000 botocore-a-la-carte-imagebuilder-1.34.87/botocore/data/imagebuilder/2019-12-02/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 01:00:35.000000 botocore-a-la-carte-imagebuilder-1.34.87/botocore/data/imagebuilder/2019-12-02/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 01:00:35.000000 botocore-a-la-carte-imagebuilder-1.34.87/botocore/data/imagebuilder/2019-12-02/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   342893 2024-04-19 01:00:35.000000 botocore-a-la-carte-imagebuilder-1.34.87/botocore/data/imagebuilder/2019-12-02/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:55.908603 botocore-a-la-carte-imagebuilder-1.34.87/botocore_a_la_carte_imagebuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-19 01:00:55.000000 botocore-a-la-carte-imagebuilder-1.34.87/botocore_a_la_carte_imagebuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-19 01:00:55.000000 botocore-a-la-carte-imagebuilder-1.34.87/botocore_a_la_carte_imagebuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:00:55.000000 botocore-a-la-carte-imagebuilder-1.34.87/botocore_a_la_carte_imagebuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 01:00:55.000000 botocore-a-la-carte-imagebuilder-1.34.87/botocore_a_la_carte_imagebuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:00:55.908603 botocore-a-la-carte-imagebuilder-1.34.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-19 01:00:55.000000 botocore-a-la-carte-imagebuilder-1.34.87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.230314 botocore-a-la-carte-imagebuilder-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:45.000000 botocore-a-la-carte-imagebuilder-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2023-12-28 01:06:46.230314 botocore-a-la-carte-imagebuilder-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.226314 botocore-a-la-carte-imagebuilder-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.226314 botocore-a-la-carte-imagebuilder-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.226314 botocore-a-la-carte-imagebuilder-1.34.9/botocore/data/imagebuilder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.230314 botocore-a-la-carte-imagebuilder-1.34.9/botocore/data/imagebuilder/2019-12-02/
+-rw-r--r--   0 runner    (1001) docker     (127)    15322 2023-12-28 01:06:26.000000 botocore-a-la-carte-imagebuilder-1.34.9/botocore/data/imagebuilder/2019-12-02/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-imagebuilder-1.34.9/botocore/data/imagebuilder/2019-12-02/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-28 01:06:26.000000 botocore-a-la-carte-imagebuilder-1.34.9/botocore/data/imagebuilder/2019-12-02/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   342458 2023-12-28 01:06:26.000000 botocore-a-la-carte-imagebuilder-1.34.9/botocore/data/imagebuilder/2019-12-02/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.230314 botocore-a-la-carte-imagebuilder-1.34.9/botocore_a_la_carte_imagebuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2023-12-28 01:06:46.000000 botocore-a-la-carte-imagebuilder-1.34.9/botocore_a_la_carte_imagebuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2023-12-28 01:06:46.000000 botocore-a-la-carte-imagebuilder-1.34.9/botocore_a_la_carte_imagebuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:46.000000 botocore-a-la-carte-imagebuilder-1.34.9/botocore_a_la_carte_imagebuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:46.000000 botocore-a-la-carte-imagebuilder-1.34.9/botocore_a_la_carte_imagebuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:46.230314 botocore-a-la-carte-imagebuilder-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-28 01:06:45.000000 botocore-a-la-carte-imagebuilder-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-imagebuilder-1.34.87/LICENSE.txt` & `botocore-a-la-carte-imagebuilder-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-imagebuilder-1.34.87/PKG-INFO` & `botocore-a-la-carte-imagebuilder-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-imagebuilder
-Version: 1.34.87
+Version: 1.34.9
 Summary: imagebuilder data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-imagebuilder-1.34.87/botocore/data/imagebuilder/2019-12-02/endpoint-rule-set-1.json` & `botocore-a-la-carte-imagebuilder-1.34.9/botocore/data/imagebuilder/2019-12-02/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-imagebuilder-1.34.87/botocore/data/imagebuilder/2019-12-02/service-2.json` & `botocore-a-la-carte-imagebuilder-1.34.9/botocore/data/imagebuilder/2019-12-02/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999887908742074%*

 * *Differences: {"'shapes'": "{'LifecycleExecutionResource': {'members': {delete: ['startTime', 'endTime']}}, "*

 * *             "'LifecycleExecutionStatus': {'enum': {delete: [5]}}, "*

 * *             "'LifecyclePolicyDetailExclusionRules': {'members': {'tagMap': {'documentation': "*

 * *             "'<p>Contains a list of tags that Image Builder uses to skip lifecycle actions for "*

 * *             "resources that have them.</p>'}}}, 'LifecyclePolicyResourceSelection': {'members': "*

 * *             "{'tagMap': {'documentation': '<p>A list  […]*

```diff
@@ -6692,18 +6692,14 @@
                     "documentation": "<p>The account that owns the impacted resource.</p>",
                     "shape": "NonEmptyString"
                 },
                 "action": {
                     "documentation": "<p>The action to take for the identified resource.</p>",
                     "shape": "LifecycleExecutionResourceAction"
                 },
-                "endTime": {
-                    "documentation": "<p>The ending timestamp from the lifecycle action that was applied to the resource.</p>",
-                    "shape": "DateTimeTimestamp"
-                },
                 "imageUris": {
                     "documentation": "<p>For an impacted container image, this identifies a list of URIs for associated container images distributed to ECR repositories.</p>",
                     "shape": "StringList"
                 },
                 "region": {
                     "documentation": "<p>The Amazon Web Services Region where the lifecycle execution resource is stored.</p>",
                     "shape": "NonEmptyString"
@@ -6712,18 +6708,14 @@
                     "documentation": "<p>Identifies the impacted resource. The resource ID depends on the type of resource, as follows.</p> <ul> <li> <p>Image Builder image resources: Amazon Resource Name (ARN)</p> </li> <li> <p>Distributed AMIs: AMI ID</p> </li> <li> <p>Container images distributed to an ECR repository: image URI or SHA Digest</p> </li> </ul>",
                     "shape": "NonEmptyString"
                 },
                 "snapshots": {
                     "documentation": "<p>A list of associated resource snapshots for the impacted resource if it\u2019s an AMI.</p>",
                     "shape": "LifecycleExecutionSnapshotResourceList"
                 },
-                "startTime": {
-                    "documentation": "<p>The starting timestamp from the lifecycle action that was applied to the resource.</p>",
-                    "shape": "DateTimeTimestamp"
-                },
                 "state": {
                     "documentation": "<p>The runtime state for the lifecycle execution.</p>",
                     "shape": "LifecycleExecutionResourceState"
                 }
             },
             "type": "structure"
         },
@@ -6825,16 +6817,15 @@
         },
         "LifecycleExecutionStatus": {
             "enum": [
                 "IN_PROGRESS",
                 "CANCELLED",
                 "CANCELLING",
                 "FAILED",
-                "SUCCESS",
-                "PENDING"
+                "SUCCESS"
             ],
             "type": "string"
         },
         "LifecycleExecutionsList": {
             "member": {
                 "shape": "LifecycleExecution"
             },
@@ -6968,15 +6959,15 @@
             "documentation": "<p>Specifies resources that lifecycle policy actions should not apply to.</p>",
             "members": {
                 "amis": {
                     "documentation": "<p>Lists configuration values that apply to AMIs that Image Builder should exclude from the lifecycle action.</p>",
                     "shape": "LifecyclePolicyDetailExclusionRulesAmis"
                 },
                 "tagMap": {
-                    "documentation": "<p>Contains a list of tags that Image Builder uses to skip lifecycle actions for Image Builder image resources that have them.</p>",
+                    "documentation": "<p>Contains a list of tags that Image Builder uses to skip lifecycle actions for resources that have them.</p>",
                     "shape": "TagMap"
                 }
             },
             "type": "structure"
         },
         "LifecyclePolicyDetailExclusionRulesAmis": {
             "documentation": "<p>Defines criteria for AMIs that are excluded from lifecycle actions.</p>",
@@ -7082,15 +7073,15 @@
             "documentation": "<p>Resource selection criteria for the lifecycle policy.</p>",
             "members": {
                 "recipes": {
                     "documentation": "<p>A list of recipes that are used as selection criteria for the output images that the lifecycle policy applies to.</p>",
                     "shape": "LifecyclePolicyResourceSelectionRecipes"
                 },
                 "tagMap": {
-                    "documentation": "<p>A list of tags that are used as selection criteria for the Image Builder image resources that the lifecycle policy applies to.</p>",
+                    "documentation": "<p>A list of tags that are used as selection criteria for the resources that the lifecycle policy applies to.</p>",
                     "shape": "TagMap"
                 }
             },
             "type": "structure"
         },
         "LifecyclePolicyResourceSelectionRecipe": {
             "documentation": "<p>Specifies an Image Builder recipe that the lifecycle policy uses for resource selection.</p>",
```

### Comparing `botocore-a-la-carte-imagebuilder-1.34.87/botocore_a_la_carte_imagebuilder.egg-info/PKG-INFO` & `botocore-a-la-carte-imagebuilder-1.34.9/botocore_a_la_carte_imagebuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-imagebuilder
-Version: 1.34.87
+Version: 1.34.9
 Summary: imagebuilder data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-imagebuilder-1.34.87/setup.py` & `botocore-a-la-carte-imagebuilder-1.34.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-imagebuilder',
-    version="1.34.87",
+    version="1.34.9",
     description='imagebuilder data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/imagebuilder/*/*.json'],
```

