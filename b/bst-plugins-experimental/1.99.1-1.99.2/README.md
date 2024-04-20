# Comparing `tmp/bst_plugins_experimental-1.99.1.tar.gz` & `tmp/bst_plugins_experimental-1.99.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bst_plugins_experimental-1.99.1.tar", last modified: Thu Apr 18 16:23:50 2024, max compression
+gzip compressed data, was "bst_plugins_experimental-1.99.2.tar", last modified: Fri Apr 19 15:38:44 2024, max compression
```

## Comparing `bst_plugins_experimental-1.99.1.tar` & `bst_plugins_experimental-1.99.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.897105 bst_plugins_experimental-1.99.1/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    26471 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/LICENSE
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       66 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/MANIFEST.in
--rw-r--r--   0 testuser  (1000) testuser  (1000)     3301 2024-04-18 16:23:50.897105 bst_plugins_experimental-1.99.1/PKG-INFO
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2705 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/README.rst
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      773 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/project.conf
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2731 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/pyproject.toml
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.883105 bst_plugins_experimental-1.99.1/requirements/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      213 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/requirements/plugin-requirements.txt
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      166 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/requirements/test-requirements.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)       38 2024-04-18 16:23:50.897105 bst_plugins_experimental-1.99.1/setup.cfg
--rwxrwxrwx   0 testuser  (1000) testuser  (1000)       61 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/setup.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.880105 bst_plugins_experimental-1.99.1/src/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.883105 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/__init__.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.891105 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/__init__.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2574 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazel_build.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1082 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazel_build.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    11344 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazelize.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazelize.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2149 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/check_forbidden.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3925 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/collect_integration.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    10872 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/collect_manifest.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8503 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_build.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1536 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_build.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    10286 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_deploy.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      912 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_deploy.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2752 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_bootimg.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1354 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3023 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_ext4.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1045 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_ext4.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     7669 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_image.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       36 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_image.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4757 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_repo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1432 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_repo.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1634 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/makemaker.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1079 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/makemaker.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1650 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/modulebuild.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1084 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/modulebuild.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35832 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/oci.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      985 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/pyproject.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      339 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/pyproject.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1570 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/qmake.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      894 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/qmake.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2895 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/snap_image.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/snap_image.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3979 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/tar_element.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      286 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/tar_element.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3021 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/x86image.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4551 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/x86image.yaml
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.894105 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/__init__.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    15455 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/_git_utils.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     6386 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/_utils.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    13073 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/bazel_source.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4025 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/cpan.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8759 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/deb.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1685 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/git_module.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3672 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/git_repo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35633 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/git_tag.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     5113 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/go_module.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     9055 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/ostree.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2662 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/patch_queue.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     5888 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/pypi.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2672 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/quilt.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     6947 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/zip.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.894105 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      375 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/__init__.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.895105 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      106 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/__init__.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3831 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/gitrepo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1883 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/ostreerepo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      743 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/tarrepo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      946 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/ziprepo.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.896105 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/
--rw-r--r--   0 testuser  (1000) testuser  (1000)     3301 2024-04-18 16:23:50.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/PKG-INFO
--rw-r--r--   0 testuser  (1000) testuser  (1000)     3476 2024-04-18 16:23:50.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/SOURCES.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)        1 2024-04-18 16:23:50.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/dependency_links.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)     1806 2024-04-18 16:23:50.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/entry_points.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)       40 2024-04-18 16:23:50.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/requires.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)       25 2024-04-18 16:23:50.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/top_level.txt
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.881105 bst_plugins_experimental-1.99.1/venv/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.881105 bst_plugins_experimental-1.99.1/venv/lib/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.881105 bst_plugins_experimental-1.99.1/venv/lib/python3.11/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.881105 bst_plugins_experimental-1.99.1/venv/lib/python3.11/site-packages/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.896105 bst_plugins_experimental-1.99.1/venv/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 testuser  (1000) testuser  (1000)     2446 2024-04-18 16:23:47.000000 bst_plugins_experimental-1.99.1/venv/lib/python3.11/site-packages/markdown_it/port.yaml
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.146917 bst_plugins_experimental-1.99.2/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    26471 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/LICENSE
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       66 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/MANIFEST.in
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     3301 2024-04-19 15:38:44.146917 bst_plugins_experimental-1.99.2/PKG-INFO
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2705 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/README.rst
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      773 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/project.conf
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2731 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/pyproject.toml
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.132918 bst_plugins_experimental-1.99.2/requirements/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      213 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/requirements/plugin-requirements.txt
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      166 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/requirements/test-requirements.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)       38 2024-04-19 15:38:44.146917 bst_plugins_experimental-1.99.2/setup.cfg
+-rwxrwxrwx   0 testuser  (1000) testuser  (1000)       61 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/setup.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.129917 bst_plugins_experimental-1.99.2/src/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.132918 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/__init__.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.140918 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/__init__.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2574 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/bazel_build.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1082 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/bazel_build.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    11344 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/bazelize.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/bazelize.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2149 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/check_forbidden.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3925 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/collect_integration.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    10872 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/collect_manifest.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8503 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/dpkg_build.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1536 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/dpkg_build.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    10286 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/dpkg_deploy.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      912 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/dpkg_deploy.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2752 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/fastboot_bootimg.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1354 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3023 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/fastboot_ext4.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1045 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/fastboot_ext4.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     7669 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/flatpak_image.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       36 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/flatpak_image.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4757 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/flatpak_repo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1432 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/flatpak_repo.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1634 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/makemaker.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1079 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/makemaker.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1650 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/modulebuild.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1084 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/modulebuild.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35832 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/oci.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      985 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/pyproject.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      339 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/pyproject.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1570 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/qmake.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      894 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/qmake.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2895 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/snap_image.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/snap_image.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3979 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/tar_element.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      286 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/tar_element.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3021 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/x86image.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4551 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/x86image.yaml
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.143917 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/__init__.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    15455 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/_git_utils.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     6386 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/_utils.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    13073 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/bazel_source.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4025 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/cpan.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8759 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/deb.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1685 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/git_module.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3672 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/git_repo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35633 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/git_tag.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     5127 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/go_module.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     9055 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/ostree.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2662 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/patch_queue.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     5888 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/pypi.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2672 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/quilt.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     6947 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/zip.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.143917 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/testutils/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      375 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/testutils/__init__.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.144918 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/testutils/repo/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      106 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/testutils/repo/__init__.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3831 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/testutils/repo/gitrepo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1883 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/testutils/repo/ostreerepo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      743 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/testutils/repo/tarrepo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      946 2024-04-19 15:38:30.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/testutils/repo/ziprepo.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.145918 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental.egg-info/
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     3301 2024-04-19 15:38:44.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental.egg-info/PKG-INFO
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     3476 2024-04-19 15:38:44.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental.egg-info/SOURCES.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)        1 2024-04-19 15:38:44.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental.egg-info/dependency_links.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     1806 2024-04-19 15:38:44.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental.egg-info/entry_points.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)       40 2024-04-19 15:38:44.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental.egg-info/requires.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)       25 2024-04-19 15:38:44.000000 bst_plugins_experimental-1.99.2/src/bst_plugins_experimental.egg-info/top_level.txt
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.130918 bst_plugins_experimental-1.99.2/venv/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.130918 bst_plugins_experimental-1.99.2/venv/lib/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.130918 bst_plugins_experimental-1.99.2/venv/lib/python3.11/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.130918 bst_plugins_experimental-1.99.2/venv/lib/python3.11/site-packages/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-19 15:38:44.145918 bst_plugins_experimental-1.99.2/venv/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     2446 2024-04-19 15:38:40.000000 bst_plugins_experimental-1.99.2/venv/lib/python3.11/site-packages/markdown_it/port.yaml
```

### Comparing `bst_plugins_experimental-1.99.1/LICENSE` & `bst_plugins_experimental-1.99.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/PKG-INFO` & `bst_plugins_experimental-1.99.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bst-plugins-experimental
-Version: 1.99.1
+Version: 1.99.2
 Summary: A collection of experimental BuildStream plugins.
 License: LGPL-2.1-or-later
 Project-URL: documentation, https://buildstream.gitlab.io/bst-plugins-experimental/
 Project-URL: repository, https://gitlab.com/BuildStream/bst-plugins-experimental
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `bst_plugins_experimental-1.99.1/README.rst` & `bst_plugins_experimental-1.99.2/README.rst`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/project.conf` & `bst_plugins_experimental-1.99.2/project.conf`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/pyproject.toml` & `bst_plugins_experimental-1.99.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazel_build.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/bazel_build.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazel_build.yaml` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/bazel_build.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazelize.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/bazelize.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/check_forbidden.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/check_forbidden.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/collect_integration.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/collect_integration.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/collect_manifest.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/collect_manifest.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_build.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/dpkg_build.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_build.yaml` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/dpkg_build.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_deploy.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/dpkg_deploy.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_deploy.yaml` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/dpkg_deploy.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_bootimg.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/fastboot_bootimg.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_ext4.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/fastboot_ext4.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_ext4.yaml` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/fastboot_ext4.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_image.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/flatpak_image.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_repo.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/flatpak_repo.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_repo.yaml` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/flatpak_repo.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/makemaker.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/makemaker.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/makemaker.yaml` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/makemaker.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/modulebuild.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/modulebuild.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/modulebuild.yaml` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/modulebuild.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/oci.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/oci.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/pyproject.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/pyproject.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/qmake.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/qmake.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/qmake.yaml` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/qmake.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/snap_image.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/snap_image.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/tar_element.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/tar_element.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/x86image.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/x86image.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/x86image.yaml` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/elements/x86image.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/_git_utils.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/_git_utils.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/_utils.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/_utils.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/bazel_source.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/bazel_source.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/cpan.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/cpan.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/deb.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/deb.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/git_module.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/git_module.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/git_repo.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/git_repo.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/git_tag.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/git_tag.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/go_module.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/go_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,26 +131,26 @@
         vendor_directory = os.path.join(directory, "vendor", self.module)
         os.makedirs(vendor_directory, exist_ok=True)
         mirror = GitMirror(
             self,
             self.url,
             self.ref["git-ref"],
         )
-        mirror.stage(directory)
+        mirror.stage(vendor_directory)
         self._append_modules_txt(directory)
 
     def init_workspace(self, directory):
         vendor_directory = os.path.join(directory, "vendor", self.module)
         os.makedirs(vendor_directory, exist_ok=True)
         mirror = GitMirror(
             self,
             self.url,
             self.ref["git-ref"],
         )
-        mirror.init_workspace(directory)
+        mirror.init_workspace(vendor_directory)
         self._append_modules_txt(directory)
 
     def _append_modules_txt(self, directory):
         modules_txt = os.path.join(directory, "vendor/modules.txt")
         with open(modules_txt, "a", encoding="utf-8") as file:
             if self.ref["explicit"]:
                 print(f"# {self.module} {self.ref['go-version']}", file=file)
```

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/ostree.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/ostree.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/patch_queue.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/patch_queue.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/pypi.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/pypi.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/quilt.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/quilt.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/zip.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/sources/zip.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/gitrepo.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/testutils/repo/gitrepo.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/ostreerepo.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/testutils/repo/ostreerepo.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/tarrepo.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/testutils/repo/tarrepo.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/ziprepo.py` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental/testutils/repo/ziprepo.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/PKG-INFO` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bst-plugins-experimental
-Version: 1.99.1
+Version: 1.99.2
 Summary: A collection of experimental BuildStream plugins.
 License: LGPL-2.1-or-later
 Project-URL: documentation, https://buildstream.gitlab.io/bst-plugins-experimental/
 Project-URL: repository, https://gitlab.com/BuildStream/bst-plugins-experimental
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/SOURCES.txt` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/entry_points.txt` & `bst_plugins_experimental-1.99.2/src/bst_plugins_experimental.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.1/venv/lib/python3.11/site-packages/markdown_it/port.yaml` & `bst_plugins_experimental-1.99.2/venv/lib/python3.11/site-packages/markdown_it/port.yaml`

 * *Files identical despite different names*

