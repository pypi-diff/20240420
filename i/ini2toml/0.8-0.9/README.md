# Comparing `tmp/ini2toml-0.8.tar.gz` & `tmp/ini2toml-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ini2toml-0.8.tar", last modified: Thu Feb 10 19:48:22 2022, max compression
+gzip compressed data, was "ini2toml-0.9.tar", last modified: Fri Mar  4 11:41:20 2022, max compression
```

## Comparing `ini2toml-0.8.tar` & `ini2toml-0.9.tar`

### file list

```diff
@@ -1,134 +1,138 @@
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.093294 ini2toml-0.8/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     8448 2022-02-07 16:54:49.000000 ini2toml-0.8/.cirrus.yml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      638 2022-02-07 14:28:30.000000 ini2toml-0.8/.coveragerc
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      550 2022-02-07 14:25:37.000000 ini2toml-0.8/.gitignore
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)       56 2022-02-07 14:25:37.000000 ini2toml-0.8/.isort.cfg
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1060 2022-02-07 16:54:49.000000 ini2toml-0.8/.pre-commit-config.yaml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      454 2021-11-21 22:59:54.000000 ini2toml-0.8/.projections.json
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      494 2022-02-07 14:29:50.000000 ini2toml-0.8/.readthedocs.yml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)       93 2022-02-07 14:25:37.000000 ini2toml-0.8/AUTHORS.rst
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     6256 2022-02-10 19:32:32.000000 ini2toml-0.8/CHANGELOG.rst
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)    11635 2022-02-07 18:56:05.000000 ini2toml-0.8/CONTRIBUTING.rst
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)    15922 2022-02-07 14:25:37.000000 ini2toml-0.8/LICENSE.txt
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1411 2022-02-10 19:32:32.000000 ini2toml-0.8/NOTICE.txt
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     5429 2022-02-10 19:48:22.093294 ini2toml-0.8/PKG-INFO
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     4534 2022-02-10 19:32:32.000000 ini2toml-0.8/README.rst
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:21.982483 ini2toml-0.8/docs/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1154 2022-02-07 14:25:37.000000 ini2toml-0.8/docs/Makefile
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:21.984537 ini2toml-0.8/docs/_static/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)       18 2022-02-07 14:25:37.000000 ini2toml-0.8/docs/_static/.gitignore
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1441 2021-11-21 22:59:54.000000 ini2toml-0.8/docs/_static/custom-adjustments.css
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)       41 2022-02-07 14:25:37.000000 ini2toml-0.8/docs/authors.rst
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)       43 2022-02-07 14:25:37.000000 ini2toml-0.8/docs/changelog.rst
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)    10743 2022-02-07 14:30:40.000000 ini2toml-0.8/docs/conf.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)       33 2022-02-07 14:25:37.000000 ini2toml-0.8/docs/contributing.rst
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)    12151 2021-11-21 22:59:54.000000 ini2toml-0.8/docs/dev-guide.rst
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      749 2022-02-07 14:30:40.000000 ini2toml-0.8/docs/index.rst
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)       67 2022-02-07 14:25:37.000000 ini2toml-0.8/docs/license.rst
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)       39 2022-02-07 14:25:37.000000 ini2toml-0.8/docs/readme.rst
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      310 2022-02-07 14:30:40.000000 ini2toml-0.8/docs/requirements.txt
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     5762 2021-12-07 16:30:42.000000 ini2toml-0.8/docs/setuptools_pep621.rst
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      355 2022-02-07 16:54:49.000000 ini2toml-0.8/pyproject.toml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2396 2022-02-10 19:48:22.113546 ini2toml-0.8/setup.cfg
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      705 2022-02-07 16:54:49.000000 ini2toml-0.8/setup.py
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:21.948152 ini2toml-0.8/src/
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:21.996888 ini2toml-0.8/src/ini2toml/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      820 2022-02-07 14:37:51.000000 ini2toml-0.8/src/ini2toml/__init__.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)       28 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/__main__.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1128 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/api.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     6595 2022-02-07 18:54:24.000000 ini2toml-0.8/src/ini2toml/base_translator.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     7348 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/cli.py
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.037950 ini2toml-0.8/src/ini2toml/drivers/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)        0 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/drivers/__init__.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      658 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/drivers/configparser.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2231 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/drivers/configupdater.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     9357 2022-02-10 19:32:32.000000 ini2toml-0.8/src/ini2toml/drivers/full_toml.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      575 2022-02-10 19:32:32.000000 ini2toml-0.8/src/ini2toml/drivers/lite_toml.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2185 2021-12-02 21:12:29.000000 ini2toml-0.8/src/ini2toml/drivers/plain_builtins.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2346 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/errors.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     8806 2022-02-10 17:18:32.000000 ini2toml-0.8/src/ini2toml/intermediate_repr.py
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.046483 ini2toml-0.8/src/ini2toml/plugins/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     3693 2021-12-07 15:07:10.000000 ini2toml-0.8/src/ini2toml/plugins/__init__.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2044 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/plugins/best_effort.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1823 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/plugins/coverage.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2387 2021-12-10 18:08:51.000000 ini2toml-0.8/src/ini2toml/plugins/isort.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2792 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/plugins/mypy.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1100 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/plugins/profile_independent_tasks.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2267 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/plugins/pytest.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)    35134 2022-02-10 19:32:32.000000 ini2toml-0.8/src/ini2toml/plugins/setuptools_pep621.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2396 2022-02-07 16:55:06.000000 ini2toml-0.8/src/ini2toml/profile.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)        0 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/py.typed
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     9908 2021-12-22 23:40:52.000000 ini2toml-0.8/src/ini2toml/transformations.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2712 2021-11-21 22:59:54.000000 ini2toml-0.8/src/ini2toml/translator.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     3229 2022-02-07 15:59:54.000000 ini2toml-0.8/src/ini2toml/types.py
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.030928 ini2toml-0.8/src/ini2toml.egg-info/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     5429 2022-02-10 19:48:21.000000 ini2toml-0.8/src/ini2toml.egg-info/PKG-INFO
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     3138 2022-02-10 19:48:21.000000 ini2toml-0.8/src/ini2toml.egg-info/SOURCES.txt
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)        1 2022-02-10 19:48:21.000000 ini2toml-0.8/src/ini2toml.egg-info/dependency_links.txt
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      424 2022-02-10 19:48:21.000000 ini2toml-0.8/src/ini2toml.egg-info/entry_points.txt
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)        1 2021-11-21 23:01:31.000000 ini2toml-0.8/src/ini2toml.egg-info/not-zip-safe
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      407 2022-02-10 19:48:21.000000 ini2toml-0.8/src/ini2toml.egg-info/requires.txt
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)        9 2022-02-10 19:48:21.000000 ini2toml-0.8/src/ini2toml.egg-info/top_level.txt
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.053516 ini2toml-0.8/tests/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)      276 2022-02-07 14:25:37.000000 ini2toml-0.8/tests/conftest.py
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.059513 ini2toml-0.8/tests/drivers/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1063 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/drivers/test_configparser.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1373 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/drivers/test_configupdater.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1709 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/drivers/test_full_toml.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1569 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/drivers/test_lite_toml.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1649 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/drivers/test_plain_builtins.py
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:21.951152 ini2toml-0.8/tests/examples/
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.061516 ini2toml-0.8/tests/examples/django/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1552 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/django/LICENSE
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2485 2022-02-07 16:54:49.000000 ini2toml-0.8/tests/examples/django/pyproject.toml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2124 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/django/setup.cfg
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.064513 ini2toml-0.8/tests/examples/flask/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1475 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/flask/LICENSE.rst
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     3368 2022-02-07 16:54:49.000000 ini2toml-0.8/tests/examples/flask/pyproject.toml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2949 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/flask/setup.cfg
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.066505 ini2toml-0.8/tests/examples/pandas/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1634 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/pandas/LICENSE
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     5149 2022-02-07 18:55:28.000000 ini2toml-0.8/tests/examples/pandas/pyproject.toml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     4955 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/pandas/setup.cfg
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.068519 ini2toml-0.8/tests/examples/pluggy/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1110 2021-12-22 23:51:44.000000 ini2toml-0.8/tests/examples/pluggy/LICENSE
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1792 2022-02-07 16:54:49.000000 ini2toml-0.8/tests/examples/pluggy/pyproject.toml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1426 2021-12-22 23:27:19.000000 ini2toml-0.8/tests/examples/pluggy/setup.cfg
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.071505 ini2toml-0.8/tests/examples/plumbum/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1080 2022-02-10 19:32:32.000000 ini2toml-0.8/tests/examples/plumbum/LICENSE
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2365 2022-02-10 19:32:32.000000 ini2toml-0.8/tests/examples/plumbum/pyproject.toml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1958 2022-02-10 19:32:32.000000 ini2toml-0.8/tests/examples/plumbum/setup.cfg
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.074505 ini2toml-0.8/tests/examples/pyscaffold/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1140 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/pyscaffold/LICENSE.txt
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     5877 2022-02-07 18:20:41.000000 ini2toml-0.8/tests/examples/pyscaffold/pyproject.toml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     5518 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/pyscaffold/setup.cfg
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.076513 ini2toml-0.8/tests/examples/setuptools_docs/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1050 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/setuptools_docs/LICENSE
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1401 2022-02-07 16:54:49.000000 ini2toml-0.8/tests/examples/setuptools_docs/pyproject.toml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1052 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/setuptools_docs/setup.cfg
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.079646 ini2toml-0.8/tests/examples/setuptools_scm/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1023 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/setuptools_scm/LICENSE
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     3195 2022-02-07 18:55:28.000000 ini2toml-0.8/tests/examples/setuptools_scm/pyproject.toml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2763 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/setuptools_scm/setup.cfg
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.082654 ini2toml-0.8/tests/examples/virtualenv/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1074 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/virtualenv/LICENSE
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     5149 2022-02-07 18:55:28.000000 ini2toml-0.8/tests/examples/virtualenv/pyproject.toml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     4641 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/examples/virtualenv/setup.cfg
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.086654 ini2toml-0.8/tests/examples/zipp/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1050 2021-12-10 15:54:44.000000 ini2toml-0.8/tests/examples/zipp/LICENSE
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1468 2022-02-07 16:54:49.000000 ini2toml-0.8/tests/examples/zipp/pyproject.toml
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1105 2021-12-10 15:54:22.000000 ini2toml-0.8/tests/examples/zipp/setup.cfg
-drwxr-xr-x   0 abravalheri  (1000) abravalheri  (1000)        0 2022-02-10 19:48:22.091653 ini2toml-0.8/tests/plugins/
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1003 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/plugins/test_best_effort.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2171 2022-02-07 14:43:57.000000 ini2toml-0.8/tests/plugins/test_coverage.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1516 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/plugins/test_isort.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1602 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/plugins/test_mypy.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1462 2022-02-07 14:43:57.000000 ini2toml-0.8/tests/plugins/test_pytest.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)    18221 2022-02-07 18:55:28.000000 ini2toml-0.8/tests/plugins/test_setuptools_pep621.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     3772 2021-11-21 23:10:18.000000 ini2toml-0.8/tests/test_cli.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     4270 2022-02-10 19:32:32.000000 ini2toml-0.8/tests/test_examples.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1613 2021-11-21 22:59:54.000000 ini2toml-0.8/tests/test_intermediate_repr.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     1861 2021-12-03 06:25:09.000000 ini2toml-0.8/tests/test_plugins.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     5235 2022-02-07 18:55:28.000000 ini2toml-0.8/tests/test_transformations.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     3708 2022-02-07 18:54:24.000000 ini2toml-0.8/tests/test_translator.py
--rw-r--r--   0 abravalheri  (1000) abravalheri  (1000)     2656 2022-02-07 16:54:49.000000 ini2toml-0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.526247 ini2toml-0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     8448 2022-03-04 11:39:55.000000 ini2toml-0.9/.cirrus.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-03-04 11:39:55.000000 ini2toml-0.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.506247 ini2toml-0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.514247 ini2toml-0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     3767 2022-03-04 11:39:55.000000 ini2toml-0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-03-04 11:39:55.000000 ini2toml-0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-03-04 11:39:55.000000 ini2toml-0.9/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-03-04 11:39:55.000000 ini2toml-0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2022-03-04 11:39:55.000000 ini2toml-0.9/.projections.json
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-03-04 11:39:55.000000 ini2toml-0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-03-04 11:39:55.000000 ini2toml-0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6548 2022-03-04 11:39:55.000000 ini2toml-0.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11635 2022-03-04 11:39:55.000000 ini2toml-0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    15922 2022-03-04 11:39:55.000000 ini2toml-0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-03-04 11:39:55.000000 ini2toml-0.9/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5458 2022-03-04 11:41:20.526247 ini2toml-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4534 2022-03-04 11:39:55.000000 ini2toml-0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.514247 ini2toml-0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-03-04 11:39:55.000000 ini2toml-0.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.514247 ini2toml-0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-03-04 11:39:55.000000 ini2toml-0.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-03-04 11:39:55.000000 ini2toml-0.9/docs/_static/custom-adjustments.css
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-03-04 11:39:55.000000 ini2toml-0.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-03-04 11:39:55.000000 ini2toml-0.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10743 2022-03-04 11:39:55.000000 ini2toml-0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-03-04 11:39:55.000000 ini2toml-0.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12151 2022-03-04 11:39:55.000000 ini2toml-0.9/docs/dev-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-03-04 11:39:55.000000 ini2toml-0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-03-04 11:39:55.000000 ini2toml-0.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-03-04 11:39:55.000000 ini2toml-0.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2022-03-04 11:39:55.000000 ini2toml-0.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5762 2022-03-04 11:39:55.000000 ini2toml-0.9/docs/setuptools_pep621.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      355 2022-03-04 11:39:55.000000 ini2toml-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-03-04 11:41:20.526247 ini2toml-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-03-04 11:39:55.000000 ini2toml-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.506247 ini2toml-0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.518247 ini2toml-0.9/src/ini2toml/
+-rw-r--r--   0 runner    (1001) docker     (121)      820 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6595 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/base_translator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8215 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.518247 ini2toml-0.9/src/ini2toml/drivers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      658 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/drivers/configparser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2231 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/drivers/configupdater.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10295 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/drivers/full_toml.py
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/drivers/lite_toml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2185 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/drivers/plain_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2346 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8806 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/intermediate_repr.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.518247 ini2toml-0.9/src/ini2toml/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)     3693 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2044 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/plugins/best_effort.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/plugins/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2387 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/plugins/isort.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2792 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/plugins/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/plugins/profile_independent_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/plugins/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35134 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/plugins/setuptools_pep621.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/profile.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     9908 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/translator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3229 2022-03-04 11:39:55.000000 ini2toml-0.9/src/ini2toml/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.518247 ini2toml-0.9/src/ini2toml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5458 2022-03-04 11:41:20.000000 ini2toml-0.9/src/ini2toml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-03-04 11:41:20.000000 ini2toml-0.9/src/ini2toml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-04 11:41:20.000000 ini2toml-0.9/src/ini2toml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2022-03-04 11:41:20.000000 ini2toml-0.9/src/ini2toml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-04 11:41:19.000000 ini2toml-0.9/src/ini2toml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2022-03-04 11:41:20.000000 ini2toml-0.9/src/ini2toml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-03-04 11:41:20.000000 ini2toml-0.9/src/ini2toml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.522247 ini2toml-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.522247 ini2toml-0.9/tests/drivers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/drivers/test_configparser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/drivers/test_configupdater.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/drivers/test_full_toml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/drivers/test_lite_toml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/drivers/test_plain_builtins.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.510247 ini2toml-0.9/tests/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.522247 ini2toml-0.9/tests/examples/django/
+-rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/django/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2483 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/django/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/django/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.522247 ini2toml-0.9/tests/examples/flask/
+-rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/flask/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/flask/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2949 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/flask/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.522247 ini2toml-0.9/tests/examples/pandas/
+-rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/pandas/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     5099 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/pandas/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     4955 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/pandas/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.522247 ini2toml-0.9/tests/examples/pluggy/
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/pluggy/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/pluggy/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/pluggy/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.522247 ini2toml-0.9/tests/examples/plumbum/
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/plumbum/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/plumbum/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/plumbum/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.522247 ini2toml-0.9/tests/examples/pyscaffold/
+-rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/pyscaffold/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5877 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/pyscaffold/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     5518 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/pyscaffold/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.522247 ini2toml-0.9/tests/examples/setuptools_docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/setuptools_docs/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1399 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/setuptools_docs/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/setuptools_docs/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.526247 ini2toml-0.9/tests/examples/setuptools_scm/
+-rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/setuptools_scm/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/setuptools_scm/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2763 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/setuptools_scm/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.526247 ini2toml-0.9/tests/examples/virtualenv/
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/virtualenv/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     5147 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/virtualenv/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     4641 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/virtualenv/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.526247 ini2toml-0.9/tests/examples/zipp/
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/zipp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/zipp/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/examples/zipp/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:41:20.526247 ini2toml-0.9/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/plugins/test_best_effort.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/plugins/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/plugins/test_isort.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/plugins/test_mypy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/plugins/test_profile_independent_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/plugins/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18217 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/plugins/test_setuptools_pep621.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4764 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4697 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/test_intermediate_repr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5235 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3708 2022-03-04 11:39:55.000000 ini2toml-0.9/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2826 2022-03-04 11:39:55.000000 ini2toml-0.9/tox.ini
```

### Comparing `ini2toml-0.8/.cirrus.yml` & `ini2toml-0.9/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/.coveragerc` & `ini2toml-0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/.gitignore` & `ini2toml-0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/.pre-commit-config.yaml` & `ini2toml-0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/CHANGELOG.rst` & `ini2toml-0.9/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
 Changelog
 =========
 
+Version 0.9
+===========
+
+- Fixed missing terminating newline at the end of the generated file, :pr:`27`, :pr:`32`
+- Added heuristic for appropriate string representation selection when
+  serialising TOML, :pr:`28`
+- [CI] Added GitHub Actions for automatic test and release of tags, :pr:`30`
+
 Version 0.8
 ===========
 
 - :pypi:`atoml` dependency replaced with :pypi:`tomlkit`, :issue:`23`
 - ``setuptools`` plugin:
     - Now commas are stripped when splitting keywords for setuptools plugin, :issue:`24`
```

### Comparing `ini2toml-0.8/CONTRIBUTING.rst` & `ini2toml-0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/LICENSE.txt` & `ini2toml-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/NOTICE.txt` & `ini2toml-0.9/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/PKG-INFO` & `ini2toml-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ini2toml
-Version: 0.8
+Version: 0.9
 Summary: Automatically conversion of .ini/.cfg files to TOML equivalents
 Home-page: https://github.com/abravalheri/ini2toml/
 Author: Anderson Bravalheri
 Author-email: andersonbravalheri@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://ini2toml.readthedocs.io/
 Project-URL: Source, https://github.com/abravalheri/ini2toml
@@ -14,14 +14,15 @@
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: full
 Provides-Extra: lite
 Provides-Extra: all
+Provides-Extra: experimental
 Provides-Extra: testing
 Provides-Extra: typechecking
 License-File: LICENSE.txt
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
```

### Comparing `ini2toml-0.8/README.rst` & `ini2toml-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/docs/Makefile` & `ini2toml-0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/docs/_static/custom-adjustments.css` & `ini2toml-0.9/docs/_static/custom-adjustments.css`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/docs/conf.py` & `ini2toml-0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/docs/dev-guide.rst` & `ini2toml-0.9/docs/dev-guide.rst`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/docs/index.rst` & `ini2toml-0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/docs/setuptools_pep621.rst` & `ini2toml-0.9/docs/setuptools_pep621.rst`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/setup.cfg` & `ini2toml-0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -33,22 +33,24 @@
 exclude = 
 	tests
 
 [options.extras_require]
 full = 
 	importlib-metadata; python_version<"3.8"
 	configupdater>=3.0.1,<4
-	tomlkit>=0.9.2,<2
+	tomlkit>=0.10.0,<2
 lite = 
 	importlib-metadata; python_version<"3.8"
 	tomli-w>=0.4.0,<2
 all = 
 	configupdater>=3.0.1,<4
-	tomlkit>=0.9.2,<2
+	tomlkit>=0.10.0,<2
 	tomli-w>=0.4.0,<2
+experimental = 
+	pyproject-fmt>=0.3.2
 testing = 
 	setuptools
 	tomli
 	pytest
 	pytest-cov
 	validate-pyproject>=0.3.2,<2
 typechecking =
```

### Comparing `ini2toml-0.8/setup.py` & `ini2toml-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/__init__.py` & `ini2toml-0.9/src/ini2toml/__init__.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/api.py` & `ini2toml-0.9/src/ini2toml/api.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/base_translator.py` & `ini2toml-0.9/src/ini2toml/base_translator.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/cli.py` & `ini2toml-0.9/src/ini2toml/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -79,14 +79,37 @@
         dest="loglevel",
         action="store_const",
         const=logging.DEBUG,
         help="set logging level to DEBUG",
     ),
 }
 
+try:
+    from pyproject_fmt import Config, format_pyproject
+
+    META["auto_format"] = dict(
+        flags=("-F", "--auto-format"),
+        action="store_true",
+        help="**EXPERIMENTAL** - format output with `pyproject-fmt`\n"
+        "(note that auto-formatting is intrusive and may cause loss of comments).",
+    )
+
+    def apply_auto_formatting(text: str) -> str:
+        try:
+            return format_pyproject(Config(text))
+        except Exception as ex:  # pragma: no cover
+            _logger.debug(f"pyproject-fmt failed: {ex}", exc_info=True)
+            _logger.warning("Auto-formatting failed, falling back to original text")
+            return text
+
+except ImportError:  # pragma: no cover
+
+    def apply_auto_formatting(text: str) -> str:
+        return text
+
 
 def __meta__(
     profiles: Sequence[Profile], augmentations: Sequence[ProfileAugmentation]
 ) -> Dict[str, dict]:
     """'Hyper parameters' to instruct :mod:`argparse` how to create the CLI"""
     meta = {k: v.copy() for k, v in META.items()}
     meta["profile"]["help"] += _choices_help(profiles, lambda x: x.help_text.strip())
@@ -171,14 +194,16 @@
     profiles = list(translator.profiles.values())
     profile_augmentations = list(translator.augmentations.values())
     params = parse_args(args, profiles, profile_augmentations)
     setup_logging(params.loglevel)
     out = translator.translate(
         params.input_file.read(), params.profile, params.active_augmentations
     )
+    if getattr(params, "auto_format", False):
+        out = apply_auto_formatting(out)
     params.output_file.write(out)
 
 
 class Formatter(argparse.RawTextHelpFormatter):
     # Since the stdlib does not specify what is the signature we need to implement in
     # order to create our own formatter, we are left no choice other then overwrite a
     # "private" method considered to be an implementation detail.
```

### Comparing `ini2toml-0.8/src/ini2toml/drivers/configparser.py` & `ini2toml-0.9/src/ini2toml/drivers/configparser.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/drivers/configupdater.py` & `ini2toml-0.9/src/ini2toml/drivers/configupdater.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/drivers/full_toml.py` & `ini2toml-0.9/src/ini2toml/drivers/full_toml.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,18 @@
     comment,
     document,
     dumps,
     inline_table,
     item,
     loads,
     nl,
+    string,
     table,
 )
-from tomlkit.items import AoT, Array, InlineTable, Item, Table
+from tomlkit.items import AoT, Array, InlineTable, Item, String, Table
 from tomlkit.toml_document import TOMLDocument
 
 from ..errors import InvalidTOMLKey
 from ..types import (
     KV,
     Commented,
     CommentedKV,
@@ -46,23 +47,29 @@
 MAX_INLINE_TABLE_LEN = 67
 INLINE_TABLE_LONG_ELEM = 10
 MAX_INLINE_TABLE_LONG_ELEM = 5
 LONG = 120
 
 
 def convert(irepr: IntermediateRepr) -> str:
-    return dumps(collapse(irepr, root=True))
+    text = dumps(collapse(irepr, root=True))
+    return text.strip() + "\n"  # ensure terminating newline (POSIX requirement)
 
 
 @singledispatch
 def collapse(obj, root=False):
     # Catch all
     return obj
 
 
+@collapse.register(str)
+def _collapse_string(obj: str) -> String:
+    return _string(obj)
+
+
 @collapse.register(Commented)
 def _collapse_commented(obj: Commented, root=False) -> Item:
     return create_item(obj.value_or(None), obj.comment)
 
 
 @collapse.register(CommentedList)
 def _collapse_commented_list(obj: CommentedList, root=False) -> Array:
@@ -231,15 +238,15 @@
     return out
 
 
 # --- Helpers ---
 
 
 def create_item(value, comment):
-    obj = item(value)
+    obj = _item(value)
     if comment is not None:
         obj.comment(comment)
     return obj
 
 
 def create_table(m: Mapping) -> Table:
     if isinstance(m, Table):
@@ -287,7 +294,32 @@
             has_nested = has_nested or any(c in simplified_str for c in "{[")
         len_elem = len(elem_repr)
         total_len += len_elem + 2
         max_len = max(max_len, len_elem)
         has_nl = has_nl or "\n" in elem_repr
 
     return is_aot, max_len, total_len, has_nl, has_nested, len(seq)
+
+
+def _item(obj) -> Item:
+    if isinstance(obj, str):
+        return _string(obj)
+
+    return item(obj)
+
+
+def _string(obj: str) -> String:
+    """Try to guess the best TOML representation for a string"""
+    multiline = "\n" in obj
+    single_line = "".join(x.strip().rstrip("\\") for x in obj.splitlines())
+    literal = '"' in obj or "\\" in single_line
+
+    if multiline and not obj.startswith("\n"):
+        # TOML will automatically strip an starting newline
+        # so let's add it, since it is better for reading
+        obj = "\n" + obj
+
+    try:
+        return string(obj, literal=literal, multiline=multiline)
+    except ValueError:
+        # Literal strings are not always possible
+        return string(obj, multiline=multiline)
```

### Comparing `ini2toml-0.8/src/ini2toml/drivers/lite_toml.py` & `ini2toml-0.9/src/ini2toml/drivers/lite_toml.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 
 __all__ = [
     "convert",
 ]
 
 
 def convert(irepr: IntermediateRepr) -> str:
-    return dumps(plain_builtins.convert(irepr))
+    text = dumps(plain_builtins.convert(irepr))
+    return text.strip() + "\n"  # ensure terminating newline (POSIX requirement)
```

### Comparing `ini2toml-0.8/src/ini2toml/drivers/plain_builtins.py` & `ini2toml-0.9/src/ini2toml/drivers/plain_builtins.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/errors.py` & `ini2toml-0.9/src/ini2toml/errors.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/intermediate_repr.py` & `ini2toml-0.9/src/ini2toml/intermediate_repr.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/plugins/__init__.py` & `ini2toml-0.9/src/ini2toml/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/plugins/best_effort.py` & `ini2toml-0.9/src/ini2toml/plugins/best_effort.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/plugins/coverage.py` & `ini2toml-0.9/src/ini2toml/plugins/coverage.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/plugins/isort.py` & `ini2toml-0.9/src/ini2toml/plugins/isort.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/plugins/mypy.py` & `ini2toml-0.9/src/ini2toml/plugins/mypy.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/plugins/profile_independent_tasks.py` & `ini2toml-0.9/src/ini2toml/plugins/profile_independent_tasks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """Profile-independent tasks implemented via *profile augmentation*."""
 import re
 from functools import wraps
 from typing import Callable
 
 from ..types import Profile, Translator
 
-NEWLINES = re.compile(r"\n+", re.M)
+DUPLICATED_NEWLINES = re.compile(r"\n+", re.M)
 TABLE_START = re.compile(r"^\[(.*)\]", re.M)
 EMPTY_TABLES = re.compile(r"^\[(.*)\]\n+\[(\1\.(?:.*))\]", re.M)
+MISSING_TERMINATING_LINE = re.compile(r"(?<!\n)\Z", re.M)
+# ^ POSIX tools will not play nicely with text files without a terminating new line
+# https://unix.stackexchange.com/questions/18743/whats-the-point-in-adding-a-new-line-to-the-end-of-a-file
 
 
 def activate(translator: Translator):
-    tasks = [normalise_newlines, remove_empty_table_headers]
+    tasks = [
+        normalise_newlines,
+        remove_empty_table_headers,
+        ensure_terminating_newlines,
+    ]
     for task in tasks:
         translator.augment_profiles(post_process(task), active_by_default=True)
 
 
 def post_process(fn: Callable[[str], str]):
     @wraps(fn)
     def _augmentation(profile: Profile):
@@ -23,15 +30,25 @@
 
     return _augmentation
 
 
 def normalise_newlines(text: str) -> str:
     """Make sure every table is preceded by an empty newline, but remove them elsewhere
     in the output TOML document.
+    Also ensure a terminating newline is present for best POSIX tool compatibility.
     """
-    text = NEWLINES.sub(r"\n", text)
-    return TABLE_START.sub(r"\n[\1]", text)
+    text = DUPLICATED_NEWLINES.sub(r"\n", text)
+    text = TABLE_START.sub(r"\n[\1]", text)
+    return MISSING_TERMINATING_LINE.sub("\n", text)
 
 
 def remove_empty_table_headers(text: str) -> str:
     """Remove empty TOML table headers"""
-    return EMPTY_TABLES.sub(r"[\2]", text).strip()
+    prev_text = ""
+    while text != prev_text:
+        prev_text = text
+        text = EMPTY_TABLES.sub(r"[\2]", text).strip()
+    return text
+
+
+def ensure_terminating_newlines(text: str) -> str:
+    return text.strip() + "\n"
```

### Comparing `ini2toml-0.8/src/ini2toml/plugins/pytest.py` & `ini2toml-0.9/src/ini2toml/plugins/pytest.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/plugins/setuptools_pep621.py` & `ini2toml-0.9/src/ini2toml/plugins/setuptools_pep621.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/profile.py` & `ini2toml-0.9/src/ini2toml/profile.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/transformations.py` & `ini2toml-0.9/src/ini2toml/transformations.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/translator.py` & `ini2toml-0.9/src/ini2toml/translator.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml/types.py` & `ini2toml-0.9/src/ini2toml/types.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/src/ini2toml.egg-info/PKG-INFO` & `ini2toml-0.9/src/ini2toml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ini2toml
-Version: 0.8
+Version: 0.9
 Summary: Automatically conversion of .ini/.cfg files to TOML equivalents
 Home-page: https://github.com/abravalheri/ini2toml/
 Author: Anderson Bravalheri
 Author-email: andersonbravalheri@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://ini2toml.readthedocs.io/
 Project-URL: Source, https://github.com/abravalheri/ini2toml
@@ -14,14 +14,15 @@
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: full
 Provides-Extra: lite
 Provides-Extra: all
+Provides-Extra: experimental
 Provides-Extra: testing
 Provides-Extra: typechecking
 License-File: LICENSE.txt
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
```

### Comparing `ini2toml-0.8/src/ini2toml.egg-info/SOURCES.txt` & `ini2toml-0.9/src/ini2toml.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 LICENSE.txt
 NOTICE.txt
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
+.github/workflows/ci.yml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/dev-guide.rst
 docs/index.rst
@@ -103,9 +104,10 @@
 tests/examples/zipp/LICENSE
 tests/examples/zipp/pyproject.toml
 tests/examples/zipp/setup.cfg
 tests/plugins/test_best_effort.py
 tests/plugins/test_coverage.py
 tests/plugins/test_isort.py
 tests/plugins/test_mypy.py
+tests/plugins/test_profile_independent_tasks.py
 tests/plugins/test_pytest.py
 tests/plugins/test_setuptools_pep621.py
```

### Comparing `ini2toml-0.8/tests/drivers/test_configparser.py` & `ini2toml-0.9/tests/drivers/test_configparser.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/drivers/test_configupdater.py` & `ini2toml-0.9/tests/drivers/test_configupdater.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/drivers/test_full_toml.py` & `ini2toml-0.9/tests/drivers/test_full_toml.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/drivers/test_lite_toml.py` & `ini2toml-0.9/tests/drivers/test_lite_toml.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/drivers/test_plain_builtins.py` & `ini2toml-0.9/tests/drivers/test_plain_builtins.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/django/LICENSE` & `ini2toml-0.9/tests/examples/django/LICENSE`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/django/pyproject.toml` & `ini2toml-0.9/tests/examples/django/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = ["license", "version"]
 requires-python = ">=3.8"
 dependencies = [
     "asgiref >= 3.3.2",
-    "backports.zoneinfo; python_version<\"3.9\"",
+    'backports.zoneinfo; python_version<"3.9"',
     "sqlparse >= 0.2.2",
     "tzdata; sys_platform == 'win32'",
 ]
 
 [project.urls]
 Homepage = "https://www.djangoproject.com/"
 Documentation = "https://docs.djangoproject.com/"
```

### Comparing `ini2toml-0.8/tests/examples/django/setup.cfg` & `ini2toml-0.9/tests/examples/django/setup.cfg`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/flask/LICENSE.rst` & `ini2toml-0.9/tests/examples/flask/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/flask/pyproject.toml` & `ini2toml-0.9/tests/examples/flask/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -75,18 +75,30 @@
 # B = bugbear
 # E = pycodestyle errors
 # F = flake8 pyflakes
 # W = pycodestyle warnings
 # B9 = bugbear opinions
 # ISC = implicit-str-concat
 select = "B, E, F, W, B9, ISC"
-ignore = "\n# slice notation whitespace, invalid\nE203\n# import at top, too many circular import fixes\nE402\n# line length, handled by bugbear B950\nE501\n# bare except, handled by bugbear B001\nE722\n# bin op line break, invalid\nW503"
+ignore = """
+# slice notation whitespace, invalid
+E203
+# import at top, too many circular import fixes
+E402
+# line length, handled by bugbear B950
+E501
+# bare except, handled by bugbear B001
+E722
+# bin op line break, invalid
+W503"""
 # up to 88 allowed by bugbear B950
 max-line-length = "80"
-per-file-ignores = "\n# __init__ module exports names\nsrc/flask/__init__.py: F401"
+per-file-ignores = """
+# __init__ module exports names
+src/flask/__init__.py: F401"""
 
 [tool.mypy]
 files = ["src/flask"]
 python_version = "3.6"
 allow_redefinition = true
 disallow_subclassing_any = true
 # disallow_untyped_calls = True
```

### Comparing `ini2toml-0.8/tests/examples/flask/setup.cfg` & `ini2toml-0.9/tests/examples/flask/setup.cfg`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/pandas/LICENSE` & `ini2toml-0.9/tests/examples/pandas/LICENSE`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/pandas/pyproject.toml` & `ini2toml-0.9/tests/examples/pandas/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -76,27 +76,98 @@
 versionfile_source = "pandas/_version.py"
 versionfile_build = "pandas/_version.py"
 tag_prefix = "v"
 parentdir_prefix = "pandas-"
 
 [tool.flake8]
 max-line-length = "88"
-ignore = "\n# space before : (needed for how black formats slicing)\nE203,\n# line break before binary operator\nW503,\n# line break after binary operator\nW504,\n# module level import not at top of file\nE402,\n# do not assign a lambda expression, use a def\nE731,\n# found modulo formatter (incorrect picks up mod operations)\nS001,\n# controversial\nB005,\n# controversial\nB006,\n# controversial\nB007,\n# controversial\nB008,\n# setattr is used to side-step mypy\nB009,\n# getattr is used to side-step mypy\nB010,\n# tests use assert False\nB011,\n# tests use comparisons but not their returned value\nB015,\n# false positives\nB301"
-exclude = "\ndoc/sphinxext/*.py,\ndoc/build/*.py,\ndoc/temp/*.py,\n.eggs/*.py,\nversioneer.py,\n# exclude asv benchmark environments from linting\nenv"
-per-file-ignores = "\n# private import across modules\npandas/tests/*:PDF020\n# pytest.raises without match=\npandas/tests/extension/*:PDF009\n# os.remove\ndoc/make.py:PDF008\n# import from pandas._testing\npandas/testing.py:PDF014"
+ignore = """
+# space before : (needed for how black formats slicing)
+E203,
+# line break before binary operator
+W503,
+# line break after binary operator
+W504,
+# module level import not at top of file
+E402,
+# do not assign a lambda expression, use a def
+E731,
+# found modulo formatter (incorrect picks up mod operations)
+S001,
+# controversial
+B005,
+# controversial
+B006,
+# controversial
+B007,
+# controversial
+B008,
+# setattr is used to side-step mypy
+B009,
+# getattr is used to side-step mypy
+B010,
+# tests use assert False
+B011,
+# tests use comparisons but not their returned value
+B015,
+# false positives
+B301"""
+exclude = """
+doc/sphinxext/*.py,
+doc/build/*.py,
+doc/temp/*.py,
+.eggs/*.py,
+versioneer.py,
+# exclude asv benchmark environments from linting
+env"""
+per-file-ignores = """
+# private import across modules
+pandas/tests/*:PDF020
+# pytest.raises without match=
+pandas/tests/extension/*:PDF009
+# os.remove
+doc/make.py:PDF008
+# import from pandas._testing
+pandas/testing.py:PDF014"""
 
 [tool.flake8-rst]
 max-line-length = "84"
-bootstrap = "\nimport numpy as np\nimport pandas as pd\n# avoiding error when importing again numpy or pandas\nnp\n# (in some cases we want to do it to show users)\npd"
-ignore = "\n# space before : (needed for how black formats slicing)\nE203,\n# module level import not at top of file\nE402,\n# line break before binary operator\nW503,\n# Classes/functions in different blocks can generate those errors\n# expected 2 blank lines, found 0\nE302,\n# expected 2 blank lines after class or function definition, found 0\nE305,\n# We use semicolon at the end to avoid displaying plot objects\n# statement ends with a semicolon\nE703,\n# comparison to none should be 'if cond is none:'\nE711,"
-exclude = "\ndoc/source/development/contributing_docstring.rst,\n# work around issue of undefined variable warnings\n# https://github.com/pandas-dev/pandas/pull/38837#issuecomment-752884156\ndoc/source/getting_started/comparison/includes/*.rst"
+bootstrap = """
+import numpy as np
+import pandas as pd
+# avoiding error when importing again numpy or pandas
+np
+# (in some cases we want to do it to show users)
+pd"""
+ignore = """
+# space before : (needed for how black formats slicing)
+E203,
+# module level import not at top of file
+E402,
+# line break before binary operator
+W503,
+# Classes/functions in different blocks can generate those errors
+# expected 2 blank lines, found 0
+E302,
+# expected 2 blank lines after class or function definition, found 0
+E305,
+# We use semicolon at the end to avoid displaying plot objects
+# statement ends with a semicolon
+E703,
+# comparison to none should be 'if cond is none:'
+E711,"""
+exclude = """
+doc/source/development/contributing_docstring.rst,
+# work around issue of undefined variable warnings
+# https://github.com/pandas-dev/pandas/pull/38837#issuecomment-752884156
+doc/source/getting_started/comparison/includes/*.rst"""
 
 [tool.codespell]
 ignore-words-list = "ba,blocs,coo,hist,nd,sav,ser"
-ignore-regex = "https://(\\w+\\.)+"
+ignore-regex = 'https://(\w+\.)+'
 
 [tool.coverage.run]
 branch = true
 omit = [
     "*/tests/*",
     "pandas/_typing.py",
     "pandas/_version.py",
@@ -110,15 +181,15 @@
 omit = ["pandas/_version.py"]
 # Regexes for lines to exclude from consideration
 exclude_lines = [
     # Have to re-enable the standard pragma
     "pragma: no cover",
     # Don't complain about missing debug-only code:
     "def __repr__",
-    "if self\\.debug",
+    'if self\.debug',
     # Don't complain if tests don't hit defensive assertion code:
     "raise AssertionError",
     "raise NotImplementedError",
     "AbstractMethodError",
     # Don't complain if non-runnable code isn't run:
     "if 0:",
     "if __name__ == .__main__.:",
```

### Comparing `ini2toml-0.8/tests/examples/pandas/setup.cfg` & `ini2toml-0.9/tests/examples/pandas/setup.cfg`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/pluggy/LICENSE` & `ini2toml-0.9/tests/examples/pluggy/LICENSE`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/pluggy/pyproject.toml` & `ini2toml-0.9/tests/examples/pluggy/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 urls = {Homepage = "https://github.com/pytest-dev/pluggy"}
 dynamic = ["license", "version"]
 requires-python = ">=3.6"
-dependencies = ["importlib-metadata>=0.12;python_version<\"3.8\""]
+dependencies = ['importlib-metadata>=0.12;python_version<"3.8"']
 
 [project.readme]
 file = "README.rst"
 content-type = "text/x-rst"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `ini2toml-0.8/tests/examples/pluggy/setup.cfg` & `ini2toml-0.9/tests/examples/pluggy/setup.cfg`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/plumbum/LICENSE` & `ini2toml-0.9/tests/examples/plumbum/LICENSE`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/plumbum/pyproject.toml` & `ini2toml-0.9/tests/examples/plumbum/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/plumbum/setup.cfg` & `ini2toml-0.9/tests/examples/plumbum/setup.cfg`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/pyscaffold/LICENSE.txt` & `ini2toml-0.9/tests/examples/pyscaffold/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/pyscaffold/pyproject.toml` & `ini2toml-0.9/tests/examples/pyscaffold/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
 dynamic = ["license", "version"]
 requires-python = ">=3.6"
 dependencies = [
-    "importlib-metadata; python_version<\"3.8\"",
+    'importlib-metadata; python_version<"3.8"',
     "appdirs>=1.4.4,<2",
     "configupdater>=3.0,<4",
     "setuptools>=46.1.0",
     "setuptools_scm>=5",
     "tomlkit>=0.7.0,<2",
     "packaging>=20.7",
     # packaging is versioned by year, not SemVer
@@ -121,15 +121,17 @@
 [tool.pytest.ini_options]
 # Options for pytest:
 # Specify command line options as you would do when invoking pytest directly.
 # e.g. --cov-report html (or xml) for html/xml output or --junit-xml junit.xml
 # in order to write a coverage file that can be read by Jenkins.
 # CAUTION: --cov flags may prohibit setting breakpoints while debugging.
 # Comment those flags to avoid this pytest issue.
-addopts = "--cov pyscaffold --cov-config .coveragerc --cov-report term-missing\n--verbose"
+addopts = """
+--cov pyscaffold --cov-config .coveragerc --cov-report term-missing
+--verbose"""
 # In order to use xdist, the developer can add, for example, the following
 # arguments:
 # --dist=load --numprocesses=auto
 norecursedirs = [
     "dist",
     "build",
     ".tox",
@@ -156,15 +158,21 @@
 
 [tool.flake8]
 # Some sane defaults for the code style checker flake8
 # black compatibility
 max_line_length = "88"
 # E203 and W503 have edge cases handled by black
 extend_ignore = "E203, W503"
-exclude = "\nsrc/pyscaffold/contrib\n.tox\nbuild\ndist\n.eggs\ndocs/conf.py"
+exclude = """
+src/pyscaffold/contrib
+.tox
+build
+dist
+.eggs
+docs/conf.py"""
 
 [tool.mypy]
 ignore_missing_imports = true
 pretty = true
 show_error_codes = true
 show_error_context = true
 show_traceback = true
```

### Comparing `ini2toml-0.8/tests/examples/pyscaffold/setup.cfg` & `ini2toml-0.9/tests/examples/pyscaffold/setup.cfg`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/setuptools_docs/LICENSE` & `ini2toml-0.9/tests/examples/setuptools_docs/LICENSE`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/setuptools_docs/pyproject.toml` & `ini2toml-0.9/tests/examples/setuptools_docs/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.5",
 ]
 dynamic = ["readme", "license", "version"]
 dependencies = [
     "requests",
-    "importlib; python_version == \"2.6\"",
+    'importlib; python_version == "2.6"',
 ]
 
 [project.optional-dependencies]
 pdf = ["ReportLab>=1.2", "RXP"]
 rest = ["docutils>=0.3", "pack ==1.1, ==1.3"]
 
 [project.scripts]
```

### Comparing `ini2toml-0.8/tests/examples/setuptools_docs/setup.cfg` & `ini2toml-0.9/tests/examples/setuptools_docs/setup.cfg`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/setuptools_scm/LICENSE` & `ini2toml-0.9/tests/examples/setuptools_scm/LICENSE`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/setuptools_scm/pyproject.toml` & `ini2toml-0.9/tests/examples/setuptools_scm/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/setuptools_scm/setup.cfg` & `ini2toml-0.9/tests/examples/setuptools_scm/setup.cfg`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/virtualenv/LICENSE` & `ini2toml-0.9/tests/examples/virtualenv/LICENSE`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/virtualenv/pyproject.toml` & `ini2toml-0.9/tests/examples/virtualenv/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 requires-python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
 dependencies = [
     "backports.entry_points_selectable>=1.0.4",
     "distlib>=0.3.1,<1",
     "filelock>=3.0.0,<4",
     "platformdirs>=2,<3",
     "six>=1.9.0,<2", # keep it >=1.9.0 as it may cause problems on LTS platforms
-    "importlib-metadata>=0.12;python_version<\"3.8\"",
-    "importlib-resources>=1.0;python_version<\"3.7\"",
+    'importlib-metadata>=0.12;python_version<"3.8"',
+    'importlib-resources>=1.0;python_version<"3.7"',
     "pathlib2>=2.3.3,<3;python_version < '3.4' and sys.platform != 'win32'",
 ]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
@@ -95,15 +95,15 @@
     "flaky>=3",
     "pytest>=4",
     "pytest-env>=0.6.2",
     "pytest-freezegun>=0.4.1",
     "pytest-mock>=2",
     "pytest-randomly>=1",
     "pytest-timeout>=1",
-    "packaging>=20.0;python_version>\"3.4\"",
+    'packaging>=20.0;python_version>"3.4"',
 ]
 
 [project.scripts]
 virtualenv = "virtualenv.__main__:run_with_catch"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
@@ -134,8 +134,10 @@
 [tool.distutils.bdist_wheel]
 universal = true
 
 [tool.pytest.ini_options]
 markers = ["slow"]
 junit_family = "xunit2"
 addopts = "--tb=auto -ra --showlocals --no-success-flaky-report"
-env = "PYTHONWARNINGS=ignore:DEPRECATION::pip._internal.cli.base_command\nPYTHONIOENCODING=utf-8"
+env = """
+PYTHONWARNINGS=ignore:DEPRECATION::pip._internal.cli.base_command
+PYTHONIOENCODING=utf-8"""
```

### Comparing `ini2toml-0.8/tests/examples/virtualenv/setup.cfg` & `ini2toml-0.9/tests/examples/virtualenv/setup.cfg`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/zipp/LICENSE` & `ini2toml-0.9/tests/examples/zipp/LICENSE`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/examples/zipp/pyproject.toml` & `ini2toml-0.9/tests/examples/zipp/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 [project.optional-dependencies]
 testing = [
     # upstream
     "pytest >= 6",
     "pytest-checkdocs >= 2.4",
     "pytest-flake8",
-    "pytest-black >= 0.3.7; python_implementation != \"PyPy\"", # workaround for jaraco/skeleton#22
+    'pytest-black >= 0.3.7; python_implementation != "PyPy"', # workaround for jaraco/skeleton#22
     "pytest-cov",
-    "pytest-mypy; python_implementation != \"PyPy\"", # workaround for jaraco/skeleton#22
+    'pytest-mypy; python_implementation != "PyPy"', # workaround for jaraco/skeleton#22
     "pytest-enabler >= 1.0.1",
     # local
     "jaraco.itertools",
     "func-timeout",
 ]
 docs = [
     # upstream
```

### Comparing `ini2toml-0.8/tests/examples/zipp/setup.cfg` & `ini2toml-0.9/tests/examples/zipp/setup.cfg`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/plugins/test_best_effort.py` & `ini2toml-0.9/tests/plugins/test_best_effort.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/plugins/test_coverage.py` & `ini2toml-0.9/tests/plugins/test_coverage.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/plugins/test_isort.py` & `ini2toml-0.9/tests/plugins/test_isort.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/plugins/test_mypy.py` & `ini2toml-0.9/tests/plugins/test_mypy.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/plugins/test_pytest.py` & `ini2toml-0.9/tests/plugins/test_pytest.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/plugins/test_setuptools_pep621.py` & `ini2toml-0.9/tests/plugins/test_setuptools_pep621.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 ]
 keywords = ["python", "module"]
 
 [options]
 zip-safe = false # comment
 package-dir = {"" = "src"}
 install-requires = [
-    "importlib-metadata; python_version<\\"3.8\\"",
+    'importlib-metadata; python_version<"3.8"',
     "configupdater>=3,<=4",
 ]
 
 [options.cmdclass]
 customcmd = "custom_build.CustomCmd"
 other = "custom_build.OtherCmd" # Some command
```

### Comparing `ini2toml-0.8/tests/test_cli.py` & `ini2toml-0.9/tests/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import sys
+from inspect import cleandoc
 from unittest.mock import MagicMock
 
 import pytest
 
 from ini2toml import cli
 from ini2toml.profile import Profile, ProfileAugmentation
 
@@ -98,7 +99,42 @@
     - ".isort.cfg": convert settings to 'pyproject.toml' equivalent.
     - "mypy.ini": convert settings to 'pyproject.toml' equivalent.
     - "pytest.ini": convert settings to 'pyproject.toml' ('ini_options' table).
     """
     expected = " ".join(x.strip() for x in expected_profile_desc.splitlines())
     print(out)
     assert expected in text
+
+
+def test_auto_formatting(tmp_path, capsys):
+    setupcfg = """
+    [metadata]
+    version = 42
+    name = myproj
+    """
+    normal_output = """
+    requires = ["setuptools"]
+    """
+    expected = """
+    requires = [
+      "setuptools",
+    ]
+    """
+
+    # Check if the underlying function works
+    formatted = cli.apply_auto_formatting(cleandoc(expected))
+    assert formatted.strip() == cleandoc(expected).strip()
+
+    (tmp_path / "setup.cfg").write_text(cleandoc(setupcfg), encoding="utf-8")
+    assert (tmp_path / "setup.cfg").exists()
+
+    # Check the output when formatting in off
+    cli.run([str(tmp_path / "setup.cfg")])
+    out, _ = capsys.readouterr()
+    assert cleandoc(normal_output) in out
+    assert cleandoc(expected) not in out
+
+    # Check the output when formatting in on
+    cli.run(["-F", str(tmp_path / "setup.cfg")])
+    out, _ = capsys.readouterr()
+    assert cleandoc(normal_output) not in out
+    assert cleandoc(expected) in out
```

### Comparing `ini2toml-0.8/tests/test_examples.py` & `ini2toml-0.9/tests/test_examples.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,17 +37,23 @@
 
 @pytest.mark.filterwarnings("ignore::DeprecationWarning")
 @pytest.mark.parametrize(("original", "expected"), list(examples()))
 def test_examples_api(original, expected, validate):
     translator = Translator()
     available_profiles = list(translator.profiles.keys())
     profile = cli.guess_profile(None, original, available_profiles)
-    out = translator.translate(Path(original).read_text(), profile)
-    expected_text = Path(expected).read_text().strip()
+    orig = Path(original)
+
+    # Make sure file ends in a newline (requirement for posix text files)
+    out = translator.translate(orig.read_text(encoding="utf-8"), profile)
+    assert out.endswith("\n")
+
+    expected_text = Path(expected).read_text(encoding="utf-8")
     assert out == expected_text
+
     # Make sure they can be parsed
     dict_equivalent = tomli.loads(out)
     assert dict_equivalent == tomli.loads(expected_text)
     assert validate(remove_deprecated(dict_equivalent)) is not None
 
 
 COMMENT_LINE = re.compile(r"^\s*#[^\n]*\n", re.M)
@@ -60,16 +66,21 @@
     opts = {"ini_loads_fn": configparser.parse, "toml_dumps_fn": lite_toml.convert}
     translator = Translator(**opts)
     available_profiles = list(translator.profiles.keys())
     profile = cli.guess_profile(None, original, available_profiles)
     # We cannot compare "flake8" sections (currently not handled)
     # (ConfigParser automatically strips comments, contrary to ConfigUpdater)
     orig = Path(original)
-    out = remove_flake8_from_toml(translator.translate(orig.read_text(), profile))
-    expected_text = remove_flake8_from_toml(Path(expected).read_text().strip())
+
+    # Make sure file ends in a newline (requirement for posix text files)
+    translated = translator.translate(orig.read_text(encoding="utf-8"), profile)
+    assert translated.endswith("\n")
+
+    out = remove_flake8_from_toml(translated)
+    expected_text = remove_flake8_from_toml(Path(expected).read_text(encoding="utf-8"))
 
     # At least the Python-equivalents should be the same when parsing
     dict_equivalent = tomli.loads(out)
     assert dict_equivalent == tomli.loads(expected_text)
     assert validate(remove_deprecated(dict_equivalent)) is not None
 
     without_comments = COMMENT_LINE.sub("", expected_text)
@@ -83,16 +94,21 @@
 
 
 @pytest.mark.filterwarnings("ignore::DeprecationWarning")
 @pytest.mark.parametrize(("original", "expected"), list(examples()))
 def test_examples_cli(original, expected, capsys):
     cli.run([original])
     (out, err) = capsys.readouterr()
-    expected_text = Path(expected).read_text().strip()
+
+    # Make sure file ends in a newline (requirement for posix text files)
+    assert out.endswith("\n")
+
+    expected_text = Path(expected).read_text(encoding="utf-8")
     assert out == expected_text
+
     # Make sure they can be parsed
     assert tomli.loads(out) == tomli.loads(expected_text)
 
 
 def remove_flake8_from_toml(text: str) -> str:
     # full_toml should not change any formatting, just remove the
     # parts we don't want
```

### Comparing `ini2toml-0.8/tests/test_intermediate_repr.py` & `ini2toml-0.9/tests/test_intermediate_repr.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/test_plugins.py` & `ini2toml-0.9/tests/test_plugins.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,19 +24,23 @@
     # EntryPoint(name, value, group)
     entry = "mypkg.SOOOOO___fake___:activate"
     fake = EntryPoint("fake", entry, ENTRYPOINT_GROUP)
     with pytest.raises(ErrorLoadingPlugin):
         plugins.load_from_entry_point(fake)
 
 
+def is_entry_point(ep):
+    return all(hasattr(ep, attr) for attr in ("name", "load"))
+
+
 def test_iterate_entry_points():
     plugin_iter = plugins.iterate_entry_points()
     assert hasattr(plugin_iter, "__iter__")
     pluging_list = list(plugin_iter)
-    assert all([isinstance(e, EntryPoint) for e in pluging_list])
+    assert all([is_entry_point(e) for e in pluging_list])
     name_list = [e.name for e in pluging_list]
     for ext in EXISTING:
         assert ext in name_list
 
 
 def test_list_from_entry_points():
     # Should return a list with all the plugins registered in the entrypoints
```

### Comparing `ini2toml-0.8/tests/test_transformations.py` & `ini2toml-0.9/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tests/test_translator.py` & `ini2toml-0.9/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `ini2toml-0.8/tox.ini` & `ini2toml-0.9/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -11,52 +11,62 @@
 [testenv]
 description = Invoke pytest to run automated tests
 setenv =
     TOXINIDIR = {toxinidir}
 passenv =
     HOME
 extras =
-    testing
     all
+    testing
+    experimental
 # Overwrite dependency just while the latest version is not published:
 # deps =
 #    validate-pyproject @ git+https://github.com/abravalheri/validate-pyproject@main#egg=validate-pyproject
 commands =
     pytest {posargs}
 
 
+[testenv:lint]
+description = Perform static analysis and style checks
+skip_install = True
+deps = pre-commit
+passenv =
+    HOMEPATH
+    PROGRAMDATA
+commands =
+    pre-commit run --all-files {posargs:--show-diff-on-failure}
+
+
 [testenv:typecheck]
 description = Invoke mypy to typecheck the source code
 changedir = {toxinidir}
 passenv =
     TERM
     # ^ ensure colors
-deps =
-    mypy
 extras =
     typechecking
+deps =
+    mypy
 commands =
     python -m mypy {posargs:src}
 
 
 [testenv:{build,clean}]
 description =
     build: Build the package in isolation according to PEP517, see https://github.com/pypa/build
     clean: Remove old distribution files and temporary build artifacts (./build and ./dist)
-# NOTE: build is still experimental, please refer to the links for updates/issues
 # https://setuptools.pypa.io/en/stable/build_meta.html#how-to-use-it
-# https://github.com/pypa/pep517/issues/91
 skip_install = True
 changedir = {toxinidir}
 deps =
     build: build[virtualenv]
 commands =
-    clean: python -c 'from shutil import rmtree; rmtree("build", True); rmtree("dist", True)'
+    clean: python -c 'import shutil; [shutil.rmtree(p, True) for p in ("build", "dist", "docs/_build")]'
+    clean: python -c 'import pathlib, shutil; [shutil.rmtree(p, True) for p in pathlib.Path("src").glob("*.egg-info")]'
     build: python -m build {posargs}
-# By default `build` produces wheels, you can also explicitly use the flags `--sdist` and `--wheel`
 
 
 [testenv:{docs,doctests,linkcheck}]
 description =
     docs: Invoke sphinx-build to build the docs
     doctests: Invoke sphinx-build to run doctests
     linkcheck: Check for broken links in the documentation
@@ -83,8 +93,8 @@
 passenv =
     TWINE_USERNAME
     TWINE_PASSWORD
     TWINE_REPOSITORY
 deps = twine
 commands =
     python -m twine check dist/*
-    python -m twine upload {posargs:--repository testpypi} dist/*
+    python -m twine upload {posargs:--repository {env:TWINE_REPOSITORY:testpypi}} dist/*
```

