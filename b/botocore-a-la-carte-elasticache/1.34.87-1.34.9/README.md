# Comparing `tmp/botocore-a-la-carte-elasticache-1.34.87.tar.gz` & `tmp/botocore-a-la-carte-elasticache-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-elasticache-1.34.87.tar", last modified: Fri Apr 19 01:00:51 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-elasticache-1.34.9.tar", last modified: Thu Dec 28 01:06:42 2023, max compression
```

## Comparing `botocore-a-la-carte-elasticache-1.34.87.tar` & `botocore-a-la-carte-elasticache-1.34.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:51.540586 botocore-a-la-carte-elasticache-1.34.87/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-19 01:00:51.000000 botocore-a-la-carte-elasticache-1.34.87/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-19 01:00:51.540586 botocore-a-la-carte-elasticache-1.34.87/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:51.536586 botocore-a-la-carte-elasticache-1.34.87/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:51.536586 botocore-a-la-carte-elasticache-1.34.87/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:51.536586 botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:51.540586 botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2014-09-30/
--rw-r--r--   0 runner    (1001) docker     (127)    14735 2024-04-19 01:00:35.000000 botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2014-09-30/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-19 01:00:35.000000 botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2014-09-30/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   223047 2024-04-19 01:00:35.000000 botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2014-09-30/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-19 01:00:35.000000 botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2014-09-30/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:51.540586 botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2015-02-02/
--rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-04-19 01:00:35.000000 botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2015-02-02/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   111590 2024-04-19 01:00:35.000000 botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2015-02-02/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-19 01:00:35.000000 botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2015-02-02/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   427316 2024-04-19 01:00:35.000000 botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2015-02-02/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-04-19 01:00:35.000000 botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2015-02-02/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:00:51.540586 botocore-a-la-carte-elasticache-1.34.87/botocore_a_la_carte_elasticache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-19 01:00:51.000000 botocore-a-la-carte-elasticache-1.34.87/botocore_a_la_carte_elasticache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-19 01:00:51.000000 botocore-a-la-carte-elasticache-1.34.87/botocore_a_la_carte_elasticache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:00:51.000000 botocore-a-la-carte-elasticache-1.34.87/botocore_a_la_carte_elasticache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 01:00:51.000000 botocore-a-la-carte-elasticache-1.34.87/botocore_a_la_carte_elasticache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:00:51.540586 botocore-a-la-carte-elasticache-1.34.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-19 01:00:51.000000 botocore-a-la-carte-elasticache-1.34.87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:42.126282 botocore-a-la-carte-elasticache-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:41.000000 botocore-a-la-carte-elasticache-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-28 01:06:42.126282 botocore-a-la-carte-elasticache-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:42.122282 botocore-a-la-carte-elasticache-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:42.122282 botocore-a-la-carte-elasticache-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:42.122282 botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:42.126282 botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2014-09-30/
+-rw-r--r--   0 runner    (1001) docker     (127)    14735 2023-12-28 01:06:26.000000 botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2014-09-30/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2023-12-28 01:06:26.000000 botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2014-09-30/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   223047 2023-12-28 01:06:26.000000 botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2014-09-30/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2023-12-28 01:06:26.000000 botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2014-09-30/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:42.126282 botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2015-02-02/
+-rw-r--r--   0 runner    (1001) docker     (127)    15317 2023-12-28 01:06:26.000000 botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2015-02-02/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   111590 2023-12-28 01:06:26.000000 botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2015-02-02/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2023-12-28 01:06:26.000000 botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2015-02-02/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   427240 2023-12-28 01:06:26.000000 botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2015-02-02/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2023-12-28 01:06:26.000000 botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2015-02-02/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:42.126282 botocore-a-la-carte-elasticache-1.34.9/botocore_a_la_carte_elasticache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-28 01:06:42.000000 botocore-a-la-carte-elasticache-1.34.9/botocore_a_la_carte_elasticache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2023-12-28 01:06:42.000000 botocore-a-la-carte-elasticache-1.34.9/botocore_a_la_carte_elasticache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:42.000000 botocore-a-la-carte-elasticache-1.34.9/botocore_a_la_carte_elasticache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:42.000000 botocore-a-la-carte-elasticache-1.34.9/botocore_a_la_carte_elasticache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:42.126282 botocore-a-la-carte-elasticache-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2023-12-28 01:06:41.000000 botocore-a-la-carte-elasticache-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-elasticache-1.34.87/LICENSE.txt` & `botocore-a-la-carte-elasticache-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-elasticache-1.34.87/PKG-INFO` & `botocore-a-la-carte-elasticache-1.34.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-elasticache
-Version: 1.34.87
+Version: 1.34.9
 Summary: elasticache data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2014-09-30/endpoint-rule-set-1.json` & `botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2014-09-30/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2014-09-30/paginators-1.json` & `botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2014-09-30/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2014-09-30/service-2.json` & `botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2014-09-30/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2014-09-30/waiters-2.json` & `botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2014-09-30/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2015-02-02/endpoint-rule-set-1.json` & `botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2015-02-02/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2015-02-02/examples-1.json` & `botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2015-02-02/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2015-02-02/paginators-1.json` & `botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2015-02-02/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2015-02-02/service-2.json` & `botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2015-02-02/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998717985571879%*

 * *Differences: {"'operations'": "{'CreateReplicationGroup': {'documentation': '<p>Creates a Redis (cluster mode "*

 * *                 'disabled) or a Redis (cluster mode enabled) replication group.</p> <p>This API '*

 * *                 'can be used to create a standalone regional replication group or a secondary '*

 * *                 'replication group associated with a Global datastore.</p> <p>A Redis (cluster '*

 * *                 'mode disabled) replication group is a collection of clusters, where one of the '*

 * *                 'cl […]*

```diff
@@ -449,15 +449,15 @@
             "name": "CreateGlobalReplicationGroup",
             "output": {
                 "resultWrapper": "CreateGlobalReplicationGroupResult",
                 "shape": "CreateGlobalReplicationGroupResult"
             }
         },
         "CreateReplicationGroup": {
-            "documentation": "<p>Creates a Redis (cluster mode disabled) or a Redis (cluster mode enabled) replication group.</p> <p>This API can be used to create a standalone regional replication group or a secondary replication group associated with a Global datastore.</p> <p>A Redis (cluster mode disabled) replication group is a collection of nodes, where one of the nodes is a read/write primary and the others are read-only replicas. Writes to the primary are asynchronously propagated to the replicas.</p> <p>A Redis cluster-mode enabled cluster is comprised of from 1 to 90 shards (API/CLI: node groups). Each shard has a primary node and up to 5 read-only replica nodes. The configuration can range from 90 shards and 0 replicas to 15 shards and 5 replicas, which is the maximum number or replicas allowed. </p> <p>The node or shard limit can be increased to a maximum of 500 per cluster if the Redis engine version is 5.0.6 or higher. For example, you can choose to configure a 500 node cluster that ranges between 83 shards (one primary and 5 replicas per shard) and 500 shards (single primary and no replicas). Make sure there are enough available IP addresses to accommodate the increase. Common pitfalls include the subnets in the subnet group have too small a CIDR range or the subnets are shared and heavily used by other clusters. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonElastiCache/latest/red-ug/SubnetGroups.Creating.html\">Creating a Subnet Group</a>. For versions below 5.0.6, the limit is 250 per cluster.</p> <p>To request a limit increase, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_service_limits.html\">Amazon Service Limits</a> and choose the limit type <b>Nodes per cluster per instance type</b>. </p> <p>When a Redis (cluster mode disabled) replication group has been successfully created, you can add one or more read replicas to it, up to a total of 5 read replicas. If you need to increase or decrease the number of node groups (console: shards), you can avail yourself of ElastiCache for Redis' scaling. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonElastiCache/latest/red-ug/Scaling.html\">Scaling ElastiCache for Redis Clusters</a> in the <i>ElastiCache User Guide</i>.</p> <note> <p>This operation is valid for Redis only.</p> </note>",
+            "documentation": "<p>Creates a Redis (cluster mode disabled) or a Redis (cluster mode enabled) replication group.</p> <p>This API can be used to create a standalone regional replication group or a secondary replication group associated with a Global datastore.</p> <p>A Redis (cluster mode disabled) replication group is a collection of clusters, where one of the clusters is a read/write primary and the others are read-only replicas. Writes to the primary are asynchronously propagated to the replicas.</p> <p>A Redis cluster-mode enabled cluster is comprised of from 1 to 90 shards (API/CLI: node groups). Each shard has a primary node and up to 5 read-only replica nodes. The configuration can range from 90 shards and 0 replicas to 15 shards and 5 replicas, which is the maximum number or replicas allowed. </p> <p>The node or shard limit can be increased to a maximum of 500 per cluster if the Redis engine version is 5.0.6 or higher. For example, you can choose to configure a 500 node cluster that ranges between 83 shards (one primary and 5 replicas per shard) and 500 shards (single primary and no replicas). Make sure there are enough available IP addresses to accommodate the increase. Common pitfalls include the subnets in the subnet group have too small a CIDR range or the subnets are shared and heavily used by other clusters. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonElastiCache/latest/red-ug/SubnetGroups.Creating.html\">Creating a Subnet Group</a>. For versions below 5.0.6, the limit is 250 per cluster.</p> <p>To request a limit increase, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_service_limits.html\">Amazon Service Limits</a> and choose the limit type <b>Nodes per cluster per instance type</b>. </p> <p>When a Redis (cluster mode disabled) replication group has been successfully created, you can add one or more read replicas to it, up to a total of 5 read replicas. If you need to increase or decrease the number of node groups (console: shards), you can avail yourself of ElastiCache for Redis' scaling. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonElastiCache/latest/red-ug/Scaling.html\">Scaling ElastiCache for Redis Clusters</a> in the <i>ElastiCache User Guide</i>.</p> <note> <p>This operation is valid for Redis only.</p> </note>",
             "errors": [
                 {
                     "shape": "CacheClusterNotFoundFault"
                 },
                 {
                     "shape": "InvalidCacheClusterStateFault"
                 },
@@ -4092,15 +4092,15 @@
                     "shape": "IntegerOptional"
                 },
                 "PreferredCacheClusterAZs": {
                     "documentation": "<p>A list of EC2 Availability Zones in which the replication group's clusters are created. The order of the Availability Zones in the list is the order in which clusters are allocated. The primary cluster is created in the first AZ in the list.</p> <p>This parameter is not used if there is more than one node group (shard). You should use <code>NodeGroupConfiguration</code> instead.</p> <note> <p>If you are creating your replication group in an Amazon VPC (recommended), you can only locate clusters in Availability Zones associated with the subnets in the selected subnet group.</p> <p>The number of Availability Zones listed must equal the value of <code>NumCacheClusters</code>.</p> </note> <p>Default: system chosen Availability Zones.</p>",
                     "shape": "AvailabilityZonesList"
                 },
                 "PreferredMaintenanceWindow": {
-                    "documentation": "<p>Specifies the weekly time range during which maintenance on the cluster is performed. It is specified as a range in the format ddd:hh24:mi-ddd:hh24:mi (24H Clock UTC). The minimum maintenance window is a 60 minute period.</p> <p>Valid values for <code>ddd</code> are:</p> <ul> <li> <p> <code>sun</code> </p> </li> <li> <p> <code>mon</code> </p> </li> <li> <p> <code>tue</code> </p> </li> <li> <p> <code>wed</code> </p> </li> <li> <p> <code>thu</code> </p> </li> <li> <p> <code>fri</code> </p> </li> <li> <p> <code>sat</code> </p> </li> </ul> <p>Example: <code>sun:23:00-mon:01:30</code> </p>",
+                    "documentation": "<p>Specifies the weekly time range during which maintenance on the cluster is performed. It is specified as a range in the format ddd:hh24:mi-ddd:hh24:mi (24H Clock UTC). The minimum maintenance window is a 60 minute period. Valid values for <code>ddd</code> are:</p> <p>Specifies the weekly time range during which maintenance on the cluster is performed. It is specified as a range in the format ddd:hh24:mi-ddd:hh24:mi (24H Clock UTC). The minimum maintenance window is a 60 minute period.</p> <p>Valid values for <code>ddd</code> are:</p> <ul> <li> <p> <code>sun</code> </p> </li> <li> <p> <code>mon</code> </p> </li> <li> <p> <code>tue</code> </p> </li> <li> <p> <code>wed</code> </p> </li> <li> <p> <code>thu</code> </p> </li> <li> <p> <code>fri</code> </p> </li> <li> <p> <code>sat</code> </p> </li> </ul> <p>Example: <code>sun:23:00-mon:01:30</code> </p>",
                     "shape": "String"
                 },
                 "PrimaryClusterId": {
                     "documentation": "<p>The identifier of the cluster that serves as the primary for this replication group. This cluster must already exist and have a status of <code>available</code>.</p> <p>This parameter is not required if <code>NumCacheClusters</code>, <code>NumNodeGroups</code>, or <code>ReplicasPerNodeGroup</code> is specified.</p>",
                     "shape": "String"
                 },
                 "ReplicasPerNodeGroup": {
@@ -4402,24 +4402,21 @@
         "DataStorage": {
             "documentation": "<p>The data storage limit.</p>",
             "members": {
                 "Maximum": {
                     "documentation": "<p>The upper limit for data storage the cache is set to use.</p>",
                     "shape": "IntegerOptional"
                 },
-                "Minimum": {
-                    "documentation": "<p>The lower limit for data storage the cache is set to use.</p>",
-                    "shape": "IntegerOptional"
-                },
                 "Unit": {
                     "documentation": "<p>The unit that the storage is measured in, in GB.</p>",
                     "shape": "DataStorageUnit"
                 }
             },
             "required": [
+                "Maximum",
                 "Unit"
             ],
             "type": "structure"
         },
         "DataStorageUnit": {
             "enum": [
                 "GB"
@@ -5403,24 +5400,23 @@
         },
         "ECPUPerSecond": {
             "documentation": "<p>The configuration for the number of ElastiCache Processing Units (ECPU) the cache can consume per second.</p>",
             "members": {
                 "Maximum": {
                     "documentation": "<p>The configuration for the maximum number of ECPUs the cache can consume per second.</p>",
                     "shape": "IntegerOptional"
-                },
-                "Minimum": {
-                    "documentation": "<p>The configuration for the minimum number of ECPUs the cache should be able consume per second.</p>",
-                    "shape": "IntegerOptional"
                 }
             },
+            "required": [
+                "Maximum"
+            ],
             "type": "structure"
         },
         "Endpoint": {
-            "documentation": "<p>Represents the information required for client programs to connect to a cache node. This value is read-only.</p>",
+            "documentation": "<p>Represents the information required for client programs to connect to a cache node.</p>",
             "members": {
                 "Address": {
                     "documentation": "<p>The DNS hostname of the cache node.</p>",
                     "shape": "String"
                 },
                 "Port": {
                     "documentation": "<p>The port number that the cache engine is listening on.</p>",
@@ -6708,15 +6704,15 @@
                     "shape": "NodeGroupMemberList"
                 },
                 "PrimaryEndpoint": {
                     "documentation": "<p>The endpoint of the primary node in this node group (shard).</p>",
                     "shape": "Endpoint"
                 },
                 "ReaderEndpoint": {
-                    "documentation": "<p>The endpoint of the replica nodes in this node group (shard). This value is read-only.</p>",
+                    "documentation": "<p>The endpoint of the replica nodes in this node group (shard).</p>",
                     "shape": "Endpoint"
                 },
                 "Slots": {
                     "documentation": "<p>The keyspace for this node group (shard).</p>",
                     "shape": "String"
                 },
                 "Status": {
@@ -7998,15 +7994,15 @@
                     "shape": "IntegerOptional"
                 },
                 "Status": {
                     "documentation": "<p>The current status of the serverless cache. The allowed values are CREATING, AVAILABLE, DELETING, CREATE-FAILED and MODIFYING.</p>",
                     "shape": "String"
                 },
                 "SubnetIds": {
-                    "documentation": "<p>If no subnet IDs are given and your VPC is in us-west-1, then ElastiCache will select 2 default subnets across AZs in your VPC. For all other Regions, if no subnet IDs are given then ElastiCache will select 3 default subnets across AZs in your default VPC.</p>",
+                    "documentation": "<p>If no subnet IDs are given and your VPC is in SFO, then ElastiCache will select 2 default subnets across AZs in your VPC. For all other Regions, if no subnet IDs are given then ElastiCache will select 3 default subnets across AZs in your default VPC.</p>",
                     "shape": "SubnetIdsList"
                 },
                 "UserGroupId": {
                     "documentation": "<p>The identifier of the user group associated with the serverless cache. Available for Redis only. Default is NULL.</p>",
                     "shape": "String"
                 }
             },
```

### Comparing `botocore-a-la-carte-elasticache-1.34.87/botocore/data/elasticache/2015-02-02/waiters-2.json` & `botocore-a-la-carte-elasticache-1.34.9/botocore/data/elasticache/2015-02-02/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-elasticache-1.34.87/botocore_a_la_carte_elasticache.egg-info/PKG-INFO` & `botocore-a-la-carte-elasticache-1.34.9/botocore_a_la_carte_elasticache.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-elasticache
-Version: 1.34.87
+Version: 1.34.9
 Summary: elasticache data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-elasticache-1.34.87/botocore_a_la_carte_elasticache.egg-info/SOURCES.txt` & `botocore-a-la-carte-elasticache-1.34.9/botocore_a_la_carte_elasticache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-elasticache-1.34.87/setup.py` & `botocore-a-la-carte-elasticache-1.34.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-elasticache',
-    version="1.34.87",
+    version="1.34.9",
     description='elasticache data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/elasticache/*/*.json'],
```

