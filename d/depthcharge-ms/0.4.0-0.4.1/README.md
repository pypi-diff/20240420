# Comparing `tmp/depthcharge_ms-0.4.0.tar.gz` & `tmp/depthcharge_ms-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depthcharge_ms-0.4.0.tar", last modified: Wed Apr 17 20:34:40 2024, max compression
+gzip compressed data, was "depthcharge_ms-0.4.1.tar", last modified: Fri Apr 19 22:23:28 2024, max compression
```

## Comparing `depthcharge_ms-0.4.0.tar` & `depthcharge_ms-0.4.1.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.511023 depthcharge_ms-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.515023 depthcharge_ms-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.515023 depthcharge_ms-0.4.0/data/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/data/TMT10-Trial-8.mgf
--rw-r--r--   0 runner    (1001) docker     (127)   333839 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/data/TMT10-Trial-8.mzML
--rw-r--r--   0 runner    (1001) docker     (127)    67798 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/data/TMT10-Trial-8.mzXML
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.519024 depthcharge_ms-0.4.0/depthcharge/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.519024 depthcharge_ms-0.4.0/depthcharge/data/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/analyte_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11974 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    18908 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18318 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/data/spectrum_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.519024 depthcharge_ms-0.4.0/depthcharge/encoders/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/encoders/sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/feedforward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.519024 depthcharge_ms-0.4.0/depthcharge/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/tokenizers/molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/tokenizers/peptides.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/tokenizers/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.519024 depthcharge_ms-0.4.0/depthcharge/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/transformers/analytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/transformers/spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/depthcharge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/depthcharge_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-17 20:34:40.000000 depthcharge_ms-0.4.0/depthcharge_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-17 20:34:40.000000 depthcharge_ms-0.4.0/depthcharge_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:34:40.000000 depthcharge_ms-0.4.0/depthcharge_ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-17 20:34:40.000000 depthcharge_ms-0.4.0/depthcharge_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 20:34:40.000000 depthcharge_ms-0.4.0/depthcharge_ms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.523023 depthcharge_ms-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.523023 depthcharge_ms-0.4.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/api/datasets.md
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/api/encoders.md
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/api/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/api/primitives.md
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/api/tokenizers.md
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/api/transformers.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.523023 depthcharge_ms-0.4.0/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.523023 depthcharge_ms-0.4.0/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.523023 depthcharge_ms-0.4.0/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    50058 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    46385 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/static/logo-light.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.523023 depthcharge_ms-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/tests/unit_tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_data/test_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_data/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_data/test_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/tests/unit_tests/test_encoders/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_encoders/test_sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_feedforward.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/tests/unit_tests/test_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_tokenizers/test_molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_tokenizers/test_peptides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:34:40.527024 depthcharge_ms-0.4.0/tests/unit_tests/test_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_transformers/test_analyte_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_transformers/test_spectrum_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-17 20:34:28.000000 depthcharge_ms-0.4.0/tests/unit_tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.142728 depthcharge_ms-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.126728 depthcharge_ms-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.130728 depthcharge_ms-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-19 22:23:28.142728 depthcharge_ms-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.130728 depthcharge_ms-0.4.1/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/data/TMT10-Trial-8.mgf
+-rw-r--r--   0 runner    (1001) docker     (127)   333839 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/data/TMT10-Trial-8.mzML
+-rw-r--r--   0 runner    (1001) docker     (127)    67798 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/data/TMT10-Trial-8.mzXML
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.130728 depthcharge_ms-0.4.1/depthcharge/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.134728 depthcharge_ms-0.4.1/depthcharge/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/analyte_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18919 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18401 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/spectrum_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.134728 depthcharge_ms-0.4.1/depthcharge/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/encoders/sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.134728 depthcharge_ms-0.4.1/depthcharge/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/tokenizers/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/tokenizers/peptides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/tokenizers/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.134728 depthcharge_ms-0.4.1/depthcharge/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/transformers/analytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/transformers/spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/depthcharge_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-19 22:23:28.000000 depthcharge_ms-0.4.1/depthcharge_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-19 22:23:28.000000 depthcharge_ms-0.4.1/depthcharge_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:23:28.000000 depthcharge_ms-0.4.1/depthcharge_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-19 22:23:28.000000 depthcharge_ms-0.4.1/depthcharge_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 22:23:28.000000 depthcharge_ms-0.4.1/depthcharge_ms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.134728 depthcharge_ms-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.134728 depthcharge_ms-0.4.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/api/datasets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/api/encoders.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/api/primitives.md
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/api/tokenizers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/api/transformers.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/getting-started/spectra.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:23:28.142728 depthcharge_ms-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    50058 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46385 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/static/logo-light.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/tests/unit_tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/tests/unit_tests/test_encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_encoders/test_sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/tests/unit_tests/test_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_tokenizers/test_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_tokenizers/test_peptides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/tests/unit_tests/test_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_transformers/test_analyte_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_transformers/test_spectrum_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_version.py
```

### Comparing `depthcharge_ms-0.4.0/.github/workflows/lint.yml` & `depthcharge_ms-0.4.1/.github/workflows/lint.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Lint
+name: Lint Code
 
 on:
   push:
     branches: [ main ]
   pull_request:
     branches: [ main ]
```

### Comparing `depthcharge_ms-0.4.0/CHANGELOG.md` & `depthcharge_ms-0.4.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v0.4.1]
+
+### Added
+- Significant updates to documentation. Add how to model mass spectra.
+- Reading and writing from cloud storage on everything!
+
+### Changed
+- Migrated to Mike for mkdocs to manage multiple versions.
+- Moved test GitHub Action from pip to uv.
+
 ## [v0.4.0]
 
 We have completely reworked of the data module.
 Depthcharge now uses Apache Arrow-based formats instead of HDF5; spectra are converted either Parquet or streamed with PyArrow, optionally into Lance datasets.
 
 We now also have full support for small molecules, with the `MoleculeTokenizer`,
 `AnalyteTransformerEncoder`, and `AnalyteTransformerDecoder` classes.
```

### Comparing `depthcharge_ms-0.4.0/CODE_OF_CONDUCT.md` & `depthcharge_ms-0.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/CONTRIBUTING.md` & `depthcharge_ms-0.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/LICENSE` & `depthcharge_ms-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/PKG-INFO` & `depthcharge_ms-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.4.0
+Version: 0.4.1
 Summary: A mass spectrometry toolkit for deep learning with Transformer models.
 Author-email: "William E. Fondrie" <fondriew@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/wfondrie/depthcharge
 Project-URL: Documentation, https://wfondrie.github.io/depthcharge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,13 +26,16 @@
 Requires-Dist: lark>=1.1.4
 Requires-Dist: selfies>=2.1.1
 Requires-Dist: sortedcontainers>=2.4.0
 Requires-Dist: dill>=0.3.6
 Requires-Dist: rdkit>=2023.03.1
 Requires-Dist: pillow>=9.4.0
 Requires-Dist: spectrum-utils>=0.4.1
+Requires-Dist: cloudpathlib>=0.18.1
 Provides-Extra: docs
+Requires-Dist: mike; extra == "docs"
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings[python]>=0.18; extra == "docs"
+Requires-Dist: mkquartodocs; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: pre-commit>=2.7.1; extra == "dev"
```

### Comparing `depthcharge_ms-0.4.0/README.md` & `depthcharge_ms-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/data/TMT10-Trial-8.mgf` & `depthcharge_ms-0.4.1/data/TMT10-Trial-8.mgf`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/data/TMT10-Trial-8.mzML` & `depthcharge_ms-0.4.1/data/TMT10-Trial-8.mzML`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/data/TMT10-Trial-8.mzXML` & `depthcharge_ms-0.4.1/data/TMT10-Trial-8.mzXML`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge/__init__.py` & `depthcharge_ms-0.4.1/depthcharge/__init__.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge/data/analyte_datasets.py` & `depthcharge_ms-0.4.1/depthcharge/data/analyte_datasets.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge/data/arrow.py` & `depthcharge_ms-0.4.1/depthcharge/data/arrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from collections.abc import Callable, Generator, Iterable
 from os import PathLike
 from pathlib import Path
 
 import polars as pl
 import pyarrow as pa
 import pyarrow.parquet as pq
+from cloudpathlib import AnyPath
 
 from .fields import CustomField
 from .parsers import ParserFactory
 
 
 def spectra_to_stream(
     peak_file: PathLike,
@@ -207,15 +208,15 @@
         preprocessing_fn=preprocessing_fn,
         valid_charge=valid_charge,
         custom_fields=custom_fields,
         progress=progress,
     )
 
     if parquet_file is None:
-        parquet_file = Path(Path(peak_file).stem).with_suffix(".parquet")
+        parquet_file = Path(AnyPath(peak_file).stem).with_suffix(".parquet")
 
     try:
         writer = None
         for batch in streamer:
             if writer is None:
                 writer = pq.ParquetWriter(parquet_file, schema=batch.schema)
 
@@ -287,16 +288,16 @@
     custom_fields : CustomField or iterable of CustomField
         Additional fields to extract during peak file parsing.
     progress : bool, optional
         Enable or disable the progress bar.
 
     Returns
     -------
-    Path
-        The Parquet file that was written.
+    polars.DataFrame
+        A dataframe containing the parsed mass spectra.
 
     """
     streamer = spectra_to_stream(
         peak_file=peak_file,
         batch_size=None,
         metadata_df=metadata_df,
         ms_level=ms_level,
```

### Comparing `depthcharge_ms-0.4.0/depthcharge/data/fields.py` & `depthcharge_ms-0.4.1/depthcharge/data/fields.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge/data/parsers.py` & `depthcharge_ms-0.4.1/depthcharge/data/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
 from collections.abc import Callable, Iterable
 from os import PathLike
-from pathlib import Path
 from typing import Any
 
 import pyarrow as pa
+from cloudpathlib import AnyPath
 from pyteomics.mgf import MGF
 from pyteomics.mzml import MzML
 from pyteomics.mzxml import MzXML
 from tqdm.auto import tqdm
 
 from .. import utils
 from ..primitives import MassSpectrum
@@ -55,15 +55,15 @@
         preprocessing_fn: Callable | Iterable[Callable] | None = None,
         valid_charge: Iterable[int] | None = None,
         custom_fields: dict[str, str | Iterable[str]] | None = None,
         progress: bool = True,
         id_type: str = "scan",
     ) -> None:
         """Initialize the BaseParser."""
-        self.peak_file = Path(peak_file)
+        self.peak_file = AnyPath(peak_file)
         self.progress = progress
         self.ms_level = (
             ms_level if ms_level is None else set(utils.listify(ms_level))
         )
 
         if preprocessing_fn is None:
             self.preprocessing_fn = [
```

### Comparing `depthcharge_ms-0.4.0/depthcharge/data/preprocessing.py` & `depthcharge_ms-0.4.1/depthcharge/data/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 import numpy as np
 
 from ..primitives import MassSpectrum
 
 
 def scale_to_unit_norm(spectrum: MassSpectrum) -> MassSpectrum:
     """Scale intensities to unit norm."""
-    spectrum._inner._intensity = (
+    spectrum.intensity = (
         spectrum.intensity / np.sqrt(spectrum.intensity**2).sum()
     )
     return spectrum
 
 
 def _spectrum_utils_fn(func: str) -> Callable:
     """Wrap spectrum_utils.spectrum.MmsmsSpectrum preprocessing methods."""
```

### Comparing `depthcharge_ms-0.4.0/depthcharge/data/spectrum_datasets.py` & `depthcharge_ms-0.4.1/depthcharge/data/spectrum_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import Any
 
 import lance
 import polars as pl
 import pyarrow as pa
 import pyarrow.parquet as pq
 import torch
+from cloudpathlib import AnyPath
 from lance.torch.data import LanceDataset
 from torch import nn
 from torch.utils.data import IterableDataset
 
 from .. import utils
 from ..tokenizers import PeptideTokenizer
 from . import arrow
@@ -89,33 +90,33 @@
         self._parse_kwargs = {} if parse_kwargs is None else parse_kwargs
         self._tmpdir = None
         if path is None:
             # Create a random temporary file:
             self._tmpdir = TemporaryDirectory()
             path = Path(self._tmpdir.name) / f"{uuid.uuid4()}.lance"
 
-        self._path = Path(path)
+        self._path = AnyPath(path)
         if self._path.suffix != ".lance":
             self._path = self._path.with_suffix(".lance")
 
         # Now parse spectra.
         if spectra is not None:
             spectra = utils.listify(spectra)
             batch = next(_get_records(spectra, **self._parse_kwargs))
             lance.write_dataset(
                 _get_records(spectra, **self._parse_kwargs),
-                self._path,
-                mode="overwrite",
+                str(self._path),
+                mode="overwrite" if self._path.exists() else "create",
                 schema=batch.schema,
             )
 
         elif not self._path.exists():
             raise ValueError("No spectra were provided")
 
-        self._dataset = lance.dataset(self._path)
+        self._dataset = lance.dataset(str(self._path))
         if "to_tensor_fn" not in kwargs:
             kwargs["to_tensor_fn"] = self._to_tensor
 
         super().__init__(self._dataset, batch_size, **kwargs)
 
     def add_spectra(
         self,
```

### Comparing `depthcharge_ms-0.4.0/depthcharge/encoders/sinusoidal.py` & `depthcharge_ms-0.4.1/depthcharge/encoders/sinusoidal.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge/feedforward.py` & `depthcharge_ms-0.4.1/depthcharge/feedforward.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge/mixins.py` & `depthcharge_ms-0.4.1/depthcharge/mixins.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge/primitives.py` & `depthcharge_ms-0.4.1/depthcharge/primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,14 +415,24 @@
             ".(raw|mzml|mzxml|mgf|d|wiff)$",
             "",
             fname,
             flags=re.IGNORECASE,
         )
         return ":".join([fname, index_type, scan])
 
+    @MsmsSpectrum.intensity.setter
+    def intensity(self, values):
+        """Set the intensity array."""
+        self._inner._intensity = values
+
+    @MsmsSpectrum.mz.setter
+    def mz(self, values):
+        """Set the m/z array."""
+        self._inner._mz = values
+
     @property
     def precursor_mass(self) -> float:
         """The monoisotopic mass."""
         return (self.precursor_mz - PROTON) * self.precursor_charge
 
     def to_tensor(self) -> torch.tensor:
         """Combine the m/z and intensity arrays into a single tensor.
```

### Comparing `depthcharge_ms-0.4.0/depthcharge/testing.py` & `depthcharge_ms-0.4.1/depthcharge/testing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge/tokenizers/molecules.py` & `depthcharge_ms-0.4.1/depthcharge/tokenizers/molecules.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge/tokenizers/peptides.py` & `depthcharge_ms-0.4.1/depthcharge/tokenizers/peptides.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge/tokenizers/tokenizer.py` & `depthcharge_ms-0.4.1/depthcharge/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge/transformers/analytes.py` & `depthcharge_ms-0.4.1/depthcharge/transformers/analytes.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge/transformers/spectra.py` & `depthcharge_ms-0.4.1/depthcharge/transformers/spectra.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge/utils.py` & `depthcharge_ms-0.4.1/depthcharge/utils.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/depthcharge_ms.egg-info/PKG-INFO` & `depthcharge_ms-0.4.1/depthcharge_ms.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.4.0
+Version: 0.4.1
 Summary: A mass spectrometry toolkit for deep learning with Transformer models.
 Author-email: "William E. Fondrie" <fondriew@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/wfondrie/depthcharge
 Project-URL: Documentation, https://wfondrie.github.io/depthcharge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,13 +26,16 @@
 Requires-Dist: lark>=1.1.4
 Requires-Dist: selfies>=2.1.1
 Requires-Dist: sortedcontainers>=2.4.0
 Requires-Dist: dill>=0.3.6
 Requires-Dist: rdkit>=2023.03.1
 Requires-Dist: pillow>=9.4.0
 Requires-Dist: spectrum-utils>=0.4.1
+Requires-Dist: cloudpathlib>=0.18.1
 Provides-Extra: docs
+Requires-Dist: mike; extra == "docs"
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings[python]>=0.18; extra == "docs"
+Requires-Dist: mkquartodocs; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: pre-commit>=2.7.1; extra == "dev"
```

### Comparing `depthcharge_ms-0.4.0/depthcharge_ms.egg-info/SOURCES.txt` & `depthcharge_ms-0.4.1/depthcharge_ms.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 docs/api/datasets.md
 docs/api/encoders.md
 docs/api/index.md
 docs/api/primitives.md
 docs/api/tokenizers.md
 docs/api/transformers.md
 docs/getting-started/installation.md
+docs/getting-started/spectra.qmd
 docs/stylesheets/extra.css
 static/icon.svg
 static/logo-dark.png
 static/logo-light.png
 tests/conftest.py
 tests/unit_tests/test_feedforward.py
 tests/unit_tests/test_primitives.py
```

### Comparing `depthcharge_ms-0.4.0/docs/CHANGELOG.md` & `depthcharge_ms-0.4.1/docs/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v0.4.1]
+
+### Added
+- Significant updates to documentation. Add how to model mass spectra.
+- Reading and writing from cloud storage on everything!
+
+### Changed
+- Migrated to Mike for mkdocs to manage multiple versions.
+- Moved test GitHub Action from pip to uv.
+
 ## [v0.4.0]
 
 We have completely reworked of the data module.
 Depthcharge now uses Apache Arrow-based formats instead of HDF5; spectra are converted either Parquet or streamed with PyArrow, optionally into Lance datasets.
 
 We now also have full support for small molecules, with the `MoleculeTokenizer`,
 `AnalyteTransformerEncoder`, and `AnalyteTransformerDecoder` classes.
```

### Comparing `depthcharge_ms-0.4.0/docs/CODE_OF_CONDUCT.md` & `depthcharge_ms-0.4.1/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/docs/CONTRIBUTING.md` & `depthcharge_ms-0.4.1/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/docs/api/index.md` & `depthcharge_ms-0.4.1/docs/api/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # The depthcharge Python API
 
-The depthcharge package provides utilities and classes to parse, store, and use mass spectra, peptides, and small molecules in Transformer models.
-Although depthcharge is primarly focused Transformers, many of these classes can be used as building blocks for models of your own choice.
-
+The depthcharge package provides utilities and classes to parse, store, and use mass spectra, peptides, and small molecules in PyTorch models.
+Although depthcharge is primarily focused on PyTorch Transformer modules as a starting point, many of these classes and utilities can be used as building blocks for models of your own choice.
 
 ## Tokenizers
 
 Tokenizers split string inputs into tokens, such as peptide sequences or SMILES strings, into the pieces that we want to model with our neural networks.
 For example, peptide sequences need to be broken into constituent amino acids, with or without modifications (the tokens).
 In addition to specifying how tokens are created, the tokenizer classes also aid in mass calculations that are useful for modeling mass spectrometry data.
 
 Tokenizers live in the [tokenizers submodule](tokenizers).
 
-## Datasets
+## Data
+
+Depthcharge provides several utilities for interacting with data such as mass spectra, small molecules and peptides.
+
+The [data submodule](datasets) contains functions for parsing and preprocessing mass spectra.
+It also contains dataset classes for loading data into models built with PyTorch.
 
 Datasets are subclasses of PyTorch Datasets, specifically designed to store and retrieve mass spectrometry data, including the mass spectra themselves and analyte representations.
 
-Datasets live in the [datasets submodule](datsets).
+Datasets and parsing functions live in the [data submodule](datasets).
 
 ## Encoders
 
 Often the most useful representation for an input is not the raw parsed format.
 In depthcharge, we provide a collection of sinusoidal encoders to represent general floating point numbers, positions in a sequence, and peaks in a mass spectrum.
 
 Encoders live in the [encoders submodule](encoders).
```

### Comparing `depthcharge_ms-0.4.0/docs/getting-started/installation.md` & `depthcharge_ms-0.4.1/docs/getting-started/installation.md`

 * *Files 23% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 See the [Miniconda documentation](https://docs.conda.io/en/latest/miniconda.html) for details.
 
 ### PyTorch (*optional*)
 Depthcharge creates PyTorch modules which you can use to create deep learning models for your application.
 PyTorch can be installed automatically during Depthcharge installation; however, to get the most out of Depthcharge and PyTorch, you'll likely want to install PyTorch manually to account for any GPUs and their drivers that you may have installed.
 To install PyTorch, follow the installation instructions found in the [PyTorch documentation](https://pytorch.org/get-started/locally/).
 
+### cloudpathlib (*optional*)
+Depthcharge can read data directly from cloud resources using [cloudpathlib](https://cloudpathlib.drivendata.org/stable/).
+However, by default the optional requirements for each cloud provider are not included.
+If you want to interact with cloud resources, install the relevant cloudpathlib optional dependencies as instructed in [cloudpathlib documentation](https://cloudpathlib.drivendata.org/stable/#installation)
 
 ## Install depthcharge
 
 Depthcharge can be install with `pip`, directly from PyPI:
 ```sh
 $ pip install depthcharge-ms
 ```
```

### Comparing `depthcharge_ms-0.4.0/docs/index.md` & `depthcharge_ms-0.4.1/docs/index.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ![depthcharge logo](./static/logo-dark.png#gh-dark-mode-only){: style="height:200px;display:block;margin-left:auto;margin-right:auto"}
 
-Depthcharge is a deep learning toolkit for building Transformer models to analyze mass spectrometry data.
+Depthcharge is a deep learning toolkit for building models to analyze mass spectrometry data.
 
 ## About
 
 Many deep learning tools have been developed for the analysis of mass spectra or mass spectrometry analytes, like peptides and small molecules.
 However, each one has had to reinvent the wheel.
 
-Depthcharge aims to provide a flexible, but opinionated, framework for rapidly prototyping deep learning models for mass spectrometry data.
+Depthcharge aims to provide a flexible, but opinionated, framework to rapidly prototype deep learning models for mass spectrometry data.
 Think of Depthcharge as a set of building blocks to get you started on a new deep learning project focused around mass spectrometry data.
 Depthcharge delivers these building blocks in the form of PyTorch modules, which can be readily used to assemble customized deep learning models for your task.
-
+With Depthcharge we aim to get users ~80% of the way to their ideal model in only a few hours, instead of requiring days or weeks to build and test models for different tasks.
 
 <style>
   .md-typeset h1 {
     visibility: hidden;
     font-size: 2px;
     margin: 0px;
   }
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
 ![depthcharge logo](./static/logo-dark.png#gh-dark-mode-only){: style="height:
 200px;display:block;margin-left:auto;margin-right:auto"} Depthcharge is a deep
-learning toolkit for building Transformer models to analyze mass spectrometry
-data. ## About Many deep learning tools have been developed for the analysis of
-mass spectra or mass spectrometry analytes, like peptides and small molecules.
+learning toolkit for building models to analyze mass spectrometry data. ##
+About Many deep learning tools have been developed for the analysis of mass
+spectra or mass spectrometry analytes, like peptides and small molecules.
 However, each one has had to reinvent the wheel. Depthcharge aims to provide a
-flexible, but opinionated, framework for rapidly prototyping deep learning
-models for mass spectrometry data. Think of Depthcharge as a set of building
-blocks to get you started on a new deep learning project focused around mass
-spectrometry data. Depthcharge delivers these building blocks in the form of
-PyTorch modules, which can be readily used to assemble customized deep learning
-models for your task.
+flexible, but opinionated, framework to rapidly prototype deep learning models
+for mass spectrometry data. Think of Depthcharge as a set of building blocks to
+get you started on a new deep learning project focused around mass spectrometry
+data. Depthcharge delivers these building blocks in the form of PyTorch
+modules, which can be readily used to assemble customized deep learning models
+for your task. With Depthcharge we aim to get users ~80% of the way to their
+ideal model in only a few hours, instead of requiring days or weeks to build
+and test models for different tasks.
```

### Comparing `depthcharge_ms-0.4.0/docs/stylesheets/extra.css` & `depthcharge_ms-0.4.1/docs/stylesheets/extra.css`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
  [data-md-color-scheme="depthcharge"]{
   --md-default-fg-color:             #EEEEEE;
   --md-default-fg-color--light:      #EEEEEE;
   --md-primary-fg-color:             #101010;
   --md-primary-fg-color--light:      #01BCA3;
   --md-primary-fg-color--dark:       #303030;
   --md-accent-fg-color:              #01BCA3;
-  --md-accent-fg-color--transparent: #01BCA3;
-  --md-accent-fg-color--transparent: #01BCA3;
+  --md-accent-fg-color--transparent: #01BCA34D;
+  --md-accent-fg-color--transparent: #01BCA34D;
   --md-typeset-a-color:              #01BCA3;
   --md-default-bg-color:             #1d1f21;
   --md-primary-bg-color--light:      #1d1f21;
   --md-primary-bg-color--dark:       #1d1f21;
   --md-footer-bg-color--dark:        #101010;
   --md-typeset-color:                #EEEEEE;
   --md-typeset-table-color:          #01BCA3;
@@ -46,7 +46,61 @@
 }
 
 .doc .highlight .o,
 .doc .highlight .p,
 .doc .highlight .kc {
   color: var(--md-default-fg-color)
 }
+
+.md-typeset .admonition.note {
+  background-color: var(--md-code-bg-color);
+  border-color: var(--md-accent-fg-color);
+  color: var(--md-default-fg-color);
+}
+
+.md-typeset .admonition.note > p {
+  white-space: pre;
+  tab-size: 4;
+  font-variant-ligatures: none;
+  font-feature-settings: "liga" 0;
+  display: block;
+  overflow-x: auto;
+}
+
+.md-typeset .note > .admonition-title::before {
+  background-color: var(--md-accent-fg-color);
+}
+
+.md-typeset .note > .admonition-title,
+.md-typeset .note > summary {
+  background-color: var(--md-accent-fg-color--transparent);
+}
+
+
+/* From mkdocstrings: */
+/* Indentation. */
+div.doc-contents:not(.first) {
+  padding-left: 25px;
+  border-left: .05rem solid var(--md-typeset-table-color);
+}
+
+/* Mark external links as such. */
+a.external::after,
+a.autorefs-external::after {
+  /* https://primer.style/octicons/arrow-up-right-24 */
+  mask-image: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M18.25 15.5a.75.75 0 00.75-.75v-9a.75.75 0 00-.75-.75h-9a.75.75 0 000 1.5h7.19L6.22 16.72a.75.75 0 101.06 1.06L17.5 7.56v7.19c0 .414.336.75.75.75z"></path></svg>');
+  -webkit-mask-image: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M18.25 15.5a.75.75 0 00.75-.75v-9a.75.75 0 00-.75-.75h-9a.75.75 0 000 1.5h7.19L6.22 16.72a.75.75 0 101.06 1.06L17.5 7.56v7.19c0 .414.336.75.75.75z"></path></svg>');
+  content: ' ';
+
+  display: inline-block;
+  vertical-align: middle;
+  position: relative;
+
+  height: 1em;
+  width: 1em;
+  background-color: currentColor;
+}
+
+a.external:hover::after,
+a.autorefs-external:hover::after {
+  background-color: var(--md-accent-fg-color);
+}
```

### Comparing `depthcharge_ms-0.4.0/mkdocs.yml` & `depthcharge_ms-0.4.1/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 site_name: depthcharge
 repo_url: https://github.com/wfondrie/depthcharge
 nav:
   - Getting Started:
       - Introduction: "index.md"
       - Installation: "getting-started/installation.md"
+      - Modeling Mass Spectra: "getting-started/spectra.md"
   - API:
       - Overview: "api/index.md"
       - Tokenizers: "api/tokenizers.md"
       - Datasets: "api/datasets.md"
       - Encoders: "api/encoders.md"
       - Transformers: "api/transformers.md"
       - Primitives: "api/primitives.md"
@@ -21,47 +22,57 @@
     - navigation.tabs
     - navigation.footer
     - content.code.copy
   logo: static/icon.svg
   favicon: static/icon.svg
   font:
     text: Fira Code
+    code: Fira Code
   palette:
     scheme: depthcharge
 
 extra_css:
   - stylesheets/extra.css
 
 plugins:
+  - mkquartodocs
   - mkdocstrings:
       default_handler: python
       handlers:
         python:
           options:
             docstring_style: numpy
             show_root_heading: true
-            heading_level: 3
+            show_root_full_path: false
+            heading_level: 2
             docstring_section_style: spacy
             show_source: false
             merge_init_into_class: true
+            group_by_category: true
+            show_category_heading: true
             docstring_options:
               ignore_init_summary: true
               trim_doctest_flags: true
-            options:
-              members: true
+
+            inherited_members: true
+            members:
+            filters: ["!^_", "!^__"]
 
 markdown_extensions:
   - attr_list
-  - smarty
+  #- smarty
   - footnotes
   - pymdownx.highlight:
       anchor_linenums: true
       line_spans: __span
       pygments_lang_class: true
   - pymdownx.inlinehilite
   - pymdownx.snippets
   - pymdownx.superfences
+  - tables
 
 extra:
   social:
     - icon: fontawesome/brands/twitter
       link: https://twitter.com/wfondrie
+  version:
+    provider: mike
```

### Comparing `depthcharge_ms-0.4.0/pyproject.toml` & `depthcharge_ms-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,33 @@
     "lark>=1.1.4",
     "selfies>=2.1.1",
     "sortedcontainers>=2.4.0",
     "dill>=0.3.6",
     "rdkit>=2023.03.1",
     "pillow>=9.4.0",
     "spectrum-utils>=0.4.1",
+    "cloudpathlib>=0.18.1",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "REAMDE.md"
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://github.com/wfondrie/depthcharge"
 Documentation = "https://wfondrie.github.io/depthcharge"
 
 [project.optional-dependencies]
 docs = [
+     "mike",
      "mkdocs",
      "mkdocs-material",
      "mkdocstrings[python]>=0.18",
+     "mkquartodocs",
 ]
 dev = [
     "pre-commit>=2.7.1"
 ]
 
 [tool.setuptools]
 include-package-data = false
```

### Comparing `depthcharge_ms-0.4.0/static/icon.svg` & `depthcharge_ms-0.4.1/static/icon.svg`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/static/logo-dark.png` & `depthcharge_ms-0.4.1/static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/static/logo-light.png` & `depthcharge_ms-0.4.1/static/logo-light.png`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/tests/conftest.py` & `depthcharge_ms-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/tests/unit_tests/test_data/test_arrow.py` & `depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_arrow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Test the arrow functionality."""
 
+import os
+
 import polars as pl
 import pyarrow as pa
 import pytest
 
 from depthcharge.data.arrow import (
     spectra_to_df,
     spectra_to_parquet,
@@ -92,14 +94,27 @@
         progress=progress,
     )
 
     parsed = pl.read_parquet(out)
     assert parsed.shape == shape
 
 
+def test_to_parquet_with_default_file(real_mzml, tmp_path):
+    """Test that a default file can be created."""
+    os.chdir(tmp_path)
+
+    out = spectra_to_parquet(
+        real_mzml,
+        parquet_file=None,
+        progress=False,
+    )
+
+    assert out.exists()
+
+
 @pytest.mark.parametrize(PARAM_NAMES, PARAM_VALS)
 def test_to_stream(
     real_mzml,
     ms_level,
     preprocessing_fn,
     valid_charge,
     custom_fields,
```

### Comparing `depthcharge_ms-0.4.0/tests/unit_tests/test_data/test_datasets.py` & `depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/tests/unit_tests/test_data/test_loaders.py` & `depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_loaders.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/tests/unit_tests/test_data/test_parsers.py` & `depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_parsers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/tests/unit_tests/test_encoders/test_sinusoidal.py` & `depthcharge_ms-0.4.1/tests/unit_tests/test_encoders/test_sinusoidal.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/tests/unit_tests/test_feedforward.py` & `depthcharge_ms-0.4.1/tests/unit_tests/test_feedforward.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/tests/unit_tests/test_primitives.py` & `depthcharge_ms-0.4.1/tests/unit_tests/test_primitives.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,7 +121,15 @@
         "scan=1",
         mzs,
         intensities,
         precursor_mz=10.0,
         precursor_charge=3,
     )
     assert spec.to_tensor().shape == (10, 2)
+
+    new_mzs = np.ones_like(spec.mz)
+    new_intensities = np.ones_like(spec.intensity)
+    spec.mz = new_mzs
+    spec.intensity = new_intensities
+
+    np.testing.assert_equal(spec.mz, new_mzs)
+    np.testing.assert_equal(spec.intensity, new_intensities)
```

### Comparing `depthcharge_ms-0.4.0/tests/unit_tests/test_testing.py` & `depthcharge_ms-0.4.1/tests/unit_tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/tests/unit_tests/test_tokenizers/test_molecules.py` & `depthcharge_ms-0.4.1/tests/unit_tests/test_tokenizers/test_molecules.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/tests/unit_tests/test_tokenizers/test_peptides.py` & `depthcharge_ms-0.4.1/tests/unit_tests/test_tokenizers/test_peptides.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/tests/unit_tests/test_transformers/test_analyte_transformers.py` & `depthcharge_ms-0.4.1/tests/unit_tests/test_transformers/test_analyte_transformers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/tests/unit_tests/test_transformers/test_spectrum_transformers.py` & `depthcharge_ms-0.4.1/tests/unit_tests/test_transformers/test_spectrum_transformers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.0/tests/unit_tests/test_version.py` & `depthcharge_ms-0.4.1/tests/unit_tests/test_version.py`

 * *Files identical despite different names*

