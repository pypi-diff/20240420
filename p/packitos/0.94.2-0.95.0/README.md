# Comparing `tmp/packitos-0.94.2.tar.gz` & `tmp/packitos-0.95.0.tar.gz`

## Comparing `packitos-0.94.2.tar` & `packitos-0.95.0.tar`

### file list

```diff
@@ -1,408 +1,408 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 packitos-0.94.2/.git_archival.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 packitos-0.94.2/.gitattributes
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 packitos-0.94.2/.packit.yaml
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 packitos-0.94.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 packitos-0.94.2/.zuul.yaml
--rw-r--r--   0        0        0    56867 2020-02-02 00:00:00.000000 packitos-0.94.2/CHANGELOG.md
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 packitos-0.94.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 packitos-0.94.2/Containerfile
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 packitos-0.94.2/Containerfile.tests
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 packitos-0.94.2/DCO
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 packitos-0.94.2/LICENSE_HEADER.txt
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 packitos-0.94.2/Makefile
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 packitos-0.94.2/ansible.cfg
--rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 packitos-0.94.2/packit.spec
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 packitos-0.94.2/release-conf.yaml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 packitos-0.94.2/.fmf/version
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/stale.yml
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/workflows/build-and-push.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/workflows/check-release-notes.yml
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/workflows/do_release.yml
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/workflows/opened-issues-to-the-board.yml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/workflows/prepare-release.yml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0  1843517 2020-02-02 00:00:00.000000 packitos-0.94.2/design/logo-packit.sketch
--rw-r--r--   0        0        0   135444 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/hexsticker.png
--rw-r--r--   0        0        0   132230 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-dark.png
--rw-r--r--   0        0        0    75002 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-extended.jpg
--rw-r--r--   0        0        0    48468 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-extended.png
--rw-r--r--   0        0        0    24881 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-extended.svg
--rw-r--r--   0        0        0   106567 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-guideline.pdf
--rw-r--r--   0        0        0    66141 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-no-borders.jpg
--rw-r--r--   0        0        0   143587 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-no-borders.png
--rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-small.png
--rw-r--r--   0        0        0    70268 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-square-small-borders.jpg
--rw-r--r--   0        0        0   150044 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-square-small-borders.png
--rw-r--r--   0        0        0    43972 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-stg-square-bigger-borders.svg
--rw-r--r--   0        0        0   107242 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-stg-square-small-borders.png
--rw-r--r--   0        0        0    43981 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-stg-square-small-borders.svg
--rw-r--r--   0        0        0    28826 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-stg.png
--rw-r--r--   0        0        0    24351 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-stg.svg
--rw-r--r--   0        0        0    18005 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-text.jpg
--rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-text.png
--rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-text.svg
--rw-r--r--   0        0        0   144552 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-white.png
--rw-r--r--   0        0        0   158074 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo.png
--rw-r--r--   0        0        0    14697 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 packitos-0.94.2/files/install-requirements-git.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 packitos-0.94.2/files/install-requirements-pip.yaml
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 packitos-0.94.2/files/install-requirements-rpms.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 packitos-0.94.2/files/local-tests-requirements.yaml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 packitos-0.94.2/files/packit-testing-farm-prepare-session-recording.yaml
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 packitos-0.94.2/files/packit-testing-farm-prepare.yaml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 packitos-0.94.2/files/zuul-reverse-dep-packit-service.yaml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.94.2/files/zuul-tests-session-recording.yaml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 packitos-0.94.2/files/zuul-tests.yaml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 packitos-0.94.2/files/bash-completion/packit
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/build-rpm-deps.yaml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/centpkg.yaml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/generic-dnf-requirements.yaml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/install-packit-service.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/install-packit.yaml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/ogr.yaml
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/packit-service-requirements.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/project-dir.yaml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/python-compile-deps.yaml
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/requre.yaml
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/rpm-test-deps.yaml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/sandcastle.yaml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/specfile.yaml
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/__init__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/actions.py
--rw-r--r--   0        0        0    90697 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/api.py
--rw-r--r--   0        0        0    29435 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/base_git.py
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/command_handler.py
--rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/constants.py
--rw-r--r--   0        0        0    20419 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/copr_helper.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/dist_git_instance.py
--rw-r--r--   0        0        0    25019 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/distgit.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/exceptions.py
--rw-r--r--   0        0        0    40197 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/local_project.py
--rw-r--r--   0        0        0    35127 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/patches.py
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/pkgtool.py
--rw-r--r--   0        0        0    29471 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/schema.py
--rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/security.py
--rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/source_git.py
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/status.py
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/sync.py
--rw-r--r--   0        0        0    53439 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/upstream.py
--rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/vm_image_build.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/__init__.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/build.py
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/create_update.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/dist_git.py
--rw-r--r--   0        0        0    14719 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/dist_git_init.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/init.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/packit_base.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/prepare_sources.py
--rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/propose_downstream.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/push_updates.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/source_git.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/source_git_init.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/source_git_status.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/srpm.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/status.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/sync_from_downstream.py
--rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/types.py
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/update_dist_git.py
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/update_source_git.py
--rw-r--r--   0        0        0    13599 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/utils.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/validate_config.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/builds/__init__.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/builds/copr_build.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/builds/in_image_builder.py
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/builds/koji_build.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/builds/local_build.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/builds/mock_build.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/__init__.py
--rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/aliases.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/commands.py
--rw-r--r--   0        0        0    24627 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/common_package_config.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/config.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/job_config.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/notifications.py
--rw-r--r--   0        0        0    19422 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/package_config.py
--rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/package_config_validator.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/requirements.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/sources.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/data/__init__.py
--rwxr-xr-x   0        0        0     3233 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/data/_packitpatch
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/bodhi.py
--rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/changelog_helper.py
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/commands.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/decorators.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/extensions.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/koji_helper.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/logging.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/lookaside.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/monitoring.py
--rw-r--r--   0        0        0    18617 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/repo.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/source_script.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/upstream_version.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/versions.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/README.md
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/full.fmf
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/git_reference.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/main.fmf
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/rpmlint.fmf
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/session-recording.fmf
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/smoke.fmf
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/__init__.py
--rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/conftest.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/full.fmf
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/smoke.fmf
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/smoke.sh
--rw-r--r--   0        0        0    22298 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/spellbook.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/copr_config
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cockpit-ostree/Makefile
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cockpit-ostree/cockpit-ostree.spec.dg
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cockpit-ostree/cockpit-ostree.spec.in
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cockpit-ostree/packit.yaml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/.cronie.metadata
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/.gitignore
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/SOURCES/cronie-1.5.2-restart-on-failure.patch
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/SOURCES/fix-memory-leaks.patch
--rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/SOURCES/fix-unsafe-code.patch
--rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/SPECS/cronie.spec
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dg-ogr/.packit.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dg-ogr/README.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dg-ogr/README.packit
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dg-ogr/python-ogr.spec
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dg-ogr/sources
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dist_git/.packit.yaml
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dist_git/beer.spec
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dist_git_with_autochangelog/.packit.yaml
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dist_git_with_autochangelog/beer.spec
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/.packit.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/LICENSE
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/Makefile
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/README.rst
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/edd
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/edd.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/docs/man.rst
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/empty_changelog/.packit.yaml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/empty_changelog/beer.spec
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/no_version_tag_in_spec/.packit.yaml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/no_version_tag_in_spec/beer.spec
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/no_version_tag_in_spec/source
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/osbuild/.packit.yaml
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/osbuild/__init__.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/osbuild/osbuild.spec
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/osbuild/setup.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/osbuild/sources/test
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/previous/git-diff.patch
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/previous/missing-diff-line.patch
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/previous/unified-diff.patch
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/previous/weird-identical.patch
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/regenerated/git-diff.patch
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/regenerated/missing-diff-line.patch
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/regenerated/unified-diff.patch
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/regenerated/weird-identical.patch
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/rpms/hello/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/rpms/hello/hello.spec
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/src/hello/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/src/hello/.distro/hello.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/src/hello/.distro/source-git.yaml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/rpms/hello/0017-Patch-This..patch
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/rpms/hello/from-git.patch
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/rpms/hello/hello.spec
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/rpms/hello/sources
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/rpms/hello/turn-into-fedora.patch
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/snapd/.packit.yaml
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/snapd/packaging/fedora/fix-spec
--rwxr-xr-x   0        0        0     1866 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/snapd/packaging/fedora/pack-source
--rw-r--r--   0        0        0    18386 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/snapd/packaging/fedora/snapd.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/snapd/packaging/fedora/some-file-to-add
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/snapd/vendor/vendor.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sourcegit/source_git/ignored_file.txt
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sourcegit/source_git/.distro/beer.spec
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sourcegit/source_git/.distro/source-git.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sourcegit/upstream/big-source-file.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/spec_not_in_root/upstream/.packit.yaml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/spec_not_in_root/upstream/dir_with_spec/beer.spec
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/src/.gitignore
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/src/hello/Makefile
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/src/hello/README.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/src/hello/hello.rs
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sync_files/a.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sync_files/b.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sync_files/c.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sync_files/example_dir/d.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sync_files/example_dir/e.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sync_files/example_dir/f.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git/.packit.yaml
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git/beer.spec
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git_macro_in_source/.packit.yaml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git_macro_in_source/beer.spec
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git_weird_sources/.packit.yaml
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git_weird_sources/beer.spec
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git_with_multiple_sources/.packit.yaml
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git_with_multiple_sources/beer.spec
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/.packit.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/AUDIT
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/BENCHMARKS
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/BUGS
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/COPYING
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Changelog
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/FAQ
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/INSTALL
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/README
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/README.security
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/REWARD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/SIZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/SPEED
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/TODO
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/TUNING
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/vsftpd.8
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/vsftpd.conf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/vsftpd.conf.5
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/EXAMPLE/example
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd-generator
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.ftpusers
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.pam
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.service
--rw-r--r--   0        0        0    27817 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.target
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.user_list
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.xinetd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd@.service
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd_conf_migrate.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/RedHat/vsftpd.log
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/SECURITY/security
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/spellbook.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/test_local_build.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/test_prepare_sources.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/test_srpm.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/test_validate_config.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/README.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/bodhi_latest_builds.py
--rw-r--r--   0        0        0    42198 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/bodhi_status_updates.py
--rw-r--r--   0        0        0    15059 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/conftest.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_actions.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_api.py
--rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_base_git.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_build.py
--rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_changelog_helper.py
--rw-r--r--   0        0        0    21951 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_copr_build.py
--rw-r--r--   0        0        0    15035 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_create_update.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_distgit.py
--rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_get_api.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_init.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_local_project.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_pagure.py
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_patches.py
--rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_push_updates.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_security.py
--rw-r--r--   0        0        0    24135 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_source_git.py
--rw-r--r--   0        0        0     8032 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_source_git_init.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_source_git_status.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_source_git_synch_push.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_source_git_update_source_git.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_spec.py
--rw-r--r--   0        0        0    18153 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_update.py
--rw-r--r--   0        0        0    20720 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_upstream.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_using_cockpit.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_using_examples.py
--rw-r--r--   0        0        0     7837 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_validate_config.py
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_validate_synced_files.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/__init__.py
--rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/conftest.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_actions.py
--rw-r--r--   0        0        0    20019 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_api.py
--rw-r--r--   0        0        0    34220 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_base_git.py
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_cli.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_cli_utils.py
--rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_copr_helper.py
--rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_dg.py
--rw-r--r--   0        0        0     7735 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_dist_git_init.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_image_builder.py
--rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_iterate_packages.py
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_koji_build.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_load_authentication.py
--rw-r--r--   0        0        0    34254 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_local_project.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_login_with_kerberos.py
--rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_patches.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_prepare_sources.py
--rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_propose_downstream.py
--rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_security.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_specfile.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_status.py
--rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_sync.py
--rw-r--r--   0        0        0    19993 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_upstream.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/config/__init__.py
--rw-r--r--   0        0        0    22698 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/config/test_config.py
--rw-r--r--   0        0        0    14916 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/config/test_config_aliases.py
--rw-r--r--   0        0        0    94771 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/config/test_package_config.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_changelog_helper.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_commands.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_decorators.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_dist_git_instance.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_exceptions.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_koji_helper.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_lookaside.py
--rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_repo.py
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_source_script.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_upstream_version.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_versions.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/__init__.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/main.fmf
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_api.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_base_git.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_image_builder.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_local_project.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_repository_cache.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_status.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/testbase.py
--rw-r--r--   0        0        0   513530 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml
--rw-r--r--   0        0        0    53824 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz
--rw-r--r--   0        0        0  1387468 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz
--rw-r--r--   0        0        0   162050 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.packit-dist-gitfnk035np_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0  1425896 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    86697 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml
--rw-r--r--   0        0        0    64940 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.tmp5bwaoc9m_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml
--rw-r--r--   0        0        0    34569 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr_no_merge.yaml
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone2_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0  2668265 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml.tmpgtdjxv_x_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    43243 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.packit-dist-gitzea090jp_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.tmpv3zw6n9v_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0   155977 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.packit-dist-gitl12hm88e_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.tmpyqn3l5sr_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0   152944 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml.tmp9u1xyoyx_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    40654 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_status.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_status.yaml.tmp620nfd0i_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    70501 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml.tmpco60quxn_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.94.2/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 packitos-0.94.2/LICENSE
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 packitos-0.94.2/README.md
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 packitos-0.94.2/pyproject.toml
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 packitos-0.94.2/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 packitos-0.95.0/.git_archival.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 packitos-0.95.0/.gitattributes
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 packitos-0.95.0/.packit.yaml
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 packitos-0.95.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 packitos-0.95.0/.zuul.yaml
+-rw-r--r--   0        0        0    57138 2020-02-02 00:00:00.000000 packitos-0.95.0/CHANGELOG.md
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 packitos-0.95.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 packitos-0.95.0/Containerfile
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 packitos-0.95.0/Containerfile.tests
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 packitos-0.95.0/DCO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 packitos-0.95.0/LICENSE_HEADER.txt
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 packitos-0.95.0/Makefile
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 packitos-0.95.0/ansible.cfg
+-rw-r--r--   0        0        0    13350 2020-02-02 00:00:00.000000 packitos-0.95.0/packit.spec
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 packitos-0.95.0/release-conf.yaml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 packitos-0.95.0/.fmf/version
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/stale.yml
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/workflows/build-and-push.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/workflows/check-release-notes.yml
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/workflows/do_release.yml
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/workflows/opened-issues-to-the-board.yml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/workflows/prepare-release.yml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0  1843517 2020-02-02 00:00:00.000000 packitos-0.95.0/design/logo-packit.sketch
+-rw-r--r--   0        0        0   135444 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/hexsticker.png
+-rw-r--r--   0        0        0   132230 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-dark.png
+-rw-r--r--   0        0        0    75002 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-extended.jpg
+-rw-r--r--   0        0        0    48468 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-extended.png
+-rw-r--r--   0        0        0    24881 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-extended.svg
+-rw-r--r--   0        0        0   106567 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-guideline.pdf
+-rw-r--r--   0        0        0    66141 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-no-borders.jpg
+-rw-r--r--   0        0        0   143587 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-no-borders.png
+-rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-small.png
+-rw-r--r--   0        0        0    70268 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-square-small-borders.jpg
+-rw-r--r--   0        0        0   150044 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-square-small-borders.png
+-rw-r--r--   0        0        0    43972 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-stg-square-bigger-borders.svg
+-rw-r--r--   0        0        0   107242 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-stg-square-small-borders.png
+-rw-r--r--   0        0        0    43981 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-stg-square-small-borders.svg
+-rw-r--r--   0        0        0    28826 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-stg.png
+-rw-r--r--   0        0        0    24351 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-stg.svg
+-rw-r--r--   0        0        0    18005 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-text.jpg
+-rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-text.png
+-rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-text.svg
+-rw-r--r--   0        0        0   144552 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-white.png
+-rw-r--r--   0        0        0   158074 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo.png
+-rw-r--r--   0        0        0    14697 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 packitos-0.95.0/files/install-requirements-git.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 packitos-0.95.0/files/install-requirements-pip.yaml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 packitos-0.95.0/files/install-requirements-rpms.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 packitos-0.95.0/files/local-tests-requirements.yaml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 packitos-0.95.0/files/packit-testing-farm-prepare-session-recording.yaml
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 packitos-0.95.0/files/packit-testing-farm-prepare.yaml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 packitos-0.95.0/files/zuul-reverse-dep-packit-service.yaml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.95.0/files/zuul-tests-session-recording.yaml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 packitos-0.95.0/files/zuul-tests.yaml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 packitos-0.95.0/files/bash-completion/packit
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/build-rpm-deps.yaml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/centpkg.yaml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/generic-dnf-requirements.yaml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/install-packit-service.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/install-packit.yaml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/ogr.yaml
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/packit-service-requirements.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/project-dir.yaml
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/python-compile-deps.yaml
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/requre.yaml
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/rpm-test-deps.yaml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/sandcastle.yaml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/specfile.yaml
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/__init__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/actions.py
+-rw-r--r--   0        0        0    90819 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/api.py
+-rw-r--r--   0        0        0    29435 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/base_git.py
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/command_handler.py
+-rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/constants.py
+-rw-r--r--   0        0        0    20419 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/copr_helper.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/dist_git_instance.py
+-rw-r--r--   0        0        0    25019 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/distgit.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/exceptions.py
+-rw-r--r--   0        0        0    40197 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/local_project.py
+-rw-r--r--   0        0        0    35127 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/patches.py
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/pkgtool.py
+-rw-r--r--   0        0        0    29471 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/schema.py
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/security.py
+-rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/source_git.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/status.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/sync.py
+-rw-r--r--   0        0        0    53439 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/upstream.py
+-rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/vm_image_build.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/build.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/create_update.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/dist_git.py
+-rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/dist_git_init.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/init.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/packit_base.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/prepare_sources.py
+-rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/propose_downstream.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/push_updates.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/source_git.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/source_git_init.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/source_git_status.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/srpm.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/status.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/sync_from_downstream.py
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/types.py
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/update_dist_git.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/update_source_git.py
+-rw-r--r--   0        0        0    13599 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/utils.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/validate_config.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/builds/__init__.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/builds/copr_build.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/builds/in_image_builder.py
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/builds/koji_build.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/builds/local_build.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/builds/mock_build.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/__init__.py
+-rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/aliases.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/commands.py
+-rw-r--r--   0        0        0    24627 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/common_package_config.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/config.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/job_config.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/notifications.py
+-rw-r--r--   0        0        0    19870 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/package_config.py
+-rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/package_config_validator.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/requirements.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/sources.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/data/__init__.py
+-rwxr-xr-x   0        0        0     3233 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/data/_packitpatch
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/bodhi.py
+-rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/changelog_helper.py
+-rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/commands.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/decorators.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/extensions.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/koji_helper.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/logging.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/lookaside.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/monitoring.py
+-rw-r--r--   0        0        0    18617 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/repo.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/source_script.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/upstream_version.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/versions.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/README.md
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/full.fmf
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/git_reference.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/main.fmf
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/rpmlint.fmf
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/session-recording.fmf
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/smoke.fmf
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/__init__.py
+-rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/conftest.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/full.fmf
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/smoke.fmf
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/smoke.sh
+-rw-r--r--   0        0        0    22298 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/spellbook.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/copr_config
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cockpit-ostree/Makefile
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cockpit-ostree/cockpit-ostree.spec.dg
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cockpit-ostree/cockpit-ostree.spec.in
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cockpit-ostree/packit.yaml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/.cronie.metadata
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/.gitignore
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/SOURCES/cronie-1.5.2-restart-on-failure.patch
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/SOURCES/fix-memory-leaks.patch
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/SOURCES/fix-unsafe-code.patch
+-rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/SPECS/cronie.spec
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dg-ogr/.packit.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dg-ogr/README.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dg-ogr/README.packit
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dg-ogr/python-ogr.spec
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dg-ogr/sources
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dist_git/.packit.yaml
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dist_git/beer.spec
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dist_git_with_autochangelog/.packit.yaml
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dist_git_with_autochangelog/beer.spec
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/.packit.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/LICENSE
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/Makefile
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/README.rst
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/edd
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/edd.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/docs/man.rst
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/empty_changelog/.packit.yaml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/empty_changelog/beer.spec
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/no_version_tag_in_spec/.packit.yaml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/no_version_tag_in_spec/beer.spec
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/no_version_tag_in_spec/source
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/osbuild/.packit.yaml
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/osbuild/__init__.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/osbuild/osbuild.spec
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/osbuild/setup.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/osbuild/sources/test
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/previous/git-diff.patch
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/previous/missing-diff-line.patch
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/previous/unified-diff.patch
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/previous/weird-identical.patch
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/regenerated/git-diff.patch
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/regenerated/missing-diff-line.patch
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/regenerated/unified-diff.patch
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/regenerated/weird-identical.patch
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/rpms/hello/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/rpms/hello/hello.spec
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/src/hello/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/src/hello/.distro/hello.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/src/hello/.distro/source-git.yaml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/rpms/hello/0017-Patch-This..patch
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/rpms/hello/from-git.patch
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/rpms/hello/hello.spec
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/rpms/hello/sources
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/rpms/hello/turn-into-fedora.patch
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/snapd/.packit.yaml
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/snapd/packaging/fedora/fix-spec
+-rwxr-xr-x   0        0        0     1866 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/snapd/packaging/fedora/pack-source
+-rw-r--r--   0        0        0    18386 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/snapd/packaging/fedora/snapd.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/snapd/packaging/fedora/some-file-to-add
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/snapd/vendor/vendor.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sourcegit/source_git/ignored_file.txt
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sourcegit/source_git/.distro/beer.spec
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sourcegit/source_git/.distro/source-git.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sourcegit/upstream/big-source-file.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/spec_not_in_root/upstream/.packit.yaml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/spec_not_in_root/upstream/dir_with_spec/beer.spec
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/src/.gitignore
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/src/hello/Makefile
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/src/hello/README.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/src/hello/hello.rs
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sync_files/a.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sync_files/b.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sync_files/c.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sync_files/example_dir/d.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sync_files/example_dir/e.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sync_files/example_dir/f.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git/.packit.yaml
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git/beer.spec
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git_macro_in_source/.packit.yaml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git_macro_in_source/beer.spec
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git_weird_sources/.packit.yaml
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git_weird_sources/beer.spec
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git_with_multiple_sources/.packit.yaml
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git_with_multiple_sources/beer.spec
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/.packit.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/AUDIT
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/BENCHMARKS
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/BUGS
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/COPYING
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Changelog
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/FAQ
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/INSTALL
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/README
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/README.security
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/REWARD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/SIZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/SPEED
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/TODO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/TUNING
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/vsftpd.8
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/vsftpd.conf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/vsftpd.conf.5
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/EXAMPLE/example
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd-generator
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.ftpusers
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.pam
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.service
+-rw-r--r--   0        0        0    27817 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.target
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.user_list
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.xinetd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd@.service
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd_conf_migrate.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/RedHat/vsftpd.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/SECURITY/security
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/spellbook.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/test_local_build.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/test_prepare_sources.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/test_srpm.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/test_validate_config.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/README.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/bodhi_latest_builds.py
+-rw-r--r--   0        0        0    42198 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/bodhi_status_updates.py
+-rw-r--r--   0        0        0    15059 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_actions.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_api.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_base_git.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_build.py
+-rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_changelog_helper.py
+-rw-r--r--   0        0        0    21951 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_copr_build.py
+-rw-r--r--   0        0        0    15035 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_create_update.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_distgit.py
+-rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_get_api.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_init.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_local_project.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_pagure.py
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_patches.py
+-rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_push_updates.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_security.py
+-rw-r--r--   0        0        0    24135 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_source_git.py
+-rw-r--r--   0        0        0     8032 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_source_git_init.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_source_git_status.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_source_git_synch_push.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_source_git_update_source_git.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_spec.py
+-rw-r--r--   0        0        0    18153 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_update.py
+-rw-r--r--   0        0        0    20720 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_upstream.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_using_cockpit.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_using_examples.py
+-rw-r--r--   0        0        0     7837 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_validate_config.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_validate_synced_files.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_actions.py
+-rw-r--r--   0        0        0    20019 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_api.py
+-rw-r--r--   0        0        0    34220 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_base_git.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_cli.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_cli_utils.py
+-rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_copr_helper.py
+-rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_dg.py
+-rw-r--r--   0        0        0     7735 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_dist_git_init.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_image_builder.py
+-rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_iterate_packages.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_koji_build.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_load_authentication.py
+-rw-r--r--   0        0        0    34254 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_local_project.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_login_with_kerberos.py
+-rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_patches.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_prepare_sources.py
+-rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_propose_downstream.py
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_security.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_specfile.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_status.py
+-rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_sync.py
+-rw-r--r--   0        0        0    19993 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_upstream.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/config/__init__.py
+-rw-r--r--   0        0        0    22698 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/config/test_config.py
+-rw-r--r--   0        0        0    14916 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/config/test_config_aliases.py
+-rw-r--r--   0        0        0    95205 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/config/test_package_config.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_changelog_helper.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_commands.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_decorators.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_dist_git_instance.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_exceptions.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_koji_helper.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_lookaside.py
+-rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_repo.py
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_source_script.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_upstream_version.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_versions.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/__init__.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/main.fmf
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_api.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_base_git.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_image_builder.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_local_project.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_repository_cache.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_status.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/testbase.py
+-rw-r--r--   0        0        0   513530 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml
+-rw-r--r--   0        0        0    53824 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz
+-rw-r--r--   0        0        0  1387468 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz
+-rw-r--r--   0        0        0   162050 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.packit-dist-gitfnk035np_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0  1425896 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    86697 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml
+-rw-r--r--   0        0        0    64940 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.tmp5bwaoc9m_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml
+-rw-r--r--   0        0        0    34569 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr_no_merge.yaml
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone2_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0  2668265 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml.tmpgtdjxv_x_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    43243 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.packit-dist-gitzea090jp_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.tmpv3zw6n9v_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0   155977 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.packit-dist-gitl12hm88e_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.tmpyqn3l5sr_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0   152944 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml.tmp9u1xyoyx_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    40654 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_status.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_status.yaml.tmp620nfd0i_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    70501 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml.tmpco60quxn_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.95.0/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 packitos-0.95.0/LICENSE
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 packitos-0.95.0/README.md
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 packitos-0.95.0/pyproject.toml
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 packitos-0.95.0/PKG-INFO
```

### Comparing `packitos-0.94.2/.packit.yaml` & `packitos-0.95.0/.packit.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/.pre-commit-config.yaml` & `packitos-0.95.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/.zuul.yaml` & `packitos-0.95.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/CHANGELOG.md` & `packitos-0.95.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# 0.95.0
+
+- `packit dist-git init` now allows specifying `--version-update-mask` option and also any arbitrary top-level configuration options. (#2288)
+- We have fixed Packit auto-referencing Upstream Release Monitoring bug for release syncing to CentOS Stream. (#2284)
+
 # 0.94.2
 
 - Packit previously put the "[packit]" string as a prefix in the subject of pull-from-upstream commits. Now the prefix is no longer there - this is made unnecessary noise in autochangelog. This affects the default. Custom action can still override this behavior. (#2263)
 - We have fixed a race condition that could occur when multiple `copr_build` jobs sharing a Copr project but having different targets were running at the same time. (#2274)
 
 # 0.94.1
```

### Comparing `packitos-0.94.2/CONTRIBUTING.md` & `packitos-0.95.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/DCO` & `packitos-0.95.0/DCO`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/Makefile` & `packitos-0.95.0/Makefile`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit.spec` & `packitos-0.95.0/packit.spec`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 %if 0%{?el9}
 %bcond_with tests
 %else
 %bcond_without tests
 %endif
 
 Name:           packit
-Version:        0.94.2
+Version:        0.95.0
 Release:        1%{?dist}
 Summary:        A tool for integrating upstream projects with Fedora operating system
 
 License:        MIT
 URL:            https://github.com/packit/packit
 Source0:        %{pypi_source packitos}
 BuildArch:      noarch
@@ -73,14 +73,17 @@
 # Epel9 does not tag the license file in pyproject_files as a license. Manually install it in this case
 %if 0%{?el9}
 %license LICENSE
 %endif
 %doc README.md
 
 %changelog
+* Sat Apr 20 2024 Packit Team <hello@packit.dev> - 0.95.0-1
+- New upstream release 0.95.0
+
 * Mon Apr 08 2024 Packit Team <hello@packit.dev> - 0.94.2-1
 - New upstream release 0.94.2
 
 * Mon Mar 25 2024 Packit Team <hello@packit.dev> - 0.94.1-1
 - New upstream release 0.94.1
 
 * Sun Mar 17 2024 Packit Team <hello@packit.dev> - 0.94.0-1
```

### Comparing `packitos-0.94.2/.github/stale.yml` & `packitos-0.95.0/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/.github/workflows/build-and-push.yml` & `packitos-0.95.0/.github/workflows/build-and-push.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/.github/workflows/do_release.yml` & `packitos-0.95.0/.github/workflows/do_release.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/.github/workflows/prepare-release.yml` & `packitos-0.95.0/.github/workflows/prepare-release.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/.github/workflows/pypi-publish.yml` & `packitos-0.95.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/logo-packit.sketch` & `packitos-0.95.0/design/logo-packit.sketch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/hexsticker.png` & `packitos-0.95.0/design/export/hexsticker.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-dark.png` & `packitos-0.95.0/design/export/logo-dark.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-extended.jpg` & `packitos-0.95.0/design/export/logo-extended.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-extended.png` & `packitos-0.95.0/design/export/logo-extended.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-extended.svg` & `packitos-0.95.0/design/export/logo-extended.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-guideline.pdf` & `packitos-0.95.0/design/export/logo-guideline.pdf`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-no-borders.jpg` & `packitos-0.95.0/design/export/logo-no-borders.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-no-borders.png` & `packitos-0.95.0/design/export/logo-no-borders.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-small.png` & `packitos-0.95.0/design/export/logo-small.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-square-small-borders.jpg` & `packitos-0.95.0/design/export/logo-square-small-borders.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-square-small-borders.png` & `packitos-0.95.0/design/export/logo-square-small-borders.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-stg-square-bigger-borders.svg` & `packitos-0.95.0/design/export/logo-stg-square-bigger-borders.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-stg-square-small-borders.png` & `packitos-0.95.0/design/export/logo-stg-square-small-borders.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-stg-square-small-borders.svg` & `packitos-0.95.0/design/export/logo-stg-square-small-borders.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-stg.png` & `packitos-0.95.0/design/export/logo-stg.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-stg.svg` & `packitos-0.95.0/design/export/logo-stg.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-text.jpg` & `packitos-0.95.0/design/export/logo-text.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-text.png` & `packitos-0.95.0/design/export/logo-text.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-text.svg` & `packitos-0.95.0/design/export/logo-text.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo-white.png` & `packitos-0.95.0/design/export/logo-white.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo.png` & `packitos-0.95.0/design/export/logo.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/design/export/logo.svg` & `packitos-0.95.0/design/export/logo.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/files/local-tests-requirements.yaml` & `packitos-0.95.0/files/local-tests-requirements.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/files/zuul-reverse-dep-packit-service.yaml` & `packitos-0.95.0/files/zuul-reverse-dep-packit-service.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/files/zuul-tests-session-recording.yaml` & `packitos-0.95.0/files/zuul-tests-session-recording.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/files/tasks/packit-service-requirements.yaml` & `packitos-0.95.0/files/tasks/packit-service-requirements.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/files/tasks/rpm-test-deps.yaml` & `packitos-0.95.0/files/tasks/rpm-test-deps.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/actions.py` & `packitos-0.95.0/packit/actions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/api.py` & `packitos-0.95.0/packit/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -969,15 +969,16 @@
         if not force and self.up.is_dirty() and not use_local_content:
             raise PackitException(
                 "The repository is dirty, will not discard the changes. Use --force to bypass.",
             )
         upstream_ref = self.up._expand_git_ref(
             upstream_ref or self.package_config.upstream_ref,
         )
-        if not resolved_bugs:
+        # don't reference Upstream Release Monitoring bug for CentOS
+        if not resolved_bugs and self.package_config.pkg_tool in (None, "fedpkg"):
             upstream_release_monitoring_bug = self.get_upstream_release_monitoring_bug(
                 package_name=self.dg.local_project.repo_name,
                 version=version,
             )
             resolved_bugs = (
                 [upstream_release_monitoring_bug]
                 if upstream_release_monitoring_bug
```

### Comparing `packitos-0.94.2/packit/base_git.py` & `packitos-0.95.0/packit/base_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/command_handler.py` & `packitos-0.95.0/packit/command_handler.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/constants.py` & `packitos-0.95.0/packit/constants.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/copr_helper.py` & `packitos-0.95.0/packit/copr_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/dist_git_instance.py` & `packitos-0.95.0/packit/dist_git_instance.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/distgit.py` & `packitos-0.95.0/packit/distgit.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/exceptions.py` & `packitos-0.95.0/packit/exceptions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/local_project.py` & `packitos-0.95.0/packit/local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/patches.py` & `packitos-0.95.0/packit/patches.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/pkgtool.py` & `packitos-0.95.0/packit/pkgtool.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/schema.py` & `packitos-0.95.0/packit/schema.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/security.py` & `packitos-0.95.0/packit/security.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/source_git.py` & `packitos-0.95.0/packit/source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/status.py` & `packitos-0.95.0/packit/status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/sync.py` & `packitos-0.95.0/packit/sync.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/upstream.py` & `packitos-0.95.0/packit/upstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/vm_image_build.py` & `packitos-0.95.0/packit/vm_image_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/build.py` & `packitos-0.95.0/packit/cli/build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/create_update.py` & `packitos-0.95.0/packit/cli/create_update.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/dist_git_init.py` & `packitos-0.95.0/packit/cli/dist_git_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import click
 import yaml
 from yaml import safe_load
 
 from packit.api import PackitAPI
 from packit.cli.types import LocalProjectParameter
 from packit.cli.utils import cover_packit_exception, get_existing_config
-from packit.config import PackageConfig, get_context_settings
+from packit.config import PackageConfig
 from packit.config.config import Config, pass_config
 from packit.distgit import DistGit
 from packit.exceptions import PackitException
 
 logger = logging.getLogger(__name__)
 
 ONBOARD_BRANCH_NAME = "packit-config"
@@ -35,15 +35,15 @@
 PR_DESCRIPTION = """
 For more details, see https://packit.dev/docs/configuration/ or contact
 [the Packit team](https://packit.dev#contacts).
 
 """
 
 
-@click.command("init", context_settings=get_context_settings())
+@click.command("init", context_settings={"ignore_unknown_options": True})
 @click.option(
     "--upstream-git-url",
     help="URL to the upstream GIT repository",
     required=True,
 )
 @click.option(
     "--upstream-tag-template",
@@ -54,14 +54,18 @@
     help="Python regex used for filtering upstream tags to include. ",
 )
 @click.option(
     "--upstream-tag-exclude",
     help="Python regex used for filtering upstream tags to exclude. ",
 )
 @click.option(
+    "--version-update-mask",
+    help="Python regex used for comparison of the old and the new version. ",
+)
+@click.option(
     "--issue-repository",
     help="URL of a git repository that can be used for reporting errors in form of issues. ",
 )
 @click.option(
     "--no-pull",
     default=False,
     is_flag=True,
@@ -125,41 +129,44 @@
     "Otherwise clone the repo in a temporary directory.",
 )
 @click.option(
     "--commit-msg",
     help="Commit message used when creating a PR (also for the title) or pushing to dist-git. "
     f"Default: {COMMIT_MESSAGE!r}",
 )
+@click.argument("other_args", nargs=-1, type=click.UNPROCESSED)
 @click.argument(
     "path_or_url",
     type=LocalProjectParameter(),
     default=os.path.curdir,
 )
 @pass_config
 @cover_packit_exception
 def init(
     config,
     upstream_git_url,
     upstream_tag_template,
     upstream_tag_include,
     upstream_tag_exclude,
+    version_update_mask,
     issue_repository,
     no_pull,
     no_koji_build,
     allowed_committers,
     allowed_pr_authors,
     no_bodhi_update,
     actions_file,
     dist_git_branches,
     push_to_distgit,
     create_pr,
     force,
     clone_path,
     commit_msg,
     path_or_url,
+    other_args,
 ):
     """
     Create the initial Packit dist-git configuration for Fedora release syncing based on
     the input parameters.
 
     This command adds `.packit.yaml` file to the dist-git repository either:
 
@@ -190,38 +197,50 @@
 
     Local generation for dist-git repo specified by URL that will be cloned to `<my-package>` dir:
 
     \b
         $ packit dist-git init --upstream-git-url https://github.com/packit/packit --clone-path
         `<my-package>` https://src.fedoraproject.org/rpms/packit
 
+    Using arbitrary configuration options that are not provided as the command options
+    (the working dir needs to be specified in this case):
+
+    \b
+        $ packit dist-git init --upstream-git-url https://github.com/packit/packit
+        --my-option option-value .
+
     """
+    kwargs = {
+        other_args[i][2:]: other_args[i + 1] for i in range(0, len(other_args), 2)
+    }
     if no_pull and no_koji_build:
         logger.warning("At least one job needs to be defined!")
         return
 
     DistGitInitializer(
         upstream_git_url=upstream_git_url,
         upstream_tag_template=upstream_tag_template,
         upstream_tag_include=upstream_tag_include,
         upstream_tag_exclude=upstream_tag_exclude,
+        version_update_mask=version_update_mask,
         issue_repository=issue_repository,
         no_pull=no_pull,
         no_koji_build=no_koji_build,
         no_bodhi_update=no_bodhi_update,
         allowed_committers=allowed_committers,
         allowed_pr_authors=allowed_pr_authors,
         actions_file=actions_file,
         dist_git_branches=dist_git_branches,
         create_pr=create_pr,
         push_to_distgit=push_to_distgit,
         force=force,
         config=config,
         path_or_url=path_or_url,
         commit_msg=commit_msg,
+        kwargs=kwargs,
     ).initialize_dist_git()
 
 
 class PackitDumper(yaml.SafeDumper):
     # to not create yaml anchors when dumping
     # https://github.com/yaml/pyyaml/issues/535#issuecomment-1293636712
     def ignore_aliases(self, data):
@@ -238,32 +257,35 @@
         self,
         config: Config,
         path_or_url: LocalProjectParameter,
         upstream_git_url: str,
         upstream_tag_template: Optional[str] = None,
         upstream_tag_include: Optional[str] = None,
         upstream_tag_exclude: Optional[str] = None,
+        version_update_mask: Optional[str] = None,
         issue_repository: Optional[str] = None,
         no_pull: bool = False,
         no_koji_build: bool = False,
         allowed_committers: Optional[str] = None,
         allowed_pr_authors: Optional[str] = None,
         no_bodhi_update: bool = False,
         actions_file: Optional[Path] = None,
         dist_git_branches: Optional[str] = None,
         push_to_distgit: bool = False,
         create_pr: bool = False,
         force: bool = False,
         commit_msg: Optional[str] = None,
+        kwargs: Optional[dict] = None,
     ):
         self.config = config
         self.upstream_git_url = upstream_git_url
         self.upstream_tag_template = upstream_tag_template
         self.upstream_tag_include = upstream_tag_include
         self.upstream_tag_exclude = upstream_tag_exclude
+        self.version_update_mask = version_update_mask
         self.issue_repository = issue_repository
         self.no_pull = no_pull
         self.no_koji_build = no_koji_build
         self.allowed_committers = (
             allowed_committers.split(",") if allowed_committers else None
         )
         self.allowed_pr_authors = (
@@ -275,14 +297,15 @@
             dist_git_branches.split(",") if dist_git_branches else ["fedora-rawhide"]
         )
         self.push_to_distgit = push_to_distgit
         self.create_pr = create_pr
         self.path_or_url = path_or_url
         self.force = force
         self.commit_msg = commit_msg or COMMIT_MESSAGE
+        self.kwargs = kwargs or {}
 
     @property
     def working_dir(self):
         return self.path_or_url.working_dir
 
     @property
     def config_path(self):
@@ -351,25 +374,28 @@
         # TODO maybe take the URL from spec-file and check if it is a git URL?
         config: dict[str, Any] = {"upstream_project_url": self.upstream_git_url}
 
         optional_config_keys = [
             "upstream_tag_template",
             "upstream_tag_include",
             "upstream_tag_exclude",
+            "version_update_mask",
             "issue_repository",
             "allowed_committers",
             "allowed_pr_authors",
             "actions",
         ]
 
         for key in optional_config_keys:
             value = getattr(self, key, None)
             if value:
                 config[key] = value
 
+        config.update(self.kwargs)
+
         config["jobs"] = []
         if not self.no_pull:
             config["jobs"].append(
                 {
                     "job": "pull_from_upstream",
                     "trigger": "release",
                     "dist_git_branches": self.dist_git_branches,
```

### Comparing `packitos-0.94.2/packit/cli/init.py` & `packitos-0.95.0/packit/cli/init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/packit_base.py` & `packitos-0.95.0/packit/cli/packit_base.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/prepare_sources.py` & `packitos-0.95.0/packit/cli/prepare_sources.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/propose_downstream.py` & `packitos-0.95.0/packit/cli/propose_downstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/push_updates.py` & `packitos-0.95.0/packit/cli/push_updates.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/source_git.py` & `packitos-0.95.0/packit/cli/source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/source_git_init.py` & `packitos-0.95.0/packit/cli/source_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/source_git_status.py` & `packitos-0.95.0/packit/cli/source_git_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/srpm.py` & `packitos-0.95.0/packit/cli/srpm.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/status.py` & `packitos-0.95.0/packit/cli/status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/sync_from_downstream.py` & `packitos-0.95.0/packit/cli/sync_from_downstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/types.py` & `packitos-0.95.0/packit/cli/types.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/update_dist_git.py` & `packitos-0.95.0/packit/cli/update_dist_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/update_source_git.py` & `packitos-0.95.0/packit/cli/update_source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/utils.py` & `packitos-0.95.0/packit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/validate_config.py` & `packitos-0.95.0/packit/cli/validate_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/builds/copr_build.py` & `packitos-0.95.0/packit/cli/builds/copr_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/builds/in_image_builder.py` & `packitos-0.95.0/packit/cli/builds/in_image_builder.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/builds/koji_build.py` & `packitos-0.95.0/packit/cli/builds/koji_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/builds/local_build.py` & `packitos-0.95.0/packit/cli/builds/local_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/cli/builds/mock_build.py` & `packitos-0.95.0/packit/cli/builds/mock_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/config/__init__.py` & `packitos-0.95.0/packit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/config/aliases.py` & `packitos-0.95.0/packit/config/aliases.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/config/common_package_config.py` & `packitos-0.95.0/packit/config/common_package_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/config/config.py` & `packitos-0.95.0/packit/config/config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/config/job_config.py` & `packitos-0.95.0/packit/config/job_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/config/notifications.py` & `packitos-0.95.0/packit/config/notifications.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/config/package_config.py` & `packitos-0.95.0/packit/config/package_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     def __init__(
         self,
         packages: dict[str, CommonPackageConfig],
         jobs: Optional[list[JobConfig]] = None,
     ):
         self._job_views: list[Union[JobConfig, JobConfigView]] = []
         self._package_config_views: dict[str, "PackageConfigView"] = {}
+        self._raw_dict_with_defaults: Optional[dict] = None
         super().__init__(packages)
         # Directly manipulating __dict__ is not recommended.
         # It is done here to avoid triggering __setattr__ and
         # should be removed once support for a single package is
         # dropped from config objects.
         self.__dict__["jobs"] = jobs or []
 
@@ -88,15 +89,14 @@
         raw_dict: dict,
         config_file_path: Optional[str] = None,
         repo_name: Optional[str] = None,
         search_specfile: Optional[Callable[..., Optional[str]]] = None,
         **specfile_search_args,
     ) -> "PackageConfig":
         # required to avoid cyclical imports
-        from packit.schema import PackageConfigSchema
 
         # we need to process defaults first so they get propagated to JobConfigs
         raw_dict.setdefault("config_file_path", config_file_path)
 
         if packages := raw_dict.get("packages", None):
             for package in packages.values():
                 up_url_key = "upstream_project_url"
@@ -113,17 +113,31 @@
             cls.set_defaults(
                 raw_dict,
                 repo_name,
                 search_specfile,
                 **specfile_search_args,
             )
 
+        return cls.get_from_dict_without_setting_defaults(raw_dict)
+
+    @classmethod
+    def get_from_dict_without_setting_defaults(
+        cls,
+        raw_dict: dict,
+    ) -> "PackageConfig":
+        # required to avoid cyclical imports
+        from packit.schema import PackageConfigSchema
+
         package_config = PackageConfigSchema().load(raw_dict)
+        package_config._raw_dict_with_defaults = raw_dict
         return cls.post_load(package_config)
 
+    def get_raw_dict_with_defaults(self):
+        return self._raw_dict_with_defaults
+
     @classmethod
     def post_load(cls, package_config: "PackageConfig") -> "PackageConfig":
         if not package_config:
             return None
 
         package_config_views: dict[str, "PackageConfigView"] = {}
         for name, package in package_config.packages.items():
```

### Comparing `packitos-0.94.2/packit/config/package_config_validator.py` & `packitos-0.95.0/packit/config/package_config_validator.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/config/requirements.py` & `packitos-0.95.0/packit/config/requirements.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/data/_packitpatch` & `packitos-0.95.0/packit/data/_packitpatch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/__init__.py` & `packitos-0.95.0/packit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/bodhi.py` & `packitos-0.95.0/packit/utils/bodhi.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/changelog_helper.py` & `packitos-0.95.0/packit/utils/changelog_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/commands.py` & `packitos-0.95.0/packit/utils/commands.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/decorators.py` & `packitos-0.95.0/packit/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/extensions.py` & `packitos-0.95.0/packit/utils/extensions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/koji_helper.py` & `packitos-0.95.0/packit/utils/koji_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/logging.py` & `packitos-0.95.0/packit/utils/logging.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/lookaside.py` & `packitos-0.95.0/packit/utils/lookaside.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/monitoring.py` & `packitos-0.95.0/packit/utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/repo.py` & `packitos-0.95.0/packit/utils/repo.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/source_script.py` & `packitos-0.95.0/packit/utils/source_script.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/upstream_version.py` & `packitos-0.95.0/packit/utils/upstream_version.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/packit/utils/versions.py` & `packitos-0.95.0/packit/utils/versions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/plans/full.fmf` & `packitos-0.95.0/plans/full.fmf`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/plans/session-recording.fmf` & `packitos-0.95.0/plans/session-recording.fmf`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/conftest.py` & `packitos-0.95.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/full.fmf` & `packitos-0.95.0/tests/full.fmf`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/spellbook.py` & `packitos-0.95.0/tests/spellbook.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/cockpit-ostree/Makefile` & `packitos-0.95.0/tests/data/cockpit-ostree/Makefile`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/cockpit-ostree/cockpit-ostree.spec.dg` & `packitos-0.95.0/tests/data/cockpit-ostree/cockpit-ostree.spec.dg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/cockpit-ostree/cockpit-ostree.spec.in` & `packitos-0.95.0/tests/data/cockpit-ostree/cockpit-ostree.spec.in`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch` & `packitos-0.95.0/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/cronie/SOURCES/fix-memory-leaks.patch` & `packitos-0.95.0/tests/data/cronie/SOURCES/fix-memory-leaks.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/cronie/SOURCES/fix-unsafe-code.patch` & `packitos-0.95.0/tests/data/cronie/SOURCES/fix-unsafe-code.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/cronie/SPECS/cronie.spec` & `packitos-0.95.0/tests/data/cronie/SPECS/cronie.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/dg-ogr/.packit.yaml` & `packitos-0.95.0/tests/data/dg-ogr/.packit.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/dg-ogr/python-ogr.spec` & `packitos-0.95.0/tests/data/dg-ogr/python-ogr.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/edd/Makefile` & `packitos-0.95.0/tests/data/edd/Makefile`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/edd/edd.spec` & `packitos-0.95.0/tests/data/edd/edd.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/osbuild/osbuild.spec` & `packitos-0.95.0/tests/data/osbuild/osbuild.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/patches/previous/git-diff.patch` & `packitos-0.95.0/tests/data/patches/previous/git-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/patches/previous/missing-diff-line.patch` & `packitos-0.95.0/tests/data/patches/previous/missing-diff-line.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/patches/previous/unified-diff.patch` & `packitos-0.95.0/tests/data/patches/previous/unified-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/patches/previous/weird-identical.patch` & `packitos-0.95.0/tests/data/patches/previous/weird-identical.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/patches/regenerated/git-diff.patch` & `packitos-0.95.0/tests/data/patches/regenerated/git-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/patches/regenerated/missing-diff-line.patch` & `packitos-0.95.0/tests/data/patches/regenerated/missing-diff-line.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/patches/regenerated/unified-diff.patch` & `packitos-0.95.0/tests/data/patches/regenerated/unified-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/patches/regenerated/weird-identical.patch` & `packitos-0.95.0/tests/data/patches/regenerated/weird-identical.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/rpms/hello/0017-Patch-This..patch` & `packitos-0.95.0/tests/data/rpms/hello/0017-Patch-This..patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/rpms/hello/from-git.patch` & `packitos-0.95.0/tests/data/rpms/hello/from-git.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/snapd/packaging/fedora/fix-spec` & `packitos-0.95.0/tests/data/snapd/packaging/fedora/fix-spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/snapd/packaging/fedora/pack-source` & `packitos-0.95.0/tests/data/snapd/packaging/fedora/pack-source`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/snapd/packaging/fedora/snapd.spec` & `packitos-0.95.0/tests/data/snapd/packaging/fedora/snapd.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/snapd/vendor/vendor.json` & `packitos-0.95.0/tests/data/snapd/vendor/vendor.json`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/sourcegit/source_git/.distro/beer.spec` & `packitos-0.95.0/tests/data/sourcegit/source_git/.distro/beer.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/upstream_git/beer.spec` & `packitos-0.95.0/tests/data/upstream_git/beer.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/upstream_git_macro_in_source/beer.spec` & `packitos-0.95.0/tests/data/upstream_git_macro_in_source/beer.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.spec` & `packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/functional/spellbook.py` & `packitos-0.95.0/tests/functional/spellbook.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/functional/test_local_build.py` & `packitos-0.95.0/tests/functional/test_local_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/functional/test_prepare_sources.py` & `packitos-0.95.0/tests/functional/test_prepare_sources.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/functional/test_srpm.py` & `packitos-0.95.0/tests/functional/test_srpm.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/bodhi_latest_builds.py` & `packitos-0.95.0/tests/integration/bodhi_latest_builds.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/bodhi_status_updates.py` & `packitos-0.95.0/tests/integration/bodhi_status_updates.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/conftest.py` & `packitos-0.95.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_actions.py` & `packitos-0.95.0/tests/integration/test_actions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_api.py` & `packitos-0.95.0/tests/integration/test_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_base_git.py` & `packitos-0.95.0/tests/integration/test_base_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_build.py` & `packitos-0.95.0/tests/integration/test_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_changelog_helper.py` & `packitos-0.95.0/tests/integration/test_changelog_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_copr_build.py` & `packitos-0.95.0/tests/integration/test_copr_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_create_update.py` & `packitos-0.95.0/tests/integration/test_create_update.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_get_api.py` & `packitos-0.95.0/tests/integration/test_get_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_init.py` & `packitos-0.95.0/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_local_project.py` & `packitos-0.95.0/tests/integration/test_local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_pagure.py` & `packitos-0.95.0/tests/integration/test_pagure.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_patches.py` & `packitos-0.95.0/tests/integration/test_patches.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_push_updates.py` & `packitos-0.95.0/tests/integration/test_push_updates.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_security.py` & `packitos-0.95.0/tests/integration/test_security.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_source_git.py` & `packitos-0.95.0/tests/integration/test_source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_source_git_init.py` & `packitos-0.95.0/tests/integration/test_source_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_source_git_status.py` & `packitos-0.95.0/tests/integration/test_source_git_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_source_git_synch_push.py` & `packitos-0.95.0/tests/integration/test_source_git_synch_push.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_source_git_update_source_git.py` & `packitos-0.95.0/tests/integration/test_source_git_update_source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_spec.py` & `packitos-0.95.0/tests/integration/test_spec.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_update.py` & `packitos-0.95.0/tests/integration/test_update.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_upstream.py` & `packitos-0.95.0/tests/integration/test_upstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_using_cockpit.py` & `packitos-0.95.0/tests/integration/test_using_cockpit.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_using_examples.py` & `packitos-0.95.0/tests/integration/test_using_examples.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_validate_config.py` & `packitos-0.95.0/tests/integration/test_validate_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/integration/test_validate_synced_files.py` & `packitos-0.95.0/tests/integration/test_validate_synced_files.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/conftest.py` & `packitos-0.95.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_actions.py` & `packitos-0.95.0/tests/unit/test_actions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_api.py` & `packitos-0.95.0/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_base_git.py` & `packitos-0.95.0/tests/unit/test_base_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_cli.py` & `packitos-0.95.0/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_cli_utils.py` & `packitos-0.95.0/tests/unit/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_copr_helper.py` & `packitos-0.95.0/tests/unit/test_copr_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_dg.py` & `packitos-0.95.0/tests/unit/test_dg.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_dist_git_init.py` & `packitos-0.95.0/tests/unit/test_dist_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_image_builder.py` & `packitos-0.95.0/tests/unit/test_image_builder.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_iterate_packages.py` & `packitos-0.95.0/tests/unit/test_iterate_packages.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_koji_build.py` & `packitos-0.95.0/tests/unit/test_koji_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_load_authentication.py` & `packitos-0.95.0/tests/unit/test_load_authentication.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_local_project.py` & `packitos-0.95.0/tests/unit/test_local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_login_with_kerberos.py` & `packitos-0.95.0/tests/unit/test_login_with_kerberos.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_patches.py` & `packitos-0.95.0/tests/unit/test_patches.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_prepare_sources.py` & `packitos-0.95.0/tests/unit/test_prepare_sources.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_propose_downstream.py` & `packitos-0.95.0/tests/unit/test_propose_downstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_security.py` & `packitos-0.95.0/tests/unit/test_security.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_specfile.py` & `packitos-0.95.0/tests/unit/test_specfile.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_status.py` & `packitos-0.95.0/tests/unit/test_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_sync.py` & `packitos-0.95.0/tests/unit/test_sync.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_upstream.py` & `packitos-0.95.0/tests/unit/test_upstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/test_utils.py` & `packitos-0.95.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/config/test_config.py` & `packitos-0.95.0/tests/unit/config/test_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/config/test_config_aliases.py` & `packitos-0.95.0/tests/unit/config/test_config_aliases.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/config/test_package_config.py` & `packitos-0.95.0/tests/unit/config/test_package_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1829,14 +1829,30 @@
         },
         repo_name="package",
     )
     assert not pc.test_command.default_labels
     assert pc.test_command.default_identifier == identifier
 
 
+def test_get_raw_dict_with_defaults():
+    pc = PackageConfig.get_from_dict(
+        {
+            "specfile_path": "package.spec",
+        },
+        repo_name="package",
+        config_file_path="path",
+    )
+    assert pc.get_raw_dict_with_defaults() == {
+        "specfile_path": "package.spec",
+        "config_file_path": "path",
+        "upstream_package_name": "package",
+        "downstream_package_name": "package",
+    }
+
+
 def test_get_local_specfile_path():
     assert str(get_local_specfile_path(UP_OSBUILD)) == "osbuild.spec"
     assert not get_local_specfile_path(SYNC_FILES)
 
 
 @pytest.mark.parametrize(
     "directory, local_first,local_last,config_file_name,res_pc_path",
```

### Comparing `packitos-0.94.2/tests/unit/utils/test_changelog_helper.py` & `packitos-0.95.0/tests/unit/utils/test_changelog_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/utils/test_decorators.py` & `packitos-0.95.0/tests/unit/utils/test_decorators.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/utils/test_dist_git_instance.py` & `packitos-0.95.0/tests/unit/utils/test_dist_git_instance.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/utils/test_koji_helper.py` & `packitos-0.95.0/tests/unit/utils/test_koji_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/utils/test_lookaside.py` & `packitos-0.95.0/tests/unit/utils/test_lookaside.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/utils/test_repo.py` & `packitos-0.95.0/tests/unit/utils/test_repo.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/utils/test_source_script.py` & `packitos-0.95.0/tests/unit/utils/test_source_script.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/utils/test_upstream_version.py` & `packitos-0.95.0/tests/unit/utils/test_upstream_version.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests/unit/utils/test_versions.py` & `packitos-0.95.0/tests/unit/utils/test_versions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/README.md` & `packitos-0.95.0/tests_recording/README.md`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_api.py` & `packitos-0.95.0/tests_recording/test_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_base_git.py` & `packitos-0.95.0/tests_recording/test_base_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_image_builder.py` & `packitos-0.95.0/tests_recording/test_image_builder.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_local_project.py` & `packitos-0.95.0/tests_recording/test_local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_repository_cache.py` & `packitos-0.95.0/tests_recording/test_repository_cache.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_status.py` & `packitos-0.95.0/tests_recording/test_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/testbase.py` & `packitos-0.95.0/tests_recording/testbase.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml` & `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz` & `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz` & `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml` & `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz` & `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml` & `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz` & `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml` & `packitos-0.95.0/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml` & `packitos-0.95.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml` & `packitos-0.95.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml` & `packitos-0.95.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml` & `packitos-0.95.0/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml` & `packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml` & `packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml` & `packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml` & `packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml` & `packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml` & `packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml` & `packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_status.yaml` & `packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_status.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml` & `packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/LICENSE` & `packitos-0.95.0/LICENSE`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/README.md` & `packitos-0.95.0/README.md`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/pyproject.toml` & `packitos-0.95.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.2/PKG-INFO` & `packitos-0.95.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: packitos
-Version: 0.94.2
+Version: 0.95.0
 Summary: A set of tools to integrate upstream open source projects into Fedora operating system.
 Project-URL: Homepage, https://github.com/packit/packit
 Author-email: Red Hat <user-cont-team@redhat.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: dist-git,fedora,git,packaging,rpm
 Classifier: Development Status :: 4 - Beta
@@ -39,16 +39,23 @@
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: requests-kerberos
 Requires-Dist: rpkg
 Requires-Dist: specfile
 Requires-Dist: tabulate
 Provides-Extra: dev
-Requires-Dist: packitos[testing]; extra == 'dev'
+Requires-Dist: deepdiff; extra == 'dev'
+Requires-Dist: distro; extra == 'dev'
+Requires-Dist: flexmock; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: pytest-timeout; extra == 'dev'
+Requires-Dist: setuptools; extra == 'dev'
+Requires-Dist: setuptools-scm; extra == 'dev'
 Provides-Extra: testing
 Requires-Dist: deepdiff; extra == 'testing'
 Requires-Dist: distro; extra == 'testing'
 Requires-Dist: flexmock; extra == 'testing'
 Requires-Dist: pytest; extra == 'testing'
 Requires-Dist: pytest-cov; extra == 'testing'
 Requires-Dist: pytest-timeout; extra == 'testing'
```

