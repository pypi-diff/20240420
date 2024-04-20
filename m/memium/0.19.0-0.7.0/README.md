# Comparing `tmp/memium-0.19.0.tar.gz` & `tmp/memium-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memium-0.19.0.tar", last modified: Sat Apr 20 14:18:09 2024, max compression
+gzip compressed data, was "memium-0.7.0.tar", last modified: Wed Dec 27 14:05:34 2023, max compression
```

## Comparing `memium-0.19.0.tar` & `memium-0.7.0.tar`

### file list

```diff
@@ -1,102 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.586302 memium-0.19.0/
--rw-r--r--   0 root         (0) root         (0)      483 2024-04-20 14:17:59.000000 memium-0.19.0/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      735 2024-04-20 14:17:59.000000 memium-0.19.0/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.570302 memium-0.19.0/.devcontainer/
--rw-r--r--   0 root         (0) root         (0)     2468 2024-04-20 14:17:59.000000 memium-0.19.0/.devcontainer/devcontainer.json
--rw-r--r--   0 root         (0) root         (0)     1346 2024-04-20 14:17:59.000000 memium-0.19.0/.dockerignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.570302 memium-0.19.0/.github/
--rw-r--r--   0 root         (0) root         (0)     1754 2024-04-20 14:17:59.000000 memium-0.19.0/.github/recommended_repo_setup.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.574302 memium-0.19.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-20 14:17:59.000000 memium-0.19.0/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)     1264 2024-04-20 14:17:59.000000 memium-0.19.0/.github/workflows/docker-publish.yml
--rw-r--r--   0 root         (0) root         (0)     1600 2024-04-20 14:17:59.000000 memium-0.19.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      909 2024-04-20 14:17:59.000000 memium-0.19.0/.github/workflows/smoketests.yml
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-20 14:17:59.000000 memium-0.19.0/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)     1280 2024-04-20 14:17:59.000000 memium-0.19.0/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)     1330 2024-04-20 14:17:59.000000 memium-0.19.0/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.574302 memium-0.19.0/.vscode/
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-20 14:17:59.000000 memium-0.19.0/.vscode/launch.json
--rw-r--r--   0 root         (0) root         (0)      586 2024-04-20 14:17:59.000000 memium-0.19.0/.vscode/settings.json
--rw-r--r--   0 root         (0) root         (0)     2375 2024-04-20 14:17:59.000000 memium-0.19.0/.vscode/tasks.json
--rw-r--r--   0 root         (0) root         (0)   221025 2024-04-20 14:18:06.000000 memium-0.19.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)      436 2024-04-20 14:17:59.000000 memium-0.19.0/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1112 2024-04-20 14:17:59.000000 memium-0.19.0/Dockerfile.dev
--rw-r--r--   0 root         (0) root         (0)     6604 2024-04-20 14:18:09.586302 memium-0.19.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-20 14:17:59.000000 memium-0.19.0/makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.574302 memium-0.19.0/memium/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 14:17:59.000000 memium-0.19.0/memium/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4665 2024-04-20 14:17:59.000000 memium-0.19.0/memium/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.578302 memium-0.19.0/memium/destination/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.578302 memium-0.19.0/memium/destination/ankiconnect/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/ankiconnect/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2469 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/ankiconnect/anki_converter.py
--rw-r--r--   0 root         (0) root         (0)     1144 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/ankiconnect/anki_prompt.py
--rw-r--r--   0 root         (0) root         (0)     1358 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/ankiconnect/anki_prompt_cloze.py
--rw-r--r--   0 root         (0) root         (0)     2952 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/ankiconnect/anki_prompt_qa.py
--rw-r--r--   0 root         (0) root         (0)     7700 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/ankiconnect/ankiconnect_gateway.py
--rw-r--r--   0 root         (0) root         (0)     2468 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/ankiconnect/default_styling.css
--rw-r--r--   0 root         (0) root         (0)     1220 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/ankiconnect/test_anki_converter.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/ankiconnect/test_anki_prompt_qa.py
--rw-r--r--   0 root         (0) root         (0)     3360 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/ankiconnect/test_ankiconnect_gateway.py
--rw-r--r--   0 root         (0) root         (0)      596 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/destination.py
--rw-r--r--   0 root         (0) root         (0)     2742 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/destination_ankiconnect.py
--rw-r--r--   0 root         (0) root         (0)      716 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/destination_dryrun.py
--rw-r--r--   0 root         (0) root         (0)     2508 2024-04-20 14:17:59.000000 memium-0.19.0/memium/destination/test_destination_ankiconnect.py
--rw-r--r--   0 root         (0) root         (0)     1979 2024-04-20 14:17:59.000000 memium-0.19.0/memium/diff_determiner.py
--rw-r--r--   0 root         (0) root         (0)      645 2024-04-20 14:17:59.000000 memium-0.19.0/memium/environment.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 14:17:59.000000 memium-0.19.0/memium/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.582302 memium-0.19.0/memium/source/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/__init__.py
--rw-r--r--   0 root         (0) root         (0)      471 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/document.py
--rw-r--r--   0 root         (0) root         (0)     2523 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/document_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.582302 memium-0.19.0/memium/source/extractors/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/extractors/__init__.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/extractors/extractor.py
--rw-r--r--   0 root         (0) root         (0)     3285 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/extractors/extractor_cloze.py
--rw-r--r--   0 root         (0) root         (0)     2692 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/extractors/extractor_qa.py
--rw-r--r--   0 root         (0) root         (0)     5382 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/extractors/extractor_table.py
--rw-r--r--   0 root         (0) root         (0)     1999 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/extractors/test_extractor_table.py
--rw-r--r--   0 root         (0) root         (0)      458 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/extractors/test_prompt.py
--rw-r--r--   0 root         (0) root         (0)     1246 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/extractors/test_prompt_extractor_cloze.py
--rw-r--r--   0 root         (0) root         (0)      644 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/extractors/test_prompt_extractor_qa.py
--rw-r--r--   0 root         (0) root         (0)     1078 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/extractors/to_line_blocks.py
--rw-r--r--   0 root         (0) root         (0)     2329 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/prompt_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.582302 memium-0.19.0/memium/source/prompts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/prompts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.582302 memium-0.19.0/memium/source/prompts/__snapshots__/
--rw-r--r--   0 root         (0) root         (0)      123 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/prompts/__snapshots__/prompt_from_doc_test.ambr
--rw-r--r--   0 root         (0) root         (0)      955 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/prompts/prompt.py
--rw-r--r--   0 root         (0) root         (0)      995 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/prompts/prompt_cloze.py
--rw-r--r--   0 root         (0) root         (0)      775 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/prompts/prompt_from_doc.py
--rw-r--r--   0 root         (0) root         (0)      184 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/prompts/prompt_from_doc_test.py
--rw-r--r--   0 root         (0) root         (0)     1384 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/prompts/prompt_qa.py
--rw-r--r--   0 root         (0) root         (0)     2234 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/test_document_source.py
--rw-r--r--   0 root         (0) root         (0)      928 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/test_facade.py
--rw-r--r--   0 root         (0) root         (0)      688 2024-04-20 14:17:59.000000 memium-0.19.0/memium/source/test_prompt_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.586302 memium-0.19.0/memium/tasks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 14:17:59.000000 memium-0.19.0/memium/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-04-20 14:17:59.000000 memium-0.19.0/memium/tasks/github.py
--rw-r--r--   0 root         (0) root         (0)      682 2024-04-20 14:17:59.000000 memium-0.19.0/memium/tasks/graphite.py
--rw-r--r--   0 root         (0) root         (0)     2019 2024-04-20 14:17:59.000000 memium-0.19.0/memium/tasks/smoketest.py
--rw-r--r--   0 root         (0) root         (0)      243 2024-04-20 14:17:59.000000 memium-0.19.0/memium/tasks/str_parsing.py
--rw-r--r--   0 root         (0) root         (0)     2622 2024-04-20 14:17:59.000000 memium-0.19.0/memium/test_diff_determiner.py
--rw-r--r--   0 root         (0) root         (0)     1272 2024-04-20 14:17:59.000000 memium-0.19.0/memium/test_main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.586302 memium-0.19.0/memium/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 14:17:59.000000 memium-0.19.0/memium/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      231 2024-04-20 14:17:59.000000 memium-0.19.0/memium/utils/extract_terms.py
--rw-r--r--   0 root         (0) root         (0)     2339 2024-04-20 14:17:59.000000 memium-0.19.0/memium/utils/hash_cleaned_str.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-20 14:17:59.000000 memium-0.19.0/memium/utils/test_extract_terms.py
--rw-r--r--   0 root         (0) root         (0)     1368 2024-04-20 14:17:59.000000 memium-0.19.0/memium/utils/test_hash_cleaned_str.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 14:18:09.586302 memium-0.19.0/memium.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6604 2024-04-20 14:18:09.000000 memium-0.19.0/memium.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2762 2024-04-20 14:18:09.000000 memium-0.19.0/memium.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 14:18:09.000000 memium-0.19.0/memium.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-20 14:18:09.000000 memium-0.19.0/memium.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      398 2024-04-20 14:18:09.000000 memium-0.19.0/memium.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-20 14:18:09.000000 memium-0.19.0/memium.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3278 2024-04-20 14:18:06.000000 memium-0.19.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5118 2024-04-20 14:17:59.000000 memium-0.19.0/readme.md
--rw-r--r--   0 root         (0) root         (0)      313 2024-04-20 14:17:59.000000 memium-0.19.0/renovate.json
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 14:18:09.590302 memium-0.19.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3344 2024-04-20 14:17:59.000000 memium-0.19.0/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.673022 memium-0.7.0/
+-rw-r--r--   0 root         (0) root         (0)      483 2023-12-27 14:05:26.000000 memium-0.7.0/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      735 2023-12-27 14:05:26.000000 memium-0.7.0/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.657022 memium-0.7.0/.devcontainer/
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-12-27 14:05:26.000000 memium-0.7.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-12-27 14:05:26.000000 memium-0.7.0/.dockerignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.657022 memium-0.7.0/.github/
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-12-27 14:05:26.000000 memium-0.7.0/.github/recommended_repo_setup.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.657022 memium-0.7.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-12-27 14:05:26.000000 memium-0.7.0/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-12-27 14:05:26.000000 memium-0.7.0/.github/workflows/docker-publish.yml
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-12-27 14:05:26.000000 memium-0.7.0/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-12-27 14:05:26.000000 memium-0.7.0/.github/workflows/smoketests.yml
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-12-27 14:05:26.000000 memium-0.7.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-12-27 14:05:26.000000 memium-0.7.0/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-12-27 14:05:26.000000 memium-0.7.0/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.657022 memium-0.7.0/.vscode/
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-12-27 14:05:26.000000 memium-0.7.0/.vscode/launch.json
+-rw-r--r--   0 root         (0) root         (0)      586 2023-12-27 14:05:26.000000 memium-0.7.0/.vscode/settings.json
+-rw-r--r--   0 root         (0) root         (0)     2768 2023-12-27 14:05:26.000000 memium-0.7.0/.vscode/tasks.json
+-rw-r--r--   0 root         (0) root         (0)   117179 2023-12-27 14:05:26.000000 memium-0.7.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)      436 2023-12-27 14:05:26.000000 memium-0.7.0/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-12-27 14:05:26.000000 memium-0.7.0/Dockerfile.dev
+-rw-r--r--   0 root         (0) root         (0)     5999 2023-12-27 14:05:34.669022 memium-0.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      132 2023-12-27 14:05:26.000000 memium-0.7.0/makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.661022 memium-0.7.0/memium/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-27 14:05:26.000000 memium-0.7.0/memium/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       28 2023-12-27 14:05:26.000000 memium-0.7.0/memium/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2612 2023-12-27 14:05:26.000000 memium-0.7.0/memium/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.661022 memium-0.7.0/memium/data_access/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-27 14:05:26.000000 memium-0.7.0/memium/data_access/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7156 2023-12-27 14:05:26.000000 memium-0.7.0/memium/data_access/ankiconnect_gateway.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-12-27 14:05:26.000000 memium-0.7.0/memium/data_access/environment.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2023-12-27 14:05:26.000000 memium-0.7.0/memium/data_access/test_ankiconnect_gateway.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.665022 memium-0.7.0/memium/destination/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.665022 memium-0.7.0/memium/destination/ankiconnect/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/ankiconnect/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      861 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/ankiconnect/anki_card.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/ankiconnect/anki_converter.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/ankiconnect/anki_prompt_cloze.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/ankiconnect/anki_prompt_qa.py
+-rw-r--r--   0 root         (0) root         (0)     3807 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/ankiconnect/ankiconnect_css.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/ankiconnect/test_anki_converter.py
+-rw-r--r--   0 root         (0) root         (0)      559 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/ankiconnect/test_anki_prompt_qa.py
+-rw-r--r--   0 root         (0) root         (0)      592 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/destination.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/destination_ankiconnect.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/destination_commands.py
+-rw-r--r--   0 root         (0) root         (0)      742 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/destination_dryrun.py
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-12-27 14:05:26.000000 memium-0.7.0/memium/destination/test_destination_ankiconnect.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-12-27 14:05:26.000000 memium-0.7.0/memium/diff_determiner.py
+-rw-r--r--   0 root         (0) root         (0)     2136 2023-12-27 14:05:26.000000 memium-0.7.0/memium/main.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-27 14:05:26.000000 memium-0.7.0/memium/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.665022 memium-0.7.0/memium/source/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      471 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/document.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/document_ingester.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.665022 memium-0.7.0/memium/source/extractors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/extractors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      351 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/extractors/extractor.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/extractors/extractor_cloze.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/extractors/extractor_qa.py
+-rw-r--r--   0 root         (0) root         (0)      580 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/extractors/test_prompt_extractor_cloze.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/extractors/test_prompt_extractor_qa.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.669022 memium-0.7.0/memium/source/prompts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/prompts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      663 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/prompts/prompt.py
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/prompts/prompt_cloze.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/prompts/prompt_qa.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/test_document_ingester.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-12-27 14:05:26.000000 memium-0.7.0/memium/source/test_facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.669022 memium-0.7.0/memium/subtasks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-27 14:05:26.000000 memium-0.7.0/memium/subtasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-12-27 14:05:26.000000 memium-0.7.0/memium/subtasks/github.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-12-27 14:05:26.000000 memium-0.7.0/memium/subtasks/graphite.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-12-27 14:05:26.000000 memium-0.7.0/memium/subtasks/smoketest.py
+-rw-r--r--   0 root         (0) root         (0)      257 2023-12-27 14:05:26.000000 memium-0.7.0/memium/subtasks/str_parsing.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-12-27 14:05:26.000000 memium-0.7.0/memium/test_diff_determiner.py
+-rw-r--r--   0 root         (0) root         (0)      813 2023-12-27 14:05:26.000000 memium-0.7.0/memium/test_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.669022 memium-0.7.0/memium/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-27 14:05:26.000000 memium-0.7.0/memium/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-12-27 14:05:26.000000 memium-0.7.0/memium/utils/hash_cleaned_str.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-12-27 14:05:26.000000 memium-0.7.0/memium/utils/test_hash_cleaned_str.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-27 14:05:34.669022 memium-0.7.0/memium.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5999 2023-12-27 14:05:34.000000 memium-0.7.0/memium.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-12-27 14:05:34.000000 memium-0.7.0/memium.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-27 14:05:34.000000 memium-0.7.0/memium.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-12-27 14:05:34.000000 memium-0.7.0/memium.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      320 2023-12-27 14:05:34.000000 memium-0.7.0/memium.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-12-27 14:05:34.000000 memium-0.7.0/memium.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3139 2023-12-27 14:05:28.000000 memium-0.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     4750 2023-12-27 14:05:26.000000 memium-0.7.0/readme.md
+-rw-r--r--   0 root         (0) root         (0)      313 2023-12-27 14:05:26.000000 memium-0.7.0/renovate.json
+-rw-r--r--   0 root         (0) root         (0)       38 2023-12-27 14:05:34.673022 memium-0.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3567 2023-12-27 14:05:26.000000 memium-0.7.0/tasks.py
```

### Comparing `memium-0.19.0/.cruft.json` & `memium-0.7.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `memium-0.19.0/.devcontainer/devcontainer.json` & `memium-0.7.0/.devcontainer/devcontainer.json`

 * *Files 9% similar despite different names*

```diff
@@ -8,27 +8,25 @@
         // Update the 'dockerFile' property if you aren't using the standard 'Dockerfile' filename.
         "dockerfile": "../Dockerfile.dev",
         "cacheFrom": "ghcr.io/martinbernstorff/memium-devcontainer:latest"
     },
     "customizations": {
         "vscode": {
             "extensions": [
-                "ms-python.vscode-pylance",
                 "GitHub.copilot",
                 "charliermarsh.ruff",
                 "ms-python.python",
+                "ms-python.vscode-pylance",
                 "GitHub.vscode-pull-request-github",
+                "ms-vscode.makefile-tools",
                 "github.vscode-github-actions",
                 "markis.code-coverage",
+                "Gerrnperl.outline-map",
                 "SeeLog.python-init-generator",
-                "Graphite.gti-vscode",
-                "aeschli.vscode-css-formatter",
-                "esbenp.prettier-vscode",
-                "MichaelCurrin.auto-commit-msg",
-                "tamasfe.even-better-toml"
+                "Graphite.gti-vscode"
             ]
         }
     },
     "mounts": [
         "source=${localEnv:HOME}/.config/gh/hosts.yml,target=/root/.config/gh/hosts.yml,type=bind,consistency=cache", // GitHub CLI authentication login
         "source=${localEnv:HOME}/ankidecks,target=/output/,type=bind,consistency=cache",
         // "source=/Users/Shared/life-lessons/docs/life-lessons/,target=/input/,type=bind,consistency=cache",
```

### Comparing `memium-0.19.0/.dockerignore` & `memium-0.7.0/.dockerignore`

 * *Files identical despite different names*

### Comparing `memium-0.19.0/.github/recommended_repo_setup.md` & `memium-0.7.0/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `memium-0.19.0/.github/workflows/check_for_rej.yml` & `memium-0.7.0/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `memium-0.19.0/.github/workflows/release.yml` & `memium-0.7.0/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
           token: ${{ secrets.RELEASE }}
 
       - name: Python Semantic Release
         id: release
-        uses: python-semantic-release/python-semantic-release@v9.4.2
+        uses: python-semantic-release/python-semantic-release@v8.7.0
         with:
           github_token: ${{ secrets.RELEASE }}
 
       - name: Publish package distributions to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         if: steps.release.outputs.released == 'true'
         # This action supports PyPI's trusted publishing implementation, which allows authentication to PyPI without a manually
```

### Comparing `memium-0.19.0/.github/workflows/stalebot.yml` & `memium-0.7.0/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `memium-0.19.0/.gitignore` & `memium-0.7.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -113,8 +113,7 @@
 
 .pytest_cache
 pytest.xml
 pytest-coverage.txt
 BearImages*
 test_package
 .pytest_results
-.testmondata
```

### Comparing `memium-0.19.0/.vscode/settings.json` & `memium-0.7.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `memium-0.19.0/.vscode/tasks.json` & `memium-0.7.0/.vscode/tasks.json`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     // See https://go.microsoft.com/fwlink/?LinkId=733558
     // for the documentation about the tasks.json format
     "version": "2.0.0",
     "tasks": [
         {
             "label": "Submit PR",
             "type": "shell",
-            "command": "lm sync --squash --automerge",
+            "command": "inv submit",
             "dependsOn": [
                 "Ready"
             ],
             "presentation": {
                 "clear": false,
                 "group": "build",
                 "reveal": "always",
@@ -69,14 +69,28 @@
                 "group": "pr"
             }
         },
         {
             "label": "Static type check",
             "type": "shell",
             "command": "inv types",
+            "dependsOn": [
+                "Update from ancestor"
+            ],
+            "presentation": {
+                "reveal": "always",
+                "clear": true,
+                "showReuseMessage": false,
+                "group": "pr"
+            }
+        },
+        {
+            "label": "Update from ancestor",
+            "type": "shell",
+            "command": "gt sync --delete --force",
             "presentation": {
                 "reveal": "always",
                 "clear": true,
                 "showReuseMessage": false,
                 "group": "pr"
             }
         }
```

### Comparing `memium-0.19.0/Dockerfile.dev` & `memium-0.7.0/Dockerfile.dev`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Use an official Python runtime as a parent image
-FROM python:3.12
+FROM python:3.12-bookworm
 
 ####################
 # Install Graphite #
 ####################
 ENV NVM_DIR=$HOME/.nvm
 RUN mkdir -p $NVM_DIR
 ENV NODE_VERSION=18.2.0
```

### Comparing `memium-0.19.0/PKG-INFO` & `memium-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,50 @@
 Metadata-Version: 2.1
 Name: memium
-Version: 0.19.0
+Version: 0.7.0
 Summary: Memium
 Author-email: Martin Bernstorff <martinbernstorff@gmail.com>
 Project-URL: homepage, https://github.com/MartinBernstorff/memium
 Project-URL: repository, https://github.com/MartinBernstorff/memium
 Project-URL: documentation, https://MartinBernstorff.github.io/memium/
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: cffi==1.16.0
-Requires-Dist: iterpy==1.9.0
+Requires-Dist: functionalpy==0.14.0
 Requires-Dist: genanki==0.13.1
-Requires-Dist: markdown==3.6
-Requires-Dist: pydantic==2.7.0
-Requires-Dist: sentry-sdk==1.45.0
-Requires-Dist: typer==0.12.3
-Requires-Dist: tqdm==4.66.2
-Requires-Dist: unidecode==1.3.8
+Requires-Dist: misaka==2.1.1
+Requires-Dist: pydantic==2.5.3
+Requires-Dist: sentry-sdk==1.39.1
+Requires-Dist: typer==0.9.0
+Requires-Dist: tqdm==4.66.1
 Requires-Dist: wasabi==1.1.2
-Requires-Dist: bs4==0.0.1
-Provides-Extra: tests
-Requires-Dist: pytest==7.4.4; extra == "tests"
-Requires-Dist: pytest-cov==5.0.0; extra == "tests"
-Requires-Dist: pytest-xdist==3.6.0; extra == "tests"
-Requires-Dist: pytest-sugar==1.0.0; extra == "tests"
-Requires-Dist: pytest-testmon==2.1.1; extra == "tests"
-Requires-Dist: diff-cover==9.0.0; extra == "tests"
-Requires-Dist: syrupy==4.6.1; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: cruft==2.15.0; extra == "dev"
-Requires-Dist: herbarium; extra == "dev"
 Requires-Dist: invoke==2.2.0; extra == "dev"
-Requires-Dist: pyright==1.1.359; extra == "dev"
-Requires-Dist: pre-commit==3.7.0; extra == "dev"
-Requires-Dist: ruff==0.4.1; extra == "dev"
-Requires-Dist: lumberman; extra == "dev"
+Requires-Dist: pyright==1.1.343; extra == "dev"
+Requires-Dist: pre-commit==3.6.0; extra == "dev"
+Requires-Dist: ruff==0.1.9; extra == "dev"
+Provides-Extra: tests
+Requires-Dist: pytest==7.4.3; extra == "tests"
+Requires-Dist: pytest-cov==4.1.0; extra == "tests"
+Requires-Dist: pytest-xdist==3.5.0; extra == "tests"
+Requires-Dist: pytest-sugar==0.9.7; extra == "tests"
+Requires-Dist: diff-cover==8.0.2; extra == "tests"
 
 # Memium
 
 [![Open in Dev Container](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)][dev container]
 [![PyPI](https://img.shields.io/pypi/v/memium.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/memium)][pypi status]
-[![Roadmap](https://img.shields.io/badge/Board-Roadmap-green)][roadmap]
 
 [dev container]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/MartinBernstorff/memium/
 [pypi status]: https://pypi.org/project/memium/
 [documentation]: https://MartinBernstorff.github.io/memium/
-[roadmap]: https://github.com/users/MartinBernstorff/projects/2
+
 
 <!-- start short-description -->
 
 When you have to stop and look things up, it breaks up your flow. Adding this knowledge to long-term memory builds fluency, and being fluent at something makes it much more fun! The faster you can get from crawling to running, the more enjoyable it is.
 
 Unfortunately, we forget most of what we read, [even stuff we care about](https://andymatuschak.org/books/).
 
@@ -89,55 +82,49 @@
 ### In Docker container
 2. Install [Orbstack](https://orbstack.dev/) or Docker Desktop. 
 3. Setup a container
 ```bash
 $INPUT_DIR="PATH_TO_YOUR_INPUT_DIR"
 
 docker run -i \
-  --name=memium \
   -e HOST_INPUT_DIR=$INPUT_DIR \
   -v $INPUT_DIR:/input \
   --restart unless-stopped \
   ghcr.io/martinbernstorff/memium:latest \
   memium \
   --input-dir /input/
 ```
 
-This will start a docker container which updates your deck from `$INPUT_DIR`. In case of updated files, it will sync the difference (create new prompts and delete deleted prompts) to Anki. 
-
-If you want to continuously sync the directory, set the `--watch-seconds [UPDATE_SECONDS]` argument as well.
-
-Keeping the package update can be a bit of a chore, which can be automated with [WatchTower](https://github.com/containrrr/watchtower).
+This will start a docker container which updates your deck from `$INPUT_DIR`. In case of updated files, it will sync the difference (create new prompts and delete deleted prompts) to Anki. If you want to continuously sync the directory, check out the documentation for the `cli`.
 
 ## Use as library
 If you would like to build build your own Python application on top of the abstractions added here, you can install the library from pypi:
 
 ```bash
 pip install memium
 ```
 
 ### Pipeline abstractions
-The library is built as a pipeline illustrated below. Left describes the abstract pipeline, defined by interfaces. The right path describes an implementation of those interfaces from markdown to Anki, which is available in the CLI. 
+The library is built as a pipeline illustrated below. The left path describes the abstract pipeline, defined by abstract interfaces. The right path describes implementation I use, and which is part of this repo. 
 
 ```mermaid
 
 graph TD 
 	FD["File on disk"]
-        DP["Prompts at Destination"]
-	FD -- DocumentSource --> Document
-	Document -- PromptExtractor --> Prompt
-	Prompt -- Destination --> DP
+	FD -- Document ingester --> Document
+	Document -- Prompt extractor --> Prompt
+	Prompt -- Destination --> Card 
  
 	MD["Markdown file"]
-	Prompts["[QAPrompt | ClozePrompt]"]
-        Anki["Cards in the Anki app"]
+	 Prompts["[QAPrompt | ClozePrompt]"]
+  Cards["[AnkiQA | AnkiCloze]"]
  
-	MD -- MarkdownDocumentSource --> Document
+	MD -- MarkdownDocumentIngester --> Document
 	Document -- "[QAPromptExtractor, \nClozePromptExtractor]" --> Prompts
-        Prompts -- AnkiConnectDestination --> Anki
+	Prompts -- AnkiConnectDestination --> Cards
  ```
 
 ## Contributing
 ### Setting up a dev environment
 1. Install [Orbstack](https://orbstack.dev/) or Docker Desktop. Make sure to complete the full install process before continuing.
 2. If not installed, install VSCode
 3. Press this [link](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/MartinBernstorff/memium/)
```

### Comparing `memium-0.19.0/memium/destination/ankiconnect/anki_converter.py` & `memium-0.7.0/memium/destination/ankiconnect/anki_converter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,53 @@
-from ...source.prompts.prompt import BasePrompt, DestinationPrompt
-from ...source.prompts.prompt_cloze import ClozePrompt, ClozeWithoutDoc
-from ...source.prompts.prompt_qa import QAPrompt, QAWithoutDoc
-from .anki_prompt import AnkiPrompt
+from collections.abc import Sequence
+
+from functionalpy._sequence import Seq
+
+from ...source.prompts.prompt import BasePrompt
+from ...source.prompts.prompt_cloze import ClozePrompt
+from ...source.prompts.prompt_qa import QAPrompt
+from .anki_card import AnkiCard
 from .anki_prompt_cloze import AnkiCloze
 from .anki_prompt_qa import AnkiQA
-from .ankiconnect_gateway import NoteInfo
 
 
 class AnkiPromptConverter:
-    def __init__(self, base_deck: str, card_css: str, deck_prefix: str = "#anki_deck") -> None:
+    def __init__(
+        self, base_deck: str, card_css: str, deck_prefix: str = "#anki_deck"
+    ) -> None:
         self.base_deck = base_deck
         self.deck_prefix = deck_prefix
         self.card_css = card_css
 
-    def prompt_to_card(self, prompt: BasePrompt) -> AnkiPrompt:
-        deck_in_tags = [tag for tag in prompt.tags if tag.startswith(self.deck_prefix)]
+    def _prompt_to_card(self, prompt: BasePrompt) -> AnkiCard:
+        deck_in_tags = [
+            tag for tag in prompt.tags if tag.startswith(self.deck_prefix)
+        ]
         deck = deck_in_tags[0] if deck_in_tags else self.base_deck
 
         match prompt:
             case QAPrompt():
                 return AnkiQA(
                     question=prompt.question,
                     answer=prompt.answer,
                     base_deck=deck,
                     tags=prompt.tags,
                     css=self.card_css,
-                    uuid=prompt.scheduling_uid,
-                    edit_url=prompt.edit_url,
                 )
             case ClozePrompt():
                 return AnkiCloze(
                     text=prompt.text,
                     base_deck=deck,
                     tags=prompt.tags,
                     css=self.card_css,
-                    uuid=prompt.scheduling_uid,
-                    edit_url=prompt.edit_url,
                 )
             case BasePrompt():
-                raise ValueError("BasePrompt is the base class for all prompts, use a subclass")
+                raise ValueError(
+                    "BasePrompt is the base class for all prompts, use a subclass"
+                )
 
-    def note_info_to_prompt(self, note_info: NoteInfo) -> DestinationPrompt:
-        if "Question" in note_info.fields and "Answer" in note_info.fields:
-            return DestinationPrompt(
-                QAWithoutDoc(
-                    question=note_info.fields["Question"].value,
-                    answer=note_info.fields["Answer"].value,
-                    add_tags=note_info.tags,
-                ),
-                destination_id=str(note_info.noteId),
-            )
-
-        if "Text" in note_info.fields:
-            return DestinationPrompt(
-                ClozeWithoutDoc(text=note_info.fields["Text"].value, add_tags=note_info.tags),
-                destination_id=str(note_info.noteId),
-            )
+    def prompts_to_cards(
+        self, prompts: Sequence[BasePrompt]
+    ) -> Sequence[AnkiCard]:
+        """Takes an iterable of prompts and turns them into AnkiCards"""
 
-        raise ValueError(f"NoteInfo {note_info} has neither Question nor Text field")
+        return Seq(prompts).map(self._prompt_to_card).to_list()
```

### Comparing `memium-0.19.0/memium/destination/ankiconnect/anki_prompt.py` & `memium-0.7.0/memium/destination/ankiconnect/anki_card.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from abc import ABC, abstractmethod
 from collections.abc import Sequence
 from dataclasses import dataclass
 
 import genanki
-import markdown
 
 
 @dataclass(frozen=True)
-class AnkiPrompt(ABC):
+class AnkiCard(ABC):
     base_deck: str
     tags: Sequence[str]
-    uuid: int  # UUID is a unique identifier for the prompt, used for scheduling. If a new prompt is added with the same uuid, it will be treated as an update to the existing prompt. Otherwise, they will be interpreted as separate prompts.
-    edit_url: str | None
 
-    def _field_to_html(self, field: str) -> str:
-        return markdown.markdown(field)
+    @property
+    @abstractmethod
+    def uuid(self) -> int:
+        ...
 
     @property
     @abstractmethod
-    def genanki_model(self) -> genanki.Model: ...
+    def genanki_model(self) -> genanki.Model:
+        ...
 
     @abstractmethod
-    def to_genanki_note(self) -> genanki.Note: ...
+    def to_genanki_note(self) -> genanki.Note:
+        ...
 
     @property
     def deck(self) -> str:
         deck_prefix = "anki/deck/"
         deck_in_tags = (
             tag.replace(deck_prefix, "").replace("/", "::")
             for tag in self.tags
```

### Comparing `memium-0.19.0/memium/destination/ankiconnect/anki_prompt_cloze.py` & `memium-0.7.0/memium/destination/ankiconnect/anki_prompt_cloze.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 from collections.abc import Sequence
 from dataclasses import dataclass
 
 import genanki
 
-from ...utils.hash_cleaned_str import hash_str_to_int
-from .anki_prompt import AnkiPrompt
+from ...utils.hash_cleaned_str import clean_str, int_hash_str
+from .anki_card import AnkiCard
 
 
 @dataclass(frozen=True)
-class AnkiCloze(AnkiPrompt):
+class AnkiCloze(AnkiCard):
     base_deck: str
     tags: Sequence[str]
     text: str
     css: str
 
     @property
+    def uuid(self) -> int:
+        return int_hash_str(clean_str(self.text))
+
+    @property
     def genanki_model(self) -> genanki.Model:
         model_name = "Ankdown Cloze with UUID"
 
         return genanki.Model(
-            model_id=hash_str_to_int(model_name),
+            model_id=int_hash_str(model_name),
             name=model_name,
-            fields=[{"name": "Text"}, {"name": "Extra"}, {"name": "Tags"}, {"name": "UUID"}],
+            fields=[
+                {"name": "Text"},
+                {"name": "Extra"},
+                {"name": "Tags"},
+                {"name": "UUID"},
+            ],
             templates=[
                 {
                     "name": "Ankdown Cloze Card with UUID",
                     "qfmt": r"{{{{cloze:Text}}}}\n<div class='extra'>{{{{Extra}}}}</div>\n{}",
                     "afmt": r"{{{{cloze:Text}}}}\n<div class='extra'>{{{{Extra}}}}</div>\n{}",
                 }
             ],
@@ -33,10 +42,10 @@
             model_type=1,  # This is the model_type number for genanki, takes 0 for QA or 1 for cloze
         )
 
     def to_genanki_note(self) -> genanki.Note:
         return genanki.Note(
             guid=str(self.uuid),
             model=self.genanki_model,
-            fields=[self._field_to_html(self.text), "", " ".join(self.tags), str(self.uuid)],
+            fields=[self.text, "", " ".join(self.tags), str(self.uuid)],
             tags=self.tags,
         )
```

### Comparing `memium-0.19.0/memium/destination/ankiconnect/ankiconnect_gateway.py` & `memium-0.7.0/memium/data_access/ankiconnect_gateway.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from collections.abc import Iterator, Mapping, Sequence
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from time import sleep
 from typing import Any
 
-from memium.environment import in_docker
+from memium.data_access.environment import in_docker
 
 log = logging.getLogger(__name__)
 
 import genanki
 import pydantic
 
 log = logging.getLogger(__name__)
@@ -53,20 +53,16 @@
 
 class AnkiConnectCommand(Enum):
     CARDS_TO_NOTES = "cardsToNotes"
     DELETE_NOTES = "deleteNotes"
     FIND_CARDS = "findCards"
     GET_NOTE_INFOS = "notesInfo"
     IMPORT_PACKAGE = "importPackage"
-
-    # Models
-    CREATE_MODEL = "createModel"
     UPDATE_MODEL_TEMPLATES = "updateModelTemplates"
     UPDATE_MODEL_STYLING = "updateModelStyling"
-    GET_MODEL_NAMES = "modelNames"
 
 
 @dataclass(frozen=True)
 class AnkiConnectGateway:
     ankiconnect_url: str
     base_deck: str
     tmp_read_dir: Path
@@ -74,60 +70,54 @@
     max_deletions_per_run: int
     max_wait_seconds: int
 
     def __post_init__(self) -> None:
         seconds_waited = 0
         while not anki_connect_is_live(ankiconnect_url=self.ankiconnect_url):
             if seconds_waited >= self.max_wait_seconds:
-                raise ConnectionError(f"Could not connect to AnkiConnect at {self.ankiconnect_url}")
+                raise ConnectionError(
+                    f"Could not connect to AnkiConnect at {self.ankiconnect_url}"
+                )
 
             wait_seconds = 2
-            log.info(f"AnkiConnect is not live, waiting {wait_seconds} seconds...")
+            log.info(
+                f"AnkiConnect is not live, waiting {wait_seconds} seconds..."
+            )
             seconds_waited += wait_seconds
             sleep(wait_seconds)
 
     def update_model(self, model: genanki.Model) -> None:
-        existing_model_names = self._invoke(AnkiConnectCommand.GET_MODEL_NAMES)
-
-        if model.name in existing_model_names:  # type: ignore
-            self._invoke(
-                AnkiConnectCommand.UPDATE_MODEL_TEMPLATES,
-                model={
-                    "name": model.name,  # type: ignore
-                    "templates": {
-                        t["name"]: {"qfmt": t["qfmt"], "afmt": t["afmt"]}
-                        for t in model.templates  # type: ignore
-                    },
-                },
-            )
-            self._invoke(
-                AnkiConnectCommand.UPDATE_MODEL_STYLING,
-                model={"name": model.name, "css": model.css},  # type: ignore
-            )
-        else:
-            self._invoke(
-                AnkiConnectCommand.CREATE_MODEL,
-                modelName=model.name,  # type: ignore
-                inOrderFields=[field["name"] for field in model.fields],  # type: ignore
-                css=model.css,  # type: ignore
-                cardTemplates=[
-                    {"Name": t["name"], "Front": t["qfmt"], "Back": t["afmt"]}
+        self._invoke(
+            AnkiConnectCommand.UPDATE_MODEL_TEMPLATES,
+            model={
+                "name": model.name,  # type: ignore
+                "templates": {
+                    t["name"]: {"qfmt": t["qfmt"], "afmt": t["afmt"]}
                     for t in model.templates  # type: ignore
-                ],
-            )
+                },
+            },
+        )
+        self._invoke(
+            AnkiConnectCommand.UPDATE_MODEL_STYLING,
+            model={"name": model.name, "css": model.css},  # type: ignore
+        )
 
     def import_package(self, package: genanki.Package) -> None:
         subdir = "tmp_apkg_dir"
         with tempdir(self.tmp_write_dir / subdir) as tmp_write_subdir:
-            apkg_name = f"{datetime.datetime.now().strftime('%Y-%m-%d-%H-%M-%S')}.apkg"
+            apkg_name = (
+                f"{datetime.datetime.now().strftime('%Y-%m-%d-%H-%M-%S')}.apkg"
+            )
             package.write_to_file(tmp_write_subdir / apkg_name)  # type: ignore
 
             read_path = self.tmp_read_dir / subdir / apkg_name
             try:
-                self._invoke(AnkiConnectCommand.IMPORT_PACKAGE, path=str(read_path))
+                self._invoke(
+                    AnkiConnectCommand.IMPORT_PACKAGE, path=str(read_path)
+                )
                 log.info(f"Imported from {read_path}!")
             except Exception as e:
                 log.error(f"""Unable to sync from {read_path}, {e}""")
                 traceback.print_exc()
 
     def delete_notes(self, note_ids: Sequence[int]) -> None:
         if len(note_ids) > self.max_deletions_per_run:
@@ -166,27 +156,32 @@
         Args:
             action (string): the action to invoke
         Raises:
             Exception: invalid fields provided
         Returns:
             Any: the response from anki connect
         """
-        requestJson = json.dumps(self._request(action.value, **params)).encode("utf-8")
+        requestJson = json.dumps(self._request(action.value, **params)).encode(
+            "utf-8"
+        )
         response = json.load(
-            urllib.request.urlopen(urllib.request.Request(self.ankiconnect_url, requestJson))
+            urllib.request.urlopen(
+                urllib.request.Request(self.ankiconnect_url, requestJson)
+            )
         )
         if len(response) != 2:
             raise Exception("response has an unexpected number of fields")
         if response["error"] is not None:
             raise Exception(response["error"])
         return response["result"]
 
 
 @dataclass(frozen=True)
-class FakeAnkiCommand: ...
+class FakeAnkiCommand:
+    ...
 
 
 @dataclass(frozen=True)
 class ImportPackage(FakeAnkiCommand):
     package: genanki.Package
 
 
@@ -207,15 +202,19 @@
     def get_all_note_infos(self) -> Sequence[NoteInfo]:
         return self.note_infos
 
     def import_package(self, package: genanki.Package) -> None:
         self.executed_commands.append(ImportPackage(package=package))
 
 
-ANKICONNECT_URL = "http://host.docker.internal:8765" if in_docker() else "http://localhost:8765"
+ANKICONNECT_URL = (
+    "http://host.docker.internal:8765"
+    if in_docker()
+    else "http://localhost:8765"
+)
 # On host machine, port is 8765
 
 
 def anki_connect_is_live(ankiconnect_url: str = ANKICONNECT_URL) -> bool:
     try:
         if urllib.request.urlopen(ankiconnect_url).getcode() == 200:
             return True
```

### Comparing `memium-0.19.0/memium/destination/ankiconnect/test_anki_converter.py` & `memium-0.7.0/memium/destination/ankiconnect/test_anki_converter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 import pytest
 
 from ...source.prompts.prompt import BasePrompt
 from ...source.prompts.prompt_cloze import ClozeWithoutDoc
 from ...source.prompts.prompt_qa import QAWithoutDoc
+from .anki_card import AnkiCard
 from .anki_converter import AnkiPromptConverter
-from .anki_prompt import AnkiPrompt
-from .test_anki_prompt_qa import FakeAnkiCloze, FakeAnkiQA
+from .anki_prompt_cloze import AnkiCloze
+from .anki_prompt_qa import AnkiQA
+
+fake_anki_qa = AnkiQA(
+    question="FakeQuestion",
+    answer="FakeAnswer",
+    base_deck="FakeDeck",
+    tags=["FakeTag"],
+    css="FakeCSS",
+)
+
+fake_anki_cloze = AnkiCloze(
+    text="FakeText", base_deck="FakeDeck", tags=["FakeTag"], css="FakeCSS"
+)
 
 
 @pytest.mark.parametrize(
     ("input_prompt", "expected_card"),
     [
         (
-            QAWithoutDoc(question="FakeQuestion", answer="FakeAnswer", add_tags=["FakeTag"]),
-            FakeAnkiQA(
-                uuid=4875918425
-            ),  # Ensure that UUID generation remains stable to retain idempotency over time
+            QAWithoutDoc(
+                question="FakeQuestion",
+                answer="FakeAnswer",
+                add_tags=["FakeTag"],
+            ),
+            fake_anki_qa,
         ),
         (
             ClozeWithoutDoc(text="FakeText", add_tags=["FakeTag"]),
-            FakeAnkiCloze(
-                uuid=1873301177
-            ),  # Ensure that UUID generation remains stable to retain idempotency over time
+            fake_anki_cloze,
         ),
     ],
 )
-def test_anki_prompt_converter(input_prompt: BasePrompt, expected_card: AnkiPrompt):
+def test_anki_prompt_converter(
+    input_prompt: BasePrompt, expected_card: AnkiCard
+):
     """Tests the AnkiPromptConverter class"""
-    generated_card = AnkiPromptConverter(
-        base_deck="FakeBaseDeck", card_css="FakeCSS"
-    ).prompt_to_card(input_prompt)
+    card = AnkiPromptConverter(
+        base_deck="FakeDeck", card_css="FakeCSS"
+    ).prompts_to_cards([input_prompt])[0]
 
-    assert generated_card.uuid == expected_card.uuid
+    assert card.uuid == expected_card.uuid
+    for attr in expected_card.__dict__:
+        assert getattr(card, attr) == getattr(expected_card, attr)
```

### Comparing `memium-0.19.0/memium/destination/ankiconnect/test_ankiconnect_gateway.py` & `memium-0.7.0/memium/data_access/test_ankiconnect_gateway.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from collections.abc import Mapping, Sequence
 from pathlib import Path
 
 import genanki
 import pytest
 
-from ...environment import get_host_home_dir
 from .ankiconnect_gateway import (
     ANKICONNECT_URL,
     AnkiConnectGateway,
     AnkiField,
     NoteInfo,
     anki_connect_is_live,
 )
+from .environment import get_host_home_dir
 
 
 class MockNoteInfo(NoteInfo):
     noteId: int = 1
     tags: Sequence[str] = ["MockTag"]
-    fields: Mapping[str, AnkiField] = {"Text": AnkiField(value="MockText", order=0)}
+    fields: Mapping[str, AnkiField] = {
+        "Text": AnkiField(value="MockText", order=0)
+    }
     modelName: str = "MockModel"
     cards: Sequence[int] = [1]
 
 
 @pytest.mark.skipif(
-    not anki_connect_is_live() or not Path("/output").exists(),
-    reason="Tests require a running AnkiConnect server and an output directory. Use the Docker container to run the tests.",
+    not anki_connect_is_live(),
+    reason="Tests require a running AnkiConnect server",
 )
 class TestAnkiConnectGateway:
     output_path = Path("/output")
 
     def test_import_get_delete_happy_path(self):
         # Delete all .apkg in the output directory
         for f in self.output_path.glob("*.apkg"):
@@ -47,15 +49,17 @@
                 }
             ],
         )
 
         deck.add_model(model)  # type: ignore
         deck.add_note(  # type: ignore
             genanki.Note(
-                model=model, fields=["Capital of Argentina", "Buenos Aires"], tags=["TestTag"]
+                model=model,
+                fields=["Capital of Argentina", "Buenos Aires"],
+                tags=["TestTag"],
             )
         )
 
         tmp_read_dir = get_host_home_dir() / "ankidecks"
         gateway = AnkiConnectGateway(
             ankiconnect_url=ANKICONNECT_URL,
             base_deck="Test deck",
```

### Comparing `memium-0.19.0/memium/destination/destination_ankiconnect.py` & `memium-0.7.0/memium/destination/destination_ankiconnect.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,104 @@
-import logging
-from collections.abc import Sequence
+from collections.abc import Mapping, Sequence
 
 import genanki
-from iterpy import Iter
+from functionalpy._sequence import Seq
 
+from ..data_access.ankiconnect_gateway import AnkiConnectGateway, NoteInfo
 from ..source.prompts.prompt import DestinationPrompt
-from ..utils.hash_cleaned_str import clean_str, hash_str_to_int
+from ..source.prompts.prompt_cloze import ClozeWithoutDoc
+from ..source.prompts.prompt_qa import QAWithoutDoc
+from ..utils.hash_cleaned_str import hash_cleaned_str
+from .ankiconnect.anki_card import AnkiCard
 from .ankiconnect.anki_converter import AnkiPromptConverter
-from .ankiconnect.anki_prompt import AnkiPrompt
-from .ankiconnect.ankiconnect_gateway import AnkiConnectGateway
-from .destination import DeletePrompts, PromptDestination, PromptDestinationCommand, PushPrompts
-
-log = logging.getLogger(__name__)
+from .destination import PromptDestination
+from .destination_commands import (
+    DeletePrompts,
+    PromptDestinationCommand,
+    PushPrompts,
+)
 
 
 class AnkiConnectDestination(PromptDestination):
-    def __init__(self, gateway: AnkiConnectGateway, prompt_converter: AnkiPromptConverter) -> None:
+    def __init__(
+        self, gateway: AnkiConnectGateway, prompt_converter: AnkiPromptConverter
+    ) -> None:
         self.gateway = gateway
         self.prompt_converter = prompt_converter
 
+    def _note_info_to_prompt(self, note_info: NoteInfo) -> DestinationPrompt:
+        if "Question" in note_info.fields and "Answer" in note_info.fields:
+            return DestinationPrompt(
+                QAWithoutDoc(
+                    question=note_info.fields["Question"].value,
+                    answer=note_info.fields["Answer"].value,
+                    add_tags=note_info.tags,
+                ),
+                destination_id=str(note_info.noteId),
+            )
+
+        if "Text" in note_info.fields:
+            return DestinationPrompt(
+                ClozeWithoutDoc(
+                    text=note_info.fields["Text"].value, add_tags=note_info.tags
+                ),
+                destination_id=str(note_info.noteId),
+            )
+
+        raise ValueError(
+            f"NoteInfo {note_info} has neither Question nor Text field"
+        )
+
     def get_all_prompts(self) -> Sequence[DestinationPrompt]:
         return (
-            Iter(self.gateway.get_all_note_infos())
-            .map(self.prompt_converter.note_info_to_prompt)
+            Seq(self.gateway.get_all_note_infos())
+            .map(self._note_info_to_prompt)
             .to_list()
         )
 
     def _delete_prompts(self, prompts: Sequence[DestinationPrompt]) -> None:
-        prompt_ids = {int(remote_prompt.destination_id) for remote_prompt in prompts}
+        prompt_ids = {
+            int(remote_prompt.destination_id) for remote_prompt in prompts
+        }
         self.gateway.delete_notes(list(prompt_ids))
 
     def _grouped_cards_to_deck(
-        self, grouped_cards: tuple[str, Sequence[AnkiPrompt]]
+        self, grouped_cards: Mapping[str, Sequence[AnkiCard]]
     ) -> genanki.Deck:
-        deck_name = grouped_cards[0]
-        deck = genanki.Deck(name=deck_name, deck_id=hash_str_to_int(clean_str(deck_name)))
+        deck_name = next(iter(grouped_cards.keys()))
+        deck = genanki.Deck(name=deck_name, deck_id=hash_cleaned_str(deck_name))
 
-        for card in grouped_cards[1]:
+        for card in grouped_cards[deck_name]:
             deck.add_note(card.to_genanki_note())  # type: ignore
 
         return deck
 
-    def _create_package(self, cards: Sequence[AnkiPrompt]) -> genanki.Package:
-        decks = (
-            Iter(cards).groupby(lambda card: card.deck).map(self._grouped_cards_to_deck).to_list()
-        )
+    def _create_package(self, cards: Sequence[AnkiCard]) -> genanki.Package:
+        cards_grouped_by_deck = Seq(cards).groupby(lambda card: card.deck)
+        decks = [
+            self._grouped_cards_to_deck({group: cards_grouped_by_deck[group]})
+            for group in cards_grouped_by_deck
+        ]
 
         return genanki.Package(deck_or_decks=decks)
 
     def _push_prompts(self, command: PushPrompts) -> None:
-        cards = [self.prompt_converter.prompt_to_card(e) for e in command.prompts]
+        cards = self.prompt_converter.prompts_to_cards(command.prompts)
 
         models = [card.genanki_model for card in cards]
         unique_models: dict[int, genanki.Model] = {
             model.model_id: model  # type: ignore
             for model in models  # type: ignore
         }
 
         for model in unique_models.values():
             self.gateway.update_model(model)
 
         package = self._create_package(cards)
 
-        log.info(f"Pushing {len(cards)} cards to Anki")
         self.gateway.import_package(package)
 
     def update(self, commands: Sequence[PromptDestinationCommand]) -> None:
         for command in commands:
             match command:
                 case DeletePrompts(prompts):
                     self._delete_prompts(prompts)
```

### Comparing `memium-0.19.0/memium/destination/destination_dryrun.py` & `memium-0.7.0/memium/destination/destination_dryrun.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import logging
 from collections.abc import Sequence
 
-from .destination import DeletePrompts, PromptDestinationCommand, PushPrompts
 from .destination_ankiconnect import AnkiConnectDestination
+from .destination_commands import (
+    DeletePrompts,
+    PromptDestinationCommand,
+    PushPrompts,
+)
 
 log = logging.getLogger(__name__)
 
 
 class DryRunDestination(AnkiConnectDestination):
     def update(self, commands: Sequence[PromptDestinationCommand]) -> None:
         for command in commands:
```

### Comparing `memium-0.19.0/memium/destination/test_destination_ankiconnect.py` & `memium-0.7.0/memium/destination/test_destination_ankiconnect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 from collections.abc import Mapping
 
 import pytest
 
-from ..source.prompts.prompt_cloze import ClozeWithoutDoc
-from ..source.prompts.prompt_qa import QAWithoutDoc
-from .ankiconnect.anki_converter import AnkiPromptConverter
-from .ankiconnect.ankiconnect_gateway import (
+from ..data_access.ankiconnect_gateway import (
     AnkiField,
     ImportPackage,
     SpieAnkiconnectGateway,
     UpdateModel,
 )
-from .ankiconnect.test_ankiconnect_gateway import MockNoteInfo
-from .destination import PushPrompts
+from ..data_access.test_ankiconnect_gateway import MockNoteInfo
+from ..source.prompts.prompt_cloze import ClozeWithoutDoc
+from ..source.prompts.prompt_qa import QAWithoutDoc
+from .ankiconnect.anki_converter import AnkiPromptConverter
 from .destination_ankiconnect import AnkiConnectDestination
+from .destination_commands import PushPrompts
 
 
 @pytest.mark.parametrize(
     ("fields"),
     [
         ({"Text": AnkiField(value="MockText", order=0)}),
         (
             {
                 "Question": AnkiField(value="MockQuestion", order=0),
                 "Answer": AnkiField(value="MockAnswer", order=1),
             }
         ),
         pytest.param(
-            ({"UnknownField": AnkiField(value="MockText", order=0)}), marks=pytest.mark.xfail
+            ({"UnknownField": AnkiField(value="MockText", order=0)}),
+            marks=pytest.mark.xfail,
         ),
     ],
 )
 def test_ankiconnect_get_all_prompts(fields: Mapping[str, AnkiField]):
     dest = AnkiConnectDestination(
-        gateway=SpieAnkiconnectGateway(note_infos=[MockNoteInfo(fields=fields)]),
-        prompt_converter=AnkiPromptConverter(base_deck="FakeDeck", card_css="FakeCSS"),
+        gateway=SpieAnkiconnectGateway(
+            note_infos=[MockNoteInfo(fields=fields)]
+        ),
+        prompt_converter=AnkiPromptConverter(
+            base_deck="FakeDeck", card_css="FakeCSS"
+        ),
     )
     prompts = dest.get_all_prompts()
 
     assert len(prompts) == 1
 
 
 def test_ankiconnect_push_prompts():
     gateway = SpieAnkiconnectGateway()
     dest = AnkiConnectDestination(
         gateway=gateway,
-        prompt_converter=AnkiPromptConverter(base_deck="FakeDeck", card_css="FakeCSS"),
+        prompt_converter=AnkiPromptConverter(
+            base_deck="FakeDeck", card_css="FakeCSS"
+        ),
     )
     dest.update(
         [
             PushPrompts(
                 prompts=[
                     QAWithoutDoc(
                         question="FakeQuestion",
@@ -70,9 +77,16 @@
         import_package_command.package.decks[0].name  # type: ignore
         == "FakeDeck::FakeSubdeck::FakeSubSubdeck"
     )
     assert len(import_package_command.package.decks) == 2  # type: ignore
 
     for command in expected_commands:
         assert (
-            len([c for c in gateway.executed_commands if isinstance(c, command[0])]) == command[1]
+            len(
+                [
+                    c
+                    for c in gateway.executed_commands
+                    if isinstance(c, command[0])
+                ]
+            )
+            == command[1]
         )
```

### Comparing `memium-0.19.0/memium/diff_determiner.py` & `memium-0.7.0/memium/diff_determiner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,73 @@
 from collections.abc import Mapping, Sequence
 from dataclasses import dataclass
 from typing import Generic, Protocol, TypeVar
 
-from .destination.destination import DeletePrompts, PromptDestinationCommand, PushPrompts
+from .destination.destination_commands import (
+    DeletePrompts,
+    PromptDestinationCommand,
+    PushPrompts,
+)
 from .source.prompts.prompt import BasePrompt, DestinationPrompt
 
 K = TypeVar("K")
 T = TypeVar("T")
 S = TypeVar("S")
 
 
 class BaseDiffDeterminer(Protocol):
     def sync(
-        self, source_prompts: Sequence[BasePrompt], destination_prompts: Sequence[DestinationPrompt]
-    ) -> Sequence[PromptDestinationCommand]: ...
+        self,
+        source_prompts: Sequence[BasePrompt],
+        destination_prompts: Sequence[DestinationPrompt],
+    ) -> Sequence[PromptDestinationCommand]:
+        ...
 
 
 @dataclass(frozen=True)
 class GeneralSyncer(Generic[K, T, S]):
     source: Mapping[K, T]
     destination: Mapping[K, S]
 
     def only_in_source(self) -> Sequence[T]:
-        return [value for key, value in self.source.items() if key not in self.destination]
+        return [
+            value
+            for key, value in self.source.items()
+            if key not in self.destination
+        ]
 
     def only_in_destination(self) -> Sequence[S]:
-        return [value for key, value in self.destination.items() if key not in self.source]
+        return [
+            value
+            for key, value in self.destination.items()
+            if key not in self.source
+        ]
 
 
 class PromptDiffDeterminer(BaseDiffDeterminer):
     def sync(
-        self, source_prompts: Sequence[BasePrompt], destination_prompts: Sequence[DestinationPrompt]
+        self,
+        source_prompts: Sequence[BasePrompt],
+        destination_prompts: Sequence[DestinationPrompt],
     ) -> Sequence[PromptDestinationCommand]:
         # Update prompts if content or tags have changed. This doesn't affect scheduling.
         prompts_to_update = GeneralSyncer(
             source={prompt.update_uid: prompt for prompt in source_prompts},
-            destination={prompt.prompt.update_uid: prompt for prompt in destination_prompts},
+            destination={
+                prompt.prompt.update_uid: prompt
+                for prompt in destination_prompts
+            },
         ).only_in_source()
 
         # Only delete prompts whose content have changed. This essentially resets their scheduling.
         prompts_to_delete = GeneralSyncer(
             source={prompt.scheduling_uid: prompt for prompt in source_prompts},
             destination={
                 dest_prompt.prompt.scheduling_uid: dest_prompt
                 for dest_prompt in destination_prompts
             },
         ).only_in_destination()
 
-        return [DeletePrompts(prompts_to_delete), PushPrompts(prompts_to_update)]
+        return [
+            DeletePrompts(prompts_to_delete),
+            PushPrompts(prompts_to_update),
+        ]
```

### Comparing `memium-0.19.0/memium/environment.py` & `memium-0.7.0/memium/data_access/environment.py`

 * *Files identical despite different names*

### Comparing `memium-0.19.0/memium/source/extractors/extractor_cloze.py` & `memium-0.7.0/memium/source/extractors/extractor_cloze.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,85 +8,73 @@
 from .extractor import BasePromptExtractor
 
 log = logging.getLogger(__name__)
 
 
 class ClozePromptExtractor(BasePromptExtractor):
     @staticmethod
-    def _get_blocks(string: str) -> list[str]:
+    def _break_string_by_two_or_more_newlines(string: str) -> list[str]:
         """Break string into a list by 2+ newlines in a row."""
-        # Exclude entire code blocks
-        string_sans_code_blocks = re.sub(r"```.*?```", "", string, flags=re.DOTALL)
-        return re.split(r"(\n\n)+", string_sans_code_blocks)
+        return re.split(r"(\n\n)+", string)
 
     @staticmethod
     def _has_cloze(string: str) -> bool:
-        if len(re.findall(r"{.*}", string)) > 0:
+        if (
+            len(re.findall(r"{.*}", string)) > 0
+            and "BearID" not in string  # Exclude BearID
+            and "$$" not in string  # Exclude math
+            and r"```" not in string  # Exclude code
+            and "Q." not in string  # Exclude Q&A
+            and "A." not in string  # Exclude Q&A
+        ):
             return True
         return False
 
     @staticmethod
-    def _is_math_block(string: str) -> bool:
-        if string.startswith("$$"):
-            return True
-        return False
-
-    @staticmethod
-    def _is_html_comment(string: str) -> bool:
-        if string.startswith("<!--"):
-            return True
-        return False
-
-    @staticmethod
-    def _replace_cloze_id_with_unique(string: str, selected_cloze: str | None = None) -> str:
+    def _replace_cloze_id_with_unique(
+        string: str, selected_cloze: str | None = None
+    ) -> str:
         """Each cloze deletion in a note is numbered sequentially.
 
         This function ensures that the numbering is based on the content of the cloze deletion, essentially ensuring that if you modify the contents of a cloze, only the scheduling of that specific cloze is changed.
 
         Args:
             string (str): The string to replace the cloze id with a unique id.
             selected_cloze (str, optional): If you only want to replace a specific cloze, pass it here. Defaults to None.
         """
         if selected_cloze is not None:
             selected_clozes = [selected_cloze]
         else:
             selected_clozes = re.findall(r"{(?!BearID).[^}]*}", string)
 
         for cloze in selected_clozes:
-            output_hash = int(hashlib.sha256(cloze.encode("utf-8")).hexdigest(), 16) % 10**3
+            output_hash = (
+                int(hashlib.sha256(cloze.encode("utf-8")).hexdigest(), 16)
+                % 10**3
+            )
 
             new_cloze = f"{{{{c{output_hash}::{cloze[1:-1]}}}}}"
 
             string = string.replace(cloze, new_cloze)
 
         return string
 
     def extract_prompts(self, document: Document) -> Sequence[ClozePrompt]:
         prompts: list[ClozeFromDoc] = []
-        blocks = self._get_blocks(document.content)
 
-        block_starting_line_nr = 1
-        for block_string in blocks:
-            if any(
-                exclusion_criterion(block_string)
-                for exclusion_criterion in (self._is_html_comment, self._is_math_block)
-            ):
-                continue
+        blocks = self._break_string_by_two_or_more_newlines(document.content)
 
+        for block_string in blocks:
             if self._has_cloze(block_string):
                 clozes = re.findall(r"{(?!BearID).[^}]*}", block_string)
 
+                # TODO: https://github.com/MartinBernstorff/memium/issues/300 refactor: move clozeid replacement to AnkiCloze generator class
                 for selected_cloze in clozes:
                     prompt_content = self._replace_cloze_id_with_unique(
                         block_string, selected_cloze=selected_cloze
                     )
 
                     prompts.append(
-                        ClozeFromDoc(
-                            text=prompt_content, parent_doc=document, line_nr=block_starting_line_nr
-                        )
+                        ClozeFromDoc(text=prompt_content, source_doc=document)
                     )
 
-            n_block_lines = len(re.findall(r"\n", block_string, flags=re.DOTALL))
-            block_starting_line_nr += n_block_lines
-
         return prompts
```

### Comparing `memium-0.19.0/memium/source/extractors/extractor_qa.py` & `memium-0.7.0/memium/source/extractors/extractor_qa.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,58 +12,68 @@
 class QAPromptExtractor(BasePromptExtractor):
     def __init__(self, question_prefix: str, answer_prefix: str) -> None:
         self.question_prefix = question_prefix
         self.answer_prefix = answer_prefix
 
     def _get_first_question(self, content: str) -> str:
         question = re.findall(
-            self.question_prefix + r"{0,1}\.(?:(?!A\.).)*", content, flags=re.DOTALL
+            self.question_prefix + r"{0,1}\.(?:(?!A\.).)*",
+            content,
+            flags=re.DOTALL,
         )[0]
 
         return question[len(self.question_prefix) + 1 :].rstrip()
 
     def _get_first_answer(self, content: str) -> str:
         # Have to use positive lookahead to match code-blocks
         # To ensure the last answer is matched as well, we add 2 newlines to string.
         string_padded = f"{content.rstrip()}\n\n"
 
-        answer = re.findall(r"\n" + self.answer_prefix + r"[ \n]+\n*.+", string_padded, re.DOTALL)[
-            0
-        ]
+        answer = re.findall(
+            r"\n" + self.answer_prefix + r"[ \n]+\n*.+",
+            string_padded,
+            re.DOTALL,
+        )[0]
 
         return answer[len(self.answer_prefix) + 2 :].rstrip()
 
     @staticmethod
     def _string_to_blocks_by_newlines(string: str) -> list[str]:
         """Break string into a list by 2+ newlines in a row."""
         return re.split(r"(\n\n)+", string)
 
     def _has_qa(self, string: str) -> bool:
         """Check whether a string contains a qa prompt"""
         return (
             len(
                 re.findall(
-                    r"^(?![:>]).*" + self.question_prefix + r"{0,1}\. ", string, flags=re.DOTALL
+                    r"^(?![:>]).*" + self.question_prefix + r"{0,1}\. ",
+                    string,
+                    flags=re.DOTALL,
                 )
             )
             != 0
         )
 
     def extract_prompts(self, document: Document) -> Sequence[QAPrompt]:
         prompts: list[QAPrompt] = []
+
         blocks = self._string_to_blocks_by_newlines(document.content)
+
         block_starting_line_nr = 1
 
         for block_string in blocks:
             if self._has_qa(block_string):
                 question = self._get_first_question(block_string)
                 try:
                     answer = self._get_first_answer(block_string)
                 except IndexError:
-                    logging.warn(f"Could not find answer in {document.title} for {question}")
+                    logging.warn(
+                        f"Could not find answer in {document.title} for {question}"
+                    )
                     continue
 
                 prompts.append(
                     QAFromDoc(
                         question=question,
                         answer=answer,
                         parent_doc=document,
```

### Comparing `memium-0.19.0/memium/source/extractors/test_prompt_extractor_qa.py` & `memium-0.7.0/memium/source/extractors/test_prompt_extractor_qa.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 
 #anki/tag/test_tag
 
 """,
         source_path=tmpdir / "test.md",
     )
 
-    extractor = QAPromptExtractor(question_prefix="Q.", answer_prefix="A.").extract_prompts(doc)
+    extractor = QAPromptExtractor(
+        question_prefix="Q.", answer_prefix="A."
+    ).extract_prompts(doc)
 
     assert len(extractor) == 1
     prompt = extractor[0]
     assert prompt.question == "What is the meaning of life?"
     assert prompt.answer == "42"
     assert prompt.tags == ["anki/tag/test_tag"]
-    assert prompt.scheduling_uid == 3643087944
+    assert prompt.scheduling_uid == 9385242780
```

### Comparing `memium-0.19.0/memium/source/prompts/prompt_cloze.py` & `memium-0.7.0/memium/source/prompts/prompt_cloze.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 from collections.abc import Sequence
 from dataclasses import dataclass
 
-from ...utils.hash_cleaned_str import clean_str, hash_str_to_int
+from ...utils.hash_cleaned_str import clean_str, hash_cleaned_str, int_hash_str
+from ..document import Document
 from .prompt import BasePrompt
-from .prompt_from_doc import PromptFromDocMixin
 
 
 @dataclass(frozen=True)
 class ClozePrompt(BasePrompt):
     text: str
 
     @property
     def scheduling_uid(self) -> int:
-        return hash_str_to_int(clean_str(self.text))
+        return hash_cleaned_str(self.text)
 
     @property
     def update_uid(self) -> int:
-        return hash_str_to_int(f"{(self.text)}{self.tags}")
+        return int_hash_str(f"{clean_str(self.text)}{self.tags}")
 
     @property
     def tags(self) -> Sequence[str]:
         return ()
 
 
 @dataclass(frozen=True)
 class ClozeWithoutDoc(ClozePrompt):
     add_tags: Sequence[str]
 
     @property
     def tags(self) -> Sequence[str]:
         return self.add_tags
 
-    @property
-    def edit_url(self) -> str | None:
-        return None
-
 
 @dataclass(frozen=True)
-class ClozeFromDoc(ClozePrompt, PromptFromDocMixin):
+class ClozeFromDoc(ClozePrompt):
     text: str
+    source_doc: Document
+
+    @property
+    def scheduling_uid(self) -> int:
+        return int_hash_str(self.text)
 
     @property
     def tags(self) -> Sequence[str]:
-        return self.parent_doc.tags
+        return self.source_doc.tags
```

### Comparing `memium-0.19.0/memium/source/prompts/prompt_qa.py` & `memium-0.7.0/memium/source/prompts/prompt_qa.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,46 @@
 from collections.abc import Sequence
 from dataclasses import dataclass
 
-from ...utils.hash_cleaned_str import clean_str, hash_str_to_int
+from ...utils.hash_cleaned_str import hash_cleaned_str
+from ..document import Document
 from .prompt import BasePrompt
-from .prompt_from_doc import PromptFromDocMixin
 
 
 @dataclass(frozen=True)
 class QAPrompt(BasePrompt):
     question: str
     answer: str
 
     @property
-    def scheduling_uid_str(self) -> str:
-        """Str used for generating the update_uid. Super helpful for debugging."""
-        return f"{clean_str(self.question)}_{clean_str(self.answer)}"
-
-    @property
     def scheduling_uid(self) -> int:
-        return hash_str_to_int(self.scheduling_uid_str)
-
-    @property
-    def update_uid_str(self) -> str:
-        """Str used for generating the update_uid. Super helpful for debugging."""
-        return f"{self.question}_{self.answer}_{self.tags}"
+        return hash_cleaned_str(f"{self.question}_{self.answer}")
 
     @property
     def update_uid(self) -> int:
-        return hash_str_to_int(self.update_uid_str)
+        return hash_cleaned_str(f"{self.question}_{self.answer}_{self.tags}")
 
     @property
     def tags(self) -> Sequence[str]:
         return ()
 
 
 @dataclass(frozen=True)
 class QAWithoutDoc(QAPrompt):
     add_tags: Sequence[str]
 
     @property
     def tags(self) -> Sequence[str]:
         return self.add_tags
 
-    @property
-    def edit_url(self) -> str | None:
-        return None
-
 
 @dataclass(frozen=True)
-class QAFromDoc(QAPrompt, PromptFromDocMixin):
+class QAFromDoc(QAPrompt):
+    parent_doc: Document
+    line_nr: int
+
+    def __repr__(self) -> str:
+        return f"{self.parent_doc.source_path}:{self.line_nr}: \n\tQ. {self.question}\n\tA. {self.answer}"
+
     @property
     def tags(self) -> Sequence[str]:
         return self.parent_doc.tags
```

### Comparing `memium-0.19.0/memium/source/test_facade.py` & `memium-0.7.0/memium/source/test_facade.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from collections.abc import Sequence
 from pathlib import Path
 
 from .document import Document
-from .document_source import BaseDocumentSource
+from .document_ingester import BaseDocumentIngester
 from .extractors.extractor_qa import QAPromptExtractor
-from .prompt_source import DocumentPromptSource
+from .facade import DocumentPromptSource
 
 
 def test_document_prompt_source():
     source = DocumentPromptSource(
         document_ingester=FakeDocumentIngester(
             [
                 Document(
                     """Q. What is a test even?
 A. Nothing""",
                     Path("test.md"),
                 )
             ]
         ),
-        prompt_extractors=[QAPromptExtractor(question_prefix="Q.", answer_prefix="A.")],
+        prompt_extractors=[
+            QAPromptExtractor(question_prefix="Q.", answer_prefix="A.")
+        ],
     )
     prompts = source.get_prompts()
     assert len(prompts) == 1
 
 
-class FakeDocumentIngester(BaseDocumentSource):
+class FakeDocumentIngester(BaseDocumentIngester):
     def __init__(self, documents: Sequence[Document]):
         self.documents = documents
 
     def get_documents(self) -> Sequence[Document]:
         return self.documents
```

### Comparing `memium-0.19.0/memium/tasks/github.py` & `memium-0.7.0/memium/subtasks/github.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import json
 from collections.abc import Sequence
 from dataclasses import dataclass
 from time import sleep
 
 import invoke as inv
 
-from .str_parsing import get_letter_alphabet_position, get_letter_from_alphabet_position
+from .str_parsing import (
+    get_letter_alphabet_position,
+    get_letter_from_alphabet_position,
+)
 
 
 @dataclass(frozen=True)
 class GithubIssue:
     number: int
     title: str
 
 
 def get_issues_assigned_to_me(c: inv.Context) -> Sequence[GithubIssue] | None:
     """Get issues assigned to current user on current repo"""
-    my_issues_cmd = c.run("gh issue list --assignee='@me' --json number,title", hide="out")
+    my_issues_cmd = c.run(
+        "gh issue list --assignee='@me' --json number,title", hide="out"
+    )
 
     if my_issues_cmd is None:
         return None
 
-    parsed_output = [GithubIssue(**value) for value in json.loads(my_issues_cmd.stdout)]
+    parsed_output = [
+        GithubIssue(**value) for value in json.loads(my_issues_cmd.stdout)
+    ]
     return parsed_output
 
 
 def issue_dialog(my_issues: Sequence[GithubIssue]) -> int:
     issue_strings = [
         f"[{get_letter_from_alphabet_position(i+1)}] #{issue.number} {issue.title}"
         for i, issue in enumerate(my_issues)
@@ -43,15 +50,17 @@
     terminal_output = "\n".join(reversed(issue_strings))
     print(f"\n{terminal_output}\n")
 
     print(f"Latest [a] is: \n\t {my_issues[0].title}\n")
     print("I found these issues for you. Which do you want to work on?\n")
 
     issue_index = (
-        get_letter_alphabet_position(input(f"[a-{get_letter_from_alphabet_position(n_issues)}]: "))
+        get_letter_alphabet_position(
+            input(f"[a-{get_letter_from_alphabet_position(n_issues)}]: ")
+        )
         - 1
     )
 
     return issue_index
 
 
 def sanitise_issue_title(issue_title: str) -> str:
```

### Comparing `memium-0.19.0/memium/tasks/graphite.py` & `memium-0.7.0/memium/subtasks/graphite.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import invoke as inv
 
 from .github import GithubIssue, sanitise_issue_title
 
 
 @inv.task(aliases=("submit",))  # type: ignore
 def submit_pr(c: inv.Context):
-    c.run("gt submit --restack --stack --no-edit --publish --merge-when-ready")
+    c.run("gt submit -m --no-edit --publish")
     c.run("gt log short")
 
 
 def create_branch_from_issue(c: inv.Context, selected_issue: GithubIssue):
     sanitised_title = sanitise_issue_title(selected_issue.title)
     branch_title = f"{selected_issue.number}-{sanitised_title}"
-    first_commit_str = f"$'{selected_issue.title}\n\nFixes #{selected_issue.number}'"
+    first_commit_str = (
+        f"$'{selected_issue.title}\n\nFixes #{selected_issue.number}'"
+    )
     c.run(f"gt create {branch_title} --all -m {first_commit_str}")
     c.run(f"git commit --allow-empty -m {first_commit_str}")
```

### Comparing `memium-0.19.0/memium/tasks/smoketest.py` & `memium-0.7.0/memium/subtasks/smoketest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections.abc import Sequence
 from pathlib import Path
 
 import invoke as inv
 
-from memium.tasks.graphite import submit_pr  # noqa: F401 # type: ignore
+from memium.subtasks.graphite import submit_pr  # noqa: F401 # type: ignore
 
 
 def get_code_blocks_from_md(md_path: Path) -> Sequence[str]:
     md = md_path.read_text()
     code_blocks = md.split("```")[1::2]
     return code_blocks
 
@@ -23,24 +23,31 @@
 
 
 @inv.task  # type: ignore
 def smoketest_docker(c: inv.Context):
     input_dir = create_smoketest_dir()
 
     code_blocks = get_code_blocks_from_md(Path("readme.md"))
-    docker_block = next(block for block in code_blocks if "docker run" in block).strip() + " \\\n"
+    docker_block = (
+        next(block for block in code_blocks if "docker run" in block).strip()
+        + " \\\n"
+    )
 
     # Only keep content after docker line
     docker_block = docker_block[docker_block.index("docker run") :]
     replaced_image_location = docker_block.replace(
         "ghcr.io/martinbernstorff/memium:latest", "memium"
     )
-    replaced_input_dir = replaced_image_location.replace("$INPUT_DIR", str(input_dir))
+    replaced_input_dir = replaced_image_location.replace(
+        "$INPUT_DIR", str(input_dir)
+    )
 
-    smoketest_docker_command = replaced_input_dir + "  --dry-run \\\n" + "  --skip-sync"
+    smoketest_docker_command = (
+        replaced_input_dir + "  --dry-run \\\n" + "  --skip-sync"
+    )
 
     print(smoketest_docker_command)
 
     c.run("docker build . -t memium:latest -f Dockerfile")
     c.run("docker volume create ankidecks")
     c.run(smoketest_docker_command)
     print("💨🎉 Smoketest complete")
@@ -49,11 +56,13 @@
 @inv.task  # type: ignore
 def smoketest_cli(c: inv.Context):
     smoketest_dir = create_smoketest_dir()
     code_blocks = get_code_blocks_from_md(Path("readme.md"))
     cli_block = next(block for block in code_blocks if "cli-block" in block)
     sanitised_cli_block = cli_block.splitlines()[1].replace("> ", "")
 
-    cli_smoketest_cmd = sanitised_cli_block.replace("[YOUR_INPUT_DIR]", str(smoketest_dir))
+    cli_smoketest_cmd = sanitised_cli_block.replace(
+        "[YOUR_INPUT_DIR]", str(smoketest_dir)
+    )
     print(cli_smoketest_cmd)
     c.run(cli_smoketest_cmd + "  --dry-run \\\n" + "  --skip-sync")
     print("💨🎉 Smoketest complete")
```

### Comparing `memium-0.19.0/memium/test_diff_determiner.py` & `memium-0.7.0/memium/test_diff_determiner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from collections.abc import Sequence
 
 import pytest
 
-from memium.source.extractors.test_prompt import FakeQAPrompt
-
-from .destination.destination import DeletePrompts, PushPrompts
+from .destination.destination_commands import DeletePrompts, PushPrompts
 from .diff_determiner import GeneralSyncer, PromptDiffDeterminer
 from .source.prompts.prompt import BasePrompt, DestinationPrompt
-from .source.prompts.prompt_qa import QAWithoutDoc
+from .source.prompts.prompt_qa import QAPrompt, QAWithoutDoc
 
 
 @pytest.fixture()
 def diff_determiner() -> PromptDiffDeterminer:
     return PromptDiffDeterminer()
 
 
 def test_diff_determiner():
-    syncer = GeneralSyncer(source={"a": 1, "b": 2}, destination={"b": "2", "c": "3"})
+    syncer = GeneralSyncer(
+        source={"a": 1, "b": 2}, destination={"b": "2", "c": "3"}
+    )
 
     assert syncer.only_in_source() == [1]
     assert syncer.only_in_destination() == ["3"]
 
 
 from dataclasses import dataclass
 
@@ -36,42 +36,58 @@
 
 @pytest.mark.parametrize(
     "example",
     [
         DiffDeterminerExample(
             example_title="Basic",
             source_prompts=[
-                FakeQAPrompt(question="a", answer="a"),
-                FakeQAPrompt(question="b", answer="b"),
+                QAPrompt(question="a", answer="a"),
+                QAPrompt(question="b", answer="b"),
             ],
             destination_prompts=[
-                DestinationPrompt(FakeQAPrompt(question="b", answer="b"), destination_id="2"),
-                DestinationPrompt(FakeQAPrompt(question="c", answer="c"), destination_id="3"),
+                DestinationPrompt(
+                    QAPrompt(question="b", answer="b"), destination_id="2"
+                ),
+                DestinationPrompt(
+                    QAPrompt(question="c", answer="c"), destination_id="3"
+                ),
             ],
             delete_prompts=[
-                DestinationPrompt(FakeQAPrompt(question="c", answer="c"), destination_id="3")
+                DestinationPrompt(
+                    QAPrompt(question="c", answer="c"), destination_id="3"
+                )
             ],
-            push_prompts=[FakeQAPrompt(question="a", answer="a")],
+            push_prompts=[QAPrompt(question="a", answer="a")],
         ),
         (
             DiffDeterminerExample(
                 example_title="Updated tags",
-                source_prompts=[QAWithoutDoc(question="a", answer="a", add_tags=["NewTag"])],
+                source_prompts=[
+                    QAWithoutDoc(question="a", answer="a", add_tags=["NewTag"])
+                ],
                 destination_prompts=[
                     DestinationPrompt(
-                        QAWithoutDoc(question="a", answer="a", add_tags=["OldTag"]),
+                        QAWithoutDoc(
+                            question="a", answer="a", add_tags=["OldTag"]
+                        ),
                         destination_id="1",
                     )
                 ],
                 delete_prompts=[],
-                push_prompts=[QAWithoutDoc(question="a", answer="a", add_tags=["NewTag"])],
+                push_prompts=[
+                    QAWithoutDoc(question="a", answer="a", add_tags=["NewTag"])
+                ],
             )
         ),
     ],
 )
 def test_prompt_diff_determiner(
     diff_determiner: PromptDiffDeterminer, example: DiffDeterminerExample
 ):
     diff = diff_determiner.sync(
-        source_prompts=example.source_prompts, destination_prompts=example.destination_prompts
+        source_prompts=example.source_prompts,
+        destination_prompts=example.destination_prompts,
     )
-    assert diff == [DeletePrompts(example.delete_prompts), PushPrompts(example.push_prompts)]
+    assert diff == [
+        DeletePrompts(example.delete_prompts),
+        PushPrompts(example.push_prompts),
+    ]
```

### Comparing `memium-0.19.0/memium.egg-info/PKG-INFO` & `memium-0.7.0/memium.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,50 @@
 Metadata-Version: 2.1
 Name: memium
-Version: 0.19.0
+Version: 0.7.0
 Summary: Memium
 Author-email: Martin Bernstorff <martinbernstorff@gmail.com>
 Project-URL: homepage, https://github.com/MartinBernstorff/memium
 Project-URL: repository, https://github.com/MartinBernstorff/memium
 Project-URL: documentation, https://MartinBernstorff.github.io/memium/
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: cffi==1.16.0
-Requires-Dist: iterpy==1.9.0
+Requires-Dist: functionalpy==0.14.0
 Requires-Dist: genanki==0.13.1
-Requires-Dist: markdown==3.6
-Requires-Dist: pydantic==2.7.0
-Requires-Dist: sentry-sdk==1.45.0
-Requires-Dist: typer==0.12.3
-Requires-Dist: tqdm==4.66.2
-Requires-Dist: unidecode==1.3.8
+Requires-Dist: misaka==2.1.1
+Requires-Dist: pydantic==2.5.3
+Requires-Dist: sentry-sdk==1.39.1
+Requires-Dist: typer==0.9.0
+Requires-Dist: tqdm==4.66.1
 Requires-Dist: wasabi==1.1.2
-Requires-Dist: bs4==0.0.1
-Provides-Extra: tests
-Requires-Dist: pytest==7.4.4; extra == "tests"
-Requires-Dist: pytest-cov==5.0.0; extra == "tests"
-Requires-Dist: pytest-xdist==3.6.0; extra == "tests"
-Requires-Dist: pytest-sugar==1.0.0; extra == "tests"
-Requires-Dist: pytest-testmon==2.1.1; extra == "tests"
-Requires-Dist: diff-cover==9.0.0; extra == "tests"
-Requires-Dist: syrupy==4.6.1; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: cruft==2.15.0; extra == "dev"
-Requires-Dist: herbarium; extra == "dev"
 Requires-Dist: invoke==2.2.0; extra == "dev"
-Requires-Dist: pyright==1.1.359; extra == "dev"
-Requires-Dist: pre-commit==3.7.0; extra == "dev"
-Requires-Dist: ruff==0.4.1; extra == "dev"
-Requires-Dist: lumberman; extra == "dev"
+Requires-Dist: pyright==1.1.343; extra == "dev"
+Requires-Dist: pre-commit==3.6.0; extra == "dev"
+Requires-Dist: ruff==0.1.9; extra == "dev"
+Provides-Extra: tests
+Requires-Dist: pytest==7.4.3; extra == "tests"
+Requires-Dist: pytest-cov==4.1.0; extra == "tests"
+Requires-Dist: pytest-xdist==3.5.0; extra == "tests"
+Requires-Dist: pytest-sugar==0.9.7; extra == "tests"
+Requires-Dist: diff-cover==8.0.2; extra == "tests"
 
 # Memium
 
 [![Open in Dev Container](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)][dev container]
 [![PyPI](https://img.shields.io/pypi/v/memium.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/memium)][pypi status]
-[![Roadmap](https://img.shields.io/badge/Board-Roadmap-green)][roadmap]
 
 [dev container]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/MartinBernstorff/memium/
 [pypi status]: https://pypi.org/project/memium/
 [documentation]: https://MartinBernstorff.github.io/memium/
-[roadmap]: https://github.com/users/MartinBernstorff/projects/2
+
 
 <!-- start short-description -->
 
 When you have to stop and look things up, it breaks up your flow. Adding this knowledge to long-term memory builds fluency, and being fluent at something makes it much more fun! The faster you can get from crawling to running, the more enjoyable it is.
 
 Unfortunately, we forget most of what we read, [even stuff we care about](https://andymatuschak.org/books/).
 
@@ -89,55 +82,49 @@
 ### In Docker container
 2. Install [Orbstack](https://orbstack.dev/) or Docker Desktop. 
 3. Setup a container
 ```bash
 $INPUT_DIR="PATH_TO_YOUR_INPUT_DIR"
 
 docker run -i \
-  --name=memium \
   -e HOST_INPUT_DIR=$INPUT_DIR \
   -v $INPUT_DIR:/input \
   --restart unless-stopped \
   ghcr.io/martinbernstorff/memium:latest \
   memium \
   --input-dir /input/
 ```
 
-This will start a docker container which updates your deck from `$INPUT_DIR`. In case of updated files, it will sync the difference (create new prompts and delete deleted prompts) to Anki. 
-
-If you want to continuously sync the directory, set the `--watch-seconds [UPDATE_SECONDS]` argument as well.
-
-Keeping the package update can be a bit of a chore, which can be automated with [WatchTower](https://github.com/containrrr/watchtower).
+This will start a docker container which updates your deck from `$INPUT_DIR`. In case of updated files, it will sync the difference (create new prompts and delete deleted prompts) to Anki. If you want to continuously sync the directory, check out the documentation for the `cli`.
 
 ## Use as library
 If you would like to build build your own Python application on top of the abstractions added here, you can install the library from pypi:
 
 ```bash
 pip install memium
 ```
 
 ### Pipeline abstractions
-The library is built as a pipeline illustrated below. Left describes the abstract pipeline, defined by interfaces. The right path describes an implementation of those interfaces from markdown to Anki, which is available in the CLI. 
+The library is built as a pipeline illustrated below. The left path describes the abstract pipeline, defined by abstract interfaces. The right path describes implementation I use, and which is part of this repo. 
 
 ```mermaid
 
 graph TD 
 	FD["File on disk"]
-        DP["Prompts at Destination"]
-	FD -- DocumentSource --> Document
-	Document -- PromptExtractor --> Prompt
-	Prompt -- Destination --> DP
+	FD -- Document ingester --> Document
+	Document -- Prompt extractor --> Prompt
+	Prompt -- Destination --> Card 
  
 	MD["Markdown file"]
-	Prompts["[QAPrompt | ClozePrompt]"]
-        Anki["Cards in the Anki app"]
+	 Prompts["[QAPrompt | ClozePrompt]"]
+  Cards["[AnkiQA | AnkiCloze]"]
  
-	MD -- MarkdownDocumentSource --> Document
+	MD -- MarkdownDocumentIngester --> Document
 	Document -- "[QAPromptExtractor, \nClozePromptExtractor]" --> Prompts
-        Prompts -- AnkiConnectDestination --> Anki
+	Prompts -- AnkiConnectDestination --> Cards
  ```
 
 ## Contributing
 ### Setting up a dev environment
 1. Install [Orbstack](https://orbstack.dev/) or Docker Desktop. Make sure to complete the full install process before continuing.
 2. If not installed, install VSCode
 3. Press this [link](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/MartinBernstorff/memium/)
```

### Comparing `memium-0.19.0/memium.egg-info/SOURCES.txt` & `memium-0.7.0/memium.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,67 +19,61 @@
 .github/workflows/stalebot.yml
 .github/workflows/tests.yml
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 memium/__init__.py
 memium/__main__.py
+memium/cli.py
 memium/diff_determiner.py
-memium/environment.py
+memium/main.py
 memium/py.typed
 memium/test_diff_determiner.py
 memium/test_main.py
 memium.egg-info/PKG-INFO
 memium.egg-info/SOURCES.txt
 memium.egg-info/dependency_links.txt
 memium.egg-info/entry_points.txt
 memium.egg-info/requires.txt
 memium.egg-info/top_level.txt
+memium/data_access/__init__.py
+memium/data_access/ankiconnect_gateway.py
+memium/data_access/environment.py
+memium/data_access/test_ankiconnect_gateway.py
 memium/destination/__init__.py
 memium/destination/destination.py
 memium/destination/destination_ankiconnect.py
+memium/destination/destination_commands.py
 memium/destination/destination_dryrun.py
 memium/destination/test_destination_ankiconnect.py
 memium/destination/ankiconnect/__init__.py
+memium/destination/ankiconnect/anki_card.py
 memium/destination/ankiconnect/anki_converter.py
-memium/destination/ankiconnect/anki_prompt.py
 memium/destination/ankiconnect/anki_prompt_cloze.py
 memium/destination/ankiconnect/anki_prompt_qa.py
-memium/destination/ankiconnect/ankiconnect_gateway.py
-memium/destination/ankiconnect/default_styling.css
+memium/destination/ankiconnect/ankiconnect_css.py
 memium/destination/ankiconnect/test_anki_converter.py
 memium/destination/ankiconnect/test_anki_prompt_qa.py
-memium/destination/ankiconnect/test_ankiconnect_gateway.py
 memium/source/__init__.py
 memium/source/document.py
-memium/source/document_source.py
-memium/source/prompt_source.py
-memium/source/test_document_source.py
+memium/source/document_ingester.py
+memium/source/facade.py
+memium/source/test_document_ingester.py
 memium/source/test_facade.py
-memium/source/test_prompt_source.py
 memium/source/extractors/__init__.py
 memium/source/extractors/extractor.py
 memium/source/extractors/extractor_cloze.py
 memium/source/extractors/extractor_qa.py
-memium/source/extractors/extractor_table.py
-memium/source/extractors/test_extractor_table.py
-memium/source/extractors/test_prompt.py
 memium/source/extractors/test_prompt_extractor_cloze.py
 memium/source/extractors/test_prompt_extractor_qa.py
-memium/source/extractors/to_line_blocks.py
 memium/source/prompts/__init__.py
 memium/source/prompts/prompt.py
 memium/source/prompts/prompt_cloze.py
-memium/source/prompts/prompt_from_doc.py
-memium/source/prompts/prompt_from_doc_test.py
 memium/source/prompts/prompt_qa.py
-memium/source/prompts/__snapshots__/prompt_from_doc_test.ambr
-memium/tasks/__init__.py
-memium/tasks/github.py
-memium/tasks/graphite.py
-memium/tasks/smoketest.py
-memium/tasks/str_parsing.py
+memium/subtasks/__init__.py
+memium/subtasks/github.py
+memium/subtasks/graphite.py
+memium/subtasks/smoketest.py
+memium/subtasks/str_parsing.py
 memium/utils/__init__.py
-memium/utils/extract_terms.py
 memium/utils/hash_cleaned_str.py
-memium/utils/test_extract_terms.py
 memium/utils/test_hash_cleaned_str.py
```

### Comparing `memium-0.19.0/pyproject.toml` & `memium-0.7.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,56 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "memium"
-version = "0.19.0"
+version = "0.7.0"
 authors = [{ name = "Martin Bernstorff", email = "martinbernstorff@gmail.com" }]
 description = "Memium"
 classifiers = ["Programming Language :: Python :: 3.11"]
 requires-python = ">=3.11"
 
 # TODO: https://github.com/MartinBernstorff/memium/issues/260 Setup dependabot automerge
 dependencies = [
   "cffi==1.16.0",
-  "iterpy==1.9.0",
+  "functionalpy==0.14.0",
   "genanki==0.13.1",
-  "markdown==3.6",
-  "pydantic==2.7.0",
-  "sentry-sdk==1.45.0",
-  "typer==0.12.3",
-  "tqdm==4.66.2",
-  "unidecode==1.3.8",
+  "misaka==2.1.1",
+  "pydantic==2.5.3",
+  "sentry-sdk==1.39.1",
+  "typer==0.9.0",
+  "tqdm==4.66.1",
   "wasabi==1.1.2",
-  "bs4==0.0.1",
 ]
 
 [project.license]
 file = "LICENSE"
 
 [project.readme]
 file = "readme.md"
 content-type = "text/markdown"
 
 [project.scripts]
-memium = "memium.__main__:app"
+memium = "memium.cli:app"
 
 [project.optional-dependencies]
-tests = [
-  "pytest==7.4.4",
-  "pytest-cov==5.0.0",
-  "pytest-xdist==3.6.0",
-  "pytest-sugar==1.0.0",
-  "pytest-testmon==2.1.1",
-  "diff-cover==9.0.0",
-  "syrupy==4.6.1",
-]
 dev = [
   "cruft==2.15.0",
-  "herbarium",
   "invoke==2.2.0",
-  "pyright==1.1.359",
-  "pre-commit==3.7.0",
-  "ruff==0.4.1",
-  "lumberman",
+  "pyright==1.1.343",
+  "pre-commit==3.6.0",
+  "ruff==0.1.9",
+]
+tests = [
+  "pytest==7.4.3",
+  "pytest-cov==4.1.0",
+  "pytest-xdist==3.5.0",
+  "pytest-sugar==0.9.7",
+  "diff-cover==8.0.2",
 ]
 
 [project.urls]
 homepage = "https://github.com/MartinBernstorff/memium"
 repository = "https://github.com/MartinBernstorff/memium"
 documentation = "https://MartinBernstorff.github.io/memium/"
 
@@ -65,18 +59,15 @@
 pythonPlatform = "Darwin"
 reportMissingTypeStubs = false
 reportPrivateImportUsage = false
 typeCheckingMode = "strict"
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
-line-length = 100
-target-version = "py311"
-
-[tool.ruff.lint]
+line-length = 80
 select = [
   "A",
   "ANN",
   "ARG",
   "B",
   "C4",
   "C90",
@@ -137,39 +128,41 @@
   "node_modules",
   "venv",
   "__init__.py",
   "docs/conf.py",
 ]
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+target-version = "py311"
 
-[tool.ruff.lint.flake8-annotations]
+[tool.ruff.format]
+skip-magic-trailing-comma = true
+
+[tool.ruff.flake8-annotations]
 mypy-init-return = true
 suppress-none-returning = true
 
-[tool.ruff.lint.isort]
+[tool.ruff.isort]
 known-third-party = ["wandb"]
 split-on-trailing-comma = false
 
-[tool.ruff.lint.mccabe]
+[tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
-
-[tool.ruff.format]
-skip-magic-trailing-comma = true
-
 [tool.semantic_release]
 branch = "main"
 version_toml = ["pyproject.toml:project.version"]
 build_command = "python -m pip install build; python -m build"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.coverage.report]
 exclude_lines = [
-  "pragma: no cover",
-  # Ignore lines containing '...'
-  ".*[.]{3}.*",
-]
-omit = ["test_*.py"]
+    "pragma: no cover",
+    # Ignore lines containing '...'
+    ".*[.]{3}.*",
+]
+omit = [
+  "test_*.py",
+]
```

### Comparing `memium-0.19.0/readme.md` & `memium-0.7.0/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Memium
 
 [![Open in Dev Container](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)][dev container]
 [![PyPI](https://img.shields.io/pypi/v/memium.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/memium)][pypi status]
-[![Roadmap](https://img.shields.io/badge/Board-Roadmap-green)][roadmap]
 
 [dev container]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/MartinBernstorff/memium/
 [pypi status]: https://pypi.org/project/memium/
 [documentation]: https://MartinBernstorff.github.io/memium/
-[roadmap]: https://github.com/users/MartinBernstorff/projects/2
+
 
 <!-- start short-description -->
 
 When you have to stop and look things up, it breaks up your flow. Adding this knowledge to long-term memory builds fluency, and being fluent at something makes it much more fun! The faster you can get from crawling to running, the more enjoyable it is.
 
 Unfortunately, we forget most of what we read, [even stuff we care about](https://andymatuschak.org/books/).
 
@@ -50,55 +49,49 @@
 ### In Docker container
 2. Install [Orbstack](https://orbstack.dev/) or Docker Desktop. 
 3. Setup a container
 ```bash
 $INPUT_DIR="PATH_TO_YOUR_INPUT_DIR"
 
 docker run -i \
-  --name=memium \
   -e HOST_INPUT_DIR=$INPUT_DIR \
   -v $INPUT_DIR:/input \
   --restart unless-stopped \
   ghcr.io/martinbernstorff/memium:latest \
   memium \
   --input-dir /input/
 ```
 
-This will start a docker container which updates your deck from `$INPUT_DIR`. In case of updated files, it will sync the difference (create new prompts and delete deleted prompts) to Anki. 
-
-If you want to continuously sync the directory, set the `--watch-seconds [UPDATE_SECONDS]` argument as well.
-
-Keeping the package update can be a bit of a chore, which can be automated with [WatchTower](https://github.com/containrrr/watchtower).
+This will start a docker container which updates your deck from `$INPUT_DIR`. In case of updated files, it will sync the difference (create new prompts and delete deleted prompts) to Anki. If you want to continuously sync the directory, check out the documentation for the `cli`.
 
 ## Use as library
 If you would like to build build your own Python application on top of the abstractions added here, you can install the library from pypi:
 
 ```bash
 pip install memium
 ```
 
 ### Pipeline abstractions
-The library is built as a pipeline illustrated below. Left describes the abstract pipeline, defined by interfaces. The right path describes an implementation of those interfaces from markdown to Anki, which is available in the CLI. 
+The library is built as a pipeline illustrated below. The left path describes the abstract pipeline, defined by abstract interfaces. The right path describes implementation I use, and which is part of this repo. 
 
 ```mermaid
 
 graph TD 
 	FD["File on disk"]
-        DP["Prompts at Destination"]
-	FD -- DocumentSource --> Document
-	Document -- PromptExtractor --> Prompt
-	Prompt -- Destination --> DP
+	FD -- Document ingester --> Document
+	Document -- Prompt extractor --> Prompt
+	Prompt -- Destination --> Card 
  
 	MD["Markdown file"]
-	Prompts["[QAPrompt | ClozePrompt]"]
-        Anki["Cards in the Anki app"]
+	 Prompts["[QAPrompt | ClozePrompt]"]
+  Cards["[AnkiQA | AnkiCloze]"]
  
-	MD -- MarkdownDocumentSource --> Document
+	MD -- MarkdownDocumentIngester --> Document
 	Document -- "[QAPromptExtractor, \nClozePromptExtractor]" --> Prompts
-        Prompts -- AnkiConnectDestination --> Anki
+	Prompts -- AnkiConnectDestination --> Cards
  ```
 
 ## Contributing
 ### Setting up a dev environment
 1. Install [Orbstack](https://orbstack.dev/) or Docker Desktop. Make sure to complete the full install process before continuing.
 2. If not installed, install VSCode
 3. Press this [link](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/MartinBernstorff/memium/)
```

### Comparing `memium-0.19.0/tasks.py` & `memium-0.7.0/tasks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import invoke as inv
 
-from memium.tasks.github import get_issues_assigned_to_me, issue_dialog
-from memium.tasks.graphite import (
+from memium.subtasks.github import get_issues_assigned_to_me, issue_dialog
+from memium.subtasks.graphite import (
     create_branch_from_issue,
     submit_pr,  # noqa: F401 # type: ignore
 )
-from memium.tasks.smoketest import (
+from memium.subtasks.smoketest import (
     smoketest_cli,  # noqa: F401 # type: ignore
     smoketest_docker,  # noqa: F401 # type: ignore
 )
 
-PYTEST_CMD = "pytest --testmon --durations=5 --cov=memium memium --cov-report xml:.coverage.xml --cov-report lcov:.coverage.lcov"
+PYTEST_CMD = "pytest --durations=5 --cov=memium memium --cov-report xml:.coverage.xml --cov-report lcov:.coverage.lcov"
 
 
 @inv.task  # type: ignore
 def install_dev(c: inv.Context):
     print("--- Installing development dependencies ---")
     c.run("pip install --upgrade .[dev]")
     print("✅✅✅ Development dependencies installed ✅✅✅")
@@ -59,14 +59,20 @@
     missing_lines = [line for line in lines if "Missing lines" in line]
     coverage_percent = int(coverage_line.split(" ")[1][:-1])
 
     if coverage_percent < 80:
         print("\n=== Lines with missing coverage ===")
         for line in missing_lines:
             print(line)
+        proceed = input(
+            f"🚧🚧🚧 Coverage is {coverage_percent}%. Proceed? [y/N] "
+        )
+        if proceed.lower() != "y":
+            print("Aborting")
+            return
 
     print("✅✅✅ Tests passed ✅✅✅")
 
 
 @inv.task  # type: ignore
 def lint(c: inv.Context):
     print("--- Linting ---")
@@ -87,15 +93,17 @@
     my_issues = get_issues_assigned_to_me(c)
 
     if not my_issues:
         print("No issues found")
         return
 
     selected_issue_index = issue_dialog(my_issues)
-    create_branch_from_issue(c=c, selected_issue=my_issues[selected_issue_index])
+    create_branch_from_issue(
+        c=c, selected_issue=my_issues[selected_issue_index]
+    )
 
 
 @inv.task  # type: ignore
 def validate_ci(c: inv.Context):
     print("--- Validating CI ---")
     lint(c)
     types(c)
@@ -110,8 +118,10 @@
     if not my_issues:
         print("No issues assigned to you found")
         return
 
     selected_issue_index = issue_dialog(my_issues)
     c.run("git checkout main")
     c.run("git pull")
-    create_branch_from_issue(c=c, selected_issue=my_issues[selected_issue_index])
+    create_branch_from_issue(
+        c=c, selected_issue=my_issues[selected_issue_index]
+    )
```

