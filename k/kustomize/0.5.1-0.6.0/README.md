# Comparing `tmp/kustomize-0.5.1.tar.gz` & `tmp/kustomize-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kustomize-0.5.1.tar", last modified: Fri Apr 19 02:47:36 2024, max compression
+gzip compressed data, was "kustomize-0.6.0.tar", last modified: Sat Apr 20 14:14:03 2024, max compression
```

## Comparing `kustomize-0.5.1.tar` & `kustomize-0.6.0.tar`

### file list

```diff
@@ -1,281 +1,297 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.204698 kustomize-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-19 02:47:17.000000 kustomize-0.5.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-19 02:47:17.000000 kustomize-0.5.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.168698 kustomize-0.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 02:47:17.000000 kustomize-0.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.168698 kustomize-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-19 02:47:17.000000 kustomize-0.5.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-19 02:47:17.000000 kustomize-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 02:47:17.000000 kustomize-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 02:47:17.000000 kustomize-0.5.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-19 02:47:17.000000 kustomize-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-19 02:47:17.000000 kustomize-0.5.1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-19 02:47:36.200698 kustomize-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-19 02:47:17.000000 kustomize-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.168698 kustomize-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-19 02:47:17.000000 kustomize-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 02:47:17.000000 kustomize-0.5.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 02:47:17.000000 kustomize-0.5.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.168698 kustomize-0.5.1/kustomize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/kustomize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-19 02:47:17.000000 kustomize-0.5.1/kustomize/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-19 02:47:17.000000 kustomize-0.5.1/kustomize/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/kustomize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-19 02:47:36.000000 kustomize-0.5.1/kustomize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-19 02:47:36.000000 kustomize-0.5.1/kustomize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:47:36.000000 kustomize-0.5.1/kustomize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 02:47:36.000000 kustomize-0.5.1/kustomize.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 02:47:36.000000 kustomize-0.5.1/kustomize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 02:47:36.000000 kustomize-0.5.1/kustomize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 02:47:17.000000 kustomize-0.5.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-19 02:47:17.000000 kustomize-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-19 02:47:17.000000 kustomize-0.5.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 02:47:17.000000 kustomize-0.5.1/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 02:47:36.204698 kustomize-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attributes_as_dict/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/configMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/configMap/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/configMap/configMap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/deployment/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/service/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/service/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attrs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/attrs/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/python/configMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/python/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/python/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/python/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/attrs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/attrs/reference/configMap/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/reference/configMap/configMap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/attrs/reference/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/reference/deployment/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/reference/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/attrs/reference/service/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/reference/service/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/base_and_overlays/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/configMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/production/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/production/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/production/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/production/replica_count.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/staging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/staging/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/staging/special_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.156698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/configMap/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/configMap/configMap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/deployment/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/service/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/service/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.156698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/production/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/production/kustomization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/production/replica_count.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/staging/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/staging/kustomization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/staging/special_labels.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/dataclasses_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/dataclasses_/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/python/configMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/python/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/python/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/python/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/configMap/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/configMap/configMap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/deployment/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/service/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/service/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/python/configMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/python/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/python/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/python/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes/reference/configMap/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/reference/configMap/configMap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes/reference/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/reference/deployment/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/reference/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes/reference/service/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/reference/service/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes11/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes11/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/python/configMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/python/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/python/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/python/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/configMap/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/configMap/configMap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/deployment/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/service/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/service/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/patchesJson6902/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/add_init_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/configMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/add_init_container/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/add_init_container/add_init_container.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/configMap/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/configMap/configMap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/deployment/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/service/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/service/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/python/configMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/python/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/python/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/python/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict/reference/configMap/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/reference/configMap/configMap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict/reference/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/reference/deployment/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/reference/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict/reference/service/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/reference/service/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/configMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/configMap/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/configMap/configMap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/deployment/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/service/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/service/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/configmaps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/configmaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/configmaps/configMap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/deployments/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/kustomization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/services/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/configmaps/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/configmaps/configMap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/deployments/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/services/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/services/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/to_dict/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/to_dict/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/python/configMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/python/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/python/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/python/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/to_dict/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/to_dict/reference/configMap/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/reference/configMap/configMap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/to_dict/reference/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/reference/deployment/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/reference/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/to_dict/reference/service/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/reference/service/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/tuple_multiple/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/tuple_multiple/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/python/configMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/python/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/python/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/python/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/configMap/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/configMap/configMap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/deployment/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/service/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/service/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/configMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/kustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/configMap/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/configMap/configMap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/deployment/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/service/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/service/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 02:47:17.000000 kustomize-0.5.1/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-19 02:47:17.000000 kustomize-0.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.653573 kustomize-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-20 14:13:45.000000 kustomize-0.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-20 14:13:45.000000 kustomize-0.6.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.621573 kustomize-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-20 14:13:45.000000 kustomize-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.621573 kustomize-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-20 14:13:45.000000 kustomize-0.6.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-20 14:13:45.000000 kustomize-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-20 14:13:45.000000 kustomize-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-20 14:13:45.000000 kustomize-0.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-20 14:13:45.000000 kustomize-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-20 14:13:45.000000 kustomize-0.6.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-20 14:14:03.653573 kustomize-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-20 14:13:45.000000 kustomize-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.621573 kustomize-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-20 14:13:45.000000 kustomize-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 14:13:45.000000 kustomize-0.6.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-20 14:13:45.000000 kustomize-0.6.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.621573 kustomize-0.6.0/kustomize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/kustomize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-20 14:13:45.000000 kustomize-0.6.0/kustomize/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-20 14:13:45.000000 kustomize-0.6.0/kustomize/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.653573 kustomize-0.6.0/kustomize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-20 14:14:03.000000 kustomize-0.6.0/kustomize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-04-20 14:14:03.000000 kustomize-0.6.0/kustomize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 14:14:03.000000 kustomize-0.6.0/kustomize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-20 14:14:03.000000 kustomize-0.6.0/kustomize.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-20 14:14:03.000000 kustomize-0.6.0/kustomize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 14:14:03.000000 kustomize-0.6.0/kustomize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-20 14:13:45.000000 kustomize-0.6.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-20 14:13:45.000000 kustomize-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-20 14:13:45.000000 kustomize-0.6.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-20 14:13:45.000000 kustomize-0.6.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 14:14:03.653573 kustomize-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.625573 kustomize-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.625573 kustomize-0.6.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.625573 kustomize-0.6.0/tests/fixtures/attributes_as_dict/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attributes_as_dict/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.625573 kustomize-0.6.0/tests/fixtures/attributes_as_dict/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attributes_as_dict/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attributes_as_dict/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attributes_as_dict/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attributes_as_dict/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attributes_as_dict/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.625573 kustomize-0.6.0/tests/fixtures/attributes_as_dict/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.625573 kustomize-0.6.0/tests/fixtures/attributes_as_dict/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attributes_as_dict/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.625573 kustomize-0.6.0/tests/fixtures/attributes_as_dict/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attributes_as_dict/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attributes_as_dict/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.625573 kustomize-0.6.0/tests/fixtures/attributes_as_dict/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attributes_as_dict/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.625573 kustomize-0.6.0/tests/fixtures/attrs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attrs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/attrs/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attrs/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attrs/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attrs/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attrs/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attrs/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/attrs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/attrs/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attrs/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/attrs/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attrs/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attrs/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/attrs/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/attrs/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/base_and_overlays/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/base/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/base/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/base/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/base/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/overlays/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/overlays/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/overlays/production/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/overlays/production/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/overlays/production/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/overlays/production/replica_count.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/overlays/staging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/overlays/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/overlays/staging/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/python/overlays/staging/special_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.609573 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/base/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/base/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/base/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/base/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/base/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.629573 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/base/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/base/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.609573 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/overlays/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/overlays/production/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/overlays/production/kustomization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/overlays/production/replica_count.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/overlays/staging/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/overlays/staging/kustomization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/overlays/staging/special_labels.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/dataclasses_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/dataclasses_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/dataclasses_/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/dataclasses_/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/dataclasses_/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/dataclasses_/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/dataclasses_/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/dataclasses_/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/dataclasses_/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/dataclasses_/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/dataclasses_/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/dataclasses_/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/dataclasses_/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/dataclasses_/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/dataclasses_/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/dataclasses_/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/kubernetes/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/kubernetes/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/kubernetes/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/kubernetes/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.633573 kustomize-0.6.0/tests/fixtures/kubernetes/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/kubernetes11/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes11/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/kubernetes11/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes11/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes11/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes11/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes11/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes11/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/kubernetes11/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/kubernetes11/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes11/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/kubernetes11/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes11/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes11/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/kubernetes11/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/kubernetes11/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/patchesJson6902/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/patchesJson6902/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/patchesJson6902/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/patchesJson6902/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/patchesJson6902/python/add_init_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/patchesJson6902/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/patchesJson6902/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/patchesJson6902/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/patchesJson6902/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/patchesJson6902/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/patchesJson6902/reference/add_init_container/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/patchesJson6902/reference/add_init_container/add_init_container.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/patchesJson6902/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/patchesJson6902/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/patchesJson6902/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/patchesJson6902/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/patchesJson6902/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/patchesJson6902/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/patchesJson6902/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.637573 kustomize-0.6.0/tests/fixtures/pydantic_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/pydantic_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.641573 kustomize-0.6.0/tests/fixtures/pydantic_v2/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/pydantic_v2/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/pydantic_v2/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/pydantic_v2/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/pydantic_v2/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/pydantic_v2/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.641573 kustomize-0.6.0/tests/fixtures/pydantic_v2/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.641573 kustomize-0.6.0/tests/fixtures/pydantic_v2/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/pydantic_v2/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.641573 kustomize-0.6.0/tests/fixtures/pydantic_v2/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/pydantic_v2/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/pydantic_v2/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.641573 kustomize-0.6.0/tests/fixtures/pydantic_v2/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/pydantic_v2/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.641573 kustomize-0.6.0/tests/fixtures/simple_dict/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.641573 kustomize-0.6.0/tests/fixtures/simple_dict/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.641573 kustomize-0.6.0/tests/fixtures/simple_dict/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.641573 kustomize-0.6.0/tests/fixtures/simple_dict/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.641573 kustomize-0.6.0/tests/fixtures/simple_dict/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.641573 kustomize-0.6.0/tests/fixtures/simple_dict/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.641573 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.641573 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_defaults/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/python/configmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/python/configmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/python/configmaps/configMap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/python/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/python/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/python/deployments/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/python/kustomization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/python/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/python/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/python/services/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/reference/configmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/reference/configmaps/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/reference/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/reference/deployments/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/reference/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/reference/services/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/to_dict/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/to_dict/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/to_dict/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/to_dict/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/to_dict/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/to_dict/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/to_dict/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/to_dict/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.645573 kustomize-0.6.0/tests/fixtures/to_dict/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/to_dict/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/to_dict/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/to_dict/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/to_dict/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/to_dict/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/to_dict/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/to_dict/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/tuple_multiple/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/tuple_multiple/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/tuple_multiple/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/tuple_multiple/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/tuple_multiple/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/tuple_multiple/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:03.649573 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/reference/service/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-20 14:13:45.000000 kustomize-0.6.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 14:13:45.000000 kustomize-0.6.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-20 14:13:45.000000 kustomize-0.6.0/tox.ini
```

### Comparing `kustomize-0.5.1/.github/workflows/main.yml` & `kustomize-0.6.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/.gitignore` & `kustomize-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/LICENSE` & `kustomize-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/NEWS.rst` & `kustomize-0.6.0/NEWS.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,95 @@
+v0.6.0
+======
+
+Features
+--------
+
+- Adding Pydantic v2 support. (#10)
+
+
 v0.5.1
 ======
 
 Bugfixes
 --------
 
 - Refreshed the package metadata. (#1)
 - Require Python 3.8 or later.
 
 
-0.5.0
-=====
+v0.5.0
+======
 
 * Separating generated modules by directories to avoid name clashes.
 
-0.4.1
-=====
+v0.4.1
+======
 
 * Fixing directory creation for dumping built YAML files.
 
-0.4.0
-=====
+v0.4.0
+======
 
 * Now supporting models from python-kubernetes>=11.
 
-0.3.6
-=====
+v0.3.6
+======
 
 * Adding logs.
 
-0.3.5
-=====
+v0.3.5
+======
 
 * Now supporting Kubernetes objects correctly.
 
-0.3.4
-=====
+v0.3.4
+======
 
 * Fixing cleanup of data before dump.
 
-0.3.3
-=====
+v0.3.3
+======
 
 * Cleaning up the data before dumping.
 
-0.3.2
-=====
+v0.3.2
+======
 
 * Preferring to_dict() to dataclasses.asdict().
   This is because objects might need to be more specific about how they
   should convert themselves to a dict.
 
-0.3.1
-=====
+v0.3.1
+======
 
 * Fixing the serialization of objects inside tuples.
 
-0.3.0
-=====
+v0.3.0
+======
 
 * Supporting tuples for multi-section YAML generation.
 
-0.2.0
-=====
+v0.2.0
+======
 
 Supporting other types for generating dictionaries:
 
 * Classes with a ``to_dict`` method
 * Classes from the ``attr`` library
 * "Flat" classes that can be serialized through ``__dict__``
 
-0.1.2
-=====
+v0.1.2
+======
 
 * Supporting patchesJson6902
 
-0.1.1
-=====
+v0.1.1
+======
 
 * Supporting patchesStrategicMerge
 
-0.1.0
-=====
+v0.1.0
+======
 
 * First release!
 * Supporting dictionaries and dataclasses.
```

### Comparing `kustomize-0.5.1/PKG-INFO` & `kustomize-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kustomize
-Version: 0.5.1
+Version: 0.6.0
 Summary: Kustomize for Kubernetes, but in Python
 Author-email: Diogo Baeder <diogobaeder@yahoo.com.br>
 Project-URL: Homepage, https://github.com/coherent-oss/python-kustomize
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,16 @@
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: coverage; extra == "testing"
 Requires-Dist: PyYAML; extra == "testing"
 Requires-Dist: types-PyYAML; extra == "testing"
+Requires-Dist: attrs; extra == "testing"
+Requires-Dist: Pydantic>=2.0; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
 Requires-Dist: PyYAML; extra == "docs"
@@ -48,15 +50,15 @@
 
 .. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 Build your Kubernetes manifests for Kustomize in Python!
 
 * PyPI: https://pypi.org/project/kustomize/
-* Repository: https://github.com/yougov/python-kustomize
+* Repository: https://github.com/coherent-oss/python-kustomize
 * Documentation: https://python-kustomize.readthedocs.io/en/latest/
 
 Overview
 --------
 
 The reason for this project to exist is to make it easier to create dynamic
 manifests to be exported for usage in Kubernetes' "Kustomize" tool. And, by
@@ -83,14 +85,15 @@
 ----------
 
 The only mandatory dependency to this project is ``PyYAML``. This library
 supports a number of object definition types:
 
 * ``dict``
 * ``dataclasses``
+* ``BaseModel`` (from Pydantic)
 * ``attr`` (needs the library installed)
 * ``kubernetes`` (needs the library installed)
 
 This package will be available as ``kustomize``; you may install it with pip,
 for example::
 
     $ pip install kustomize
```

### Comparing `kustomize-0.5.1/README.rst` & `kustomize-0.6.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 .. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 Build your Kubernetes manifests for Kustomize in Python!
 
 * PyPI: https://pypi.org/project/kustomize/
-* Repository: https://github.com/yougov/python-kustomize
+* Repository: https://github.com/coherent-oss/python-kustomize
 * Documentation: https://python-kustomize.readthedocs.io/en/latest/
 
 Overview
 --------
 
 The reason for this project to exist is to make it easier to create dynamic
 manifests to be exported for usage in Kubernetes' "Kustomize" tool. And, by
@@ -51,14 +51,15 @@
 ----------
 
 The only mandatory dependency to this project is ``PyYAML``. This library
 supports a number of object definition types:
 
 * ``dict``
 * ``dataclasses``
+* ``BaseModel`` (from Pydantic)
 * ``attr`` (needs the library installed)
 * ``kubernetes`` (needs the library installed)
 
 This package will be available as ``kustomize``; you may install it with pip,
 for example::
 
     $ pip install kustomize
```

### Comparing `kustomize-0.5.1/docs/conf.py` & `kustomize-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/kustomize/generators.py` & `kustomize-0.6.0/kustomize/generators.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,14 +156,23 @@
         import attr
     except ImportError:  # pragma: no cover
         return False
 
     return attr.has(type(obj))
 
 
+def is_pydantic_model(obj) -> bool:
+    try:
+        from pydantic import BaseModel
+    except ImportError:  # pragma: no cover
+        return False
+
+    return isinstance(obj, BaseModel)
+
+
 def _is_kubernetes(obj):
     return (
         hasattr(obj, 'to_dict')
         and hasattr(obj, 'attribute_map')
         and (
             # python-kubernetes<11
             hasattr(obj, 'swagger_types')
@@ -223,13 +232,16 @@
         logger.debug('Object is dataclass, using it for conversion')
         obj = asdict(obj)
     elif is_attr_class(obj):
         logger.debug('Object is from attr class, using it for conversion')
         import attr
 
         obj = attr.asdict(obj, recurse=True)
+    elif is_pydantic_model(obj):
+        logger.debug('Object is a Pydantic model, using it for conversion')
+        obj = obj.model_dump()
     elif hasattr(obj, '__dict__'):
         obj = obj.__dict__
 
     obj = deepcopy(obj)
 
     return obj
```

### Comparing `kustomize-0.5.1/kustomize/main.py` & `kustomize-0.6.0/kustomize/main.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/kustomize.egg-info/PKG-INFO` & `kustomize-0.6.0/kustomize.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kustomize
-Version: 0.5.1
+Version: 0.6.0
 Summary: Kustomize for Kubernetes, but in Python
 Author-email: Diogo Baeder <diogobaeder@yahoo.com.br>
 Project-URL: Homepage, https://github.com/coherent-oss/python-kustomize
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,16 @@
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: coverage; extra == "testing"
 Requires-Dist: PyYAML; extra == "testing"
 Requires-Dist: types-PyYAML; extra == "testing"
+Requires-Dist: attrs; extra == "testing"
+Requires-Dist: Pydantic>=2.0; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
 Requires-Dist: PyYAML; extra == "docs"
@@ -48,15 +50,15 @@
 
 .. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 Build your Kubernetes manifests for Kustomize in Python!
 
 * PyPI: https://pypi.org/project/kustomize/
-* Repository: https://github.com/yougov/python-kustomize
+* Repository: https://github.com/coherent-oss/python-kustomize
 * Documentation: https://python-kustomize.readthedocs.io/en/latest/
 
 Overview
 --------
 
 The reason for this project to exist is to make it easier to create dynamic
 manifests to be exported for usage in Kubernetes' "Kustomize" tool. And, by
@@ -83,14 +85,15 @@
 ----------
 
 The only mandatory dependency to this project is ``PyYAML``. This library
 supports a number of object definition types:
 
 * ``dict``
 * ``dataclasses``
+* ``BaseModel`` (from Pydantic)
 * ``attr`` (needs the library installed)
 * ``kubernetes`` (needs the library installed)
 
 This package will be available as ``kustomize``; you may install it with pip,
 for example::
 
     $ pip install kustomize
```

### Comparing `kustomize-0.5.1/kustomize.egg-info/SOURCES.txt` & `kustomize-0.6.0/kustomize.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -112,14 +112,24 @@
 tests/fixtures/patchesJson6902/python/kustomization.py
 tests/fixtures/patchesJson6902/python/service.py
 tests/fixtures/patchesJson6902/reference/kustomization.yaml
 tests/fixtures/patchesJson6902/reference/add_init_container/add_init_container.yaml
 tests/fixtures/patchesJson6902/reference/configMap/configMap.yaml
 tests/fixtures/patchesJson6902/reference/deployment/deployment.yaml
 tests/fixtures/patchesJson6902/reference/service/service.yaml
+tests/fixtures/pydantic_v2/__init__.py
+tests/fixtures/pydantic_v2/python/__init__.py
+tests/fixtures/pydantic_v2/python/configMap.py
+tests/fixtures/pydantic_v2/python/deployment.py
+tests/fixtures/pydantic_v2/python/kustomization.py
+tests/fixtures/pydantic_v2/python/service.py
+tests/fixtures/pydantic_v2/reference/kustomization.yaml
+tests/fixtures/pydantic_v2/reference/configMap/configMap.yaml
+tests/fixtures/pydantic_v2/reference/deployment/deployment.yaml
+tests/fixtures/pydantic_v2/reference/service/service.yaml
 tests/fixtures/simple_dict/__init__.py
 tests/fixtures/simple_dict/python/__init__.py
 tests/fixtures/simple_dict/python/configMap.py
 tests/fixtures/simple_dict/python/deployment.py
 tests/fixtures/simple_dict/python/kustomization.py
 tests/fixtures/simple_dict/python/service.py
 tests/fixtures/simple_dict/reference/kustomization.yaml
```

### Comparing `kustomize-0.5.1/pyproject.toml` & `kustomize-0.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 	"pytest-enabler >= 2.2",
 	"pytest-ruff >= 0.2.1",
 
 	# local
 	"coverage",
 	"PyYAML",
 	"types-PyYAML",
+	"attrs",
+	"Pydantic >= 2.0",
 ]
 docs = [
 	# upstream
 	"sphinx >= 3.5",
 	"jaraco.packaging >= 9.3",
 	"rst.linker >= 1.9",
 	"furo",
```

### Comparing `kustomize-0.5.1/pytest.ini` & `kustomize-0.6.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/base.py` & `kustomize-0.6.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/conftest.py` & `kustomize-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/configMap.py` & `kustomize-0.6.0/tests/fixtures/attributes_as_dict/python/configMap.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/deployment.py` & `kustomize-0.6.0/tests/fixtures/attributes_as_dict/python/deployment.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/deployment/deployment.yaml` & `kustomize-0.6.0/tests/fixtures/attributes_as_dict/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/attrs/python/deployment.py` & `kustomize-0.6.0/tests/fixtures/kubernetes/python/deployment.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/attrs/reference/deployment/deployment.yaml` & `kustomize-0.6.0/tests/fixtures/attrs/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/deployment.py` & `kustomize-0.6.0/tests/fixtures/base_and_overlays/python/base/deployment.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/deployment/deployment.yaml` & `kustomize-0.6.0/tests/fixtures/base_and_overlays/reference/base/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/dataclasses_/python/deployment.py` & `kustomize-0.6.0/tests/fixtures/dataclasses_/python/deployment.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/dataclasses_/reference/deployment/deployment.yaml` & `kustomize-0.6.0/tests/fixtures/dataclasses_/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/kubernetes/python/configMap.py` & `kustomize-0.6.0/tests/fixtures/kubernetes/python/configMap.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/kubernetes/python/deployment.py` & `kustomize-0.6.0/tests/fixtures/kubernetes11/python/deployment.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/kubernetes/reference/deployment/deployment.yaml` & `kustomize-0.6.0/tests/fixtures/kubernetes/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/kubernetes11/python/configMap.py` & `kustomize-0.6.0/tests/fixtures/kubernetes11/python/configMap.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/kubernetes11/python/deployment.py` & `kustomize-0.6.0/tests/fixtures/pydantic_v2/python/deployment.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/kubernetes11/reference/deployment/deployment.yaml` & `kustomize-0.6.0/tests/fixtures/kubernetes11/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/patchesJson6902/python/deployment.py` & `kustomize-0.6.0/tests/fixtures/patchesJson6902/python/deployment.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/deployment/deployment.yaml` & `kustomize-0.6.0/tests/fixtures/patchesJson6902/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/simple_dict/python/deployment.py` & `kustomize-0.6.0/tests/fixtures/simple_dict/python/deployment.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/simple_dict/reference/deployment/deployment.yaml` & `kustomize-0.6.0/tests/fixtures/pydantic_v2/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/deployment.py` & `kustomize-0.6.0/tests/fixtures/simple_dict_defaults/python/deployment.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/deployment/deployment.yaml` & `kustomize-0.6.0/tests/fixtures/simple_dict/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/deployments/deployment.py` & `kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/python/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/deployments/deployment.yaml` & `kustomize-0.6.0/tests/fixtures/simple_dict_defaults/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/to_dict/python/configMap.py` & `kustomize-0.6.0/tests/fixtures/to_dict/python/configMap.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/to_dict/python/deployment.py` & `kustomize-0.6.0/tests/fixtures/to_dict/python/deployment.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/to_dict/reference/deployment/deployment.yaml` & `kustomize-0.6.0/tests/fixtures/simple_dict_subdirs/reference/deployments/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/tuple_multiple/python/deployment.py` & `kustomize-0.6.0/tests/fixtures/tuple_multiple/python/deployment.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/deployment/deployment.yaml` & `kustomize-0.6.0/tests/fixtures/to_dict/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/deployment.py` & `kustomize-0.6.0/tests/fixtures/tuple_multiple_attr/python/deployment.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/deployment/deployment.yaml` & `kustomize-0.6.0/tests/fixtures/tuple_multiple/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tests/test_generators.py` & `kustomize-0.6.0/tests/test_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,25 @@
     reference_path = fixtures_path / 'reference'
 
     generate(python_path, build_path)
 
     assert_yaml_dirs_equal(build_path, reference_path)
 
 
+def test_generates_pydantic_v2(cd_fixtures, create_build_path):
+    fixtures_path = cd_fixtures('pydantic_v2')
+    build_path = create_build_path()
+    python_path = fixtures_path / 'python'
+    reference_path = fixtures_path / 'reference'
+
+    generate(python_path, build_path)
+
+    assert_yaml_dirs_equal(build_path, reference_path)
+
+
 def test_generates_tuple_multiple(cd_fixtures, create_build_path):
     fixtures_path = cd_fixtures('tuple_multiple')
     build_path = create_build_path()
     python_path = fixtures_path / 'python'
     reference_path = fixtures_path / 'reference'
 
     generate(python_path, build_path)
```

### Comparing `kustomize-0.5.1/tests/test_main.py` & `kustomize-0.6.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.1/tox.ini` & `kustomize-0.6.0/tox.ini`

 * *Files identical despite different names*

