# Comparing `tmp/pluggy-1.3.0.tar.gz` & `tmp/pluggy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluggy-1.3.0.tar", last modified: Sat Aug 26 19:10:07 2023, max compression
+gzip compressed data, was "pluggy-1.4.0.tar", last modified: Wed Jan 24 13:45:05 2024, max compression
```

## Comparing `pluggy-1.3.0.tar` & `pluggy-1.4.0.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.999779 pluggy-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (999)      539 2023-08-26 19:09:48.000000 pluggy-1.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.975779 pluggy-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.987779 pluggy-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)     3625 2023-08-26 19:09:48.000000 pluggy-1.3.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (999)      884 2023-08-26 19:09:48.000000 pluggy-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)     1600 2023-08-26 19:09:48.000000 pluggy-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      221 2023-08-26 19:09:48.000000 pluggy-1.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (999)    18618 2023-08-26 19:09:48.000000 pluggy-1.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1110 2023-08-26 19:09:48.000000 pluggy-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      132 2023-08-26 19:09:48.000000 pluggy-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     4102 2023-08-26 19:10:06.999779 pluggy-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2827 2023-08-26 19:09:48.000000 pluggy-1.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (999)      855 2023-08-26 19:09:48.000000 pluggy-1.3.0/RELEASING.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.987779 pluggy-1.3.0/changelog/
--rw-r--r--   0 runner    (1001) docker     (999)     1662 2023-08-26 19:09:48.000000 pluggy-1.3.0/changelog/README.rst
--rw-r--r--   0 runner    (1001) docker     (999)      939 2023-08-26 19:09:48.000000 pluggy-1.3.0/changelog/_template.rst
--rw-r--r--   0 runner    (1001) docker     (999)       86 2023-08-26 19:09:48.000000 pluggy-1.3.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.987779 pluggy-1.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.979779 pluggy-1.3.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.987779 pluggy-1.3.0/docs/_static/img/
--rw-r--r--   0 runner    (1001) docker     (999)     9350 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/_static/img/plug.png
--rw-r--r--   0 runner    (1001) docker     (999)      858 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (999)       30 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (999)     3855 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.987779 pluggy-1.3.0/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.987779 pluggy-1.3.0/docs/examples/eggsample/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.991779 pluggy-1.3.0/docs/examples/eggsample/eggsample/
--rw-r--r--   0 runner    (1001) docker     (999)      139 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/examples/eggsample/eggsample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      512 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/examples/eggsample/eggsample/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (999)     1578 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/examples/eggsample/eggsample/host.py
--rw-r--r--   0 runner    (1001) docker     (999)      335 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/examples/eggsample/eggsample/lib.py
--rw-r--r--   0 runner    (1001) docker     (999)      242 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/examples/eggsample/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.991779 pluggy-1.3.0/docs/examples/eggsample-spam/
--rw-r--r--   0 runner    (1001) docker     (999)      616 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/examples/eggsample-spam/eggsample_spam.py
--rw-r--r--   0 runner    (1001) docker     (999)      194 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/examples/eggsample-spam/setup.py
--rw-r--r--   0 runner    (1001) docker     (999)      887 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/examples/toy-example.py
--rw-r--r--   0 runner    (1001) docker     (999)    32810 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)      111 2023-08-26 19:09:48.000000 pluggy-1.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.995779 pluggy-1.3.0/downstream/
--rw-r--r--   0 runner    (1001) docker     (999)       51 2023-08-26 19:09:48.000000 pluggy-1.3.0/downstream/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)      107 2023-08-26 19:09:48.000000 pluggy-1.3.0/downstream/README.md
--rwxr-xr-x   0 runner    (1001) docker     (999)      255 2023-08-26 19:09:48.000000 pluggy-1.3.0/downstream/conda.sh
--rwxr-xr-x   0 runner    (1001) docker     (999)      244 2023-08-26 19:09:48.000000 pluggy-1.3.0/downstream/datasette.sh
--rwxr-xr-x   0 runner    (1001) docker     (999)      317 2023-08-26 19:09:48.000000 pluggy-1.3.0/downstream/devpi.sh
--rwxr-xr-x   0 runner    (1001) docker     (999)      245 2023-08-26 19:09:48.000000 pluggy-1.3.0/downstream/hatch.sh
--rwxr-xr-x   0 runner    (1001) docker     (999)      242 2023-08-26 19:09:48.000000 pluggy-1.3.0/downstream/pytest.sh
--rwxr-xr-x   0 runner    (1001) docker     (999)      221 2023-08-26 19:09:48.000000 pluggy-1.3.0/downstream/tox.sh
--rw-r--r--   0 runner    (1001) docker     (999)     1609 2023-08-26 19:09:48.000000 pluggy-1.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.995779 pluggy-1.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (999)     1996 2023-08-26 19:09:48.000000 pluggy-1.3.0/scripts/release.py
--rw-r--r--   0 runner    (1001) docker     (999)      428 2023-08-26 19:09:48.000000 pluggy-1.3.0/scripts/towncrier-draft-to-file.py
--rwxr-xr-x   0 runner    (1001) docker     (999)      423 2023-08-26 19:09:48.000000 pluggy-1.3.0/scripts/upload-coverage.sh
--rw-r--r--   0 runner    (1001) docker     (999)     1334 2023-08-26 19:10:06.999779 pluggy-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      124 2023-08-26 19:09:48.000000 pluggy-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.979779 pluggy-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.995779 pluggy-1.3.0/src/pluggy/
--rw-r--r--   0 runner    (1001) docker     (999)      714 2023-08-26 19:09:48.000000 pluggy-1.3.0/src/pluggy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6233 2023-08-26 19:09:48.000000 pluggy-1.3.0/src/pluggy/_callers.py
--rw-r--r--   0 runner    (1001) docker     (999)    23877 2023-08-26 19:09:48.000000 pluggy-1.3.0/src/pluggy/_hooks.py
--rw-r--r--   0 runner    (1001) docker     (999)    19517 2023-08-26 19:09:48.000000 pluggy-1.3.0/src/pluggy/_manager.py
--rw-r--r--   0 runner    (1001) docker     (999)     3238 2023-08-26 19:09:48.000000 pluggy-1.3.0/src/pluggy/_result.py
--rw-r--r--   0 runner    (1001) docker     (999)     2088 2023-08-26 19:09:48.000000 pluggy-1.3.0/src/pluggy/_tracing.py
--rw-r--r--   0 runner    (1001) docker     (999)      160 2023-08-26 19:10:06.000000 pluggy-1.3.0/src/pluggy/_version.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-26 19:09:48.000000 pluggy-1.3.0/src/pluggy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.995779 pluggy-1.3.0/src/pluggy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     4102 2023-08-26 19:10:06.000000 pluggy-1.3.0/src/pluggy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1506 2023-08-26 19:10:06.000000 pluggy-1.3.0/src/pluggy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-26 19:10:06.000000 pluggy-1.3.0/src/pluggy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       57 2023-08-26 19:10:06.000000 pluggy-1.3.0/src/pluggy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        7 2023-08-26 19:10:06.000000 pluggy-1.3.0/src/pluggy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 19:10:06.999779 pluggy-1.3.0/testing/
--rw-r--r--   0 runner    (1001) docker     (999)     2540 2023-08-26 19:09:48.000000 pluggy-1.3.0/testing/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (999)      549 2023-08-26 19:09:48.000000 pluggy-1.3.0/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (999)     4388 2023-08-26 19:09:48.000000 pluggy-1.3.0/testing/test_details.py
--rw-r--r--   0 runner    (1001) docker     (999)     2432 2023-08-26 19:09:48.000000 pluggy-1.3.0/testing/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (999)    10501 2023-08-26 19:09:48.000000 pluggy-1.3.0/testing/test_hookcaller.py
--rw-r--r--   0 runner    (1001) docker     (999)     7958 2023-08-26 19:09:48.000000 pluggy-1.3.0/testing/test_invocations.py
--rw-r--r--   0 runner    (1001) docker     (999)     9868 2023-08-26 19:09:48.000000 pluggy-1.3.0/testing/test_multicall.py
--rw-r--r--   0 runner    (1001) docker     (999)    16052 2023-08-26 19:09:48.000000 pluggy-1.3.0/testing/test_pluginmanager.py
--rw-r--r--   0 runner    (1001) docker     (999)     1900 2023-08-26 19:09:48.000000 pluggy-1.3.0/testing/test_tracer.py
--rw-r--r--   0 runner    (1001) docker     (999)     1351 2023-08-26 19:09:48.000000 pluggy-1.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.854347 pluggy-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-01-24 13:44:57.000000 pluggy-1.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.838347 pluggy-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.846347 pluggy-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-01-24 13:44:57.000000 pluggy-1.4.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-01-24 13:44:57.000000 pluggy-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-01-24 13:44:57.000000 pluggy-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-24 13:44:57.000000 pluggy-1.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19539 2024-01-24 13:44:57.000000 pluggy-1.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-01-24 13:44:57.000000 pluggy-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-24 13:44:57.000000 pluggy-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-01-24 13:45:05.854347 pluggy-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-01-24 13:44:57.000000 pluggy-1.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-01-24 13:44:57.000000 pluggy-1.4.0/RELEASING.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.846347 pluggy-1.4.0/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-01-24 13:44:57.000000 pluggy-1.4.0/changelog/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-01-24 13:44:57.000000 pluggy-1.4.0/changelog/_template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-24 13:44:57.000000 pluggy-1.4.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.846347 pluggy-1.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.842347 pluggy-1.4.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.846347 pluggy-1.4.0/docs/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/_static/img/plug.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.846347 pluggy-1.4.0/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.846347 pluggy-1.4.0/docs/examples/eggsample/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.846347 pluggy-1.4.0/docs/examples/eggsample/eggsample/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/examples/eggsample/eggsample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/examples/eggsample/eggsample/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/examples/eggsample/eggsample/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/examples/eggsample/eggsample/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/examples/eggsample/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.846347 pluggy-1.4.0/docs/examples/eggsample-spam/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/examples/eggsample-spam/eggsample_spam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/examples/eggsample-spam/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/examples/toy-example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32809 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-24 13:44:57.000000 pluggy-1.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.850347 pluggy-1.4.0/downstream/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-24 13:44:57.000000 pluggy-1.4.0/downstream/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-24 13:44:57.000000 pluggy-1.4.0/downstream/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      255 2024-01-24 13:44:57.000000 pluggy-1.4.0/downstream/conda.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-01-24 13:44:57.000000 pluggy-1.4.0/downstream/datasette.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      317 2024-01-24 13:44:57.000000 pluggy-1.4.0/downstream/devpi.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-01-24 13:44:57.000000 pluggy-1.4.0/downstream/hatch.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-01-24 13:44:57.000000 pluggy-1.4.0/downstream/pytest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-01-24 13:44:57.000000 pluggy-1.4.0/downstream/tox.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-01-24 13:44:57.000000 pluggy-1.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.850347 pluggy-1.4.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-01-24 13:44:57.000000 pluggy-1.4.0/scripts/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-01-24 13:44:57.000000 pluggy-1.4.0/scripts/towncrier-draft-to-file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      423 2024-01-24 13:44:57.000000 pluggy-1.4.0/scripts/upload-coverage.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-01-24 13:45:05.854347 pluggy-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-24 13:44:57.000000 pluggy-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.842347 pluggy-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.850347 pluggy-1.4.0/src/pluggy/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-24 13:44:57.000000 pluggy-1.4.0/src/pluggy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-01-24 13:44:57.000000 pluggy-1.4.0/src/pluggy/_callers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24364 2024-01-24 13:44:57.000000 pluggy-1.4.0/src/pluggy/_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19936 2024-01-24 13:44:57.000000 pluggy-1.4.0/src/pluggy/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-01-24 13:44:57.000000 pluggy-1.4.0/src/pluggy/_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-24 13:44:57.000000 pluggy-1.4.0/src/pluggy/_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-24 13:45:05.000000 pluggy-1.4.0/src/pluggy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-01-24 13:44:57.000000 pluggy-1.4.0/src/pluggy/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 13:44:57.000000 pluggy-1.4.0/src/pluggy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.854347 pluggy-1.4.0/src/pluggy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-01-24 13:45:05.000000 pluggy-1.4.0/src/pluggy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-01-24 13:45:05.000000 pluggy-1.4.0/src/pluggy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 13:45:05.000000 pluggy-1.4.0/src/pluggy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-24 13:45:05.000000 pluggy-1.4.0/src/pluggy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-24 13:45:05.000000 pluggy-1.4.0/src/pluggy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 13:45:05.854347 pluggy-1.4.0/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-01-24 13:44:57.000000 pluggy-1.4.0/testing/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-01-24 13:44:57.000000 pluggy-1.4.0/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-01-24 13:44:57.000000 pluggy-1.4.0/testing/test_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-01-24 13:44:57.000000 pluggy-1.4.0/testing/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12077 2024-01-24 13:44:57.000000 pluggy-1.4.0/testing/test_hookcaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-01-24 13:44:57.000000 pluggy-1.4.0/testing/test_invocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9868 2024-01-24 13:44:57.000000 pluggy-1.4.0/testing/test_multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18247 2024-01-24 13:44:57.000000 pluggy-1.4.0/testing/test_pluginmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-01-24 13:44:57.000000 pluggy-1.4.0/testing/test_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-01-24 13:44:57.000000 pluggy-1.4.0/testing/test_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-01-24 13:44:57.000000 pluggy-1.4.0/tox.ini
```

### Comparing `pluggy-1.3.0/.coveragerc` & `pluggy-1.4.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/.github/workflows/main.yml` & `pluggy-1.4.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/.gitignore` & `pluggy-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/.pre-commit-config.yaml` & `pluggy-1.4.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 repos:
 -   repo: https://github.com/PyCQA/autoflake
-    rev: v2.2.0
+    rev: v2.2.1
     hooks:
     -   id: autoflake
         name: autoflake
         args: ["--in-place", "--remove-unused-variables", "--remove-all-unused-imports"]
         language: python
         files: \.py$
 -   repo: https://github.com/asottile/reorder-python-imports
-    rev: v3.10.0
+    rev: v3.12.0
     hooks:
     -   id: reorder-python-imports
         args: ['--application-directories=.:src', --py38-plus]
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v2.1.0
     hooks:
     -   id: trailing-whitespace
@@ -20,20 +20,20 @@
     -   id: flake8
         additional_dependencies: [flake8-typing-imports]
 -   repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
     -   id: rst-backticks
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.10.1
+    rev: v3.15.0
     hooks:
     -   id: pyupgrade
         args: [--py38-plus]
 -   repo: https://github.com/psf/black
-    rev: 23.7.0
+    rev: 23.12.1
     hooks:
     -   id: black
         args: [--safe, --quiet]
 -   repo: https://github.com/asottile/blacken-docs
     rev: 1.16.0
     hooks:
     -   id: blacken-docs
@@ -43,13 +43,13 @@
     -   id: rst
         name: rst
         entry: rst-lint --encoding utf-8
         files: ^(HOWTORELEASE.rst|README.rst)$
         language: python
         additional_dependencies: [pygments, restructuredtext_lint]
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.5.1
+    rev: v1.8.0
     hooks:
     -   id: mypy
         files: ^(src/|testing/)
         args: []
         additional_dependencies: [pytest]
```

### Comparing `pluggy-1.3.0/CHANGELOG.rst` & `pluggy-1.4.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,33 @@
     .. The 'changelog_towncrier_draft' tag is included by our 'tox -e docs',
        but not on readthedocs.
 
     .. include:: _changelog_towncrier_draft.rst
 
 .. towncrier release notes start
 
+pluggy 1.4.0 (2024-01-24)
+=========================
+
+Features
+--------
+
+- `#463 <https://github.com/pytest-dev/pluggy/issues/463>`_: A warning :class:`~pluggy.PluggyTeardownRaisedWarning` is now issued when an old-style hookwrapper raises an exception during teardown.
+  See the warning documentation for more details.
+
+- `#471 <https://github.com/pytest-dev/pluggy/issues/471>`_: Add :func:`PluginManager.unblock <pluggy.PluginManager.unblock>` method to unblock a plugin by plugin name.
+
+Bug Fixes
+---------
+
+- `#441 <https://github.com/pytest-dev/pluggy/issues/441>`_: Fix :func:`~pluggy.HookCaller.call_extra()` extra methods getting ordered before everything else in some circumstances. Regressed in pluggy 1.1.0.
+
+- `#438 <https://github.com/pytest-dev/pluggy/issues/438>`_: Fix plugins registering other plugins in a hook when the other plugins implement the same hook itself. Regressed in pluggy 1.1.0.
+
+
 pluggy 1.3.0 (2023-08-26)
 =========================
 
 Deprecations and Removals
 -------------------------
 
 - `#426 <https://github.com/pytest-dev/pluggy/issues/426>`_: Python 3.7 is no longer supported.
@@ -144,25 +163,25 @@
 
 
 
 Features
 --------
 
 - `#282 <https://github.com/pytest-dev/pluggy/issues/282>`_: When registering a hookimpl which is declared as ``hookwrapper=True`` but whose
-  function is not a generator function, a ``PluggyValidationError`` exception is
+  function is not a generator function, a :class:`~pluggy.PluginValidationError` exception is
   now raised.
 
   Previously this problem would cause an error only later, when calling the hook.
 
   In the unlikely case that you have a hookwrapper that *returns* a generator
   instead of yielding directly, for example:
 
   .. code-block:: python
 
-      def my_hook_real_implementation(arg):
+      def my_hook_implementation(arg):
           print("before")
           yield
           print("after")
 
 
       @hookimpl(hookwrapper=True)
       def my_hook(arg):
```

### Comparing `pluggy-1.3.0/LICENSE` & `pluggy-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/PKG-INFO` & `pluggy-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluggy
-Version: 1.3.0
+Version: 1.4.0
 Summary: plugin and hook calling mechanisms for python
 Home-page: https://github.com/pytest-dev/pluggy
 Author: Holger Krekel
 Author-email: holger@merlinux.eu
 License: MIT
 Platform: unix
 Platform: linux
@@ -25,17 +25,21 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 Provides-Extra: testing
-License-File: LICENSE
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-benchmark; extra == "testing"
 
 ====================================================
 pluggy - A minimalist production ready plugin system
 ====================================================
 
 |pypi| |conda-forge| |versions| |github-actions| |gitter| |black| |codecov|
```

### Comparing `pluggy-1.3.0/README.rst` & `pluggy-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/RELEASING.rst` & `pluggy-1.4.0/RELEASING.rst`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/changelog/README.rst` & `pluggy-1.4.0/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/changelog/_template.rst` & `pluggy-1.4.0/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/docs/_static/img/plug.png` & `pluggy-1.4.0/docs/_static/img/plug.png`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/docs/conf.py` & `pluggy-1.4.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "logo": "img/plug.png",
     "description": "The pytest plugin system",
     "github_user": "pytest-dev",
     "github_repo": "pluggy",
     "github_button": "true",
     "github_banner": "true",
     "github_type": "star",
-    "badge_branch": "master",
+    "badge_branch": "main",
     "page_width": "1080px",
     "sidebar_width": "300px",
     "fixed_sidebar": "false",
 }
 html_sidebars = {
     "**": ["about.html", "localtoc.html", "relations.html", "searchbox.html"]
 }
```

### Comparing `pluggy-1.3.0/docs/examples/eggsample/eggsample/hookspecs.py` & `pluggy-1.4.0/docs/examples/eggsample/eggsample/hookspecs.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/docs/examples/eggsample/eggsample/host.py` & `pluggy-1.4.0/docs/examples/eggsample/eggsample/host.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/docs/examples/eggsample-spam/eggsample_spam.py` & `pluggy-1.4.0/docs/examples/eggsample-spam/eggsample_spam.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/docs/examples/toy-example.py` & `pluggy-1.4.0/docs/examples/toy-example.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/docs/index.rst` & `pluggy-1.4.0/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -412,17 +412,19 @@
             return result
 
 The generator is :py:meth:`sent <python:generator.send>` the return value
 of the hook thus far, or, if the previous calls raised an exception, it is
 :py:meth:`thrown <python:generator.throw>` the exception.
 
 The function should do one of two things:
-- Return a value, which can be the same value as received from the ``yield``, or
-something else entirely.
+
+- Return a value, which can be the same value as received from the ``yield``, or something else entirely.
+
 - Raise an exception.
+
 The return value or exception propagate to further hook wrappers, and finally
 to the hook caller.
 
 Also see the :ref:`pytest:hookwrapper` section in the ``pytest`` docs.
 
 .. _old_style_hookwrappers:
 
@@ -1024,19 +1026,19 @@
 .. _publish-subscribe:
     https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern
 .. _hooking:
     https://en.wikipedia.org/wiki/Hooking
 .. _callbacks:
     https://en.wikipedia.org/wiki/Callback_(computer_programming)
 .. _tox test suite:
-    https://github.com/pytest-dev/pluggy/blob/master/tox.ini
+    https://github.com/pytest-dev/pluggy/blob/main/tox.ini
 .. _Semantic Versioning:
     https://semver.org/
 .. _Python interpreters:
-    https://github.com/pytest-dev/pluggy/blob/master/tox.ini#L2
+    https://github.com/pytest-dev/pluggy/blob/main/tox.ini#L2
 .. _500+ plugins:
     https://docs.pytest.org/en/latest/reference/plugin_list.html
 .. _pre-commit:
     https://pre-commit.com/
 
 
 .. Indices and tables
```

### Comparing `pluggy-1.3.0/pyproject.toml` & `pluggy-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/scripts/release.py` & `pluggy-1.4.0/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/setup.cfg` & `pluggy-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/src/pluggy/__init__.py` & `pluggy-1.4.0/src/pluggy/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,20 +14,26 @@
     "HookspecOpts",
     "HookimplOpts",
     "HookImpl",
     "HookRelay",
     "HookspecMarker",
     "HookimplMarker",
     "Result",
+    "PluggyWarning",
+    "PluggyTeardownRaisedWarning",
 ]
 
 from ._manager import PluginManager, PluginValidationError
 from ._result import HookCallError, Result
 from ._hooks import (
     HookspecMarker,
     HookimplMarker,
     HookCaller,
     HookRelay,
     HookspecOpts,
     HookimplOpts,
     HookImpl,
 )
+from ._warnings import (
+    PluggyWarning,
+    PluggyTeardownRaisedWarning,
+)
```

### Comparing `pluggy-1.3.0/src/pluggy/_callers.py` & `pluggy-1.4.0/src/pluggy/_callers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,58 @@
 """
 Call loop machinery
 """
 from __future__ import annotations
 
+import warnings
 from typing import cast
 from typing import Generator
 from typing import Mapping
+from typing import NoReturn
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
 from ._hooks import HookImpl
-from ._result import _raise_wrapfail
 from ._result import HookCallError
 from ._result import Result
+from ._warnings import PluggyTeardownRaisedWarning
 
 
 # Need to distinguish between old- and new-style hook wrappers.
-# Wrapping one a singleton tuple is the fastest type-safe way I found to do it.
+# Wrapping with a tuple is the fastest type-safe way I found to do it.
 Teardown = Union[
-    Tuple[Generator[None, Result[object], None]],
+    Tuple[Generator[None, Result[object], None], HookImpl],
     Generator[None, object, object],
 ]
 
 
+def _raise_wrapfail(
+    wrap_controller: (
+        Generator[None, Result[object], None] | Generator[None, object, object]
+    ),
+    msg: str,
+) -> NoReturn:
+    co = wrap_controller.gi_code
+    raise RuntimeError(
+        "wrap_controller at %r %s:%d %s"
+        % (co.co_name, co.co_filename, co.co_firstlineno, msg)
+    )
+
+
+def _warn_teardown_exception(
+    hook_name: str, hook_impl: HookImpl, e: BaseException
+) -> None:
+    msg = "A plugin raised an exception during an old-style hookwrapper teardown.\n"
+    msg += f"Plugin: {hook_impl.plugin_name}, Hook: {hook_name}\n"
+    msg += f"{type(e).__name__}: {e}\n"
+    msg += "For more information see https://pluggy.readthedocs.io/en/stable/api_reference.html#pluggy.PluggyTeardownRaisedWarning"  # noqa: E501
+    warnings.warn(PluggyTeardownRaisedWarning(msg), stacklevel=5)
+
+
 def _multicall(
     hook_name: str,
     hook_impls: Sequence[HookImpl],
     caller_kwargs: Mapping[str, object],
     firstresult: bool,
 ) -> object | list[object]:
     """Execute a call into multiple python functions/methods and return the
@@ -56,15 +81,15 @@
                     only_new_style_wrappers = False
                     try:
                         # If this cast is not valid, a type error is raised below,
                         # which is the desired response.
                         res = hook_impl.function(*args)
                         wrapper_gen = cast(Generator[None, Result[object], None], res)
                         next(wrapper_gen)  # first yield
-                        teardowns.append((wrapper_gen,))
+                        teardowns.append((wrapper_gen, hook_impl))
                     except StopIteration:
                         _raise_wrapfail(wrapper_gen, "did not yield")
                 elif hook_impl.wrapper:
                     try:
                         # If this cast is not valid, a type error is raised below,
                         # which is the desired response.
                         res = hook_impl.function(*args)
@@ -124,17 +149,21 @@
                 outcome = Result(results, exception)
 
             # run all wrapper post-yield blocks
             for teardown in reversed(teardowns):
                 if isinstance(teardown, tuple):
                     try:
                         teardown[0].send(outcome)
-                        _raise_wrapfail(teardown[0], "has second yield")
                     except StopIteration:
                         pass
+                    except BaseException as e:
+                        _warn_teardown_exception(hook_name, teardown[1], e)
+                        raise
+                    else:
+                        _raise_wrapfail(teardown[0], "has second yield")
                 else:
                     try:
                         if outcome._exception is not None:
                             teardown.throw(outcome._exception)
                         else:
                             teardown.send(outcome._result)
                         # Following is unreachable for a well behaved hook wrapper.
```

### Comparing `pluggy-1.3.0/src/pluggy/_hooks.py` & `pluggy-1.4.0/src/pluggy/_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,14 +385,21 @@
         specmodule_or_class: _Namespace | None = None,
         spec_opts: HookspecOpts | None = None,
     ) -> None:
         """:meta private:"""
         #: Name of the hook getting called.
         self.name: Final = name
         self._hookexec: Final = hook_execute
+        # The hookimpls list. The caller iterates it *in reverse*. Format:
+        # 1. trylast nonwrappers
+        # 2. nonwrappers
+        # 3. tryfirst nonwrappers
+        # 4. trylast wrappers
+        # 5. wrappers
+        # 6. tryfirst wrappers
         self._hookimpls: Final[list[HookImpl]] = []
         self._call_history: _CallHistory | None = None
         # TODO: Document, or make private.
         self.spec: HookSpec | None = None
         if specmodule_or_class is not None:
             assert spec_opts is not None
             self.set_specification(specmodule_or_class, spec_opts)
@@ -486,15 +493,16 @@
         :ref:`calling`.
         """
         assert (
             not self.is_historic()
         ), "Cannot directly call a historic hook - use call_historic instead."
         self._verify_all_args_are_provided(kwargs)
         firstresult = self.spec.opts.get("firstresult", False) if self.spec else False
-        return self._hookexec(self.name, self._hookimpls, kwargs, firstresult)
+        # Copy because plugins may register other plugins during iteration (#438).
+        return self._hookexec(self.name, self._hookimpls.copy(), kwargs, firstresult)
 
     def call_historic(
         self,
         result_callback: Callable[[Any], None] | None = None,
         kwargs: Mapping[str, object] | None = None,
     ) -> None:
         """Call the hook with given ``kwargs`` for all registered plugins and
@@ -507,15 +515,16 @@
         """
         assert self._call_history is not None
         kwargs = kwargs or {}
         self._verify_all_args_are_provided(kwargs)
         self._call_history.append((kwargs, result_callback))
         # Historizing hooks don't return results.
         # Remember firstresult isn't compatible with historic.
-        res = self._hookexec(self.name, self._hookimpls, kwargs, False)
+        # Copy because plugins may register other plugins during iteration (#438).
+        res = self._hookexec(self.name, self._hookimpls.copy(), kwargs, False)
         if result_callback is None:
             return
         if isinstance(res, list):
             for x in res:
                 result_callback(x)
 
     def call_extra(
@@ -537,18 +546,19 @@
             "specname": None,
         }
         hookimpls = self._hookimpls.copy()
         for method in methods:
             hookimpl = HookImpl(None, "<temp>", method, opts)
             # Find last non-tryfirst nonwrapper method.
             i = len(hookimpls) - 1
-            while (
-                i >= 0
-                and hookimpls[i].tryfirst
-                and not (hookimpls[i].hookwrapper or hookimpls[i].wrapper)
+            while i >= 0 and (
+                # Skip wrappers.
+                (hookimpls[i].hookwrapper or hookimpls[i].wrapper)
+                # Skip tryfirst nonwrappers.
+                or hookimpls[i].tryfirst
             ):
                 i -= 1
             hookimpls.insert(i + 1, hookimpl)
         firstresult = self.spec.opts.get("firstresult", False) if self.spec else False
         return self._hookexec(self.name, hookimpls, kwargs, firstresult)
 
     def _maybe_apply_history(self, method: HookImpl) -> None:
```

### Comparing `pluggy-1.3.0/src/pluggy/_manager.py` & `pluggy-1.4.0/src/pluggy/_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
-import importlib.metadata
 import inspect
 import types
 import warnings
 from typing import Any
 from typing import Callable
 from typing import cast
 from typing import Final
 from typing import Iterable
 from typing import Mapping
 from typing import Sequence
+from typing import TYPE_CHECKING
 
 from . import _tracing
 from ._callers import _multicall
 from ._hooks import _HookImplFunction
 from ._hooks import _Namespace
 from ._hooks import _Plugin
 from ._hooks import _SubsetHookCaller
@@ -22,14 +22,18 @@
 from ._hooks import HookImpl
 from ._hooks import HookimplOpts
 from ._hooks import HookRelay
 from ._hooks import HookspecOpts
 from ._hooks import normalize_hookimpl_opts
 from ._result import Result
 
+if TYPE_CHECKING:
+    # importtlib.metadata import is slow, defer it.
+    import importlib.metadata
+
 
 _BeforeTrace = Callable[[str, Sequence[HookImpl], Mapping[str, Any]], None]
 _AfterTrace = Callable[[Result[Any], str, Sequence[HookImpl], Mapping[str, Any]], None]
 
 
 def _warn_for_function(warning: Warning, function: Callable[..., object]) -> None:
     func = cast(types.FunctionType, function)
@@ -227,14 +231,24 @@
         self.unregister(name=name)
         self._name2plugin[name] = None
 
     def is_blocked(self, name: str) -> bool:
         """Return whether the given plugin name is blocked."""
         return name in self._name2plugin and self._name2plugin[name] is None
 
+    def unblock(self, name: str) -> bool:
+        """Unblocks a name.
+
+        Returns whether the name was actually blocked.
+        """
+        if self._name2plugin.get(name, -1) is None:
+            del self._name2plugin[name]
+            return True
+        return False
+
     def add_hookspecs(self, module_or_class: _Namespace) -> None:
         """Add new hook specifications defined in the given ``module_or_class``.
 
         Functions are recognized as hook specifications if they have been
         decorated with a matching :class:`HookspecMarker`.
         """
         names = []
@@ -380,14 +394,16 @@
             Entry point group to load plugins.
         :param name:
             If given, loads only plugins with the given ``name``.
 
         :return:
             The number of plugins loaded by this call.
         """
+        import importlib.metadata
+
         count = 0
         for dist in list(importlib.metadata.distributions()):
             for ep in dist.entry_points:
                 if (
                     ep.group != group
                     or (name is not None and ep.name != name)
                     # already registered
```

### Comparing `pluggy-1.3.0/src/pluggy/_result.py` & `pluggy-1.4.0/src/pluggy/_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,40 +3,25 @@
 """
 from __future__ import annotations
 
 from types import TracebackType
 from typing import Callable
 from typing import cast
 from typing import final
-from typing import Generator
 from typing import Generic
-from typing import NoReturn
 from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import TypeVar
 
 
 _ExcInfo = Tuple[Type[BaseException], BaseException, Optional[TracebackType]]
 ResultType = TypeVar("ResultType")
 
 
-def _raise_wrapfail(
-    wrap_controller: (
-        Generator[None, Result[ResultType], None] | Generator[None, object, object]
-    ),
-    msg: str,
-) -> NoReturn:
-    co = wrap_controller.gi_code
-    raise RuntimeError(
-        "wrap_controller at %r %s:%d %s"
-        % (co.co_name, co.co_filename, co.co_firstlineno, msg)
-    )
-
-
 class HookCallError(Exception):
     """Hook was called incorrectly."""
 
 
 @final
 class Result(Generic[ResultType]):
     """An object used to inspect and set the result in a :ref:`hook wrapper
```

### Comparing `pluggy-1.3.0/src/pluggy/_tracing.py` & `pluggy-1.4.0/src/pluggy/_tracing.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/src/pluggy.egg-info/PKG-INFO` & `pluggy-1.4.0/src/pluggy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluggy
-Version: 1.3.0
+Version: 1.4.0
 Summary: plugin and hook calling mechanisms for python
 Home-page: https://github.com/pytest-dev/pluggy
 Author: Holger Krekel
 Author-email: holger@merlinux.eu
 License: MIT
 Platform: unix
 Platform: linux
@@ -25,17 +25,21 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 Provides-Extra: testing
-License-File: LICENSE
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-benchmark; extra == "testing"
 
 ====================================================
 pluggy - A minimalist production ready plugin system
 ====================================================
 
 |pypi| |conda-forge| |versions| |github-actions| |gitter| |black| |codecov|
```

### Comparing `pluggy-1.3.0/src/pluggy.egg-info/SOURCES.txt` & `pluggy-1.4.0/src/pluggy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -43,22 +43,24 @@
 src/pluggy/__init__.py
 src/pluggy/_callers.py
 src/pluggy/_hooks.py
 src/pluggy/_manager.py
 src/pluggy/_result.py
 src/pluggy/_tracing.py
 src/pluggy/_version.py
+src/pluggy/_warnings.py
 src/pluggy/py.typed
 src/pluggy.egg-info/PKG-INFO
 src/pluggy.egg-info/SOURCES.txt
 src/pluggy.egg-info/dependency_links.txt
 src/pluggy.egg-info/requires.txt
 src/pluggy.egg-info/top_level.txt
 testing/benchmark.py
 testing/conftest.py
 testing/test_details.py
 testing/test_helpers.py
 testing/test_hookcaller.py
 testing/test_invocations.py
 testing/test_multicall.py
 testing/test_pluginmanager.py
-testing/test_tracer.py
+testing/test_tracer.py
+testing/test_warnings.py
```

### Comparing `pluggy-1.3.0/testing/benchmark.py` & `pluggy-1.4.0/testing/benchmark.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/testing/conftest.py` & `pluggy-1.4.0/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/testing/test_details.py` & `pluggy-1.4.0/testing/test_details.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/testing/test_helpers.py` & `pluggy-1.4.0/testing/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/testing/test_hookcaller.py` & `pluggy-1.4.0/testing/test_hookcaller.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Callable
+from typing import Generator
 from typing import List
 from typing import Sequence
 from typing import TypeVar
 
 import pytest
 
 from pluggy import HookimplMarker
@@ -444,7 +445,78 @@
     pm.add_hookspecs(Api1)
     with pytest.raises(ValueError) as exc:
         pm.add_hookspecs(Api2)
     assert str(exc.value) == (
         "Hook 'conflict' is already registered within namespace "
         "<class 'test_hookcaller.test_hook_conflict.<locals>.Api1'>"
     )
+
+
+def test_call_extra_hook_order(hc: HookCaller, addmeth: AddMeth) -> None:
+    """Ensure that call_extra is calling hooks in the right order."""
+    order = []
+
+    @addmeth(tryfirst=True)
+    def method1() -> str:
+        order.append("1")
+        return "1"
+
+    @addmeth()
+    def method2() -> str:
+        order.append("2")
+        return "2"
+
+    @addmeth(trylast=True)
+    def method3() -> str:
+        order.append("3")
+        return "3"
+
+    @addmeth(wrapper=True, tryfirst=True)
+    def method4() -> Generator[None, str, str]:
+        order.append("4pre")
+        result = yield
+        order.append("4post")
+        return result
+
+    @addmeth(wrapper=True)
+    def method5() -> Generator[None, str, str]:
+        order.append("5pre")
+        result = yield
+        order.append("5post")
+        return result
+
+    @addmeth(wrapper=True, trylast=True)
+    def method6() -> Generator[None, str, str]:
+        order.append("6pre")
+        result = yield
+        order.append("6post")
+        return result
+
+    def extra1() -> str:
+        order.append("extra1")
+        return "extra1"
+
+    def extra2() -> str:
+        order.append("extra2")
+        return "extra2"
+
+    result = hc.call_extra([extra1, extra2], {"arg": "test"})
+    assert order == [
+        "4pre",
+        "5pre",
+        "6pre",
+        "1",
+        "extra2",
+        "extra1",
+        "2",
+        "3",
+        "6post",
+        "5post",
+        "4post",
+    ]
+    assert result == [
+        "1",
+        "extra2",
+        "extra1",
+        "2",
+        "3",
+    ]
```

### Comparing `pluggy-1.3.0/testing/test_invocations.py` & `pluggy-1.4.0/testing/test_invocations.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/testing/test_multicall.py` & `pluggy-1.4.0/testing/test_multicall.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/testing/test_pluginmanager.py` & `pluggy-1.4.0/testing/test_pluginmanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,21 @@
 
     pm.set_blocked("somename")
     assert pm.is_blocked("somename")
     assert not pm.register(A(), "somename")
     pm.unregister(name="somename")
     assert pm.is_blocked("somename")
 
+    # Unblock.
+    assert not pm.unblock("someothername")
+    assert pm.unblock("somename")
+    assert not pm.is_blocked("somename")
+    assert not pm.unblock("somename")
+    assert pm.register(A(), "somename")
+
 
 def test_register_mismatch_method(he_pm: PluginManager) -> None:
     class hello:
         @hookimpl
         def he_method_notexists(self):
             pass
 
@@ -671,7 +678,83 @@
 
         with pytest.raises(ValueError):
             he_pm.hook.he_method1(arg=1)
         assert he_pm.trace.root.indent == indent
         assert saveindent[0] > indent
     finally:
         undo()
+
+
+@pytest.mark.parametrize("historic", [False, True])
+def test_register_while_calling(
+    pm: PluginManager,
+    historic: bool,
+) -> None:
+    """Test that registering an impl of a hook while it is being called does
+    not affect the call itself, only later calls.
+
+    For historic hooks however, the hook is called immediately on registration.
+
+    Regression test for #438.
+    """
+    hookspec = HookspecMarker("example")
+
+    class Hooks:
+        @hookspec(historic=historic)
+        def configure(self) -> int:
+            raise NotImplementedError()
+
+    class Plugin1:
+        @hookimpl
+        def configure(self) -> int:
+            return 1
+
+    class Plugin2:
+        def __init__(self) -> None:
+            self.already_registered = False
+
+        @hookimpl
+        def configure(self) -> int:
+            if not self.already_registered:
+                pm.register(Plugin4())
+                pm.register(Plugin5())
+                pm.register(Plugin6())
+                self.already_registered = True
+            return 2
+
+    class Plugin3:
+        @hookimpl
+        def configure(self) -> int:
+            return 3
+
+    class Plugin4:
+        @hookimpl(tryfirst=True)
+        def configure(self) -> int:
+            return 4
+
+    class Plugin5:
+        @hookimpl()
+        def configure(self) -> int:
+            return 5
+
+    class Plugin6:
+        @hookimpl(trylast=True)
+        def configure(self) -> int:
+            return 6
+
+    pm.add_hookspecs(Hooks)
+    pm.register(Plugin1())
+    pm.register(Plugin2())
+    pm.register(Plugin3())
+
+    if not historic:
+        result = pm.hook.configure()
+        assert result == [3, 2, 1]
+        result = pm.hook.configure()
+        assert result == [4, 5, 3, 2, 1, 6]
+    else:
+        result = []
+        pm.hook.configure.call_historic(result.append)
+        assert result == [4, 5, 6, 3, 2, 1]
+        result = []
+        pm.hook.configure.call_historic(result.append)
+        assert result == [4, 5, 3, 2, 1, 6]
```

### Comparing `pluggy-1.3.0/testing/test_tracer.py` & `pluggy-1.4.0/testing/test_tracer.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.3.0/tox.ini` & `pluggy-1.4.0/tox.ini`

 * *Files identical despite different names*

