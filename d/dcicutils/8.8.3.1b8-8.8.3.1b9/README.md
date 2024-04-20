# Comparing `tmp/dcicutils-8.8.3.1b8.tar.gz` & `tmp/dcicutils-8.8.3.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-8.8.3.1b8.tar", max compression
+gzip compressed data, was "dcicutils-8.8.3.1b9.tar", max compression
```

## Comparing `dcicutils-8.8.3.1b8.tar` & `dcicutils-8.8.3.1b9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1102 2024-04-15 18:33:13.340207 dcicutils-8.8.3.1b8/LICENSE.txt
--rw-r--r--   0        0        0     1166 2024-04-15 18:33:13.340207 dcicutils-8.8.3.1b8/README.rst
--rw-r--r--   0        0        0        0 2024-04-15 18:33:13.340207 dcicutils-8.8.3.1b8/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2024-04-15 18:33:13.340207 dcicutils-8.8.3.1b8/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2024-04-15 18:33:13.340207 dcicutils-8.8.3.1b8/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    34669 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/bundle_utils.py
--rw-r--r--   0        0        0     3108 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/captured_output.py
--rw-r--r--   0        0        0    13786 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3955 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     7414 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/data_readers.py
--rw-r--r--   0        0        0     3098 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/data_utils.py
--rw-r--r--   0        0        0     4666 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/datetime_utils.py
--rw-r--r--   0        0        0    69908 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    72972 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     2663 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/file_utils.py
--rw-r--r--   0        0        0    10026 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    34149 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    28151 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/lang_utils.py
--rw-r--r--   0        0        0      278 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/license_policies/c4-infrastructure.jsonc
--rw-r--r--   0        0        0      296 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/license_policies/c4-python-infrastructure.jsonc
--rw-r--r--   0        0        0     5790 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/license_policies/park-lab-common-server.jsonc
--rw-r--r--   0        0        0    18864 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/license_policies/park-lab-common.jsonc
--rw-r--r--   0        0        0     3260 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
--rw-r--r--   0        0        0      283 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/license_policies/park-lab-pipeline.jsonc
--rw-r--r--   0        0        0    46978 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/log_utils.py
--rw-r--r--   0        0        0   103041 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    15422 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/portal_object_utils.py
--rw-r--r--   0        0        0    30480 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/portal_utils.py
--rw-r--r--   0        0        0    16569 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/progress_bar.py
--rw-r--r--   0        0        0    31250 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20534 2024-04-15 18:33:13.344207 dcicutils-8.8.3.1b8/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   160208 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     7055 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28868 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    10095 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/schema_utils.py
--rw-r--r--   0        0        0    13889 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0     4184 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/scripts/run_license_checker.py
--rw-r--r--   0        0        0    26262 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/scripts/view_portal_object.py
--rw-r--r--   0        0        0    19745 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    33629 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/sheet_utils.py
--rw-r--r--   0        0        0    22961 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0    59927 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/structured_data.py
--rw-r--r--   0        0        0     2895 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/submitr/progress_constants.py
--rw-r--r--   0        0        0     3467 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/submitr/ref_lookup_strategy.py
--rw-r--r--   0        0        0     8082 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1403 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/tmpfile_utils.py
--rw-r--r--   0        0        0     1769 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/trace_utils.py
--rw-r--r--   0        0        0    14797 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/validation_utils.py
--rw-r--r--   0        0        0     4343 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/variant_utils.py
--rw-r--r--   0        0        0     2027 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/dcicutils/zip_utils.py
--rw-r--r--   0        0        0     4714 2024-04-15 18:33:13.348207 dcicutils-8.8.3.1b8/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.3.1b8/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/README.rst
+-rw-r--r--   0        0        0        0 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    34669 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/bundle_utils.py
+-rw-r--r--   0        0        0     3108 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/captured_output.py
+-rw-r--r--   0        0        0    13786 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3955 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     7414 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/data_readers.py
+-rw-r--r--   0        0        0     3098 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/data_utils.py
+-rw-r--r--   0        0        0     4666 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/datetime_utils.py
+-rw-r--r--   0        0        0    69908 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2024-04-16 12:36:50.786350 dcicutils-8.8.3.1b9/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    72972 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     2663 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/file_utils.py
+-rw-r--r--   0        0        0    10026 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    34149 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    28151 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0      278 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/license_policies/c4-infrastructure.jsonc
+-rw-r--r--   0        0        0      296 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/license_policies/c4-python-infrastructure.jsonc
+-rw-r--r--   0        0        0     5790 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/license_policies/park-lab-common-server.jsonc
+-rw-r--r--   0        0        0    18864 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/license_policies/park-lab-common.jsonc
+-rw-r--r--   0        0        0     3260 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
+-rw-r--r--   0        0        0      283 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/license_policies/park-lab-pipeline.jsonc
+-rw-r--r--   0        0        0    46978 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/log_utils.py
+-rw-r--r--   0        0        0   103041 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    15422 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/portal_object_utils.py
+-rw-r--r--   0        0        0    30480 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/portal_utils.py
+-rw-r--r--   0        0        0    17007 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/progress_bar.py
+-rw-r--r--   0        0        0    31250 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20534 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   160208 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     7055 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28868 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    10095 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/schema_utils.py
+-rw-r--r--   0        0        0    13889 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0     4184 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/scripts/run_license_checker.py
+-rw-r--r--   0        0        0    26262 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/scripts/view_portal_object.py
+-rw-r--r--   0        0        0    19745 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    33629 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/sheet_utils.py
+-rw-r--r--   0        0        0    22961 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2024-04-16 12:36:50.790350 dcicutils-8.8.3.1b9/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0    59927 2024-04-16 12:36:50.794350 dcicutils-8.8.3.1b9/dcicutils/structured_data.py
+-rw-r--r--   0        0        0     2895 2024-04-16 12:36:50.794350 dcicutils-8.8.3.1b9/dcicutils/submitr/progress_constants.py
+-rw-r--r--   0        0        0     3467 2024-04-16 12:36:50.794350 dcicutils-8.8.3.1b9/dcicutils/submitr/ref_lookup_strategy.py
+-rw-r--r--   0        0        0     8082 2024-04-16 12:36:50.794350 dcicutils-8.8.3.1b9/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1403 2024-04-16 12:36:50.794350 dcicutils-8.8.3.1b9/dcicutils/tmpfile_utils.py
+-rw-r--r--   0        0        0     1769 2024-04-16 12:36:50.794350 dcicutils-8.8.3.1b9/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0    14797 2024-04-16 12:36:50.794350 dcicutils-8.8.3.1b9/dcicutils/validation_utils.py
+-rw-r--r--   0        0        0     4343 2024-04-16 12:36:50.794350 dcicutils-8.8.3.1b9/dcicutils/variant_utils.py
+-rw-r--r--   0        0        0     2027 2024-04-16 12:36:50.794350 dcicutils-8.8.3.1b9/dcicutils/zip_utils.py
+-rw-r--r--   0        0        0     4714 2024-04-16 12:36:50.794350 dcicutils-8.8.3.1b9/pyproject.toml
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.3.1b9/PKG-INFO
```

### Comparing `dcicutils-8.8.3.1b8/LICENSE.txt` & `dcicutils-8.8.3.1b9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/README.rst` & `dcicutils-8.8.3.1b9/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/base.py` & `dcicutils-8.8.3.1b9/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/beanstalk_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/bundle_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/captured_output.py` & `dcicutils-8.8.3.1b9/dcicutils/captured_output.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/cloudformation_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/codebuild_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/command_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/common.py` & `dcicutils-8.8.3.1b9/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/contribution_scripts.py` & `dcicutils-8.8.3.1b9/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/contribution_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/creds_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/data_readers.py` & `dcicutils-8.8.3.1b9/dcicutils/data_readers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/data_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/datetime_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/deployment_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/diff_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/docker_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/ecr_scripts.py` & `dcicutils-8.8.3.1b9/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/ecr_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/ecs_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/env_base.py` & `dcicutils-8.8.3.1b9/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/env_manager.py` & `dcicutils-8.8.3.1b9/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/env_scripts.py` & `dcicutils-8.8.3.1b9/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/env_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/env_utils_legacy.py` & `dcicutils-8.8.3.1b9/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/es_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/exceptions.py` & `dcicutils-8.8.3.1b9/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/ff_mocks.py` & `dcicutils-8.8.3.1b9/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/ff_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/file_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/function_cache_decorator.py` & `dcicutils-8.8.3.1b9/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/glacier_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/jh_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/kibana/dashboards.json` & `dcicutils-8.8.3.1b9/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/kibana/readme.md` & `dcicutils-8.8.3.1b9/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/lang_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/license_policies/park-lab-common-server.jsonc` & `dcicutils-8.8.3.1b9/dcicutils/license_policies/park-lab-common-server.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/license_policies/park-lab-common.jsonc` & `dcicutils-8.8.3.1b9/dcicutils/license_policies/park-lab-common.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc` & `dcicutils-8.8.3.1b9/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/license_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/log_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/misc_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/obfuscation_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/opensearch_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/portal_object_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/portal_object_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/portal_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/portal_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/progress_bar.py` & `dcicutils-8.8.3.1b9/dcicutils/progress_bar.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,55 +102,63 @@
             self._bar = TQDM(total=self._total, desc=self._description,
                              dynamic_ncols=True, bar_format=bar_format, unit="", file=sys.stdout)
             if self._disabled:
                 self._bar.disable = True
             return True
         return False
 
-    def set_total(self, value: int) -> None:
+    def set_total(self, value: int, _norefresh: bool = False) -> None:
         if value == self._total:
             # If the total has not changed since last set then do nothing.
             return
         if isinstance(value, int) and value > 0:
             self._total = value
             if self._bar is not None:
                 # This reset is needed to get the ETA to reset properly when we reset
                 # the total during the course of a single ProgressBar instance.
                 self._bar.reset()
                 self._bar.total = value
-                self._bar.refresh()
+                if not _norefresh:
+                    self._bar.refresh()
 
-    def set_progress(self, value: int) -> None:
+    def set_progress(self, value: int, _norefresh: bool = False) -> None:
         if isinstance(value, int) and value >= 0:
             if (self._bar is not None) or self._initialize():
                 self._bar.n = value
-                self._bar.refresh()
+                if not _norefresh:
+                    self._bar.refresh()
 
     def increment_progress(self, value: int) -> None:
         if isinstance(value, int) and value > 0:
             if (self._bar is not None) or self._initialize():
                 self._bar.update(value)
                 self._bar.refresh()
 
+    def set_description(self, value: str) -> None:
+        if isinstance(value, str):
+            self._description = self._format_description(value)
+            if self._bar is not None:
+                # FYI: tqdm.set_description seems to imply a refresh.
+                self._bar.set_description(self._description)
+
     def reset_eta(self) -> None:
         # Since set_total does nothing if total is the same, provide
         # a way to reset the ETA if starting over with the same total.
         # But NOTE that resetting ETA will ALSO reset the ELAPSED time.
         if self._bar is not None:
             progress = self._bar.n
             self._bar.reset()
             self._bar.total = self._total
             self._bar.n = progress
             self._bar.refresh()
 
-    def set_description(self, value: str) -> None:
-        if isinstance(value, str):
-            self._description = self._format_description(value)
-            if self._bar is not None:
-                self._bar.set_description(self._description)
+    def reset(self, total: int, progress: int = 0, description: Optional[str] = None) -> None:
+        self.set_total(total, _norefresh=True)
+        self.set_progress(progress, _norefresh=True)
+        self.set_description(description)
 
     def done(self, description: Optional[str] = None) -> None:
         if self._done or self._bar is None:
             return
         self._ended = time.time()
         self.set_progress(self.total)
         self.set_description(description)
```

### Comparing `dcicutils-8.8.3.1b8/dcicutils/project_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/qa_checkers.py` & `dcicutils-8.8.3.1b9/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/qa_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/redis_tools.py` & `dcicutils-8.8.3.1b9/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/redis_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/s3_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/schema_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-8.8.3.1b9/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/scripts/run_license_checker.py` & `dcicutils-8.8.3.1b9/dcicutils/scripts/run_license_checker.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/scripts/view_portal_object.py` & `dcicutils-8.8.3.1b9/dcicutils/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/secrets_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/sheet_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/sheet_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/snapshot_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/ssl_certificate_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/structured_data.py` & `dcicutils-8.8.3.1b9/dcicutils/structured_data.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/submitr/progress_constants.py` & `dcicutils-8.8.3.1b9/dcicutils/submitr/progress_constants.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/submitr/ref_lookup_strategy.py` & `dcicutils-8.8.3.1b9/dcicutils/submitr/ref_lookup_strategy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/task_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/tmpfile_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/tmpfile_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/trace_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/validation_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/variant_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/variant_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/dcicutils/zip_utils.py` & `dcicutils-8.8.3.1b9/dcicutils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b8/pyproject.toml` & `dcicutils-8.8.3.1b9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "8.8.3.1b8"  # TODO: To become 8.8.4
+version = "8.8.3.1b9"  # TODO: To become 8.8.4
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-8.8.3.1b8/PKG-INFO` & `dcicutils-8.8.3.1b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 8.8.3.1b8
+Version: 8.8.3.1b9
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
```

