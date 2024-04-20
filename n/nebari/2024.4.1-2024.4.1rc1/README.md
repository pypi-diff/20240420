# Comparing `tmp/nebari-2024.4.1.tar.gz` & `tmp/nebari-2024.4.1rc1.tar.gz`

## Comparing `nebari-2024.4.1.tar` & `nebari-2024.4.1rc1.tar`

### file list

```diff
@@ -1,429 +1,429 @@
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nebari-2024.4.1/.cirun.yml
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 nebari-2024.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2024.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2024.4.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nebari-2024.4.1/MANIFEST.in
--rw-r--r--   0        0        0    88441 2020-02-02 00:00:00.000000 nebari-2024.4.1/RELEASE.md
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 nebari-2024.4.1/SECURITY.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.4.1/flake.lock
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 nebari-2024.4.1/flake.nix
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nebari-2024.4.1/pytest.ini
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/release-notes-sync-config.yaml
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/ISSUE_TEMPLATE/general-issue.yml
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/ISSUE_TEMPLATE/release-checklist.md
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/ISSUE_TEMPLATE/testing-checklist.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/actions/publish-from-template/action.yml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/actions/publish-from-template/render_template.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/failed-workflow-issue-templates/test-provider.md
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/workflows/generate_cli_doc.yml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/workflows/release-notes-sync.yaml
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/workflows/run-precommit.yaml
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/workflows/test-provider.yaml
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/workflows/test_aws_integration.yaml
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/workflows/test_conda_build.yaml
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/workflows/test_do_integration.yaml
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/workflows/test_gcp_integration.yaml
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/workflows/test_helm_charts.yaml
--rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/workflows/test_local_integration.yaml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nebari-2024.4.1/.github/workflows/typing.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nebari-2024.4.1/docs-sphinx/Makefile
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.4.1/docs-sphinx/README.md
--rw-r--r--   0        0        0    46502 2020-02-02 00:00:00.000000 nebari-2024.4.1/docs-sphinx/cli.html
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nebari-2024.4.1/docs-sphinx/cli.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 nebari-2024.4.1/docs-sphinx/conf.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 nebari-2024.4.1/docs-sphinx/index.rst
--rw-r--r--   0        0        0    14306 2020-02-02 00:00:00.000000 nebari-2024.4.1/scripts/aws-force-destroy.py
--rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2024.4.1/scripts/aws-force-destroy.sh
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 nebari-2024.4.1/scripts/helm-validate.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nebari-2024.4.1/scripts/keycloak-export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/__init__.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/_version.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/cli.py
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/config.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/constants.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/deploy.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/deprecate.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/destroy.py
--rw-r--r--   0        0        0    11159 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/initialize.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/keycloak.py
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/render.py
--rw-r--r--   0        0        0    32660 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/upgrade.py
--rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/utils.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/__init__.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/git.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/terraform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/cicd/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/cicd/common.py
--rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/cicd/github.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/cicd/gitlab.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/cicd/linter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/cloud/__init__.py
--rw-r--r--   0        0        0    38296 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/cloud/amazon_web_services.py
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/cloud/azure_cloud.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/cloud/commons.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/cloud/digital_ocean.py
--rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/cloud/google_cloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/dns/__init__.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/dns/cloudflare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/oauth/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/provider/oauth/auth0.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/__init__.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/base.py
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/tf_objects.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/bootstrap/__init__.py
--rw-r--r--   0        0        0    32575 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/locals.tf
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/main.tf
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/outputs.tf
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/variables.tf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/versions.tf
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/variables.tf
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/efs/main.tf
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/efs/outputs.tf
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/outputs.tf
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/network/outputs.tf
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/outputs.tf
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/rds/outputs.tf
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/registry/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/registry/outputs.tf
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/registry/variables.tf
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/s3/main.tf
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/s3/outputs.tf
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/s3/variables.tf
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/main.tf
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/outputs.tf
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/providers.tf
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/versions.tf
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/modules/registry/main.tf
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/modules/registry/variables.tf
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/outputs.tf
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/providers.tf
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/modules/registry/main.tf
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/modules/registry/variable.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/modules/registry/versions.tf
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/existing/main.tf
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/variables.tf
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/versions.tf
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/service_account.tf
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/templates/kubeconfig.yaml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/network/main.tf
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/network/variables.tf
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/main.tf
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/variables.tf
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/local/main.tf
--rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/local/metallb.yaml
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/local/outputs.tf
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/infrastructure/template/local/variables.tf
--rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/template/locals.tf
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/template/main.tf
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/template/outputs.tf
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/template/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/template/versions.tf
--rw-r--r--   0        0        0     9777 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/outputs.tf
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/external-container-registry.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/locals.tf
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/main.tf
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/versions.tf
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/variables.tf
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/main.tf
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/variables.tf
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/variables.tf
--rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf
--rw-r--r--   0        0        0     9398 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/__init__.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/template/main.tf
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/template/outputs.tf
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/template/versions.tf
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/outputs.tf
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak_configuration/template/outputs.tf
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak_configuration/template/providers.tf
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak_configuration/template/versions.tf
--rw-r--r--   0        0        0    22258 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/__init__.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/conda-store.tf
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/forward-auth.tf
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/jupyterhub_ssh.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/locals.tf
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/monitoring.tf
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/outputs.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/providers.tf
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/versions.tf
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/outputs.tf
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/variables.tf
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/output.tf
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/variables.tf
--rw-r--r--   0        0        0    16354 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/values.yaml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/versions.tf
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/outputs.tf
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py
--rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/middleware.tf
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/outputs.tf
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
--rw-r--r--   0        0        0    19781 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/versions.tf
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/values.yaml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf
--rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/values.yaml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/versions.tf
--rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json
--rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json
--rw-r--r--   0        0        0    34598 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json
--rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json
--rw-r--r--   0        0        0    28438 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_minio.yaml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_promtail.yaml
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/outputs.tf
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/values.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/values.yaml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/__init__.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/helm-extension.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/nebari-config.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/providers.tf
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/versions.tf
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/main.tf
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf
--rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/aws/main.tf
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/output.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/azure/main.tf
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/do/main.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/do/modules/spaces/main.tf
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/do/modules/spaces/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/do/modules/spaces/versions.tf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/versions.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/existing/main.tf
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/gcp/main.tf
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/main.tf
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/stages/terraform_state/template/local/main.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/subcommands/__init__.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/subcommands/deploy.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/subcommands/destroy.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/subcommands/dev.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/subcommands/info.py
--rw-r--r--   0        0        0    36979 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/subcommands/init.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/subcommands/keycloak.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/subcommands/render.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/subcommands/support.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/subcommands/upgrade.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/_nebari/subcommands/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/nebari/__init__.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/nebari/__main__.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/nebari/hookspecs.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/nebari/plugins.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 nebari-2024.4.1/src/nebari/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/conftest.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/common/__init__.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/common/config_mod_utils.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/common/kube_api.py
--rw-r--r--   0        0        0    16519 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/common/navigator.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/common/playwright_fixtures.py
--rw-r--r--   0        0        0    10512 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/common/run_notebook.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/common/notebooks/test_notebook_output.ipynb
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/common/tests/test_notebook.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_deployment/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_deployment/constants.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_deployment/test_dask_gateway.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_deployment/test_grafana_api.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_deployment/test_jupyterhub_ssh.py
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_deployment/test_loki_deployment.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_deployment/utils.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_deployment/assets/notebook/simple.ipynb
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_e2e/.gitignore
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_e2e/cypress.json
--rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_e2e/package-lock.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_e2e/package.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_e2e/cypress/.gitignore
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_e2e/cypress/integration/main.js
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_e2e/cypress/plugins/index.js
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_e2e/cypress/support/index.js
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_e2e/playwright/.env.tpl
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_e2e/playwright/README.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_e2e/playwright/test_playwright.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_integration/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_integration/__init__.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_integration/conftest.py
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_integration/deployment_fixtures.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_integration/test_all_clouds.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_integration/test_gpu.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_integration/test_preemptible.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/__init__.py
--rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/conftest.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_cli.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_cli_deploy.py
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_cli_dev.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_cli_init.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_cli_init_repository.py
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_cli_keycloak.py
--rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_cli_support.py
--rw-r--r--   0        0        0    18509 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_cli_upgrade.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_cli_validate.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_commons.py
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_config.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_dependencies.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_init.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_links.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_provider.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_render.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_schema.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/test_upgrade.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/utils.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/aws.error.kubernetes-version.yaml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/aws.happy.yaml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/azure.happy.yaml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/do.happy.yaml
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/gcp.happy.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/local.error.authentication-type-called-custom.yaml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/local.error.extra-fields.yaml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/local.error.project_name.ends_with_special.yaml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/local.error.project_name.starts_with_number.yaml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/local.error.project_name.too_long.yaml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/local.happy.auth0.yaml
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/local.happy.github.yaml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/local.happy.project_name.with_numbers.yaml
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/local.happy.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/min.happy.jupyterlab.default_settings.yaml
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/min.happy.monitoring.overrides.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/cli_validate/min.happy.yaml
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2024.4.1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 nebari-2024.4.1/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2024.4.1/LICENSE
--rw-r--r--   0        0        0     9814 2020-02-02 00:00:00.000000 nebari-2024.4.1/README.md
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 nebari-2024.4.1/pyproject.toml
--rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 nebari-2024.4.1/PKG-INFO
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.cirun.yml
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/MANIFEST.in
+-rw-r--r--   0        0        0    87041 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/RELEASE.md
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/SECURITY.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/flake.lock
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/flake.nix
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/pytest.ini
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/release-notes-sync-config.yaml
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/actions/publish-from-template/action.yml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/actions/publish-from-template/render_template.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/failed-workflow-issue-templates/test-provider.md
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/generate_cli_doc.yml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/release-notes-sync.yaml
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/run-precommit.yaml
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test-provider.yaml
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_aws_integration.yaml
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_conda_build.yaml
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_do_integration.yaml
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_gcp_integration.yaml
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_helm_charts.yaml
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_local_integration.yaml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/typing.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/Makefile
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/README.md
+-rw-r--r--   0        0        0    46502 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/cli.html
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/cli.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/conf.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/index.rst
+-rw-r--r--   0        0        0    14306 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/scripts/aws-force-destroy.py
+-rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/scripts/aws-force-destroy.sh
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/scripts/helm-validate.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/scripts/keycloak-export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/__init__.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/_version.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/cli.py
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/config.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/constants.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/deploy.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/deprecate.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/destroy.py
+-rw-r--r--   0        0        0    11250 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/initialize.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/keycloak.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/render.py
+-rw-r--r--   0        0        0    31183 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/upgrade.py
+-rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/utils.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/__init__.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/git.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/terraform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/common.py
+-rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/github.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/gitlab.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/linter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/__init__.py
+-rw-r--r--   0        0        0    38296 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/amazon_web_services.py
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/azure_cloud.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/commons.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/digital_ocean.py
+-rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/google_cloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/dns/__init__.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/dns/cloudflare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/oauth/__init__.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/oauth/auth0.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/__init__.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/base.py
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/tf_objects.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/bootstrap/__init__.py
+-rw-r--r--   0        0        0    32085 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/locals.tf
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/main.tf
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/versions.tf
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/variables.tf
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/main.tf
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/outputs.tf
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/outputs.tf
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/outputs.tf
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/outputs.tf
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/outputs.tf
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/outputs.tf
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/variables.tf
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/main.tf
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/outputs.tf
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/variables.tf
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/main.tf
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/outputs.tf
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/providers.tf
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/versions.tf
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/main.tf
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/variables.tf
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/providers.tf
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/main.tf
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/variable.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/versions.tf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/existing/main.tf
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/versions.tf
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/service_account.tf
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/templates/kubeconfig.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/main.tf
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/variables.tf
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/main.tf
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/variables.tf
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/main.tf
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/variables.tf
+-rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/locals.tf
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/outputs.tf
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/versions.tf
+-rw-r--r--   0        0        0     9777 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/outputs.tf
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/__init__.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/external-container-registry.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/locals.tf
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/versions.tf
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/variables.tf
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/main.tf
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/variables.tf
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/variables.tf
+-rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf
+-rw-r--r--   0        0        0     9398 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/main.tf
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/outputs.tf
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/versions.tf
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/outputs.tf
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/outputs.tf
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/providers.tf
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/versions.tf
+-rw-r--r--   0        0        0    22258 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/__init__.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/forward-auth.tf
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub_ssh.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/locals.tf
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/providers.tf
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/versions.tf
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/outputs.tf
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/variables.tf
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/output.tf
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/variables.tf
+-rw-r--r--   0        0        0    16354 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/values.yaml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/versions.tf
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/outputs.tf
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py
+-rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/middleware.tf
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/outputs.tf
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
+-rw-r--r--   0        0        0    19781 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/versions.tf
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/values.yaml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf
+-rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/values.yaml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/versions.tf
+-rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json
+-rw-r--r--   0        0        0    34598 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json
+-rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json
+-rw-r--r--   0        0        0    28438 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_minio.yaml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_promtail.yaml
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/outputs.tf
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/values.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/values.yaml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/helm-extension.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/nebari-config.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/providers.tf
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/versions.tf
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/main.tf
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf
+-rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/main.tf
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/output.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/main.tf
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/main.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/main.tf
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/versions.tf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/versions.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/existing/main.tf
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/main.tf
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/local/main.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/__init__.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/deploy.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/destroy.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/dev.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/info.py
+-rw-r--r--   0        0        0    36979 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/init.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/keycloak.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/render.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/support.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/upgrade.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/__init__.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/__main__.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/hookspecs.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/plugins.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/conftest.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/__init__.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/config_mod_utils.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/kube_api.py
+-rw-r--r--   0        0        0    16519 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/navigator.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/playwright_fixtures.py
+-rw-r--r--   0        0        0    10512 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/run_notebook.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/notebooks/test_notebook_output.ipynb
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/tests/test_notebook.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/constants.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/test_dask_gateway.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/test_grafana_api.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/test_jupyterhub_ssh.py
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/test_loki_deployment.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/utils.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/assets/notebook/simple.ipynb
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/.gitignore
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress.json
+-rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/package-lock.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/package.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/.gitignore
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/integration/main.js
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/plugins/index.js
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/support/index.js
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/playwright/.env.tpl
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/playwright/README.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/playwright/test_playwright.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/__init__.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/conftest.py
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/deployment_fixtures.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/test_all_clouds.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/test_gpu.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/test_preemptible.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/__init__.py
+-rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/conftest.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_deploy.py
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_dev.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_init.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_init_repository.py
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_keycloak.py
+-rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_support.py
+-rw-r--r--   0        0        0    18509 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_upgrade.py
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_validate.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_commons.py
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_config.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_dependencies.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_init.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_links.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_provider.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_render.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_schema.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_upgrade.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/utils.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/aws.error.kubernetes-version.yaml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/aws.happy.yaml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/azure.happy.yaml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/do.happy.yaml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/gcp.happy.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.authentication-type-called-custom.yaml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.extra-fields.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.project_name.ends_with_special.yaml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.project_name.starts_with_number.yaml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.project_name.too_long.yaml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.auth0.yaml
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.github.yaml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.project_name.with_numbers.yaml
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/min.happy.jupyterlab.default_settings.yaml
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/min.happy.monitoring.overrides.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/min.happy.yaml
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/LICENSE
+-rw-r--r--   0        0        0     9814 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/README.md
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    12409 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/PKG-INFO
```

### Comparing `nebari-2024.4.1/.cirun.yml` & `nebari-2024.4.1rc1/.cirun.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.pre-commit-config.yaml` & `nebari-2024.4.1rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/CODE_OF_CONDUCT.md` & `nebari-2024.4.1rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/CONTRIBUTING.md` & `nebari-2024.4.1rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/RELEASE.md` & `nebari-2024.4.1rc1/RELEASE.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,34 +5,14 @@
 <!-- Note:
 The RELEASE.md file at the root of the Nebari codebase is the source of truth for all release notes.
 If you want to update the release notes, open a PR against nebari-dev/nebari.
 This file is copied to nebari-dev/nebari-docs using a GitHub Action. -->
 
 ---
 
-## Release 2024.4.1 - April 20, 2024
-
-### What's Changed
-* update azurerm version by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2370
-* Get JupyterHub `groups` from Keycloak, support `oauthenticator` 16.3+ by @krassowski in https://github.com/nebari-dev/nebari/pull/2361
-* add full names for cloud providers in guided init by @exitflynn in https://github.com/nebari-dev/nebari/pull/2375
-* Add middleware to prefix JupyterHub navbar items with /hub. by @marcelovilla in https://github.com/nebari-dev/nebari/pull/2360
-* CLN: split #1928, refactor render test by @fangchenli in https://github.com/nebari-dev/nebari/pull/2246
-* add trailing slash for jupyterhub proxy paths by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2387
-* remove references to deprecated cdsdashboards by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2390
-* add default node groups to config by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2398
-* Update concurrency settings for Integration tests by @viniciusdc in https://github.com/nebari-dev/nebari/pull/2393
-* Make CI/CD Cloud Provider Test Conditional by @tylergraff in https://github.com/nebari-dev/nebari/pull/2369
-
-### New Contributors
-* @exitflynn made their first contribution in https://github.com/nebari-dev/nebari/pull/2375
-
-**Full Changelog**: https://github.com/nebari-dev/nebari/compare/2024.3.3...2024.4.1
-
-
 ## Release 2024.3.3 - March 27, 2024
 
 ### What's Changed
 * get default variable value when following a terraform variable by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2322
 * Upgrade Actions versions by @isumitjha in https://github.com/nebari-dev/nebari/pull/2291
 * Cleanup spawner logs by @krassowski in https://github.com/nebari-dev/nebari/pull/2328
 * Fix loki gateway url when deployed on non-dev namespace by @aktech in https://github.com/nebari-dev/nebari/pull/2327
```

### Comparing `nebari-2024.4.1/SECURITY.md` & `nebari-2024.4.1rc1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/flake.lock` & `nebari-2024.4.1rc1/flake.lock`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/flake.nix` & `nebari-2024.4.1rc1/flake.nix`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/PULL_REQUEST_TEMPLATE.md` & `nebari-2024.4.1rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/ISSUE_TEMPLATE/bug-report.yml` & `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/ISSUE_TEMPLATE/config.yml` & `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/ISSUE_TEMPLATE/feature-request.yml` & `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/ISSUE_TEMPLATE/general-issue.yml` & `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/ISSUE_TEMPLATE/release-checklist.md` & `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/ISSUE_TEMPLATE/testing-checklist.md` & `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/actions/publish-from-template/action.yml` & `nebari-2024.4.1rc1/.github/actions/publish-from-template/action.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/workflows/generate_cli_doc.yml` & `nebari-2024.4.1rc1/.github/workflows/generate_cli_doc.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/workflows/release-notes-sync.yaml` & `nebari-2024.4.1rc1/.github/workflows/release-notes-sync.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/workflows/release.yaml` & `nebari-2024.4.1rc1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/workflows/run-precommit.yaml` & `nebari-2024.4.1rc1/.github/workflows/run-precommit.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/workflows/test-provider.yaml` & `nebari-2024.4.1rc1/.github/workflows/test-provider.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -28,21 +28,16 @@
     inputs:
       pr_number:
         required: true
         type: string
 
 jobs:
   test-render-providers:
-    # Prevents the execution of this test under the following conditions:
-    # 1. When the 'NO_PROVIDER_CREDENTIALS' GitHub variable is set, indicating the absence of provider credentials.
-    # 2. For pull requests (PRs) originating from a fork, since GitHub does not provide the fork's credentials to the destination repository.
-    # ref. https://github.com/nebari-dev/nebari/issues/2379
-    if: |
-      vars.NO_PROVIDER_CREDENTIALS == '' &&
-      (github.event.pull_request.head.repo.full_name == github.repository || github.event_name != 'pull_request')
+    # avoid running on PRs coming from a fork
+    if: github.event.pull_request.head.repo.full_name == github.repository || github.event_name != 'pull_request'
     name: "Test Nebari Provider"
     runs-on: ubuntu-latest
     permissions:
       id-token: write
       contents: read
       pull-requests: write
     strategy:
```

### Comparing `nebari-2024.4.1/.github/workflows/test.yaml` & `nebari-2024.4.1rc1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/workflows/test_aws_integration.yaml` & `nebari-2024.4.1rc1/.github/workflows/test_aws_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/workflows/test_conda_build.yaml` & `nebari-2024.4.1rc1/.github/workflows/test_conda_build.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/workflows/test_do_integration.yaml` & `nebari-2024.4.1rc1/.github/workflows/test_do_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/workflows/test_gcp_integration.yaml` & `nebari-2024.4.1rc1/.github/workflows/test_gcp_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/workflows/test_helm_charts.yaml` & `nebari-2024.4.1rc1/.github/workflows/test_helm_charts.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.github/workflows/test_local_integration.yaml` & `nebari-2024.4.1rc1/.github/workflows/test_local_integration.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -30,27 +30,22 @@
       - ".cirun.yml"
   workflow_call:
     inputs:
       pr_number:
         required: true
         type: string
 
-# When the cancel-in-progress: true option is specified, any concurrent jobs or workflows using the same
-# concurrency group will cancel both the pending and currently running jobs or workflows. This allows only
-# one job or workflow in the concurrency group to be in progress at a time.
-concurrency:
-  group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
-  cancel-in-progress: true
-
 jobs:
   test-local-integration:
     runs-on: "cirun-runner--${{ github.run_id }}"
     defaults:
       run:
         shell: bash -l {0}
+    concurrency:
+      group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
     steps:
       - name: 'Checkout Infrastructure'
         uses: actions/checkout@main
         with:
           fetch-depth: 0
 
       - name: Checkout the branch from the PR that triggered the job
```

### Comparing `nebari-2024.4.1/.github/workflows/typing.yaml` & `nebari-2024.4.1rc1/.github/workflows/typing.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/docs-sphinx/Makefile` & `nebari-2024.4.1rc1/docs-sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/docs-sphinx/README.md` & `nebari-2024.4.1rc1/docs-sphinx/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/docs-sphinx/cli.html` & `nebari-2024.4.1rc1/docs-sphinx/cli.html`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/scripts/aws-force-destroy.py` & `nebari-2024.4.1rc1/scripts/aws-force-destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/scripts/aws-force-destroy.sh` & `nebari-2024.4.1rc1/scripts/aws-force-destroy.sh`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/scripts/helm-validate.py` & `nebari-2024.4.1rc1/scripts/helm-validate.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/scripts/keycloak-export.py` & `nebari-2024.4.1rc1/scripts/keycloak-export.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/cli.py` & `nebari-2024.4.1rc1/src/_nebari/cli.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/config.py` & `nebari-2024.4.1rc1/src/_nebari/config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/constants.py` & `nebari-2024.4.1rc1/src/_nebari/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CURRENT_RELEASE = "2024.4.1"
+CURRENT_RELEASE = "2024.3.3"
 
 # NOTE: Terraform cannot be upgraded further due to Hashicorp licensing changes
 # implemented in August 2023.
 # https://www.hashicorp.com/license-faq
 TERRAFORM_VERSION = "1.5.7"
 
 # 04-kubernetes-ingress
```

### Comparing `nebari-2024.4.1/src/_nebari/deploy.py` & `nebari-2024.4.1rc1/src/_nebari/deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/destroy.py` & `nebari-2024.4.1rc1/src/_nebari/destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/initialize.py` & `nebari-2024.4.1rc1/src/_nebari/initialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,668 +31,674 @@
 000001e0: 4546 4155 4c54 5f41 5753 5f4e 4f44 455f  EFAULT_AWS_NODE_
 000001f0: 4752 4f55 5053 2c0a 2020 2020 4445 4641  GROUPS,.    DEFA
 00000200: 554c 545f 415a 5552 455f 4e4f 4445 5f47  ULT_AZURE_NODE_G
 00000210: 524f 5550 532c 0a20 2020 2044 4546 4155  ROUPS,.    DEFAU
 00000220: 4c54 5f44 4f5f 4e4f 4445 5f47 524f 5550  LT_DO_NODE_GROUP
 00000230: 532c 0a20 2020 2044 4546 4155 4c54 5f47  S,.    DEFAULT_G
 00000240: 4350 5f4e 4f44 455f 4752 4f55 5053 2c0a  CP_NODE_GROUPS,.
-00000250: 2020 2020 6e6f 6465 5f67 726f 7570 735f      node_groups_
-00000260: 746f 5f64 6963 742c 0a29 0a66 726f 6d20  to_dict,.).from 
-00000270: 5f6e 6562 6172 692e 7374 6167 6573 2e6b  _nebari.stages.k
-00000280: 7562 6572 6e65 7465 735f 696e 6772 6573  ubernetes_ingres
-00000290: 7320 696d 706f 7274 2043 6572 7469 6669  s import Certifi
-000002a0: 6361 7465 456e 756d 0a66 726f 6d20 5f6e  cateEnum.from _n
-000002b0: 6562 6172 692e 7374 6167 6573 2e6b 7562  ebari.stages.kub
-000002c0: 6572 6e65 7465 735f 6b65 7963 6c6f 616b  ernetes_keycloak
-000002d0: 2069 6d70 6f72 7420 4175 7468 656e 7469   import Authenti
-000002e0: 6361 7469 6f6e 456e 756d 0a66 726f 6d20  cationEnum.from 
-000002f0: 5f6e 6562 6172 692e 7374 6167 6573 2e74  _nebari.stages.t
-00000300: 6572 7261 666f 726d 5f73 7461 7465 2069  erraform_state i
-00000310: 6d70 6f72 7420 5465 7272 6166 6f72 6d53  mport TerraformS
-00000320: 7461 7465 456e 756d 0a66 726f 6d20 5f6e  tateEnum.from _n
-00000330: 6562 6172 692e 7574 696c 7320 696d 706f  ebari.utils impo
-00000340: 7274 2067 6574 5f6c 6174 6573 745f 6b75  rt get_latest_ku
-00000350: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
-00000360: 2c20 7261 6e64 6f6d 5f73 6563 7572 655f  , random_secure_
-00000370: 7374 7269 6e67 0a66 726f 6d20 5f6e 6562  string.from _neb
-00000380: 6172 692e 7665 7273 696f 6e20 696d 706f  ari.version impo
-00000390: 7274 205f 5f76 6572 7369 6f6e 5f5f 0a66  rt __version__.f
-000003a0: 726f 6d20 6e65 6261 7269 2e73 6368 656d  rom nebari.schem
-000003b0: 6120 696d 706f 7274 2050 726f 7669 6465  a import Provide
-000003c0: 7245 6e75 6d2c 2067 6974 6875 625f 7572  rEnum, github_ur
-000003d0: 6c5f 7265 6765 780a 0a6c 6f67 6765 7220  l_regex..logger 
-000003e0: 3d20 6c6f 6767 696e 672e 6765 744c 6f67  = logging.getLog
-000003f0: 6765 7228 5f5f 6e61 6d65 5f5f 290a 0a57  ger(__name__)..W
-00000400: 454c 434f 4d45 5f48 4541 4445 525f 5445  ELCOME_HEADER_TE
-00000410: 5854 203d 2022 596f 7572 206f 7065 6e20  XT = "Your open 
-00000420: 736f 7572 6365 2064 6174 6120 7363 6965  source data scie
-00000430: 6e63 6520 706c 6174 666f 726d 2c20 686f  nce platform, ho
-00000440: 7374 6564 220a 0a0a 6465 6620 7265 6e64  sted"...def rend
-00000450: 6572 5f63 6f6e 6669 6728 0a20 2020 2070  er_config(.    p
-00000460: 726f 6a65 6374 5f6e 616d 653a 2073 7472  roject_name: str
-00000470: 2c0a 2020 2020 6e65 6261 7269 5f64 6f6d  ,.    nebari_dom
-00000480: 6169 6e3a 2073 7472 203d 204e 6f6e 652c  ain: str = None,
-00000490: 0a20 2020 2063 6c6f 7564 5f70 726f 7669  .    cloud_provi
-000004a0: 6465 723a 2050 726f 7669 6465 7245 6e75  der: ProviderEnu
-000004b0: 6d20 3d20 5072 6f76 6964 6572 456e 756d  m = ProviderEnum
-000004c0: 2e6c 6f63 616c 2c0a 2020 2020 6369 5f70  .local,.    ci_p
-000004d0: 726f 7669 6465 723a 2043 6945 6e75 6d20  rovider: CiEnum 
-000004e0: 3d20 4369 456e 756d 2e6e 6f6e 652c 0a20  = CiEnum.none,. 
-000004f0: 2020 2072 6570 6f73 6974 6f72 793a 2073     repository: s
-00000500: 7472 203d 204e 6f6e 652c 0a20 2020 2061  tr = None,.    a
-00000510: 7574 685f 7072 6f76 6964 6572 3a20 4175  uth_provider: Au
-00000520: 7468 656e 7469 6361 7469 6f6e 456e 756d  thenticationEnum
-00000530: 203d 2041 7574 6865 6e74 6963 6174 696f   = Authenticatio
-00000540: 6e45 6e75 6d2e 7061 7373 776f 7264 2c0a  nEnum.password,.
-00000550: 2020 2020 6e61 6d65 7370 6163 653a 2073      namespace: s
-00000560: 7472 203d 2022 6465 7622 2c0a 2020 2020  tr = "dev",.    
-00000570: 7265 706f 7369 746f 7279 5f61 7574 6f5f  repository_auto_
-00000580: 7072 6f76 6973 696f 6e3a 2062 6f6f 6c20  provision: bool 
-00000590: 3d20 4661 6c73 652c 0a20 2020 2061 7574  = False,.    aut
-000005a0: 685f 6175 746f 5f70 726f 7669 7369 6f6e  h_auto_provision
-000005b0: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-000005c0: 2020 2020 7465 7272 6166 6f72 6d5f 7374      terraform_st
-000005d0: 6174 653a 2054 6572 7261 666f 726d 5374  ate: TerraformSt
-000005e0: 6174 6545 6e75 6d20 3d20 5465 7272 6166  ateEnum = Terraf
-000005f0: 6f72 6d53 7461 7465 456e 756d 2e72 656d  ormStateEnum.rem
-00000600: 6f74 652c 0a20 2020 206b 7562 6572 6e65  ote,.    kuberne
-00000610: 7465 735f 7665 7273 696f 6e3a 2073 7472  tes_version: str
-00000620: 203d 204e 6f6e 652c 0a20 2020 2072 6567   = None,.    reg
-00000630: 696f 6e3a 2073 7472 203d 204e 6f6e 652c  ion: str = None,
-00000640: 0a20 2020 2064 6973 6162 6c65 5f70 726f  .    disable_pro
-00000650: 6d70 743a 2062 6f6f 6c20 3d20 4661 6c73  mpt: bool = Fals
-00000660: 652c 0a20 2020 2073 736c 5f63 6572 745f  e,.    ssl_cert_
-00000670: 656d 6169 6c3a 2073 7472 203d 204e 6f6e  email: str = Non
-00000680: 652c 0a29 3a0a 2020 2020 636f 6e66 6967  e,.):.    config
-00000690: 203d 207b 0a20 2020 2020 2020 2022 7072   = {.        "pr
-000006a0: 6f76 6964 6572 223a 2063 6c6f 7564 5f70  ovider": cloud_p
-000006b0: 726f 7669 6465 722c 0a20 2020 2020 2020  rovider,.       
-000006c0: 2022 6e61 6d65 7370 6163 6522 3a20 6e61   "namespace": na
-000006d0: 6d65 7370 6163 652c 0a20 2020 2020 2020  mespace,.       
-000006e0: 2022 6e65 6261 7269 5f76 6572 7369 6f6e   "nebari_version
-000006f0: 223a 205f 5f76 6572 7369 6f6e 5f5f 2c0a  ": __version__,.
-00000700: 2020 2020 7d0a 0a20 2020 2069 6620 7072      }..    if pr
-00000710: 6f6a 6563 745f 6e61 6d65 2069 7320 4e6f  oject_name is No
-00000720: 6e65 2061 6e64 206e 6f74 2064 6973 6162  ne and not disab
-00000730: 6c65 5f70 726f 6d70 743a 0a20 2020 2020  le_prompt:.     
-00000740: 2020 2070 726f 6a65 6374 5f6e 616d 6520     project_name 
-00000750: 3d20 696e 7075 7428 2250 726f 7669 6465  = input("Provide
-00000760: 2070 726f 6a65 6374 206e 616d 653a 2022   project name: "
-00000770: 290a 2020 2020 636f 6e66 6967 5b22 7072  ).    config["pr
-00000780: 6f6a 6563 745f 6e61 6d65 225d 203d 2070  oject_name"] = p
-00000790: 726f 6a65 6374 5f6e 616d 650a 0a20 2020  roject_name..   
-000007a0: 2069 6620 6e65 6261 7269 5f64 6f6d 6169   if nebari_domai
-000007b0: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-000007c0: 2020 2020 2020 2063 6f6e 6669 675b 2264         config["d
-000007d0: 6f6d 6169 6e22 5d20 3d20 6e65 6261 7269  omain"] = nebari
-000007e0: 5f64 6f6d 6169 6e0a 0a20 2020 2063 6f6e  _domain..    con
-000007f0: 6669 675b 2263 695f 6364 225d 203d 207b  fig["ci_cd"] = {
-00000800: 2274 7970 6522 3a20 6369 5f70 726f 7669  "type": ci_provi
-00000810: 6465 727d 0a20 2020 2063 6f6e 6669 675b  der}.    config[
-00000820: 2274 6572 7261 666f 726d 5f73 7461 7465  "terraform_state
-00000830: 225d 203d 207b 2274 7970 6522 3a20 7465  "] = {"type": te
-00000840: 7272 6166 6f72 6d5f 7374 6174 657d 0a0a  rraform_state}..
-00000850: 2020 2020 2320 5361 7665 2064 6566 6175      # Save defau
-00000860: 6c74 2070 6173 7377 6f72 6420 746f 2066  lt password to f
-00000870: 696c 650a 2020 2020 6465 6661 756c 745f  ile.    default_
-00000880: 7061 7373 776f 7264 5f66 696c 656e 616d  password_filenam
-00000890: 6520 3d20 5061 7468 2874 656d 7066 696c  e = Path(tempfil
-000008a0: 652e 6765 7474 656d 7064 6972 2829 2920  e.gettempdir()) 
-000008b0: 2f20 224e 4542 4152 495f 4445 4641 554c  / "NEBARI_DEFAUL
-000008c0: 545f 5041 5353 574f 5244 220a 2020 2020  T_PASSWORD".    
-000008d0: 636f 6e66 6967 5b22 7365 6375 7269 7479  config["security
-000008e0: 225d 203d 207b 0a20 2020 2020 2020 2022  "] = {.        "
-000008f0: 6b65 7963 6c6f 616b 223a 207b 2269 6e69  keycloak": {"ini
-00000900: 7469 616c 5f72 6f6f 745f 7061 7373 776f  tial_root_passwo
-00000910: 7264 223a 2072 616e 646f 6d5f 7365 6375  rd": random_secu
-00000920: 7265 5f73 7472 696e 6728 6c65 6e67 7468  re_string(length
-00000930: 3d33 3229 7d0a 2020 2020 7d0a 2020 2020  =32)}.    }.    
-00000940: 7769 7468 2064 6566 6175 6c74 5f70 6173  with default_pas
-00000950: 7377 6f72 645f 6669 6c65 6e61 6d65 2e6f  sword_filename.o
-00000960: 7065 6e28 2277 2229 2061 7320 663a 0a20  pen("w") as f:. 
-00000970: 2020 2020 2020 2066 2e77 7269 7465 2863         f.write(c
-00000980: 6f6e 6669 675b 2273 6563 7572 6974 7922  onfig["security"
-00000990: 5d5b 226b 6579 636c 6f61 6b22 5d5b 2269  ]["keycloak"]["i
-000009a0: 6e69 7469 616c 5f72 6f6f 745f 7061 7373  nitial_root_pass
-000009b0: 776f 7264 225d 290a 2020 2020 6465 6661  word"]).    defa
-000009c0: 756c 745f 7061 7373 776f 7264 5f66 696c  ult_password_fil
-000009d0: 656e 616d 652e 6368 6d6f 6428 306f 3730  ename.chmod(0o70
-000009e0: 3029 0a0a 2020 2020 636f 6e66 6967 5b22  0)..    config["
-000009f0: 7468 656d 6522 5d20 3d20 7b22 6a75 7079  theme"] = {"jupy
-00000a00: 7465 7268 7562 223a 207b 2268 7562 5f74  terhub": {"hub_t
-00000a10: 6974 6c65 223a 2066 224e 6562 6172 6920  itle": f"Nebari 
-00000a20: 2d20 7b20 7072 6f6a 6563 745f 6e61 6d65  - { project_name
-00000a30: 207d 227d 7d0a 2020 2020 636f 6e66 6967   }"}}.    config
-00000a40: 5b22 7468 656d 6522 5d5b 226a 7570 7974  ["theme"]["jupyt
-00000a50: 6572 6875 6222 5d5b 0a20 2020 2020 2020  erhub"][.       
-00000a60: 2022 7765 6c63 6f6d 6522 0a20 2020 205d   "welcome".    ]
-00000a70: 203d 2022 2222 5765 6c63 6f6d 6521 204c   = """Welcome! L
-00000a80: 6561 726e 2061 626f 7574 204e 6562 6172  earn about Nebar
-00000a90: 6927 7320 6665 6174 7572 6573 2061 6e64  i's features and
-00000aa0: 2063 6f6e 6669 6775 7261 7469 6f6e 7320   configurations 
-00000ab0: 696e 203c 6120 6872 6566 3d22 6874 7470  in <a href="http
-00000ac0: 733a 2f2f 7777 772e 6e65 6261 7269 2e64  s://www.nebari.d
-00000ad0: 6576 2f64 6f63 732f 7765 6c63 6f6d 6522  ev/docs/welcome"
-00000ae0: 3e74 6865 2064 6f63 756d 656e 7461 7469  >the documentati
-00000af0: 6f6e 3c2f 613e 2e20 4966 2079 6f75 2068  on</a>. If you h
-00000b00: 6176 6520 616e 7920 7175 6573 7469 6f6e  ave any question
-00000b10: 7320 6f72 2066 6565 6462 6163 6b2c 2072  s or feedback, r
-00000b20: 6561 6368 2074 6865 2074 6561 6d20 6f6e  each the team on
-00000b30: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000b40: 2f2f 7777 772e 6e65 6261 7269 2e64 6576  //www.nebari.dev
-00000b50: 2f64 6f63 732f 636f 6d6d 756e 6974 7923  /docs/community#
-00000b60: 6765 7474 696e 672d 7375 7070 6f72 7422  getting-support"
-00000b70: 3e4e 6562 6172 6927 7320 7375 7070 6f72  >Nebari's suppor
-00000b80: 7420 666f 7275 6d73 3c2f 613e 2e22 2222  t forums</a>."""
-00000b90: 0a0a 2020 2020 636f 6e66 6967 5b22 7365  ..    config["se
-00000ba0: 6375 7269 7479 225d 5b22 6175 7468 656e  curity"]["authen
-00000bb0: 7469 6361 7469 6f6e 225d 203d 207b 2274  tication"] = {"t
-00000bc0: 7970 6522 3a20 6175 7468 5f70 726f 7669  ype": auth_provi
-00000bd0: 6465 727d 0a0a 2020 2020 6966 2061 7574  der}..    if aut
-00000be0: 685f 7072 6f76 6964 6572 203d 3d20 4175  h_provider == Au
-00000bf0: 7468 656e 7469 6361 7469 6f6e 456e 756d  thenticationEnum
-00000c00: 2e67 6974 6875 623a 0a20 2020 2020 2020  .github:.       
-00000c10: 2063 6f6e 6669 675b 2273 6563 7572 6974   config["securit
-00000c20: 7922 5d5b 2261 7574 6865 6e74 6963 6174  y"]["authenticat
-00000c30: 696f 6e22 5d5b 2263 6f6e 6669 6722 5d20  ion"]["config"] 
-00000c40: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00000c50: 2263 6c69 656e 745f 6964 223a 206f 732e  "client_id": os.
-00000c60: 656e 7669 726f 6e2e 6765 7428 0a20 2020  environ.get(.   
-00000c70: 2020 2020 2020 2020 2020 2020 2022 4749               "GI
-00000c80: 5448 5542 5f43 4c49 454e 545f 4944 222c  THUB_CLIENT_ID",
-00000c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ca0: 2022 3c65 6e74 6572 2063 6c69 656e 7420   "<enter client 
-00000cb0: 6964 206f 7220 7265 6d6f 7665 2074 6f20  id or remove to 
-00000cc0: 7573 6520 4749 5448 5542 5f43 4c49 454e  use GITHUB_CLIEN
-00000cd0: 545f 4944 2065 6e76 6972 6f6e 6d65 6e74  T_ID environment
-00000ce0: 2076 6172 6961 626c 6520 2870 7265 6665   variable (prefe
-00000cf0: 7272 6564 293e 222c 0a20 2020 2020 2020  rred)>",.       
-00000d00: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-00000d10: 2020 2020 2263 6c69 656e 745f 7365 6372      "client_secr
-00000d20: 6574 223a 206f 732e 656e 7669 726f 6e2e  et": os.environ.
-00000d30: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
-00000d40: 2020 2020 2022 4749 5448 5542 5f43 4c49       "GITHUB_CLI
-00000d50: 454e 545f 5345 4352 4554 222c 0a20 2020  ENT_SECRET",.   
-00000d60: 2020 2020 2020 2020 2020 2020 2022 3c65               "<e
-00000d70: 6e74 6572 2063 6c69 656e 7420 7365 6372  nter client secr
-00000d80: 6574 206f 7220 7265 6d6f 7665 2074 6f20  et or remove to 
-00000d90: 7573 6520 4749 5448 5542 5f43 4c49 454e  use GITHUB_CLIEN
-00000da0: 545f 5345 4352 4554 2065 6e76 6972 6f6e  T_SECRET environ
-00000db0: 6d65 6e74 2076 6172 6961 626c 6520 2870  ment variable (p
-00000dc0: 7265 6665 7272 6564 293e 222c 0a20 2020  referred)>",.   
-00000dd0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00000de0: 2020 2020 7d0a 2020 2020 656c 6966 2061      }.    elif a
-00000df0: 7574 685f 7072 6f76 6964 6572 203d 3d20  uth_provider == 
-00000e00: 4175 7468 656e 7469 6361 7469 6f6e 456e  AuthenticationEn
-00000e10: 756d 2e61 7574 6830 3a0a 2020 2020 2020  um.auth0:.      
-00000e20: 2020 6966 2061 7574 685f 6175 746f 5f70    if auth_auto_p
-00000e30: 726f 7669 7369 6f6e 3a0a 2020 2020 2020  rovision:.      
-00000e40: 2020 2020 2020 6175 7468 305f 636f 6e66        auth0_conf
-00000e50: 6967 203d 2063 7265 6174 655f 636c 6965  ig = create_clie
-00000e60: 6e74 2863 6f6e 6669 672e 646f 6d61 696e  nt(config.domain
-00000e70: 2c20 636f 6e66 6967 2e70 726f 6a65 6374  , config.project
-00000e80: 5f6e 616d 6529 0a20 2020 2020 2020 2020  _name).         
-00000e90: 2020 2063 6f6e 6669 675b 2273 6563 7572     config["secur
-00000ea0: 6974 7922 5d5b 2261 7574 6865 6e74 6963  ity"]["authentic
-00000eb0: 6174 696f 6e22 5d5b 2263 6f6e 6669 6722  ation"]["config"
-00000ec0: 5d20 3d20 6175 7468 305f 636f 6e66 6967  ] = auth0_config
-00000ed0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00000ee0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00000ef0: 675b 2273 6563 7572 6974 7922 5d5b 2261  g["security"]["a
-00000f00: 7574 6865 6e74 6963 6174 696f 6e22 5d5b  uthentication"][
-00000f10: 2263 6f6e 6669 6722 5d20 3d20 7b0a 2020  "config"] = {.  
-00000f20: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-00000f30: 6c69 656e 745f 6964 223a 206f 732e 656e  lient_id": os.en
-00000f40: 7669 726f 6e2e 6765 7428 0a20 2020 2020  viron.get(.     
-00000f50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000f60: 4155 5448 305f 434c 4945 4e54 5f49 4422  AUTH0_CLIENT_ID"
-00000f70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000f80: 2020 2020 2020 223c 656e 7465 7220 636c        "<enter cl
-00000f90: 6965 6e74 2069 6420 6f72 2072 656d 6f76  ient id or remov
-00000fa0: 6520 746f 2075 7365 2041 5554 4830 5f43  e to use AUTH0_C
-00000fb0: 4c49 454e 545f 4944 2065 6e76 6972 6f6e  LIENT_ID environ
-00000fc0: 6d65 6e74 2076 6172 6961 626c 6520 2870  ment variable (p
-00000fd0: 7265 6665 7272 6564 293e 222c 0a20 2020  referred)>",.   
-00000fe0: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001000: 2263 6c69 656e 745f 7365 6372 6574 223a  "client_secret":
-00001010: 206f 732e 656e 7669 726f 6e2e 6765 7428   os.environ.get(
-00001020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001030: 2020 2020 2022 4155 5448 305f 434c 4945       "AUTH0_CLIE
-00001040: 4e54 5f53 4543 5245 5422 2c0a 2020 2020  NT_SECRET",.    
-00001050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001060: 223c 656e 7465 7220 636c 6965 6e74 2073  "<enter client s
-00001070: 6563 7265 7420 6f72 2072 656d 6f76 6520  ecret or remove 
-00001080: 746f 2075 7365 2041 5554 4830 5f43 4c49  to use AUTH0_CLI
-00001090: 454e 545f 5345 4352 4554 2065 6e76 6972  ENT_SECRET envir
-000010a0: 6f6e 6d65 6e74 2076 6172 6961 626c 6520  onment variable 
-000010b0: 2870 7265 6665 7272 6564 293e 222c 0a20  (preferred)>",. 
-000010c0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000010d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000010e0: 2020 2261 7574 6830 5f73 7562 646f 6d61    "auth0_subdoma
-000010f0: 696e 223a 206f 732e 656e 7669 726f 6e2e  in": os.environ.
-00001100: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
-00001110: 2020 2020 2020 2020 2022 4155 5448 305f           "AUTH0_
-00001120: 444f 4d41 494e 222c 0a20 2020 2020 2020  DOMAIN",.       
-00001130: 2020 2020 2020 2020 2020 2020 2022 3c65               "<e
-00001140: 6e74 6572 2073 7562 646f 6d61 696e 2028  nter subdomain (
-00001150: 7769 7468 6f75 7420 2e61 7574 6830 2e63  without .auth0.c
-00001160: 6f6d 2920 6f72 2072 656d 6f76 6520 746f  om) or remove to
-00001170: 2075 7365 2041 5554 4830 5f44 4f4d 4149   use AUTH0_DOMAI
-00001180: 4e20 656e 7669 726f 6e6d 656e 7420 7661  N environment va
-00001190: 7269 6162 6c65 3e22 2c0a 2020 2020 2020  riable>",.      
-000011a0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-000011b0: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
-000011c0: 6966 2063 6c6f 7564 5f70 726f 7669 6465  if cloud_provide
-000011d0: 7220 3d3d 2050 726f 7669 6465 7245 6e75  r == ProviderEnu
-000011e0: 6d2e 646f 3a0a 2020 2020 2020 2020 646f  m.do:.        do
-000011f0: 5f72 6567 696f 6e20 3d20 7265 6769 6f6e  _region = region
-00001200: 206f 7220 636f 6e73 7461 6e74 732e 444f   or constants.DO
-00001210: 5f44 4546 4155 4c54 5f52 4547 494f 4e0a  _DEFAULT_REGION.
-00001220: 2020 2020 2020 2020 646f 5f6b 7562 6572          do_kuber
-00001230: 6e65 7465 735f 7665 7273 696f 6e73 203d  netes_versions =
-00001240: 206b 7562 6572 6e65 7465 735f 7665 7273   kubernetes_vers
-00001250: 696f 6e20 6f72 2067 6574 5f6c 6174 6573  ion or get_lates
-00001260: 745f 6b75 6265 726e 6574 6573 5f76 6572  t_kubernetes_ver
-00001270: 7369 6f6e 280a 2020 2020 2020 2020 2020  sion(.          
-00001280: 2020 6469 6769 7461 6c5f 6f63 6561 6e2e    digital_ocean.
-00001290: 6b75 6265 726e 6574 6573 5f76 6572 7369  kubernetes_versi
-000012a0: 6f6e 7328 646f 5f72 6567 696f 6e29 0a20  ons(do_region). 
-000012b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000012c0: 2063 6f6e 6669 675b 2264 6967 6974 616c   config["digital
-000012d0: 5f6f 6365 616e 225d 203d 207b 0a20 2020  _ocean"] = {.   
-000012e0: 2020 2020 2020 2020 2022 6b75 6265 726e           "kubern
-000012f0: 6574 6573 5f76 6572 7369 6f6e 223a 2064  etes_version": d
-00001300: 6f5f 6b75 6265 726e 6574 6573 5f76 6572  o_kubernetes_ver
-00001310: 7369 6f6e 732c 0a20 2020 2020 2020 2020  sions,.         
-00001320: 2020 2022 7265 6769 6f6e 223a 2064 6f5f     "region": do_
-00001330: 7265 6769 6f6e 2c0a 2020 2020 2020 2020  region,.        
-00001340: 2020 2020 226e 6f64 655f 6772 6f75 7073      "node_groups
-00001350: 223a 206e 6f64 655f 6772 6f75 7073 5f74  ": node_groups_t
-00001360: 6f5f 6469 6374 2844 4546 4155 4c54 5f44  o_dict(DEFAULT_D
-00001370: 4f5f 4e4f 4445 5f47 524f 5550 5329 2c0a  O_NODE_GROUPS),.
-00001380: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00001390: 2020 2063 6f6e 6669 675b 2274 6865 6d65     config["theme
-000013a0: 225d 5b22 6a75 7079 7465 7268 7562 225d  "]["jupyterhub"]
-000013b0: 5b0a 2020 2020 2020 2020 2020 2020 2268  [.            "h
-000013c0: 7562 5f73 7562 7469 746c 6522 0a20 2020  ub_subtitle".   
-000013d0: 2020 2020 205d 203d 2066 227b 5745 4c43       ] = f"{WELC
-000013e0: 4f4d 455f 4845 4144 4552 5f54 4558 547d  OME_HEADER_TEXT}
-000013f0: 206f 6e20 4469 6769 7461 6c20 4f63 6561   on Digital Ocea
-00001400: 6e22 0a0a 2020 2020 656c 6966 2063 6c6f  n"..    elif clo
-00001410: 7564 5f70 726f 7669 6465 7220 3d3d 2050  ud_provider == P
-00001420: 726f 7669 6465 7245 6e75 6d2e 6763 703a  roviderEnum.gcp:
-00001430: 0a20 2020 2020 2020 2067 6370 5f72 6567  .        gcp_reg
-00001440: 696f 6e20 3d20 7265 6769 6f6e 206f 7220  ion = region or 
-00001450: 636f 6e73 7461 6e74 732e 4743 505f 4445  constants.GCP_DE
-00001460: 4641 554c 545f 5245 4749 4f4e 0a20 2020  FAULT_REGION.   
-00001470: 2020 2020 2067 6370 5f6b 7562 6572 6e65       gcp_kuberne
-00001480: 7465 735f 7665 7273 696f 6e20 3d20 6b75  tes_version = ku
-00001490: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
-000014a0: 206f 7220 6765 745f 6c61 7465 7374 5f6b   or get_latest_k
-000014b0: 7562 6572 6e65 7465 735f 7665 7273 696f  ubernetes_versio
-000014c0: 6e28 0a20 2020 2020 2020 2020 2020 2067  n(.            g
-000014d0: 6f6f 676c 655f 636c 6f75 642e 6b75 6265  oogle_cloud.kube
-000014e0: 726e 6574 6573 5f76 6572 7369 6f6e 7328  rnetes_versions(
-000014f0: 6763 705f 7265 6769 6f6e 290a 2020 2020  gcp_region).    
-00001500: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
-00001510: 6e66 6967 5b22 676f 6f67 6c65 5f63 6c6f  nfig["google_clo
-00001520: 7564 5f70 6c61 7466 6f72 6d22 5d20 3d20  ud_platform"] = 
-00001530: 7b0a 2020 2020 2020 2020 2020 2020 226b  {.            "k
-00001540: 7562 6572 6e65 7465 735f 7665 7273 696f  ubernetes_versio
-00001550: 6e22 3a20 6763 705f 6b75 6265 726e 6574  n": gcp_kubernet
-00001560: 6573 5f76 6572 7369 6f6e 2c0a 2020 2020  es_version,.    
-00001570: 2020 2020 2020 2020 2272 6567 696f 6e22          "region"
-00001580: 3a20 6763 705f 7265 6769 6f6e 2c0a 2020  : gcp_region,.  
-00001590: 2020 2020 2020 2020 2020 226e 6f64 655f            "node_
-000015a0: 6772 6f75 7073 223a 206e 6f64 655f 6772  groups": node_gr
-000015b0: 6f75 7073 5f74 6f5f 6469 6374 2844 4546  oups_to_dict(DEF
-000015c0: 4155 4c54 5f47 4350 5f4e 4f44 455f 4752  AULT_GCP_NODE_GR
-000015d0: 4f55 5053 292c 0a20 2020 2020 2020 207d  OUPS),.        }
-000015e0: 0a0a 2020 2020 2020 2020 636f 6e66 6967  ..        config
-000015f0: 5b22 7468 656d 6522 5d5b 226a 7570 7974  ["theme"]["jupyt
-00001600: 6572 6875 6222 5d5b 0a20 2020 2020 2020  erhub"][.       
-00001610: 2020 2020 2022 6875 625f 7375 6274 6974       "hub_subtit
-00001620: 6c65 220a 2020 2020 2020 2020 5d20 3d20  le".        ] = 
-00001630: 6622 7b57 454c 434f 4d45 5f48 4541 4445  f"{WELCOME_HEADE
-00001640: 525f 5445 5854 7d20 6f6e 2047 6f6f 676c  R_TEXT} on Googl
-00001650: 6520 436c 6f75 6420 506c 6174 666f 726d  e Cloud Platform
-00001660: 220a 2020 2020 2020 2020 6966 2022 5052  ".        if "PR
-00001670: 4f4a 4543 545f 4944 2220 696e 206f 732e  OJECT_ID" in os.
-00001680: 656e 7669 726f 6e3a 0a20 2020 2020 2020  environ:.       
-00001690: 2020 2020 2063 6f6e 6669 675b 2267 6f6f       config["goo
-000016a0: 676c 655f 636c 6f75 645f 706c 6174 666f  gle_cloud_platfo
-000016b0: 726d 225d 5b22 7072 6f6a 6563 7422 5d20  rm"]["project"] 
-000016c0: 3d20 6f73 2e65 6e76 6972 6f6e 5b22 5052  = os.environ["PR
-000016d0: 4f4a 4543 545f 4944 225d 0a20 2020 2020  OJECT_ID"].     
-000016e0: 2020 2065 6c69 6620 6e6f 7420 6469 7361     elif not disa
-000016f0: 626c 655f 7072 6f6d 7074 3a0a 2020 2020  ble_prompt:.    
-00001700: 2020 2020 2020 2020 636f 6e66 6967 5b22          config["
-00001710: 676f 6f67 6c65 5f63 6c6f 7564 5f70 6c61  google_cloud_pla
-00001720: 7466 6f72 6d22 5d5b 2270 726f 6a65 6374  tform"]["project
-00001730: 225d 203d 2069 6e70 7574 280a 2020 2020  "] = input(.    
-00001740: 2020 2020 2020 2020 2020 2020 2245 6e74              "Ent
-00001750: 6572 2047 6f6f 676c 6520 436c 6f75 6420  er Google Cloud 
-00001760: 506c 6174 666f 726d 2050 726f 6a65 6374  Platform Project
-00001770: 2049 443a 2022 0a20 2020 2020 2020 2020   ID: ".         
-00001780: 2020 2029 0a0a 2020 2020 656c 6966 2063     )..    elif c
-00001790: 6c6f 7564 5f70 726f 7669 6465 7220 3d3d  loud_provider ==
-000017a0: 2050 726f 7669 6465 7245 6e75 6d2e 617a   ProviderEnum.az
-000017b0: 7572 653a 0a20 2020 2020 2020 2061 7a75  ure:.        azu
-000017c0: 7265 5f72 6567 696f 6e20 3d20 7265 6769  re_region = regi
-000017d0: 6f6e 206f 7220 636f 6e73 7461 6e74 732e  on or constants.
-000017e0: 415a 5552 455f 4445 4641 554c 545f 5245  AZURE_DEFAULT_RE
-000017f0: 4749 4f4e 0a20 2020 2020 2020 2061 7a75  GION.        azu
-00001800: 7265 5f6b 7562 6572 6e65 7465 735f 7665  re_kubernetes_ve
-00001810: 7273 696f 6e20 3d20 6b75 6265 726e 6574  rsion = kubernet
-00001820: 6573 5f76 6572 7369 6f6e 206f 7220 6765  es_version or ge
-00001830: 745f 6c61 7465 7374 5f6b 7562 6572 6e65  t_latest_kuberne
-00001840: 7465 735f 7665 7273 696f 6e28 0a20 2020  tes_version(.   
-00001850: 2020 2020 2020 2020 2061 7a75 7265 5f63           azure_c
-00001860: 6c6f 7564 2e6b 7562 6572 6e65 7465 735f  loud.kubernetes_
-00001870: 7665 7273 696f 6e73 2861 7a75 7265 5f72  versions(azure_r
-00001880: 6567 696f 6e29 0a20 2020 2020 2020 2029  egion).        )
-00001890: 0a20 2020 2020 2020 2063 6f6e 6669 675b  .        config[
-000018a0: 2261 7a75 7265 225d 203d 207b 0a20 2020  "azure"] = {.   
-000018b0: 2020 2020 2020 2020 2022 6b75 6265 726e           "kubern
-000018c0: 6574 6573 5f76 6572 7369 6f6e 223a 2061  etes_version": a
-000018d0: 7a75 7265 5f6b 7562 6572 6e65 7465 735f  zure_kubernetes_
-000018e0: 7665 7273 696f 6e2c 0a20 2020 2020 2020  version,.       
-000018f0: 2020 2020 2022 7265 6769 6f6e 223a 2061       "region": a
-00001900: 7a75 7265 5f72 6567 696f 6e2c 0a20 2020  zure_region,.   
-00001910: 2020 2020 2020 2020 2022 7374 6f72 6167           "storag
-00001920: 655f 6163 636f 756e 745f 706f 7374 6669  e_account_postfi
-00001930: 7822 3a20 7261 6e64 6f6d 5f73 6563 7572  x": random_secur
-00001940: 655f 7374 7269 6e67 286c 656e 6774 683d  e_string(length=
-00001950: 3429 2c0a 2020 2020 2020 2020 2020 2020  4),.            
-00001960: 226e 6f64 655f 6772 6f75 7073 223a 206e  "node_groups": n
-00001970: 6f64 655f 6772 6f75 7073 5f74 6f5f 6469  ode_groups_to_di
-00001980: 6374 2844 4546 4155 4c54 5f41 5a55 5245  ct(DEFAULT_AZURE
-00001990: 5f4e 4f44 455f 4752 4f55 5053 292c 0a20  _NODE_GROUPS),. 
-000019a0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-000019b0: 2020 636f 6e66 6967 5b22 7468 656d 6522    config["theme"
-000019c0: 5d5b 226a 7570 7974 6572 6875 6222 5d5b  ]["jupyterhub"][
-000019d0: 0a20 2020 2020 2020 2020 2020 2022 6875  .            "hu
-000019e0: 625f 7375 6274 6974 6c65 220a 2020 2020  b_subtitle".    
-000019f0: 2020 2020 5d20 3d20 6622 7b57 454c 434f      ] = f"{WELCO
-00001a00: 4d45 5f48 4541 4445 525f 5445 5854 7d20  ME_HEADER_TEXT} 
-00001a10: 6f6e 2041 7a75 7265 220a 0a20 2020 2065  on Azure"..    e
-00001a20: 6c69 6620 636c 6f75 645f 7072 6f76 6964  lif cloud_provid
-00001a30: 6572 203d 3d20 5072 6f76 6964 6572 456e  er == ProviderEn
-00001a40: 756d 2e61 7773 3a0a 2020 2020 2020 2020  um.aws:.        
-00001a50: 6177 735f 7265 6769 6f6e 203d 2028 0a20  aws_region = (. 
-00001a60: 2020 2020 2020 2020 2020 2072 6567 696f             regio
-00001a70: 6e0a 2020 2020 2020 2020 2020 2020 6f72  n.            or
-00001a80: 206f 732e 656e 7669 726f 6e2e 6765 7428   os.environ.get(
-00001a90: 2241 5753 5f44 4546 4155 4c54 5f52 4547  "AWS_DEFAULT_REG
-00001aa0: 494f 4e22 290a 2020 2020 2020 2020 2020  ION").          
-00001ab0: 2020 6f72 2063 6f6e 7374 616e 7473 2e41    or constants.A
-00001ac0: 5753 5f44 4546 4155 4c54 5f52 4547 494f  WS_DEFAULT_REGIO
-00001ad0: 4e0a 2020 2020 2020 2020 290a 2020 2020  N.        ).    
-00001ae0: 2020 2020 6177 735f 6b75 6265 726e 6574      aws_kubernet
-00001af0: 6573 5f76 6572 7369 6f6e 203d 206b 7562  es_version = kub
-00001b00: 6572 6e65 7465 735f 7665 7273 696f 6e20  ernetes_version 
-00001b10: 6f72 2067 6574 5f6c 6174 6573 745f 6b75  or get_latest_ku
-00001b20: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
-00001b30: 280a 2020 2020 2020 2020 2020 2020 616d  (.            am
-00001b40: 617a 6f6e 5f77 6562 5f73 6572 7669 6365  azon_web_service
-00001b50: 732e 6b75 6265 726e 6574 6573 5f76 6572  s.kubernetes_ver
-00001b60: 7369 6f6e 7328 6177 735f 7265 6769 6f6e  sions(aws_region
-00001b70: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-00001b80: 2020 2020 636f 6e66 6967 5b22 616d 617a      config["amaz
-00001b90: 6f6e 5f77 6562 5f73 6572 7669 6365 7322  on_web_services"
-00001ba0: 5d20 3d20 7b0a 2020 2020 2020 2020 2020  ] = {.          
-00001bb0: 2020 226b 7562 6572 6e65 7465 735f 7665    "kubernetes_ve
-00001bc0: 7273 696f 6e22 3a20 6177 735f 6b75 6265  rsion": aws_kube
-00001bd0: 726e 6574 6573 5f76 6572 7369 6f6e 2c0a  rnetes_version,.
-00001be0: 2020 2020 2020 2020 2020 2020 2272 6567              "reg
-00001bf0: 696f 6e22 3a20 6177 735f 7265 6769 6f6e  ion": aws_region
-00001c00: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
-00001c10: 6f64 655f 6772 6f75 7073 223a 206e 6f64  ode_groups": nod
-00001c20: 655f 6772 6f75 7073 5f74 6f5f 6469 6374  e_groups_to_dict
-00001c30: 2844 4546 4155 4c54 5f41 5753 5f4e 4f44  (DEFAULT_AWS_NOD
-00001c40: 455f 4752 4f55 5053 292c 0a20 2020 2020  E_GROUPS),.     
-00001c50: 2020 207d 0a20 2020 2020 2020 2063 6f6e     }.        con
-00001c60: 6669 675b 2274 6865 6d65 225d 5b22 6a75  fig["theme"]["ju
-00001c70: 7079 7465 7268 7562 225d 5b0a 2020 2020  pyterhub"][.    
-00001c80: 2020 2020 2020 2020 2268 7562 5f73 7562          "hub_sub
-00001c90: 7469 746c 6522 0a20 2020 2020 2020 205d  title".        ]
-00001ca0: 203d 2066 227b 5745 4c43 4f4d 455f 4845   = f"{WELCOME_HE
-00001cb0: 4144 4552 5f54 4558 547d 206f 6e20 416d  ADER_TEXT} on Am
-00001cc0: 617a 6f6e 2057 6562 2053 6572 7669 6365  azon Web Service
-00001cd0: 7322 0a0a 2020 2020 656c 6966 2063 6c6f  s"..    elif clo
-00001ce0: 7564 5f70 726f 7669 6465 7220 3d3d 2050  ud_provider == P
-00001cf0: 726f 7669 6465 7245 6e75 6d2e 6578 6973  roviderEnum.exis
-00001d00: 7469 6e67 3a0a 2020 2020 2020 2020 636f  ting:.        co
-00001d10: 6e66 6967 5b22 7468 656d 6522 5d5b 226a  nfig["theme"]["j
-00001d20: 7570 7974 6572 6875 6222 5d5b 2268 7562  upyterhub"]["hub
-00001d30: 5f73 7562 7469 746c 6522 5d20 3d20 5745  _subtitle"] = WE
-00001d40: 4c43 4f4d 455f 4845 4144 4552 5f54 4558  LCOME_HEADER_TEX
-00001d50: 540a 0a20 2020 2065 6c69 6620 636c 6f75  T..    elif clou
-00001d60: 645f 7072 6f76 6964 6572 203d 3d20 5072  d_provider == Pr
-00001d70: 6f76 6964 6572 456e 756d 2e6c 6f63 616c  oviderEnum.local
-00001d80: 3a0a 2020 2020 2020 2020 636f 6e66 6967  :.        config
-00001d90: 5b22 7468 656d 6522 5d5b 226a 7570 7974  ["theme"]["jupyt
-00001da0: 6572 6875 6222 5d5b 2268 7562 5f73 7562  erhub"]["hub_sub
-00001db0: 7469 746c 6522 5d20 3d20 5745 4c43 4f4d  title"] = WELCOM
-00001dc0: 455f 4845 4144 4552 5f54 4558 540a 0a20  E_HEADER_TEXT.. 
-00001dd0: 2020 2069 6620 7373 6c5f 6365 7274 5f65     if ssl_cert_e
-00001de0: 6d61 696c 3a0a 2020 2020 2020 2020 636f  mail:.        co
-00001df0: 6e66 6967 5b22 6365 7274 6966 6963 6174  nfig["certificat
-00001e00: 6522 5d20 3d20 7b22 7479 7065 223a 2043  e"] = {"type": C
-00001e10: 6572 7469 6669 6361 7465 456e 756d 2e6c  ertificateEnum.l
-00001e20: 6574 7365 6e63 7279 7074 2e76 616c 7565  etsencrypt.value
-00001e30: 7d0a 2020 2020 2020 2020 636f 6e66 6967  }.        config
-00001e40: 5b22 6365 7274 6966 6963 6174 6522 5d5b  ["certificate"][
-00001e50: 2261 636d 655f 656d 6169 6c22 5d20 3d20  "acme_email"] = 
-00001e60: 7373 6c5f 6365 7274 5f65 6d61 696c 0a0a  ssl_cert_email..
-00001e70: 2020 2020 2320 7661 6c69 6461 7465 2063      # validate c
-00001e80: 6f6e 6669 6775 7261 7469 6f6e 2061 6e64  onfiguration and
-00001e90: 2063 6f6e 7665 7274 2074 6f20 6d6f 6465   convert to mode
-00001ea0: 6c0a 2020 2020 6672 6f6d 206e 6562 6172  l.    from nebar
-00001eb0: 692e 706c 7567 696e 7320 696d 706f 7274  i.plugins import
-00001ec0: 206e 6562 6172 695f 706c 7567 696e 5f6d   nebari_plugin_m
-00001ed0: 616e 6167 6572 0a0a 2020 2020 7472 793a  anager..    try:
-00001ee0: 0a20 2020 2020 2020 2063 6f6e 6669 675f  .        config_
-00001ef0: 6d6f 6465 6c20 3d20 6e65 6261 7269 5f70  model = nebari_p
-00001f00: 6c75 6769 6e5f 6d61 6e61 6765 722e 636f  lugin_manager.co
-00001f10: 6e66 6967 5f73 6368 656d 612e 7061 7273  nfig_schema.pars
-00001f20: 655f 6f62 6a28 636f 6e66 6967 290a 2020  e_obj(config).  
-00001f30: 2020 6578 6365 7074 2070 7964 616e 7469    except pydanti
-00001f40: 632e 5661 6c69 6461 7469 6f6e 4572 726f  c.ValidationErro
-00001f50: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
-00001f60: 7072 696e 7428 7374 7228 6529 290a 0a20  print(str(e)).. 
-00001f70: 2020 2069 6620 7265 706f 7369 746f 7279     if repository
-00001f80: 5f61 7574 6f5f 7072 6f76 6973 696f 6e3a  _auto_provision:
-00001f90: 0a20 2020 2020 2020 206d 6174 6368 203d  .        match =
-00001fa0: 2072 652e 7365 6172 6368 2867 6974 6875   re.search(githu
-00001fb0: 625f 7572 6c5f 7265 6765 782c 2072 6570  b_url_regex, rep
-00001fc0: 6f73 6974 6f72 7929 0a20 2020 2020 2020  ository).       
-00001fd0: 2069 6620 6d61 7463 683a 0a20 2020 2020   if match:.     
-00001fe0: 2020 2020 2020 2067 6974 5f72 6570 6f73         git_repos
-00001ff0: 6974 6f72 7920 3d20 6769 7468 7562 5f61  itory = github_a
-00002000: 7574 6f5f 7072 6f76 6973 696f 6e28 0a20  uto_provision(. 
-00002010: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00002020: 6f6e 6669 675f 6d6f 6465 6c2c 206d 6174  onfig_model, mat
-00002030: 6368 2e67 726f 7570 2832 292c 206d 6174  ch.group(2), mat
-00002040: 6368 2e67 726f 7570 2833 290a 2020 2020  ch.group(3).    
-00002050: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00002060: 2020 2020 2020 6769 745f 7265 706f 7369        git_reposi
-00002070: 746f 7279 5f69 6e69 7469 616c 697a 6528  tory_initialize(
-00002080: 6769 745f 7265 706f 7369 746f 7279 290a  git_repository).
-00002090: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000020a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000020b0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-000020c0: 2020 2020 2020 2020 2020 2020 6622 5265              f"Re
-000020d0: 706f 7369 746f 7279 2074 6f20 6265 2061  pository to be a
-000020e0: 7574 6f2d 7072 6f76 6973 696f 6e65 6420  uto-provisioned 
-000020f0: 6973 206e 6f74 2074 6865 2066 756c 6c20  is not the full 
-00002100: 5552 4c20 6f66 2061 2047 6974 4875 6220  URL of a GitHub 
-00002110: 7265 706f 3a20 7b72 6570 6f73 6974 6f72  repo: {repositor
-00002120: 797d 220a 2020 2020 2020 2020 2020 2020  y}".            
-00002130: 290a 0a20 2020 2072 6574 7572 6e20 636f  )..    return co
-00002140: 6e66 6967 0a0a 0a64 6566 2067 6974 6875  nfig...def githu
-00002150: 625f 6175 746f 5f70 726f 7669 7369 6f6e  b_auto_provision
-00002160: 2863 6f6e 6669 673a 2070 7964 616e 7469  (config: pydanti
-00002170: 632e 4261 7365 4d6f 6465 6c2c 206f 776e  c.BaseModel, own
-00002180: 6572 3a20 7374 722c 2072 6570 6f3a 2073  er: str, repo: s
-00002190: 7472 293a 0a20 2020 2061 6c72 6561 6479  tr):.    already
-000021a0: 5f65 7869 7374 7320 3d20 5472 7565 0a20  _exists = True. 
-000021b0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000021c0: 6769 7468 7562 2e67 6574 5f72 6570 6f73  github.get_repos
-000021d0: 6974 6f72 7928 6f77 6e65 722c 2072 6570  itory(owner, rep
-000021e0: 6f29 0a20 2020 2065 7863 6570 7420 7265  o).    except re
-000021f0: 7175 6573 7473 2e65 7863 6570 7469 6f6e  quests.exception
-00002200: 732e 4854 5450 4572 726f 723a 0a20 2020  s.HTTPError:.   
-00002210: 2020 2020 2023 2072 6570 6f20 6e6f 7420       # repo not 
-00002220: 666f 756e 640a 2020 2020 2020 2020 616c  found.        al
-00002230: 7265 6164 795f 6578 6973 7473 203d 2046  ready_exists = F
-00002240: 616c 7365 0a0a 2020 2020 6966 206e 6f74  alse..    if not
-00002250: 2061 6c72 6561 6479 5f65 7869 7374 733a   already_exists:
-00002260: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00002270: 2020 2020 2020 2020 2020 6769 7468 7562            github
-00002280: 2e63 7265 6174 655f 7265 706f 7369 746f  .create_reposito
-00002290: 7279 280a 2020 2020 2020 2020 2020 2020  ry(.            
-000022a0: 2020 2020 6f77 6e65 722c 0a20 2020 2020      owner,.     
-000022b0: 2020 2020 2020 2020 2020 2072 6570 6f2c             repo,
-000022c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000022d0: 2064 6573 6372 6970 7469 6f6e 3d66 224e   description=f"N
-000022e0: 6562 6172 6920 7b63 6f6e 6669 672e 7072  ebari {config.pr
-000022f0: 6f6a 6563 745f 6e61 6d65 7d2d 7b63 6f6e  oject_name}-{con
-00002300: 6669 672e 7072 6f76 6964 6572 7d22 2c0a  fig.provider}",.
-00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002320: 686f 6d65 7061 6765 3d66 2268 7474 7073  homepage=f"https
-00002330: 3a2f 2f7b 636f 6e66 6967 2e64 6f6d 6169  ://{config.domai
-00002340: 6e7d 222c 0a20 2020 2020 2020 2020 2020  n}",.           
-00002350: 2029 0a20 2020 2020 2020 2065 7863 6570   ).        excep
-00002360: 7420 7265 7175 6573 7473 2e65 7863 6570  t requests.excep
-00002370: 7469 6f6e 732e 4854 5450 4572 726f 7220  tions.HTTPError 
-00002380: 6173 2068 653a 0a20 2020 2020 2020 2020  as he:.         
-00002390: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-000023a0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-000023b0: 2020 2020 2066 2255 6e61 626c 6520 746f       f"Unable to
-000023c0: 2063 7265 6174 6520 4769 7448 7562 2072   create GitHub r
-000023d0: 6570 6f20 6874 7470 733a 2f2f 6769 7468  epo https://gith
-000023e0: 7562 2e63 6f6d 2f7b 6f77 6e65 727d 2f7b  ub.com/{owner}/{
-000023f0: 7265 706f 7d20 2d20 6572 726f 7220 6d65  repo} - error me
-00002400: 7373 6167 6520 6672 6f6d 2047 6974 4875  ssage from GitHu
-00002410: 6220 6973 3a20 7b68 657d 220a 2020 2020  b is: {he}".    
-00002420: 2020 2020 2020 2020 290a 2020 2020 656c          ).    el
-00002430: 7365 3a0a 2020 2020 2020 2020 6c6f 6767  se:.        logg
-00002440: 6572 2e77 6172 6e69 6e67 2866 2247 6974  er.warning(f"Git
-00002450: 4875 6220 7265 706f 2068 7474 7073 3a2f  Hub repo https:/
-00002460: 2f67 6974 6875 622e 636f 6d2f 7b6f 776e  /github.com/{own
-00002470: 6572 7d2f 7b72 6570 6f7d 2061 6c72 6561  er}/{repo} alrea
-00002480: 6479 2065 7869 7374 7322 290a 0a20 2020  dy exists")..   
-00002490: 2074 7279 3a0a 2020 2020 2020 2020 2320   try:.        # 
-000024a0: 5365 6372 6574 730a 2020 2020 2020 2020  Secrets.        
-000024b0: 6966 2063 6f6e 6669 672e 7072 6f76 6964  if config.provid
-000024c0: 6572 203d 3d20 5072 6f76 6964 6572 456e  er == ProviderEn
-000024d0: 756d 2e64 6f3a 0a20 2020 2020 2020 2020  um.do:.         
-000024e0: 2020 2066 6f72 206e 616d 6520 696e 207b     for name in {
-000024f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002500: 2022 4157 535f 4143 4345 5353 5f4b 4559   "AWS_ACCESS_KEY
-00002510: 5f49 4422 2c0a 2020 2020 2020 2020 2020  _ID",.          
-00002520: 2020 2020 2020 2241 5753 5f53 4543 5245        "AWS_SECRE
-00002530: 545f 4143 4345 5353 5f4b 4559 222c 0a20  T_ACCESS_KEY",. 
-00002540: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002550: 5350 4143 4553 5f41 4343 4553 535f 4b45  SPACES_ACCESS_KE
-00002560: 595f 4944 222c 0a20 2020 2020 2020 2020  Y_ID",.         
-00002570: 2020 2020 2020 2022 5350 4143 4553 5f53         "SPACES_S
-00002580: 4543 5245 545f 4143 4345 5353 5f4b 4559  ECRET_ACCESS_KEY
-00002590: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000025a0: 2020 2022 4449 4749 5441 4c4f 4345 414e     "DIGITALOCEAN
-000025b0: 5f54 4f4b 454e 222c 0a20 2020 2020 2020  _TOKEN",.       
-000025c0: 2020 2020 207d 3a0a 2020 2020 2020 2020       }:.        
-000025d0: 2020 2020 2020 2020 6769 7468 7562 2e75          github.u
-000025e0: 7064 6174 655f 7365 6372 6574 286f 776e  pdate_secret(own
-000025f0: 6572 2c20 7265 706f 2c20 6e61 6d65 2c20  er, repo, name, 
-00002600: 6f73 2e65 6e76 6972 6f6e 5b6e 616d 655d  os.environ[name]
-00002610: 290a 2020 2020 2020 2020 656c 6966 2063  ).        elif c
-00002620: 6f6e 6669 672e 7072 6f76 6964 6572 203d  onfig.provider =
-00002630: 3d20 5072 6f76 6964 6572 456e 756d 2e61  = ProviderEnum.a
-00002640: 7773 3a0a 2020 2020 2020 2020 2020 2020  ws:.            
-00002650: 666f 7220 6e61 6d65 2069 6e20 7b0a 2020  for name in {.  
-00002660: 2020 2020 2020 2020 2020 2020 2020 2241                "A
-00002670: 5753 5f41 4343 4553 535f 4b45 595f 4944  WS_ACCESS_KEY_ID
-00002680: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002690: 2020 2022 4157 535f 5345 4352 4554 5f41     "AWS_SECRET_A
-000026a0: 4343 4553 535f 4b45 5922 2c0a 2020 2020  CCESS_KEY",.    
-000026b0: 2020 2020 2020 2020 7d3a 0a20 2020 2020          }:.     
-000026c0: 2020 2020 2020 2020 2020 2067 6974 6875             githu
-000026d0: 622e 7570 6461 7465 5f73 6563 7265 7428  b.update_secret(
-000026e0: 6f77 6e65 722c 2072 6570 6f2c 206e 616d  owner, repo, nam
-000026f0: 652c 206f 732e 656e 7669 726f 6e5b 6e61  e, os.environ[na
-00002700: 6d65 5d29 0a20 2020 2020 2020 2065 6c69  me]).        eli
-00002710: 6620 636f 6e66 6967 2e70 726f 7669 6465  f config.provide
-00002720: 7220 3d3d 2050 726f 7669 6465 7245 6e75  r == ProviderEnu
-00002730: 6d2e 6763 703a 0a20 2020 2020 2020 2020  m.gcp:.         
-00002740: 2020 2067 6974 6875 622e 7570 6461 7465     github.update
-00002750: 5f73 6563 7265 7428 6f77 6e65 722c 2072  _secret(owner, r
-00002760: 6570 6f2c 2022 5052 4f4a 4543 545f 4944  epo, "PROJECT_ID
-00002770: 222c 206f 732e 656e 7669 726f 6e5b 2250  ", os.environ["P
-00002780: 524f 4a45 4354 5f49 4422 5d29 0a20 2020  ROJECT_ID"]).   
-00002790: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-000027a0: 656e 286f 732e 656e 7669 726f 6e5b 2247  en(os.environ["G
-000027b0: 4f4f 474c 455f 4352 4544 454e 5449 414c  OOGLE_CREDENTIAL
-000027c0: 5322 5d29 2061 7320 663a 0a20 2020 2020  S"]) as f:.     
-000027d0: 2020 2020 2020 2020 2020 2067 6974 6875             githu
-000027e0: 622e 7570 6461 7465 5f73 6563 7265 7428  b.update_secret(
-000027f0: 6f77 6e65 722c 2072 6570 6f2c 2022 474f  owner, repo, "GO
-00002800: 4f47 4c45 5f43 5245 4445 4e54 4941 4c53  OGLE_CREDENTIALS
-00002810: 222c 2066 2e72 6561 6428 2929 0a20 2020  ", f.read()).   
-00002820: 2020 2020 2065 6c69 6620 636f 6e66 6967       elif config
-00002830: 2e70 726f 7669 6465 7220 3d3d 2050 726f  .provider == Pro
-00002840: 7669 6465 7245 6e75 6d2e 617a 7572 653a  viderEnum.azure:
-00002850: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00002860: 206e 616d 6520 696e 207b 0a20 2020 2020   name in {.     
-00002870: 2020 2020 2020 2020 2020 2022 4152 4d5f             "ARM_
-00002880: 434c 4945 4e54 5f49 4422 2c0a 2020 2020  CLIENT_ID",.    
-00002890: 2020 2020 2020 2020 2020 2020 2241 524d              "ARM
-000028a0: 5f43 4c49 454e 545f 5345 4352 4554 222c  _CLIENT_SECRET",
-000028b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000028c0: 2022 4152 4d5f 5355 4253 4352 4950 5449   "ARM_SUBSCRIPTI
-000028d0: 4f4e 5f49 4422 2c0a 2020 2020 2020 2020  ON_ID",.        
-000028e0: 2020 2020 2020 2020 2241 524d 5f54 454e          "ARM_TEN
-000028f0: 414e 545f 4944 222c 0a20 2020 2020 2020  ANT_ID",.       
-00002900: 2020 2020 207d 3a0a 2020 2020 2020 2020       }:.        
-00002910: 2020 2020 2020 2020 6769 7468 7562 2e75          github.u
-00002920: 7064 6174 655f 7365 6372 6574 286f 776e  pdate_secret(own
-00002930: 6572 2c20 7265 706f 2c20 6e61 6d65 2c20  er, repo, name, 
-00002940: 6f73 2e65 6e76 6972 6f6e 5b6e 616d 655d  os.environ[name]
-00002950: 290a 2020 2020 2020 2020 6769 7468 7562  ).        github
-00002960: 2e75 7064 6174 655f 7365 6372 6574 280a  .update_secret(.
-00002970: 2020 2020 2020 2020 2020 2020 6f77 6e65              owne
-00002980: 722c 2072 6570 6f2c 2022 5245 504f 5349  r, repo, "REPOSI
-00002990: 544f 5259 5f41 4343 4553 535f 544f 4b45  TORY_ACCESS_TOKE
-000029a0: 4e22 2c20 6f73 2e65 6e76 6972 6f6e 5b22  N", os.environ["
-000029b0: 4749 5448 5542 5f54 4f4b 454e 225d 0a20  GITHUB_TOKEN"]. 
-000029c0: 2020 2020 2020 2029 0a20 2020 2065 7863         ).    exc
-000029d0: 6570 7420 7265 7175 6573 7473 2e65 7863  ept requests.exc
-000029e0: 6570 7469 6f6e 732e 4854 5450 4572 726f  eptions.HTTPErro
-000029f0: 7220 6173 2068 653a 0a20 2020 2020 2020  r as he:.       
-00002a00: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00002a10: 7228 0a20 2020 2020 2020 2020 2020 2066  r(.            f
-00002a20: 2255 6e61 626c 6520 746f 2073 6574 2053  "Unable to set S
-00002a30: 6563 7265 7473 206f 6e20 4769 7448 7562  ecrets on GitHub
-00002a40: 2072 6570 6f20 6874 7470 733a 2f2f 6769   repo https://gi
-00002a50: 7468 7562 2e63 6f6d 2f7b 6f77 6e65 727d  thub.com/{owner}
-00002a60: 2f7b 7265 706f 7d20 2d20 6572 726f 7220  /{repo} - error 
-00002a70: 6d65 7373 6167 6520 6672 6f6d 2047 6974  message from Git
-00002a80: 4875 6220 6973 3a20 7b68 657d 220a 2020  Hub is: {he}".  
-00002a90: 2020 2020 2020 290a 0a20 2020 2072 6574        )..    ret
-00002aa0: 7572 6e20 6622 6769 7440 6769 7468 7562  urn f"git@github
-00002ab0: 2e63 6f6d 3a7b 6f77 6e65 727d 2f7b 7265  .com:{owner}/{re
-00002ac0: 706f 7d2e 6769 7422 0a0a 0a64 6566 2067  po}.git"...def g
-00002ad0: 6974 5f72 6570 6f73 6974 6f72 795f 696e  it_repository_in
-00002ae0: 6974 6961 6c69 7a65 2867 6974 5f72 6570  itialize(git_rep
-00002af0: 6f73 6974 6f72 7929 3a0a 2020 2020 6966  ository):.    if
-00002b00: 206e 6f74 2067 6974 2e69 735f 6769 745f   not git.is_git_
-00002b10: 7265 706f 2850 6174 682e 6377 6428 2929  repo(Path.cwd())
-00002b20: 3a0a 2020 2020 2020 2020 6769 742e 696e  :.        git.in
-00002b30: 6974 6961 6c69 7a65 5f67 6974 2850 6174  itialize_git(Pat
-00002b40: 682e 6377 6428 2929 0a20 2020 2067 6974  h.cwd()).    git
-00002b50: 2e61 6464 5f67 6974 5f72 656d 6f74 6528  .add_git_remote(
-00002b60: 6769 745f 7265 706f 7369 746f 7279 2c20  git_repository, 
-00002b70: 7061 7468 3d50 6174 682e 6377 6428 292c  path=Path.cwd(),
-00002b80: 2072 656d 6f74 655f 6e61 6d65 3d22 6f72   remote_name="or
-00002b90: 6967 696e 2229 0a                        igin").
+00000250: 290a 6672 6f6d 205f 6e65 6261 7269 2e73  ).from _nebari.s
+00000260: 7461 6765 732e 6b75 6265 726e 6574 6573  tages.kubernetes
+00000270: 5f69 6e67 7265 7373 2069 6d70 6f72 7420  _ingress import 
+00000280: 4365 7274 6966 6963 6174 6545 6e75 6d0a  CertificateEnum.
+00000290: 6672 6f6d 205f 6e65 6261 7269 2e73 7461  from _nebari.sta
+000002a0: 6765 732e 6b75 6265 726e 6574 6573 5f6b  ges.kubernetes_k
+000002b0: 6579 636c 6f61 6b20 696d 706f 7274 2041  eycloak import A
+000002c0: 7574 6865 6e74 6963 6174 696f 6e45 6e75  uthenticationEnu
+000002d0: 6d0a 6672 6f6d 205f 6e65 6261 7269 2e73  m.from _nebari.s
+000002e0: 7461 6765 732e 7465 7272 6166 6f72 6d5f  tages.terraform_
+000002f0: 7374 6174 6520 696d 706f 7274 2054 6572  state import Ter
+00000300: 7261 666f 726d 5374 6174 6545 6e75 6d0a  raformStateEnum.
+00000310: 6672 6f6d 205f 6e65 6261 7269 2e75 7469  from _nebari.uti
+00000320: 6c73 2069 6d70 6f72 7420 6765 745f 6c61  ls import get_la
+00000330: 7465 7374 5f6b 7562 6572 6e65 7465 735f  test_kubernetes_
+00000340: 7665 7273 696f 6e2c 2072 616e 646f 6d5f  version, random_
+00000350: 7365 6375 7265 5f73 7472 696e 670a 6672  secure_string.fr
+00000360: 6f6d 205f 6e65 6261 7269 2e76 6572 7369  om _nebari.versi
+00000370: 6f6e 2069 6d70 6f72 7420 5f5f 7665 7273  on import __vers
+00000380: 696f 6e5f 5f0a 6672 6f6d 206e 6562 6172  ion__.from nebar
+00000390: 692e 7363 6865 6d61 2069 6d70 6f72 7420  i.schema import 
+000003a0: 5072 6f76 6964 6572 456e 756d 2c20 6769  ProviderEnum, gi
+000003b0: 7468 7562 5f75 726c 5f72 6567 6578 0a0a  thub_url_regex..
+000003c0: 6c6f 6767 6572 203d 206c 6f67 6769 6e67  logger = logging
+000003d0: 2e67 6574 4c6f 6767 6572 285f 5f6e 616d  .getLogger(__nam
+000003e0: 655f 5f29 0a0a 5745 4c43 4f4d 455f 4845  e__)..WELCOME_HE
+000003f0: 4144 4552 5f54 4558 5420 3d20 2259 6f75  ADER_TEXT = "You
+00000400: 7220 6f70 656e 2073 6f75 7263 6520 6461  r open source da
+00000410: 7461 2073 6369 656e 6365 2070 6c61 7466  ta science platf
+00000420: 6f72 6d2c 2068 6f73 7465 6422 0a0a 0a64  orm, hosted"...d
+00000430: 6566 205f 6e6f 6465 5f67 726f 7570 735f  ef _node_groups_
+00000440: 746f 5f64 6963 7428 6e6f 6465 5f67 726f  to_dict(node_gro
+00000450: 7570 7329 3a0a 2020 2020 7265 7475 726e  ups):.    return
+00000460: 207b 6e67 5f6e 616d 653a 206e 672e 6469   {ng_name: ng.di
+00000470: 6374 2829 2066 6f72 206e 675f 6e61 6d65  ct() for ng_name
+00000480: 2c20 6e67 2069 6e20 6e6f 6465 5f67 726f  , ng in node_gro
+00000490: 7570 732e 6974 656d 7328 297d 0a0a 0a64  ups.items()}...d
+000004a0: 6566 2072 656e 6465 725f 636f 6e66 6967  ef render_config
+000004b0: 280a 2020 2020 7072 6f6a 6563 745f 6e61  (.    project_na
+000004c0: 6d65 3a20 7374 722c 0a20 2020 206e 6562  me: str,.    neb
+000004d0: 6172 695f 646f 6d61 696e 3a20 7374 7220  ari_domain: str 
+000004e0: 3d20 4e6f 6e65 2c0a 2020 2020 636c 6f75  = None,.    clou
+000004f0: 645f 7072 6f76 6964 6572 3a20 5072 6f76  d_provider: Prov
+00000500: 6964 6572 456e 756d 203d 2050 726f 7669  iderEnum = Provi
+00000510: 6465 7245 6e75 6d2e 6c6f 6361 6c2c 0a20  derEnum.local,. 
+00000520: 2020 2063 695f 7072 6f76 6964 6572 3a20     ci_provider: 
+00000530: 4369 456e 756d 203d 2043 6945 6e75 6d2e  CiEnum = CiEnum.
+00000540: 6e6f 6e65 2c0a 2020 2020 7265 706f 7369  none,.    reposi
+00000550: 746f 7279 3a20 7374 7220 3d20 4e6f 6e65  tory: str = None
+00000560: 2c0a 2020 2020 6175 7468 5f70 726f 7669  ,.    auth_provi
+00000570: 6465 723a 2041 7574 6865 6e74 6963 6174  der: Authenticat
+00000580: 696f 6e45 6e75 6d20 3d20 4175 7468 656e  ionEnum = Authen
+00000590: 7469 6361 7469 6f6e 456e 756d 2e70 6173  ticationEnum.pas
+000005a0: 7377 6f72 642c 0a20 2020 206e 616d 6573  sword,.    names
+000005b0: 7061 6365 3a20 7374 7220 3d20 2264 6576  pace: str = "dev
+000005c0: 222c 0a20 2020 2072 6570 6f73 6974 6f72  ",.    repositor
+000005d0: 795f 6175 746f 5f70 726f 7669 7369 6f6e  y_auto_provision
+000005e0: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+000005f0: 2020 2020 6175 7468 5f61 7574 6f5f 7072      auth_auto_pr
+00000600: 6f76 6973 696f 6e3a 2062 6f6f 6c20 3d20  ovision: bool = 
+00000610: 4661 6c73 652c 0a20 2020 2074 6572 7261  False,.    terra
+00000620: 666f 726d 5f73 7461 7465 3a20 5465 7272  form_state: Terr
+00000630: 6166 6f72 6d53 7461 7465 456e 756d 203d  aformStateEnum =
+00000640: 2054 6572 7261 666f 726d 5374 6174 6545   TerraformStateE
+00000650: 6e75 6d2e 7265 6d6f 7465 2c0a 2020 2020  num.remote,.    
+00000660: 6b75 6265 726e 6574 6573 5f76 6572 7369  kubernetes_versi
+00000670: 6f6e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  on: str = None,.
+00000680: 2020 2020 7265 6769 6f6e 3a20 7374 7220      region: str 
+00000690: 3d20 4e6f 6e65 2c0a 2020 2020 6469 7361  = None,.    disa
+000006a0: 626c 655f 7072 6f6d 7074 3a20 626f 6f6c  ble_prompt: bool
+000006b0: 203d 2046 616c 7365 2c0a 2020 2020 7373   = False,.    ss
+000006c0: 6c5f 6365 7274 5f65 6d61 696c 3a20 7374  l_cert_email: st
+000006d0: 7220 3d20 4e6f 6e65 2c0a 293a 0a20 2020  r = None,.):.   
+000006e0: 2063 6f6e 6669 6720 3d20 7b0a 2020 2020   config = {.    
+000006f0: 2020 2020 2270 726f 7669 6465 7222 3a20      "provider": 
+00000700: 636c 6f75 645f 7072 6f76 6964 6572 2c0a  cloud_provider,.
+00000710: 2020 2020 2020 2020 226e 616d 6573 7061          "namespa
+00000720: 6365 223a 206e 616d 6573 7061 6365 2c0a  ce": namespace,.
+00000730: 2020 2020 2020 2020 226e 6562 6172 695f          "nebari_
+00000740: 7665 7273 696f 6e22 3a20 5f5f 7665 7273  version": __vers
+00000750: 696f 6e5f 5f2c 0a20 2020 207d 0a0a 2020  ion__,.    }..  
+00000760: 2020 6966 2070 726f 6a65 6374 5f6e 616d    if project_nam
+00000770: 6520 6973 204e 6f6e 6520 616e 6420 6e6f  e is None and no
+00000780: 7420 6469 7361 626c 655f 7072 6f6d 7074  t disable_prompt
+00000790: 3a0a 2020 2020 2020 2020 7072 6f6a 6563  :.        projec
+000007a0: 745f 6e61 6d65 203d 2069 6e70 7574 2822  t_name = input("
+000007b0: 5072 6f76 6964 6520 7072 6f6a 6563 7420  Provide project 
+000007c0: 6e61 6d65 3a20 2229 0a20 2020 2063 6f6e  name: ").    con
+000007d0: 6669 675b 2270 726f 6a65 6374 5f6e 616d  fig["project_nam
+000007e0: 6522 5d20 3d20 7072 6f6a 6563 745f 6e61  e"] = project_na
+000007f0: 6d65 0a0a 2020 2020 6966 206e 6562 6172  me..    if nebar
+00000800: 695f 646f 6d61 696e 2069 7320 6e6f 7420  i_domain is not 
+00000810: 4e6f 6e65 3a0a 2020 2020 2020 2020 636f  None:.        co
+00000820: 6e66 6967 5b22 646f 6d61 696e 225d 203d  nfig["domain"] =
+00000830: 206e 6562 6172 695f 646f 6d61 696e 0a0a   nebari_domain..
+00000840: 2020 2020 636f 6e66 6967 5b22 6369 5f63      config["ci_c
+00000850: 6422 5d20 3d20 7b22 7479 7065 223a 2063  d"] = {"type": c
+00000860: 695f 7072 6f76 6964 6572 7d0a 2020 2020  i_provider}.    
+00000870: 636f 6e66 6967 5b22 7465 7272 6166 6f72  config["terrafor
+00000880: 6d5f 7374 6174 6522 5d20 3d20 7b22 7479  m_state"] = {"ty
+00000890: 7065 223a 2074 6572 7261 666f 726d 5f73  pe": terraform_s
+000008a0: 7461 7465 7d0a 0a20 2020 2023 2053 6176  tate}..    # Sav
+000008b0: 6520 6465 6661 756c 7420 7061 7373 776f  e default passwo
+000008c0: 7264 2074 6f20 6669 6c65 0a20 2020 2064  rd to file.    d
+000008d0: 6566 6175 6c74 5f70 6173 7377 6f72 645f  efault_password_
+000008e0: 6669 6c65 6e61 6d65 203d 2050 6174 6828  filename = Path(
+000008f0: 7465 6d70 6669 6c65 2e67 6574 7465 6d70  tempfile.gettemp
+00000900: 6469 7228 2929 202f 2022 4e45 4241 5249  dir()) / "NEBARI
+00000910: 5f44 4546 4155 4c54 5f50 4153 5357 4f52  _DEFAULT_PASSWOR
+00000920: 4422 0a20 2020 2063 6f6e 6669 675b 2273  D".    config["s
+00000930: 6563 7572 6974 7922 5d20 3d20 7b0a 2020  ecurity"] = {.  
+00000940: 2020 2020 2020 226b 6579 636c 6f61 6b22        "keycloak"
+00000950: 3a20 7b22 696e 6974 6961 6c5f 726f 6f74  : {"initial_root
+00000960: 5f70 6173 7377 6f72 6422 3a20 7261 6e64  _password": rand
+00000970: 6f6d 5f73 6563 7572 655f 7374 7269 6e67  om_secure_string
+00000980: 286c 656e 6774 683d 3332 297d 0a20 2020  (length=32)}.   
+00000990: 207d 0a20 2020 2077 6974 6820 6465 6661   }.    with defa
+000009a0: 756c 745f 7061 7373 776f 7264 5f66 696c  ult_password_fil
+000009b0: 656e 616d 652e 6f70 656e 2822 7722 2920  ename.open("w") 
+000009c0: 6173 2066 3a0a 2020 2020 2020 2020 662e  as f:.        f.
+000009d0: 7772 6974 6528 636f 6e66 6967 5b22 7365  write(config["se
+000009e0: 6375 7269 7479 225d 5b22 6b65 7963 6c6f  curity"]["keyclo
+000009f0: 616b 225d 5b22 696e 6974 6961 6c5f 726f  ak"]["initial_ro
+00000a00: 6f74 5f70 6173 7377 6f72 6422 5d29 0a20  ot_password"]). 
+00000a10: 2020 2064 6566 6175 6c74 5f70 6173 7377     default_passw
+00000a20: 6f72 645f 6669 6c65 6e61 6d65 2e63 686d  ord_filename.chm
+00000a30: 6f64 2830 6f37 3030 290a 0a20 2020 2063  od(0o700)..    c
+00000a40: 6f6e 6669 675b 2274 6865 6d65 225d 203d  onfig["theme"] =
+00000a50: 207b 226a 7570 7974 6572 6875 6222 3a20   {"jupyterhub": 
+00000a60: 7b22 6875 625f 7469 746c 6522 3a20 6622  {"hub_title": f"
+00000a70: 4e65 6261 7269 202d 207b 2070 726f 6a65  Nebari - { proje
+00000a80: 6374 5f6e 616d 6520 7d22 7d7d 0a20 2020  ct_name }"}}.   
+00000a90: 2063 6f6e 6669 675b 2274 6865 6d65 225d   config["theme"]
+00000aa0: 5b22 6a75 7079 7465 7268 7562 225d 5b0a  ["jupyterhub"][.
+00000ab0: 2020 2020 2020 2020 2277 656c 636f 6d65          "welcome
+00000ac0: 220a 2020 2020 5d20 3d20 2222 2257 656c  ".    ] = """Wel
+00000ad0: 636f 6d65 2120 4c65 6172 6e20 6162 6f75  come! Learn abou
+00000ae0: 7420 4e65 6261 7269 2773 2066 6561 7475  t Nebari's featu
+00000af0: 7265 7320 616e 6420 636f 6e66 6967 7572  res and configur
+00000b00: 6174 696f 6e73 2069 6e20 3c61 2068 7265  ations in <a hre
+00000b10: 663d 2268 7474 7073 3a2f 2f77 7777 2e6e  f="https://www.n
+00000b20: 6562 6172 692e 6465 762f 646f 6373 2f77  ebari.dev/docs/w
+00000b30: 656c 636f 6d65 223e 7468 6520 646f 6375  elcome">the docu
+00000b40: 6d65 6e74 6174 696f 6e3c 2f61 3e2e 2049  mentation</a>. I
+00000b50: 6620 796f 7520 6861 7665 2061 6e79 2071  f you have any q
+00000b60: 7565 7374 696f 6e73 206f 7220 6665 6564  uestions or feed
+00000b70: 6261 636b 2c20 7265 6163 6820 7468 6520  back, reach the 
+00000b80: 7465 616d 206f 6e20 3c61 2068 7265 663d  team on <a href=
+00000b90: 2268 7474 7073 3a2f 2f77 7777 2e6e 6562  "https://www.neb
+00000ba0: 6172 692e 6465 762f 646f 6373 2f63 6f6d  ari.dev/docs/com
+00000bb0: 6d75 6e69 7479 2367 6574 7469 6e67 2d73  munity#getting-s
+00000bc0: 7570 706f 7274 223e 4e65 6261 7269 2773  upport">Nebari's
+00000bd0: 2073 7570 706f 7274 2066 6f72 756d 733c   support forums<
+00000be0: 2f61 3e2e 2222 220a 0a20 2020 2063 6f6e  /a>."""..    con
+00000bf0: 6669 675b 2273 6563 7572 6974 7922 5d5b  fig["security"][
+00000c00: 2261 7574 6865 6e74 6963 6174 696f 6e22  "authentication"
+00000c10: 5d20 3d20 7b22 7479 7065 223a 2061 7574  ] = {"type": aut
+00000c20: 685f 7072 6f76 6964 6572 7d0a 0a20 2020  h_provider}..   
+00000c30: 2069 6620 6175 7468 5f70 726f 7669 6465   if auth_provide
+00000c40: 7220 3d3d 2041 7574 6865 6e74 6963 6174  r == Authenticat
+00000c50: 696f 6e45 6e75 6d2e 6769 7468 7562 3a0a  ionEnum.github:.
+00000c60: 2020 2020 2020 2020 636f 6e66 6967 5b22          config["
+00000c70: 7365 6375 7269 7479 225d 5b22 6175 7468  security"]["auth
+00000c80: 656e 7469 6361 7469 6f6e 225d 5b22 636f  entication"]["co
+00000c90: 6e66 6967 225d 203d 207b 0a20 2020 2020  nfig"] = {.     
+00000ca0: 2020 2020 2020 2022 636c 6965 6e74 5f69         "client_i
+00000cb0: 6422 3a20 6f73 2e65 6e76 6972 6f6e 2e67  d": os.environ.g
+00000cc0: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+00000cd0: 2020 2020 2247 4954 4855 425f 434c 4945      "GITHUB_CLIE
+00000ce0: 4e54 5f49 4422 2c0a 2020 2020 2020 2020  NT_ID",.        
+00000cf0: 2020 2020 2020 2020 223c 656e 7465 7220          "<enter 
+00000d00: 636c 6965 6e74 2069 6420 6f72 2072 656d  client id or rem
+00000d10: 6f76 6520 746f 2075 7365 2047 4954 4855  ove to use GITHU
+00000d20: 425f 434c 4945 4e54 5f49 4420 656e 7669  B_CLIENT_ID envi
+00000d30: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00000d40: 2028 7072 6566 6572 7265 6429 3e22 2c0a   (preferred)>",.
+00000d50: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+00000d60: 2020 2020 2020 2020 2020 2022 636c 6965             "clie
+00000d70: 6e74 5f73 6563 7265 7422 3a20 6f73 2e65  nt_secret": os.e
+00000d80: 6e76 6972 6f6e 2e67 6574 280a 2020 2020  nviron.get(.    
+00000d90: 2020 2020 2020 2020 2020 2020 2247 4954              "GIT
+00000da0: 4855 425f 434c 4945 4e54 5f53 4543 5245  HUB_CLIENT_SECRE
+00000db0: 5422 2c0a 2020 2020 2020 2020 2020 2020  T",.            
+00000dc0: 2020 2020 223c 656e 7465 7220 636c 6965      "<enter clie
+00000dd0: 6e74 2073 6563 7265 7420 6f72 2072 656d  nt secret or rem
+00000de0: 6f76 6520 746f 2075 7365 2047 4954 4855  ove to use GITHU
+00000df0: 425f 434c 4945 4e54 5f53 4543 5245 5420  B_CLIENT_SECRET 
+00000e00: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+00000e10: 6162 6c65 2028 7072 6566 6572 7265 6429  able (preferred)
+00000e20: 3e22 2c0a 2020 2020 2020 2020 2020 2020  >",.            
+00000e30: 292c 0a20 2020 2020 2020 207d 0a20 2020  ),.        }.   
+00000e40: 2065 6c69 6620 6175 7468 5f70 726f 7669   elif auth_provi
+00000e50: 6465 7220 3d3d 2041 7574 6865 6e74 6963  der == Authentic
+00000e60: 6174 696f 6e45 6e75 6d2e 6175 7468 303a  ationEnum.auth0:
+00000e70: 0a20 2020 2020 2020 2069 6620 6175 7468  .        if auth
+00000e80: 5f61 7574 6f5f 7072 6f76 6973 696f 6e3a  _auto_provision:
+00000e90: 0a20 2020 2020 2020 2020 2020 2061 7574  .            aut
+00000ea0: 6830 5f63 6f6e 6669 6720 3d20 6372 6561  h0_config = crea
+00000eb0: 7465 5f63 6c69 656e 7428 636f 6e66 6967  te_client(config
+00000ec0: 2e64 6f6d 6169 6e2c 2063 6f6e 6669 672e  .domain, config.
+00000ed0: 7072 6f6a 6563 745f 6e61 6d65 290a 2020  project_name).  
+00000ee0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00000ef0: 5b22 7365 6375 7269 7479 225d 5b22 6175  ["security"]["au
+00000f00: 7468 656e 7469 6361 7469 6f6e 225d 5b22  thentication"]["
+00000f10: 636f 6e66 6967 225d 203d 2061 7574 6830  config"] = auth0
+00000f20: 5f63 6f6e 6669 670a 2020 2020 2020 2020  _config.        
+00000f30: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00000f40: 2020 636f 6e66 6967 5b22 7365 6375 7269    config["securi
+00000f50: 7479 225d 5b22 6175 7468 656e 7469 6361  ty"]["authentica
+00000f60: 7469 6f6e 225d 5b22 636f 6e66 6967 225d  tion"]["config"]
+00000f70: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00000f80: 2020 2020 2022 636c 6965 6e74 5f69 6422       "client_id"
+00000f90: 3a20 6f73 2e65 6e76 6972 6f6e 2e67 6574  : os.environ.get
+00000fa0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00000fb0: 2020 2020 2020 2241 5554 4830 5f43 4c49        "AUTH0_CLI
+00000fc0: 454e 545f 4944 222c 0a20 2020 2020 2020  ENT_ID",.       
+00000fd0: 2020 2020 2020 2020 2020 2020 2022 3c65               "<e
+00000fe0: 6e74 6572 2063 6c69 656e 7420 6964 206f  nter client id o
+00000ff0: 7220 7265 6d6f 7665 2074 6f20 7573 6520  r remove to use 
+00001000: 4155 5448 305f 434c 4945 4e54 5f49 4420  AUTH0_CLIENT_ID 
+00001010: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+00001020: 6162 6c65 2028 7072 6566 6572 7265 6429  able (preferred)
+00001030: 3e22 2c0a 2020 2020 2020 2020 2020 2020  >",.            
+00001040: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00001050: 2020 2020 2020 2022 636c 6965 6e74 5f73         "client_s
+00001060: 6563 7265 7422 3a20 6f73 2e65 6e76 6972  ecret": os.envir
+00001070: 6f6e 2e67 6574 280a 2020 2020 2020 2020  on.get(.        
+00001080: 2020 2020 2020 2020 2020 2020 2241 5554              "AUT
+00001090: 4830 5f43 4c49 454e 545f 5345 4352 4554  H0_CLIENT_SECRET
+000010a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000010b0: 2020 2020 2020 2022 3c65 6e74 6572 2063         "<enter c
+000010c0: 6c69 656e 7420 7365 6372 6574 206f 7220  lient secret or 
+000010d0: 7265 6d6f 7665 2074 6f20 7573 6520 4155  remove to use AU
+000010e0: 5448 305f 434c 4945 4e54 5f53 4543 5245  TH0_CLIENT_SECRE
+000010f0: 5420 656e 7669 726f 6e6d 656e 7420 7661  T environment va
+00001100: 7269 6162 6c65 2028 7072 6566 6572 7265  riable (preferre
+00001110: 6429 3e22 2c0a 2020 2020 2020 2020 2020  d)>",.          
+00001120: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00001130: 2020 2020 2020 2020 2022 6175 7468 305f           "auth0_
+00001140: 7375 6264 6f6d 6169 6e22 3a20 6f73 2e65  subdomain": os.e
+00001150: 6e76 6972 6f6e 2e67 6574 280a 2020 2020  nviron.get(.    
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 2241 5554 4830 5f44 4f4d 4149 4e22 2c0a  "AUTH0_DOMAIN",.
+00001180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001190: 2020 2020 223c 656e 7465 7220 7375 6264      "<enter subd
+000011a0: 6f6d 6169 6e20 2877 6974 686f 7574 202e  omain (without .
+000011b0: 6175 7468 302e 636f 6d29 206f 7220 7265  auth0.com) or re
+000011c0: 6d6f 7665 2074 6f20 7573 6520 4155 5448  move to use AUTH
+000011d0: 305f 444f 4d41 494e 2065 6e76 6972 6f6e  0_DOMAIN environ
+000011e0: 6d65 6e74 2076 6172 6961 626c 653e 222c  ment variable>",
+000011f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001200: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00001210: 7d0a 0a20 2020 2069 6620 636c 6f75 645f  }..    if cloud_
+00001220: 7072 6f76 6964 6572 203d 3d20 5072 6f76  provider == Prov
+00001230: 6964 6572 456e 756d 2e64 6f3a 0a20 2020  iderEnum.do:.   
+00001240: 2020 2020 2064 6f5f 7265 6769 6f6e 203d       do_region =
+00001250: 2072 6567 696f 6e20 6f72 2063 6f6e 7374   region or const
+00001260: 616e 7473 2e44 4f5f 4445 4641 554c 545f  ants.DO_DEFAULT_
+00001270: 5245 4749 4f4e 0a20 2020 2020 2020 2064  REGION.        d
+00001280: 6f5f 6b75 6265 726e 6574 6573 5f76 6572  o_kubernetes_ver
+00001290: 7369 6f6e 7320 3d20 6b75 6265 726e 6574  sions = kubernet
+000012a0: 6573 5f76 6572 7369 6f6e 206f 7220 6765  es_version or ge
+000012b0: 745f 6c61 7465 7374 5f6b 7562 6572 6e65  t_latest_kuberne
+000012c0: 7465 735f 7665 7273 696f 6e28 0a20 2020  tes_version(.   
+000012d0: 2020 2020 2020 2020 2064 6967 6974 616c           digital
+000012e0: 5f6f 6365 616e 2e6b 7562 6572 6e65 7465  _ocean.kubernete
+000012f0: 735f 7665 7273 696f 6e73 2864 6f5f 7265  s_versions(do_re
+00001300: 6769 6f6e 290a 2020 2020 2020 2020 290a  gion).        ).
+00001310: 2020 2020 2020 2020 636f 6e66 6967 5b22          config["
+00001320: 6469 6769 7461 6c5f 6f63 6561 6e22 5d20  digital_ocean"] 
+00001330: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00001340: 226b 7562 6572 6e65 7465 735f 7665 7273  "kubernetes_vers
+00001350: 696f 6e22 3a20 646f 5f6b 7562 6572 6e65  ion": do_kuberne
+00001360: 7465 735f 7665 7273 696f 6e73 2c0a 2020  tes_versions,.  
+00001370: 2020 2020 2020 2020 2020 2272 6567 696f            "regio
+00001380: 6e22 3a20 646f 5f72 6567 696f 6e2c 0a20  n": do_region,. 
+00001390: 2020 2020 2020 2020 2020 2022 6e6f 6465             "node
+000013a0: 5f67 726f 7570 7322 3a20 5f6e 6f64 655f  _groups": _node_
+000013b0: 6772 6f75 7073 5f74 6f5f 6469 6374 2844  groups_to_dict(D
+000013c0: 4546 4155 4c54 5f44 4f5f 4e4f 4445 5f47  EFAULT_DO_NODE_G
+000013d0: 524f 5550 5329 2c0a 2020 2020 2020 2020  ROUPS),.        
+000013e0: 7d0a 0a20 2020 2020 2020 2063 6f6e 6669  }..        confi
+000013f0: 675b 2274 6865 6d65 225d 5b22 6a75 7079  g["theme"]["jupy
+00001400: 7465 7268 7562 225d 5b0a 2020 2020 2020  terhub"][.      
+00001410: 2020 2020 2020 2268 7562 5f73 7562 7469        "hub_subti
+00001420: 746c 6522 0a20 2020 2020 2020 205d 203d  tle".        ] =
+00001430: 2066 227b 5745 4c43 4f4d 455f 4845 4144   f"{WELCOME_HEAD
+00001440: 4552 5f54 4558 547d 206f 6e20 4469 6769  ER_TEXT} on Digi
+00001450: 7461 6c20 4f63 6561 6e22 0a0a 2020 2020  tal Ocean"..    
+00001460: 656c 6966 2063 6c6f 7564 5f70 726f 7669  elif cloud_provi
+00001470: 6465 7220 3d3d 2050 726f 7669 6465 7245  der == ProviderE
+00001480: 6e75 6d2e 6763 703a 0a20 2020 2020 2020  num.gcp:.       
+00001490: 2067 6370 5f72 6567 696f 6e20 3d20 7265   gcp_region = re
+000014a0: 6769 6f6e 206f 7220 636f 6e73 7461 6e74  gion or constant
+000014b0: 732e 4743 505f 4445 4641 554c 545f 5245  s.GCP_DEFAULT_RE
+000014c0: 4749 4f4e 0a20 2020 2020 2020 2067 6370  GION.        gcp
+000014d0: 5f6b 7562 6572 6e65 7465 735f 7665 7273  _kubernetes_vers
+000014e0: 696f 6e20 3d20 6b75 6265 726e 6574 6573  ion = kubernetes
+000014f0: 5f76 6572 7369 6f6e 206f 7220 6765 745f  _version or get_
+00001500: 6c61 7465 7374 5f6b 7562 6572 6e65 7465  latest_kubernete
+00001510: 735f 7665 7273 696f 6e28 0a20 2020 2020  s_version(.     
+00001520: 2020 2020 2020 2067 6f6f 676c 655f 636c         google_cl
+00001530: 6f75 642e 6b75 6265 726e 6574 6573 5f76  oud.kubernetes_v
+00001540: 6572 7369 6f6e 7328 6763 705f 7265 6769  ersions(gcp_regi
+00001550: 6f6e 290a 2020 2020 2020 2020 290a 2020  on).        ).  
+00001560: 2020 2020 2020 636f 6e66 6967 5b22 676f        config["go
+00001570: 6f67 6c65 5f63 6c6f 7564 5f70 6c61 7466  ogle_cloud_platf
+00001580: 6f72 6d22 5d20 3d20 7b0a 2020 2020 2020  orm"] = {.      
+00001590: 2020 2020 2020 226b 7562 6572 6e65 7465        "kubernete
+000015a0: 735f 7665 7273 696f 6e22 3a20 6763 705f  s_version": gcp_
+000015b0: 6b75 6265 726e 6574 6573 5f76 6572 7369  kubernetes_versi
+000015c0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+000015d0: 2272 6567 696f 6e22 3a20 6763 705f 7265  "region": gcp_re
+000015e0: 6769 6f6e 2c0a 2020 2020 2020 2020 2020  gion,.          
+000015f0: 2020 226e 6f64 655f 6772 6f75 7073 223a    "node_groups":
+00001600: 205f 6e6f 6465 5f67 726f 7570 735f 746f   _node_groups_to
+00001610: 5f64 6963 7428 4445 4641 554c 545f 4743  _dict(DEFAULT_GC
+00001620: 505f 4e4f 4445 5f47 524f 5550 5329 2c0a  P_NODE_GROUPS),.
+00001630: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00001640: 2020 2063 6f6e 6669 675b 2274 6865 6d65     config["theme
+00001650: 225d 5b22 6a75 7079 7465 7268 7562 225d  "]["jupyterhub"]
+00001660: 5b0a 2020 2020 2020 2020 2020 2020 2268  [.            "h
+00001670: 7562 5f73 7562 7469 746c 6522 0a20 2020  ub_subtitle".   
+00001680: 2020 2020 205d 203d 2066 227b 5745 4c43       ] = f"{WELC
+00001690: 4f4d 455f 4845 4144 4552 5f54 4558 547d  OME_HEADER_TEXT}
+000016a0: 206f 6e20 476f 6f67 6c65 2043 6c6f 7564   on Google Cloud
+000016b0: 2050 6c61 7466 6f72 6d22 0a20 2020 2020   Platform".     
+000016c0: 2020 2069 6620 2250 524f 4a45 4354 5f49     if "PROJECT_I
+000016d0: 4422 2069 6e20 6f73 2e65 6e76 6972 6f6e  D" in os.environ
+000016e0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+000016f0: 6e66 6967 5b22 676f 6f67 6c65 5f63 6c6f  nfig["google_clo
+00001700: 7564 5f70 6c61 7466 6f72 6d22 5d5b 2270  ud_platform"]["p
+00001710: 726f 6a65 6374 225d 203d 206f 732e 656e  roject"] = os.en
+00001720: 7669 726f 6e5b 2250 524f 4a45 4354 5f49  viron["PROJECT_I
+00001730: 4422 5d0a 2020 2020 2020 2020 656c 6966  D"].        elif
+00001740: 206e 6f74 2064 6973 6162 6c65 5f70 726f   not disable_pro
+00001750: 6d70 743a 0a20 2020 2020 2020 2020 2020  mpt:.           
+00001760: 2063 6f6e 6669 675b 2267 6f6f 676c 655f   config["google_
+00001770: 636c 6f75 645f 706c 6174 666f 726d 225d  cloud_platform"]
+00001780: 5b22 7072 6f6a 6563 7422 5d20 3d20 696e  ["project"] = in
+00001790: 7075 7428 0a20 2020 2020 2020 2020 2020  put(.           
+000017a0: 2020 2020 2022 456e 7465 7220 476f 6f67       "Enter Goog
+000017b0: 6c65 2043 6c6f 7564 2050 6c61 7466 6f72  le Cloud Platfor
+000017c0: 6d20 5072 6f6a 6563 7420 4944 3a20 220a  m Project ID: ".
+000017d0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+000017e0: 2020 2065 6c69 6620 636c 6f75 645f 7072     elif cloud_pr
+000017f0: 6f76 6964 6572 203d 3d20 5072 6f76 6964  ovider == Provid
+00001800: 6572 456e 756d 2e61 7a75 7265 3a0a 2020  erEnum.azure:.  
+00001810: 2020 2020 2020 617a 7572 655f 7265 6769        azure_regi
+00001820: 6f6e 203d 2072 6567 696f 6e20 6f72 2063  on = region or c
+00001830: 6f6e 7374 616e 7473 2e41 5a55 5245 5f44  onstants.AZURE_D
+00001840: 4546 4155 4c54 5f52 4547 494f 4e0a 2020  EFAULT_REGION.  
+00001850: 2020 2020 2020 617a 7572 655f 6b75 6265        azure_kube
+00001860: 726e 6574 6573 5f76 6572 7369 6f6e 203d  rnetes_version =
+00001870: 206b 7562 6572 6e65 7465 735f 7665 7273   kubernetes_vers
+00001880: 696f 6e20 6f72 2067 6574 5f6c 6174 6573  ion or get_lates
+00001890: 745f 6b75 6265 726e 6574 6573 5f76 6572  t_kubernetes_ver
+000018a0: 7369 6f6e 280a 2020 2020 2020 2020 2020  sion(.          
+000018b0: 2020 617a 7572 655f 636c 6f75 642e 6b75    azure_cloud.ku
+000018c0: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
+000018d0: 7328 617a 7572 655f 7265 6769 6f6e 290a  s(azure_region).
+000018e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000018f0: 2020 636f 6e66 6967 5b22 617a 7572 6522    config["azure"
+00001900: 5d20 3d20 7b0a 2020 2020 2020 2020 2020  ] = {.          
+00001910: 2020 226b 7562 6572 6e65 7465 735f 7665    "kubernetes_ve
+00001920: 7273 696f 6e22 3a20 617a 7572 655f 6b75  rsion": azure_ku
+00001930: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
+00001940: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
+00001950: 6567 696f 6e22 3a20 617a 7572 655f 7265  egion": azure_re
+00001960: 6769 6f6e 2c0a 2020 2020 2020 2020 2020  gion,.          
+00001970: 2020 2273 746f 7261 6765 5f61 6363 6f75    "storage_accou
+00001980: 6e74 5f70 6f73 7466 6978 223a 2072 616e  nt_postfix": ran
+00001990: 646f 6d5f 7365 6375 7265 5f73 7472 696e  dom_secure_strin
+000019a0: 6728 6c65 6e67 7468 3d34 292c 0a20 2020  g(length=4),.   
+000019b0: 2020 2020 2020 2020 2022 6e6f 6465 5f67           "node_g
+000019c0: 726f 7570 7322 3a20 5f6e 6f64 655f 6772  roups": _node_gr
+000019d0: 6f75 7073 5f74 6f5f 6469 6374 2844 4546  oups_to_dict(DEF
+000019e0: 4155 4c54 5f41 5a55 5245 5f4e 4f44 455f  AULT_AZURE_NODE_
+000019f0: 4752 4f55 5053 292c 0a20 2020 2020 2020  GROUPS),.       
+00001a00: 207d 0a0a 2020 2020 2020 2020 636f 6e66   }..        conf
+00001a10: 6967 5b22 7468 656d 6522 5d5b 226a 7570  ig["theme"]["jup
+00001a20: 7974 6572 6875 6222 5d5b 0a20 2020 2020  yterhub"][.     
+00001a30: 2020 2020 2020 2022 6875 625f 7375 6274         "hub_subt
+00001a40: 6974 6c65 220a 2020 2020 2020 2020 5d20  itle".        ] 
+00001a50: 3d20 6622 7b57 454c 434f 4d45 5f48 4541  = f"{WELCOME_HEA
+00001a60: 4445 525f 5445 5854 7d20 6f6e 2041 7a75  DER_TEXT} on Azu
+00001a70: 7265 220a 0a20 2020 2065 6c69 6620 636c  re"..    elif cl
+00001a80: 6f75 645f 7072 6f76 6964 6572 203d 3d20  oud_provider == 
+00001a90: 5072 6f76 6964 6572 456e 756d 2e61 7773  ProviderEnum.aws
+00001aa0: 3a0a 2020 2020 2020 2020 6177 735f 7265  :.        aws_re
+00001ab0: 6769 6f6e 203d 2028 0a20 2020 2020 2020  gion = (.       
+00001ac0: 2020 2020 2072 6567 696f 6e0a 2020 2020       region.    
+00001ad0: 2020 2020 2020 2020 6f72 206f 732e 656e          or os.en
+00001ae0: 7669 726f 6e2e 6765 7428 2241 5753 5f44  viron.get("AWS_D
+00001af0: 4546 4155 4c54 5f52 4547 494f 4e22 290a  EFAULT_REGION").
+00001b00: 2020 2020 2020 2020 2020 2020 6f72 2063              or c
+00001b10: 6f6e 7374 616e 7473 2e41 5753 5f44 4546  onstants.AWS_DEF
+00001b20: 4155 4c54 5f52 4547 494f 4e0a 2020 2020  AULT_REGION.    
+00001b30: 2020 2020 290a 2020 2020 2020 2020 6177      ).        aw
+00001b40: 735f 6b75 6265 726e 6574 6573 5f76 6572  s_kubernetes_ver
+00001b50: 7369 6f6e 203d 206b 7562 6572 6e65 7465  sion = kubernete
+00001b60: 735f 7665 7273 696f 6e20 6f72 2067 6574  s_version or get
+00001b70: 5f6c 6174 6573 745f 6b75 6265 726e 6574  _latest_kubernet
+00001b80: 6573 5f76 6572 7369 6f6e 280a 2020 2020  es_version(.    
+00001b90: 2020 2020 2020 2020 616d 617a 6f6e 5f77          amazon_w
+00001ba0: 6562 5f73 6572 7669 6365 732e 6b75 6265  eb_services.kube
+00001bb0: 726e 6574 6573 5f76 6572 7369 6f6e 7328  rnetes_versions(
+00001bc0: 6177 735f 7265 6769 6f6e 290a 2020 2020  aws_region).    
+00001bd0: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
+00001be0: 6e66 6967 5b22 616d 617a 6f6e 5f77 6562  nfig["amazon_web
+00001bf0: 5f73 6572 7669 6365 7322 5d20 3d20 7b0a  _services"] = {.
+00001c00: 2020 2020 2020 2020 2020 2020 226b 7562              "kub
+00001c10: 6572 6e65 7465 735f 7665 7273 696f 6e22  ernetes_version"
+00001c20: 3a20 6177 735f 6b75 6265 726e 6574 6573  : aws_kubernetes
+00001c30: 5f76 6572 7369 6f6e 2c0a 2020 2020 2020  _version,.      
+00001c40: 2020 2020 2020 2272 6567 696f 6e22 3a20        "region": 
+00001c50: 6177 735f 7265 6769 6f6e 2c0a 2020 2020  aws_region,.    
+00001c60: 2020 2020 2020 2020 226e 6f64 655f 6772          "node_gr
+00001c70: 6f75 7073 223a 205f 6e6f 6465 5f67 726f  oups": _node_gro
+00001c80: 7570 735f 746f 5f64 6963 7428 4445 4641  ups_to_dict(DEFA
+00001c90: 554c 545f 4157 535f 4e4f 4445 5f47 524f  ULT_AWS_NODE_GRO
+00001ca0: 5550 5329 2c0a 2020 2020 2020 2020 7d0a  UPS),.        }.
+00001cb0: 2020 2020 2020 2020 636f 6e66 6967 5b22          config["
+00001cc0: 7468 656d 6522 5d5b 226a 7570 7974 6572  theme"]["jupyter
+00001cd0: 6875 6222 5d5b 0a20 2020 2020 2020 2020  hub"][.         
+00001ce0: 2020 2022 6875 625f 7375 6274 6974 6c65     "hub_subtitle
+00001cf0: 220a 2020 2020 2020 2020 5d20 3d20 6622  ".        ] = f"
+00001d00: 7b57 454c 434f 4d45 5f48 4541 4445 525f  {WELCOME_HEADER_
+00001d10: 5445 5854 7d20 6f6e 2041 6d61 7a6f 6e20  TEXT} on Amazon 
+00001d20: 5765 6220 5365 7276 6963 6573 220a 0a20  Web Services".. 
+00001d30: 2020 2065 6c69 6620 636c 6f75 645f 7072     elif cloud_pr
+00001d40: 6f76 6964 6572 203d 3d20 5072 6f76 6964  ovider == Provid
+00001d50: 6572 456e 756d 2e65 7869 7374 696e 673a  erEnum.existing:
+00001d60: 0a20 2020 2020 2020 2063 6f6e 6669 675b  .        config[
+00001d70: 2274 6865 6d65 225d 5b22 6a75 7079 7465  "theme"]["jupyte
+00001d80: 7268 7562 225d 5b22 6875 625f 7375 6274  rhub"]["hub_subt
+00001d90: 6974 6c65 225d 203d 2057 454c 434f 4d45  itle"] = WELCOME
+00001da0: 5f48 4541 4445 525f 5445 5854 0a0a 2020  _HEADER_TEXT..  
+00001db0: 2020 656c 6966 2063 6c6f 7564 5f70 726f    elif cloud_pro
+00001dc0: 7669 6465 7220 3d3d 2050 726f 7669 6465  vider == Provide
+00001dd0: 7245 6e75 6d2e 6c6f 6361 6c3a 0a20 2020  rEnum.local:.   
+00001de0: 2020 2020 2063 6f6e 6669 675b 2274 6865       config["the
+00001df0: 6d65 225d 5b22 6a75 7079 7465 7268 7562  me"]["jupyterhub
+00001e00: 225d 5b22 6875 625f 7375 6274 6974 6c65  "]["hub_subtitle
+00001e10: 225d 203d 2057 454c 434f 4d45 5f48 4541  "] = WELCOME_HEA
+00001e20: 4445 525f 5445 5854 0a0a 2020 2020 6966  DER_TEXT..    if
+00001e30: 2073 736c 5f63 6572 745f 656d 6169 6c3a   ssl_cert_email:
+00001e40: 0a20 2020 2020 2020 2063 6f6e 6669 675b  .        config[
+00001e50: 2263 6572 7469 6669 6361 7465 225d 203d  "certificate"] =
+00001e60: 207b 2274 7970 6522 3a20 4365 7274 6966   {"type": Certif
+00001e70: 6963 6174 6545 6e75 6d2e 6c65 7473 656e  icateEnum.letsen
+00001e80: 6372 7970 742e 7661 6c75 657d 0a20 2020  crypt.value}.   
+00001e90: 2020 2020 2063 6f6e 6669 675b 2263 6572       config["cer
+00001ea0: 7469 6669 6361 7465 225d 5b22 6163 6d65  tificate"]["acme
+00001eb0: 5f65 6d61 696c 225d 203d 2073 736c 5f63  _email"] = ssl_c
+00001ec0: 6572 745f 656d 6169 6c0a 0a20 2020 2023  ert_email..    #
+00001ed0: 2076 616c 6964 6174 6520 636f 6e66 6967   validate config
+00001ee0: 7572 6174 696f 6e20 616e 6420 636f 6e76  uration and conv
+00001ef0: 6572 7420 746f 206d 6f64 656c 0a20 2020  ert to model.   
+00001f00: 2066 726f 6d20 6e65 6261 7269 2e70 6c75   from nebari.plu
+00001f10: 6769 6e73 2069 6d70 6f72 7420 6e65 6261  gins import neba
+00001f20: 7269 5f70 6c75 6769 6e5f 6d61 6e61 6765  ri_plugin_manage
+00001f30: 720a 0a20 2020 2074 7279 3a0a 2020 2020  r..    try:.    
+00001f40: 2020 2020 636f 6e66 6967 5f6d 6f64 656c      config_model
+00001f50: 203d 206e 6562 6172 695f 706c 7567 696e   = nebari_plugin
+00001f60: 5f6d 616e 6167 6572 2e63 6f6e 6669 675f  _manager.config_
+00001f70: 7363 6865 6d61 2e70 6172 7365 5f6f 626a  schema.parse_obj
+00001f80: 2863 6f6e 6669 6729 0a20 2020 2065 7863  (config).    exc
+00001f90: 6570 7420 7079 6461 6e74 6963 2e56 616c  ept pydantic.Val
+00001fa0: 6964 6174 696f 6e45 7272 6f72 2061 7320  idationError as 
+00001fb0: 653a 0a20 2020 2020 2020 2070 7269 6e74  e:.        print
+00001fc0: 2873 7472 2865 2929 0a0a 2020 2020 6966  (str(e))..    if
+00001fd0: 2072 6570 6f73 6974 6f72 795f 6175 746f   repository_auto
+00001fe0: 5f70 726f 7669 7369 6f6e 3a0a 2020 2020  _provision:.    
+00001ff0: 2020 2020 6d61 7463 6820 3d20 7265 2e73      match = re.s
+00002000: 6561 7263 6828 6769 7468 7562 5f75 726c  earch(github_url
+00002010: 5f72 6567 6578 2c20 7265 706f 7369 746f  _regex, reposito
+00002020: 7279 290a 2020 2020 2020 2020 6966 206d  ry).        if m
+00002030: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
+00002040: 2020 6769 745f 7265 706f 7369 746f 7279    git_repository
+00002050: 203d 2067 6974 6875 625f 6175 746f 5f70   = github_auto_p
+00002060: 726f 7669 7369 6f6e 280a 2020 2020 2020  rovision(.      
+00002070: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00002080: 5f6d 6f64 656c 2c20 6d61 7463 682e 6772  _model, match.gr
+00002090: 6f75 7028 3229 2c20 6d61 7463 682e 6772  oup(2), match.gr
+000020a0: 6f75 7028 3329 0a20 2020 2020 2020 2020  oup(3).         
+000020b0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000020c0: 2067 6974 5f72 6570 6f73 6974 6f72 795f   git_repository_
+000020d0: 696e 6974 6961 6c69 7a65 2867 6974 5f72  initialize(git_r
+000020e0: 6570 6f73 6974 6f72 7929 0a20 2020 2020  epository).     
+000020f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00002100: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00002110: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00002120: 2020 2020 2020 2066 2252 6570 6f73 6974         f"Reposit
+00002130: 6f72 7920 746f 2062 6520 6175 746f 2d70  ory to be auto-p
+00002140: 726f 7669 7369 6f6e 6564 2069 7320 6e6f  rovisioned is no
+00002150: 7420 7468 6520 6675 6c6c 2055 524c 206f  t the full URL o
+00002160: 6620 6120 4769 7448 7562 2072 6570 6f3a  f a GitHub repo:
+00002170: 207b 7265 706f 7369 746f 7279 7d22 0a20   {repository}". 
+00002180: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00002190: 2020 7265 7475 726e 2063 6f6e 6669 670a    return config.
+000021a0: 0a0a 6465 6620 6769 7468 7562 5f61 7574  ..def github_aut
+000021b0: 6f5f 7072 6f76 6973 696f 6e28 636f 6e66  o_provision(conf
+000021c0: 6967 3a20 7079 6461 6e74 6963 2e42 6173  ig: pydantic.Bas
+000021d0: 654d 6f64 656c 2c20 6f77 6e65 723a 2073  eModel, owner: s
+000021e0: 7472 2c20 7265 706f 3a20 7374 7229 3a0a  tr, repo: str):.
+000021f0: 2020 2020 616c 7265 6164 795f 6578 6973      already_exis
+00002200: 7473 203d 2054 7275 650a 2020 2020 7472  ts = True.    tr
+00002210: 793a 0a20 2020 2020 2020 2067 6974 6875  y:.        githu
+00002220: 622e 6765 745f 7265 706f 7369 746f 7279  b.get_repository
+00002230: 286f 776e 6572 2c20 7265 706f 290a 2020  (owner, repo).  
+00002240: 2020 6578 6365 7074 2072 6571 7565 7374    except request
+00002250: 732e 6578 6365 7074 696f 6e73 2e48 5454  s.exceptions.HTT
+00002260: 5045 7272 6f72 3a0a 2020 2020 2020 2020  PError:.        
+00002270: 2320 7265 706f 206e 6f74 2066 6f75 6e64  # repo not found
+00002280: 0a20 2020 2020 2020 2061 6c72 6561 6479  .        already
+00002290: 5f65 7869 7374 7320 3d20 4661 6c73 650a  _exists = False.
+000022a0: 0a20 2020 2069 6620 6e6f 7420 616c 7265  .    if not alre
+000022b0: 6164 795f 6578 6973 7473 3a0a 2020 2020  ady_exists:.    
+000022c0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+000022d0: 2020 2020 2067 6974 6875 622e 6372 6561       github.crea
+000022e0: 7465 5f72 6570 6f73 6974 6f72 7928 0a20  te_repository(. 
+000022f0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00002300: 776e 6572 2c0a 2020 2020 2020 2020 2020  wner,.          
+00002310: 2020 2020 2020 7265 706f 2c0a 2020 2020        repo,.    
+00002320: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00002330: 7269 7074 696f 6e3d 6622 4e65 6261 7269  ription=f"Nebari
+00002340: 207b 636f 6e66 6967 2e70 726f 6a65 6374   {config.project
+00002350: 5f6e 616d 657d 2d7b 636f 6e66 6967 2e70  _name}-{config.p
+00002360: 726f 7669 6465 727d 222c 0a20 2020 2020  rovider}",.     
+00002370: 2020 2020 2020 2020 2020 2068 6f6d 6570             homep
+00002380: 6167 653d 6622 6874 7470 733a 2f2f 7b63  age=f"https://{c
+00002390: 6f6e 6669 672e 646f 6d61 696e 7d22 2c0a  onfig.domain}",.
+000023a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000023b0: 2020 2020 2020 6578 6365 7074 2072 6571        except req
+000023c0: 7565 7374 732e 6578 6365 7074 696f 6e73  uests.exceptions
+000023d0: 2e48 5454 5045 7272 6f72 2061 7320 6865  .HTTPError as he
+000023e0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+000023f0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002410: 6622 556e 6162 6c65 2074 6f20 6372 6561  f"Unable to crea
+00002420: 7465 2047 6974 4875 6220 7265 706f 2068  te GitHub repo h
+00002430: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002440: 6d2f 7b6f 776e 6572 7d2f 7b72 6570 6f7d  m/{owner}/{repo}
+00002450: 202d 2065 7272 6f72 206d 6573 7361 6765   - error message
+00002460: 2066 726f 6d20 4769 7448 7562 2069 733a   from GitHub is:
+00002470: 207b 6865 7d22 0a20 2020 2020 2020 2020   {he}".         
+00002480: 2020 2029 0a20 2020 2065 6c73 653a 0a20     ).    else:. 
+00002490: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
+000024a0: 726e 696e 6728 6622 4769 7448 7562 2072  rning(f"GitHub r
+000024b0: 6570 6f20 6874 7470 733a 2f2f 6769 7468  epo https://gith
+000024c0: 7562 2e63 6f6d 2f7b 6f77 6e65 727d 2f7b  ub.com/{owner}/{
+000024d0: 7265 706f 7d20 616c 7265 6164 7920 6578  repo} already ex
+000024e0: 6973 7473 2229 0a0a 2020 2020 7472 793a  ists")..    try:
+000024f0: 0a20 2020 2020 2020 2023 2053 6563 7265  .        # Secre
+00002500: 7473 0a20 2020 2020 2020 2069 6620 636f  ts.        if co
+00002510: 6e66 6967 2e70 726f 7669 6465 7220 3d3d  nfig.provider ==
+00002520: 2050 726f 7669 6465 7245 6e75 6d2e 646f   ProviderEnum.do
+00002530: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00002540: 7220 6e61 6d65 2069 6e20 7b0a 2020 2020  r name in {.    
+00002550: 2020 2020 2020 2020 2020 2020 2241 5753              "AWS
+00002560: 5f41 4343 4553 535f 4b45 595f 4944 222c  _ACCESS_KEY_ID",
+00002570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002580: 2022 4157 535f 5345 4352 4554 5f41 4343   "AWS_SECRET_ACC
+00002590: 4553 535f 4b45 5922 2c0a 2020 2020 2020  ESS_KEY",.      
+000025a0: 2020 2020 2020 2020 2020 2253 5041 4345            "SPACE
+000025b0: 535f 4143 4345 5353 5f4b 4559 5f49 4422  S_ACCESS_KEY_ID"
+000025c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000025d0: 2020 2253 5041 4345 535f 5345 4352 4554    "SPACES_SECRET
+000025e0: 5f41 4343 4553 535f 4b45 5922 2c0a 2020  _ACCESS_KEY",.  
+000025f0: 2020 2020 2020 2020 2020 2020 2020 2244                "D
+00002600: 4947 4954 414c 4f43 4541 4e5f 544f 4b45  IGITALOCEAN_TOKE
+00002610: 4e22 2c0a 2020 2020 2020 2020 2020 2020  N",.            
+00002620: 7d3a 0a20 2020 2020 2020 2020 2020 2020  }:.             
+00002630: 2020 2067 6974 6875 622e 7570 6461 7465     github.update
+00002640: 5f73 6563 7265 7428 6f77 6e65 722c 2072  _secret(owner, r
+00002650: 6570 6f2c 206e 616d 652c 206f 732e 656e  epo, name, os.en
+00002660: 7669 726f 6e5b 6e61 6d65 5d29 0a20 2020  viron[name]).   
+00002670: 2020 2020 2065 6c69 6620 636f 6e66 6967       elif config
+00002680: 2e70 726f 7669 6465 7220 3d3d 2050 726f  .provider == Pro
+00002690: 7669 6465 7245 6e75 6d2e 6177 733a 0a20  viderEnum.aws:. 
+000026a0: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
+000026b0: 616d 6520 696e 207b 0a20 2020 2020 2020  ame in {.       
+000026c0: 2020 2020 2020 2020 2022 4157 535f 4143           "AWS_AC
+000026d0: 4345 5353 5f4b 4559 5f49 4422 2c0a 2020  CESS_KEY_ID",.  
+000026e0: 2020 2020 2020 2020 2020 2020 2020 2241                "A
+000026f0: 5753 5f53 4543 5245 545f 4143 4345 5353  WS_SECRET_ACCESS
+00002700: 5f4b 4559 222c 0a20 2020 2020 2020 2020  _KEY",.         
+00002710: 2020 207d 3a0a 2020 2020 2020 2020 2020     }:.          
+00002720: 2020 2020 2020 6769 7468 7562 2e75 7064        github.upd
+00002730: 6174 655f 7365 6372 6574 286f 776e 6572  ate_secret(owner
+00002740: 2c20 7265 706f 2c20 6e61 6d65 2c20 6f73  , repo, name, os
+00002750: 2e65 6e76 6972 6f6e 5b6e 616d 655d 290a  .environ[name]).
+00002760: 2020 2020 2020 2020 656c 6966 2063 6f6e          elif con
+00002770: 6669 672e 7072 6f76 6964 6572 203d 3d20  fig.provider == 
+00002780: 5072 6f76 6964 6572 456e 756d 2e67 6370  ProviderEnum.gcp
+00002790: 3a0a 2020 2020 2020 2020 2020 2020 6769  :.            gi
+000027a0: 7468 7562 2e75 7064 6174 655f 7365 6372  thub.update_secr
+000027b0: 6574 286f 776e 6572 2c20 7265 706f 2c20  et(owner, repo, 
+000027c0: 2250 524f 4a45 4354 5f49 4422 2c20 6f73  "PROJECT_ID", os
+000027d0: 2e65 6e76 6972 6f6e 5b22 5052 4f4a 4543  .environ["PROJEC
+000027e0: 545f 4944 225d 290a 2020 2020 2020 2020  T_ID"]).        
+000027f0: 2020 2020 7769 7468 206f 7065 6e28 6f73      with open(os
+00002800: 2e65 6e76 6972 6f6e 5b22 474f 4f47 4c45  .environ["GOOGLE
+00002810: 5f43 5245 4445 4e54 4941 4c53 225d 2920  _CREDENTIALS"]) 
+00002820: 6173 2066 3a0a 2020 2020 2020 2020 2020  as f:.          
+00002830: 2020 2020 2020 6769 7468 7562 2e75 7064        github.upd
+00002840: 6174 655f 7365 6372 6574 286f 776e 6572  ate_secret(owner
+00002850: 2c20 7265 706f 2c20 2247 4f4f 474c 455f  , repo, "GOOGLE_
+00002860: 4352 4544 454e 5449 414c 5322 2c20 662e  CREDENTIALS", f.
+00002870: 7265 6164 2829 290a 2020 2020 2020 2020  read()).        
+00002880: 656c 6966 2063 6f6e 6669 672e 7072 6f76  elif config.prov
+00002890: 6964 6572 203d 3d20 5072 6f76 6964 6572  ider == Provider
+000028a0: 456e 756d 2e61 7a75 7265 3a0a 2020 2020  Enum.azure:.    
+000028b0: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
+000028c0: 2069 6e20 7b0a 2020 2020 2020 2020 2020   in {.          
+000028d0: 2020 2020 2020 2241 524d 5f43 4c49 454e        "ARM_CLIEN
+000028e0: 545f 4944 222c 0a20 2020 2020 2020 2020  T_ID",.         
+000028f0: 2020 2020 2020 2022 4152 4d5f 434c 4945         "ARM_CLIE
+00002900: 4e54 5f53 4543 5245 5422 2c0a 2020 2020  NT_SECRET",.    
+00002910: 2020 2020 2020 2020 2020 2020 2241 524d              "ARM
+00002920: 5f53 5542 5343 5249 5054 494f 4e5f 4944  _SUBSCRIPTION_ID
+00002930: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002940: 2020 2022 4152 4d5f 5445 4e41 4e54 5f49     "ARM_TENANT_I
+00002950: 4422 2c0a 2020 2020 2020 2020 2020 2020  D",.            
+00002960: 7d3a 0a20 2020 2020 2020 2020 2020 2020  }:.             
+00002970: 2020 2067 6974 6875 622e 7570 6461 7465     github.update
+00002980: 5f73 6563 7265 7428 6f77 6e65 722c 2072  _secret(owner, r
+00002990: 6570 6f2c 206e 616d 652c 206f 732e 656e  epo, name, os.en
+000029a0: 7669 726f 6e5b 6e61 6d65 5d29 0a20 2020  viron[name]).   
+000029b0: 2020 2020 2067 6974 6875 622e 7570 6461       github.upda
+000029c0: 7465 5f73 6563 7265 7428 0a20 2020 2020  te_secret(.     
+000029d0: 2020 2020 2020 206f 776e 6572 2c20 7265         owner, re
+000029e0: 706f 2c20 2252 4550 4f53 4954 4f52 595f  po, "REPOSITORY_
+000029f0: 4143 4345 5353 5f54 4f4b 454e 222c 206f  ACCESS_TOKEN", o
+00002a00: 732e 656e 7669 726f 6e5b 2247 4954 4855  s.environ["GITHU
+00002a10: 425f 544f 4b45 4e22 5d0a 2020 2020 2020  B_TOKEN"].      
+00002a20: 2020 290a 2020 2020 6578 6365 7074 2072    ).    except r
+00002a30: 6571 7565 7374 732e 6578 6365 7074 696f  equests.exceptio
+00002a40: 6e73 2e48 5454 5045 7272 6f72 2061 7320  ns.HTTPError as 
+00002a50: 6865 3a0a 2020 2020 2020 2020 7261 6973  he:.        rais
+00002a60: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+00002a70: 2020 2020 2020 2020 2020 6622 556e 6162            f"Unab
+00002a80: 6c65 2074 6f20 7365 7420 5365 6372 6574  le to set Secret
+00002a90: 7320 6f6e 2047 6974 4875 6220 7265 706f  s on GitHub repo
+00002aa0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00002ab0: 636f 6d2f 7b6f 776e 6572 7d2f 7b72 6570  com/{owner}/{rep
+00002ac0: 6f7d 202d 2065 7272 6f72 206d 6573 7361  o} - error messa
+00002ad0: 6765 2066 726f 6d20 4769 7448 7562 2069  ge from GitHub i
+00002ae0: 733a 207b 6865 7d22 0a20 2020 2020 2020  s: {he}".       
+00002af0: 2029 0a0a 2020 2020 7265 7475 726e 2066   )..    return f
+00002b00: 2267 6974 4067 6974 6875 622e 636f 6d3a  "git@github.com:
+00002b10: 7b6f 776e 6572 7d2f 7b72 6570 6f7d 2e67  {owner}/{repo}.g
+00002b20: 6974 220a 0a0a 6465 6620 6769 745f 7265  it"...def git_re
+00002b30: 706f 7369 746f 7279 5f69 6e69 7469 616c  pository_initial
+00002b40: 697a 6528 6769 745f 7265 706f 7369 746f  ize(git_reposito
+00002b50: 7279 293a 0a20 2020 2069 6620 6e6f 7420  ry):.    if not 
+00002b60: 6769 742e 6973 5f67 6974 5f72 6570 6f28  git.is_git_repo(
+00002b70: 5061 7468 2e63 7764 2829 293a 0a20 2020  Path.cwd()):.   
+00002b80: 2020 2020 2067 6974 2e69 6e69 7469 616c       git.initial
+00002b90: 697a 655f 6769 7428 5061 7468 2e63 7764  ize_git(Path.cwd
+00002ba0: 2829 290a 2020 2020 6769 742e 6164 645f  ()).    git.add_
+00002bb0: 6769 745f 7265 6d6f 7465 2867 6974 5f72  git_remote(git_r
+00002bc0: 6570 6f73 6974 6f72 792c 2070 6174 683d  epository, path=
+00002bd0: 5061 7468 2e63 7764 2829 2c20 7265 6d6f  Path.cwd(), remo
+00002be0: 7465 5f6e 616d 653d 226f 7269 6769 6e22  te_name="origin"
+00002bf0: 290a                                     ).
```

### Comparing `nebari-2024.4.1/src/_nebari/keycloak.py` & `nebari-2024.4.1rc1/src/_nebari/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/render.py` & `nebari-2024.4.1rc1/src/_nebari/render.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/upgrade.py` & `nebari-2024.4.1rc1/src/_nebari/upgrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 
 import rich
 from packaging.version import Version
 from pydantic.error_wrappers import ValidationError
 from rich.prompt import Prompt
 
 from _nebari.config import backup_configuration
-from _nebari.stages.infrastructure import (
-    provider_enum_default_node_groups_map,
-    provider_enum_name_map,
-)
 from _nebari.utils import (
     get_k8s_version_prefix,
     get_provider_config_block_name,
     load_yaml,
     yaml,
 )
 from _nebari.version import __version__, rounded_ver_parse
@@ -738,45 +734,14 @@
         self, config, start_version, config_filename: Path, *args, **kwargs
     ):
         rich.print("Ready to upgrade to Nebari version [green]2024.3.3[/green].")
 
         return config
 
 
-class Upgrade_2024_4_1(UpgradeStep):
-    version = "2024.4.1"
-
-    def _version_specific_upgrade(
-        self, config, start_version, config_filename: Path, *args, **kwargs
-    ):
-        # Default configuration for the node groups was added in this version. Therefore,
-        # users upgrading who don't have any specific node groups defined on their config
-        # file already, will be prompted and asked whether they want to include the default
-        if provider := config.get("provider", ""):
-            provider_full_name = provider_enum_name_map[provider]
-            if provider_full_name in config and "node_groups" not in config.get(
-                provider_full_name, {}
-            ):
-                try:
-                    default_node_groups = provider_enum_default_node_groups_map[
-                        provider
-                    ]
-                    continue_ = Prompt.ask(
-                        f"Would you like to include the default configuration for the node groups in [purple]{config_filename}[/purple]?",
-                        choices=["y", "N"],
-                        default="N",
-                    )
-                    if continue_ == "y":
-                        config[provider_full_name]["node_groups"] = default_node_groups
-                except KeyError:
-                    pass
-
-        return config
-
-
 __rounded_version__ = str(rounded_ver_parse(__version__))
 
 # Manually-added upgrade steps must go above this line
 if not UpgradeStep.has_step(__rounded_version__):
     # Always have a way to upgrade to the latest full version number, even if no customizations
     # Don't let dev/prerelease versions cloud things
     class UpgradeLatest(UpgradeStep):
```

### Comparing `nebari-2024.4.1/src/_nebari/utils.py` & `nebari-2024.4.1rc1/src/_nebari/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/version.py` & `nebari-2024.4.1rc1/src/_nebari/version.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/provider/git.py` & `nebari-2024.4.1rc1/src/_nebari/provider/git.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/provider/terraform.py` & `nebari-2024.4.1rc1/src/_nebari/provider/terraform.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/provider/cicd/github.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cicd/github.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/provider/cicd/gitlab.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cicd/gitlab.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/provider/cicd/linter.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cicd/linter.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/provider/cloud/amazon_web_services.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cloud/amazon_web_services.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/provider/cloud/azure_cloud.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cloud/azure_cloud.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/provider/cloud/digital_ocean.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cloud/digital_ocean.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/provider/cloud/google_cloud.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cloud/google_cloud.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/provider/dns/cloudflare.py` & `nebari-2024.4.1rc1/src/_nebari/provider/dns/cloudflare.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/provider/oauth/auth0.py` & `nebari-2024.4.1rc1/src/_nebari/provider/oauth/auth0.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/base.py` & `nebari-2024.4.1rc1/src/_nebari/stages/base.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/tf_objects.py` & `nebari-2024.4.1rc1/src/_nebari/stages/tf_objects.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/bootstrap/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,18 +179,14 @@
         }
     elif config.provider == schema.ProviderEnum.existing:
         return config.existing.node_selectors
     else:
         return config.local.dict()["node_selectors"]
 
 
-def node_groups_to_dict(node_groups):
-    return {ng_name: ng.dict() for ng_name, ng in node_groups.items()}
-
-
 @contextlib.contextmanager
 def kubernetes_provider_context(kubernetes_credentials: Dict[str, str]):
     credential_mapping = {
         "config_path": "KUBE_CONFIG_PATH",
         "config_context": "KUBE_CTX",
         "username": "KUBE_USER",
         "password": "KUBE_PASSWORD",
@@ -542,21 +538,14 @@
     schema.ProviderEnum.do: "digital_ocean",
 }
 
 provider_name_abbreviation_map: Dict[str, str] = {
     value: key.value for key, value in provider_enum_name_map.items()
 }
 
-provider_enum_default_node_groups_map: Dict[schema.ProviderEnum, Any] = {
-    schema.ProviderEnum.gcp: node_groups_to_dict(DEFAULT_GCP_NODE_GROUPS),
-    schema.ProviderEnum.aws: node_groups_to_dict(DEFAULT_AWS_NODE_GROUPS),
-    schema.ProviderEnum.azure: node_groups_to_dict(DEFAULT_AZURE_NODE_GROUPS),
-    schema.ProviderEnum.do: node_groups_to_dict(DEFAULT_DO_NODE_GROUPS),
-}
-
 
 class InputSchema(schema.Base):
     local: Optional[LocalProvider]
     existing: Optional[ExistingProvider]
     google_cloud_platform: Optional[GoogleCloudPlatformProvider]
     amazon_web_services: Optional[AmazonWebServicesProvider]
     azure: Optional[AzureProvider]
```

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/local/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/local/metallb.yaml` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/infrastructure/template/local/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/template/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/template/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/conda-store.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/monitoring.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/middleware.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/middleware.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/terraform_state/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/terraform_state/template/aws/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/terraform_state/template/azure/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/terraform_state/template/do/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/terraform_state/template/gcp/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/subcommands/deploy.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/subcommands/destroy.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/subcommands/dev.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/dev.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/subcommands/info.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/info.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/subcommands/init.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/init.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/subcommands/keycloak.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/subcommands/render.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/render.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/subcommands/support.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/support.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/subcommands/upgrade.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/_nebari/subcommands/validate.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/validate.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/nebari/hookspecs.py` & `nebari-2024.4.1rc1/src/nebari/hookspecs.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/nebari/plugins.py` & `nebari-2024.4.1rc1/src/nebari/plugins.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/src/nebari/schema.py` & `nebari-2024.4.1rc1/src/nebari/schema.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/utils.py` & `nebari-2024.4.1rc1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/common/config_mod_utils.py` & `nebari-2024.4.1rc1/tests/common/config_mod_utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/common/kube_api.py` & `nebari-2024.4.1rc1/tests/common/kube_api.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/common/navigator.py` & `nebari-2024.4.1rc1/tests/common/navigator.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/common/playwright_fixtures.py` & `nebari-2024.4.1rc1/tests/common/playwright_fixtures.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/common/run_notebook.py` & `nebari-2024.4.1rc1/tests/common/run_notebook.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/common/notebooks/test_notebook_output.ipynb` & `nebari-2024.4.1rc1/tests/common/notebooks/test_notebook_output.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/common/tests/test_notebook.py` & `nebari-2024.4.1rc1/tests/common/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_deployment/test_dask_gateway.py` & `nebari-2024.4.1rc1/tests/tests_deployment/test_dask_gateway.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_deployment/test_grafana_api.py` & `nebari-2024.4.1rc1/tests/tests_deployment/test_grafana_api.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_deployment/test_jupyterhub_ssh.py` & `nebari-2024.4.1rc1/tests/tests_deployment/test_jupyterhub_ssh.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_deployment/test_loki_deployment.py` & `nebari-2024.4.1rc1/tests/tests_deployment/test_loki_deployment.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_deployment/utils.py` & `nebari-2024.4.1rc1/tests/tests_deployment/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_deployment/assets/notebook/simple.ipynb` & `nebari-2024.4.1rc1/tests/tests_deployment/assets/notebook/simple.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_e2e/package-lock.json` & `nebari-2024.4.1rc1/tests/tests_e2e/package-lock.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_e2e/cypress/integration/main.js` & `nebari-2024.4.1rc1/tests/tests_e2e/cypress/integration/main.js`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb` & `nebari-2024.4.1rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_e2e/cypress/plugins/index.js` & `nebari-2024.4.1rc1/tests/tests_e2e/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_e2e/cypress/support/index.js` & `nebari-2024.4.1rc1/tests/tests_e2e/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_e2e/playwright/README.md` & `nebari-2024.4.1rc1/tests/tests_e2e/playwright/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_e2e/playwright/test_playwright.py` & `nebari-2024.4.1rc1/tests/tests_e2e/playwright/test_playwright.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_integration/README.md` & `nebari-2024.4.1rc1/tests/tests_integration/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_integration/deployment_fixtures.py` & `nebari-2024.4.1rc1/tests/tests_integration/deployment_fixtures.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_integration/test_all_clouds.py` & `nebari-2024.4.1rc1/tests/tests_integration/test_all_clouds.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_integration/test_gpu.py` & `nebari-2024.4.1rc1/tests/tests_integration/test_gpu.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_integration/test_preemptible.py` & `nebari-2024.4.1rc1/tests/tests_integration/test_preemptible.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/conftest.py` & `nebari-2024.4.1rc1/tests/tests_unit/conftest.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_cli.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_cli_deploy.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_cli_dev.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_dev.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_cli_init.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_init.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_cli_init_repository.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_init_repository.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_cli_keycloak.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_cli_support.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_support.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_cli_upgrade.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_cli_validate.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_validate.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_commons.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_commons.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_config.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_dependencies.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_init.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_init.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_provider.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_provider.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_render.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_render.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_schema.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/test_upgrade.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/utils.py` & `nebari-2024.4.1rc1/tests/tests_unit/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/cli_validate/aws.happy.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/aws.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/cli_validate/azure.happy.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/azure.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/cli_validate/do.happy.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/do.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/cli_validate/gcp.happy.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/gcp.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/cli_validate/local.happy.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/.gitignore` & `nebari-2024.4.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/LICENSE` & `nebari-2024.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/README.md` & `nebari-2024.4.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/pyproject.toml` & `nebari-2024.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1/PKG-INFO` & `nebari-2024.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nebari
-Version: 2024.4.1
+Version: 2024.4.1rc1
 Summary: A Jupyter and Dask-powered open source data science platform.
 Project-URL: Documentation, https://www.nebari.dev/docs
 Project-URL: Source, https://github.com/nebari-dev/nebari
 Author-email: Nebari development team <internal-it@quansight.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: aws,azure,dask,do,gcp,jupyter,nebari
```

