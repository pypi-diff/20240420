# Comparing `tmp/luis-v-subtitler-0.1.8.tar.gz` & `tmp/luis-v-subtitler-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luis-v-subtitler-0.1.8.tar", last modified: Fri Dec 29 22:45:28 2023, max compression
+gzip compressed data, was "luis-v-subtitler-0.1.9.tar", last modified: Wed Jan 10 19:49:48 2024, max compression
```

## Comparing `luis-v-subtitler-0.1.8.tar` & `luis-v-subtitler-0.1.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2023-12-29 22:45:28.306783 luis-v-subtitler-0.1.8/
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     2178 2023-12-29 22:45:06.000000 luis-v-subtitler-0.1.8/.cookiecutterrc
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      184 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/.coveragerc
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      353 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/.editorconfig
-drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2023-12-29 22:45:28.298783 luis-v-subtitler-0.1.8/.github/
-drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2023-12-29 22:45:28.298783 luis-v-subtitler-0.1.8/.github/workflows/
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     5643 2023-12-04 22:56:36.000000 luis-v-subtitler-0.1.8/.github/workflows/github-actions.yml
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      687 2023-12-04 23:02:10.000000 luis-v-subtitler-0.1.8/.pre-commit-config.yaml
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      282 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/.readthedocs.yml
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       90 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/AUTHORS.rst
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       86 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/CHANGELOG.rst
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     2436 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/CONTRIBUTING.rst
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     1115 2023-12-04 23:03:25.000000 luis-v-subtitler-0.1.8/LICENSE
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      421 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/MANIFEST.in
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     2339 2023-12-29 22:45:28.306783 luis-v-subtitler-0.1.8/PKG-INFO
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     2645 2023-12-29 22:45:06.000000 luis-v-subtitler-0.1.8/README.rst
-drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2023-12-29 22:45:28.302783 luis-v-subtitler-0.1.8/ci/
--rwxrwxr-x   0 luisv     (1000) luisv     (1000)     2867 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/ci/bootstrap.py
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       72 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/ci/requirements.txt
-drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2023-12-29 22:45:28.298783 luis-v-subtitler-0.1.8/ci/templates/
-drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2023-12-29 22:45:28.298783 luis-v-subtitler-0.1.8/ci/templates/.github/
-drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2023-12-29 22:45:28.302783 luis-v-subtitler-0.1.8/ci/templates/.github/workflows/
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     1965 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/ci/templates/.github/workflows/github-actions.yml
-drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2023-12-29 22:45:28.302783 luis-v-subtitler-0.1.8/docs/
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       28 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/docs/authors.rst
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       30 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/docs/changelog.rst
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     1198 2023-12-29 22:45:06.000000 luis-v-subtitler-0.1.8/docs/conf.py
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       33 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/docs/contributing.rst
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      244 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/docs/index.rst
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       96 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/docs/installation.rst
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       27 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/docs/readme.rst
-drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2023-12-29 22:45:28.302783 luis-v-subtitler-0.1.8/docs/reference/
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       68 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/docs/reference/index.rst
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      134 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/docs/reference/luis_v_subtitler.rst
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       29 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/docs/requirements.txt
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      109 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/docs/spelling_wordlist.txt
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       84 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/docs/usage.rst
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     1194 2023-12-05 00:24:50.000000 luis-v-subtitler-0.1.8/pyproject.toml
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      781 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/pytest.ini
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       38 2023-12-29 22:45:28.306783 luis-v-subtitler-0.1.8/setup.cfg
--rwxrwxr-x   0 luisv     (1000) luisv     (1000)     3424 2023-12-29 22:45:06.000000 luis-v-subtitler-0.1.8/setup.py
-drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2023-12-29 22:45:28.298783 luis-v-subtitler-0.1.8/src/
-drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2023-12-29 22:45:28.306783 luis-v-subtitler-0.1.8/src/luis_v_subtitler/
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      138 2023-12-29 22:45:06.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler/__init__.py
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      379 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler/__main__.py
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      948 2023-12-28 19:22:07.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler/cli.py
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     2302 2023-12-16 13:49:19.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler/language_identification.py
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     2648 2023-12-29 20:41:53.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler/save_subtitles.py
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     3250 2023-12-29 22:43:42.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler/subtitler.py
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     2150 2023-12-29 13:31:39.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler/utils.py
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     2751 2023-12-29 20:33:24.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler/whisperx_transcribe.py
-drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2023-12-29 22:45:28.306783 luis-v-subtitler-0.1.8/src/luis_v_subtitler.egg-info/
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     2339 2023-12-29 22:45:28.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler.egg-info/PKG-INFO
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     1211 2023-12-29 22:45:28.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler.egg-info/SOURCES.txt
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       84 2023-12-29 22:45:28.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler.egg-info/dependency_links.txt
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       63 2023-12-29 22:45:28.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler.egg-info/entry_points.txt
--rw-rw-r--   0 luisv     (1000) luisv     (1000)        1 2023-12-29 22:45:28.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler.egg-info/not-zip-safe
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      218 2023-12-29 22:45:28.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler.egg-info/requires.txt
--rw-rw-r--   0 luisv     (1000) luisv     (1000)       17 2023-12-29 22:45:28.000000 luis-v-subtitler-0.1.8/src/luis_v_subtitler.egg-info/top_level.txt
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     1381 2023-12-29 22:45:06.000000 luis-v-subtitler-0.1.8/tbump.toml
-drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2023-12-29 22:45:28.306783 luis-v-subtitler-0.1.8/tests/
--rw-rw-r--   0 luisv     (1000) luisv     (1000)      266 2023-12-05 01:46:19.000000 luis-v-subtitler-0.1.8/tests/test_luis_v_subtitler.py
--rw-rw-r--   0 luisv     (1000) luisv     (1000)     1670 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.8/tox.ini
+drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2024-01-10 19:49:48.601286 luis-v-subtitler-0.1.9/
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     2178 2024-01-10 19:44:17.000000 luis-v-subtitler-0.1.9/.cookiecutterrc
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      184 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/.coveragerc
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      353 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/.editorconfig
+drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2024-01-10 19:49:48.593286 luis-v-subtitler-0.1.9/.github/
+drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2024-01-10 19:49:48.597286 luis-v-subtitler-0.1.9/.github/workflows/
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     5643 2023-12-04 22:56:36.000000 luis-v-subtitler-0.1.9/.github/workflows/github-actions.yml
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      687 2023-12-04 23:02:10.000000 luis-v-subtitler-0.1.9/.pre-commit-config.yaml
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      282 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/.readthedocs.yml
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       90 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/AUTHORS.rst
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       86 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/CHANGELOG.rst
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     2436 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/CONTRIBUTING.rst
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     1115 2023-12-04 23:03:25.000000 luis-v-subtitler-0.1.9/LICENSE
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      421 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/MANIFEST.in
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     2339 2024-01-10 19:49:48.601286 luis-v-subtitler-0.1.9/PKG-INFO
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     2645 2024-01-10 19:44:17.000000 luis-v-subtitler-0.1.9/README.rst
+drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2024-01-10 19:49:48.597286 luis-v-subtitler-0.1.9/ci/
+-rwxrwxr-x   0 luisv     (1000) luisv     (1000)     2867 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/ci/bootstrap.py
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       72 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/ci/requirements.txt
+drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2024-01-10 19:49:48.593286 luis-v-subtitler-0.1.9/ci/templates/
+drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2024-01-10 19:49:48.593286 luis-v-subtitler-0.1.9/ci/templates/.github/
+drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2024-01-10 19:49:48.597286 luis-v-subtitler-0.1.9/ci/templates/.github/workflows/
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     1965 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/ci/templates/.github/workflows/github-actions.yml
+drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2024-01-10 19:49:48.601286 luis-v-subtitler-0.1.9/docs/
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       28 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/docs/authors.rst
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       30 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/docs/changelog.rst
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     1198 2024-01-10 19:44:17.000000 luis-v-subtitler-0.1.9/docs/conf.py
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       33 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/docs/contributing.rst
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      244 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/docs/index.rst
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       96 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/docs/installation.rst
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       27 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/docs/readme.rst
+drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2024-01-10 19:49:48.601286 luis-v-subtitler-0.1.9/docs/reference/
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       68 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/docs/reference/index.rst
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      134 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/docs/reference/luis_v_subtitler.rst
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       29 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/docs/requirements.txt
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      109 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/docs/spelling_wordlist.txt
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       84 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/docs/usage.rst
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     1194 2023-12-05 00:24:50.000000 luis-v-subtitler-0.1.9/pyproject.toml
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      781 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/pytest.ini
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       38 2024-01-10 19:49:48.601286 luis-v-subtitler-0.1.9/setup.cfg
+-rwxrwxr-x   0 luisv     (1000) luisv     (1000)     3424 2024-01-10 19:44:17.000000 luis-v-subtitler-0.1.9/setup.py
+drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2024-01-10 19:49:48.593286 luis-v-subtitler-0.1.9/src/
+drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2024-01-10 19:49:48.601286 luis-v-subtitler-0.1.9/src/luis_v_subtitler/
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      138 2024-01-10 19:44:17.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler/__init__.py
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      379 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler/__main__.py
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      948 2023-12-28 19:22:07.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler/cli.py
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     2302 2023-12-16 13:49:19.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler/language_identification.py
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     2648 2023-12-29 20:41:53.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler/save_subtitles.py
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     5196 2024-01-10 19:43:58.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler/subtitler.py
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     2150 2023-12-29 13:31:39.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler/utils.py
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     2751 2023-12-29 20:33:24.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler/whisperx_transcribe.py
+drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2024-01-10 19:49:48.601286 luis-v-subtitler-0.1.9/src/luis_v_subtitler.egg-info/
+-rw-r--r--   0 luisv     (1000) luisv     (1000)     2339 2024-01-10 19:49:48.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler.egg-info/PKG-INFO
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     1211 2024-01-10 19:49:48.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler.egg-info/SOURCES.txt
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       84 2024-01-10 19:49:48.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler.egg-info/dependency_links.txt
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       63 2024-01-10 19:49:48.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler.egg-info/entry_points.txt
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)        1 2024-01-10 19:45:58.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler.egg-info/not-zip-safe
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      218 2024-01-10 19:49:48.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler.egg-info/requires.txt
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)       17 2024-01-10 19:49:48.000000 luis-v-subtitler-0.1.9/src/luis_v_subtitler.egg-info/top_level.txt
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     1381 2024-01-10 19:44:17.000000 luis-v-subtitler-0.1.9/tbump.toml
+drwxrwxr-x   0 luisv     (1000) luisv     (1000)        0 2024-01-10 19:49:48.601286 luis-v-subtitler-0.1.9/tests/
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)      266 2023-12-05 01:46:19.000000 luis-v-subtitler-0.1.9/tests/test_luis_v_subtitler.py
+-rw-rw-r--   0 luisv     (1000) luisv     (1000)     1670 2023-12-04 22:56:19.000000 luis-v-subtitler-0.1.9/tox.ini
```

### Comparing `luis-v-subtitler-0.1.8/.cookiecutterrc` & `luis-v-subtitler-0.1.9/.cookiecutterrc`

 * *Files 0% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     scrutinizer: "no"
     setup_py_uses_setuptools_scm: "no"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://python-luis-v-subtitler.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "sphinx-rtd-theme"
     test_matrix_separate_coverage: "no"
-    version: "0.1.8"
+    version: "0.1.9"
     version_manager: "tbump"
     website: "https://luis-antonio-vasquez.glide.page/"
     year_from: "2023"
     year_to: "2023"
```

### Comparing `luis-v-subtitler-0.1.8/.github/workflows/github-actions.yml` & `luis-v-subtitler-0.1.9/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/.pre-commit-config.yaml` & `luis-v-subtitler-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/CONTRIBUTING.rst` & `luis-v-subtitler-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/LICENSE` & `luis-v-subtitler-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/PKG-INFO` & `luis-v-subtitler-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luis-v-subtitler
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python package to use AI to subtitle any video in any language
 Home-page: https://github.com/LuisAVasquez/python-luis-v-subtitler
 Author: Luis Antonio VASQUEZ REINA
 Author-email: luis.vasquez.work.contact@gmail.com
 License: MIT
 Project-URL: Documentation, https://python-luis-v-subtitler.readthedocs.io/
 Project-URL: Changelog, https://python-luis-v-subtitler.readthedocs.io/en/latest/changelog.html
```

### Comparing `luis-v-subtitler-0.1.8/README.rst` & `luis-v-subtitler-0.1.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/luis-v-subtitler
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/luis-v-subtitler.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/luis-v-subtitler
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/LuisAVasquez/python-luis-v-subtitler/v0.1.8.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/LuisAVasquez/python-luis-v-subtitler/v0.1.9.svg
     :alt: Commits since latest release
-    :target: https://github.com/LuisAVasquez/python-luis-v-subtitler/compare/v0.1.8...main
+    :target: https://github.com/LuisAVasquez/python-luis-v-subtitler/compare/v0.1.9...main
 
 
 
 .. end-badges
 
 A Python package to use AI to subtitle any video in any language
```

### Comparing `luis-v-subtitler-0.1.8/ci/bootstrap.py` & `luis-v-subtitler-0.1.9/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/ci/templates/.github/workflows/github-actions.yml` & `luis-v-subtitler-0.1.9/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/docs/conf.py` & `luis-v-subtitler-0.1.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "Luis V subtitler"
 year = "2023"
 author = "Luis Antonio VASQUEZ REINA"
 copyright = f"{year}, {author}"
-version = release = "0.1.8"
+version = release = "0.1.9"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/LuisAVasquez/python-luis-v-subtitler/issues/%s", "#"),
     "pr": ("https://github.com/LuisAVasquez/python-luis-v-subtitler/pull/%s", "PR #"),
 }
```

### Comparing `luis-v-subtitler-0.1.8/pyproject.toml` & `luis-v-subtitler-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/pytest.ini` & `luis-v-subtitler-0.1.9/pytest.ini`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/setup.py` & `luis-v-subtitler-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="luis-v-subtitler",
-    version="0.1.8",
+    version="0.1.9",
     license="MIT",
     description="A Python package to use AI to subtitle any video in any language",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="Luis Antonio VASQUEZ REINA",
```

### Comparing `luis-v-subtitler-0.1.8/src/luis_v_subtitler/cli.py` & `luis-v-subtitler-0.1.9/src/luis_v_subtitler/cli.py`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/src/luis_v_subtitler/language_identification.py` & `luis-v-subtitler-0.1.9/src/luis_v_subtitler/language_identification.py`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/src/luis_v_subtitler/save_subtitles.py` & `luis-v-subtitler-0.1.9/src/luis_v_subtitler/save_subtitles.py`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/src/luis_v_subtitler/utils.py` & `luis-v-subtitler-0.1.9/src/luis_v_subtitler/utils.py`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/src/luis_v_subtitler/whisperx_transcribe.py` & `luis-v-subtitler-0.1.9/src/luis_v_subtitler/whisperx_transcribe.py`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/src/luis_v_subtitler.egg-info/PKG-INFO` & `luis-v-subtitler-0.1.9/src/luis_v_subtitler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luis-v-subtitler
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python package to use AI to subtitle any video in any language
 Home-page: https://github.com/LuisAVasquez/python-luis-v-subtitler
 Author: Luis Antonio VASQUEZ REINA
 Author-email: luis.vasquez.work.contact@gmail.com
 License: MIT
 Project-URL: Documentation, https://python-luis-v-subtitler.readthedocs.io/
 Project-URL: Changelog, https://python-luis-v-subtitler.readthedocs.io/en/latest/changelog.html
```

### Comparing `luis-v-subtitler-0.1.8/src/luis_v_subtitler.egg-info/SOURCES.txt` & `luis-v-subtitler-0.1.9/src/luis_v_subtitler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luis-v-subtitler-0.1.8/tbump.toml` & `luis-v-subtitler-0.1.9/tbump.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/LuisAVasquez/python-luis-v-subtitler/"
 
 [version]
-current = "0.1.8"
+current = "0.1.9"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `luis-v-subtitler-0.1.8/tox.ini` & `luis-v-subtitler-0.1.9/tox.ini`

 * *Files identical despite different names*

