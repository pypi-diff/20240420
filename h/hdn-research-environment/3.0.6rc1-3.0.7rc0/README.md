# Comparing `tmp/hdn-research-environment-3.0.6rc1.tar.gz` & `tmp/hdn-research-environment-3.0.7rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdn-research-environment-3.0.6rc1.tar", last modified: Tue Apr 16 13:27:30 2024, max compression
+gzip compressed data, was "hdn-research-environment-3.0.7rc0.tar", last modified: Wed Apr 10 10:04:39 2024, max compression
```

## Comparing `hdn-research-environment-3.0.6rc1.tar` & `hdn-research-environment-3.0.7rc0.tar`

### file list

```diff
@@ -1,107 +1,106 @@
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.315404 hdn-research-environment-3.0.6rc1/
--rw-r--r--   0 rafal      (501) staff       (20)     1551 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6rc1/LICENSE
--rw-r--r--   0 rafal      (501) staff       (20)      115 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6rc1/MANIFEST.in
--rw-r--r--   0 rafal      (501) staff       (20)      981 2024-04-16 13:27:30.315525 hdn-research-environment-3.0.6rc1/PKG-INFO
--rw-r--r--   0 rafal      (501) staff       (20)      229 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/README.md
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.297506 hdn-research-environment-3.0.6rc1/environment/
--rw-r--r--   0 rafal      (501) staff       (20)        0 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6rc1/environment/__init__.py
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.298184 hdn-research-environment-3.0.6rc1/environment/api/
--rw-r--r--   0 rafal      (501) staff       (20)     8203 2024-03-26 11:53:16.000000 hdn-research-environment-3.0.6rc1/environment/api/__init__.py
--rw-r--r--   0 rafal      (501) staff       (20)      939 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/api/decorators.py
--rw-r--r--   0 rafal      (501) staff       (20)      154 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6rc1/environment/apps.py
--rw-r--r--   0 rafal      (501) staff       (20)     4179 2024-04-16 13:25:47.000000 hdn-research-environment-3.0.6rc1/environment/constants.py
--rw-r--r--   0 rafal      (501) staff       (20)     1546 2024-02-16 14:02:50.000000 hdn-research-environment-3.0.6rc1/environment/decorators.py
--rw-r--r--   0 rafal      (501) staff       (20)     5362 2024-02-29 13:11:14.000000 hdn-research-environment-3.0.6rc1/environment/deserializers.py
--rw-r--r--   0 rafal      (501) staff       (20)     4724 2024-04-16 13:25:47.000000 hdn-research-environment-3.0.6rc1/environment/entities.py
--rw-r--r--   0 rafal      (501) staff       (20)     1421 2024-01-29 13:36:38.000000 hdn-research-environment-3.0.6rc1/environment/exceptions.py
--rw-r--r--   0 rafal      (501) staff       (20)     8008 2024-04-16 13:25:47.000000 hdn-research-environment-3.0.6rc1/environment/forms.py
--rw-r--r--   0 rafal      (501) staff       (20)     2518 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/mailers.py
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.301983 hdn-research-environment-3.0.6rc1/environment/migrations/
--rw-r--r--   0 rafal      (501) staff       (20)     2174 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/migrations/00012_bucketsharinginvite.py
--rw-r--r--   0 rafal      (501) staff       (20)     1443 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/migrations/0001_initial.py
--rw-r--r--   0 rafal      (501) staff       (20)     1579 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 rafal      (501) staff       (20)      403 2023-05-16 11:52:08.000000 hdn-research-environment-3.0.6rc1/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 rafal      (501) staff       (20)      420 2023-05-16 11:52:08.000000 hdn-research-environment-3.0.6rc1/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 rafal      (501) staff       (20)     2220 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/migrations/0005_workflow.py
--rw-r--r--   0 rafal      (501) staff       (20)      394 2023-05-26 09:35:04.000000 hdn-research-environment-3.0.6rc1/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 rafal      (501) staff       (20)     2348 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 rafal      (501) staff       (20)      476 2023-05-29 14:50:53.000000 hdn-research-environment-3.0.6rc1/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 rafal      (501) staff       (20)      420 2023-05-29 14:50:53.000000 hdn-research-environment-3.0.6rc1/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 rafal      (501) staff       (20)     1364 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 rafal      (501) staff       (20)      858 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/migrations/0011_refactor_workflow.py
--rw-r--r--   0 rafal      (501) staff       (20)     1042 2024-03-05 12:56:41.000000 hdn-research-environment-3.0.6rc1/environment/migrations/0013_bucketsharinginvite_type_and_more.py
--rw-r--r--   0 rafal      (501) staff       (20)        0 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6rc1/environment/migrations/__init__.py
--rw-r--r--   0 rafal      (501) staff       (20)     2423 2024-03-05 12:56:41.000000 hdn-research-environment-3.0.6rc1/environment/models.py
--rw-r--r--   0 rafal      (501) staff       (20)    25434 2024-03-11 11:52:51.000000 hdn-research-environment-3.0.6rc1/environment/services.py
--rw-r--r--   0 rafal      (501) staff       (20)     4519 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/signals.py
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.291307 hdn-research-environment-3.0.6rc1/environment/static/
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.302079 hdn-research-environment-3.0.6rc1/environment/static/environment/
--rw-r--r--   0 rafal      (501) staff       (20)     6148 2023-02-02 14:12:52.000000 hdn-research-environment-3.0.6rc1/environment/static/environment/.DS_Store
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.304730 hdn-research-environment-3.0.6rc1/environment/static/environment/css/
--rw-r--r--   0 rafal      (501) staff       (20)    11789 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/static/environment/css/bucket_files_dropzone.css
--rw-r--r--   0 rafal      (501) staff       (20)      342 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/static/environment/css/creation_form.css
--rw-r--r--   0 rafal      (501) staff       (20)     6583 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6rc1/environment/static/environment/css/environment-base.css
--rw-r--r--   0 rafal      (501) staff       (20)      117 2023-05-29 14:50:53.000000 hdn-research-environment-3.0.6rc1/environment/static/environment/css/management_views.css
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.306303 hdn-research-environment-3.0.6rc1/environment/static/environment/js/
--rw-r--r--   0 rafal      (501) staff       (20)   114702 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/static/environment/js/bucket_files_dropzone.min.js
--rw-r--r--   0 rafal      (501) staff       (20)      564 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6rc1/environment/static/environment/js/cookie.js
--rw-r--r--   0 rafal      (501) staff       (20)      199 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/static/environment/js/destroy_shared_bucket.js
--rw-r--r--   0 rafal      (501) staff       (20)      291 2023-06-12 13:30:54.000000 hdn-research-environment-3.0.6rc1/environment/static/environment/js/forms.js
--rw-r--r--   0 rafal      (501) staff       (20)     2835 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 rafal      (501) staff       (20)     3308 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/tasks.py
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.291611 hdn-research-environment-3.0.6rc1/environment/templates/
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.310995 hdn-research-environment-3.0.6rc1/environment/templates/environment/
--rw-r--r--   0 rafal      (501) staff       (20)     7510 2023-09-08 13:35:54.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 rafal      (501) staff       (20)     3268 2023-09-08 13:35:54.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 rafal      (501) staff       (20)     2964 2024-04-09 13:28:41.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/_environment_tabs.html
--rw-r--r--   0 rafal      (501) staff       (20)     5553 2024-03-01 11:52:17.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/_shared_buckets_list.html
--rw-r--r--   0 rafal      (501) staff       (20)     1073 2023-06-12 13:30:54.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 rafal      (501) staff       (20)     3847 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/bucket_files_form.html
--rw-r--r--   0 rafal      (501) staff       (20)     3628 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 rafal      (501) staff       (20)     1208 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/create_shared_bucket.html
--rw-r--r--   0 rafal      (501) staff       (20)     1154 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/create_shared_workspace.html
--rw-r--r--   0 rafal      (501) staff       (20)     1630 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.311535 hdn-research-environment-3.0.6rc1/environment/templates/environment/email/
--rw-r--r--   0 rafal      (501) staff       (20)      272 2023-06-12 13:30:54.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/email/billing_sharing_confirmation.html
--rw-r--r--   0 rafal      (501) staff       (20)      263 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/email/bucket_sharing_confirmation.html
--rw-r--r--   0 rafal      (501) staff       (20)      351 2023-06-05 07:22:20.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 rafal      (501) staff       (20)     1163 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 rafal      (501) staff       (20)     5936 2024-03-01 10:40:36.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 rafal      (501) staff       (20)     1010 2024-01-29 13:36:38.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/manage_shared_billing_invitation.html
--rw-r--r--   0 rafal      (501) staff       (20)     6113 2024-03-01 10:40:36.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/manage_shared_bucket.html
--rw-r--r--   0 rafal      (501) staff       (20)     1075 2024-03-01 10:51:33.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/manage_shared_bucket_files.html
--rw-r--r--   0 rafal      (501) staff       (20)     1007 2024-01-29 13:36:38.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/manage_shared_bucket_invitation.html
--rw-r--r--   0 rafal      (501) staff       (20)     1719 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/research_environments.html
--rw-r--r--   0 rafal      (501) staff       (20)     5970 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/templates/environment/shared_bucket_files.html
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.312681 hdn-research-environment-3.0.6rc1/environment/templates/tag/
--rw-r--r--   0 rafal      (501) staff       (20)     1287 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/templates/tag/bucket_modal_button.html
--rw-r--r--   0 rafal      (501) staff       (20)      241 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6rc1/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 rafal      (501) staff       (20)     1486 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/templates/tag/environment_modal_button.html
--rw-r--r--   0 rafal      (501) staff       (20)     1955 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/templates/tag/workspace_destroy_modal_button.html
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.313045 hdn-research-environment-3.0.6rc1/environment/templatetags/
--rw-r--r--   0 rafal      (501) staff       (20)        0 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6rc1/environment/templatetags/__init__.py
--rw-r--r--   0 rafal      (501) staff       (20)     5724 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/templatetags/action_buttons.py
--rw-r--r--   0 rafal      (501) staff       (20)      136 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/templatetags/environment_templatetags.py
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.314767 hdn-research-environment-3.0.6rc1/environment/tests/
--rw-r--r--   0 rafal      (501) staff       (20)        0 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6rc1/environment/tests/__init__.py
--rw-r--r--   0 rafal      (501) staff       (20)      645 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/tests/helpers.py
--rw-r--r--   0 rafal      (501) staff       (20)    12158 2023-05-29 14:50:53.000000 hdn-research-environment-3.0.6rc1/environment/tests/mocks.py
--rw-r--r--   0 rafal      (501) staff       (20)     3007 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/tests/test_decorators.py
--rw-r--r--   0 rafal      (501) staff       (20)    10682 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/tests/test_services.py
--rw-r--r--   0 rafal      (501) staff       (20)     5327 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/tests/test_signals.py
--rw-r--r--   0 rafal      (501) staff       (20)     2909 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/tests/test_utilities.py
--rw-r--r--   0 rafal      (501) staff       (20)      640 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/tests/test_validators.py
--rw-r--r--   0 rafal      (501) staff       (20)     3380 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/tests/test_views.py
--rw-r--r--   0 rafal      (501) staff       (20)     3175 2024-03-01 10:23:41.000000 hdn-research-environment-3.0.6rc1/environment/urls.py
--rw-r--r--   0 rafal      (501) staff       (20)     1243 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6rc1/environment/utilities.py
--rw-r--r--   0 rafal      (501) staff       (20)      235 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6rc1/environment/validators.py
--rw-r--r--   0 rafal      (501) staff       (20)    23604 2024-04-09 13:28:41.000000 hdn-research-environment-3.0.6rc1/environment/views.py
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-16 13:27:30.315305 hdn-research-environment-3.0.6rc1/hdn_research_environment.egg-info/
--rw-r--r--   0 rafal      (501) staff       (20)      981 2024-04-16 13:27:30.000000 hdn-research-environment-3.0.6rc1/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 rafal      (501) staff       (20)     4041 2024-04-16 13:27:30.000000 hdn-research-environment-3.0.6rc1/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 rafal      (501) staff       (20)        1 2024-04-16 13:27:30.000000 hdn-research-environment-3.0.6rc1/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 rafal      (501) staff       (20)       84 2024-04-16 13:27:30.000000 hdn-research-environment-3.0.6rc1/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 rafal      (501) staff       (20)       12 2024-04-16 13:27:30.000000 hdn-research-environment-3.0.6rc1/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 rafal      (501) staff       (20)      109 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6rc1/pyproject.toml
--rw-r--r--   0 rafal      (501) staff       (20)     1059 2024-04-16 13:27:30.315894 hdn-research-environment-3.0.6rc1/setup.cfg
--rw-r--r--   0 rafal      (501) staff       (20)       38 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6rc1/setup.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.023335 hdn-research-environment-3.0.7rc0/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1551 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/LICENSE
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      115 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/MANIFEST.in
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      981 2024-04-10 10:04:39.023429 hdn-research-environment-3.0.7rc0/PKG-INFO
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      229 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/README.md
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.006991 hdn-research-environment-3.0.7rc0/environment/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        0 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/__init__.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.007896 hdn-research-environment-3.0.7rc0/environment/api/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     8203 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/api/__init__.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      939 2024-03-07 11:56:49.000000 hdn-research-environment-3.0.7rc0/environment/api/decorators.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      154 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/apps.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3074 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/constants.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1546 2024-04-08 12:07:08.000000 hdn-research-environment-3.0.7rc0/environment/decorators.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5362 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/deserializers.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     4404 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/entities.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1421 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/exceptions.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     7674 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/forms.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2518 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/mailers.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.010996 hdn-research-environment-3.0.7rc0/environment/migrations/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2174 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/00012_bucketsharinginvite.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1443 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0001_initial.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1579 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      403 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      420 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2220 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0005_workflow.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      394 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2348 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      476 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      420 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1364 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      858 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0011_refactor_workflow.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1042 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0013_bucketsharinginvite_type_and_more.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        0 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/__init__.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2423 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/models.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    25434 2024-04-08 12:07:19.000000 hdn-research-environment-3.0.7rc0/environment/services.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     4519 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/signals.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.001438 hdn-research-environment-3.0.7rc0/environment/static/
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.001535 hdn-research-environment-3.0.7rc0/environment/static/environment/
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.011779 hdn-research-environment-3.0.7rc0/environment/static/environment/css/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    11789 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/css/bucket_files_dropzone.css
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      342 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/css/creation_form.css
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     6583 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      117 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/css/management_views.css
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.013959 hdn-research-environment-3.0.7rc0/environment/static/environment/js/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)   114702 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/js/bucket_files_dropzone.min.js
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      564 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/js/cookie.js
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      199 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/js/destroy_shared_bucket.js
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      291 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/js/forms.js
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2835 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3308 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tasks.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.001729 hdn-research-environment-3.0.7rc0/environment/templates/
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.018075 hdn-research-environment-3.0.7rc0/environment/templates/environment/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     7510 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3268 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2996 2024-04-10 09:06:57.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/_environment_tabs.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5553 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/_shared_buckets_list.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1073 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3847 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/bucket_files_form.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3628 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1208 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/create_shared_bucket.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1154 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/create_shared_workspace.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1630 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.018769 hdn-research-environment-3.0.7rc0/environment/templates/environment/email/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      272 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/email/billing_sharing_confirmation.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      263 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/email/bucket_sharing_confirmation.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      351 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1163 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5936 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1010 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_billing_invitation.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     6113 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_bucket.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1075 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_bucket_files.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1007 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_bucket_invitation.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1719 2024-03-29 15:28:54.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/research_environments.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5970 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/shared_bucket_files.html
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.019566 hdn-research-environment-3.0.7rc0/environment/templates/tag/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1287 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/tag/bucket_modal_button.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      241 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1486 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/tag/environment_modal_button.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1955 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/tag/workspace_destroy_modal_button.html
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.020116 hdn-research-environment-3.0.7rc0/environment/templatetags/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        0 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templatetags/__init__.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5724 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templatetags/action_buttons.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      136 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templatetags/environment_templatetags.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.021959 hdn-research-environment-3.0.7rc0/environment/tests/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        0 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/__init__.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      645 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/helpers.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    12158 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/mocks.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3007 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/test_decorators.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    10682 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/test_services.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5327 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/test_signals.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2909 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/test_utilities.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      640 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/test_validators.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3380 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/test_views.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3175 2024-04-04 08:30:59.000000 hdn-research-environment-3.0.7rc0/environment/urls.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1243 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/utilities.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      235 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/validators.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    23604 2024-04-08 14:44:30.000000 hdn-research-environment-3.0.7rc0/environment/views.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.023239 hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      981 2024-04-10 10:04:38.000000 hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     4000 2024-04-10 10:04:38.000000 hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        1 2024-04-10 10:04:38.000000 hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)       84 2024-04-10 10:04:38.000000 hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)       12 2024-04-10 10:04:38.000000 hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      109 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/pyproject.toml
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1058 2024-04-10 10:04:39.023667 hdn-research-environment-3.0.7rc0/setup.cfg
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)       38 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/setup.py
```

### Comparing `hdn-research-environment-3.0.6rc1/LICENSE` & `hdn-research-environment-3.0.7rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/PKG-INFO` & `hdn-research-environment-3.0.7rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdn-research-environment
-Version: 3.0.6rc1
+Version: 3.0.7rc0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `hdn-research-environment-3.0.6rc1/environment/api/__init__.py` & `hdn-research-environment-3.0.7rc0/environment/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/api/decorators.py` & `hdn-research-environment-3.0.7rc0/environment/api/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/decorators.py` & `hdn-research-environment-3.0.7rc0/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/deserializers.py` & `hdn-research-environment-3.0.7rc0/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/entities.py` & `hdn-research-environment-3.0.7rc0/environment/entities.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,30 +21,22 @@
 
 class InstanceType(Enum):
     N1_STANDARD_1 = "n1-standard-1"
     N1_STANDARD_2 = "n1-standard-2"
     N1_STANDARD_4 = "n1-standard-4"
     N1_STANDARD_8 = "n1-standard-8"
     N1_STANDARD_16 = "n1-standard-16"
-    N2_STANDARD_2 = "n2-standard-2"
-    N2_STANDARD_4 = "n2-standard-4"
-    N2_STANDARD_8 = "n2-standard-8"
-    N2_STANDARD_16 = "n2-standard-16"
 
     def cpus(self):
         INSTANCE_TO_CPU_MAP = {
             InstanceType.N1_STANDARD_1: 1,
             InstanceType.N1_STANDARD_2: 2,
             InstanceType.N1_STANDARD_4: 4,
             InstanceType.N1_STANDARD_8: 8,
             InstanceType.N1_STANDARD_16: 16,
-            InstanceType.N2_STANDARD_2: 2,
-            InstanceType.N2_STANDARD_4: 4,
-            InstanceType.N2_STANDARD_8: 8,
-            InstanceType.N2_STANDARD_16: 16,
         }
 
         return INSTANCE_TO_CPU_MAP[self]
 
 
 class GPUAcceleratorType(Enum):
     NVIDIA_TESLA_T4 = "nvidia-tesla-t4"
```

### Comparing `hdn-research-environment-3.0.6rc1/environment/exceptions.py` & `hdn-research-environment-3.0.7rc0/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/forms.py` & `hdn-research-environment-3.0.7rc0/environment/forms.py`

 * *Files 13% similar despite different names*

```diff
@@ -56,18 +56,14 @@
 
 class CreateResearchEnvironmentForm(forms.Form):
     AVAILABLE_MACHINE_TYPES = [
         ("n1-standard-2", MACHINE_TYPE_SPECIFICATION[InstanceType.N1_STANDARD_2]),
         ("n1-standard-4", MACHINE_TYPE_SPECIFICATION[InstanceType.N1_STANDARD_4]),
         ("n1-standard-8", MACHINE_TYPE_SPECIFICATION[InstanceType.N1_STANDARD_8]),
         ("n1-standard-16", MACHINE_TYPE_SPECIFICATION[InstanceType.N1_STANDARD_16]),
-        ("n2-standard-2", MACHINE_TYPE_SPECIFICATION[InstanceType.N2_STANDARD_2]),
-        ("n2-standard-4", MACHINE_TYPE_SPECIFICATION[InstanceType.N2_STANDARD_4]),
-        ("n2-standard-8", MACHINE_TYPE_SPECIFICATION[InstanceType.N2_STANDARD_8]),
-        ("n2-standard-16", MACHINE_TYPE_SPECIFICATION[InstanceType.N2_STANDARD_16]),
     ]
     AVAILABLE_ENVIRONMENT_TYPES = [
         ("jupyter", "Jupyter"),
         ("rstudio", "RStudio"),
     ]
     AVAILABLE_GPU_ACCELERATOR_TYPES = [
         ("", "Machine without GPU attached"),
```

### Comparing `hdn-research-environment-3.0.6rc1/environment/mailers.py` & `hdn-research-environment-3.0.7rc0/environment/mailers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/migrations/00012_bucketsharinginvite.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/00012_bucketsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/migrations/0001_initial.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/migrations/0005_workflow.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/migrations/0011_refactor_workflow.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0011_refactor_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/migrations/0013_bucketsharinginvite_type_and_more.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0013_bucketsharinginvite_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/models.py` & `hdn-research-environment-3.0.7rc0/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/services.py` & `hdn-research-environment-3.0.7rc0/environment/services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/signals.py` & `hdn-research-environment-3.0.7rc0/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/static/environment/css/bucket_files_dropzone.css` & `hdn-research-environment-3.0.7rc0/environment/static/environment/css/bucket_files_dropzone.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/static/environment/css/environment-base.css` & `hdn-research-environment-3.0.7rc0/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/static/environment/js/bucket_files_dropzone.min.js` & `hdn-research-environment-3.0.7rc0/environment/static/environment/js/bucket_files_dropzone.min.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/static/environment/js/cookie.js` & `hdn-research-environment-3.0.7rc0/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-3.0.7rc0/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/tasks.py` & `hdn-research-environment-3.0.7rc0/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/_available_environments_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/_billing_accounts_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/_environment_tabs.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/_environment_tabs.html`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         .then(({ finished }) => {
             if (finished) {
                 refreshCards(executionId);
             }
         });
     }
 
-    var socket = io("{{ websocket_url }}");
+    var socket = io("{{ websocket_url }}", { transports : ['websocket'] });
 
     socket.on('workflow_update', function(data) {
         refreshCards(data.workbench_activity_id);
     });
 
     {% for workflow in workflows %}
         socket.emit("join", "{{ workflow.execution_resource_name }}");
```

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/_shared_buckets_list.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/_shared_buckets_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/bucket_files_form.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/bucket_files_form.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/create_shared_bucket.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/create_shared_bucket.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/create_shared_workspace.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/create_shared_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/create_workspace.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/create_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/manage_shared_billing_invitation.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_billing_invitation.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/manage_shared_bucket.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_bucket.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/manage_shared_bucket_files.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_bucket_files.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/manage_shared_bucket_invitation.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_bucket_invitation.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/research_environments.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/environment/shared_bucket_files.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/shared_bucket_files.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/tag/bucket_modal_button.html` & `hdn-research-environment-3.0.7rc0/environment/templates/tag/bucket_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-3.0.7rc0/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templates/tag/workspace_destroy_modal_button.html` & `hdn-research-environment-3.0.7rc0/environment/templates/tag/workspace_destroy_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/templatetags/action_buttons.py` & `hdn-research-environment-3.0.7rc0/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/tests/helpers.py` & `hdn-research-environment-3.0.7rc0/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/tests/mocks.py` & `hdn-research-environment-3.0.7rc0/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/tests/test_decorators.py` & `hdn-research-environment-3.0.7rc0/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/tests/test_services.py` & `hdn-research-environment-3.0.7rc0/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/tests/test_signals.py` & `hdn-research-environment-3.0.7rc0/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/tests/test_utilities.py` & `hdn-research-environment-3.0.7rc0/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/tests/test_validators.py` & `hdn-research-environment-3.0.7rc0/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/tests/test_views.py` & `hdn-research-environment-3.0.7rc0/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/urls.py` & `hdn-research-environment-3.0.7rc0/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/utilities.py` & `hdn-research-environment-3.0.7rc0/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/environment/views.py` & `hdn-research-environment-3.0.7rc0/environment/views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.6rc1/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdn-research-environment
-Version: 3.0.6rc1
+Version: 3.0.7rc0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `hdn-research-environment-3.0.6rc1/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 environment/migrations/0007_billingaccountsharinginvite.py
 environment/migrations/0008_workflow_workspace_name.py
 environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
 environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
 environment/migrations/0011_refactor_workflow.py
 environment/migrations/0013_bucketsharinginvite_type_and_more.py
 environment/migrations/__init__.py
-environment/static/environment/.DS_Store
 environment/static/environment/css/bucket_files_dropzone.css
 environment/static/environment/css/creation_form.css
 environment/static/environment/css/environment-base.css
 environment/static/environment/css/management_views.css
 environment/static/environment/js/bucket_files_dropzone.min.js
 environment/static/environment/js/cookie.js
 environment/static/environment/js/destroy_shared_bucket.js
```

### Comparing `hdn-research-environment-3.0.6rc1/setup.cfg` & `hdn-research-environment-3.0.7rc0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 3.0.6rc1
+version = 3.0.7rc
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

