# Comparing `tmp/phidata-2.3.8.tar.gz` & `tmp/phidata-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-2.3.8.tar", last modified: Mon Jan 29 15:46:37 2024, max compression
+gzip compressed data, was "phidata-2.3.9.tar", last modified: Tue Jan 30 14:44:14 2024, max compression
```

## Comparing `phidata-2.3.8.tar` & `phidata-2.3.9.tar`

### file list

```diff
@@ -1,559 +1,559 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.772107 phidata-2.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-01-29 15:46:19.000000 phidata-2.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    29992 2024-01-29 15:46:37.772107 phidata-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    28996 2024-01-29 15:46:19.000000 phidata-2.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.692107 phidata-2.3.8/phi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.692107 phidata-2.3.8/phi/ai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/ai/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/ai/phi_ai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.700107 phidata-2.3.8/phi/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/ai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.700107 phidata-2.3.8/phi/api/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/schemas/ai.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/schemas/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/schemas/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/schemas/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.700107 phidata-2.3.8/phi/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/app/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/app/db_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/app/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.700107 phidata-2.3.8/phi/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34089 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.700107 phidata-2.3.8/phi/assistant/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12062 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/openai/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/openai/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.700107 phidata-2.3.8/phi/assistant/openai/file/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/openai/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/openai/file/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/openai/file/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/openai/file/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/openai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/openai/row.py
--rw-r--r--   0 runner    (1001) docker     (127)    14892 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/openai/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/openai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/assistant/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.700107 phidata-2.3.8/phi/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.700107 phidata-2.3.8/phi/aws/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34343 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/app/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.700107 phidata-2.3.8/phi/aws/app/django/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/app/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/app/django/django.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.708107 phidata-2.3.8/phi/aws/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.708107 phidata-2.3.8/phi/aws/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/app/jupyter/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.708107 phidata-2.3.8/phi/aws/app/qdrant/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/app/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/app/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.708107 phidata-2.3.8/phi/aws/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.708107 phidata-2.3.8/phi/aws/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.708107 phidata-2.3.8/phi/aws/resource/acm/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/acm/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.708107 phidata-2.3.8/phi/aws/resource/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.708107 phidata-2.3.8/phi/aws/resource/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25483 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/ec2/security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/ec2/subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/ec2/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.712108 phidata-2.3.8/phi/aws/resource/ecs/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/ecs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/ecs/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    19749 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/ecs/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    23497 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/ecs/task_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/ecs/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.712108 phidata-2.3.8/phi/aws/resource/eks/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/eks/addon.py
--rw-r--r--   0 runner    (1001) docker     (127)    31036 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    13621 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    23482 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/eks/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.712108 phidata-2.3.8/phi/aws/resource/elasticache/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22351 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/elasticache/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.712108 phidata-2.3.8/phi/aws/resource/elb/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/elb/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/elb/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/elb/target_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.712108 phidata-2.3.8/phi/aws/resource/emr/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/emr/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.712108 phidata-2.3.8/phi/aws/resource/glue/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/glue/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.712108 phidata-2.3.8/phi/aws/resource/iam/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/aws/resource/rds/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42214 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/rds/db_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    36599 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/rds/db_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/rds/db_subnet_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/aws/resource/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/s3/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/s3/object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/aws/resource/secret/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/secret/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/secret/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    31439 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/aws/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/cli/auth_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/cli/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/cli/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    20694 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/cli/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/cli/k/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/cli/k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/cli/k/k_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13585 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/cli/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/cli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27968 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/cli/ws/ws_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/docker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/docker/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/docker/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17444 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/airflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/airflow/flower.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/airflow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/airflow/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/airflow/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/docker/app/django/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/django/django.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/docker/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/docker/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/jupyter/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/docker/app/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/mysql/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/docker/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/postgres/pgvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/postgres/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/docker/app/qdrant/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/docker/app/redis/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.716107 phidata-2.3.8/phi/docker/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.720107 phidata-2.3.8/phi/docker/app/superset/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/superset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/superset/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/superset/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/superset/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/superset/worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.720107 phidata-2.3.8/phi/docker/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/traefik/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.720107 phidata-2.3.8/phi/docker/app/whoami/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/whoami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/app/whoami/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.720107 phidata-2.3.8/phi/docker/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15995 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/resource/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/resource/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/resource/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    31615 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/docker/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.720107 phidata-2.3.8/phi/document/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/document/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.724107 phidata-2.3.8/phi/document/reader/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/document/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/document/reader/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/document/reader/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/document/reader/docx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/document/reader/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/document/reader/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.724107 phidata-2.3.8/phi/document/reader/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/document/reader/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/document/reader/s3/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/document/reader/s3/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/document/reader/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/document/reader/website.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.724107 phidata-2.3.8/phi/embedder/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/embedder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/embedder/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/embedder/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.724107 phidata-2.3.8/phi/file/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.724107 phidata-2.3.8/phi/file/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/file/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/file/local/csv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.724107 phidata-2.3.8/phi/infra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/infra/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/infra/type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.724107 phidata-2.3.8/phi/k8s/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.732107 phidata-2.3.8/phi/k8s/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.732107 phidata-2.3.8/phi/k8s/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14290 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/airflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/airflow/flower.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/airflow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/airflow/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/airflow/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    59184 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.732107 phidata-2.3.8/phi/k8s/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.732107 phidata-2.3.8/phi/k8s/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/jupyter/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.732107 phidata-2.3.8/phi/k8s/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/postgres/pgvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/postgres/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.732107 phidata-2.3.8/phi/k8s/app/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.732107 phidata-2.3.8/phi/k8s/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.732107 phidata-2.3.8/phi/k8s/app/superset/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/superset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/superset/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/superset/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/superset/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/superset/worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.736107 phidata-2.3.8/phi/k8s/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   115745 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/traefik/crds.py
--rw-r--r--   0 runner    (1001) docker     (127)    13305 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/app/traefik/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.736107 phidata-2.3.8/phi/k8s/create/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.736107 phidata-2.3.8/phi/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.736107 phidata-2.3.8/phi/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.736107 phidata-2.3.8/phi/k8s/create/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.736107 phidata-2.3.8/phi/k8s/create/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.736107 phidata-2.3.8/phi/k8s/create/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/common/port.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.736107 phidata-2.3.8/phi/k8s/create/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.740107 phidata-2.3.8/phi/k8s/create/core/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.740107 phidata-2.3.8/phi/k8s/create/crb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/crb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/crb/eks_admin_crb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.740107 phidata-2.3.8/phi/k8s/create/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.740107 phidata-2.3.8/phi/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.740107 phidata-2.3.8/phi/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.740107 phidata-2.3.8/phi/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.740107 phidata-2.3.8/phi/k8s/create/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.740107 phidata-2.3.8/phi/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.740107 phidata-2.3.8/phi/k8s/enums/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/enums/api_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/enums/api_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/enums/image_pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/enums/kind.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/enums/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/enums/pv.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/enums/restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/enums/service_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/enums/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/enums/volume_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10016 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/core/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    18798 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    20764 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.744107 phidata-2.3.8/phi/k8s/resource/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.748108 phidata-2.3.8/phi/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resource/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)    44793 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/k8s/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.748108 phidata-2.3.8/phi/knowledge/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/docx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.748108 phidata-2.3.8/phi/knowledge/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/s3/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/s3/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/s3/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/website.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/knowledge/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.748108 phidata-2.3.8/phi/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.752107 phidata-2.3.8/phi/llm/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/llm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14445 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/llm/aws/bedrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/llm/aws/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/llm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/llm/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.752107 phidata-2.3.8/phi/llm/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/llm/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35855 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/llm/openai/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/llm/references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.752107 phidata-2.3.8/phi/memory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/memory/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.752107 phidata-2.3.8/phi/memory/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/memory/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/memory/task/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.752107 phidata-2.3.8/phi/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/resource/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.752107 phidata-2.3.8/phi/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.752107 phidata-2.3.8/phi/storage/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/storage/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/storage/assistant/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/storage/assistant/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/storage/assistant/sqllite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.752107 phidata-2.3.8/phi/table/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.752107 phidata-2.3.8/phi/table/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/table/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/table/sql/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.752107 phidata-2.3.8/phi/task/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/task/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.756107 phidata-2.3.8/phi/task/llm/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/task/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31776 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/task/llm/llm_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.756107 phidata-2.3.8/phi/task/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/task/py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/task/py/python_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.756107 phidata-2.3.8/phi/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)    14658 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.756107 phidata-2.3.8/phi/tools/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/fastapi/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/phi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.756107 phidata-2.3.8/phi/tools/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/streamlit/components.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/tool_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/tools/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.760107 phidata-2.3.8/phi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/format_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/json_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/merge_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/py_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/response_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/utils/yaml_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.760107 phidata-2.3.8/phi/vectordb/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/vectordb/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/vectordb/distance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.764107 phidata-2.3.8/phi/vectordb/pgvector/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/vectordb/pgvector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/vectordb/pgvector/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    13209 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/vectordb/pgvector/pgvector.py
--rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/vectordb/pgvector/pgvector2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.764107 phidata-2.3.8/phi/vectordb/qdrant/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/vectordb/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/vectordb/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.764107 phidata-2.3.8/phi/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25334 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/workspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/workspace/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/workspace/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/workspace/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-01-29 15:46:19.000000 phidata-2.3.8/phi/workspace/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.764107 phidata-2.3.8/phidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29992 2024-01-29 15:46:37.000000 phidata-2.3.8/phidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13155 2024-01-29 15:46:37.000000 phidata-2.3.8/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 15:46:37.000000 phidata-2.3.8/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-29 15:46:37.000000 phidata-2.3.8/phidata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-29 15:46:37.000000 phidata-2.3.8/phidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-29 15:46:37.000000 phidata-2.3.8/phidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-01-29 15:46:19.000000 phidata-2.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 15:46:37.772107 phidata-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-29 15:46:19.000000 phidata-2.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:46:37.764107 phidata-2.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-29 15:46:19.000000 phidata-2.3.8/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.826252 phidata-2.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-01-30 14:43:57.000000 phidata-2.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    29985 2024-01-30 14:44:14.822251 phidata-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    28996 2024-01-30 14:43:57.000000 phidata-2.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.750252 phidata-2.3.9/phi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.750252 phidata-2.3.9/phi/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/ai/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/ai/phi_ai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.754252 phidata-2.3.9/phi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.754252 phidata-2.3.9/phi/api/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/schemas/ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/schemas/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/schemas/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/schemas/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.754252 phidata-2.3.9/phi/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/app/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/app/db_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/app/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.754252 phidata-2.3.9/phi/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34089 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.758252 phidata-2.3.9/phi/assistant/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12390 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/openai/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/openai/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.758252 phidata-2.3.9/phi/assistant/openai/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/openai/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/openai/file/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/openai/file/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/openai/file/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/openai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/openai/row.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/openai/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/openai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/assistant/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.758252 phidata-2.3.9/phi/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.758252 phidata-2.3.9/phi/aws/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34343 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/app/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.758252 phidata-2.3.9/phi/aws/app/django/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/app/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/app/django/django.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.758252 phidata-2.3.9/phi/aws/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.758252 phidata-2.3.9/phi/aws/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/app/jupyter/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.762252 phidata-2.3.9/phi/aws/app/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/app/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/app/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.762252 phidata-2.3.9/phi/aws/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.762252 phidata-2.3.9/phi/aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.762252 phidata-2.3.9/phi/aws/resource/acm/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/acm/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.762252 phidata-2.3.9/phi/aws/resource/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.762252 phidata-2.3.9/phi/aws/resource/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25483 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/ec2/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/ec2/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/ec2/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.762252 phidata-2.3.9/phi/aws/resource/ecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/ecs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/ecs/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19749 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/ecs/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23497 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/ecs/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.766252 phidata-2.3.9/phi/aws/resource/eks/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/eks/addon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31036 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13621 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23482 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/eks/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.766252 phidata-2.3.9/phi/aws/resource/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22351 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.766252 phidata-2.3.9/phi/aws/resource/elb/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/elb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/elb/target_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.766252 phidata-2.3.9/phi/aws/resource/emr/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/emr/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.766252 phidata-2.3.9/phi/aws/resource/glue/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/glue/crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.766252 phidata-2.3.9/phi/aws/resource/iam/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.766252 phidata-2.3.9/phi/aws/resource/rds/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42214 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36599 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/rds/db_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/rds/db_subnet_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.770252 phidata-2.3.9/phi/aws/resource/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/s3/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/s3/object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.770252 phidata-2.3.9/phi/aws/resource/secret/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/secret/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/secret/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31439 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/aws/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.770252 phidata-2.3.9/phi/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/cli/auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/cli/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20694 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/cli/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.770252 phidata-2.3.9/phi/cli/k/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/cli/k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/cli/k/k_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13585 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/cli/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/cli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.770252 phidata-2.3.9/phi/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27968 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/cli/ws/ws_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.770252 phidata-2.3.9/phi/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.770252 phidata-2.3.9/phi/docker/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.774252 phidata-2.3.9/phi/docker/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17444 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/airflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/airflow/flower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/airflow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/airflow/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/airflow/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.774252 phidata-2.3.9/phi/docker/app/django/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/django/django.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.774252 phidata-2.3.9/phi/docker/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.774252 phidata-2.3.9/phi/docker/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/jupyter/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.774252 phidata-2.3.9/phi/docker/app/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/mysql/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.774252 phidata-2.3.9/phi/docker/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/postgres/pgvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/postgres/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.774252 phidata-2.3.9/phi/docker/app/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.774252 phidata-2.3.9/phi/docker/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/redis/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.774252 phidata-2.3.9/phi/docker/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.778252 phidata-2.3.9/phi/docker/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/superset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/superset/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/superset/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/superset/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/superset/worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.778252 phidata-2.3.9/phi/docker/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/traefik/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.778252 phidata-2.3.9/phi/docker/app/whoami/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/whoami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/app/whoami/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.778252 phidata-2.3.9/phi/docker/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15995 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/resource/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/resource/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/resource/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31615 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/docker/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.778252 phidata-2.3.9/phi/document/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/document/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.778252 phidata-2.3.9/phi/document/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/document/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/document/reader/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/document/reader/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/document/reader/docx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/document/reader/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/document/reader/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.782252 phidata-2.3.9/phi/document/reader/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/document/reader/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/document/reader/s3/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/document/reader/s3/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/document/reader/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/document/reader/website.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.782252 phidata-2.3.9/phi/embedder/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/embedder/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/embedder/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.782252 phidata-2.3.9/phi/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.782252 phidata-2.3.9/phi/file/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/file/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/file/local/csv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.782252 phidata-2.3.9/phi/infra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/infra/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/infra/type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.782252 phidata-2.3.9/phi/k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.782252 phidata-2.3.9/phi/k8s/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.786252 phidata-2.3.9/phi/k8s/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14290 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/airflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/airflow/flower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/airflow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/airflow/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/airflow/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59184 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.786252 phidata-2.3.9/phi/k8s/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.786252 phidata-2.3.9/phi/k8s/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/jupyter/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.786252 phidata-2.3.9/phi/k8s/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/postgres/pgvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/postgres/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.786252 phidata-2.3.9/phi/k8s/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/redis/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.786252 phidata-2.3.9/phi/k8s/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.786252 phidata-2.3.9/phi/k8s/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/superset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/superset/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/superset/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/superset/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/superset/worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.786252 phidata-2.3.9/phi/k8s/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   115745 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/traefik/crds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13305 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/app/traefik/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.786252 phidata-2.3.9/phi/k8s/create/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.790252 phidata-2.3.9/phi/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.790252 phidata-2.3.9/phi/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.790252 phidata-2.3.9/phi/k8s/create/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.790252 phidata-2.3.9/phi/k8s/create/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.790252 phidata-2.3.9/phi/k8s/create/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/common/port.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.790252 phidata-2.3.9/phi/k8s/create/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.790252 phidata-2.3.9/phi/k8s/create/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.790252 phidata-2.3.9/phi/k8s/create/crb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/crb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/crb/eks_admin_crb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.790252 phidata-2.3.9/phi/k8s/create/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.794252 phidata-2.3.9/phi/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.794252 phidata-2.3.9/phi/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.794252 phidata-2.3.9/phi/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.794252 phidata-2.3.9/phi/k8s/create/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.794252 phidata-2.3.9/phi/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.794252 phidata-2.3.9/phi/k8s/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/enums/api_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/enums/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/enums/kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/enums/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/enums/pv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/enums/restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/enums/service_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/enums/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/enums/volume_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.794252 phidata-2.3.9/phi/k8s/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.794252 phidata-2.3.9/phi/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.798252 phidata-2.3.9/phi/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.798252 phidata-2.3.9/phi/k8s/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.798252 phidata-2.3.9/phi/k8s/resource/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10016 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.798252 phidata-2.3.9/phi/k8s/resource/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.802252 phidata-2.3.9/phi/k8s/resource/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18798 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20764 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.802252 phidata-2.3.9/phi/k8s/resource/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.802252 phidata-2.3.9/phi/k8s/resource/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.802252 phidata-2.3.9/phi/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.802252 phidata-2.3.9/phi/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.802252 phidata-2.3.9/phi/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.802252 phidata-2.3.9/phi/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.802252 phidata-2.3.9/phi/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.802252 phidata-2.3.9/phi/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resource/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44793 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/k8s/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.806252 phidata-2.3.9/phi/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/docx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.806252 phidata-2.3.9/phi/knowledge/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/s3/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/s3/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/s3/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/knowledge/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.806252 phidata-2.3.9/phi/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.806252 phidata-2.3.9/phi/llm/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/llm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14445 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/llm/aws/bedrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/llm/aws/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/llm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/llm/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.806252 phidata-2.3.9/phi/llm/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/llm/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35855 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/llm/openai/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/llm/references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.806252 phidata-2.3.9/phi/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/memory/assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.810252 phidata-2.3.9/phi/memory/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/memory/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/memory/task/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.810252 phidata-2.3.9/phi/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/resource/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.810252 phidata-2.3.9/phi/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.810252 phidata-2.3.9/phi/storage/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/storage/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/storage/assistant/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/storage/assistant/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/storage/assistant/sqllite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.810252 phidata-2.3.9/phi/table/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.810252 phidata-2.3.9/phi/table/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/table/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/table/sql/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.810252 phidata-2.3.9/phi/task/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/task/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.810252 phidata-2.3.9/phi/task/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/task/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31776 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/task/llm/llm_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.810252 phidata-2.3.9/phi/task/py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/task/py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/task/py/python_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.814252 phidata-2.3.9/phi/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14658 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.814252 phidata-2.3.9/phi/tools/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/fastapi/playground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/phi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.814252 phidata-2.3.9/phi/tools/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/streamlit/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/tool_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/tools/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.818251 phidata-2.3.9/phi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/format_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/merge_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/py_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/response_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/utils/yaml_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.818251 phidata-2.3.9/phi/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/vectordb/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/vectordb/distance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.822251 phidata-2.3.9/phi/vectordb/pgvector/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/vectordb/pgvector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/vectordb/pgvector/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13209 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/vectordb/pgvector/pgvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14839 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/vectordb/pgvector/pgvector2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.822251 phidata-2.3.9/phi/vectordb/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/vectordb/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/vectordb/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.822251 phidata-2.3.9/phi/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25334 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/workspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/workspace/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/workspace/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/workspace/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-01-30 14:43:57.000000 phidata-2.3.9/phi/workspace/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.822251 phidata-2.3.9/phidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29985 2024-01-30 14:44:14.000000 phidata-2.3.9/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13159 2024-01-30 14:44:14.000000 phidata-2.3.9/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 14:44:14.000000 phidata-2.3.9/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-30 14:44:14.000000 phidata-2.3.9/phidata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-30 14:44:14.000000 phidata-2.3.9/phidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-30 14:44:14.000000 phidata-2.3.9/phidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-01-30 14:43:57.000000 phidata-2.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 14:44:14.826252 phidata-2.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-30 14:43:57.000000 phidata-2.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:44:14.822251 phidata-2.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-30 14:43:57.000000 phidata-2.3.9/tests/test_placeholder.py
```

### Comparing `phidata-2.3.8/LICENSE` & `phidata-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/PKG-INFO` & `phidata-2.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.3.8
+Version: 2.3.9
 Summary: Build AI Assistants using language models
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: docker
 Requires-Dist: gitpython
 Requires-Dist: httpx
-Requires-Dist: pydantic==2.3.0
+Requires-Dist: pydantic
 Requires-Dist: pydantic-settings
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 Requires-Dist: rich
 Requires-Dist: tomli
 Requires-Dist: typer
 Requires-Dist: typing-extensions
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: phidata Version: 2.3.8 Summary: Build AI Assistants
+Metadata-Version: 2.1 Name: phidata Version: 2.3.9 Summary: Build AI Assistants
 using language models Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: boto3
 Requires-Dist: botocore Requires-Dist: docker Requires-Dist: gitpython
-Requires-Dist: httpx Requires-Dist: pydantic==2.3.0 Requires-Dist: pydantic-
-settings Requires-Dist: python-dotenv Requires-Dist: pyyaml Requires-Dist: rich
+Requires-Dist: httpx Requires-Dist: pydantic Requires-Dist: pydantic-settings
+Requires-Dist: python-dotenv Requires-Dist: pyyaml Requires-Dist: rich
 Requires-Dist: tomli Requires-Dist: typer Requires-Dist: typing-extensions
 Provides-Extra: dev Requires-Dist: mypy==v1.4.1; extra == "dev" Requires-Dist:
 black; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
 ruff; extra == "dev" Requires-Dist: types-pyyaml; extra == "dev" Provides-
 Extra: aws Requires-Dist: boto3; extra == "aws" Provides-Extra: k8s Requires-
 Dist: kubernetes; extra == "k8s"
                              ************ pphhiiddaattaa ************
```

### Comparing `phidata-2.3.8/README.md` & `phidata-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/ai/operator.py` & `phidata-2.3.9/phi/ai/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/ai/phi_ai.py` & `phidata-2.3.9/phi/ai/phi_ai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/api/ai.py` & `phidata-2.3.9/phi/api/ai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/api/api.py` & `phidata-2.3.9/phi/api/api.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/api/assistant.py` & `phidata-2.3.9/phi/api/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/api/llm.py` & `phidata-2.3.9/phi/api/llm.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/api/monitor.py` & `phidata-2.3.9/phi/api/monitor.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/api/routes.py` & `phidata-2.3.9/phi/api/routes.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/api/schemas/assistant.py` & `phidata-2.3.9/phi/api/schemas/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/api/schemas/workspace.py` & `phidata-2.3.9/phi/api/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/api/user.py` & `phidata-2.3.9/phi/api/user.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/api/workspace.py` & `phidata-2.3.9/phi/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/app/base.py` & `phidata-2.3.9/phi/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/app/context.py` & `phidata-2.3.9/phi/app/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/app/db_app.py` & `phidata-2.3.9/phi/app/db_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/app/group.py` & `phidata-2.3.9/phi/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/assistant/assistant.py` & `phidata-2.3.9/phi/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/assistant/custom.py` & `phidata-2.3.9/phi/assistant/custom.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/assistant/duckdb.py` & `phidata-2.3.9/phi/assistant/duckdb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/assistant/openai/assistant.py` & `phidata-2.3.9/phi/assistant/openai/assistant.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     description: Optional[str] = None
     # The system instructions that the assistant uses. The maximum length is 32768 characters.
     instructions: Optional[str] = None
 
     # -*- OpenAIAssistant Tools
     # A list of tools provided to the assistant. There can be a maximum of 128 tools per assistant.
     # Tools can be of types code_interpreter, retrieval, or function.
-    tools: Optional[List[Union[Tool, ToolRegistry, Callable, Dict]]] = None
+    tools: Optional[List[Union[Tool, ToolRegistry, Callable, Dict, Function]]] = None
     # -*- Functions available to the OpenAIAssistant to call
     # Functions extracted from the tools which can be executed locally by the assistant.
     functions: Optional[Dict[str, Function]] = None
 
     # -*- OpenAIAssistant Files
     # A list of file IDs attached to this assistant.
     # There can be a maximum of 20 files attached to the assistant.
@@ -96,14 +96,17 @@
         if self.tools is not None:
             for tool in self.tools:
                 if self.functions is None:
                     self.functions = {}
                 if isinstance(tool, ToolRegistry):
                     self.functions.update(tool.functions)
                     logger.debug(f"Functions from {tool.name} added to OpenAIAssistant.")
+                elif isinstance(tool, Function):
+                    self.functions[tool.name] = tool
+                    logger.debug(f"Function {tool.name} added to OpenAIAssistant.")
                 elif callable(tool):
                     f = Function.from_callable(tool)
                     self.functions[f.name] = f
                     logger.debug(f"Function {f.name} added to OpenAIAssistant")
         return self
 
     def __enter__(self):
@@ -131,14 +134,16 @@
                 tools_for_api.append(tool)
             elif callable(tool):
                 func = Function.from_callable(tool)
                 tools_for_api.append({"type": "function", "function": func.to_dict()})
             elif isinstance(tool, ToolRegistry):
                 for _f in tool.functions.values():
                     tools_for_api.append({"type": "function", "function": _f.to_dict()})
+            elif isinstance(tool, Function):
+                tools_for_api.append({"type": "function", "function": tool.to_dict()})
         return tools_for_api
 
     def create(self) -> "OpenAIAssistant":
         request_body: Dict[str, Any] = {}
         if self.name is not None:
             request_body["name"] = self.name
         if self.description is not None:
```

### Comparing `phidata-2.3.8/phi/assistant/openai/file/file.py` & `phidata-2.3.9/phi/assistant/openai/file/file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/assistant/openai/file/local.py` & `phidata-2.3.9/phi/assistant/openai/file/local.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/assistant/openai/file/url.py` & `phidata-2.3.9/phi/assistant/openai/file/url.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/assistant/openai/message.py` & `phidata-2.3.9/phi/assistant/openai/message.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/assistant/openai/row.py` & `phidata-2.3.9/phi/assistant/openai/row.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/assistant/openai/run.py` & `phidata-2.3.9/phi/assistant/openai/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     # If not, the model associated with the assistant will be used.
     model: Optional[str] = None
     # Override the default system message of the assistant.
     # This is useful for modifying the behavior on a per-run basis.
     instructions: Optional[str] = None
     # Override the tools the assistant can use for this run.
     # This is useful for modifying the behavior on a per-run basis.
-    tools: Optional[List[Union[Tool, ToolRegistry, Callable, Dict]]] = None
+    tools: Optional[List[Union[Tool, ToolRegistry, Callable, Dict, Function]]] = None
     # Functions extracted from the tools which can be executed locally by the assistant.
     functions: Optional[Dict[str, Function]] = None
 
     # The last error associated with this run. Will be null if there are no errors.
     last_error: Optional[LastError] = None
 
     # Set of 16 key-value pairs that can be attached to an object.
@@ -103,14 +103,17 @@
         if self.tools is not None:
             for tool in self.tools:
                 if self.functions is None:
                     self.functions = {}
                 if isinstance(tool, ToolRegistry):
                     self.functions.update(tool.functions)
                     logger.debug(f"Functions from {tool.name} added to OpenAIAssistant.")
+                elif isinstance(tool, Function):
+                    self.functions[tool.name] = tool
+                    logger.debug(f"Function {tool.name} added to OpenAIAssistant.")
                 elif callable(tool):
                     f = Function.from_callable(tool)
                     self.functions[f.name] = f
                     logger.debug(f"Function {f.name} added to OpenAIAssistant")
         return self
 
     def load_from_openai(self, openai_run: OpenAIRun):
@@ -140,14 +143,16 @@
                 tools_for_api.append(tool)
             elif callable(tool):
                 func = Function.from_callable(tool)
                 tools_for_api.append({"type": "function", "function": func.to_dict()})
             elif isinstance(tool, ToolRegistry):
                 for _f in tool.functions.values():
                     tools_for_api.append({"type": "function", "function": _f.to_dict()})
+            elif isinstance(tool, Function):
+                tools_for_api.append({"type": "function", "function": tool.to_dict()})
         return tools_for_api
 
     def create(
         self,
         thread_id: Optional[str] = None,
         assistant: Optional[OpenAIAssistant] = None,
         assistant_id: Optional[str] = None,
```

### Comparing `phidata-2.3.8/phi/assistant/openai/thread.py` & `phidata-2.3.9/phi/assistant/openai/thread.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/assistant/python.py` & `phidata-2.3.9/phi/assistant/python.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/assistant/run.py` & `phidata-2.3.9/phi/assistant/run.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/api_client.py` & `phidata-2.3.9/phi/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/app/base.py` & `phidata-2.3.9/phi/aws/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/app/django/django.py` & `phidata-2.3.9/phi/aws/app/django/django.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/app/fastapi/fastapi.py` & `phidata-2.3.9/phi/aws/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/app/jupyter/jupyter.py` & `phidata-2.3.9/phi/aws/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/app/qdrant/qdrant.py` & `phidata-2.3.9/phi/aws/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/app/streamlit/streamlit.py` & `phidata-2.3.9/phi/aws/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/acm/certificate.py` & `phidata-2.3.9/phi/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/base.py` & `phidata-2.3.9/phi/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/cloudformation/stack.py` & `phidata-2.3.9/phi/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/ec2/security_group.py` & `phidata-2.3.9/phi/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/ec2/subnet.py` & `phidata-2.3.9/phi/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/ec2/volume.py` & `phidata-2.3.9/phi/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/ecs/cluster.py` & `phidata-2.3.9/phi/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/ecs/container.py` & `phidata-2.3.9/phi/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/ecs/service.py` & `phidata-2.3.9/phi/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/ecs/task_definition.py` & `phidata-2.3.9/phi/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/ecs/volume.py` & `phidata-2.3.9/phi/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/eks/addon.py` & `phidata-2.3.9/phi/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/eks/cluster.py` & `phidata-2.3.9/phi/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/eks/fargate_profile.py` & `phidata-2.3.9/phi/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/eks/kubeconfig.py` & `phidata-2.3.9/phi/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/eks/node_group.py` & `phidata-2.3.9/phi/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/elasticache/cluster.py` & `phidata-2.3.9/phi/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/elasticache/subnet_group.py` & `phidata-2.3.9/phi/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/elb/listener.py` & `phidata-2.3.9/phi/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/elb/load_balancer.py` & `phidata-2.3.9/phi/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/elb/target_group.py` & `phidata-2.3.9/phi/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/emr/cluster.py` & `phidata-2.3.9/phi/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/glue/crawler.py` & `phidata-2.3.9/phi/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/iam/policy.py` & `phidata-2.3.9/phi/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/iam/role.py` & `phidata-2.3.9/phi/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/rds/db_cluster.py` & `phidata-2.3.9/phi/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/rds/db_instance.py` & `phidata-2.3.9/phi/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/rds/db_subnet_group.py` & `phidata-2.3.9/phi/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/s3/bucket.py` & `phidata-2.3.9/phi/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/s3/object.py` & `phidata-2.3.9/phi/aws/resource/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/secret/manager.py` & `phidata-2.3.9/phi/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/secret/reader.py` & `phidata-2.3.9/phi/aws/resource/secret/reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resource/types.py` & `phidata-2.3.9/phi/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/aws/resources.py` & `phidata-2.3.9/phi/aws/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/base.py` & `phidata-2.3.9/phi/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/cli/auth_server.py` & `phidata-2.3.9/phi/cli/auth_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/cli/config.py` & `phidata-2.3.9/phi/cli/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/cli/console.py` & `phidata-2.3.9/phi/cli/console.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/cli/credentials.py` & `phidata-2.3.9/phi/cli/credentials.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/cli/entrypoint.py` & `phidata-2.3.9/phi/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/cli/k/k_cli.py` & `phidata-2.3.9/phi/cli/k/k_cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/cli/operator.py` & `phidata-2.3.9/phi/cli/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/cli/settings.py` & `phidata-2.3.9/phi/cli/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/cli/ws/ws_cli.py` & `phidata-2.3.9/phi/cli/ws/ws_cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/constants.py` & `phidata-2.3.9/phi/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/api_client.py` & `phidata-2.3.9/phi/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/app/airflow/base.py` & `phidata-2.3.9/phi/docker/app/airflow/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/app/airflow/worker.py` & `phidata-2.3.9/phi/docker/app/airflow/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/app/base.py` & `phidata-2.3.9/phi/docker/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/app/django/django.py` & `phidata-2.3.9/phi/docker/app/django/django.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/app/fastapi/fastapi.py` & `phidata-2.3.9/phi/docker/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/app/jupyter/jupyter.py` & `phidata-2.3.9/phi/docker/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/app/mysql/mysql.py` & `phidata-2.3.9/phi/docker/app/mysql/mysql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/app/postgres/postgres.py` & `phidata-2.3.9/phi/docker/app/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/app/qdrant/qdrant.py` & `phidata-2.3.9/phi/docker/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/app/redis/redis.py` & `phidata-2.3.9/phi/docker/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/app/streamlit/streamlit.py` & `phidata-2.3.9/phi/docker/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/app/superset/base.py` & `phidata-2.3.9/phi/docker/app/superset/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/app/traefik/router.py` & `phidata-2.3.9/phi/docker/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/resource/base.py` & `phidata-2.3.9/phi/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/resource/container.py` & `phidata-2.3.9/phi/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/resource/image.py` & `phidata-2.3.9/phi/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/resource/network.py` & `phidata-2.3.9/phi/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/resource/types.py` & `phidata-2.3.9/phi/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/resource/volume.py` & `phidata-2.3.9/phi/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/docker/resources.py` & `phidata-2.3.9/phi/docker/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/document/base.py` & `phidata-2.3.9/phi/document/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/document/reader/arxiv.py` & `phidata-2.3.9/phi/document/reader/arxiv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/document/reader/base.py` & `phidata-2.3.9/phi/document/reader/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,18 +57,24 @@
             # If the end is greater than the content length, then set it to the content length
             if end > content_length:
                 end = content_length
 
             chunk = cleaned_content[start:end]
             meta_data = chunk_meta_data.copy()
             meta_data["chunk"] = chunk_number
+            chunk_id = None
+            if document.id:
+                chunk_id = f"{document.id}_{chunk_number}"
+            elif document.name:
+                chunk_id = f"{document.name}_{chunk_number}"
             meta_data["chunk_size"] = len(chunk)
             chunked_documents.append(
                 Document(
-                    content=chunk,
+                    id=chunk_id,
                     name=document.name,
                     meta_data=meta_data,
+                    content=chunk,
                 )
             )
             chunk_number += 1
             start = end
         return chunked_documents
```

### Comparing `phidata-2.3.8/phi/document/reader/docx.py` & `phidata-2.3.9/phi/document/reader/docx.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/document/reader/json.py` & `phidata-2.3.9/phi/document/reader/json.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/document/reader/pdf.py` & `phidata-2.3.9/phi/document/reader/pdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
         logger.info(f"Reading: {doc_name}")
         doc_reader = DocumentReader(pdf)
 
         documents = [
             Document(
                 name=doc_name,
+                id=f"{doc_name}_{page_number}",
                 meta_data={"page": page_number},
                 content=page.extract_text(),
             )
             for page_number, page in enumerate(doc_reader.pages, start=1)
         ]
         if self.chunk:
             chunked_documents = []
```

### Comparing `phidata-2.3.8/phi/document/reader/s3/pdf.py` & `phidata-2.3.9/phi/document/reader/s3/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/document/reader/s3/text.py` & `phidata-2.3.9/phi/document/reader/s3/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/document/reader/text.py` & `phidata-2.3.9/phi/document/reader/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/document/reader/website.py` & `phidata-2.3.9/phi/document/reader/website.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/embedder/openai.py` & `phidata-2.3.9/phi/embedder/openai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/file/local/csv.py` & `phidata-2.3.9/phi/file/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/infra/resources.py` & `phidata-2.3.9/phi/infra/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/api_client.py` & `phidata-2.3.9/phi/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/app/airflow/base.py` & `phidata-2.3.9/phi/k8s/app/airflow/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/app/airflow/worker.py` & `phidata-2.3.9/phi/k8s/app/airflow/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/app/base.py` & `phidata-2.3.9/phi/k8s/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/app/fastapi/fastapi.py` & `phidata-2.3.9/phi/k8s/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/app/jupyter/jupyter.py` & `phidata-2.3.9/phi/k8s/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/app/postgres/postgres.py` & `phidata-2.3.9/phi/k8s/app/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/app/redis/redis.py` & `phidata-2.3.9/phi/k8s/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/app/streamlit/streamlit.py` & `phidata-2.3.9/phi/k8s/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/app/superset/base.py` & `phidata-2.3.9/phi/k8s/app/superset/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/app/traefik/crds.py` & `phidata-2.3.9/phi/k8s/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/app/traefik/router.py` & `phidata-2.3.9/phi/k8s/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.3.9/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.3.9/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/apps/v1/deployment.py` & `phidata-2.3.9/phi/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/base.py` & `phidata-2.3.9/phi/k8s/create/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/common/port.py` & `phidata-2.3.9/phi/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/core/v1/config_map.py` & `phidata-2.3.9/phi/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/core/v1/container.py` & `phidata-2.3.9/phi/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/core/v1/namespace.py` & `phidata-2.3.9/phi/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/core/v1/persistent_volume.py` & `phidata-2.3.9/phi/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-2.3.9/phi/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/core/v1/secret.py` & `phidata-2.3.9/phi/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/core/v1/service.py` & `phidata-2.3.9/phi/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/core/v1/service_account.py` & `phidata-2.3.9/phi/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/core/v1/volume.py` & `phidata-2.3.9/phi/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/crb/eks_admin_crb.py` & `phidata-2.3.9/phi/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-2.3.9/phi/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.3.9/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.3.9/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-2.3.9/phi/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/enums/api_version.py` & `phidata-2.3.9/phi/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/enums/kind.py` & `phidata-2.3.9/phi/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/enums/pv.py` & `phidata-2.3.9/phi/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/operator.py` & `phidata-2.3.9/phi/k8s/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.3.9/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.3.9/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/apps/v1/deployment.py` & `phidata-2.3.9/phi/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-2.3.9/phi/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/base.py` & `phidata-2.3.9/phi/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/config_map.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/container.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/local_object_reference.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/namespace.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/node_selector.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/object_reference.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/persistent_volume.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/pod.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/pod_spec.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/pod_template_spec.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/resource_requirements.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/secret.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/service.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/service_account.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/toleration.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/volume.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/core/v1/volume_source.py` & `phidata-2.3.9/phi/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/kubeconfig.py` & `phidata-2.3.9/phi/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/meta/v1/label_selector.py` & `phidata-2.3.9/phi/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/meta/v1/object_meta.py` & `phidata-2.3.9/phi/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-2.3.9/phi/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.3.9/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.3.9/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-2.3.9/phi/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/types.py` & `phidata-2.3.9/phi/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resource/yaml.py` & `phidata-2.3.9/phi/k8s/resource/yaml.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/k8s/resources.py` & `phidata-2.3.9/phi/k8s/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/arxiv.py` & `phidata-2.3.9/phi/knowledge/arxiv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/base.py` & `phidata-2.3.9/phi/knowledge/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/combined.py` & `phidata-2.3.9/phi/knowledge/combined.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/document.py` & `phidata-2.3.9/phi/knowledge/document.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/docx.py` & `phidata-2.3.9/phi/knowledge/docx.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/json.py` & `phidata-2.3.9/phi/knowledge/json.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/langchain.py` & `phidata-2.3.9/phi/knowledge/langchain.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/pdf.py` & `phidata-2.3.9/phi/knowledge/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/s3/base.py` & `phidata-2.3.9/phi/knowledge/s3/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/s3/pdf.py` & `phidata-2.3.9/phi/knowledge/s3/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/s3/text.py` & `phidata-2.3.9/phi/knowledge/s3/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/text.py` & `phidata-2.3.9/phi/knowledge/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/website.py` & `phidata-2.3.9/phi/knowledge/website.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/knowledge/wikipedia.py` & `phidata-2.3.9/phi/knowledge/wikipedia.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/llm/aws/bedrock.py` & `phidata-2.3.9/phi/llm/aws/bedrock.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/llm/aws/claude.py` & `phidata-2.3.9/phi/llm/aws/claude.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/llm/base.py` & `phidata-2.3.9/phi/llm/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/llm/message.py` & `phidata-2.3.9/phi/llm/message.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/llm/openai/chat.py` & `phidata-2.3.9/phi/llm/openai/chat.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/memory/assistant.py` & `phidata-2.3.9/phi/memory/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/memory/task/llm.py` & `phidata-2.3.9/phi/memory/task/llm.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/resource/base.py` & `phidata-2.3.9/phi/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/resource/group.py` & `phidata-2.3.9/phi/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/storage/assistant/base.py` & `phidata-2.3.9/phi/storage/assistant/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/storage/assistant/postgres.py` & `phidata-2.3.9/phi/storage/assistant/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/storage/assistant/sqllite.py` & `phidata-2.3.9/phi/storage/assistant/sqllite.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/task/decorator.py` & `phidata-2.3.9/phi/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/task/llm/llm_task.py` & `phidata-2.3.9/phi/task/llm/llm_task.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/task/py/python_task.py` & `phidata-2.3.9/phi/task/py/python_task.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/task/task.py` & `phidata-2.3.9/phi/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/airflow.py` & `phidata-2.3.9/phi/tools/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/arxiv.py` & `phidata-2.3.9/phi/tools/arxiv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/duckdb.py` & `phidata-2.3.9/phi/tools/duckdb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/email.py` & `phidata-2.3.9/phi/tools/email.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/file.py` & `phidata-2.3.9/phi/tools/file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/function.py` & `phidata-2.3.9/phi/tools/function.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/google.py` & `phidata-2.3.9/phi/tools/google.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/pandas.py` & `phidata-2.3.9/phi/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/phi.py` & `phidata-2.3.9/phi/tools/phi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/python.py` & `phidata-2.3.9/phi/tools/python.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/shell.py` & `phidata-2.3.9/phi/tools/shell.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/streamlit/components.py` & `phidata-2.3.9/phi/tools/streamlit/components.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/tool_registry.py` & `phidata-2.3.9/phi/tools/tool_registry.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/website.py` & `phidata-2.3.9/phi/tools/website.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/tools/wikipedia.py` & `phidata-2.3.9/phi/tools/wikipedia.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/common.py` & `phidata-2.3.9/phi/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/defaults.py` & `phidata-2.3.9/phi/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/enum.py` & `phidata-2.3.9/phi/utils/enum.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/filesystem.py` & `phidata-2.3.9/phi/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/functions.py` & `phidata-2.3.9/phi/utils/functions.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/git.py` & `phidata-2.3.9/phi/utils/git.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/json_io.py` & `phidata-2.3.9/phi/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/json_schema.py` & `phidata-2.3.9/phi/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/load_env.py` & `phidata-2.3.9/phi/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/log.py` & `phidata-2.3.9/phi/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/merge_dict.py` & `phidata-2.3.9/phi/utils/merge_dict.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/message.py` & `phidata-2.3.9/phi/utils/message.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/pickle.py` & `phidata-2.3.9/phi/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/py_io.py` & `phidata-2.3.9/phi/utils/py_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/pyproject.py` & `phidata-2.3.9/phi/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/resource_filter.py` & `phidata-2.3.9/phi/utils/resource_filter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/timer.py` & `phidata-2.3.9/phi/utils/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/utils/yaml_io.py` & `phidata-2.3.9/phi/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/vectordb/base.py` & `phidata-2.3.9/phi/vectordb/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/vectordb/pgvector/pgvector.py` & `phidata-2.3.9/phi/vectordb/pgvector/pgvector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/vectordb/pgvector/pgvector2.py` & `phidata-2.3.9/phi/vectordb/pgvector/pgvector2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, List, Union
+from typing import Optional, List, Union, Dict, Any
 from hashlib import md5
 
 try:
     from sqlalchemy.dialects import postgresql
     from sqlalchemy.engine import create_engine, Engine
     from sqlalchemy.inspection import inspect
     from sqlalchemy.orm import Session, sessionmaker
@@ -228,29 +228,35 @@
                     counter = 0
 
             # Commit any remaining documents
             if counter > 0:
                 sess.commit()
                 logger.debug(f"Committed {counter} documents")
 
-    def search(self, query: str, limit: int = 5) -> List[Document]:
+    def search(self, query: str, limit: int = 5, filters: Optional[Dict[str, Any]] = None) -> List[Document]:
         query_embedding = self.embedder.get_embedding(query)
         if query_embedding is None:
             logger.error(f"Error getting embedding for Query: {query}")
             return []
 
         columns = [
             self.table.c.name,
             self.table.c.meta_data,
             self.table.c.content,
             self.table.c.embedding,
             self.table.c.usage,
         ]
 
         stmt = select(*columns)
+
+        if filters is not None:
+            for key, value in filters.items():
+                if hasattr(self.table.c, key):
+                    stmt = stmt.where(getattr(self.table.c, key) == value)
+
         if self.distance == Distance.l2:
             stmt = stmt.order_by(self.table.c.embedding.max_inner_product(query_embedding))
         if self.distance == Distance.cosine:
             stmt = stmt.order_by(self.table.c.embedding.cosine_distance(query_embedding))
         if self.distance == Distance.max_inner_product:
             stmt = stmt.order_by(self.table.c.embedding.max_inner_product(query_embedding))
```

### Comparing `phidata-2.3.8/phi/vectordb/qdrant/qdrant.py` & `phidata-2.3.9/phi/vectordb/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/workspace/config.py` & `phidata-2.3.9/phi/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/workspace/helpers.py` & `phidata-2.3.9/phi/workspace/helpers.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/workspace/operator.py` & `phidata-2.3.9/phi/workspace/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phi/workspace/settings.py` & `phidata-2.3.9/phi/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.8/phidata.egg-info/PKG-INFO` & `phidata-2.3.9/phidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.3.8
+Version: 2.3.9
 Summary: Build AI Assistants using language models
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: docker
 Requires-Dist: gitpython
 Requires-Dist: httpx
-Requires-Dist: pydantic==2.3.0
+Requires-Dist: pydantic
 Requires-Dist: pydantic-settings
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 Requires-Dist: rich
 Requires-Dist: tomli
 Requires-Dist: typer
 Requires-Dist: typing-extensions
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: phidata Version: 2.3.8 Summary: Build AI Assistants
+Metadata-Version: 2.1 Name: phidata Version: 2.3.9 Summary: Build AI Assistants
 using language models Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: boto3
 Requires-Dist: botocore Requires-Dist: docker Requires-Dist: gitpython
-Requires-Dist: httpx Requires-Dist: pydantic==2.3.0 Requires-Dist: pydantic-
-settings Requires-Dist: python-dotenv Requires-Dist: pyyaml Requires-Dist: rich
+Requires-Dist: httpx Requires-Dist: pydantic Requires-Dist: pydantic-settings
+Requires-Dist: python-dotenv Requires-Dist: pyyaml Requires-Dist: rich
 Requires-Dist: tomli Requires-Dist: typer Requires-Dist: typing-extensions
 Provides-Extra: dev Requires-Dist: mypy==v1.4.1; extra == "dev" Requires-Dist:
 black; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
 ruff; extra == "dev" Requires-Dist: types-pyyaml; extra == "dev" Provides-
 Extra: aws Requires-Dist: boto3; extra == "aws" Provides-Extra: k8s Requires-
 Dist: kubernetes; extra == "k8s"
                              ************ pphhiiddaattaa ************
```

### Comparing `phidata-2.3.8/phidata.egg-info/SOURCES.txt` & `phidata-2.3.9/phidata.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 phi/tools/python.py
 phi/tools/shell.py
 phi/tools/tool.py
 phi/tools/tool_registry.py
 phi/tools/website.py
 phi/tools/wikipedia.py
 phi/tools/fastapi/__init__.py
-phi/tools/fastapi/routes.py
+phi/tools/fastapi/playground.py
 phi/tools/streamlit/__init__.py
 phi/tools/streamlit/components.py
 phi/utils/__init__.py
 phi/utils/common.py
 phi/utils/defaults.py
 phi/utils/dttm.py
 phi/utils/enum.py
```

### Comparing `phidata-2.3.8/pyproject.toml` & `phidata-2.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "phidata"
-version = "2.3.8"
+version = "2.3.9"
 description = "Build AI Assistants using language models"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
   "boto3",
   "botocore",
   "docker",
   "gitpython",
   "httpx",
-  "pydantic==2.3.0",
+  "pydantic",
   "pydantic-settings",
   "python-dotenv",
   "pyyaml",
   "rich",
   "tomli",
   "typer",
   "typing-extensions",
```

