# Comparing `tmp/botocore-a-la-carte-cloud9-1.34.87.tar.gz` & `tmp/botocore-a-la-carte-cloud9-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-cloud9-1.34.87.tar", last modified: Fri Apr 19 01:00:42 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-cloud9-1.34.9.tar", last modified: Thu Dec 28 01:06:34 2023, max compression
```

## Comparing `botocore-a-la-carte-cloud9-1.34.87.tar` & `botocore-a-la-carte-cloud9-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:42.668550 botocore-a-la-carte-cloud9-1.34.87/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-19 01:00:42.000000 botocore-a-la-carte-cloud9-1.34.87/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-19 01:00:42.668550 botocore-a-la-carte-cloud9-1.34.87/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:42.664550 botocore-a-la-carte-cloud9-1.34.87/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:42.664550 botocore-a-la-carte-cloud9-1.34.87/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:42.664550 botocore-a-la-carte-cloud9-1.34.87/botocore/data/cloud9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:42.664550 botocore-a-la-carte-cloud9-1.34.87/botocore/data/cloud9/2017-09-23/
--rw-r--r--   0 runner    (1001) docker     (127)    13726 2024-04-19 01:00:35.000000 botocore-a-la-carte-cloud9-1.34.87/botocore/data/cloud9/2017-09-23/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-19 01:00:35.000000 botocore-a-la-carte-cloud9-1.34.87/botocore/data/cloud9/2017-09-23/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-19 01:00:35.000000 botocore-a-la-carte-cloud9-1.34.87/botocore/data/cloud9/2017-09-23/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    39834 2024-04-19 01:00:35.000000 botocore-a-la-carte-cloud9-1.34.87/botocore/data/cloud9/2017-09-23/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:42.664550 botocore-a-la-carte-cloud9-1.34.87/botocore_a_la_carte_cloud9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-19 01:00:42.000000 botocore-a-la-carte-cloud9-1.34.87/botocore_a_la_carte_cloud9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-19 01:00:42.000000 botocore-a-la-carte-cloud9-1.34.87/botocore_a_la_carte_cloud9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:00:42.000000 botocore-a-la-carte-cloud9-1.34.87/botocore_a_la_carte_cloud9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 01:00:42.000000 botocore-a-la-carte-cloud9-1.34.87/botocore_a_la_carte_cloud9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:00:42.668550 botocore-a-la-carte-cloud9-1.34.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-19 01:00:42.000000 botocore-a-la-carte-cloud9-1.34.87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:34.894226 botocore-a-la-carte-cloud9-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:34.000000 botocore-a-la-carte-cloud9-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2023-12-28 01:06:34.890226 botocore-a-la-carte-cloud9-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:34.890226 botocore-a-la-carte-cloud9-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:34.890226 botocore-a-la-carte-cloud9-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:34.890226 botocore-a-la-carte-cloud9-1.34.9/botocore/data/cloud9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:34.890226 botocore-a-la-carte-cloud9-1.34.9/botocore/data/cloud9/2017-09-23/
+-rw-r--r--   0 runner    (1001) docker     (127)    13726 2023-12-28 01:06:26.000000 botocore-a-la-carte-cloud9-1.34.9/botocore/data/cloud9/2017-09-23/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2023-12-28 01:06:26.000000 botocore-a-la-carte-cloud9-1.34.9/botocore/data/cloud9/2017-09-23/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-28 01:06:26.000000 botocore-a-la-carte-cloud9-1.34.9/botocore/data/cloud9/2017-09-23/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40334 2023-12-28 01:06:26.000000 botocore-a-la-carte-cloud9-1.34.9/botocore/data/cloud9/2017-09-23/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:34.890226 botocore-a-la-carte-cloud9-1.34.9/botocore_a_la_carte_cloud9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2023-12-28 01:06:34.000000 botocore-a-la-carte-cloud9-1.34.9/botocore_a_la_carte_cloud9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2023-12-28 01:06:34.000000 botocore-a-la-carte-cloud9-1.34.9/botocore_a_la_carte_cloud9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:34.000000 botocore-a-la-carte-cloud9-1.34.9/botocore_a_la_carte_cloud9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:34.000000 botocore-a-la-carte-cloud9-1.34.9/botocore_a_la_carte_cloud9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:34.894226 botocore-a-la-carte-cloud9-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-12-28 01:06:34.000000 botocore-a-la-carte-cloud9-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-cloud9-1.34.87/LICENSE.txt` & `botocore-a-la-carte-cloud9-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloud9-1.34.87/PKG-INFO` & `botocore-a-la-carte-cloud9-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-cloud9
-Version: 1.34.87
+Version: 1.34.9
 Summary: cloud9 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-cloud9-1.34.87/botocore/data/cloud9/2017-09-23/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloud9-1.34.9/botocore/data/cloud9/2017-09-23/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloud9-1.34.87/botocore/data/cloud9/2017-09-23/examples-1.json` & `botocore-a-la-carte-cloud9-1.34.9/botocore/data/cloud9/2017-09-23/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloud9-1.34.87/botocore/data/cloud9/2017-09-23/service-2.json` & `botocore-a-la-carte-cloud9-1.34.9/botocore/data/cloud9/2017-09-23/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999986275801493%*

 * *Differences: {"'shapes'": "{'CreateEnvironmentEC2Request': {'members': {'imageId': {'documentation': "*

 * *             '"<p>The identifier for the Amazon Machine Image (AMI) that\'s used to create the EC2 '*

 * *             'instance. To choose an AMI for the instance, you must specify a valid AMI alias or a '*

 * *             'valid Amazon EC2 Systems Manager (SSM) path.</p> <p>From December 04, 2023, you will '*

 * *             'be required to include the <code>imageId</code> parameter for the '*

 * *             '<code>CreateEnvironment […]*

```diff
@@ -533,15 +533,15 @@
                     "shape": "EnvironmentDescription"
                 },
                 "dryRun": {
                     "documentation": "<p>Checks whether you have the required permissions for the action, without actually making the request, and provides an error response. If you have the required permissions, the error response is <code>DryRunOperation</code>. Otherwise, it is <code>UnauthorizedOperation</code>.</p>",
                     "shape": "NullableBoolean"
                 },
                 "imageId": {
-                    "documentation": "<p>The identifier for the Amazon Machine Image (AMI) that's used to create the EC2 instance. To choose an AMI for the instance, you must specify a valid AMI alias or a valid Amazon EC2 Systems Manager (SSM) path.</p> <p>From December 04, 2023, you will be required to include the <code>imageId</code> parameter for the <code>CreateEnvironmentEC2</code> action. This change will be reflected across all direct methods of communicating with the API, such as Amazon Web Services SDK, Amazon Web Services CLI and Amazon Web Services CloudFormation. This change will only affect direct API consumers, and not Cloud9 console users.</p> <p>We recommend using Amazon Linux 2023 as the AMI to create your environment as it is fully supported. </p> <p>Since Ubuntu 18.04 has ended standard support as of May 31, 2023, we recommend you choose Ubuntu 22.04.</p> <p> <b>AMI aliases </b> </p> <ul> <li> <p>Amazon Linux 2: <code>amazonlinux-2-x86_64</code> </p> </li> <li> <p>Amazon Linux 2023 (recommended): <code>amazonlinux-2023-x86_64</code> </p> </li> <li> <p>Ubuntu 18.04: <code>ubuntu-18.04-x86_64</code> </p> </li> <li> <p>Ubuntu 22.04: <code>ubuntu-22.04-x86_64</code> </p> </li> </ul> <p> <b>SSM paths</b> </p> <ul> <li> <p>Amazon Linux 2: <code>resolve:ssm:/aws/service/cloud9/amis/amazonlinux-2-x86_64</code> </p> </li> <li> <p>Amazon Linux 2023 (recommended): <code>resolve:ssm:/aws/service/cloud9/amis/amazonlinux-2023-x86_64</code> </p> </li> <li> <p>Ubuntu 18.04: <code>resolve:ssm:/aws/service/cloud9/amis/ubuntu-18.04-x86_64</code> </p> </li> <li> <p>Ubuntu 22.04: <code>resolve:ssm:/aws/service/cloud9/amis/ubuntu-22.04-x86_64</code> </p> </li> </ul>",
+                    "documentation": "<p>The identifier for the Amazon Machine Image (AMI) that's used to create the EC2 instance. To choose an AMI for the instance, you must specify a valid AMI alias or a valid Amazon EC2 Systems Manager (SSM) path.</p> <p>From December 04, 2023, you will be required to include the <code>imageId</code> parameter for the <code>CreateEnvironmentEC2</code> action. This change will be reflected across all direct methods of communicating with the API, such as Amazon Web Services SDK, Amazon Web Services CLI and Amazon Web Services CloudFormation. This change will only affect direct API consumers, and not Cloud9 console users.</p> <p>From January 22, 2024, Amazon Linux (AL1) will be removed from the list of available image IDs for Cloud9. This is necessary as AL1 will reach the end of maintenance support in December 2023, and as a result will no longer receive security updates. We recommend using Amazon Linux 2023 as the AMI to create your environment as it is fully supported. This change will only affect direct API consumers, and not Cloud9 console users.</p> <p>Since Ubuntu 18.04 has ended standard support as of May 31, 2023, we recommend you choose Ubuntu 22.04.</p> <p> <b>AMI aliases </b> </p> <ul> <li> <p>Amazon Linux: <code>amazonlinux-1-x86_64</code> </p> </li> <li> <p>Amazon Linux 2: <code>amazonlinux-2-x86_64</code> </p> </li> <li> <p>Amazon Linux 2023 (recommended): <code>amazonlinux-2023-x86_64</code> </p> </li> <li> <p>Ubuntu 18.04: <code>ubuntu-18.04-x86_64</code> </p> </li> <li> <p>Ubuntu 22.04: <code>ubuntu-22.04-x86_64</code> </p> </li> </ul> <p> <b>SSM paths</b> </p> <ul> <li> <p>Amazon Linux: <code>resolve:ssm:/aws/service/cloud9/amis/amazonlinux-1-x86_64</code> </p> </li> <li> <p>Amazon Linux 2: <code>resolve:ssm:/aws/service/cloud9/amis/amazonlinux-2-x86_64</code> </p> </li> <li> <p>Amazon Linux 2023 (recommended): <code>resolve:ssm:/aws/service/cloud9/amis/amazonlinux-2023-x86_64</code> </p> </li> <li> <p>Ubuntu 18.04: <code>resolve:ssm:/aws/service/cloud9/amis/ubuntu-18.04-x86_64</code> </p> </li> <li> <p>Ubuntu 22.04: <code>resolve:ssm:/aws/service/cloud9/amis/ubuntu-22.04-x86_64</code> </p> </li> </ul>",
                     "shape": "ImageId"
                 },
                 "instanceType": {
                     "documentation": "<p>The type of instance to connect to the environment (for example, <code>t2.micro</code>).</p>",
                     "shape": "InstanceType"
                 },
                 "name": {
```

### Comparing `botocore-a-la-carte-cloud9-1.34.87/botocore_a_la_carte_cloud9.egg-info/PKG-INFO` & `botocore-a-la-carte-cloud9-1.34.9/botocore_a_la_carte_cloud9.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-cloud9
-Version: 1.34.87
+Version: 1.34.9
 Summary: cloud9 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-cloud9-1.34.87/setup.py` & `botocore-a-la-carte-cloud9-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-cloud9',
-    version="1.34.87",
+    version="1.34.9",
     description='cloud9 data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/cloud9/*/*.json'],
```

