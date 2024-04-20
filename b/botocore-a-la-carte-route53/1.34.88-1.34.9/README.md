# Comparing `tmp/botocore-a-la-carte-route53-1.34.88.tar.gz` & `tmp/botocore-a-la-carte-route53-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-route53-1.34.88.tar", last modified: Sat Apr 20 01:01:14 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-route53-1.34.9.tar", last modified: Thu Dec 28 01:07:01 2023, max compression
```

## Comparing `botocore-a-la-carte-route53-1.34.88.tar` & `botocore-a-la-carte-route53-1.34.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:01:14.203432 botocore-a-la-carte-route53-1.34.88/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-20 01:01:13.000000 botocore-a-la-carte-route53-1.34.88/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-20 01:01:14.203432 botocore-a-la-carte-route53-1.34.88/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:01:14.203432 botocore-a-la-carte-route53-1.34.88/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:01:14.203432 botocore-a-la-carte-route53-1.34.88/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:01:14.203432 botocore-a-la-carte-route53-1.34.88/botocore/data/route53/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:01:14.203432 botocore-a-la-carte-route53-1.34.88/botocore/data/route53/2013-04-01/
--rw-r--r--   0 runner    (1001) docker     (127)    35205 2024-04-20 01:00:41.000000 botocore-a-la-carte-route53-1.34.88/botocore/data/route53/2013-04-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    29631 2024-04-20 01:00:41.000000 botocore-a-la-carte-route53-1.34.88/botocore/data/route53/2013-04-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-20 01:00:41.000000 botocore-a-la-carte-route53-1.34.88/botocore/data/route53/2013-04-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   413898 2024-04-20 01:00:41.000000 botocore-a-la-carte-route53-1.34.88/botocore/data/route53/2013-04-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-20 01:00:41.000000 botocore-a-la-carte-route53-1.34.88/botocore/data/route53/2013-04-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:01:14.203432 botocore-a-la-carte-route53-1.34.88/botocore_a_la_carte_route53.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-20 01:01:14.000000 botocore-a-la-carte-route53-1.34.88/botocore_a_la_carte_route53.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-20 01:01:14.000000 botocore-a-la-carte-route53-1.34.88/botocore_a_la_carte_route53.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:01:14.000000 botocore-a-la-carte-route53-1.34.88/botocore_a_la_carte_route53.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 01:01:14.000000 botocore-a-la-carte-route53-1.34.88/botocore_a_la_carte_route53.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:01:14.203432 botocore-a-la-carte-route53-1.34.88/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-20 01:01:13.000000 botocore-a-la-carte-route53-1.34.88/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:01.014431 botocore-a-la-carte-route53-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:07:00.000000 botocore-a-la-carte-route53-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-28 01:07:01.014431 botocore-a-la-carte-route53-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:01.014431 botocore-a-la-carte-route53-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:01.014431 botocore-a-la-carte-route53-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:01.014431 botocore-a-la-carte-route53-1.34.9/botocore/data/route53/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:01.014431 botocore-a-la-carte-route53-1.34.9/botocore/data/route53/2013-04-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    35205 2023-12-28 01:06:26.000000 botocore-a-la-carte-route53-1.34.9/botocore/data/route53/2013-04-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    29631 2023-12-28 01:06:26.000000 botocore-a-la-carte-route53-1.34.9/botocore/data/route53/2013-04-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-12-28 01:06:26.000000 botocore-a-la-carte-route53-1.34.9/botocore/data/route53/2013-04-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   409774 2023-12-28 01:06:26.000000 botocore-a-la-carte-route53-1.34.9/botocore/data/route53/2013-04-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-28 01:06:26.000000 botocore-a-la-carte-route53-1.34.9/botocore/data/route53/2013-04-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:01.014431 botocore-a-la-carte-route53-1.34.9/botocore_a_la_carte_route53.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-28 01:07:00.000000 botocore-a-la-carte-route53-1.34.9/botocore_a_la_carte_route53.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2023-12-28 01:07:00.000000 botocore-a-la-carte-route53-1.34.9/botocore_a_la_carte_route53.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:07:00.000000 botocore-a-la-carte-route53-1.34.9/botocore_a_la_carte_route53.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:07:00.000000 botocore-a-la-carte-route53-1.34.9/botocore_a_la_carte_route53.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:07:01.014431 botocore-a-la-carte-route53-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-28 01:07:00.000000 botocore-a-la-carte-route53-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-route53-1.34.88/LICENSE.txt` & `botocore-a-la-carte-route53-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53-1.34.88/PKG-INFO` & `botocore-a-la-carte-route53-1.34.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-route53
-Version: 1.34.88
+Version: 1.34.9
 Summary: route53 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-route53-1.34.88/botocore/data/route53/2013-04-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-route53-1.34.9/botocore/data/route53/2013-04-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53-1.34.88/botocore/data/route53/2013-04-01/examples-1.json` & `botocore-a-la-carte-route53-1.34.9/botocore/data/route53/2013-04-01/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53-1.34.88/botocore/data/route53/2013-04-01/paginators-1.json` & `botocore-a-la-carte-route53-1.34.9/botocore/data/route53/2013-04-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53-1.34.88/botocore/data/route53/2013-04-01/service-2.json` & `botocore-a-la-carte-route53-1.34.9/botocore/data/route53/2013-04-01/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982377331877746%*

 * *Differences: {"'shapes'": "{'AliasTarget': {'members': {'HostedZoneId': {'documentation': '<p> <i>Alias "*

 * *             'resource records sets only</i>: The value used depends on where you want to route '*

 * *             'traffic:</p> <dl> <dt>Amazon API Gateway custom regional APIs and edge-optimized '*

 * *             'APIs</dt> <dd> <p>Specify the hosted zone ID for your API. You can get the '*

 * *             'applicable value using the CLI command <a '*

 * *             'href="https://docs.aws.amazon.com/cli/latest/reference/apigat […]*

```diff
@@ -1970,19 +1970,14 @@
             "min": 20,
             "pattern": ".*\\S.*",
             "type": "string"
         },
         "AWSAccountID": {
             "type": "string"
         },
-        "AWSRegion": {
-            "max": 64,
-            "min": 1,
-            "type": "string"
-        },
         "AccountLimit": {
             "documentation": "<p>A complex type that contains the type of limit that you specified in the request and the current value for that limit.</p>",
             "members": {
                 "Type": {
                     "documentation": "<p>The limit that you requested. Valid values include the following:</p> <ul> <li> <p> <b>MAX_HEALTH_CHECKS_BY_OWNER</b>: The maximum number of health checks that you can create using the current account.</p> </li> <li> <p> <b>MAX_HOSTED_ZONES_BY_OWNER</b>: The maximum number of hosted zones that you can create using the current account.</p> </li> <li> <p> <b>MAX_REUSABLE_DELEGATION_SETS_BY_OWNER</b>: The maximum number of reusable delegation sets that you can create using the current account.</p> </li> <li> <p> <b>MAX_TRAFFIC_POLICIES_BY_OWNER</b>: The maximum number of traffic policies that you can create using the current account.</p> </li> <li> <p> <b>MAX_TRAFFIC_POLICY_INSTANCES_BY_OWNER</b>: The maximum number of traffic policy instances that you can create using the current account. (Traffic policy instances are referred to as traffic flow policy records in the Amazon Route 53 console.)</p> </li> </ul>",
                     "shape": "AccountLimitType"
                 },
@@ -2073,15 +2068,15 @@
                     "shape": "DNSName"
                 },
                 "EvaluateTargetHealth": {
                     "documentation": "<p> <i>Applies only to alias, failover alias, geolocation alias, latency alias, and weighted alias resource record sets:</i> When <code>EvaluateTargetHealth</code> is <code>true</code>, an alias resource record set inherits the health of the referenced Amazon Web Services resource, such as an ELB load balancer or another resource record set in the hosted zone.</p> <p>Note the following:</p> <dl> <dt>CloudFront distributions</dt> <dd> <p>You can't set <code>EvaluateTargetHealth</code> to <code>true</code> when the alias target is a CloudFront distribution.</p> </dd> <dt>Elastic Beanstalk environments that have regionalized subdomains</dt> <dd> <p>If you specify an Elastic Beanstalk environment in <code>DNSName</code> and the environment contains an ELB load balancer, Elastic Load Balancing routes queries only to the healthy Amazon EC2 instances that are registered with the load balancer. (An environment automatically contains an ELB load balancer if it includes more than one Amazon EC2 instance.) If you set <code>EvaluateTargetHealth</code> to <code>true</code> and either no Amazon EC2 instances are healthy or the load balancer itself is unhealthy, Route 53 routes queries to other available resources that are healthy, if any. </p> <p>If the environment contains a single Amazon EC2 instance, there are no special requirements.</p> </dd> <dt>ELB load balancers</dt> <dd> <p>Health checking behavior depends on the type of load balancer:</p> <ul> <li> <p> <b>Classic Load Balancers</b>: If you specify an ELB Classic Load Balancer in <code>DNSName</code>, Elastic Load Balancing routes queries only to the healthy Amazon EC2 instances that are registered with the load balancer. If you set <code>EvaluateTargetHealth</code> to <code>true</code> and either no EC2 instances are healthy or the load balancer itself is unhealthy, Route 53 routes queries to other resources.</p> </li> <li> <p> <b>Application and Network Load Balancers</b>: If you specify an ELB Application or Network Load Balancer and you set <code>EvaluateTargetHealth</code> to <code>true</code>, Route 53 routes queries to the load balancer based on the health of the target groups that are associated with the load balancer:</p> <ul> <li> <p>For an Application or Network Load Balancer to be considered healthy, every target group that contains targets must contain at least one healthy target. If any target group contains only unhealthy targets, the load balancer is considered unhealthy, and Route 53 routes queries to other resources.</p> </li> <li> <p>A target group that has no registered targets is considered unhealthy.</p> </li> </ul> </li> </ul> <note> <p>When you create a load balancer, you configure settings for Elastic Load Balancing health checks; they're not Route 53 health checks, but they perform a similar function. Do not create Route 53 health checks for the EC2 instances that you register with an ELB load balancer. </p> </note> </dd> <dt>S3 buckets</dt> <dd> <p>There are no special requirements for setting <code>EvaluateTargetHealth</code> to <code>true</code> when the alias target is an S3 bucket.</p> </dd> <dt>Other records in the same hosted zone</dt> <dd> <p>If the Amazon Web Services resource that you specify in <code>DNSName</code> is a record or a group of records (for example, a group of weighted records) but is not another alias record, we recommend that you associate a health check with all of the records in the alias target. For more information, see <a href=\"https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover-complex-configs.html#dns-failover-complex-configs-hc-omitting\">What Happens When You Omit Health Checks?</a> in the <i>Amazon Route 53 Developer Guide</i>.</p> </dd> </dl> <p>For more information and examples, see <a href=\"https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover.html\">Amazon Route 53 Health Checks and DNS Failover</a> in the <i>Amazon Route 53 Developer Guide</i>.</p>",
                     "shape": "AliasHealthEnabled"
                 },
                 "HostedZoneId": {
-                    "documentation": "<p> <i>Alias resource records sets only</i>: The value used depends on where you want to route traffic:</p> <dl> <dt>Amazon API Gateway custom regional APIs and edge-optimized APIs</dt> <dd> <p>Specify the hosted zone ID for your API. You can get the applicable value using the CLI command <a href=\"https://docs.aws.amazon.com/cli/latest/reference/apigateway/get-domain-names.html\">get-domain-names</a>:</p> <ul> <li> <p>For regional APIs, specify the value of <code>regionalHostedZoneId</code>.</p> </li> <li> <p>For edge-optimized APIs, specify the value of <code>distributionHostedZoneId</code>.</p> </li> </ul> </dd> <dt>Amazon Virtual Private Cloud interface VPC endpoint</dt> <dd> <p>Specify the hosted zone ID for your interface endpoint. You can get the value of <code>HostedZoneId</code> using the CLI command <a href=\"https://docs.aws.amazon.com/cli/latest/reference/ec2/describe-vpc-endpoints.html\">describe-vpc-endpoints</a>.</p> </dd> <dt>CloudFront distribution</dt> <dd> <p>Specify <code>Z2FDTNDATAQYW2</code>.</p> <note> <p>Alias resource record sets for CloudFront can't be created in a private zone.</p> </note> </dd> <dt>Elastic Beanstalk environment</dt> <dd> <p>Specify the hosted zone ID for the region that you created the environment in. The environment must have a regionalized subdomain. For a list of regions and the corresponding hosted zone IDs, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/elasticbeanstalk.html\">Elastic Beanstalk endpoints and quotas</a> in the <i>Amazon Web Services General Reference</i>.</p> </dd> <dt>ELB load balancer</dt> <dd> <p>Specify the value of the hosted zone ID for the load balancer. Use the following methods to get the hosted zone ID:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/general/latest/gr/elb.html\">Elastic Load Balancing endpoints and quotas</a> topic in the <i>Amazon Web Services General Reference</i>: Use the value that corresponds with the region that you created your load balancer in. Note that there are separate columns for Application and Classic Load Balancers and for Network Load Balancers.</p> </li> <li> <p> <b>Amazon Web Services Management Console</b>: Go to the Amazon EC2 page, choose <b>Load Balancers</b> in the navigation pane, select the load balancer, and get the value of the <b>Hosted zone</b> field on the <b>Description</b> tab.</p> </li> <li> <p> <b>Elastic Load Balancing API</b>: Use <code>DescribeLoadBalancers</code> to get the applicable value. For more information, see the applicable guide:</p> <ul> <li> <p>Classic Load Balancers: Use <a href=\"https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_DescribeLoadBalancers.html\">DescribeLoadBalancers</a> to get the value of <code>CanonicalHostedZoneNameId</code>.</p> </li> <li> <p>Application and Network Load Balancers: Use <a href=\"https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_DescribeLoadBalancers.html\">DescribeLoadBalancers</a> to get the value of <code>CanonicalHostedZoneId</code>.</p> </li> </ul> </li> <li> <p> <b>CLI</b>: Use <code>describe-load-balancers</code> to get the applicable value. For more information, see the applicable guide:</p> <ul> <li> <p>Classic Load Balancers: Use <a href=\"http://docs.aws.amazon.com/cli/latest/reference/elb/describe-load-balancers.html\">describe-load-balancers</a> to get the value of <code>CanonicalHostedZoneNameId</code>.</p> </li> <li> <p>Application and Network Load Balancers: Use <a href=\"http://docs.aws.amazon.com/cli/latest/reference/elbv2/describe-load-balancers.html\">describe-load-balancers</a> to get the value of <code>CanonicalHostedZoneId</code>.</p> </li> </ul> </li> </ul> </dd> <dt>Global Accelerator accelerator</dt> <dd> <p>Specify <code>Z2BJ6XQ5FK7U4H</code>.</p> </dd> <dt>An Amazon S3 bucket configured as a static website</dt> <dd> <p>Specify the hosted zone ID for the region that you created the bucket in. For more information about valid values, see the table <a href=\"https://docs.aws.amazon.com/general/latest/gr/s3.html#s3_website_region_endpoints\">Amazon S3 Website Endpoints</a> in the <i>Amazon Web Services General Reference</i>.</p> </dd> <dt>Another Route 53 resource record set in your hosted zone</dt> <dd> <p>Specify the hosted zone ID of your hosted zone. (An alias resource record set can't reference a resource record set in a different hosted zone.)</p> </dd> </dl>",
+                    "documentation": "<p> <i>Alias resource records sets only</i>: The value used depends on where you want to route traffic:</p> <dl> <dt>Amazon API Gateway custom regional APIs and edge-optimized APIs</dt> <dd> <p>Specify the hosted zone ID for your API. You can get the applicable value using the CLI command <a href=\"https://docs.aws.amazon.com/cli/latest/reference/apigateway/get-domain-names.html\">get-domain-names</a>:</p> <ul> <li> <p>For regional APIs, specify the value of <code>regionalHostedZoneId</code>.</p> </li> <li> <p>For edge-optimized APIs, specify the value of <code>distributionHostedZoneId</code>.</p> </li> </ul> </dd> <dt>Amazon Virtual Private Cloud interface VPC endpoint</dt> <dd> <p>Specify the hosted zone ID for your interface endpoint. You can get the value of <code>HostedZoneId</code> using the CLI command <a href=\"https://docs.aws.amazon.com/cli/latest/reference/ec2/describe-vpc-endpoints.html\">describe-vpc-endpoints</a>.</p> </dd> <dt>CloudFront distribution</dt> <dd> <p>Specify <code>Z2FDTNDATAQYW2</code>.</p> <note> <p>Alias resource record sets for CloudFront can't be created in a private zone.</p> </note> </dd> <dt>Elastic Beanstalk environment</dt> <dd> <p>Specify the hosted zone ID for the region that you created the environment in. The environment must have a regionalized subdomain. For a list of regions and the corresponding hosted zone IDs, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/elasticbeanstalk.html\">Elastic Beanstalk endpoints and quotas</a> in the the <i>Amazon Web Services General Reference</i>.</p> </dd> <dt>ELB load balancer</dt> <dd> <p>Specify the value of the hosted zone ID for the load balancer. Use the following methods to get the hosted zone ID:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/general/latest/gr/elb.html\">Elastic Load Balancing endpoints and quotas</a> topic in the <i>Amazon Web Services General Reference</i>: Use the value that corresponds with the region that you created your load balancer in. Note that there are separate columns for Application and Classic Load Balancers and for Network Load Balancers.</p> </li> <li> <p> <b>Amazon Web Services Management Console</b>: Go to the Amazon EC2 page, choose <b>Load Balancers</b> in the navigation pane, select the load balancer, and get the value of the <b>Hosted zone</b> field on the <b>Description</b> tab.</p> </li> <li> <p> <b>Elastic Load Balancing API</b>: Use <code>DescribeLoadBalancers</code> to get the applicable value. For more information, see the applicable guide:</p> <ul> <li> <p>Classic Load Balancers: Use <a href=\"https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_DescribeLoadBalancers.html\">DescribeLoadBalancers</a> to get the value of <code>CanonicalHostedZoneNameId</code>.</p> </li> <li> <p>Application and Network Load Balancers: Use <a href=\"https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_DescribeLoadBalancers.html\">DescribeLoadBalancers</a> to get the value of <code>CanonicalHostedZoneId</code>.</p> </li> </ul> </li> <li> <p> <b>CLI</b>: Use <code>describe-load-balancers</code> to get the applicable value. For more information, see the applicable guide:</p> <ul> <li> <p>Classic Load Balancers: Use <a href=\"http://docs.aws.amazon.com/cli/latest/reference/elb/describe-load-balancers.html\">describe-load-balancers</a> to get the value of <code>CanonicalHostedZoneNameId</code>.</p> </li> <li> <p>Application and Network Load Balancers: Use <a href=\"http://docs.aws.amazon.com/cli/latest/reference/elbv2/describe-load-balancers.html\">describe-load-balancers</a> to get the value of <code>CanonicalHostedZoneId</code>.</p> </li> </ul> </li> </ul> </dd> <dt>Global Accelerator accelerator</dt> <dd> <p>Specify <code>Z2BJ6XQ5FK7U4H</code>.</p> </dd> <dt>An Amazon S3 bucket configured as a static website</dt> <dd> <p>Specify the hosted zone ID for the region that you created the bucket in. For more information about valid values, see the table <a href=\"https://docs.aws.amazon.com/general/latest/gr/s3.html#s3_website_region_endpoints\">Amazon S3 Website Endpoints</a> in the <i>Amazon Web Services General Reference</i>.</p> </dd> <dt>Another Route 53 resource record set in your hosted zone</dt> <dd> <p>Specify the hosted zone ID of your hosted zone. (An alias resource record set can't reference a resource record set in a different hosted zone.)</p> </dd> </dl>",
                     "shape": "ResourceId"
                 }
             },
             "required": [
                 "HostedZoneId",
                 "DNSName",
                 "EvaluateTargetHealth"
@@ -2124,19 +2119,14 @@
                 }
             },
             "required": [
                 "ChangeInfo"
             ],
             "type": "structure"
         },
-        "Bias": {
-            "max": 99,
-            "min": -99,
-            "type": "integer"
-        },
         "Change": {
             "documentation": "<p>The information for each resource record set that you want to change.</p>",
             "members": {
                 "Action": {
                     "documentation": "<p>The action to perform:</p> <ul> <li> <p> <code>CREATE</code>: Creates a resource record set that has the specified values.</p> </li> <li> <p> <code>DELETE</code>: Deletes a existing resource record set.</p> <important> <p>To delete the resource record set that is associated with a traffic policy instance, use <a href=\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_DeleteTrafficPolicyInstance.html\">DeleteTrafficPolicyInstance</a>. Amazon Route 53 will delete the resource record set automatically. If you delete the resource record set by using <code>ChangeResourceRecordSets</code>, Route 53 doesn't automatically delete the traffic policy instance, and you'll continue to be charged for it even though it's no longer in use. </p> </important> </li> <li> <p> <code>UPSERT</code>: If a resource record set doesn't already exist, Route 53 creates it. If a resource record set does exist, Route 53 updates it with the values in the request.</p> </li> </ul>",
                     "shape": "ChangeAction"
                 },
@@ -2694,32 +2684,14 @@
                 "message": {
                     "documentation": "<p/>",
                     "shape": "ErrorMessage"
                 }
             },
             "type": "structure"
         },
-        "Coordinates": {
-            "documentation": "<p> A complex type that lists the coordinates for a geoproximity resource record. </p>",
-            "members": {
-                "Latitude": {
-                    "documentation": "<p> Specifies a coordinate of the north\u2013south position of a geographic point on the surface of the Earth (-90 - 90). </p>",
-                    "shape": "Latitude"
-                },
-                "Longitude": {
-                    "documentation": "<p> Specifies a coordinate of the east\u2013west position of a geographic point on the surface of the Earth (-180 - 180). </p>",
-                    "shape": "Longitude"
-                }
-            },
-            "required": [
-                "Latitude",
-                "Longitude"
-            ],
-            "type": "structure"
-        },
         "CreateCidrCollectionRequest": {
             "members": {
                 "CallerReference": {
                     "documentation": "<p>A client-specific token that allows requests to be securely retried so that the intended outcome will only occur once, retries receive a similar response, and there are no additional edge cases to handle.</p>",
                     "shape": "CidrNonce"
                 },
                 "Name": {
@@ -3170,15 +3142,15 @@
                 "message": {
                     "shape": "ErrorMessage"
                 }
             },
             "type": "structure"
         },
         "DNSSECStatus": {
-            "documentation": "<p>A string representing the status of DNSSEC signing.</p>",
+            "documentation": "<p>A string repesenting the status of DNSSEC signing.</p>",
             "members": {
                 "ServeSignature": {
                     "documentation": "<p>A string that represents the current hosted zone signing status.</p> <p>Status can have one of the following values:</p> <dl> <dt>SIGNING</dt> <dd> <p>DNSSEC signing is enabled for the hosted zone.</p> </dd> <dt>NOT_SIGNING</dt> <dd> <p>DNSSEC signing is not enabled for the hosted zone.</p> </dd> <dt>DELETING</dt> <dd> <p>DNSSEC signing is in the process of being removed for the hosted zone.</p> </dd> <dt>ACTION_NEEDED</dt> <dd> <p>There is a problem with signing in the hosted zone that requires you to take action to resolve. For example, the customer managed key might have been deleted, or the permissions for the customer managed key might have been changed.</p> </dd> <dt>INTERNAL_FAILURE</dt> <dd> <p>There was an error during a request. Before you can continue to work with DNSSEC signing, including with key-signing keys (KSKs), you must correct the problem by enabling or disabling DNSSEC signing for the hosted zone.</p> </dd> </dl>",
                     "shape": "ServeSignature"
                 },
                 "StatusMessage": {
                     "documentation": "<p>The status message provided for the following DNSSEC signing status: <code>INTERNAL_FAILURE</code>. The status message includes information about what the problem might be and steps that you can take to correct the issue.</p>",
@@ -3672,15 +3644,15 @@
             "documentation": "<p>A complex type that contains information about a geographic location.</p>",
             "members": {
                 "ContinentCode": {
                     "documentation": "<p>The two-letter code for the continent.</p> <p>Amazon Route 53 supports the following continent codes:</p> <ul> <li> <p> <b>AF</b>: Africa</p> </li> <li> <p> <b>AN</b>: Antarctica</p> </li> <li> <p> <b>AS</b>: Asia</p> </li> <li> <p> <b>EU</b>: Europe</p> </li> <li> <p> <b>OC</b>: Oceania</p> </li> <li> <p> <b>NA</b>: North America</p> </li> <li> <p> <b>SA</b>: South America</p> </li> </ul> <p>Constraint: Specifying <code>ContinentCode</code> with either <code>CountryCode</code> or <code>SubdivisionCode</code> returns an <code>InvalidInput</code> error.</p>",
                     "shape": "GeoLocationContinentCode"
                 },
                 "CountryCode": {
-                    "documentation": "<p>For geolocation resource record sets, the two-letter code for a country.</p> <p>Amazon Route 53 uses the two-letter country codes that are specified in <a href=\"https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2\">ISO standard 3166-1 alpha-2</a>.</p> <p>Route 53 also supports the country code <b>UA</b> for Ukraine.</p>",
+                    "documentation": "<p>For geolocation resource record sets, the two-letter code for a country.</p> <p>Amazon Route 53 uses the two-letter country codes that are specified in <a href=\"https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2\">ISO standard 3166-1 alpha-2</a>.</p> <p>Route 53 also supports the contry code <b>UA</b> forr Ukraine.</p>",
                     "shape": "GeoLocationCountryCode"
                 },
                 "SubdivisionCode": {
                     "documentation": "<p>For geolocation resource record sets, the two-letter code for a state of the United States. Route 53 doesn't support any other values for <code>SubdivisionCode</code>. For a list of state abbreviations, see <a href=\"https://pe.usps.com/text/pub28/28apb.htm\">Appendix B: Two\u2013Letter State and Possession Abbreviations</a> on the United States Postal Service website. </p> <p>If you specify <code>subdivisioncode</code>, you must also specify <code>US</code> for <code>CountryCode</code>. </p>",
                     "shape": "GeoLocationSubdivisionCode"
                 }
             },
@@ -3749,36 +3721,14 @@
             "type": "string"
         },
         "GeoLocationSubdivisionName": {
             "max": 64,
             "min": 1,
             "type": "string"
         },
-        "GeoProximityLocation": {
-            "documentation": "<p> (Resource record sets only): A complex type that lets you specify where your resources are located. Only one of <code>LocalZoneGroup</code>, <code>Coordinates</code>, or <code>Amazon Web ServicesRegion</code> is allowed per request at a time.</p> <p>For more information about geoproximity routing, see <a href=\"https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy-geoproximity.html\">Geoproximity routing</a> in the <i>Amazon Route\u00a053 Developer Guide</i>.</p>",
-            "members": {
-                "AWSRegion": {
-                    "documentation": "<p> The Amazon Web Services Region the resource you are directing DNS traffic to, is in. </p>",
-                    "shape": "AWSRegion"
-                },
-                "Bias": {
-                    "documentation": "<p> The bias increases or decreases the size of the geographic region from which Route\u00a053 routes traffic to a resource. </p> <p>To use <code>Bias</code> to change the size of the geographic region, specify the applicable value for the bias:</p> <ul> <li> <p>To expand the size of the geographic region from which Route\u00a053 routes traffic to a resource, specify a positive integer from 1 to 99 for the bias. Route\u00a053 shrinks the size of adjacent regions. </p> </li> <li> <p>To shrink the size of the geographic region from which Route\u00a053 routes traffic to a resource, specify a negative bias of -1 to -99. Route\u00a053 expands the size of adjacent regions. </p> </li> </ul>",
-                    "shape": "Bias"
-                },
-                "Coordinates": {
-                    "documentation": "<p> Contains the longitude and latitude for a geographic region. </p>",
-                    "shape": "Coordinates"
-                },
-                "LocalZoneGroup": {
-                    "documentation": "<p> Specifies an Amazon Web Services Local Zone Group. </p> <p>A local Zone Group is usually the Local Zone code without the ending character. For example, if the Local Zone is <code>us-east-1-bue-1a</code> the Local Zone Group is <code>us-east-1-bue-1</code>.</p> <p>You can identify the Local Zones Group for a specific Local Zone by using the <a href=\"https://docs.aws.amazon.com/cli/latest/reference/ec2/describe-availability-zones.html\">describe-availability-zones</a> CLI command:</p> <p>This command returns: <code>\"GroupName\": \"us-west-2-den-1\"</code>, specifying that the Local Zone <code>us-west-2-den-1a</code> belongs to the Local Zone Group <code>us-west-2-den-1</code>.</p>",
-                    "shape": "LocalZoneGroup"
-                }
-            },
-            "type": "structure"
-        },
         "GetAccountLimitRequest": {
             "documentation": "<p>A complex type that contains information about the request to create a hosted zone.</p>",
             "members": {
                 "Type": {
                     "documentation": "<p>The limit that you want to get. Valid values include the following:</p> <ul> <li> <p> <b>MAX_HEALTH_CHECKS_BY_OWNER</b>: The maximum number of health checks that you can create using the current account.</p> </li> <li> <p> <b>MAX_HOSTED_ZONES_BY_OWNER</b>: The maximum number of hosted zones that you can create using the current account.</p> </li> <li> <p> <b>MAX_REUSABLE_DELEGATION_SETS_BY_OWNER</b>: The maximum number of reusable delegation sets that you can create using the current account.</p> </li> <li> <p> <b>MAX_TRAFFIC_POLICIES_BY_OWNER</b>: The maximum number of traffic policies that you can create using the current account.</p> </li> <li> <p> <b>MAX_TRAFFIC_POLICY_INSTANCES_BY_OWNER</b>: The maximum number of traffic policy instances that you can create using the current account. (Traffic policy instances are referred to as traffic flow policy records in the Amazon Route 53 console.)</p> </li> </ul>",
                     "location": "uri",
                     "locationName": "Type",
@@ -3871,15 +3821,15 @@
         "GetDNSSECResponse": {
             "members": {
                 "KeySigningKeys": {
                     "documentation": "<p>The key-signing keys (KSKs) in your account.</p>",
                     "shape": "KeySigningKeys"
                 },
                 "Status": {
-                    "documentation": "<p>A string representing the status of DNSSEC.</p>",
+                    "documentation": "<p>A string repesenting the status of DNSSEC.</p>",
                     "shape": "DNSSECStatus"
                 }
             },
             "required": [
                 "Status",
                 "KeySigningKeys"
             ],
@@ -3891,15 +3841,15 @@
                 "ContinentCode": {
                     "documentation": "<p>For geolocation resource record sets, a two-letter abbreviation that identifies a continent. Amazon Route 53 supports the following continent codes:</p> <ul> <li> <p> <b>AF</b>: Africa</p> </li> <li> <p> <b>AN</b>: Antarctica</p> </li> <li> <p> <b>AS</b>: Asia</p> </li> <li> <p> <b>EU</b>: Europe</p> </li> <li> <p> <b>OC</b>: Oceania</p> </li> <li> <p> <b>NA</b>: North America</p> </li> <li> <p> <b>SA</b>: South America</p> </li> </ul>",
                     "location": "querystring",
                     "locationName": "continentcode",
                     "shape": "GeoLocationContinentCode"
                 },
                 "CountryCode": {
-                    "documentation": "<p>Amazon Route 53 uses the two-letter country codes that are specified in <a href=\"https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2\">ISO standard 3166-1 alpha-2</a>.</p> <p>Route 53 also supports the country code <b>UA</b> for Ukraine.</p>",
+                    "documentation": "<p>Amazon Route 53 uses the two-letter country codes that are specified in <a href=\"https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2\">ISO standard 3166-1 alpha-2</a>.</p> <p>Route 53 also supports the contry code <b>UA</b> forr Ukraine.</p>",
                     "location": "querystring",
                     "locationName": "countrycode",
                     "shape": "GeoLocationCountryCode"
                 },
                 "SubdivisionCode": {
                     "documentation": "<p>The code for the subdivision, such as a particular state within the United States. For a list of US state abbreviations, see <a href=\"https://pe.usps.com/text/pub28/28apb.htm\">Appendix B: Two\u2013Letter State and Possession Abbreviations</a> on the United States Postal Service website. For a list of all supported subdivision codes, use the <a href=\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_ListGeoLocations.html\">ListGeoLocations</a> API.</p>",
                     "location": "querystring",
@@ -4411,15 +4361,15 @@
                     "shape": "RoutingControlArn"
                 },
                 "SearchString": {
                     "documentation": "<p>If the value of Type is <code>HTTP_STR_MATCH</code> or <code>HTTPS_STR_MATCH</code>, the string that you want Amazon Route 53 to search for in the response body from the specified resource. If the string appears in the response body, Route 53 considers the resource healthy.</p> <p>Route 53 considers case when searching for <code>SearchString</code> in the response body. </p>",
                     "shape": "SearchString"
                 },
                 "Type": {
-                    "documentation": "<p>The type of health check that you want to create, which indicates how Amazon Route 53 determines whether an endpoint is healthy.</p> <important> <p>You can't change the value of <code>Type</code> after you create a health check.</p> </important> <p>You can create the following types of health checks:</p> <ul> <li> <p> <b>HTTP</b>: Route 53 tries to establish a TCP connection. If successful, Route 53 submits an HTTP request and waits for an HTTP status code of 200 or greater and less than 400.</p> </li> <li> <p> <b>HTTPS</b>: Route 53 tries to establish a TCP connection. If successful, Route 53 submits an HTTPS request and waits for an HTTP status code of 200 or greater and less than 400.</p> <important> <p>If you specify <code>HTTPS</code> for the value of <code>Type</code>, the endpoint must support TLS v1.0 or later.</p> </important> </li> <li> <p> <b>HTTP_STR_MATCH</b>: Route 53 tries to establish a TCP connection. If successful, Route 53 submits an HTTP request and searches the first 5,120 bytes of the response body for the string that you specify in <code>SearchString</code>.</p> </li> <li> <p> <b>HTTPS_STR_MATCH</b>: Route 53 tries to establish a TCP connection. If successful, Route 53 submits an <code>HTTPS</code> request and searches the first 5,120 bytes of the response body for the string that you specify in <code>SearchString</code>.</p> </li> <li> <p> <b>TCP</b>: Route 53 tries to establish a TCP connection.</p> </li> <li> <p> <b>CLOUDWATCH_METRIC</b>: The health check is associated with a CloudWatch alarm. If the state of the alarm is <code>OK</code>, the health check is considered healthy. If the state is <code>ALARM</code>, the health check is considered unhealthy. If CloudWatch doesn't have sufficient data to determine whether the state is <code>OK</code> or <code>ALARM</code>, the health check status depends on the setting for <code>InsufficientDataHealthStatus</code>: <code>Healthy</code>, <code>Unhealthy</code>, or <code>LastKnownStatus</code>. </p> </li> <li> <p> <b>CALCULATED</b>: For health checks that monitor the status of other health checks, Route 53 adds up the number of health checks that Route 53 health checkers consider to be healthy and compares that number with the value of <code>HealthThreshold</code>. </p> </li> <li> <p> <b>RECOVERY_CONTROL</b>: The health check is associated with a Route53 Application Recovery Controller routing control. If the routing control state is <code>ON</code>, the health check is considered healthy. If the state is <code>OFF</code>, the health check is considered unhealthy. </p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover-determining-health-of-endpoints.html\">How Route 53 Determines Whether an Endpoint Is Healthy</a> in the <i>Amazon Route 53 Developer Guide</i>.</p>",
+                    "documentation": "<p>The type of health check that you want to create, which indicates how Amazon Route 53 determines whether an endpoint is healthy.</p> <important> <p>You can't change the value of <code>Type</code> after you create a health check.</p> </important> <p>You can create the following types of health checks:</p> <ul> <li> <p> <b>HTTP</b>: Route 53 tries to establish a TCP connection. If successful, Route 53 submits an HTTP request and waits for an HTTP status code of 200 or greater and less than 400.</p> </li> <li> <p> <b>HTTPS</b>: Route 53 tries to establish a TCP connection. If successful, Route 53 submits an HTTPS request and waits for an HTTP status code of 200 or greater and less than 400.</p> <important> <p>If you specify <code>HTTPS</code> for the value of <code>Type</code>, the endpoint must support TLS v1.0 or later.</p> </important> </li> <li> <p> <b>HTTP_STR_MATCH</b>: Route 53 tries to establish a TCP connection. If successful, Route 53 submits an HTTP request and searches the first 5,120 bytes of the response body for the string that you specify in <code>SearchString</code>.</p> </li> <li> <p> <b>HTTPS_STR_MATCH</b>: Route 53 tries to establish a TCP connection. If successful, Route 53 submits an <code>HTTPS</code> request and searches the first 5,120 bytes of the response body for the string that you specify in <code>SearchString</code>.</p> </li> <li> <p> <b>TCP</b>: Route 53 tries to establish a TCP connection.</p> </li> <li> <p> <b>CLOUDWATCH_METRIC</b>: The health check is associated with a CloudWatch alarm. If the state of the alarm is <code>OK</code>, the health check is considered healthy. If the state is <code>ALARM</code>, the health check is considered unhealthy. If CloudWatch doesn't have sufficient data to determine whether the state is <code>OK</code> or <code>ALARM</code>, the health check status depends on the setting for <code>InsufficientDataHealthStatus</code>: <code>Healthy</code>, <code>Unhealthy</code>, or <code>LastKnownStatus</code>. </p> </li> <li> <p> <b>CALCULATED</b>: For health checks that monitor the status of other health checks, Route 53 adds up the number of health checks that Route 53 health checkers consider to be healthy and compares that number with the value of <code>HealthThreshold</code>. </p> </li> <li> <p> <b>RECOVERY_CONTROL</b>: The health check is assocated with a Route53 Application Recovery Controller routing control. If the routing control state is <code>ON</code>, the health check is considered healthy. If the state is <code>OFF</code>, the health check is considered unhealthy. </p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover-determining-health-of-endpoints.html\">How Route 53 Determines Whether an Endpoint Is Healthy</a> in the <i>Amazon Route 53 Developer Guide</i>.</p>",
                     "shape": "HealthCheckType"
                 }
             },
             "required": [
                 "Type"
             ],
             "type": "structure"
@@ -5063,20 +5013,14 @@
                 "message": {
                     "documentation": "<p/>",
                     "shape": "ErrorMessage"
                 }
             },
             "type": "structure"
         },
-        "Latitude": {
-            "max": 6,
-            "min": 1,
-            "pattern": "[-+]?[0-9]{1,2}(\\.[0-9]{0,2})?",
-            "type": "string"
-        },
         "LimitValue": {
             "min": 1,
             "type": "long"
         },
         "LimitsExceeded": {
             "documentation": "<p>This operation can't be completed because the current account has reached the limit on the resource you are trying to create. To request a higher limit, <a href=\"http://aws.amazon.com/route53-request\">create a case</a> with the Amazon Web Services Support Center.</p>",
             "exception": true,
@@ -6097,19 +6041,14 @@
             },
             "required": [
                 "HostedZoneId",
                 "VPCs"
             ],
             "type": "structure"
         },
-        "LocalZoneGroup": {
-            "max": 64,
-            "min": 1,
-            "type": "string"
-        },
         "LocationSummaries": {
             "member": {
                 "shape": "LocationSummary"
             },
             "type": "list"
         },
         "LocationSummary": {
@@ -6118,20 +6057,14 @@
                 "LocationName": {
                     "documentation": "<p>A string that specifies a location name.</p>",
                     "shape": "CidrLocationNameDefaultAllowed"
                 }
             },
             "type": "structure"
         },
-        "Longitude": {
-            "max": 7,
-            "min": 1,
-            "pattern": "[-+]?[0-9]{1,3}(\\.[0-9]{0,2})?",
-            "type": "string"
-        },
         "MaxResults": {
             "type": "string"
         },
         "MeasureLatency": {
             "type": "boolean"
         },
         "Message": {
@@ -6524,21 +6457,17 @@
                     "shape": "CidrRoutingConfig"
                 },
                 "Failover": {
                     "documentation": "<p> <i>Failover resource record sets only:</i> To configure failover, you add the <code>Failover</code> element to two resource record sets. For one resource record set, you specify <code>PRIMARY</code> as the value for <code>Failover</code>; for the other resource record set, you specify <code>SECONDARY</code>. In addition, you include the <code>HealthCheckId</code> element and specify the health check that you want Amazon Route 53 to perform for each resource record set.</p> <p>Except where noted, the following failover behaviors assume that you have included the <code>HealthCheckId</code> element in both resource record sets:</p> <ul> <li> <p>When the primary resource record set is healthy, Route 53 responds to DNS queries with the applicable value from the primary resource record set regardless of the health of the secondary resource record set.</p> </li> <li> <p>When the primary resource record set is unhealthy and the secondary resource record set is healthy, Route 53 responds to DNS queries with the applicable value from the secondary resource record set.</p> </li> <li> <p>When the secondary resource record set is unhealthy, Route 53 responds to DNS queries with the applicable value from the primary resource record set regardless of the health of the primary resource record set.</p> </li> <li> <p>If you omit the <code>HealthCheckId</code> element for the secondary resource record set, and if the primary resource record set is unhealthy, Route 53 always responds to DNS queries with the applicable value from the secondary resource record set. This is true regardless of the health of the associated endpoint.</p> </li> </ul> <p>You can't create non-failover resource record sets that have the same values for the <code>Name</code> and <code>Type</code> elements as failover resource record sets.</p> <p>For failover alias resource record sets, you must also include the <code>EvaluateTargetHealth</code> element and set the value to true.</p> <p>For more information about configuring failover for Route 53, see the following topics in the <i>Amazon Route 53 Developer Guide</i>: </p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover.html\">Route 53 Health Checks and DNS Failover</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover-private-hosted-zones.html\">Configuring Failover in a Private Hosted Zone</a> </p> </li> </ul>",
                     "shape": "ResourceRecordSetFailover"
                 },
                 "GeoLocation": {
-                    "documentation": "<p> <i>Geolocation resource record sets only:</i> A complex type that lets you control how Amazon Route 53 responds to DNS queries based on the geographic origin of the query. For example, if you want all queries from Africa to be routed to a web server with an IP address of <code>192.0.2.111</code>, create a resource record set with a <code>Type</code> of <code>A</code> and a <code>ContinentCode</code> of <code>AF</code>.</p> <p>If you create separate resource record sets for overlapping geographic regions (for example, one resource record set for a continent and one for a country on the same continent), priority goes to the smallest geographic region. This allows you to route most queries for a continent to one resource and to route queries for a country on that continent to a different resource.</p> <p>You can't create two geolocation resource record sets that specify the same geographic location.</p> <p>The value <code>*</code> in the <code>CountryCode</code> element matches all geographic locations that aren't specified in other geolocation resource record sets that have the same values for the <code>Name</code> and <code>Type</code> elements.</p> <important> <p>Geolocation works by mapping IP addresses to locations. However, some IP addresses aren't mapped to geographic locations, so even if you create geolocation resource record sets that cover all seven continents, Route 53 will receive some DNS queries from locations that it can't identify. We recommend that you create a resource record set for which the value of <code>CountryCode</code> is <code>*</code>. Two groups of queries are routed to the resource that you specify in this record: queries that come from locations for which you haven't created geolocation resource record sets and queries from IP addresses that aren't mapped to a location. If you don't create a <code>*</code> resource record set, Route 53 returns a \"no answer\" response for queries from those locations.</p> </important> <p>You can't create non-geolocation resource record sets that have the same values for the <code>Name</code> and <code>Type</code> elements as geolocation resource record sets.</p>",
+                    "documentation": "<p> <i>Geolocation resource record sets only:</i> A complex type that lets you control how Amazon Route 53 responds to DNS queries based on the geographic origin of the query. For example, if you want all queries from Africa to be routed to a web server with an IP address of <code>192.0.2.111</code>, create a resource record set with a <code>Type</code> of <code>A</code> and a <code>ContinentCode</code> of <code>AF</code>.</p> <note> <p>Although creating geolocation and geolocation alias resource record sets in a private hosted zone is allowed, it's not supported.</p> </note> <p>If you create separate resource record sets for overlapping geographic regions (for example, one resource record set for a continent and one for a country on the same continent), priority goes to the smallest geographic region. This allows you to route most queries for a continent to one resource and to route queries for a country on that continent to a different resource.</p> <p>You can't create two geolocation resource record sets that specify the same geographic location.</p> <p>The value <code>*</code> in the <code>CountryCode</code> element matches all geographic locations that aren't specified in other geolocation resource record sets that have the same values for the <code>Name</code> and <code>Type</code> elements.</p> <important> <p>Geolocation works by mapping IP addresses to locations. However, some IP addresses aren't mapped to geographic locations, so even if you create geolocation resource record sets that cover all seven continents, Route 53 will receive some DNS queries from locations that it can't identify. We recommend that you create a resource record set for which the value of <code>CountryCode</code> is <code>*</code>. Two groups of queries are routed to the resource that you specify in this record: queries that come from locations for which you haven't created geolocation resource record sets and queries from IP addresses that aren't mapped to a location. If you don't create a <code>*</code> resource record set, Route 53 returns a \"no answer\" response for queries from those locations.</p> </important> <p>You can't create non-geolocation resource record sets that have the same values for the <code>Name</code> and <code>Type</code> elements as geolocation resource record sets.</p>",
                     "shape": "GeoLocation"
                 },
-                "GeoProximityLocation": {
-                    "documentation": "<p> <i> GeoproximityLocation resource record sets only:</i> A complex type that lets you control how Route\u00a053 responds to DNS queries based on the geographic origin of the query and your resources. </p>",
-                    "shape": "GeoProximityLocation"
-                },
                 "HealthCheckId": {
                     "documentation": "<p>If you want Amazon Route 53 to return this resource record set in response to a DNS query only when the status of a health check is healthy, include the <code>HealthCheckId</code> element and specify the ID of the applicable health check.</p> <p>Route 53 determines whether a resource record set is healthy based on one of the following:</p> <ul> <li> <p>By periodically sending a request to the endpoint that is specified in the health check</p> </li> <li> <p>By aggregating the status of a specified group of health checks (calculated health checks)</p> </li> <li> <p>By determining the current state of a CloudWatch alarm (CloudWatch metric health checks)</p> </li> </ul> <important> <p>Route 53 doesn't check the health of the endpoint that is specified in the resource record set, for example, the endpoint specified by the IP address in the <code>Value</code> element. When you add a <code>HealthCheckId</code> element to a resource record set, Route 53 checks the health of the endpoint that you specified in the health check. </p> </important> <p>For more information, see the following topics in the <i>Amazon Route 53 Developer Guide</i>:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover-determining-health-of-endpoints.html\">How Amazon Route 53 Determines Whether an Endpoint Is Healthy</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover.html\">Route 53 Health Checks and DNS Failover</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover-private-hosted-zones.html\">Configuring Failover in a Private Hosted Zone</a> </p> </li> </ul> <p> <b>When to Specify HealthCheckId</b> </p> <p>Specifying a value for <code>HealthCheckId</code> is useful only when Route 53 is choosing between two or more resource record sets to respond to a DNS query, and you want Route 53 to base the choice in part on the status of a health check. Configuring health checks makes sense only in the following configurations:</p> <ul> <li> <p> <b>Non-alias resource record sets</b>: You're checking the health of a group of non-alias resource record sets that have the same routing policy, name, and type (such as multiple weighted records named www.example.com with a type of A) and you specify health check IDs for all the resource record sets. </p> <p>If the health check status for a resource record set is healthy, Route 53 includes the record among the records that it responds to DNS queries with.</p> <p>If the health check status for a resource record set is unhealthy, Route 53 stops responding to DNS queries using the value for that resource record set.</p> <p>If the health check status for all resource record sets in the group is unhealthy, Route 53 considers all resource record sets in the group healthy and responds to DNS queries accordingly. </p> </li> <li> <p> <b>Alias resource record sets</b>: You specify the following settings:</p> <ul> <li> <p>You set <code>EvaluateTargetHealth</code> to true for an alias resource record set in a group of resource record sets that have the same routing policy, name, and type (such as multiple weighted records named www.example.com with a type of A). </p> </li> <li> <p>You configure the alias resource record set to route traffic to a non-alias resource record set in the same hosted zone.</p> </li> <li> <p>You specify a health check ID for the non-alias resource record set. </p> </li> </ul> <p>If the health check status is healthy, Route 53 considers the alias resource record set to be healthy and includes the alias record among the records that it responds to DNS queries with.</p> <p>If the health check status is unhealthy, Route 53 stops responding to DNS queries using the alias resource record set.</p> <note> <p>The alias resource record set can also route traffic to a <i>group</i> of non-alias resource record sets that have the same routing policy, name, and type. In that configuration, associate health checks with all of the resource record sets in the group of non-alias resource record sets.</p> </note> </li> </ul> <p> <b>Geolocation Routing</b> </p> <p>For geolocation resource record sets, if an endpoint is unhealthy, Route 53 looks for a resource record set for the larger, associated geographic region. For example, suppose you have resource record sets for a state in the United States, for the entire United States, for North America, and a resource record set that has <code>*</code> for <code>CountryCode</code> is <code>*</code>, which applies to all locations. If the endpoint for the state resource record set is unhealthy, Route 53 checks for healthy resource record sets in the following order until it finds a resource record set for which the endpoint is healthy:</p> <ul> <li> <p>The United States</p> </li> <li> <p>North America</p> </li> <li> <p>The default resource record set</p> </li> </ul> <p> <b>Specifying the Health Check Endpoint by Domain Name</b> </p> <p>If your health checks specify the endpoint only by domain name, we recommend that you create a separate health check for each endpoint. For example, create a health check for each <code>HTTP</code> server that is serving content for <code>www.example.com</code>. For the value of <code>FullyQualifiedDomainName</code>, specify the domain name of the server (such as <code>us-east-2-www.example.com</code>), not the name of the resource record sets (<code>www.example.com</code>).</p> <important> <p>Health check results will be unpredictable if you do the following:</p> <ul> <li> <p>Create a health check that has the same value for <code>FullyQualifiedDomainName</code> as the name of a resource record set.</p> </li> <li> <p>Associate that health check with the resource record set.</p> </li> </ul> </important>",
                     "shape": "HealthCheckId"
                 },
                 "MultiValueAnswer": {
                     "documentation": "<p> <i>Multivalue answer resource record sets only</i>: To route traffic approximately randomly to multiple resources, such as web servers, create one multivalue answer record for each resource and specify <code>true</code> for <code>MultiValueAnswer</code>. Note the following:</p> <ul> <li> <p>If you associate a health check with a multivalue answer resource record set, Amazon Route 53 responds to DNS queries with the corresponding IP address only when the health check is healthy.</p> </li> <li> <p>If you don't associate a health check with a multivalue answer record, Route 53 always considers the record to be healthy.</p> </li> <li> <p>Route 53 responds to DNS queries with up to eight healthy records; if you have eight or fewer healthy records, Route 53 responds to all DNS queries with all the healthy records.</p> </li> <li> <p>If you have more than eight healthy records, Route 53 responds to different DNS resolvers with different combinations of healthy records.</p> </li> <li> <p>When all records are unhealthy, Route 53 responds to DNS queries with up to eight unhealthy records.</p> </li> <li> <p>If a resource becomes unavailable after a resolver caches a response, client software typically tries another of the IP addresses in the response.</p> </li> </ul> <p>You can't create multivalue answer alias records.</p>",
                     "shape": "ResourceRecordSetMultiValueAnswer"
@@ -7293,15 +7222,15 @@
                     "shape": "EnableSNI"
                 },
                 "FailureThreshold": {
                     "documentation": "<p>The number of consecutive health checks that an endpoint must pass or fail for Amazon Route 53 to change the current status of the endpoint from unhealthy to healthy or vice versa. For more information, see <a href=\"https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover-determining-health-of-endpoints.html\">How Amazon Route 53 Determines Whether an Endpoint Is Healthy</a> in the <i>Amazon Route 53 Developer Guide</i>.</p> <p>If you don't specify a value for <code>FailureThreshold</code>, the default value is three health checks.</p>",
                     "shape": "FailureThreshold"
                 },
                 "FullyQualifiedDomainName": {
-                    "documentation": "<p>Amazon Route 53 behavior depends on whether you specify a value for <code>IPAddress</code>.</p> <note> <p>If a health check already has a value for <code>IPAddress</code>, you can change the value. However, you can't update an existing health check to add or remove the value of <code>IPAddress</code>. </p> </note> <p> <b>If you specify a value for</b> <code>IPAddress</code>:</p> <p>Route 53 sends health check requests to the specified IPv4 or IPv6 address and passes the value of <code>FullyQualifiedDomainName</code> in the <code>Host</code> header for all health checks except TCP health checks. This is typically the fully qualified DNS name of the endpoint on which you want Route 53 to perform health checks.</p> <p>When Route 53 checks the health of an endpoint, here is how it constructs the <code>Host</code> header:</p> <ul> <li> <p>If you specify a value of <code>80</code> for <code>Port</code> and <code>HTTP</code> or <code>HTTP_STR_MATCH</code> for <code>Type</code>, Route 53 passes the value of <code>FullyQualifiedDomainName</code> to the endpoint in the <code>Host</code> header.</p> </li> <li> <p>If you specify a value of <code>443</code> for <code>Port</code> and <code>HTTPS</code> or <code>HTTPS_STR_MATCH</code> for <code>Type</code>, Route 53 passes the value of <code>FullyQualifiedDomainName</code> to the endpoint in the <code>Host</code> header.</p> </li> <li> <p>If you specify another value for <code>Port</code> and any value except <code>TCP</code> for <code>Type</code>, Route 53 passes <i> <code>FullyQualifiedDomainName</code>:<code>Port</code> </i> to the endpoint in the <code>Host</code> header.</p> </li> </ul> <p>If you don't specify a value for <code>FullyQualifiedDomainName</code>, Route 53 substitutes the value of <code>IPAddress</code> in the <code>Host</code> header in each of the above cases.</p> <p> <b>If you don't specify a value for</b> <code>IPAddress</code>:</p> <p>If you don't specify a value for <code>IPAddress</code>, Route 53 sends a DNS request to the domain that you specify in <code>FullyQualifiedDomainName</code> at the interval you specify in <code>RequestInterval</code>. Using an IPv4 address that is returned by DNS, Route 53 then checks the health of the endpoint.</p> <p>If you don't specify a value for <code>IPAddress</code>, you can\u2019t update the health check to remove the <code>FullyQualifiedDomainName</code>; if you don\u2019t specify a value for <code>IPAddress</code> on creation, a <code>FullyQualifiedDomainName</code> is required.</p> <note> <p>If you don't specify a value for <code>IPAddress</code>, Route 53 uses only IPv4 to send health checks to the endpoint. If there's no resource record set with a type of A for the name that you specify for <code>FullyQualifiedDomainName</code>, the health check fails with a \"DNS resolution failed\" error.</p> </note> <p>If you want to check the health of weighted, latency, or failover resource record sets and you choose to specify the endpoint only by <code>FullyQualifiedDomainName</code>, we recommend that you create a separate health check for each endpoint. For example, create a health check for each HTTP server that is serving content for www.example.com. For the value of <code>FullyQualifiedDomainName</code>, specify the domain name of the server (such as <code>us-east-2-www.example.com</code>), not the name of the resource record sets (www.example.com).</p> <important> <p>In this configuration, if the value of <code>FullyQualifiedDomainName</code> matches the name of the resource record sets and you then associate the health check with those resource record sets, health check results will be unpredictable.</p> </important> <p>In addition, if the value of <code>Type</code> is <code>HTTP</code>, <code>HTTPS</code>, <code>HTTP_STR_MATCH</code>, or <code>HTTPS_STR_MATCH</code>, Route 53 passes the value of <code>FullyQualifiedDomainName</code> in the <code>Host</code> header, as it does when you specify a value for <code>IPAddress</code>. If the value of <code>Type</code> is <code>TCP</code>, Route 53 doesn't pass a <code>Host</code> header.</p>",
+                    "documentation": "<p>Amazon Route 53 behavior depends on whether you specify a value for <code>IPAddress</code>.</p> <note> <p>If a health check already has a value for <code>IPAddress</code>, you can change the value. However, you can't update an existing health check to add or remove the value of <code>IPAddress</code>. </p> </note> <p> <b>If you specify a value for</b> <code>IPAddress</code>:</p> <p>Route 53 sends health check requests to the specified IPv4 or IPv6 address and passes the value of <code>FullyQualifiedDomainName</code> in the <code>Host</code> header for all health checks except TCP health checks. This is typically the fully qualified DNS name of the endpoint on which you want Route 53 to perform health checks.</p> <p>When Route 53 checks the health of an endpoint, here is how it constructs the <code>Host</code> header:</p> <ul> <li> <p>If you specify a value of <code>80</code> for <code>Port</code> and <code>HTTP</code> or <code>HTTP_STR_MATCH</code> for <code>Type</code>, Route 53 passes the value of <code>FullyQualifiedDomainName</code> to the endpoint in the <code>Host</code> header.</p> </li> <li> <p>If you specify a value of <code>443</code> for <code>Port</code> and <code>HTTPS</code> or <code>HTTPS_STR_MATCH</code> for <code>Type</code>, Route 53 passes the value of <code>FullyQualifiedDomainName</code> to the endpoint in the <code>Host</code> header.</p> </li> <li> <p>If you specify another value for <code>Port</code> and any value except <code>TCP</code> for <code>Type</code>, Route 53 passes <i> <code>FullyQualifiedDomainName</code>:<code>Port</code> </i> to the endpoint in the <code>Host</code> header.</p> </li> </ul> <p>If you don't specify a value for <code>FullyQualifiedDomainName</code>, Route 53 substitutes the value of <code>IPAddress</code> in the <code>Host</code> header in each of the above cases.</p> <p> <b>If you don't specify a value for</b> <code>IPAddress</code>:</p> <p>If you don't specify a value for <code>IPAddress</code>, Route 53 sends a DNS request to the domain that you specify in <code>FullyQualifiedDomainName</code> at the interval you specify in <code>RequestInterval</code>. Using an IPv4 address that is returned by DNS, Route 53 then checks the health of the endpoint.</p> <note> <p>If you don't specify a value for <code>IPAddress</code>, Route 53 uses only IPv4 to send health checks to the endpoint. If there's no resource record set with a type of A for the name that you specify for <code>FullyQualifiedDomainName</code>, the health check fails with a \"DNS resolution failed\" error.</p> </note> <p>If you want to check the health of weighted, latency, or failover resource record sets and you choose to specify the endpoint only by <code>FullyQualifiedDomainName</code>, we recommend that you create a separate health check for each endpoint. For example, create a health check for each HTTP server that is serving content for www.example.com. For the value of <code>FullyQualifiedDomainName</code>, specify the domain name of the server (such as <code>us-east-2-www.example.com</code>), not the name of the resource record sets (www.example.com).</p> <important> <p>In this configuration, if the value of <code>FullyQualifiedDomainName</code> matches the name of the resource record sets and you then associate the health check with those resource record sets, health check results will be unpredictable.</p> </important> <p>In addition, if the value of <code>Type</code> is <code>HTTP</code>, <code>HTTPS</code>, <code>HTTP_STR_MATCH</code>, or <code>HTTPS_STR_MATCH</code>, Route 53 passes the value of <code>FullyQualifiedDomainName</code> in the <code>Host</code> header, as it does when you specify a value for <code>IPAddress</code>. If the value of <code>Type</code> is <code>TCP</code>, Route 53 doesn't pass a <code>Host</code> header.</p>",
                     "shape": "FullyQualifiedDomainName"
                 },
                 "HealthCheckId": {
                     "documentation": "<p>The ID for the health check for which you want detailed information. When you created the health check, <code>CreateHealthCheck</code> returned the ID in the response, in the <code>HealthCheckId</code> element.</p>",
                     "location": "uri",
                     "locationName": "HealthCheckId",
                     "shape": "HealthCheckId"
```

### Comparing `botocore-a-la-carte-route53-1.34.88/botocore_a_la_carte_route53.egg-info/PKG-INFO` & `botocore-a-la-carte-route53-1.34.9/botocore_a_la_carte_route53.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-route53
-Version: 1.34.88
+Version: 1.34.9
 Summary: route53 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-route53-1.34.88/setup.py` & `botocore-a-la-carte-route53-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-route53',
-    version="1.34.88",
+    version="1.34.9",
     description='route53 data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/route53/*/*.json'],
```

