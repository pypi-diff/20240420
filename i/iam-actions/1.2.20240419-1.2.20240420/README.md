# Comparing `tmp/iam_actions-1.2.20240419.tar.gz` & `tmp/iam_actions-1.2.20240420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240419.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240420.tar", max compression
```

## Comparing `iam_actions-1.2.20240419.tar` & `iam_actions-1.2.20240420.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-19 02:19:05.225713 iam_actions-1.2.20240419/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-19 02:19:05.225713 iam_actions-1.2.20240419/README.md
--rw-r--r--   0        0        0      228 2024-04-19 02:19:05.225713 iam_actions-1.2.20240419/iam_actions/__init__.py
--rw-r--r--   0        0        0  4804186 2024-04-19 02:20:52.567164 iam_actions-1.2.20240419/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-19 02:19:05.225713 iam_actions-1.2.20240419/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-19 02:19:05.225713 iam_actions-1.2.20240419/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-19 02:19:05.225713 iam_actions-1.2.20240419/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-19 02:19:05.225713 iam_actions-1.2.20240419/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-19 02:19:05.225713 iam_actions-1.2.20240419/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-19 02:19:05.225713 iam_actions-1.2.20240419/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-19 02:19:05.225713 iam_actions-1.2.20240419/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-19 02:19:05.225713 iam_actions-1.2.20240419/iam_actions/generate/services.py
--rw-r--r--   0        0        0   624279 2024-04-19 02:20:52.567164 iam_actions-1.2.20240419/iam_actions/policies.json
--rw-r--r--   0        0        0   208291 2024-04-19 02:20:52.567164 iam_actions-1.2.20240419/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   605646 2024-04-19 02:20:52.567164 iam_actions-1.2.20240419/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-19 02:20:53.247172 iam_actions-1.2.20240419/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240419/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240419/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-20 02:15:23.085828 iam_actions-1.2.20240420/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-20 02:15:23.085828 iam_actions-1.2.20240420/README.md
+-rw-r--r--   0        0        0      228 2024-04-20 02:15:23.085828 iam_actions-1.2.20240420/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4805273 2024-04-20 02:17:14.646827 iam_actions-1.2.20240420/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-20 02:15:23.085828 iam_actions-1.2.20240420/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-20 02:15:23.085828 iam_actions-1.2.20240420/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-20 02:15:23.085828 iam_actions-1.2.20240420/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-20 02:15:23.085828 iam_actions-1.2.20240420/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-20 02:15:23.085828 iam_actions-1.2.20240420/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-20 02:15:23.085828 iam_actions-1.2.20240420/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-20 02:15:23.085828 iam_actions-1.2.20240420/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-20 02:15:23.085828 iam_actions-1.2.20240420/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   624345 2024-04-20 02:17:14.646827 iam_actions-1.2.20240420/iam_actions/policies.json
+-rw-r--r--   0        0        0   208291 2024-04-20 02:17:14.646827 iam_actions-1.2.20240420/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   605709 2024-04-20 02:17:14.646827 iam_actions-1.2.20240420/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-20 02:17:15.318833 iam_actions-1.2.20240420/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240420/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240420/PKG-INFO
```

### Comparing `iam_actions-1.2.20240419/LICENSE` & `iam_actions-1.2.20240420/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240419/README.md` & `iam_actions-1.2.20240420/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240419/iam_actions/actions.json` & `iam_actions-1.2.20240420/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999900412087912%*

 * *Differences: {"'appmesh'": "{'PutMeshPolicy': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *              "'PutMeshPolicy'), ('condition_keys', []), ('description', 'Not Documented by AWS'), "*

 * *              "('orphan', False), ('resources', [])]), 'GetMeshPolicy': "*

 * *              "OrderedDict([('access_level', 'Undocumented'), ('action', 'GetMeshPolicy'), "*

 * *              "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', "*

 * *              "False), ('resources', [])]), 'DeleteMeshPo […]*

```diff
@@ -5679,14 +5679,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete an existing service mesh",
             "orphan": false,
             "resources": [
                 "mesh"
             ]
         },
+        "DeleteMeshPolicy": {
+            "access_level": "Undocumented",
+            "action": "DeleteMeshPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteRoute": {
             "access_level": "Write",
             "action": "DeleteRoute",
             "condition_keys": [],
             "description": "Grants permission to delete an existing route",
             "orphan": false,
             "resources": [
@@ -5799,14 +5807,22 @@
             "condition_keys": [],
             "description": "Grants permission to describe an existing virtual service",
             "orphan": false,
             "resources": [
                 "virtualService"
             ]
         },
+        "GetMeshPolicy": {
+            "access_level": "Undocumented",
+            "action": "GetMeshPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListGatewayRoutes": {
             "access_level": "List",
             "action": "ListGatewayRoutes",
             "condition_keys": [],
             "description": "Grants permission to list existing gateway routes in a service mesh",
             "orphan": false,
             "resources": [
@@ -5883,14 +5899,22 @@
             "condition_keys": [],
             "description": "Grants permission to list existing virtual services in a service mesh",
             "orphan": false,
             "resources": [
                 "mesh"
             ]
         },
+        "PutMeshPolicy": {
+            "access_level": "Undocumented",
+            "action": "PutMeshPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StreamAggregatedResources": {
             "access_level": "Read",
             "action": "StreamAggregatedResources",
             "condition_keys": [],
             "description": "Grants permission to receive streamed resources for an App Mesh endpoint (VirtualNode/VirtualGateway)",
             "orphan": false,
             "resources": [
@@ -170615,18 +170639,18 @@
             "resources": [
                 "RawMessage"
             ]
         }
     },
     "workspaces": {
         "AcceptAccountLinkInvitation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AcceptAccountLinkInvitation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to accept invitations from other AWS accounts to share the same configuration for WorkSpaces BYOL",
             "orphan": false,
             "resources": []
         },
         "AssociateConnectionAlias": {
             "access_level": "Write",
             "action": "AssociateConnectionAlias",
             "condition_keys": [],
@@ -170681,18 +170705,18 @@
             "description": "Grants permission to copy a WorkSpace image",
             "orphan": false,
             "resources": [
                 "workspaceimage"
             ]
         },
         "CreateAccountLinkInvitation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateAccountLinkInvitation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to invite other AWS accounts to share the same configuration for WorkSpaces BYOL",
             "orphan": false,
             "resources": []
         },
         "CreateConnectClientAddIn": {
             "access_level": "Write",
             "action": "CreateConnectClientAddIn",
             "condition_keys": [],
@@ -170801,18 +170825,18 @@
             "resources": [
                 "directoryid",
                 "workspacebundle",
                 "workspaceid"
             ]
         },
         "DeleteAccountLinkInvitation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteAccountLinkInvitation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete invitations to other AWS accounts to share the same configuration for WorkSpaces BYOL",
             "orphan": false,
             "resources": []
         },
         "DeleteClientBranding": {
             "access_level": "Write",
             "action": "DeleteClientBranding",
             "condition_keys": [],
@@ -171134,18 +171158,18 @@
             "orphan": false,
             "resources": [
                 "workspaceapplication",
                 "workspaceid"
             ]
         },
         "GetAccountLink": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetAccountLink",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve a link with another AWS Account for sharing configuration for WorkSpaces BYOL",
             "orphan": false,
             "resources": []
         },
         "ImportClientBranding": {
             "access_level": "Write",
             "action": "ImportClientBranding",
             "condition_keys": [],
@@ -171160,18 +171184,18 @@
             "action": "ImportWorkspaceImage",
             "condition_keys": [],
             "description": "Grants permission to import Bring Your Own License (BYOL) images into Amazon WorkSpaces",
             "orphan": false,
             "resources": []
         },
         "ListAccountLinks": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListAccountLinks",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve links with the AWS Account(s) that share your configuration for WorkSpaces BYOL",
             "orphan": false,
             "resources": []
         },
         "ListAvailableManagementCidrRanges": {
             "access_level": "List",
             "action": "ListAvailableManagementCidrRanges",
             "condition_keys": [],
@@ -171308,18 +171332,18 @@
             "description": "Grants permission to register directories for use with Amazon WorkSpaces",
             "orphan": false,
             "resources": [
                 "directoryid"
             ]
         },
         "RejectAccountLinkInvitation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RejectAccountLinkInvitation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to reject invitations from other AWS accounts to share the same configuration for WorkSpaces BYOL",
             "orphan": false,
             "resources": []
         },
         "RestoreWorkspace": {
             "access_level": "Write",
             "action": "RestoreWorkspace",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20240419/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240420/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240419/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240420/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240419/iam_actions/generate/generate.py` & `iam_actions-1.2.20240420/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240419/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240420/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240419/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240420/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240419/iam_actions/generate/services.py` & `iam_actions-1.2.20240420/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240419/iam_actions/policies.json` & `iam_actions-1.2.20240420/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999992705415499%*

 * *Differences: {"'serviceMap'": "{'AWS App Mesh': {'Actions': {insert: [(9, 'DeleteMeshPolicy'), (22, "*

 * *                 "'GetMeshPolicy'), (31, 'PutMeshPolicy')]}}}"}*

```diff
@@ -336,34 +336,37 @@
                 "CreateRoute",
                 "CreateVirtualGateway",
                 "CreateVirtualNode",
                 "CreateVirtualRouter",
                 "CreateVirtualService",
                 "DeleteGatewayRoute",
                 "DeleteMesh",
+                "DeleteMeshPolicy",
                 "DeleteRoute",
                 "DeleteVirtualGateway",
                 "DeleteVirtualNode",
                 "DeleteVirtualRouter",
                 "DeleteVirtualService",
                 "DescribeGatewayRoute",
                 "DescribeMesh",
                 "DescribeRoute",
                 "DescribeVirtualGateway",
                 "DescribeVirtualNode",
                 "DescribeVirtualRouter",
                 "DescribeVirtualService",
+                "GetMeshPolicy",
                 "ListGatewayRoutes",
                 "ListMeshes",
                 "ListRoutes",
                 "ListTagsForResource",
                 "ListVirtualGateways",
                 "ListVirtualNodes",
                 "ListVirtualRouters",
                 "ListVirtualServices",
+                "PutMeshPolicy",
                 "StreamAggregatedResources",
                 "TagResource",
                 "UntagResource",
                 "UpdateGatewayRoute",
                 "UpdateMesh",
                 "UpdateRoute",
                 "UpdateVirtualGateway",
```

### Comparing `iam_actions-1.2.20240419/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240420/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240419/iam_actions/services.json` & `iam_actions-1.2.20240420/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999923687423687%*

 * *Differences: {"'appmesh'": "{'Actions': {insert: [(9, 'DeleteMeshPolicy'), (22, 'GetMeshPolicy'), (31, "*

 * *              "'PutMeshPolicy')]}}"}*

```diff
@@ -973,34 +973,37 @@
             "CreateRoute",
             "CreateVirtualGateway",
             "CreateVirtualNode",
             "CreateVirtualRouter",
             "CreateVirtualService",
             "DeleteGatewayRoute",
             "DeleteMesh",
+            "DeleteMeshPolicy",
             "DeleteRoute",
             "DeleteVirtualGateway",
             "DeleteVirtualNode",
             "DeleteVirtualRouter",
             "DeleteVirtualService",
             "DescribeGatewayRoute",
             "DescribeMesh",
             "DescribeRoute",
             "DescribeVirtualGateway",
             "DescribeVirtualNode",
             "DescribeVirtualRouter",
             "DescribeVirtualService",
+            "GetMeshPolicy",
             "ListGatewayRoutes",
             "ListMeshes",
             "ListRoutes",
             "ListTagsForResource",
             "ListVirtualGateways",
             "ListVirtualNodes",
             "ListVirtualRouters",
             "ListVirtualServices",
+            "PutMeshPolicy",
             "StreamAggregatedResources",
             "TagResource",
             "UntagResource",
             "UpdateGatewayRoute",
             "UpdateMesh",
             "UpdateRoute",
             "UpdateVirtualGateway",
```

### Comparing `iam_actions-1.2.20240419/pyproject.toml` & `iam_actions-1.2.20240420/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240419"
+version = "1.2.20240420"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240419/setup.py` & `iam_actions-1.2.20240420/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240419',
+    'version': '1.2.20240420',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240419/PKG-INFO` & `iam_actions-1.2.20240420/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240419
+Version: 1.2.20240420
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

