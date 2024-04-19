# Comparing `tmp/code_size_analyzer_client-python-0.6.2.tar.gz` & `tmp/code_size_analyzer_client_python-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_size_analyzer_client-python-0.6.2.tar", last modified: Thu Jan 25 21:58:32 2024, max compression
+gzip compressed data, was "code_size_analyzer_client_python-0.7.0.tar", last modified: Fri Apr 19 17:29:31 2024, max compression
```

## Comparing `code_size_analyzer_client-python-0.6.2.tar` & `code_size_analyzer_client_python-0.7.0.tar`

### file list

```diff
@@ -1,72 +1,81 @@
-drwxr-xr-x   0 jasavage   (503) staff       (20)        0 2024-01-25 21:58:32.287040 code_size_analyzer_client-python-0.6.2/
--rw-r--r--   0 jasavage   (503) staff       (20)      418 2024-01-25 21:58:32.287128 code_size_analyzer_client-python-0.6.2/PKG-INFO
--rw-r--r--   0 jasavage   (503) staff       (20)     6374 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/README.md
--rw-r--r--   0 jasavage   (503) staff       (20)     3116 2024-01-25 21:56:39.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_cli.py
-drwxr-xr-x   0 jasavage   (503) staff       (20)        0 2024-01-25 21:58:32.248083 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/
--rw-r--r--   0 jasavage   (503) staff       (20)      854 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/__init__.py
-drwxr-xr-x   0 jasavage   (503) staff       (20)        0 2024-01-25 21:58:32.249124 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/api/
--rw-r--r--   0 jasavage   (503) staff       (20)      230 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/api/__init__.py
--rw-r--r--   0 jasavage   (503) staff       (20)     6156 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/api/analyzer_api.py
--rw-r--r--   0 jasavage   (503) staff       (20)     5499 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/api/default_api.py
--rw-r--r--   0 jasavage   (503) staff       (20)     6236 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/api/parser_api.py
--rw-r--r--   0 jasavage   (503) staff       (20)    32225 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/api/results_api.py
--rw-r--r--   0 jasavage   (503) staff       (20)    39150 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/api_client.py
-drwxr-xr-x   0 jasavage   (503) staff       (20)        0 2024-01-25 21:58:32.249894 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/apis/
--rw-r--r--   0 jasavage   (503) staff       (20)      700 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/apis/__init__.py
--rw-r--r--   0 jasavage   (503) staff       (20)     3274 2024-01-23 15:02:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/client_wrapper.py
--rw-r--r--   0 jasavage   (503) staff       (20)    16440 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/configuration.py
--rw-r--r--   0 jasavage   (503) staff       (20)     5098 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/exceptions.py
-drwxr-xr-x   0 jasavage   (503) staff       (20)        0 2024-01-25 21:58:32.266247 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/
--rw-r--r--   0 jasavage   (503) staff       (20)      359 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/__init__.py
--rw-r--r--   0 jasavage   (503) staff       (20)    12498 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/application_combination.py
--rw-r--r--   0 jasavage   (503) staff       (20)    12998 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/classification_rule.py
--rw-r--r--   0 jasavage   (503) staff       (20)    14641 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/data_record.py
--rw-r--r--   0 jasavage   (503) staff       (20)    11715 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/http_validation_error.py
--rw-r--r--   0 jasavage   (503) staff       (20)    14068 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_memory_config.py
--rw-r--r--   0 jasavage   (503) staff       (20)    11669 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_parse_request.py
--rw-r--r--   0 jasavage   (503) staff       (20)    12686 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_parse_response.py
--rw-r--r--   0 jasavage   (503) staff       (20)    17114 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_request.py
--rw-r--r--   0 jasavage   (503) staff       (20)    12420 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_response.py
--rw-r--r--   0 jasavage   (503) staff       (20)    11973 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_section.py
--rw-r--r--   0 jasavage   (503) staff       (20)    12293 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_summary.py
--rw-r--r--   0 jasavage   (503) staff       (20)    12357 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/module.py
--rw-r--r--   0 jasavage   (503) staff       (20)    12372 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/module_group.py
--rw-r--r--   0 jasavage   (503) staff       (20)    11888 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/summary_record.py
--rw-r--r--   0 jasavage   (503) staff       (20)    12183 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/symbol.py
--rw-r--r--   0 jasavage   (503) staff       (20)    12312 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/target_info.py
--rw-r--r--   0 jasavage   (503) staff       (20)    11861 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/validation_error.py
--rw-r--r--   0 jasavage   (503) staff       (20)    82527 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model_utils.py
-drwxr-xr-x   0 jasavage   (503) staff       (20)        0 2024-01-25 21:58:32.266548 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/models/
--rw-r--r--   0 jasavage   (503) staff       (20)     1685 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/models/__init__.py
--rw-r--r--   0 jasavage   (503) staff       (20)    14313 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/rest.py
-drwxr-xr-x   0 jasavage   (503) staff       (20)        0 2024-01-25 21:58:32.267929 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client_python.egg-info/
--rw-r--r--   0 jasavage   (503) staff       (20)      418 2024-01-25 21:58:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client_python.egg-info/PKG-INFO
--rw-r--r--   0 jasavage   (503) staff       (20)     2518 2024-01-25 21:58:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 jasavage   (503) staff       (20)        1 2024-01-25 21:58:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 jasavage   (503) staff       (20)       72 2024-01-25 21:58:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client_python.egg-info/entry_points.txt
--rw-r--r--   0 jasavage   (503) staff       (20)      167 2024-01-25 21:58:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client_python.egg-info/requires.txt
--rw-r--r--   0 jasavage   (503) staff       (20)       49 2024-01-25 21:58:32.000000 code_size_analyzer_client-python-0.6.2/code_size_analyzer_client_python.egg-info/top_level.txt
--rw-r--r--   0 jasavage   (503) staff       (20)       69 2024-01-25 21:58:32.287402 code_size_analyzer_client-python-0.6.2/setup.cfg
--rw-r--r--   0 jasavage   (503) staff       (20)     1475 2024-01-25 21:55:47.000000 code_size_analyzer_client-python-0.6.2/setup.py
-drwxr-xr-x   0 jasavage   (503) staff       (20)        0 2024-01-25 21:58:32.286776 code_size_analyzer_client-python-0.6.2/test/
--rw-r--r--   0 jasavage   (503) staff       (20)      764 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_analyzer_api.py
--rw-r--r--   0 jasavage   (503) staff       (20)      858 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_application_combination.py
--rw-r--r--   0 jasavage   (503) staff       (20)      830 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_classification_rule.py
--rw-r--r--   0 jasavage   (503) staff       (20)      774 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_data_record.py
--rw-r--r--   0 jasavage   (503) staff       (20)      751 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_default_api.py
--rw-r--r--   0 jasavage   (503) staff       (20)      962 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_http_validation_error.py
--rw-r--r--   0 jasavage   (503) staff       (20)      960 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_map_file_memory_config.py
--rw-r--r--   0 jasavage   (503) staff       (20)      839 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_map_file_parse_request.py
--rw-r--r--   0 jasavage   (503) staff       (20)     1109 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_map_file_parse_response.py
--rw-r--r--   0 jasavage   (503) staff       (20)      939 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_map_file_request.py
--rw-r--r--   0 jasavage   (503) staff       (20)     1030 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_map_file_response.py
--rw-r--r--   0 jasavage   (503) staff       (20)      803 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_map_file_section.py
--rw-r--r--   0 jasavage   (503) staff       (20)      911 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_map_file_summary.py
--rw-r--r--   0 jasavage   (503) staff       (20)      832 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_module.py
--rw-r--r--   0 jasavage   (503) staff       (20)      868 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_module_group.py
--rw-r--r--   0 jasavage   (503) staff       (20)      750 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_parser_api.py
--rw-r--r--   0 jasavage   (503) staff       (20)     1545 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_results_api.py
--rw-r--r--   0 jasavage   (503) staff       (20)      795 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_summary_record.py
--rw-r--r--   0 jasavage   (503) staff       (20)      745 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_symbol.py
--rw-r--r--   0 jasavage   (503) staff       (20)      774 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_target_info.py
--rw-r--r--   0 jasavage   (503) staff       (20)      809 2023-12-07 17:43:32.000000 code_size_analyzer_client-python-0.6.2/test/test_validation_error.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:29:31.295833 code_size_analyzer_client_python-0.7.0/
+-rw-rw-rw-   0        0        0      666 2024-04-19 17:29:31.294716 code_size_analyzer_client_python-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6840 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/README.md
+-rw-rw-rw-   0        0        0     3215 2024-01-23 19:57:43.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_cli.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:29:31.088945 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/
+-rw-rw-rw-   0        0        0      881 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:29:31.105306 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/api/
+-rw-rw-rw-   0        0        0      233 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/api/__init__.py
+-rw-rw-rw-   0        0        0     6329 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/api/analyzer_api.py
+-rw-rw-rw-   0        0        0     5649 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/api/default_api.py
+-rw-rw-rw-   0        0        0     6409 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/api/parser_api.py
+-rw-rw-rw-   0        0        0    34368 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/api/results_api.py
+-rw-rw-rw-   0        0        0    40046 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/api_client.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:29:31.109772 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/apis/
+-rw-rw-rw-   0        0        0      720 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/apis/__init__.py
+-rw-rw-rw-   0        0        0     5757 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/client_wrapper.py
+-rw-rw-rw-   0        0        0    16890 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/configuration.py
+-rw-rw-rw-   0        0        0     5256 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:29:31.192277 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/
+-rw-rw-rw-   0        0        0      364 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/__init__.py
+-rw-rw-rw-   0        0        0    15752 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/application_analysis_result_with_detail.py
+-rw-rw-rw-   0        0        0    12791 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/application_combination.py
+-rw-rw-rw-   0        0        0    13285 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/classification_rule.py
+-rw-rw-rw-   0        0        0    14964 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/data_record.py
+-rw-rw-rw-   0        0        0    14028 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/file_data.py
+-rw-rw-rw-   0        0        0    11984 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/http_validation_error.py
+-rw-rw-rw-   0        0        0    14397 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/map_file_memory_config.py
+-rw-rw-rw-   0        0        0    11938 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/map_file_parse_request.py
+-rw-rw-rw-   0        0        0    12981 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/map_file_parse_response.py
+-rw-rw-rw-   0        0        0    17455 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/map_file_request.py
+-rw-rw-rw-   0        0        0    13042 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/map_file_response.py
+-rw-rw-rw-   0        0        0    12254 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/map_file_section.py
+-rw-rw-rw-   0        0        0    12580 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/map_file_summary.py
+-rw-rw-rw-   0        0        0    12650 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/module.py
+-rw-rw-rw-   0        0        0    12665 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/module_group.py
+-rw-rw-rw-   0        0        0    11956 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/response_get_app_analysis_details_results_get_app_analysis_details_get.py
+-rw-rw-rw-   0        0        0    12056 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/section_summary.py
+-rw-rw-rw-   0        0        0    12155 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/summary_record.py
+-rw-rw-rw-   0        0        0    12470 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/symbol.py
+-rw-rw-rw-   0        0        0    12817 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/target_info.py
+-rw-rw-rw-   0        0        0    12142 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/validation_error.py
+-rw-rw-rw-   0        0        0    84583 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:29:31.196182 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/models/
+-rw-rw-rw-   0        0        0     2151 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/models/__init__.py
+-rw-rw-rw-   0        0        0    14665 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/rest.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:29:31.292394 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client_python.egg-info/
+-rw-rw-rw-   0        0        0      666 2024-04-19 17:29:31.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3009 2024-04-19 17:29:31.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 17:29:31.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2024-04-19 17:29:31.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      151 2024-04-19 17:29:31.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       71 2024-04-19 17:29:31.000000 code_size_analyzer_client_python-0.7.0/code_size_analyzer_client_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2951 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/code_size_results_cli.py
+-rw-rw-rw-   0        0        0       76 2024-04-19 17:29:31.297000 code_size_analyzer_client_python-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1600 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:29:31.289164 code_size_analyzer_client_python-0.7.0/test/
+-rw-rw-rw-   0        0        0      799 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_analyzer_api.py
+-rw-rw-rw-   0        0        0     1207 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/test/test_application_analysis_result_with_detail.py
+-rw-rw-rw-   0        0        0      893 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_application_combination.py
+-rw-rw-rw-   0        0        0      865 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_classification_rule.py
+-rw-rw-rw-   0        0        0      809 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_data_record.py
+-rw-rw-rw-   0        0        0      784 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/test/test_default_api.py
+-rw-rw-rw-   0        0        0      795 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/test/test_file_data.py
+-rw-rw-rw-   0        0        0      999 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_http_validation_error.py
+-rw-rw-rw-   0        0        0      997 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_map_file_memory_config.py
+-rw-rw-rw-   0        0        0      874 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_map_file_parse_request.py
+-rw-rw-rw-   0        0        0     1148 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_map_file_parse_response.py
+-rw-rw-rw-   0        0        0      976 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_map_file_request.py
+-rw-rw-rw-   0        0        0     1069 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_map_file_response.py
+-rw-rw-rw-   0        0        0      838 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_map_file_section.py
+-rw-rw-rw-   0        0        0      948 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_map_file_summary.py
+-rw-rw-rw-   0        0        0      869 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_module.py
+-rw-rw-rw-   0        0        0      905 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_module_group.py
+-rw-rw-rw-   0        0        0      785 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_parser_api.py
+-rw-rw-rw-   0        0        0     1377 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/test/test_response_get_app_analysis_details_results_get_app_analysis_details_get.py
+-rw-rw-rw-   0        0        0     1615 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_results_api.py
+-rw-rw-rw-   0        0        0      837 2024-04-19 17:28:57.000000 code_size_analyzer_client_python-0.7.0/test/test_section_summary.py
+-rw-rw-rw-   0        0        0      830 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_summary_record.py
+-rw-rw-rw-   0        0        0      780 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_symbol.py
+-rw-rw-rw-   0        0        0      809 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_target_info.py
+-rw-rw-rw-   0        0        0      844 2023-05-19 01:53:07.000000 code_size_analyzer_client_python-0.7.0/test/test_validation_error.py
```

### Comparing `code_size_analyzer_client-python-0.6.2/README.md` & `code_size_analyzer_client_python-0.7.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,167 +1,171 @@
-# code_size_analyzer_client-python
-No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
-
-This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
-
-- API version: 0.1.0
-- Package version: 0.5.0
-- Build package: org.openapitools.codegen.languages.PythonClientCodegen
-
-## Requirements.
-
-Python >=3.6
-
-## Installation & Usage
-### pip install
-
-If the python package is hosted on a repository, you can install directly using:
-
-```sh
-pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
-```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
-
-Then import the package:
-```python
-import code_size_analyzer_client
-```
-
-### Setuptools
-
-Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
-
-```sh
-python setup.py install --user
-```
-(or `sudo python setup.py install` to install the package for all users)
-
-Then import the package:
-```python
-import code_size_analyzer_client
-```
-
-## Getting Started
-
-Please follow the [installation procedure](#installation--usage) and then run the following:
-
-```python
-
-import time
-import code_size_analyzer_client
-from pprint import pprint
-from code_size_analyzer_client.api import analyzer_api
-from code_size_analyzer_client.model.http_validation_error import HTTPValidationError
-from code_size_analyzer_client.model.map_file_request import MapFileRequest
-from code_size_analyzer_client.model.map_file_response import MapFileResponse
-# Defining the host is optional and defaults to https://code-size-analyzer.silabs.net
-# See configuration.py for a list of all supported configuration parameters.
-configuration = code_size_analyzer_client.Configuration(
-    host = "https://code-size-analyzer.silabs.net"
-)
-
-
-
-# Enter a context with an instance of the API client
-with code_size_analyzer_client.ApiClient(configuration) as api_client:
-    # Create an instance of the API class
-    api_instance = analyzer_api.AnalyzerApi(api_client)
-    map_file_request = MapFileRequest(
-        map_file="map_file_example",
-        stack_name="stack_name_example",
-        target_part="target_part_example",
-        target_board="target_board_example",
-        app_name="app_name_example",
-        compiler="compiler_example",
-        project_file="project_file_example",
-        project_file_name="project_file_name_example",
-        branch_name="branch_name_example",
-        build_number="build_number_example",
-        commit="commit_example",
-        store_results=True,
-        build_url="build_url_example",
-        classification_rules=[
-            ClassificationRule(
-                matcher="matcher_example",
-                module="module_example",
-                component="component_example",
-                team_owner="team_owner_example",
-            ),
-        ],
-        ignore_default_rules=False,
-        uc_component_branch_name="uc_component_branch_name_example",
-    ) # MapFileRequest | 
-
-    try:
-        # Analyze Map File Post
-        api_response = api_instance.analyze_map_file(map_file_request)
-        pprint(api_response)
-    except code_size_analyzer_client.ApiException as e:
-        print("Exception when calling AnalyzerApi->analyze_map_file: %s\n" % e)
-```
-
-## Documentation for API Endpoints
-
-All URIs are relative to *https://code-size-analyzer.silabs.net*
-
-Class | Method | HTTP request | Description
------------- | ------------- | ------------- | -------------
-*AnalyzerApi* | [**analyze_map_file**](docs/AnalyzerApi.md#analyze_map_file) | **POST** /analyze_map_file | Analyze Map File Post
-*DefaultApi* | [**metrics_metrics_get**](docs/DefaultApi.md#metrics_metrics_get) | **GET** /metrics | Metrics
-*ParserApi* | [**parse_map_file**](docs/ParserApi.md#parse_map_file) | **POST** /parse_map_file | Analyze Map File Post
-*ResultsApi* | [**get_app_analysis_details**](docs/ResultsApi.md#get_app_analysis_details) | **GET** /results/get_app_analysis_details | Get App Analysis Details
-*ResultsApi* | [**get_app_combinations**](docs/ResultsApi.md#get_app_combinations) | **GET** /results/get_app_combinations | Get App Combinations
-*ResultsApi* | [**get_app_stack_names**](docs/ResultsApi.md#get_app_stack_names) | **GET** /results/get_app_stack_names | Get App Stack Names
-*ResultsApi* | [**get_app_summary_records**](docs/ResultsApi.md#get_app_summary_records) | **GET** /results/get_app_summary_records | Get App Summary Records
-*ResultsApi* | [**get_branch_builds**](docs/ResultsApi.md#get_branch_builds) | **GET** /results/get_branch_builds | Get Branch Builds
-*ResultsApi* | [**get_target_info**](docs/ResultsApi.md#get_target_info) | **GET** /results/get_target_info | Get Target Info
-
-
-## Documentation For Models
-
- - [ApplicationCombination](docs/ApplicationCombination.md)
- - [ClassificationRule](docs/ClassificationRule.md)
- - [DataRecord](docs/DataRecord.md)
- - [HTTPValidationError](docs/HTTPValidationError.md)
- - [MapFileMemoryConfig](docs/MapFileMemoryConfig.md)
- - [MapFileParseRequest](docs/MapFileParseRequest.md)
- - [MapFileParseResponse](docs/MapFileParseResponse.md)
- - [MapFileRequest](docs/MapFileRequest.md)
- - [MapFileResponse](docs/MapFileResponse.md)
- - [MapFileSection](docs/MapFileSection.md)
- - [MapFileSummary](docs/MapFileSummary.md)
- - [Module](docs/Module.md)
- - [ModuleGroup](docs/ModuleGroup.md)
- - [SummaryRecord](docs/SummaryRecord.md)
- - [Symbol](docs/Symbol.md)
- - [TargetInfo](docs/TargetInfo.md)
- - [ValidationError](docs/ValidationError.md)
-
-
-## Documentation For Authorization
-
- All endpoints do not require authorization.
-
-## Author
-
-
-
-
-## Notes for Large OpenAPI documents
-If the OpenAPI document is large, imports in code_size_analyzer_client.apis and code_size_analyzer_client.models may fail with a
-RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
-
-Solution 1:
-Use specific imports for apis and models like:
-- `from code_size_analyzer_client.api.default_api import DefaultApi`
-- `from code_size_analyzer_client.model.pet import Pet`
-
-Solution 2:
-Before importing the package, adjust the maximum recursion limit as shown below:
-```
-import sys
-sys.setrecursionlimit(1500)
-import code_size_analyzer_client
-from code_size_analyzer_client.apis import *
-from code_size_analyzer_client.models import *
-```
-
+# code_size_analyzer_client-python
+No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
+
+- API version: 0.1.0
+- Package version: 0.7.0
+- Build package: org.openapitools.codegen.languages.PythonClientCodegen
+
+## Requirements.
+
+Python >=3.6
+
+## Installation & Usage
+### pip install
+
+If the python package is hosted on a repository, you can install directly using:
+
+```sh
+pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+```
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
+
+Then import the package:
+```python
+import code_size_analyzer_client
+```
+
+### Setuptools
+
+Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
+
+```sh
+python setup.py install --user
+```
+(or `sudo python setup.py install` to install the package for all users)
+
+Then import the package:
+```python
+import code_size_analyzer_client
+```
+
+## Getting Started
+
+Please follow the [installation procedure](#installation--usage) and then run the following:
+
+```python
+
+import time
+import code_size_analyzer_client
+from pprint import pprint
+from code_size_analyzer_client.api import analyzer_api
+from code_size_analyzer_client.model.http_validation_error import HTTPValidationError
+from code_size_analyzer_client.model.map_file_request import MapFileRequest
+from code_size_analyzer_client.model.map_file_response import MapFileResponse
+# Defining the host is optional and defaults to https://code-size-analyzer.silabs.net
+# See configuration.py for a list of all supported configuration parameters.
+configuration = code_size_analyzer_client.Configuration(
+    host = "https://code-size-analyzer.silabs.net"
+)
+
+
+
+# Enter a context with an instance of the API client
+with code_size_analyzer_client.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
+    api_instance = analyzer_api.AnalyzerApi(api_client)
+    map_file_request = MapFileRequest(
+        map_file="map_file_example",
+        stack_name="stack_name_example",
+        target_part="target_part_example",
+        target_board="target_board_example",
+        app_name="app_name_example",
+        compiler="compiler_example",
+        project_file="project_file_example",
+        project_file_name="project_file_name_example",
+        branch_name="branch_name_example",
+        build_number="build_number_example",
+        commit="commit_example",
+        store_results=True,
+        build_url="build_url_example",
+        classification_rules=[
+            ClassificationRule(
+                matcher="matcher_example",
+                module="module_example",
+                component="component_example",
+                team_owner="team_owner_example",
+            ),
+        ],
+        ignore_default_rules=False,
+        uc_component_branch_name="uc_component_branch_name_example",
+    ) # MapFileRequest | 
+
+    try:
+        # Analyze Map File Post
+        api_response = api_instance.analyze_map_file(map_file_request)
+        pprint(api_response)
+    except code_size_analyzer_client.ApiException as e:
+        print("Exception when calling AnalyzerApi->analyze_map_file: %s\n" % e)
+```
+
+## Documentation for API Endpoints
+
+All URIs are relative to *https://code-size-analyzer.silabs.net*
+
+Class | Method | HTTP request | Description
+------------ | ------------- | ------------- | -------------
+*AnalyzerApi* | [**analyze_map_file**](docs/AnalyzerApi.md#analyze_map_file) | **POST** /analyze_map_file | Analyze Map File Post
+*DefaultApi* | [**metrics_health_get**](docs/DefaultApi.md#metrics_health_get) | **GET** /health | Metrics
+*ParserApi* | [**parse_map_file**](docs/ParserApi.md#parse_map_file) | **POST** /parse_map_file | Analyze Map File Post
+*ResultsApi* | [**get_app_analysis_details**](docs/ResultsApi.md#get_app_analysis_details) | **GET** /results/get_app_analysis_details | Get App Analysis Details
+*ResultsApi* | [**get_app_combinations**](docs/ResultsApi.md#get_app_combinations) | **GET** /results/get_app_combinations | Get App Combinations
+*ResultsApi* | [**get_app_stack_names**](docs/ResultsApi.md#get_app_stack_names) | **GET** /results/get_app_stack_names | Get App Stack Names
+*ResultsApi* | [**get_app_summary_records**](docs/ResultsApi.md#get_app_summary_records) | **GET** /results/get_app_summary_records | Get App Summary Records
+*ResultsApi* | [**get_branch_builds**](docs/ResultsApi.md#get_branch_builds) | **GET** /results/get_branch_builds | Get Branch Builds
+*ResultsApi* | [**get_target_info**](docs/ResultsApi.md#get_target_info) | **GET** /results/get_target_info | Get Target Info
+
+
+## Documentation For Models
+
+ - [ApplicationAnalysisResultWithDetail](docs/ApplicationAnalysisResultWithDetail.md)
+ - [ApplicationCombination](docs/ApplicationCombination.md)
+ - [ClassificationRule](docs/ClassificationRule.md)
+ - [DataRecord](docs/DataRecord.md)
+ - [FileData](docs/FileData.md)
+ - [HTTPValidationError](docs/HTTPValidationError.md)
+ - [MapFileMemoryConfig](docs/MapFileMemoryConfig.md)
+ - [MapFileParseRequest](docs/MapFileParseRequest.md)
+ - [MapFileParseResponse](docs/MapFileParseResponse.md)
+ - [MapFileRequest](docs/MapFileRequest.md)
+ - [MapFileResponse](docs/MapFileResponse.md)
+ - [MapFileSection](docs/MapFileSection.md)
+ - [MapFileSummary](docs/MapFileSummary.md)
+ - [Module](docs/Module.md)
+ - [ModuleGroup](docs/ModuleGroup.md)
+ - [ResponseGetAppAnalysisDetailsResultsGetAppAnalysisDetailsGet](docs/ResponseGetAppAnalysisDetailsResultsGetAppAnalysisDetailsGet.md)
+ - [SectionSummary](docs/SectionSummary.md)
+ - [SummaryRecord](docs/SummaryRecord.md)
+ - [Symbol](docs/Symbol.md)
+ - [TargetInfo](docs/TargetInfo.md)
+ - [ValidationError](docs/ValidationError.md)
+
+
+## Documentation For Authorization
+
+ All endpoints do not require authorization.
+
+## Author
+
+
+
+
+## Notes for Large OpenAPI documents
+If the OpenAPI document is large, imports in code_size_analyzer_client.apis and code_size_analyzer_client.models may fail with a
+RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
+
+Solution 1:
+Use specific imports for apis and models like:
+- `from code_size_analyzer_client.api.default_api import DefaultApi`
+- `from code_size_analyzer_client.model.pet import Pet`
+
+Solution 2:
+Before importing the package, adjust the maximum recursion limit as shown below:
+```
+import sys
+sys.setrecursionlimit(1500)
+import code_size_analyzer_client
+from code_size_analyzer_client.apis import *
+from code_size_analyzer_client.models import *
+```
+
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_cli.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_cli.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import click
-from code_size_analyzer_client.client_wrapper import ClientWrapper
-from code_size_analyzer_client.api_client import ApiClient
-import json
-from otel_extensions import (
-    init_telemetry_provider,
-    TelemetryOptions,
-    flush_telemetry_data,
-)
-from retry import retry
-import logging
-
-
-@click.command()
-@click.option("--map_file", required=True, help="path to map file")
-@click.option(
-    "--stack_name", required=True, help="stack owner name (i.e. zigbee, matter)"
-)
-@click.option(
-    "--target_part", required=True, help="target part (e.g. efr32mg22c224f512im40)"
-)
-@click.option("--compiler", required=True, help="compiler name (gcc or iar)")
-@click.option("--project_file", default=None, help="path to project file")
-@click.option(
-    "--service_url",
-    default="https://code-size-analyzer.silabs.net",
-    help="service endpoint",
-)
-@click.option(
-    "--output_file",
-    default=None,
-    help="path to output json file (default is to stdout)",
-)
-@click.option("--verify_ssl", default=False, help="verify ssl certificate on server")
-@click.option("--target_board", default=None, help="target board (e.g. brd4181a)")
-@click.option("--app_name", default=None, help="application name")
-@click.option("--branch_name", default=None, help="branch name")
-@click.option("--build_number", default=None, help="build number")
-@click.option("--sdk_commit_hash", default=None, help="SDK commit hash")
-@click.option("--store_results", default=False, help="store results to database")
-@click.option(
-    "--uc_component_branch_name",
-    default=None,
-    help="branch name for uc component-based categorization (e.g. use develop/22q4 for a feature branch branched off develop/22q4)",
-)
-def main(
-    map_file,
-    stack_name,
-    target_part,
-    compiler,
-    project_file,
-    service_url,
-    output_file,
-    verify_ssl,
-    target_board,
-    app_name,
-    branch_name,
-    build_number,
-    sdk_commit_hash,
-    store_results,
-    uc_component_branch_name,
-):
-    logging.getLogger("opentelemetry.util._time").setLevel(logging.ERROR)
-    init_telemetry_provider(
-        TelemetryOptions(
-            OTEL_SERVICE_NAME="Code Size Analyzer CLI",
-        )
-    )
-    client_wrapper = ClientWrapper(server_url=service_url, verify_ssl=verify_ssl)
-
-    @retry(tries=6, delay=1, max_delay=10, backoff=2)
-    def call_analyzer():
-        r = client_wrapper.analyze_map_file(
-            map_file,
-            stack_name,
-            target_part,
-            compiler,
-            project_file,
-            target_board=target_board,
-            app_name=app_name,
-            branch_name=branch_name,
-            build_number=build_number,
-            sdk_commit_hash=sdk_commit_hash,
-            store_results=store_results,
-            uc_component_branch_name=uc_component_branch_name,
-        )
-        j = json.dumps(ApiClient.sanitize_for_serialization(r), indent=2)
-        if output_file is not None:
-            with open(output_file, "w") as f:
-                f.write(j)
-        else:
-            print(j)
-
-    call_analyzer()
-    flush_telemetry_data()
-
-
-if __name__ == "__main__":
-    main()
+import click
+from code_size_analyzer_client.client_wrapper import ClientWrapper
+from code_size_analyzer_client.api_client import ApiClient
+import json
+from otel_extensions import (
+    init_telemetry_provider,
+    TelemetryOptions,
+    flush_telemetry_data,
+)
+from retry import retry
+import logging
+
+
+@click.command()
+@click.option("--map_file", required=True, help="path to map file")
+@click.option(
+    "--stack_name", required=True, help="stack owner name (i.e. zigbee, matter)"
+)
+@click.option(
+    "--target_part", required=True, help="target part (e.g. efr32mg22c224f512im40)"
+)
+@click.option("--compiler", required=True, help="compiler name (gcc or iar)")
+@click.option("--project_file", default=None, help="path to project file")
+@click.option(
+    "--service_url",
+    default="https://code-size-analyzer.silabs.net",
+    help="service endpoint",
+)
+@click.option(
+    "--output_file",
+    default=None,
+    help="path to output json file (default is to stdout)",
+)
+@click.option("--verify_ssl", default=False, help="verify ssl certificate on server")
+@click.option("--target_board", default=None, help="target board (e.g. brd4181a)")
+@click.option("--app_name", default=None, help="application name")
+@click.option("--branch_name", default=None, help="branch name")
+@click.option("--build_number", default=None, help="build number")
+@click.option("--sdk_commit_hash", default=None, help="SDK commit hash")
+@click.option("--store_results", default=False, help="store results to database")
+@click.option(
+    "--uc_component_branch_name",
+    default=None,
+    help="branch name for uc component-based categorization (e.g. use develop/22q4 for a feature branch branched off develop/22q4)",
+)
+def main(
+    map_file,
+    stack_name,
+    target_part,
+    compiler,
+    project_file,
+    service_url,
+    output_file,
+    verify_ssl,
+    target_board,
+    app_name,
+    branch_name,
+    build_number,
+    sdk_commit_hash,
+    store_results,
+    uc_component_branch_name,
+):
+    logging.getLogger("opentelemetry.util._time").setLevel(logging.ERROR)
+    init_telemetry_provider(
+        TelemetryOptions(
+            OTEL_SERVICE_NAME="Code Size Analyzer CLI",
+        )
+    )
+    client_wrapper = ClientWrapper(server_url=service_url, verify_ssl=verify_ssl)
+
+    @retry(tries=6, delay=1, max_delay=10, backoff=2)
+    def call_analyzer():
+        r = client_wrapper.analyze_map_file(
+            map_file,
+            stack_name,
+            target_part,
+            compiler,
+            project_file,
+            target_board=target_board,
+            app_name=app_name,
+            branch_name=branch_name,
+            build_number=build_number,
+            sdk_commit_hash=sdk_commit_hash,
+            store_results=store_results,
+            uc_component_branch_name=uc_component_branch_name,
+        )
+        j = json.dumps(ApiClient.sanitize_for_serialization(r), indent=2)
+        if output_file is not None:
+            with open(output_file, "w") as f:
+                f.write(j)
+        else:
+            print(j)
+
+    call_analyzer()
+    flush_telemetry_data()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/__init__.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# flake8: noqa
-
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-__version__ = "0.5.0"
-
-# import ApiClient
-from code_size_analyzer_client.api_client import ApiClient
-
-# import Configuration
-from code_size_analyzer_client.configuration import Configuration
-
-# import exceptions
-from code_size_analyzer_client.exceptions import OpenApiException
-from code_size_analyzer_client.exceptions import ApiAttributeError
-from code_size_analyzer_client.exceptions import ApiTypeError
-from code_size_analyzer_client.exceptions import ApiValueError
-from code_size_analyzer_client.exceptions import ApiKeyError
-from code_size_analyzer_client.exceptions import ApiException
+# flake8: noqa
+
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+__version__ = "0.7.0"
+
+# import ApiClient
+from code_size_analyzer_client.api_client import ApiClient
+
+# import Configuration
+from code_size_analyzer_client.configuration import Configuration
+
+# import exceptions
+from code_size_analyzer_client.exceptions import OpenApiException
+from code_size_analyzer_client.exceptions import ApiAttributeError
+from code_size_analyzer_client.exceptions import ApiTypeError
+from code_size_analyzer_client.exceptions import ApiValueError
+from code_size_analyzer_client.exceptions import ApiKeyError
+from code_size_analyzer_client.exceptions import ApiException
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/api/analyzer_api.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/api/parser_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.api_client import ApiClient, Endpoint as _Endpoint
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    check_allowed_values,
-    check_validations,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_and_convert_types
-)
-from code_size_analyzer_client.model.http_validation_error import HTTPValidationError
-from code_size_analyzer_client.model.map_file_request import MapFileRequest
-from code_size_analyzer_client.model.map_file_response import MapFileResponse
-
-
-class AnalyzerApi(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-
-    def __init__(self, api_client=None):
-        if api_client is None:
-            api_client = ApiClient()
-        self.api_client = api_client
-        self.analyze_map_file_endpoint = _Endpoint(
-            settings={
-                'response_type': (MapFileResponse,),
-                'auth': [],
-                'endpoint_path': '/analyze_map_file',
-                'operation_id': 'analyze_map_file',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'map_file_request',
-                ],
-                'required': [
-                    'map_file_request',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'map_file_request':
-                        (MapFileRequest,),
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                    'map_file_request': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
-
-    def analyze_map_file(
-        self,
-        map_file_request,
-        **kwargs
-    ):
-        """Analyze Map File Post  # noqa: E501
-
-        analyze a map file  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.analyze_map_file(map_file_request, async_req=True)
-        >>> result = thread.get()
-
-        Args:
-            map_file_request (MapFileRequest):
-
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            MapFileResponse
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['map_file_request'] = \
-            map_file_request
-        return self.analyze_map_file_endpoint.call_with_http_info(**kwargs)
-
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.api_client import ApiClient, Endpoint as _Endpoint
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    check_allowed_values,
+    check_validations,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_and_convert_types
+)
+from code_size_analyzer_client.model.http_validation_error import HTTPValidationError
+from code_size_analyzer_client.model.map_file_parse_request import MapFileParseRequest
+from code_size_analyzer_client.model.map_file_parse_response import MapFileParseResponse
+
+
+class ParserApi(object):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+
+    def __init__(self, api_client=None):
+        if api_client is None:
+            api_client = ApiClient()
+        self.api_client = api_client
+        self.parse_map_file_endpoint = _Endpoint(
+            settings={
+                'response_type': (MapFileParseResponse,),
+                'auth': [],
+                'endpoint_path': '/parse_map_file',
+                'operation_id': 'parse_map_file',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'map_file_parse_request',
+                ],
+                'required': [
+                    'map_file_parse_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'map_file_parse_request':
+                        (MapFileParseRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'map_file_parse_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+
+    def parse_map_file(
+        self,
+        map_file_parse_request,
+        **kwargs
+    ):
+        """Analyze Map File Post  # noqa: E501
+
+        parse a map file  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.parse_map_file(map_file_parse_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            map_file_parse_request (MapFileParseRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            MapFileParseResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['map_file_parse_request'] = \
+            map_file_parse_request
+        return self.parse_map_file_endpoint.call_with_http_info(**kwargs)
+
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/api/parser_api.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/api/analyzer_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.api_client import ApiClient, Endpoint as _Endpoint
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    check_allowed_values,
-    check_validations,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_and_convert_types
-)
-from code_size_analyzer_client.model.http_validation_error import HTTPValidationError
-from code_size_analyzer_client.model.map_file_parse_request import MapFileParseRequest
-from code_size_analyzer_client.model.map_file_parse_response import MapFileParseResponse
-
-
-class ParserApi(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-
-    def __init__(self, api_client=None):
-        if api_client is None:
-            api_client = ApiClient()
-        self.api_client = api_client
-        self.parse_map_file_endpoint = _Endpoint(
-            settings={
-                'response_type': (MapFileParseResponse,),
-                'auth': [],
-                'endpoint_path': '/parse_map_file',
-                'operation_id': 'parse_map_file',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'map_file_parse_request',
-                ],
-                'required': [
-                    'map_file_parse_request',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'map_file_parse_request':
-                        (MapFileParseRequest,),
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                    'map_file_parse_request': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
-
-    def parse_map_file(
-        self,
-        map_file_parse_request,
-        **kwargs
-    ):
-        """Analyze Map File Post  # noqa: E501
-
-        parse a map file  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.parse_map_file(map_file_parse_request, async_req=True)
-        >>> result = thread.get()
-
-        Args:
-            map_file_parse_request (MapFileParseRequest):
-
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            MapFileParseResponse
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['map_file_parse_request'] = \
-            map_file_parse_request
-        return self.parse_map_file_endpoint.call_with_http_info(**kwargs)
-
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.api_client import ApiClient, Endpoint as _Endpoint
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    check_allowed_values,
+    check_validations,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_and_convert_types
+)
+from code_size_analyzer_client.model.http_validation_error import HTTPValidationError
+from code_size_analyzer_client.model.map_file_request import MapFileRequest
+from code_size_analyzer_client.model.map_file_response import MapFileResponse
+
+
+class AnalyzerApi(object):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+
+    def __init__(self, api_client=None):
+        if api_client is None:
+            api_client = ApiClient()
+        self.api_client = api_client
+        self.analyze_map_file_endpoint = _Endpoint(
+            settings={
+                'response_type': (MapFileResponse,),
+                'auth': [],
+                'endpoint_path': '/analyze_map_file',
+                'operation_id': 'analyze_map_file',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'map_file_request',
+                ],
+                'required': [
+                    'map_file_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'map_file_request':
+                        (MapFileRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'map_file_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+
+    def analyze_map_file(
+        self,
+        map_file_request,
+        **kwargs
+    ):
+        """Analyze Map File Post  # noqa: E501
+
+        analyze a map file  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.analyze_map_file(map_file_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            map_file_request (MapFileRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            MapFileResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['map_file_request'] = \
+            map_file_request
+        return self.analyze_map_file_endpoint.call_with_http_info(**kwargs)
+
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/api/results_api.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/api/results_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,856 +1,879 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.api_client import ApiClient, Endpoint as _Endpoint
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    check_allowed_values,
-    check_validations,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_and_convert_types
-)
-from code_size_analyzer_client.model.application_combination import ApplicationCombination
-from code_size_analyzer_client.model.http_validation_error import HTTPValidationError
-from code_size_analyzer_client.model.target_info import TargetInfo
-
-
-class ResultsApi(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-
-    def __init__(self, api_client=None):
-        if api_client is None:
-            api_client = ApiClient()
-        self.api_client = api_client
-        self.get_app_analysis_details_endpoint = _Endpoint(
-            settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
-                'auth': [],
-                'endpoint_path': '/results/get_app_analysis_details',
-                'operation_id': 'get_app_analysis_details',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'stack',
-                    'target',
-                    'build',
-                    'app_name',
-                    'compiler',
-                ],
-                'required': [
-                    'stack',
-                    'target',
-                    'build',
-                    'app_name',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'stack':
-                        (str,),
-                    'target':
-                        (str,),
-                    'build':
-                        ([str],),
-                    'app_name':
-                        ([str],),
-                    'compiler':
-                        (str,),
-                },
-                'attribute_map': {
-                    'stack': 'stack',
-                    'target': 'target',
-                    'build': 'build',
-                    'app_name': 'app_name',
-                    'compiler': 'compiler',
-                },
-                'location_map': {
-                    'stack': 'query',
-                    'target': 'query',
-                    'build': 'query',
-                    'app_name': 'query',
-                    'compiler': 'query',
-                },
-                'collection_format_map': {
-                    'build': 'multi',
-                    'app_name': 'multi',
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.get_app_combinations_endpoint = _Endpoint(
-            settings={
-                'response_type': ([ApplicationCombination],),
-                'auth': [],
-                'endpoint_path': '/results/get_app_combinations',
-                'operation_id': 'get_app_combinations',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.get_app_stack_names_endpoint = _Endpoint(
-            settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
-                'auth': [],
-                'endpoint_path': '/results/get_app_stack_names',
-                'operation_id': 'get_app_stack_names',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'branch',
-                ],
-                'required': [
-                    'branch',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'branch':
-                        ([str],),
-                },
-                'attribute_map': {
-                    'branch': 'branch',
-                },
-                'location_map': {
-                    'branch': 'query',
-                },
-                'collection_format_map': {
-                    'branch': 'multi',
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.get_app_summary_records_endpoint = _Endpoint(
-            settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
-                'auth': [],
-                'endpoint_path': '/results/get_app_summary_records',
-                'operation_id': 'get_app_summary_records',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'stack',
-                    'application_name',
-                    'branch',
-                ],
-                'required': [
-                    'stack',
-                    'application_name',
-                    'branch',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'stack':
-                        (str,),
-                    'application_name':
-                        (str,),
-                    'branch':
-                        ([str],),
-                },
-                'attribute_map': {
-                    'stack': 'stack',
-                    'application_name': 'application_name',
-                    'branch': 'branch',
-                },
-                'location_map': {
-                    'stack': 'query',
-                    'application_name': 'query',
-                    'branch': 'query',
-                },
-                'collection_format_map': {
-                    'branch': 'multi',
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.get_branch_builds_endpoint = _Endpoint(
-            settings={
-                'response_type': ([bool, date, datetime, dict, float, int, list, str, none_type],),
-                'auth': [],
-                'endpoint_path': '/results/get_branch_builds',
-                'operation_id': 'get_branch_builds',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.get_target_info_endpoint = _Endpoint(
-            settings={
-                'response_type': ([TargetInfo],),
-                'auth': [],
-                'endpoint_path': '/results/get_target_info',
-                'operation_id': 'get_target_info',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-
-    def get_app_analysis_details(
-        self,
-        stack,
-        target,
-        build,
-        app_name,
-        **kwargs
-    ):
-        """Get App Analysis Details  # noqa: E501
-
-        Get the detailed analysis results for one or more apps  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_app_analysis_details(stack, target, build, app_name, async_req=True)
-        >>> result = thread.get()
-
-        Args:
-            stack (str):
-            target (str):
-            build ([str]):
-            app_name ([str]):
-
-        Keyword Args:
-            compiler (str): [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['stack'] = \
-            stack
-        kwargs['target'] = \
-            target
-        kwargs['build'] = \
-            build
-        kwargs['app_name'] = \
-            app_name
-        return self.get_app_analysis_details_endpoint.call_with_http_info(**kwargs)
-
-    def get_app_combinations(
-        self,
-        **kwargs
-    ):
-        """Get App Combinations  # noqa: E501
-
-        Get the set of combinations of app name / compiler / stack / target / board  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_app_combinations(async_req=True)
-        >>> result = thread.get()
-
-
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            [ApplicationCombination]
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.get_app_combinations_endpoint.call_with_http_info(**kwargs)
-
-    def get_app_stack_names(
-        self,
-        branch,
-        **kwargs
-    ):
-        """Get App Stack Names  # noqa: E501
-
-        Get the list of all analyzed app & stack combinations, filtered by branch  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_app_stack_names(branch, async_req=True)
-        >>> result = thread.get()
-
-        Args:
-            branch ([str]):
-
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['branch'] = \
-            branch
-        return self.get_app_stack_names_endpoint.call_with_http_info(**kwargs)
-
-    def get_app_summary_records(
-        self,
-        stack,
-        application_name,
-        branch,
-        **kwargs
-    ):
-        """Get App Summary Records  # noqa: E501
-
-        Get the high-level analysis results for an app  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_app_summary_records(stack, application_name, branch, async_req=True)
-        >>> result = thread.get()
-
-        Args:
-            stack (str):
-            application_name (str):
-            branch ([str]):
-
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['stack'] = \
-            stack
-        kwargs['application_name'] = \
-            application_name
-        kwargs['branch'] = \
-            branch
-        return self.get_app_summary_records_endpoint.call_with_http_info(**kwargs)
-
-    def get_branch_builds(
-        self,
-        **kwargs
-    ):
-        """Get Branch Builds  # noqa: E501
-
-        Get the list of all branch/build combinations  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_branch_builds(async_req=True)
-        >>> result = thread.get()
-
-
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            [bool, date, datetime, dict, float, int, list, str, none_type]
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.get_branch_builds_endpoint.call_with_http_info(**kwargs)
-
-    def get_target_info(
-        self,
-        **kwargs
-    ):
-        """Get Target Info  # noqa: E501
-
-        Get the list of all analyzed app names  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_target_info(async_req=True)
-        >>> result = thread.get()
-
-
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            [TargetInfo]
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.get_target_info_endpoint.call_with_http_info(**kwargs)
-
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.api_client import ApiClient, Endpoint as _Endpoint
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    check_allowed_values,
+    check_validations,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_and_convert_types
+)
+from code_size_analyzer_client.model.application_combination import ApplicationCombination
+from code_size_analyzer_client.model.http_validation_error import HTTPValidationError
+from code_size_analyzer_client.model.response_get_app_analysis_details_results_get_app_analysis_details_get import ResponseGetAppAnalysisDetailsResultsGetAppAnalysisDetailsGet
+from code_size_analyzer_client.model.target_info import TargetInfo
+
+
+class ResultsApi(object):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+
+    def __init__(self, api_client=None):
+        if api_client is None:
+            api_client = ApiClient()
+        self.api_client = api_client
+        self.get_app_analysis_details_endpoint = _Endpoint(
+            settings={
+                'response_type': (ResponseGetAppAnalysisDetailsResultsGetAppAnalysisDetailsGet,),
+                'auth': [],
+                'endpoint_path': '/results/get_app_analysis_details',
+                'operation_id': 'get_app_analysis_details',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'stack',
+                    'target',
+                    'build',
+                    'app_name',
+                    'compiler',
+                    'board',
+                    'result_format',
+                ],
+                'required': [
+                    'stack',
+                    'target',
+                    'build',
+                    'app_name',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                    'result_format',
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                    ('result_format',): {
+
+                        "LIST": "list",
+                        "BY_BUILD": "by_build",
+                        "BY_APP_NAME": "by_app_name"
+                    },
+                },
+                'openapi_types': {
+                    'stack':
+                        (str,),
+                    'target':
+                        (str,),
+                    'build':
+                        ([str],),
+                    'app_name':
+                        ([str],),
+                    'compiler':
+                        (str,),
+                    'board':
+                        (str,),
+                    'result_format':
+                        (str,),
+                },
+                'attribute_map': {
+                    'stack': 'stack',
+                    'target': 'target',
+                    'build': 'build',
+                    'app_name': 'app_name',
+                    'compiler': 'compiler',
+                    'board': 'board',
+                    'result_format': 'result_format',
+                },
+                'location_map': {
+                    'stack': 'query',
+                    'target': 'query',
+                    'build': 'query',
+                    'app_name': 'query',
+                    'compiler': 'query',
+                    'board': 'query',
+                    'result_format': 'query',
+                },
+                'collection_format_map': {
+                    'build': 'multi',
+                    'app_name': 'multi',
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_app_combinations_endpoint = _Endpoint(
+            settings={
+                'response_type': ([ApplicationCombination],),
+                'auth': [],
+                'endpoint_path': '/results/get_app_combinations',
+                'operation_id': 'get_app_combinations',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_app_stack_names_endpoint = _Endpoint(
+            settings={
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'auth': [],
+                'endpoint_path': '/results/get_app_stack_names',
+                'operation_id': 'get_app_stack_names',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'branch',
+                ],
+                'required': [
+                    'branch',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'branch':
+                        ([str],),
+                },
+                'attribute_map': {
+                    'branch': 'branch',
+                },
+                'location_map': {
+                    'branch': 'query',
+                },
+                'collection_format_map': {
+                    'branch': 'multi',
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_app_summary_records_endpoint = _Endpoint(
+            settings={
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'auth': [],
+                'endpoint_path': '/results/get_app_summary_records',
+                'operation_id': 'get_app_summary_records',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'stack',
+                    'application_name',
+                    'branch',
+                    'sdk_commit_hash',
+                ],
+                'required': [
+                    'stack',
+                    'application_name',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'stack':
+                        (str,),
+                    'application_name':
+                        (str,),
+                    'branch':
+                        ([str],),
+                    'sdk_commit_hash':
+                        ([str],),
+                },
+                'attribute_map': {
+                    'stack': 'stack',
+                    'application_name': 'application_name',
+                    'branch': 'branch',
+                    'sdk_commit_hash': 'sdk_commit_hash',
+                },
+                'location_map': {
+                    'stack': 'query',
+                    'application_name': 'query',
+                    'branch': 'query',
+                    'sdk_commit_hash': 'query',
+                },
+                'collection_format_map': {
+                    'branch': 'multi',
+                    'sdk_commit_hash': 'multi',
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_branch_builds_endpoint = _Endpoint(
+            settings={
+                'response_type': ([bool, date, datetime, dict, float, int, list, str, none_type],),
+                'auth': [],
+                'endpoint_path': '/results/get_branch_builds',
+                'operation_id': 'get_branch_builds',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_target_info_endpoint = _Endpoint(
+            settings={
+                'response_type': ([TargetInfo],),
+                'auth': [],
+                'endpoint_path': '/results/get_target_info',
+                'operation_id': 'get_target_info',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+
+    def get_app_analysis_details(
+        self,
+        stack,
+        target,
+        build,
+        app_name,
+        **kwargs
+    ):
+        """Get App Analysis Details  # noqa: E501
+
+        Get the detailed analysis results for one or more apps  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_app_analysis_details(stack, target, build, app_name, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            stack (str):
+            target (str):
+            build ([str]):
+            app_name ([str]):
+
+        Keyword Args:
+            compiler (str): [optional]
+            board (str): [optional]
+            result_format (str): [optional] if omitted the server will use the default value of "list"
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ResponseGetAppAnalysisDetailsResultsGetAppAnalysisDetailsGet
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['stack'] = \
+            stack
+        kwargs['target'] = \
+            target
+        kwargs['build'] = \
+            build
+        kwargs['app_name'] = \
+            app_name
+        return self.get_app_analysis_details_endpoint.call_with_http_info(**kwargs)
+
+    def get_app_combinations(
+        self,
+        **kwargs
+    ):
+        """Get App Combinations  # noqa: E501
+
+        Get the set of combinations of app name / compiler / stack / target / board  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_app_combinations(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [ApplicationCombination]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.get_app_combinations_endpoint.call_with_http_info(**kwargs)
+
+    def get_app_stack_names(
+        self,
+        branch,
+        **kwargs
+    ):
+        """Get App Stack Names  # noqa: E501
+
+        Get the list of all analyzed app & stack combinations, filtered by branch  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_app_stack_names(branch, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            branch ([str]):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            bool, date, datetime, dict, float, int, list, str, none_type
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['branch'] = \
+            branch
+        return self.get_app_stack_names_endpoint.call_with_http_info(**kwargs)
+
+    def get_app_summary_records(
+        self,
+        stack,
+        application_name,
+        **kwargs
+    ):
+        """Get App Summary Records  # noqa: E501
+
+        Get the high-level analysis results for an app  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_app_summary_records(stack, application_name, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            stack (str):
+            application_name (str):
+
+        Keyword Args:
+            branch ([str]): [optional] if omitted the server will use the default value of []
+            sdk_commit_hash ([str]): [optional] if omitted the server will use the default value of []
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            bool, date, datetime, dict, float, int, list, str, none_type
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['stack'] = \
+            stack
+        kwargs['application_name'] = \
+            application_name
+        return self.get_app_summary_records_endpoint.call_with_http_info(**kwargs)
+
+    def get_branch_builds(
+        self,
+        **kwargs
+    ):
+        """Get Branch Builds  # noqa: E501
+
+        Get the list of all branch/build combinations  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_branch_builds(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [bool, date, datetime, dict, float, int, list, str, none_type]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.get_branch_builds_endpoint.call_with_http_info(**kwargs)
+
+    def get_target_info(
+        self,
+        **kwargs
+    ):
+        """Get Target Info  # noqa: E501
+
+        Get the list of all analyzed app names  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_target_info(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [TargetInfo]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.get_target_info_endpoint.call_with_http_info(**kwargs)
+
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/apis/__init__.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/apis/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-
-# flake8: noqa
-
-# Import all APIs into this package.
-# If you have many APIs here with many many models used in each API this may
-# raise a `RecursionError`.
-# In order to avoid this, import only the API that you directly need like:
-#
-#   from code_size_analyzer_client.api.analyzer_api import AnalyzerApi
-#
-# or import this package, but before doing it, use:
-#
-#   import sys
-#   sys.setrecursionlimit(n)
-
-# Import APIs into API package:
-from code_size_analyzer_client.api.analyzer_api import AnalyzerApi
-from code_size_analyzer_client.api.default_api import DefaultApi
-from code_size_analyzer_client.api.parser_api import ParserApi
-from code_size_analyzer_client.api.results_api import ResultsApi
+
+# flake8: noqa
+
+# Import all APIs into this package.
+# If you have many APIs here with many many models used in each API this may
+# raise a `RecursionError`.
+# In order to avoid this, import only the API that you directly need like:
+#
+#   from code_size_analyzer_client.api.analyzer_api import AnalyzerApi
+#
+# or import this package, but before doing it, use:
+#
+#   import sys
+#   sys.setrecursionlimit(n)
+
+# Import APIs into API package:
+from code_size_analyzer_client.api.analyzer_api import AnalyzerApi
+from code_size_analyzer_client.api.default_api import DefaultApi
+from code_size_analyzer_client.api.parser_api import ParserApi
+from code_size_analyzer_client.api.results_api import ResultsApi
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/configuration.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/configuration.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,450 +1,450 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import copy
-import logging
-import multiprocessing
-import sys
-import urllib3
-
-from http import client as http_client
-from code_size_analyzer_client.exceptions import ApiValueError
-
-
-JSON_SCHEMA_VALIDATION_KEYWORDS = {
-    'multipleOf', 'maximum', 'exclusiveMaximum',
-    'minimum', 'exclusiveMinimum', 'maxLength',
-    'minLength', 'pattern', 'maxItems', 'minItems'
-}
-
-class Configuration(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-
-    Ref: https://openapi-generator.tech
-    Do not edit the class manually.
-
-    :param host: Base url
-    :param api_key: Dict to store API key(s).
-      Each entry in the dict specifies an API key.
-      The dict key is the name of the security scheme in the OAS specification.
-      The dict value is the API key secret.
-    :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
-      The dict key is the name of the security scheme in the OAS specification.
-      The dict value is an API key prefix when generating the auth data.
-    :param username: Username for HTTP basic authentication
-    :param password: Password for HTTP basic authentication
-    :param discard_unknown_keys: Boolean value indicating whether to discard
-      unknown properties. A server may send a response that includes additional
-      properties that are not known by the client in the following scenarios:
-      1. The OpenAPI document is incomplete, i.e. it does not match the server
-         implementation.
-      2. The client was generated using an older version of the OpenAPI document
-         and the server has been upgraded since then.
-      If a schema in the OpenAPI document defines the additionalProperties attribute,
-      then all undeclared properties received by the server are injected into the
-      additional properties map. In that case, there are undeclared properties, and
-      nothing to discard.
-    :param disabled_client_side_validations (string): Comma-separated list of
-      JSON schema validation keywords to disable JSON schema structural validation
-      rules. The following keywords may be specified: multipleOf, maximum,
-      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
-      maxItems, minItems.
-      By default, the validation is performed for data generated locally by the client
-      and data received from the server, independent of any validation performed by
-      the server side. If the input data does not satisfy the JSON schema validation
-      rules specified in the OpenAPI document, an exception is raised.
-      If disabled_client_side_validations is set, structural validation is
-      disabled. This can be useful to troubleshoot data validation problem, such as
-      when the OpenAPI document validation rules do not match the actual API data
-      received by the server.
-    :param server_index: Index to servers configuration.
-    :param server_variables: Mapping with string values to replace variables in
-      templated server configuration. The validation of enums is performed for
-      variables with defined enum values before.
-    :param server_operation_index: Mapping from operation ID to an index to server
-      configuration.
-    :param server_operation_variables: Mapping from operation ID to a mapping with
-      string values to replace variables in templated server configuration.
-      The validation of enums is performed for variables with defined enum values before.
-    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
-      in PEM format
-
-    """
-
-    _default = None
-
-    def __init__(self, host=None,
-                 api_key=None, api_key_prefix=None,
-                 access_token=None,
-                 username=None, password=None,
-                 discard_unknown_keys=False,
-                 disabled_client_side_validations="",
-                 server_index=None, server_variables=None,
-                 server_operation_index=None, server_operation_variables=None,
-                 ssl_ca_cert=None,
-                 ):
-        """Constructor
-        """
-        self._base_path = "https://code-size-analyzer.silabs.net" if host is None else host
-        """Default Base url
-        """
-        self.server_index = 0 if server_index is None and host is None else server_index
-        self.server_operation_index = server_operation_index or {}
-        """Default server index
-        """
-        self.server_variables = server_variables or {}
-        self.server_operation_variables = server_operation_variables or {}
-        """Default server variables
-        """
-        self.temp_folder_path = None
-        """Temp file folder for downloading files
-        """
-        # Authentication Settings
-        self.access_token = access_token
-        self.api_key = {}
-        if api_key:
-            self.api_key = api_key
-        """dict to store API key(s)
-        """
-        self.api_key_prefix = {}
-        if api_key_prefix:
-            self.api_key_prefix = api_key_prefix
-        """dict to store API prefix (e.g. Bearer)
-        """
-        self.refresh_api_key_hook = None
-        """function hook to refresh API key if expired
-        """
-        self.username = username
-        """Username for HTTP basic authentication
-        """
-        self.password = password
-        """Password for HTTP basic authentication
-        """
-        self.discard_unknown_keys = discard_unknown_keys
-        self.disabled_client_side_validations = disabled_client_side_validations
-        self.logger = {}
-        """Logging Settings
-        """
-        self.logger["package_logger"] = logging.getLogger("code_size_analyzer_client")
-        self.logger["urllib3_logger"] = logging.getLogger("urllib3")
-        self.logger_format = '%(asctime)s %(levelname)s %(message)s'
-        """Log format
-        """
-        self.logger_stream_handler = None
-        """Log stream handler
-        """
-        self.logger_file_handler = None
-        """Log file handler
-        """
-        self.logger_file = None
-        """Debug file location
-        """
-        self.debug = False
-        """Debug switch
-        """
-
-        self.verify_ssl = True
-        """SSL/TLS verification
-           Set this to false to skip verifying SSL certificate when calling API
-           from https server.
-        """
-        self.ssl_ca_cert = ssl_ca_cert
-        """Set this to customize the certificate file to verify the peer.
-        """
-        self.cert_file = None
-        """client certificate file
-        """
-        self.key_file = None
-        """client key file
-        """
-        self.assert_hostname = None
-        """Set this to True/False to enable/disable SSL hostname verification.
-        """
-
-        self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
-        """urllib3 connection pool's maximum number of connections saved
-           per pool. urllib3 uses 1 connection as default value, but this is
-           not the best value when you are making a lot of possibly parallel
-           requests to the same host, which is often the case here.
-           cpu_count * 5 is used as default value to increase performance.
-        """
-
-        self.proxy = None
-        """Proxy URL
-        """
-        self.no_proxy = None
-        """bypass proxy for host in the no_proxy list.
-        """
-        self.proxy_headers = None
-        """Proxy headers
-        """
-        self.safe_chars_for_path_param = ''
-        """Safe chars for path_param
-        """
-        self.retries = None
-        """Adding retries to override urllib3 default value 3
-        """
-        # Enable client side validation
-        self.client_side_validation = True
-
-        # Options to pass down to the underlying urllib3 socket
-        self.socket_options = None
-
-    def __deepcopy__(self, memo):
-        cls = self.__class__
-        result = cls.__new__(cls)
-        memo[id(self)] = result
-        for k, v in self.__dict__.items():
-            if k not in ('logger', 'logger_file_handler'):
-                setattr(result, k, copy.deepcopy(v, memo))
-        # shallow copy of loggers
-        result.logger = copy.copy(self.logger)
-        # use setters to configure loggers
-        result.logger_file = self.logger_file
-        result.debug = self.debug
-        return result
-
-    def __setattr__(self, name, value):
-        object.__setattr__(self, name, value)
-        if name == 'disabled_client_side_validations':
-            s = set(filter(None, value.split(',')))
-            for v in s:
-                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError(
-                        "Invalid keyword: '{0}''".format(v))
-            self._disabled_client_side_validations = s
-
-    @classmethod
-    def set_default(cls, default):
-        """Set default instance of configuration.
-
-        It stores default configuration, which can be
-        returned by get_default_copy method.
-
-        :param default: object of Configuration
-        """
-        cls._default = copy.deepcopy(default)
-
-    @classmethod
-    def get_default_copy(cls):
-        """Return new instance of configuration.
-
-        This method returns newly created, based on default constructor,
-        object of Configuration class or returns a copy of default
-        configuration passed by the set_default method.
-
-        :return: The configuration object.
-        """
-        if cls._default is not None:
-            return copy.deepcopy(cls._default)
-        return Configuration()
-
-    @property
-    def logger_file(self):
-        """The logger file.
-
-        If the logger_file is None, then add stream handler and remove file
-        handler. Otherwise, add file handler and remove stream handler.
-
-        :param value: The logger_file path.
-        :type: str
-        """
-        return self.__logger_file
-
-    @logger_file.setter
-    def logger_file(self, value):
-        """The logger file.
-
-        If the logger_file is None, then add stream handler and remove file
-        handler. Otherwise, add file handler and remove stream handler.
-
-        :param value: The logger_file path.
-        :type: str
-        """
-        self.__logger_file = value
-        if self.__logger_file:
-            # If set logging file,
-            # then add file handler and remove stream handler.
-            self.logger_file_handler = logging.FileHandler(self.__logger_file)
-            self.logger_file_handler.setFormatter(self.logger_formatter)
-            for _, logger in self.logger.items():
-                logger.addHandler(self.logger_file_handler)
-
-    @property
-    def debug(self):
-        """Debug status
-
-        :param value: The debug status, True or False.
-        :type: bool
-        """
-        return self.__debug
-
-    @debug.setter
-    def debug(self, value):
-        """Debug status
-
-        :param value: The debug status, True or False.
-        :type: bool
-        """
-        self.__debug = value
-        if self.__debug:
-            # if debug status is True, turn on debug logging
-            for _, logger in self.logger.items():
-                logger.setLevel(logging.DEBUG)
-            # turn on http_client debug
-            http_client.HTTPConnection.debuglevel = 1
-        else:
-            # if debug status is False, turn off debug logging,
-            # setting log level to default `logging.WARNING`
-            for _, logger in self.logger.items():
-                logger.setLevel(logging.WARNING)
-            # turn off http_client debug
-            http_client.HTTPConnection.debuglevel = 0
-
-    @property
-    def logger_format(self):
-        """The logger format.
-
-        The logger_formatter will be updated when sets logger_format.
-
-        :param value: The format string.
-        :type: str
-        """
-        return self.__logger_format
-
-    @logger_format.setter
-    def logger_format(self, value):
-        """The logger format.
-
-        The logger_formatter will be updated when sets logger_format.
-
-        :param value: The format string.
-        :type: str
-        """
-        self.__logger_format = value
-        self.logger_formatter = logging.Formatter(self.__logger_format)
-
-    def get_api_key_with_prefix(self, identifier, alias=None):
-        """Gets API key (with prefix if set).
-
-        :param identifier: The identifier of apiKey.
-        :param alias: The alternative identifier of apiKey.
-        :return: The token for api key authentication.
-        """
-        if self.refresh_api_key_hook is not None:
-            self.refresh_api_key_hook(self)
-        key = self.api_key.get(identifier, self.api_key.get(alias) if alias is not None else None)
-        if key:
-            prefix = self.api_key_prefix.get(identifier)
-            if prefix:
-                return "%s %s" % (prefix, key)
-            else:
-                return key
-
-    def get_basic_auth_token(self):
-        """Gets HTTP basic authentication header (string).
-
-        :return: The token for basic HTTP authentication.
-        """
-        username = ""
-        if self.username is not None:
-            username = self.username
-        password = ""
-        if self.password is not None:
-            password = self.password
-        return urllib3.util.make_headers(
-            basic_auth=username + ':' + password
-        ).get('authorization')
-
-    def auth_settings(self):
-        """Gets Auth Settings dict for api client.
-
-        :return: The Auth Settings information dict.
-        """
-        auth = {}
-        return auth
-
-    def to_debug_report(self):
-        """Gets the essential information for debugging.
-
-        :return: The report for debugging.
-        """
-        return "Python SDK Debug Report:\n"\
-               "OS: {env}\n"\
-               "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 0.5.0".\
-               format(env=sys.platform, pyversion=sys.version)
-
-    def get_host_settings(self):
-        """Gets an array of host settings
-
-        :return: An array of host settings
-        """
-        return [
-            {
-                'url': "https://code-size-analyzer.silabs.net",
-                'description': "Production server",
-            },
-            {
-                'url': "https://code-size-analyzer.dev.silabs.net",
-                'description': "Development server",
-            }
-        ]
-
-    def get_host_from_settings(self, index, variables=None, servers=None):
-        """Gets host URL based on the index and variables
-        :param index: array index of the host settings
-        :param variables: hash of variable and the corresponding value
-        :param servers: an array of host settings or None
-        :return: URL based on host settings
-        """
-        if index is None:
-            return self._base_path
-
-        variables = {} if variables is None else variables
-        servers = self.get_host_settings() if servers is None else servers
-
-        try:
-            server = servers[index]
-        except IndexError:
-            raise ValueError(
-                "Invalid index {0} when selecting the host settings. "
-                "Must be less than {1}".format(index, len(servers)))
-
-        url = server['url']
-
-        # go through variables and replace placeholders
-        for variable_name, variable in server.get('variables', {}).items():
-            used_value = variables.get(
-                variable_name, variable['default_value'])
-
-            if 'enum_values' in variable \
-                    and used_value not in variable['enum_values']:
-                raise ValueError(
-                    "The variable `{0}` in the host URL has invalid value "
-                    "{1}. Must be {2}.".format(
-                        variable_name, variables[variable_name],
-                        variable['enum_values']))
-
-            url = url.replace("{" + variable_name + "}", used_value)
-
-        return url
-
-    @property
-    def host(self):
-        """Return generated host."""
-        return self.get_host_from_settings(self.server_index, variables=self.server_variables)
-
-    @host.setter
-    def host(self, value):
-        """Fix base path."""
-        self._base_path = value
-        self.server_index = None
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import copy
+import logging
+import multiprocessing
+import sys
+import urllib3
+
+from http import client as http_client
+from code_size_analyzer_client.exceptions import ApiValueError
+
+
+JSON_SCHEMA_VALIDATION_KEYWORDS = {
+    'multipleOf', 'maximum', 'exclusiveMaximum',
+    'minimum', 'exclusiveMinimum', 'maxLength',
+    'minLength', 'pattern', 'maxItems', 'minItems'
+}
+
+class Configuration(object):
+    """NOTE: This class is auto generated by OpenAPI Generator
+
+    Ref: https://openapi-generator.tech
+    Do not edit the class manually.
+
+    :param host: Base url
+    :param api_key: Dict to store API key(s).
+      Each entry in the dict specifies an API key.
+      The dict key is the name of the security scheme in the OAS specification.
+      The dict value is the API key secret.
+    :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
+      The dict key is the name of the security scheme in the OAS specification.
+      The dict value is an API key prefix when generating the auth data.
+    :param username: Username for HTTP basic authentication
+    :param password: Password for HTTP basic authentication
+    :param discard_unknown_keys: Boolean value indicating whether to discard
+      unknown properties. A server may send a response that includes additional
+      properties that are not known by the client in the following scenarios:
+      1. The OpenAPI document is incomplete, i.e. it does not match the server
+         implementation.
+      2. The client was generated using an older version of the OpenAPI document
+         and the server has been upgraded since then.
+      If a schema in the OpenAPI document defines the additionalProperties attribute,
+      then all undeclared properties received by the server are injected into the
+      additional properties map. In that case, there are undeclared properties, and
+      nothing to discard.
+    :param disabled_client_side_validations (string): Comma-separated list of
+      JSON schema validation keywords to disable JSON schema structural validation
+      rules. The following keywords may be specified: multipleOf, maximum,
+      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
+      maxItems, minItems.
+      By default, the validation is performed for data generated locally by the client
+      and data received from the server, independent of any validation performed by
+      the server side. If the input data does not satisfy the JSON schema validation
+      rules specified in the OpenAPI document, an exception is raised.
+      If disabled_client_side_validations is set, structural validation is
+      disabled. This can be useful to troubleshoot data validation problem, such as
+      when the OpenAPI document validation rules do not match the actual API data
+      received by the server.
+    :param server_index: Index to servers configuration.
+    :param server_variables: Mapping with string values to replace variables in
+      templated server configuration. The validation of enums is performed for
+      variables with defined enum values before.
+    :param server_operation_index: Mapping from operation ID to an index to server
+      configuration.
+    :param server_operation_variables: Mapping from operation ID to a mapping with
+      string values to replace variables in templated server configuration.
+      The validation of enums is performed for variables with defined enum values before.
+    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
+      in PEM format
+
+    """
+
+    _default = None
+
+    def __init__(self, host=None,
+                 api_key=None, api_key_prefix=None,
+                 access_token=None,
+                 username=None, password=None,
+                 discard_unknown_keys=False,
+                 disabled_client_side_validations="",
+                 server_index=None, server_variables=None,
+                 server_operation_index=None, server_operation_variables=None,
+                 ssl_ca_cert=None,
+                 ):
+        """Constructor
+        """
+        self._base_path = "https://code-size-analyzer.silabs.net" if host is None else host
+        """Default Base url
+        """
+        self.server_index = 0 if server_index is None and host is None else server_index
+        self.server_operation_index = server_operation_index or {}
+        """Default server index
+        """
+        self.server_variables = server_variables or {}
+        self.server_operation_variables = server_operation_variables or {}
+        """Default server variables
+        """
+        self.temp_folder_path = None
+        """Temp file folder for downloading files
+        """
+        # Authentication Settings
+        self.access_token = access_token
+        self.api_key = {}
+        if api_key:
+            self.api_key = api_key
+        """dict to store API key(s)
+        """
+        self.api_key_prefix = {}
+        if api_key_prefix:
+            self.api_key_prefix = api_key_prefix
+        """dict to store API prefix (e.g. Bearer)
+        """
+        self.refresh_api_key_hook = None
+        """function hook to refresh API key if expired
+        """
+        self.username = username
+        """Username for HTTP basic authentication
+        """
+        self.password = password
+        """Password for HTTP basic authentication
+        """
+        self.discard_unknown_keys = discard_unknown_keys
+        self.disabled_client_side_validations = disabled_client_side_validations
+        self.logger = {}
+        """Logging Settings
+        """
+        self.logger["package_logger"] = logging.getLogger("code_size_analyzer_client")
+        self.logger["urllib3_logger"] = logging.getLogger("urllib3")
+        self.logger_format = '%(asctime)s %(levelname)s %(message)s'
+        """Log format
+        """
+        self.logger_stream_handler = None
+        """Log stream handler
+        """
+        self.logger_file_handler = None
+        """Log file handler
+        """
+        self.logger_file = None
+        """Debug file location
+        """
+        self.debug = False
+        """Debug switch
+        """
+
+        self.verify_ssl = True
+        """SSL/TLS verification
+           Set this to false to skip verifying SSL certificate when calling API
+           from https server.
+        """
+        self.ssl_ca_cert = ssl_ca_cert
+        """Set this to customize the certificate file to verify the peer.
+        """
+        self.cert_file = None
+        """client certificate file
+        """
+        self.key_file = None
+        """client key file
+        """
+        self.assert_hostname = None
+        """Set this to True/False to enable/disable SSL hostname verification.
+        """
+
+        self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
+        """urllib3 connection pool's maximum number of connections saved
+           per pool. urllib3 uses 1 connection as default value, but this is
+           not the best value when you are making a lot of possibly parallel
+           requests to the same host, which is often the case here.
+           cpu_count * 5 is used as default value to increase performance.
+        """
+
+        self.proxy = None
+        """Proxy URL
+        """
+        self.no_proxy = None
+        """bypass proxy for host in the no_proxy list.
+        """
+        self.proxy_headers = None
+        """Proxy headers
+        """
+        self.safe_chars_for_path_param = ''
+        """Safe chars for path_param
+        """
+        self.retries = None
+        """Adding retries to override urllib3 default value 3
+        """
+        # Enable client side validation
+        self.client_side_validation = True
+
+        # Options to pass down to the underlying urllib3 socket
+        self.socket_options = None
+
+    def __deepcopy__(self, memo):
+        cls = self.__class__
+        result = cls.__new__(cls)
+        memo[id(self)] = result
+        for k, v in self.__dict__.items():
+            if k not in ('logger', 'logger_file_handler'):
+                setattr(result, k, copy.deepcopy(v, memo))
+        # shallow copy of loggers
+        result.logger = copy.copy(self.logger)
+        # use setters to configure loggers
+        result.logger_file = self.logger_file
+        result.debug = self.debug
+        return result
+
+    def __setattr__(self, name, value):
+        object.__setattr__(self, name, value)
+        if name == 'disabled_client_side_validations':
+            s = set(filter(None, value.split(',')))
+            for v in s:
+                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
+                    raise ApiValueError(
+                        "Invalid keyword: '{0}''".format(v))
+            self._disabled_client_side_validations = s
+
+    @classmethod
+    def set_default(cls, default):
+        """Set default instance of configuration.
+
+        It stores default configuration, which can be
+        returned by get_default_copy method.
+
+        :param default: object of Configuration
+        """
+        cls._default = copy.deepcopy(default)
+
+    @classmethod
+    def get_default_copy(cls):
+        """Return new instance of configuration.
+
+        This method returns newly created, based on default constructor,
+        object of Configuration class or returns a copy of default
+        configuration passed by the set_default method.
+
+        :return: The configuration object.
+        """
+        if cls._default is not None:
+            return copy.deepcopy(cls._default)
+        return Configuration()
+
+    @property
+    def logger_file(self):
+        """The logger file.
+
+        If the logger_file is None, then add stream handler and remove file
+        handler. Otherwise, add file handler and remove stream handler.
+
+        :param value: The logger_file path.
+        :type: str
+        """
+        return self.__logger_file
+
+    @logger_file.setter
+    def logger_file(self, value):
+        """The logger file.
+
+        If the logger_file is None, then add stream handler and remove file
+        handler. Otherwise, add file handler and remove stream handler.
+
+        :param value: The logger_file path.
+        :type: str
+        """
+        self.__logger_file = value
+        if self.__logger_file:
+            # If set logging file,
+            # then add file handler and remove stream handler.
+            self.logger_file_handler = logging.FileHandler(self.__logger_file)
+            self.logger_file_handler.setFormatter(self.logger_formatter)
+            for _, logger in self.logger.items():
+                logger.addHandler(self.logger_file_handler)
+
+    @property
+    def debug(self):
+        """Debug status
+
+        :param value: The debug status, True or False.
+        :type: bool
+        """
+        return self.__debug
+
+    @debug.setter
+    def debug(self, value):
+        """Debug status
+
+        :param value: The debug status, True or False.
+        :type: bool
+        """
+        self.__debug = value
+        if self.__debug:
+            # if debug status is True, turn on debug logging
+            for _, logger in self.logger.items():
+                logger.setLevel(logging.DEBUG)
+            # turn on http_client debug
+            http_client.HTTPConnection.debuglevel = 1
+        else:
+            # if debug status is False, turn off debug logging,
+            # setting log level to default `logging.WARNING`
+            for _, logger in self.logger.items():
+                logger.setLevel(logging.WARNING)
+            # turn off http_client debug
+            http_client.HTTPConnection.debuglevel = 0
+
+    @property
+    def logger_format(self):
+        """The logger format.
+
+        The logger_formatter will be updated when sets logger_format.
+
+        :param value: The format string.
+        :type: str
+        """
+        return self.__logger_format
+
+    @logger_format.setter
+    def logger_format(self, value):
+        """The logger format.
+
+        The logger_formatter will be updated when sets logger_format.
+
+        :param value: The format string.
+        :type: str
+        """
+        self.__logger_format = value
+        self.logger_formatter = logging.Formatter(self.__logger_format)
+
+    def get_api_key_with_prefix(self, identifier, alias=None):
+        """Gets API key (with prefix if set).
+
+        :param identifier: The identifier of apiKey.
+        :param alias: The alternative identifier of apiKey.
+        :return: The token for api key authentication.
+        """
+        if self.refresh_api_key_hook is not None:
+            self.refresh_api_key_hook(self)
+        key = self.api_key.get(identifier, self.api_key.get(alias) if alias is not None else None)
+        if key:
+            prefix = self.api_key_prefix.get(identifier)
+            if prefix:
+                return "%s %s" % (prefix, key)
+            else:
+                return key
+
+    def get_basic_auth_token(self):
+        """Gets HTTP basic authentication header (string).
+
+        :return: The token for basic HTTP authentication.
+        """
+        username = ""
+        if self.username is not None:
+            username = self.username
+        password = ""
+        if self.password is not None:
+            password = self.password
+        return urllib3.util.make_headers(
+            basic_auth=username + ':' + password
+        ).get('authorization')
+
+    def auth_settings(self):
+        """Gets Auth Settings dict for api client.
+
+        :return: The Auth Settings information dict.
+        """
+        auth = {}
+        return auth
+
+    def to_debug_report(self):
+        """Gets the essential information for debugging.
+
+        :return: The report for debugging.
+        """
+        return "Python SDK Debug Report:\n"\
+               "OS: {env}\n"\
+               "Python Version: {pyversion}\n"\
+               "Version of the API: 0.1.0\n"\
+               "SDK Package Version: 0.7.0".\
+               format(env=sys.platform, pyversion=sys.version)
+
+    def get_host_settings(self):
+        """Gets an array of host settings
+
+        :return: An array of host settings
+        """
+        return [
+            {
+                'url': "https://code-size-analyzer.silabs.net",
+                'description': "Production server",
+            },
+            {
+                'url': "https://code-size-analyzer.dev.silabs.net",
+                'description': "Development server",
+            }
+        ]
+
+    def get_host_from_settings(self, index, variables=None, servers=None):
+        """Gets host URL based on the index and variables
+        :param index: array index of the host settings
+        :param variables: hash of variable and the corresponding value
+        :param servers: an array of host settings or None
+        :return: URL based on host settings
+        """
+        if index is None:
+            return self._base_path
+
+        variables = {} if variables is None else variables
+        servers = self.get_host_settings() if servers is None else servers
+
+        try:
+            server = servers[index]
+        except IndexError:
+            raise ValueError(
+                "Invalid index {0} when selecting the host settings. "
+                "Must be less than {1}".format(index, len(servers)))
+
+        url = server['url']
+
+        # go through variables and replace placeholders
+        for variable_name, variable in server.get('variables', {}).items():
+            used_value = variables.get(
+                variable_name, variable['default_value'])
+
+            if 'enum_values' in variable \
+                    and used_value not in variable['enum_values']:
+                raise ValueError(
+                    "The variable `{0}` in the host URL has invalid value "
+                    "{1}. Must be {2}.".format(
+                        variable_name, variables[variable_name],
+                        variable['enum_values']))
+
+            url = url.replace("{" + variable_name + "}", used_value)
+
+        return url
+
+    @property
+    def host(self):
+        """Return generated host."""
+        return self.get_host_from_settings(self.server_index, variables=self.server_variables)
+
+    @host.setter
+    def host(self, value):
+        """Fix base path."""
+        self._base_path = value
+        self.server_index = None
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/exceptions.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/exceptions.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-class OpenApiException(Exception):
-    """The base exception class for all OpenAPIExceptions"""
-
-
-class ApiTypeError(OpenApiException, TypeError):
-    def __init__(self, msg, path_to_item=None, valid_classes=None,
-                 key_type=None):
-        """ Raises an exception for TypeErrors
-
-        Args:
-            msg (str): the exception message
-
-        Keyword Args:
-            path_to_item (list): a list of keys an indices to get to the
-                                 current_item
-                                 None if unset
-            valid_classes (tuple): the primitive classes that current item
-                                   should be an instance of
-                                   None if unset
-            key_type (bool): False if our value is a value in a dict
-                             True if it is a key in a dict
-                             False if our item is an item in a list
-                             None if unset
-        """
-        self.path_to_item = path_to_item
-        self.valid_classes = valid_classes
-        self.key_type = key_type
-        full_msg = msg
-        if path_to_item:
-            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
-        super(ApiTypeError, self).__init__(full_msg)
-
-
-class ApiValueError(OpenApiException, ValueError):
-    def __init__(self, msg, path_to_item=None):
-        """
-        Args:
-            msg (str): the exception message
-
-        Keyword Args:
-            path_to_item (list) the path to the exception in the
-                received_data dict. None if unset
-        """
-
-        self.path_to_item = path_to_item
-        full_msg = msg
-        if path_to_item:
-            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
-        super(ApiValueError, self).__init__(full_msg)
-
-
-class ApiAttributeError(OpenApiException, AttributeError):
-    def __init__(self, msg, path_to_item=None):
-        """
-        Raised when an attribute reference or assignment fails.
-
-        Args:
-            msg (str): the exception message
-
-        Keyword Args:
-            path_to_item (None/list) the path to the exception in the
-                received_data dict
-        """
-        self.path_to_item = path_to_item
-        full_msg = msg
-        if path_to_item:
-            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
-        super(ApiAttributeError, self).__init__(full_msg)
-
-
-class ApiKeyError(OpenApiException, KeyError):
-    def __init__(self, msg, path_to_item=None):
-        """
-        Args:
-            msg (str): the exception message
-
-        Keyword Args:
-            path_to_item (None/list) the path to the exception in the
-                received_data dict
-        """
-        self.path_to_item = path_to_item
-        full_msg = msg
-        if path_to_item:
-            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
-        super(ApiKeyError, self).__init__(full_msg)
-
-
-class ApiException(OpenApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        if http_resp:
-            self.status = http_resp.status
-            self.reason = http_resp.reason
-            self.body = http_resp.data
-            self.headers = http_resp.getheaders()
-        else:
-            self.status = status
-            self.reason = reason
-            self.body = None
-            self.headers = None
-
-    def __str__(self):
-        """Custom error messages for exception"""
-        error_message = "Status Code: {0}\n"\
-                        "Reason: {1}\n".format(self.status, self.reason)
-        if self.headers:
-            error_message += "HTTP response headers: {0}\n".format(
-                self.headers)
-
-        if self.body:
-            error_message += "HTTP response body: {0}\n".format(self.body)
-
-        return error_message
-
-
-class NotFoundException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(NotFoundException, self).__init__(status, reason, http_resp)
-
-
-class UnauthorizedException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(UnauthorizedException, self).__init__(status, reason, http_resp)
-
-
-class ForbiddenException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ForbiddenException, self).__init__(status, reason, http_resp)
-
-
-class ServiceException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ServiceException, self).__init__(status, reason, http_resp)
-
-
-def render_path(path_to_item):
-    """Returns a string representation of a path"""
-    result = ""
-    for pth in path_to_item:
-        if isinstance(pth, int):
-            result += "[{0}]".format(pth)
-        else:
-            result += "['{0}']".format(pth)
-    return result
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+class OpenApiException(Exception):
+    """The base exception class for all OpenAPIExceptions"""
+
+
+class ApiTypeError(OpenApiException, TypeError):
+    def __init__(self, msg, path_to_item=None, valid_classes=None,
+                 key_type=None):
+        """ Raises an exception for TypeErrors
+
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (list): a list of keys an indices to get to the
+                                 current_item
+                                 None if unset
+            valid_classes (tuple): the primitive classes that current item
+                                   should be an instance of
+                                   None if unset
+            key_type (bool): False if our value is a value in a dict
+                             True if it is a key in a dict
+                             False if our item is an item in a list
+                             None if unset
+        """
+        self.path_to_item = path_to_item
+        self.valid_classes = valid_classes
+        self.key_type = key_type
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiTypeError, self).__init__(full_msg)
+
+
+class ApiValueError(OpenApiException, ValueError):
+    def __init__(self, msg, path_to_item=None):
+        """
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (list) the path to the exception in the
+                received_data dict. None if unset
+        """
+
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiValueError, self).__init__(full_msg)
+
+
+class ApiAttributeError(OpenApiException, AttributeError):
+    def __init__(self, msg, path_to_item=None):
+        """
+        Raised when an attribute reference or assignment fails.
+
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (None/list) the path to the exception in the
+                received_data dict
+        """
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiAttributeError, self).__init__(full_msg)
+
+
+class ApiKeyError(OpenApiException, KeyError):
+    def __init__(self, msg, path_to_item=None):
+        """
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (None/list) the path to the exception in the
+                received_data dict
+        """
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiKeyError, self).__init__(full_msg)
+
+
+class ApiException(OpenApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        if http_resp:
+            self.status = http_resp.status
+            self.reason = http_resp.reason
+            self.body = http_resp.data
+            self.headers = http_resp.getheaders()
+        else:
+            self.status = status
+            self.reason = reason
+            self.body = None
+            self.headers = None
+
+    def __str__(self):
+        """Custom error messages for exception"""
+        error_message = "Status Code: {0}\n"\
+                        "Reason: {1}\n".format(self.status, self.reason)
+        if self.headers:
+            error_message += "HTTP response headers: {0}\n".format(
+                self.headers)
+
+        if self.body:
+            error_message += "HTTP response body: {0}\n".format(self.body)
+
+        return error_message
+
+
+class NotFoundException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(NotFoundException, self).__init__(status, reason, http_resp)
+
+
+class UnauthorizedException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(UnauthorizedException, self).__init__(status, reason, http_resp)
+
+
+class ForbiddenException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ForbiddenException, self).__init__(status, reason, http_resp)
+
+
+class ServiceException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ServiceException, self).__init__(status, reason, http_resp)
+
+
+def render_path(path_to_item):
+    """Returns a string representation of a path"""
+    result = ""
+    for pth in path_to_item:
+        if isinstance(pth, int):
+            result += "[{0}]".format(pth)
+        else:
+            result += "['{0}']".format(pth)
+    return result
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/application_combination.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/response_get_app_analysis_details_results_get_app_analysis_details_get.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,293 +1,265 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-
-class ApplicationCombination(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'application_name': (str,),  # noqa: E501
-            'stack': (str,),  # noqa: E501
-            'compiler': (str,),  # noqa: E501
-            'target': (str,),  # noqa: E501
-            'board': (str,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'application_name': 'application_name',  # noqa: E501
-        'stack': 'stack',  # noqa: E501
-        'compiler': 'compiler',  # noqa: E501
-        'target': 'target',  # noqa: E501
-        'board': 'board',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, application_name, stack, compiler, target, board, *args, **kwargs):  # noqa: E501
-        """ApplicationCombination - a model defined in OpenAPI
-
-        Args:
-            application_name (str):
-            stack (str):
-            compiler (str):
-            target (str):
-            board (str):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.application_name = application_name
-        self.stack = stack
-        self.compiler = compiler
-        self.target = target
-        self.board = board
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, application_name, stack, compiler, target, board, *args, **kwargs):  # noqa: E501
-        """ApplicationCombination - a model defined in OpenAPI
-
-        Args:
-            application_name (str):
-            stack (str):
-            compiler (str):
-            target (str):
-            board (str):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.application_name = application_name
-        self.stack = stack
-        self.compiler = compiler
-        self.target = target
-        self.board = board
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from code_size_analyzer_client.model.application_analysis_result_with_detail import ApplicationAnalysisResultWithDetail
+    globals()['ApplicationAnalysisResultWithDetail'] = ApplicationAnalysisResultWithDetail
+
+
+class ResponseGetAppAnalysisDetailsResultsGetAppAnalysisDetailsGet(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ResponseGetAppAnalysisDetailsResultsGetAppAnalysisDetailsGet - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ResponseGetAppAnalysisDetailsResultsGetAppAnalysisDetailsGet - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/classification_rule.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/classification_rule.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,287 +1,287 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-
-class ClassificationRule(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'matcher': (str,),  # noqa: E501
-            'module': (str,),  # noqa: E501
-            'component': (str,),  # noqa: E501
-            'team_owner': (str,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'matcher': 'matcher',  # noqa: E501
-        'module': 'module',  # noqa: E501
-        'component': 'component',  # noqa: E501
-        'team_owner': 'team_owner',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, matcher, module, component, team_owner, *args, **kwargs):  # noqa: E501
-        """ClassificationRule - a model defined in OpenAPI
-
-        Args:
-            matcher (str): string representation of lambda function for a source file/library to this category.  Lambda function takes a 'data' parameter which has 'file_name' and 'library_name' attributes
-            module (str): Module category for this file/library.  Should be one of 'Toolchain' ,'Platform' ,'OSI_NETWORK' ,'OSI_APP' ,'Security' ,'BOOTLOADER' ,'NON VOLATILE MEMORY'
-            component (str): name of component
-            team_owner (str): name of owning team
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.matcher = matcher
-        self.module = module
-        self.component = component
-        self.team_owner = team_owner
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, matcher, module, component, team_owner, *args, **kwargs):  # noqa: E501
-        """ClassificationRule - a model defined in OpenAPI
-
-        Args:
-            matcher (str): string representation of lambda function for a source file/library to this category.  Lambda function takes a 'data' parameter which has 'file_name' and 'library_name' attributes
-            module (str): Module category for this file/library.  Should be one of 'Toolchain' ,'Platform' ,'OSI_NETWORK' ,'OSI_APP' ,'Security' ,'BOOTLOADER' ,'NON VOLATILE MEMORY'
-            component (str): name of component
-            team_owner (str): name of owning team
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.matcher = matcher
-        self.module = module
-        self.component = component
-        self.team_owner = team_owner
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+
+class ClassificationRule(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'matcher': (str,),  # noqa: E501
+            'module': (str,),  # noqa: E501
+            'component': (str,),  # noqa: E501
+            'team_owner': (str,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'matcher': 'matcher',  # noqa: E501
+        'module': 'module',  # noqa: E501
+        'component': 'component',  # noqa: E501
+        'team_owner': 'team_owner',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, matcher, module, component, team_owner, *args, **kwargs):  # noqa: E501
+        """ClassificationRule - a model defined in OpenAPI
+
+        Args:
+            matcher (str): string representation of lambda function for a source file/library to this category.  Lambda function takes a 'data' parameter which has 'file_name' and 'library_name' attributes
+            module (str): Module category for this file/library.  Should be one of 'Toolchain' ,'Platform' ,'OSI_NETWORK' ,'OSI_APP' ,'Security' ,'BOOTLOADER' ,'NON VOLATILE MEMORY'
+            component (str): name of component
+            team_owner (str): name of owning team
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.matcher = matcher
+        self.module = module
+        self.component = component
+        self.team_owner = team_owner
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, matcher, module, component, team_owner, *args, **kwargs):  # noqa: E501
+        """ClassificationRule - a model defined in OpenAPI
+
+        Args:
+            matcher (str): string representation of lambda function for a source file/library to this category.  Lambda function takes a 'data' parameter which has 'file_name' and 'library_name' attributes
+            module (str): Module category for this file/library.  Should be one of 'Toolchain' ,'Platform' ,'OSI_NETWORK' ,'OSI_APP' ,'Security' ,'BOOTLOADER' ,'NON VOLATILE MEMORY'
+            component (str): name of component
+            team_owner (str): name of owning team
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.matcher = matcher
+        self.module = module
+        self.component = component
+        self.team_owner = team_owner
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/data_record.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/data_record.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,323 +1,323 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-
-class DataRecord(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'code_size': (int,),  # noqa: E501
-            'ram_size': (int,),  # noqa: E501
-            'library_name': (str, none_type,),  # noqa: E501
-            'file_name': (str, none_type,),  # noqa: E501
-            'distribution_type': (str, none_type,),  # noqa: E501
-            'mode': (str, none_type,),  # noqa: E501
-            'role': (str, none_type,),  # noqa: E501
-            'target': (str, none_type,),  # noqa: E501
-            'module': (str, none_type,),  # noqa: E501
-            'component': (str, none_type,),  # noqa: E501
-            'team_owner': (str, none_type,),  # noqa: E501
-            'path_in_source': (str, none_type,),  # noqa: E501
-            'uc_component_path': (str, none_type,),  # noqa: E501
-            'uc_categories': ([str],),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'code_size': 'code_size',  # noqa: E501
-        'ram_size': 'RAM_size',  # noqa: E501
-        'library_name': 'library_name',  # noqa: E501
-        'file_name': 'file_name',  # noqa: E501
-        'distribution_type': 'distribution_type',  # noqa: E501
-        'mode': 'mode',  # noqa: E501
-        'role': 'role',  # noqa: E501
-        'target': 'target',  # noqa: E501
-        'module': 'module',  # noqa: E501
-        'component': 'component',  # noqa: E501
-        'team_owner': 'team_owner',  # noqa: E501
-        'path_in_source': 'path_in_source',  # noqa: E501
-        'uc_component_path': 'uc_component_path',  # noqa: E501
-        'uc_categories': 'uc_categories',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, code_size, ram_size, *args, **kwargs):  # noqa: E501
-        """DataRecord - a model defined in OpenAPI
-
-        Args:
-            code_size (int):
-            ram_size (int):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            library_name (str, none_type): [optional]  # noqa: E501
-            file_name (str, none_type): [optional]  # noqa: E501
-            distribution_type (str, none_type): [optional]  # noqa: E501
-            mode (str, none_type): [optional]  # noqa: E501
-            role (str, none_type): [optional]  # noqa: E501
-            target (str, none_type): [optional]  # noqa: E501
-            module (str, none_type): [optional]  # noqa: E501
-            component (str, none_type): [optional]  # noqa: E501
-            team_owner (str, none_type): [optional]  # noqa: E501
-            path_in_source (str, none_type): [optional]  # noqa: E501
-            uc_component_path (str, none_type): [optional]  # noqa: E501
-            uc_categories ([str]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.code_size = code_size
-        self.ram_size = ram_size
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, code_size, ram_size, *args, **kwargs):  # noqa: E501
-        """DataRecord - a model defined in OpenAPI
-
-        Args:
-            code_size (int):
-            ram_size (int):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            library_name (str, none_type): [optional]  # noqa: E501
-            file_name (str, none_type): [optional]  # noqa: E501
-            distribution_type (str, none_type): [optional]  # noqa: E501
-            mode (str, none_type): [optional]  # noqa: E501
-            role (str, none_type): [optional]  # noqa: E501
-            target (str, none_type): [optional]  # noqa: E501
-            module (str, none_type): [optional]  # noqa: E501
-            component (str, none_type): [optional]  # noqa: E501
-            team_owner (str, none_type): [optional]  # noqa: E501
-            path_in_source (str, none_type): [optional]  # noqa: E501
-            uc_component_path (str, none_type): [optional]  # noqa: E501
-            uc_categories ([str]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.code_size = code_size
-        self.ram_size = ram_size
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+
+class DataRecord(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'code_size': (int,),  # noqa: E501
+            'ram_size': (int,),  # noqa: E501
+            'library_name': (str, none_type,),  # noqa: E501
+            'file_name': (str, none_type,),  # noqa: E501
+            'distribution_type': (str, none_type,),  # noqa: E501
+            'mode': (str, none_type,),  # noqa: E501
+            'role': (str, none_type,),  # noqa: E501
+            'target': (str, none_type,),  # noqa: E501
+            'module': (str, none_type,),  # noqa: E501
+            'component': (str, none_type,),  # noqa: E501
+            'team_owner': (str, none_type,),  # noqa: E501
+            'path_in_source': (str, none_type,),  # noqa: E501
+            'uc_component_path': (str, none_type,),  # noqa: E501
+            'uc_categories': ([str],),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'code_size': 'code_size',  # noqa: E501
+        'ram_size': 'RAM_size',  # noqa: E501
+        'library_name': 'library_name',  # noqa: E501
+        'file_name': 'file_name',  # noqa: E501
+        'distribution_type': 'distribution_type',  # noqa: E501
+        'mode': 'mode',  # noqa: E501
+        'role': 'role',  # noqa: E501
+        'target': 'target',  # noqa: E501
+        'module': 'module',  # noqa: E501
+        'component': 'component',  # noqa: E501
+        'team_owner': 'team_owner',  # noqa: E501
+        'path_in_source': 'path_in_source',  # noqa: E501
+        'uc_component_path': 'uc_component_path',  # noqa: E501
+        'uc_categories': 'uc_categories',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, code_size, ram_size, *args, **kwargs):  # noqa: E501
+        """DataRecord - a model defined in OpenAPI
+
+        Args:
+            code_size (int):
+            ram_size (int):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            library_name (str, none_type): [optional]  # noqa: E501
+            file_name (str, none_type): [optional]  # noqa: E501
+            distribution_type (str, none_type): [optional]  # noqa: E501
+            mode (str, none_type): [optional]  # noqa: E501
+            role (str, none_type): [optional]  # noqa: E501
+            target (str, none_type): [optional]  # noqa: E501
+            module (str, none_type): [optional]  # noqa: E501
+            component (str, none_type): [optional]  # noqa: E501
+            team_owner (str, none_type): [optional]  # noqa: E501
+            path_in_source (str, none_type): [optional]  # noqa: E501
+            uc_component_path (str, none_type): [optional]  # noqa: E501
+            uc_categories ([str]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.code_size = code_size
+        self.ram_size = ram_size
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, code_size, ram_size, *args, **kwargs):  # noqa: E501
+        """DataRecord - a model defined in OpenAPI
+
+        Args:
+            code_size (int):
+            ram_size (int):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            library_name (str, none_type): [optional]  # noqa: E501
+            file_name (str, none_type): [optional]  # noqa: E501
+            distribution_type (str, none_type): [optional]  # noqa: E501
+            mode (str, none_type): [optional]  # noqa: E501
+            role (str, none_type): [optional]  # noqa: E501
+            target (str, none_type): [optional]  # noqa: E501
+            module (str, none_type): [optional]  # noqa: E501
+            component (str, none_type): [optional]  # noqa: E501
+            team_owner (str, none_type): [optional]  # noqa: E501
+            path_in_source (str, none_type): [optional]  # noqa: E501
+            uc_component_path (str, none_type): [optional]  # noqa: E501
+            uc_categories ([str]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.code_size = code_size
+        self.ram_size = ram_size
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/http_validation_error.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/map_file_parse_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,269 +1,269 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from code_size_analyzer_client.model.validation_error import ValidationError
-    globals()['ValidationError'] = ValidationError
-
-
-class HTTPValidationError(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'detail': ([ValidationError],),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'detail': 'detail',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """HTTPValidationError - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            detail ([ValidationError]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """HTTPValidationError - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            detail ([ValidationError]): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+
+class MapFileParseRequest(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'map_file': (str,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'map_file': 'map_file',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, map_file, *args, **kwargs):  # noqa: E501
+        """MapFileParseRequest - a model defined in OpenAPI
+
+        Args:
+            map_file (str): base64-encoded string representation of map file contents
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.map_file = map_file
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, map_file, *args, **kwargs):  # noqa: E501
+        """MapFileParseRequest - a model defined in OpenAPI
+
+        Args:
+            map_file (str): base64-encoded string representation of map file contents
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.map_file = map_file
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_memory_config.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/map_file_memory_config.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,329 +1,329 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from code_size_analyzer_client.model.map_file_section import MapFileSection
-    globals()['MapFileSection'] = MapFileSection
-
-
-class MapFileMemoryConfig(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'name': (str,),  # noqa: E501
-            'origin': (int,),  # noqa: E501
-            'size': (int,),  # noqa: E501
-            'attr': (str,),  # noqa: E501
-            'end': (int,),  # noqa: E501
-            'sections': ([MapFileSection],),  # noqa: E501
-            'registered_sections': ([MapFileSection],),  # noqa: E501
-            'unregistered_sections': ([MapFileSection],),  # noqa: E501
-            'used_space': (int,),  # noqa: E501
-            'free_space': (int,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'name': 'name',  # noqa: E501
-        'origin': 'origin',  # noqa: E501
-        'size': 'size',  # noqa: E501
-        'attr': 'attr',  # noqa: E501
-        'end': 'end',  # noqa: E501
-        'sections': 'sections',  # noqa: E501
-        'registered_sections': 'registered_sections',  # noqa: E501
-        'unregistered_sections': 'unregistered_sections',  # noqa: E501
-        'used_space': 'used_space',  # noqa: E501
-        'free_space': 'free_space',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, origin, size, attr, end, sections, registered_sections, unregistered_sections, used_space, free_space, *args, **kwargs):  # noqa: E501
-        """MapFileMemoryConfig - a model defined in OpenAPI
-
-        Args:
-            name (str):
-            origin (int):
-            size (int):
-            attr (str):
-            end (int):
-            sections ([MapFileSection]):
-            registered_sections ([MapFileSection]):
-            unregistered_sections ([MapFileSection]):
-            used_space (int):
-            free_space (int):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.name = name
-        self.origin = origin
-        self.size = size
-        self.attr = attr
-        self.end = end
-        self.sections = sections
-        self.registered_sections = registered_sections
-        self.unregistered_sections = unregistered_sections
-        self.used_space = used_space
-        self.free_space = free_space
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, name, origin, size, attr, end, sections, registered_sections, unregistered_sections, used_space, free_space, *args, **kwargs):  # noqa: E501
-        """MapFileMemoryConfig - a model defined in OpenAPI
-
-        Args:
-            name (str):
-            origin (int):
-            size (int):
-            attr (str):
-            end (int):
-            sections ([MapFileSection]):
-            registered_sections ([MapFileSection]):
-            unregistered_sections ([MapFileSection]):
-            used_space (int):
-            free_space (int):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.name = name
-        self.origin = origin
-        self.size = size
-        self.attr = attr
-        self.end = end
-        self.sections = sections
-        self.registered_sections = registered_sections
-        self.unregistered_sections = unregistered_sections
-        self.used_space = used_space
-        self.free_space = free_space
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from code_size_analyzer_client.model.map_file_section import MapFileSection
+    globals()['MapFileSection'] = MapFileSection
+
+
+class MapFileMemoryConfig(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'name': (str,),  # noqa: E501
+            'origin': (int,),  # noqa: E501
+            'size': (int,),  # noqa: E501
+            'attr': (str,),  # noqa: E501
+            'end': (int,),  # noqa: E501
+            'sections': ([MapFileSection],),  # noqa: E501
+            'registered_sections': ([MapFileSection],),  # noqa: E501
+            'unregistered_sections': ([MapFileSection],),  # noqa: E501
+            'used_space': (int,),  # noqa: E501
+            'free_space': (int,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'name': 'name',  # noqa: E501
+        'origin': 'origin',  # noqa: E501
+        'size': 'size',  # noqa: E501
+        'attr': 'attr',  # noqa: E501
+        'end': 'end',  # noqa: E501
+        'sections': 'sections',  # noqa: E501
+        'registered_sections': 'registered_sections',  # noqa: E501
+        'unregistered_sections': 'unregistered_sections',  # noqa: E501
+        'used_space': 'used_space',  # noqa: E501
+        'free_space': 'free_space',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, name, origin, size, attr, end, sections, registered_sections, unregistered_sections, used_space, free_space, *args, **kwargs):  # noqa: E501
+        """MapFileMemoryConfig - a model defined in OpenAPI
+
+        Args:
+            name (str):
+            origin (int):
+            size (int):
+            attr (str):
+            end (int):
+            sections ([MapFileSection]):
+            registered_sections ([MapFileSection]):
+            unregistered_sections ([MapFileSection]):
+            used_space (int):
+            free_space (int):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.name = name
+        self.origin = origin
+        self.size = size
+        self.attr = attr
+        self.end = end
+        self.sections = sections
+        self.registered_sections = registered_sections
+        self.unregistered_sections = unregistered_sections
+        self.used_space = used_space
+        self.free_space = free_space
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, name, origin, size, attr, end, sections, registered_sections, unregistered_sections, used_space, free_space, *args, **kwargs):  # noqa: E501
+        """MapFileMemoryConfig - a model defined in OpenAPI
+
+        Args:
+            name (str):
+            origin (int):
+            size (int):
+            attr (str):
+            end (int):
+            sections ([MapFileSection]):
+            registered_sections ([MapFileSection]):
+            unregistered_sections ([MapFileSection]):
+            used_space (int):
+            free_space (int):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.name = name
+        self.origin = origin
+        self.size = size
+        self.attr = attr
+        self.end = end
+        self.sections = sections
+        self.registered_sections = registered_sections
+        self.unregistered_sections = unregistered_sections
+        self.used_space = used_space
+        self.free_space = free_space
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_parse_request.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/section_summary.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,269 +1,275 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-
-class MapFileParseRequest(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'map_file': (str,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'map_file': 'map_file',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, map_file, *args, **kwargs):  # noqa: E501
-        """MapFileParseRequest - a model defined in OpenAPI
-
-        Args:
-            map_file (str): base64-encoded string representation of map file contents
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.map_file = map_file
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, map_file, *args, **kwargs):  # noqa: E501
-        """MapFileParseRequest - a model defined in OpenAPI
-
-        Args:
-            map_file (str): base64-encoded string representation of map file contents
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.map_file = map_file
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+
+class SectionSummary(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'code_size': (int,),  # noqa: E501
+            'ram_size': (int,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'code_size': 'codeSize',  # noqa: E501
+        'ram_size': 'RAMSize',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, code_size, ram_size, *args, **kwargs):  # noqa: E501
+        """SectionSummary - a model defined in OpenAPI
+
+        Args:
+            code_size (int):
+            ram_size (int):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.code_size = code_size
+        self.ram_size = ram_size
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, code_size, ram_size, *args, **kwargs):  # noqa: E501
+        """SectionSummary - a model defined in OpenAPI
+
+        Args:
+            code_size (int):
+            ram_size (int):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.code_size = code_size
+        self.ram_size = ram_size
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_parse_response.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/module.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,295 +1,293 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from code_size_analyzer_client.model.map_file_memory_config import MapFileMemoryConfig
-    from code_size_analyzer_client.model.map_file_summary import MapFileSummary
-    globals()['MapFileMemoryConfig'] = MapFileMemoryConfig
-    globals()['MapFileSummary'] = MapFileSummary
-
-
-class MapFileParseResponse(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'compiler_type': (str,),  # noqa: E501
-            'flash': (MapFileMemoryConfig,),  # noqa: E501
-            'ram': (MapFileMemoryConfig,),  # noqa: E501
-            'summary': (MapFileSummary,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'compiler_type': 'compiler_type',  # noqa: E501
-        'flash': 'flash',  # noqa: E501
-        'ram': 'ram',  # noqa: E501
-        'summary': 'summary',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, compiler_type, flash, ram, summary, *args, **kwargs):  # noqa: E501
-        """MapFileParseResponse - a model defined in OpenAPI
-
-        Args:
-            compiler_type (str):
-            flash (MapFileMemoryConfig):
-            ram (MapFileMemoryConfig):
-            summary (MapFileSummary):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.compiler_type = compiler_type
-        self.flash = flash
-        self.ram = ram
-        self.summary = summary
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, compiler_type, flash, ram, summary, *args, **kwargs):  # noqa: E501
-        """MapFileParseResponse - a model defined in OpenAPI
-
-        Args:
-            compiler_type (str):
-            flash (MapFileMemoryConfig):
-            ram (MapFileMemoryConfig):
-            summary (MapFileSummary):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.compiler_type = compiler_type
-        self.flash = flash
-        self.ram = ram
-        self.summary = summary
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from code_size_analyzer_client.model.symbol import Symbol
+    globals()['Symbol'] = Symbol
+
+
+class Module(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'flash_size': (int,),  # noqa: E501
+            'ram_size': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'symbols': ([Symbol],),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'flash_size': 'flash_size',  # noqa: E501
+        'ram_size': 'ram_size',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'symbols': 'symbols',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, flash_size, ram_size, name, symbols, *args, **kwargs):  # noqa: E501
+        """Module - a model defined in OpenAPI
+
+        Args:
+            flash_size (int):
+            ram_size (int):
+            name (str):
+            symbols ([Symbol]):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.flash_size = flash_size
+        self.ram_size = ram_size
+        self.name = name
+        self.symbols = symbols
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, flash_size, ram_size, name, symbols, *args, **kwargs):  # noqa: E501
+        """Module - a model defined in OpenAPI
+
+        Args:
+            flash_size (int):
+            ram_size (int):
+            name (str):
+            symbols ([Symbol]):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.flash_size = flash_size
+        self.ram_size = ram_size
+        self.name = name
+        self.symbols = symbols
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_request.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/map_file_request.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,341 +1,341 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from code_size_analyzer_client.model.classification_rule import ClassificationRule
-    globals()['ClassificationRule'] = ClassificationRule
-
-
-class MapFileRequest(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'map_file': (str,),  # noqa: E501
-            'stack_name': (str,),  # noqa: E501
-            'target_part': (str,),  # noqa: E501
-            'compiler': (str,),  # noqa: E501
-            'target_board': (str,),  # noqa: E501
-            'app_name': (str,),  # noqa: E501
-            'project_file': (str,),  # noqa: E501
-            'project_file_name': (str,),  # noqa: E501
-            'branch_name': (str,),  # noqa: E501
-            'build_number': (str,),  # noqa: E501
-            'commit': (str,),  # noqa: E501
-            'store_results': (bool,),  # noqa: E501
-            'build_url': (str,),  # noqa: E501
-            'classification_rules': ([ClassificationRule],),  # noqa: E501
-            'ignore_default_rules': (bool,),  # noqa: E501
-            'uc_component_branch_name': (str,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'map_file': 'map_file',  # noqa: E501
-        'stack_name': 'stack_name',  # noqa: E501
-        'target_part': 'target_part',  # noqa: E501
-        'compiler': 'compiler',  # noqa: E501
-        'target_board': 'target_board',  # noqa: E501
-        'app_name': 'app_name',  # noqa: E501
-        'project_file': 'project_file',  # noqa: E501
-        'project_file_name': 'project_file_name',  # noqa: E501
-        'branch_name': 'branch_name',  # noqa: E501
-        'build_number': 'build_number',  # noqa: E501
-        'commit': 'commit',  # noqa: E501
-        'store_results': 'store_results',  # noqa: E501
-        'build_url': 'build_url',  # noqa: E501
-        'classification_rules': 'classification_rules',  # noqa: E501
-        'ignore_default_rules': 'ignore_default_rules',  # noqa: E501
-        'uc_component_branch_name': 'uc_component_branch_name',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, map_file, stack_name, target_part, compiler, *args, **kwargs):  # noqa: E501
-        """MapFileRequest - a model defined in OpenAPI
-
-        Args:
-            map_file (str): base64-encoded string representation of map file contents
-            stack_name (str): end product name; e.g. zigbee
-            target_part (str): target part OPN; e.g. 'efr32mg22c224f512im40'
-            compiler (str): compiler that produced the map file.  Must be one of 'iar' or 'gcc'
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            target_board (str): Optional board name; e.g. brd4181a.  Required if store_results is True. [optional]  # noqa: E501
-            app_name (str): Name of application; e.g. soc_empty.  Required if store_results is True. [optional]  # noqa: E501
-            project_file (str): base64-encoded string representation of project file contents. [optional]  # noqa: E501
-            project_file_name (str): project file name. [optional]  # noqa: E501
-            branch_name (str): branch name; e.g. 'develop/22q2'.  Required if store_results is True. [optional]  # noqa: E501
-            build_number (str): build number; e.g. b1234.  Required if store_results is True. [optional]  # noqa: E501
-            commit (str): [optional]  # noqa: E501
-            store_results (bool): set to True to store results to reporting database. [optional]  # noqa: E501
-            build_url (str): [optional]  # noqa: E501
-            classification_rules ([ClassificationRule]): optional list of ClassificationRule objects to add additional classification rules. [optional]  # noqa: E501
-            ignore_default_rules (bool): Set to true to ignore default classification rules and exclusively use rules from classification_rules. [optional] if omitted the server will use the default value of False  # noqa: E501
-            uc_component_branch_name (str): branch name for uc component database; e.g. 'develop/22q2'. [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.map_file = map_file
-        self.stack_name = stack_name
-        self.target_part = target_part
-        self.compiler = compiler
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, map_file, stack_name, target_part, compiler, *args, **kwargs):  # noqa: E501
-        """MapFileRequest - a model defined in OpenAPI
-
-        Args:
-            map_file (str): base64-encoded string representation of map file contents
-            stack_name (str): end product name; e.g. zigbee
-            target_part (str): target part OPN; e.g. 'efr32mg22c224f512im40'
-            compiler (str): compiler that produced the map file.  Must be one of 'iar' or 'gcc'
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            target_board (str): Optional board name; e.g. brd4181a.  Required if store_results is True. [optional]  # noqa: E501
-            app_name (str): Name of application; e.g. soc_empty.  Required if store_results is True. [optional]  # noqa: E501
-            project_file (str): base64-encoded string representation of project file contents. [optional]  # noqa: E501
-            project_file_name (str): project file name. [optional]  # noqa: E501
-            branch_name (str): branch name; e.g. 'develop/22q2'.  Required if store_results is True. [optional]  # noqa: E501
-            build_number (str): build number; e.g. b1234.  Required if store_results is True. [optional]  # noqa: E501
-            commit (str): [optional]  # noqa: E501
-            store_results (bool): set to True to store results to reporting database. [optional]  # noqa: E501
-            build_url (str): [optional]  # noqa: E501
-            classification_rules ([ClassificationRule]): optional list of ClassificationRule objects to add additional classification rules. [optional]  # noqa: E501
-            ignore_default_rules (bool): Set to true to ignore default classification rules and exclusively use rules from classification_rules. [optional] if omitted the server will use the default value of False  # noqa: E501
-            uc_component_branch_name (str): branch name for uc component database; e.g. 'develop/22q2'. [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.map_file = map_file
-        self.stack_name = stack_name
-        self.target_part = target_part
-        self.compiler = compiler
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from code_size_analyzer_client.model.classification_rule import ClassificationRule
+    globals()['ClassificationRule'] = ClassificationRule
+
+
+class MapFileRequest(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'map_file': (str,),  # noqa: E501
+            'stack_name': (str,),  # noqa: E501
+            'target_part': (str,),  # noqa: E501
+            'compiler': (str,),  # noqa: E501
+            'target_board': (str,),  # noqa: E501
+            'app_name': (str,),  # noqa: E501
+            'project_file': (str,),  # noqa: E501
+            'project_file_name': (str,),  # noqa: E501
+            'branch_name': (str,),  # noqa: E501
+            'build_number': (str,),  # noqa: E501
+            'commit': (str,),  # noqa: E501
+            'store_results': (bool,),  # noqa: E501
+            'build_url': (str,),  # noqa: E501
+            'classification_rules': ([ClassificationRule],),  # noqa: E501
+            'ignore_default_rules': (bool,),  # noqa: E501
+            'uc_component_branch_name': (str,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'map_file': 'map_file',  # noqa: E501
+        'stack_name': 'stack_name',  # noqa: E501
+        'target_part': 'target_part',  # noqa: E501
+        'compiler': 'compiler',  # noqa: E501
+        'target_board': 'target_board',  # noqa: E501
+        'app_name': 'app_name',  # noqa: E501
+        'project_file': 'project_file',  # noqa: E501
+        'project_file_name': 'project_file_name',  # noqa: E501
+        'branch_name': 'branch_name',  # noqa: E501
+        'build_number': 'build_number',  # noqa: E501
+        'commit': 'commit',  # noqa: E501
+        'store_results': 'store_results',  # noqa: E501
+        'build_url': 'build_url',  # noqa: E501
+        'classification_rules': 'classification_rules',  # noqa: E501
+        'ignore_default_rules': 'ignore_default_rules',  # noqa: E501
+        'uc_component_branch_name': 'uc_component_branch_name',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, map_file, stack_name, target_part, compiler, *args, **kwargs):  # noqa: E501
+        """MapFileRequest - a model defined in OpenAPI
+
+        Args:
+            map_file (str): base64-encoded string representation of map file contents
+            stack_name (str): end product name; e.g. zigbee
+            target_part (str): target part OPN; e.g. 'efr32mg22c224f512im40'
+            compiler (str): compiler that produced the map file.  Must be one of 'iar' or 'gcc'
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            target_board (str): Optional board name; e.g. brd4181a.  Required if store_results is True. [optional]  # noqa: E501
+            app_name (str): Name of application; e.g. soc_empty.  Required if store_results is True. [optional]  # noqa: E501
+            project_file (str): base64-encoded string representation of project file contents. [optional]  # noqa: E501
+            project_file_name (str): project file name. [optional]  # noqa: E501
+            branch_name (str): branch name; e.g. 'develop/22q2'.  Required if store_results is True. [optional]  # noqa: E501
+            build_number (str): build number; e.g. b1234.  Required if store_results is True. [optional]  # noqa: E501
+            commit (str): [optional]  # noqa: E501
+            store_results (bool): set to True to store results to reporting database. [optional]  # noqa: E501
+            build_url (str): [optional]  # noqa: E501
+            classification_rules ([ClassificationRule]): optional list of ClassificationRule objects to add additional classification rules. [optional]  # noqa: E501
+            ignore_default_rules (bool): Set to true to ignore default classification rules and exclusively use rules from classification_rules. [optional] if omitted the server will use the default value of False  # noqa: E501
+            uc_component_branch_name (str): branch name for uc component database; e.g. 'develop/22q2'. [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.map_file = map_file
+        self.stack_name = stack_name
+        self.target_part = target_part
+        self.compiler = compiler
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, map_file, stack_name, target_part, compiler, *args, **kwargs):  # noqa: E501
+        """MapFileRequest - a model defined in OpenAPI
+
+        Args:
+            map_file (str): base64-encoded string representation of map file contents
+            stack_name (str): end product name; e.g. zigbee
+            target_part (str): target part OPN; e.g. 'efr32mg22c224f512im40'
+            compiler (str): compiler that produced the map file.  Must be one of 'iar' or 'gcc'
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            target_board (str): Optional board name; e.g. brd4181a.  Required if store_results is True. [optional]  # noqa: E501
+            app_name (str): Name of application; e.g. soc_empty.  Required if store_results is True. [optional]  # noqa: E501
+            project_file (str): base64-encoded string representation of project file contents. [optional]  # noqa: E501
+            project_file_name (str): project file name. [optional]  # noqa: E501
+            branch_name (str): branch name; e.g. 'develop/22q2'.  Required if store_results is True. [optional]  # noqa: E501
+            build_number (str): build number; e.g. b1234.  Required if store_results is True. [optional]  # noqa: E501
+            commit (str): [optional]  # noqa: E501
+            store_results (bool): set to True to store results to reporting database. [optional]  # noqa: E501
+            build_url (str): [optional]  # noqa: E501
+            classification_rules ([ClassificationRule]): optional list of ClassificationRule objects to add additional classification rules. [optional]  # noqa: E501
+            ignore_default_rules (bool): Set to true to ignore default classification rules and exclusively use rules from classification_rules. [optional] if omitted the server will use the default value of False  # noqa: E501
+            uc_component_branch_name (str): branch name for uc component database; e.g. 'develop/22q2'. [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.map_file = map_file
+        self.stack_name = stack_name
+        self.target_part = target_part
+        self.compiler = compiler
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_response.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/symbol.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,289 +1,287 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from code_size_analyzer_client.model.data_record import DataRecord
-    from code_size_analyzer_client.model.summary_record import SummaryRecord
-    globals()['DataRecord'] = DataRecord
-    globals()['SummaryRecord'] = SummaryRecord
-
-
-class MapFileResponse(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'summary': ({str: (SummaryRecord,)},),  # noqa: E501
-            'data': ([DataRecord],),  # noqa: E501
-            'categories': ({str: ([DataRecord],)},),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'summary': 'summary',  # noqa: E501
-        'data': 'data',  # noqa: E501
-        'categories': 'categories',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, summary, data, categories, *args, **kwargs):  # noqa: E501
-        """MapFileResponse - a model defined in OpenAPI
-
-        Args:
-            summary ({str: (SummaryRecord,)}):
-            data ([DataRecord]):
-            categories ({str: ([DataRecord],)}):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.summary = summary
-        self.data = data
-        self.categories = categories
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, summary, data, categories, *args, **kwargs):  # noqa: E501
-        """MapFileResponse - a model defined in OpenAPI
-
-        Args:
-            summary ({str: (SummaryRecord,)}):
-            data ([DataRecord]):
-            categories ({str: ([DataRecord],)}):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.summary = summary
-        self.data = data
-        self.categories = categories
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+
+class Symbol(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'flash_size': (int,),  # noqa: E501
+            'ram_size': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'address': (int,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'flash_size': 'flash_size',  # noqa: E501
+        'ram_size': 'ram_size',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'address': 'address',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, flash_size, ram_size, name, address, *args, **kwargs):  # noqa: E501
+        """Symbol - a model defined in OpenAPI
+
+        Args:
+            flash_size (int):
+            ram_size (int):
+            name (str):
+            address (int):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.flash_size = flash_size
+        self.ram_size = ram_size
+        self.name = name
+        self.address = address
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, flash_size, ram_size, name, address, *args, **kwargs):  # noqa: E501
+        """Symbol - a model defined in OpenAPI
+
+        Args:
+            flash_size (int):
+            ram_size (int):
+            name (str):
+            address (int):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.flash_size = flash_size
+        self.ram_size = ram_size
+        self.name = name
+        self.address = address
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_section.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/map_file_section.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,281 +1,281 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-
-class MapFileSection(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'name': (str,),  # noqa: E501
-            'start_address': (int,),  # noqa: E501
-            'size': (int,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'name': 'name',  # noqa: E501
-        'start_address': 'start_address',  # noqa: E501
-        'size': 'size',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, start_address, size, *args, **kwargs):  # noqa: E501
-        """MapFileSection - a model defined in OpenAPI
-
-        Args:
-            name (str):
-            start_address (int):
-            size (int):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.name = name
-        self.start_address = start_address
-        self.size = size
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, name, start_address, size, *args, **kwargs):  # noqa: E501
-        """MapFileSection - a model defined in OpenAPI
-
-        Args:
-            name (str):
-            start_address (int):
-            size (int):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.name = name
-        self.start_address = start_address
-        self.size = size
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+
+class MapFileSection(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'name': (str,),  # noqa: E501
+            'start_address': (int,),  # noqa: E501
+            'size': (int,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'name': 'name',  # noqa: E501
+        'start_address': 'start_address',  # noqa: E501
+        'size': 'size',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, name, start_address, size, *args, **kwargs):  # noqa: E501
+        """MapFileSection - a model defined in OpenAPI
+
+        Args:
+            name (str):
+            start_address (int):
+            size (int):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.name = name
+        self.start_address = start_address
+        self.size = size
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, name, start_address, size, *args, **kwargs):  # noqa: E501
+        """MapFileSection - a model defined in OpenAPI
+
+        Args:
+            name (str):
+            start_address (int):
+            size (int):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.name = name
+        self.start_address = start_address
+        self.size = size
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/map_file_summary.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/module_group.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,287 +1,293 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from code_size_analyzer_client.model.module_group import ModuleGroup
-    globals()['ModuleGroup'] = ModuleGroup
-
-
-class MapFileSummary(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'flash_size': (int,),  # noqa: E501
-            'ram_size': (int,),  # noqa: E501
-            'module_groups': ([ModuleGroup],),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'flash_size': 'flash_size',  # noqa: E501
-        'ram_size': 'ram_size',  # noqa: E501
-        'module_groups': 'module_groups',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, flash_size, ram_size, module_groups, *args, **kwargs):  # noqa: E501
-        """MapFileSummary - a model defined in OpenAPI
-
-        Args:
-            flash_size (int):
-            ram_size (int):
-            module_groups ([ModuleGroup]):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.flash_size = flash_size
-        self.ram_size = ram_size
-        self.module_groups = module_groups
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, flash_size, ram_size, module_groups, *args, **kwargs):  # noqa: E501
-        """MapFileSummary - a model defined in OpenAPI
-
-        Args:
-            flash_size (int):
-            ram_size (int):
-            module_groups ([ModuleGroup]):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.flash_size = flash_size
-        self.ram_size = ram_size
-        self.module_groups = module_groups
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from code_size_analyzer_client.model.module import Module
+    globals()['Module'] = Module
+
+
+class ModuleGroup(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'flash_size': (int,),  # noqa: E501
+            'ram_size': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'modules': ([Module],),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'flash_size': 'flash_size',  # noqa: E501
+        'ram_size': 'ram_size',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'modules': 'modules',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, flash_size, ram_size, name, modules, *args, **kwargs):  # noqa: E501
+        """ModuleGroup - a model defined in OpenAPI
+
+        Args:
+            flash_size (int):
+            ram_size (int):
+            name (str):
+            modules ([Module]):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.flash_size = flash_size
+        self.ram_size = ram_size
+        self.name = name
+        self.modules = modules
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, flash_size, ram_size, name, modules, *args, **kwargs):  # noqa: E501
+        """ModuleGroup - a model defined in OpenAPI
+
+        Args:
+            flash_size (int):
+            ram_size (int):
+            name (str):
+            modules ([Module]):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.flash_size = flash_size
+        self.ram_size = ram_size
+        self.name = name
+        self.modules = modules
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/module.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/map_file_summary.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,293 +1,287 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from code_size_analyzer_client.model.symbol import Symbol
-    globals()['Symbol'] = Symbol
-
-
-class Module(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'flash_size': (int,),  # noqa: E501
-            'ram_size': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'symbols': ([Symbol],),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'flash_size': 'flash_size',  # noqa: E501
-        'ram_size': 'ram_size',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'symbols': 'symbols',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, flash_size, ram_size, name, symbols, *args, **kwargs):  # noqa: E501
-        """Module - a model defined in OpenAPI
-
-        Args:
-            flash_size (int):
-            ram_size (int):
-            name (str):
-            symbols ([Symbol]):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.flash_size = flash_size
-        self.ram_size = ram_size
-        self.name = name
-        self.symbols = symbols
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, flash_size, ram_size, name, symbols, *args, **kwargs):  # noqa: E501
-        """Module - a model defined in OpenAPI
-
-        Args:
-            flash_size (int):
-            ram_size (int):
-            name (str):
-            symbols ([Symbol]):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.flash_size = flash_size
-        self.ram_size = ram_size
-        self.name = name
-        self.symbols = symbols
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from code_size_analyzer_client.model.module_group import ModuleGroup
+    globals()['ModuleGroup'] = ModuleGroup
+
+
+class MapFileSummary(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'flash_size': (int,),  # noqa: E501
+            'ram_size': (int,),  # noqa: E501
+            'module_groups': ([ModuleGroup],),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'flash_size': 'flash_size',  # noqa: E501
+        'ram_size': 'ram_size',  # noqa: E501
+        'module_groups': 'module_groups',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, flash_size, ram_size, module_groups, *args, **kwargs):  # noqa: E501
+        """MapFileSummary - a model defined in OpenAPI
+
+        Args:
+            flash_size (int):
+            ram_size (int):
+            module_groups ([ModuleGroup]):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.flash_size = flash_size
+        self.ram_size = ram_size
+        self.module_groups = module_groups
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, flash_size, ram_size, module_groups, *args, **kwargs):  # noqa: E501
+        """MapFileSummary - a model defined in OpenAPI
+
+        Args:
+            flash_size (int):
+            ram_size (int):
+            module_groups ([ModuleGroup]):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.flash_size = flash_size
+        self.ram_size = ram_size
+        self.module_groups = module_groups
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/module_group.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/application_combination.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,293 +1,293 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from code_size_analyzer_client.model.module import Module
-    globals()['Module'] = Module
-
-
-class ModuleGroup(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'flash_size': (int,),  # noqa: E501
-            'ram_size': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'modules': ([Module],),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'flash_size': 'flash_size',  # noqa: E501
-        'ram_size': 'ram_size',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'modules': 'modules',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, flash_size, ram_size, name, modules, *args, **kwargs):  # noqa: E501
-        """ModuleGroup - a model defined in OpenAPI
-
-        Args:
-            flash_size (int):
-            ram_size (int):
-            name (str):
-            modules ([Module]):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.flash_size = flash_size
-        self.ram_size = ram_size
-        self.name = name
-        self.modules = modules
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, flash_size, ram_size, name, modules, *args, **kwargs):  # noqa: E501
-        """ModuleGroup - a model defined in OpenAPI
-
-        Args:
-            flash_size (int):
-            ram_size (int):
-            name (str):
-            modules ([Module]):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.flash_size = flash_size
-        self.ram_size = ram_size
-        self.name = name
-        self.modules = modules
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+
+class ApplicationCombination(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'application_name': (str,),  # noqa: E501
+            'stack': (str,),  # noqa: E501
+            'compiler': (str,),  # noqa: E501
+            'target': (str,),  # noqa: E501
+            'board': (str,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'application_name': 'application_name',  # noqa: E501
+        'stack': 'stack',  # noqa: E501
+        'compiler': 'compiler',  # noqa: E501
+        'target': 'target',  # noqa: E501
+        'board': 'board',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, application_name, stack, compiler, target, board, *args, **kwargs):  # noqa: E501
+        """ApplicationCombination - a model defined in OpenAPI
+
+        Args:
+            application_name (str):
+            stack (str):
+            compiler (str):
+            target (str):
+            board (str):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.application_name = application_name
+        self.stack = stack
+        self.compiler = compiler
+        self.target = target
+        self.board = board
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, application_name, stack, compiler, target, board, *args, **kwargs):  # noqa: E501
+        """ApplicationCombination - a model defined in OpenAPI
+
+        Args:
+            application_name (str):
+            stack (str):
+            compiler (str):
+            target (str):
+            board (str):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.application_name = application_name
+        self.stack = stack
+        self.compiler = compiler
+        self.target = target
+        self.board = board
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/summary_record.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/validation_error.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,267 +1,281 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-
-class SummaryRecord(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'code_size': (int,),  # noqa: E501
-            'ram_size': (int,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'code_size': 'code_size',  # noqa: E501
-        'ram_size': 'RAM_size',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SummaryRecord - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            code_size (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
-            ram_size (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """SummaryRecord - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            code_size (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
-            ram_size (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+
+class ValidationError(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'loc': ([str],),  # noqa: E501
+            'msg': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'loc': 'loc',  # noqa: E501
+        'msg': 'msg',  # noqa: E501
+        'type': 'type',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, loc, msg, type, *args, **kwargs):  # noqa: E501
+        """ValidationError - a model defined in OpenAPI
+
+        Args:
+            loc ([str]):
+            msg (str):
+            type (str):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.loc = loc
+        self.msg = msg
+        self.type = type
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, loc, msg, type, *args, **kwargs):  # noqa: E501
+        """ValidationError - a model defined in OpenAPI
+
+        Args:
+            loc ([str]):
+            msg (str):
+            type (str):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.loc = loc
+        self.msg = msg
+        self.type = type
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/symbol.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/summary_record.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,287 +1,267 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-
-class Symbol(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'flash_size': (int,),  # noqa: E501
-            'ram_size': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'address': (int,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'flash_size': 'flash_size',  # noqa: E501
-        'ram_size': 'ram_size',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'address': 'address',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, flash_size, ram_size, name, address, *args, **kwargs):  # noqa: E501
-        """Symbol - a model defined in OpenAPI
-
-        Args:
-            flash_size (int):
-            ram_size (int):
-            name (str):
-            address (int):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.flash_size = flash_size
-        self.ram_size = ram_size
-        self.name = name
-        self.address = address
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, flash_size, ram_size, name, address, *args, **kwargs):  # noqa: E501
-        """Symbol - a model defined in OpenAPI
-
-        Args:
-            flash_size (int):
-            ram_size (int):
-            name (str):
-            address (int):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.flash_size = flash_size
-        self.ram_size = ram_size
-        self.name = name
-        self.address = address
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+
+class SummaryRecord(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'code_size': (int,),  # noqa: E501
+            'ram_size': (int,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'code_size': 'code_size',  # noqa: E501
+        'ram_size': 'RAM_size',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """SummaryRecord - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            code_size (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+            ram_size (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """SummaryRecord - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            code_size (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+            ram_size (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model/target_info.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model/target_info.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,287 +1,293 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from code_size_analyzer_client.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from code_size_analyzer_client.exceptions import ApiAttributeError
-
-
-
-class TargetInfo(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'board': (str,),  # noqa: E501
-            'code_size_bytes': (int,),  # noqa: E501
-            'device': (str,),  # noqa: E501
-            'ram_size_bytes': (int,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'board': 'board',  # noqa: E501
-        'code_size_bytes': 'codeSizeBytes',  # noqa: E501
-        'device': 'device',  # noqa: E501
-        'ram_size_bytes': 'ramSizeBytes',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, board, code_size_bytes, device, ram_size_bytes, *args, **kwargs):  # noqa: E501
-        """TargetInfo - a model defined in OpenAPI
-
-        Args:
-            board (str):
-            code_size_bytes (int):
-            device (str):
-            ram_size_bytes (int):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.board = board
-        self.code_size_bytes = code_size_bytes
-        self.device = device
-        self.ram_size_bytes = ram_size_bytes
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, board, code_size_bytes, device, ram_size_bytes, *args, **kwargs):  # noqa: E501
-        """TargetInfo - a model defined in OpenAPI
-
-        Args:
-            board (str):
-            code_size_bytes (int):
-            device (str):
-            ram_size_bytes (int):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.board = board
-        self.code_size_bytes = code_size_bytes
-        self.device = device
-        self.ram_size_bytes = ram_size_bytes
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from code_size_analyzer_client.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from code_size_analyzer_client.exceptions import ApiAttributeError
+
+
+
+class TargetInfo(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'board': (str,),  # noqa: E501
+            'code_size_bytes': (int,),  # noqa: E501
+            'device': (str,),  # noqa: E501
+            'ram_size_bytes': (int,),  # noqa: E501
+            'family': (str,),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'board': 'board',  # noqa: E501
+        'code_size_bytes': 'codeSizeBytes',  # noqa: E501
+        'device': 'device',  # noqa: E501
+        'ram_size_bytes': 'ramSizeBytes',  # noqa: E501
+        'family': 'family',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, board, code_size_bytes, device, ram_size_bytes, family, *args, **kwargs):  # noqa: E501
+        """TargetInfo - a model defined in OpenAPI
+
+        Args:
+            board (str):
+            code_size_bytes (int):
+            device (str):
+            ram_size_bytes (int):
+            family (str):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.board = board
+        self.code_size_bytes = code_size_bytes
+        self.device = device
+        self.ram_size_bytes = ram_size_bytes
+        self.family = family
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, board, code_size_bytes, device, ram_size_bytes, family, *args, **kwargs):  # noqa: E501
+        """TargetInfo - a model defined in OpenAPI
+
+        Args:
+            board (str):
+            code_size_bytes (int):
+            device (str):
+            ram_size_bytes (int):
+            family (str):
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        self.board = board
+        self.code_size_bytes = code_size_bytes
+        self.device = device
+        self.ram_size_bytes = ram_size_bytes
+        self.family = family
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/model_utils.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/model_utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,2056 +1,2056 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-from datetime import date, datetime  # noqa: F401
-from copy import deepcopy
-import inspect
-import io
-import os
-import pprint
-import re
-import tempfile
-import uuid
-
-from dateutil.parser import parse
-
-from code_size_analyzer_client.exceptions import (
-    ApiKeyError,
-    ApiAttributeError,
-    ApiTypeError,
-    ApiValueError,
-)
-
-none_type = type(None)
-file_type = io.IOBase
-
-
-def convert_js_args_to_python_args(fn):
-    from functools import wraps
-    @wraps(fn)
-    def wrapped_init(_self, *args, **kwargs):
-        """
-        An attribute named `self` received from the api will conflicts with the reserved `self`
-        parameter of a class method. During generation, `self` attributes are mapped
-        to `_self` in models. Here, we name `_self` instead of `self` to avoid conflicts.
-        """
-        spec_property_naming = kwargs.get('_spec_property_naming', False)
-        if spec_property_naming:
-            kwargs = change_keys_js_to_python(
-                kwargs, _self if isinstance(
-                    _self, type) else _self.__class__)
-        return fn(_self, *args, **kwargs)
-    return wrapped_init
-
-
-class cached_property(object):
-    # this caches the result of the function call for fn with no inputs
-    # use this as a decorator on function methods that you want converted
-    # into cached properties
-    result_key = '_results'
-
-    def __init__(self, fn):
-        self._fn = fn
-
-    def __get__(self, instance, cls=None):
-        if self.result_key in vars(self):
-            return vars(self)[self.result_key]
-        else:
-            result = self._fn()
-            setattr(self, self.result_key, result)
-            return result
-
-
-PRIMITIVE_TYPES = (list, float, int, bool, datetime, date, str, file_type)
-
-
-def allows_single_value_input(cls):
-    """
-    This function returns True if the input composed schema model or any
-    descendant model allows a value only input
-    This is true for cases where oneOf contains items like:
-    oneOf:
-      - float
-      - NumberWithValidation
-      - StringEnum
-      - ArrayModel
-      - null
-    TODO: lru_cache this
-    """
-    if (
-        issubclass(cls, ModelSimple) or
-        cls in PRIMITIVE_TYPES
-    ):
-        return True
-    elif issubclass(cls, ModelComposed):
-        if not cls._composed_schemas['oneOf']:
-            return False
-        return any(allows_single_value_input(c) for c in cls._composed_schemas['oneOf'])
-    return False
-
-
-def composed_model_input_classes(cls):
-    """
-    This function returns a list of the possible models that can be accepted as
-    inputs.
-    TODO: lru_cache this
-    """
-    if issubclass(cls, ModelSimple) or cls in PRIMITIVE_TYPES:
-        return [cls]
-    elif issubclass(cls, ModelNormal):
-        if cls.discriminator is None:
-            return [cls]
-        else:
-            return get_discriminated_classes(cls)
-    elif issubclass(cls, ModelComposed):
-        if not cls._composed_schemas['oneOf']:
-            return []
-        if cls.discriminator is None:
-            input_classes = []
-            for c in cls._composed_schemas['oneOf']:
-                input_classes.extend(composed_model_input_classes(c))
-            return input_classes
-        else:
-            return get_discriminated_classes(cls)
-    return []
-
-
-class OpenApiModel(object):
-    """The base class for all OpenAPIModels"""
-
-    def set_attribute(self, name, value):
-        # this is only used to set properties on self
-
-        path_to_item = []
-        if self._path_to_item:
-            path_to_item.extend(self._path_to_item)
-        path_to_item.append(name)
-
-        if name in self.openapi_types:
-            required_types_mixed = self.openapi_types[name]
-        elif self.additional_properties_type is None:
-            raise ApiAttributeError(
-                "{0} has no attribute '{1}'".format(
-                    type(self).__name__, name),
-                path_to_item
-            )
-        elif self.additional_properties_type is not None:
-            required_types_mixed = self.additional_properties_type
-
-        if get_simple_class(name) != str:
-            error_msg = type_error_message(
-                var_name=name,
-                var_value=name,
-                valid_classes=(str,),
-                key_type=True
-            )
-            raise ApiTypeError(
-                error_msg,
-                path_to_item=path_to_item,
-                valid_classes=(str,),
-                key_type=True
-            )
-
-        if self._check_type:
-            value = validate_and_convert_types(
-                value, required_types_mixed, path_to_item, self._spec_property_naming,
-                self._check_type, configuration=self._configuration)
-        if (name,) in self.allowed_values:
-            check_allowed_values(
-                self.allowed_values,
-                (name,),
-                value
-            )
-        if (name,) in self.validations:
-            check_validations(
-                self.validations,
-                (name,),
-                value,
-                self._configuration
-            )
-        self.__dict__['_data_store'][name] = value
-
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
-
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        return not self == other
-
-    def __setattr__(self, attr, value):
-        """set the value of an attribute using dot notation: `instance.attr = val`"""
-        self[attr] = value
-
-    def __getattr__(self, attr):
-        """get the value of an attribute using dot notation: `instance.attr`"""
-        return self.__getitem__(attr)
-
-    def __copy__(self):
-        cls = self.__class__
-        if self.get("_spec_property_naming", False):
-            return cls._new_from_openapi_data(**self.__dict__)
-        else:
-            return cls.__new__(cls, **self.__dict__)
-
-    def __deepcopy__(self, memo):
-        cls = self.__class__
-
-        if self.get("_spec_property_naming", False):
-            new_inst = cls._new_from_openapi_data()
-        else:
-            new_inst = cls.__new__(cls)
-
-        for k, v in self.__dict__.items():
-            setattr(new_inst, k, deepcopy(v, memo))
-        return new_inst
-
-
-    def __new__(cls, *args, **kwargs):
-        # this function uses the discriminator to
-        # pick a new schema/class to instantiate because a discriminator
-        # propertyName value was passed in
-
-        if len(args) == 1:
-            arg = args[0]
-            if arg is None and is_type_nullable(cls):
-                # The input data is the 'null' value and the type is nullable.
-                return None
-
-            if issubclass(cls, ModelComposed) and allows_single_value_input(cls):
-                model_kwargs = {}
-                oneof_instance = get_oneof_instance(cls, model_kwargs, kwargs, model_arg=arg)
-                return oneof_instance
-
-        visited_composed_classes = kwargs.get('_visited_composed_classes', ())
-        if (
-            cls.discriminator is None or
-            cls in visited_composed_classes
-        ):
-            # Use case 1: this openapi schema (cls) does not have a discriminator
-            # Use case 2: we have already visited this class before and are sure that we
-            # want to instantiate it this time. We have visited this class deserializing
-            # a payload with a discriminator. During that process we traveled through
-            # this class but did not make an instance of it. Now we are making an
-            # instance of a composed class which contains cls in it, so this time make an instance of cls.
-            #
-            # Here's an example of use case 2: If Animal has a discriminator
-            # petType and we pass in "Dog", and the class Dog
-            # allOf includes Animal, we move through Animal
-            # once using the discriminator, and pick Dog.
-            # Then in the composed schema dog Dog, we will make an instance of the
-            # Animal class (because Dal has allOf: Animal) but this time we won't travel
-            # through Animal's discriminator because we passed in
-            # _visited_composed_classes = (Animal,)
-
-            return super(OpenApiModel, cls).__new__(cls)
-
-        # Get the name and value of the discriminator property.
-        # The discriminator name is obtained from the discriminator meta-data
-        # and the discriminator value is obtained from the input data.
-        discr_propertyname_py = list(cls.discriminator.keys())[0]
-        discr_propertyname_js = cls.attribute_map[discr_propertyname_py]
-        if discr_propertyname_js in kwargs:
-            discr_value = kwargs[discr_propertyname_js]
-        elif discr_propertyname_py in kwargs:
-            discr_value = kwargs[discr_propertyname_py]
-        else:
-            # The input data does not contain the discriminator property.
-            path_to_item = kwargs.get('_path_to_item', ())
-            raise ApiValueError(
-                "Cannot deserialize input data due to missing discriminator. "
-                "The discriminator property '%s' is missing at path: %s" %
-                (discr_propertyname_js, path_to_item)
-            )
-
-        # Implementation note: the last argument to get_discriminator_class
-        # is a list of visited classes. get_discriminator_class may recursively
-        # call itself and update the list of visited classes, and the initial
-        # value must be an empty list. Hence not using 'visited_composed_classes'
-        new_cls = get_discriminator_class(
-            cls, discr_propertyname_py, discr_value, [])
-        if new_cls is None:
-            path_to_item = kwargs.get('_path_to_item', ())
-            disc_prop_value = kwargs.get(
-                discr_propertyname_js, kwargs.get(discr_propertyname_py))
-            raise ApiValueError(
-                "Cannot deserialize input data due to invalid discriminator "
-                "value. The OpenAPI document has no mapping for discriminator "
-                "property '%s'='%s' at path: %s" %
-                (discr_propertyname_js, disc_prop_value, path_to_item)
-            )
-
-        if new_cls in visited_composed_classes:
-            # if we are making an instance of a composed schema Descendent
-            # which allOf includes Ancestor, then Ancestor contains
-            # a discriminator that includes Descendent.
-            # So if we make an instance of Descendent, we have to make an
-            # instance of Ancestor to hold the allOf properties.
-            # This code detects that use case and makes the instance of Ancestor
-            # For example:
-            # When making an instance of Dog, _visited_composed_classes = (Dog,)
-            # then we make an instance of Animal to include in dog._composed_instances
-            # so when we are here, cls is Animal
-            # cls.discriminator != None
-            # cls not in _visited_composed_classes
-            # new_cls = Dog
-            # but we know we know that we already have Dog
-            # because it is in visited_composed_classes
-            # so make Animal here
-            return super(OpenApiModel, cls).__new__(cls)
-
-        # Build a list containing all oneOf and anyOf descendants.
-        oneof_anyof_classes = None
-        if cls._composed_schemas is not None:
-            oneof_anyof_classes = (
-                cls._composed_schemas.get('oneOf', ()) +
-                cls._composed_schemas.get('anyOf', ()))
-        oneof_anyof_child = new_cls in oneof_anyof_classes
-        kwargs['_visited_composed_classes'] = visited_composed_classes + (cls,)
-
-        if cls._composed_schemas.get('allOf') and oneof_anyof_child:
-            # Validate that we can make self because when we make the
-            # new_cls it will not include the allOf validations in self
-            self_inst = super(OpenApiModel, cls).__new__(cls)
-            self_inst.__init__(*args, **kwargs)
-
-        if kwargs.get("_spec_property_naming", False):
-            # when true, implies new is from deserialization
-            new_inst = new_cls._new_from_openapi_data(*args, **kwargs)
-        else:
-            new_inst = new_cls.__new__(new_cls, *args, **kwargs)
-            new_inst.__init__(*args, **kwargs)
-
-        return new_inst
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _new_from_openapi_data(cls, *args, **kwargs):
-        # this function uses the discriminator to
-        # pick a new schema/class to instantiate because a discriminator
-        # propertyName value was passed in
-
-        if len(args) == 1:
-            arg = args[0]
-            if arg is None and is_type_nullable(cls):
-                # The input data is the 'null' value and the type is nullable.
-                return None
-
-            if issubclass(cls, ModelComposed) and allows_single_value_input(cls):
-                model_kwargs = {}
-                oneof_instance = get_oneof_instance(cls, model_kwargs, kwargs, model_arg=arg)
-                return oneof_instance
-
-        visited_composed_classes = kwargs.get('_visited_composed_classes', ())
-        if (
-            cls.discriminator is None or
-            cls in visited_composed_classes
-        ):
-            # Use case 1: this openapi schema (cls) does not have a discriminator
-            # Use case 2: we have already visited this class before and are sure that we
-            # want to instantiate it this time. We have visited this class deserializing
-            # a payload with a discriminator. During that process we traveled through
-            # this class but did not make an instance of it. Now we are making an
-            # instance of a composed class which contains cls in it, so this time make an instance of cls.
-            #
-            # Here's an example of use case 2: If Animal has a discriminator
-            # petType and we pass in "Dog", and the class Dog
-            # allOf includes Animal, we move through Animal
-            # once using the discriminator, and pick Dog.
-            # Then in the composed schema dog Dog, we will make an instance of the
-            # Animal class (because Dal has allOf: Animal) but this time we won't travel
-            # through Animal's discriminator because we passed in
-            # _visited_composed_classes = (Animal,)
-
-            return cls._from_openapi_data(*args, **kwargs)
-
-        # Get the name and value of the discriminator property.
-        # The discriminator name is obtained from the discriminator meta-data
-        # and the discriminator value is obtained from the input data.
-        discr_propertyname_py = list(cls.discriminator.keys())[0]
-        discr_propertyname_js = cls.attribute_map[discr_propertyname_py]
-        if discr_propertyname_js in kwargs:
-            discr_value = kwargs[discr_propertyname_js]
-        elif discr_propertyname_py in kwargs:
-            discr_value = kwargs[discr_propertyname_py]
-        else:
-            # The input data does not contain the discriminator property.
-            path_to_item = kwargs.get('_path_to_item', ())
-            raise ApiValueError(
-                "Cannot deserialize input data due to missing discriminator. "
-                "The discriminator property '%s' is missing at path: %s" %
-                (discr_propertyname_js, path_to_item)
-            )
-
-        # Implementation note: the last argument to get_discriminator_class
-        # is a list of visited classes. get_discriminator_class may recursively
-        # call itself and update the list of visited classes, and the initial
-        # value must be an empty list. Hence not using 'visited_composed_classes'
-        new_cls = get_discriminator_class(
-            cls, discr_propertyname_py, discr_value, [])
-        if new_cls is None:
-            path_to_item = kwargs.get('_path_to_item', ())
-            disc_prop_value = kwargs.get(
-                discr_propertyname_js, kwargs.get(discr_propertyname_py))
-            raise ApiValueError(
-                "Cannot deserialize input data due to invalid discriminator "
-                "value. The OpenAPI document has no mapping for discriminator "
-                "property '%s'='%s' at path: %s" %
-                (discr_propertyname_js, disc_prop_value, path_to_item)
-            )
-
-        if new_cls in visited_composed_classes:
-            # if we are making an instance of a composed schema Descendent
-            # which allOf includes Ancestor, then Ancestor contains
-            # a discriminator that includes Descendent.
-            # So if we make an instance of Descendent, we have to make an
-            # instance of Ancestor to hold the allOf properties.
-            # This code detects that use case and makes the instance of Ancestor
-            # For example:
-            # When making an instance of Dog, _visited_composed_classes = (Dog,)
-            # then we make an instance of Animal to include in dog._composed_instances
-            # so when we are here, cls is Animal
-            # cls.discriminator != None
-            # cls not in _visited_composed_classes
-            # new_cls = Dog
-            # but we know we know that we already have Dog
-            # because it is in visited_composed_classes
-            # so make Animal here
-            return cls._from_openapi_data(*args, **kwargs)
-
-        # Build a list containing all oneOf and anyOf descendants.
-        oneof_anyof_classes = None
-        if cls._composed_schemas is not None:
-            oneof_anyof_classes = (
-                cls._composed_schemas.get('oneOf', ()) +
-                cls._composed_schemas.get('anyOf', ()))
-        oneof_anyof_child = new_cls in oneof_anyof_classes
-        kwargs['_visited_composed_classes'] = visited_composed_classes + (cls,)
-
-        if cls._composed_schemas.get('allOf') and oneof_anyof_child:
-            # Validate that we can make self because when we make the
-            # new_cls it will not include the allOf validations in self
-            self_inst = cls._from_openapi_data(*args, **kwargs)
-
-        new_inst = new_cls._new_from_openapi_data(*args, **kwargs)
-        return new_inst
-
-
-class ModelSimple(OpenApiModel):
-    """the parent class of models whose type != object in their
-    swagger/openapi"""
-
-    def __setitem__(self, name, value):
-        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
-        if name in self.required_properties:
-            self.__dict__[name] = value
-            return
-
-        self.set_attribute(name, value)
-
-    def get(self, name, default=None):
-        """returns the value of an attribute or some default value if the attribute was not set"""
-        if name in self.required_properties:
-            return self.__dict__[name]
-
-        return self.__dict__['_data_store'].get(name, default)
-
-    def __getitem__(self, name):
-        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
-        if name in self:
-            return self.get(name)
-
-        raise ApiAttributeError(
-            "{0} has no attribute '{1}'".format(
-                type(self).__name__, name),
-            [e for e in [self._path_to_item, name] if e]
-        )
-
-    def __contains__(self, name):
-        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
-        if name in self.required_properties:
-            return name in self.__dict__
-
-        return name in self.__dict__['_data_store']
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return str(self.value)
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, self.__class__):
-            return False
-
-        this_val = self._data_store['value']
-        that_val = other._data_store['value']
-        types = set()
-        types.add(this_val.__class__)
-        types.add(that_val.__class__)
-        vals_equal = this_val == that_val
-        return vals_equal
-
-
-class ModelNormal(OpenApiModel):
-    """the parent class of models whose type == object in their
-    swagger/openapi"""
-
-    def __setitem__(self, name, value):
-        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
-        if name in self.required_properties:
-            self.__dict__[name] = value
-            return
-
-        self.set_attribute(name, value)
-
-    def get(self, name, default=None):
-        """returns the value of an attribute or some default value if the attribute was not set"""
-        if name in self.required_properties:
-            return self.__dict__[name]
-
-        return self.__dict__['_data_store'].get(name, default)
-
-    def __getitem__(self, name):
-        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
-        if name in self:
-            return self.get(name)
-
-        raise ApiAttributeError(
-            "{0} has no attribute '{1}'".format(
-                type(self).__name__, name),
-            [e for e in [self._path_to_item, name] if e]
-        )
-
-    def __contains__(self, name):
-        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
-        if name in self.required_properties:
-            return name in self.__dict__
-
-        return name in self.__dict__['_data_store']
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        return model_to_dict(self, serialize=False)
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, self.__class__):
-            return False
-
-        if not set(self._data_store.keys()) == set(other._data_store.keys()):
-            return False
-        for _var_name, this_val in self._data_store.items():
-            that_val = other._data_store[_var_name]
-            types = set()
-            types.add(this_val.__class__)
-            types.add(that_val.__class__)
-            vals_equal = this_val == that_val
-            if not vals_equal:
-                return False
-        return True
-
-
-class ModelComposed(OpenApiModel):
-    """the parent class of models whose type == object in their
-    swagger/openapi and have oneOf/allOf/anyOf
-
-    When one sets a property we use var_name_to_model_instances to store the value in
-    the correct class instances + run any type checking + validation code.
-    When one gets a property we use var_name_to_model_instances to get the value
-    from the correct class instances.
-    This allows multiple composed schemas to contain the same property with additive
-    constraints on the value.
-
-    _composed_schemas (dict) stores the anyOf/allOf/oneOf classes
-    key (str): allOf/oneOf/anyOf
-    value (list): the classes in the XOf definition.
-        Note: none_type can be included when the openapi document version >= 3.1.0
-    _composed_instances (list): stores a list of instances of the composed schemas
-    defined in _composed_schemas. When properties are accessed in the self instance,
-    they are returned from the self._data_store or the data stores in the instances
-    in self._composed_schemas
-    _var_name_to_model_instances (dict): maps between a variable name on self and
-    the composed instances (self included) which contain that data
-    key (str): property name
-    value (list): list of class instances, self or instances in _composed_instances
-    which contain the value that the key is referring to.
-    """
-
-    def __setitem__(self, name, value):
-        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
-        if name in self.required_properties:
-            self.__dict__[name] = value
-            return
-
-        """
-        Use cases:
-        1. additional_properties_type is None (additionalProperties == False in spec)
-            Check for property presence in self.openapi_types
-            if not present then throw an error
-            if present set in self, set attribute
-            always set on composed schemas
-        2.  additional_properties_type exists
-            set attribute on self
-            always set on composed schemas
-        """
-        if self.additional_properties_type is None:
-            """
-            For an attribute to exist on a composed schema it must:
-            - fulfill schema_requirements in the self composed schema not considering oneOf/anyOf/allOf schemas AND
-            - fulfill schema_requirements in each oneOf/anyOf/allOf schemas
-
-            schema_requirements:
-            For an attribute to exist on a schema it must:
-            - be present in properties at the schema OR
-            - have additionalProperties unset (defaults additionalProperties = any type) OR
-            - have additionalProperties set
-            """
-            if name not in self.openapi_types:
-                raise ApiAttributeError(
-                    "{0} has no attribute '{1}'".format(
-                        type(self).__name__, name),
-                    [e for e in [self._path_to_item, name] if e]
-                )
-        # attribute must be set on self and composed instances
-        self.set_attribute(name, value)
-        for model_instance in self._composed_instances:
-            setattr(model_instance, name, value)
-        if name not in self._var_name_to_model_instances:
-            # we assigned an additional property
-            self.__dict__['_var_name_to_model_instances'][name] = self._composed_instances + [self]
-        return None
-
-    __unset_attribute_value__ = object()
-
-    def get(self, name, default=None):
-        """returns the value of an attribute or some default value if the attribute was not set"""
-        if name in self.required_properties:
-            return self.__dict__[name]
-
-        # get the attribute from the correct instance
-        model_instances = self._var_name_to_model_instances.get(name)
-        values = []
-        # A composed model stores self and child (oneof/anyOf/allOf) models under
-        # self._var_name_to_model_instances.
-        # Any property must exist in self and all model instances
-        # The value stored in all model instances must be the same
-        if model_instances:
-            for model_instance in model_instances:
-                if name in model_instance._data_store:
-                    v = model_instance._data_store[name]
-                    if v not in values:
-                        values.append(v)
-        len_values = len(values)
-        if len_values == 0:
-            return default
-        elif len_values == 1:
-            return values[0]
-        elif len_values > 1:
-            raise ApiValueError(
-                "Values stored for property {0} in {1} differ when looking "
-                "at self and self's composed instances. All values must be "
-                "the same".format(name, type(self).__name__),
-                [e for e in [self._path_to_item, name] if e]
-            )
-
-    def __getitem__(self, name):
-        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
-        value = self.get(name, self.__unset_attribute_value__)
-        if value is self.__unset_attribute_value__:
-            raise ApiAttributeError(
-                "{0} has no attribute '{1}'".format(
-                    type(self).__name__, name),
-                    [e for e in [self._path_to_item, name] if e]
-            )
-        return value
-
-    def __contains__(self, name):
-        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
-
-        if name in self.required_properties:
-            return name in self.__dict__
-
-        model_instances = self._var_name_to_model_instances.get(
-            name, self._additional_properties_model_instances)
-
-        if model_instances:
-            for model_instance in model_instances:
-                if name in model_instance._data_store:
-                    return True
-
-        return False
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        return model_to_dict(self, serialize=False)
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, self.__class__):
-            return False
-
-        if not set(self._data_store.keys()) == set(other._data_store.keys()):
-            return False
-        for _var_name, this_val in self._data_store.items():
-            that_val = other._data_store[_var_name]
-            types = set()
-            types.add(this_val.__class__)
-            types.add(that_val.__class__)
-            vals_equal = this_val == that_val
-            if not vals_equal:
-                return False
-        return True
-
-
-COERCION_INDEX_BY_TYPE = {
-    ModelComposed: 0,
-    ModelNormal: 1,
-    ModelSimple: 2,
-    none_type: 3,    # The type of 'None'.
-    list: 4,
-    dict: 5,
-    float: 6,
-    int: 7,
-    bool: 8,
-    datetime: 9,
-    date: 10,
-    str: 11,
-    file_type: 12,   # 'file_type' is an alias for the built-in 'file' or 'io.IOBase' type.
-}
-
-# these are used to limit what type conversions we try to do
-# when we have a valid type already and we want to try converting
-# to another type
-UPCONVERSION_TYPE_PAIRS = (
-    (str, datetime),
-    (str, date),
-    # A float may be serialized as an integer, e.g. '3' is a valid serialized float.
-    (int, float),
-    (list, ModelComposed),
-    (dict, ModelComposed),
-    (str, ModelComposed),
-    (int, ModelComposed),
-    (float, ModelComposed),
-    (list, ModelComposed),
-    (list, ModelNormal),
-    (dict, ModelNormal),
-    (str, ModelSimple),
-    (int, ModelSimple),
-    (float, ModelSimple),
-    (list, ModelSimple),
-)
-
-COERCIBLE_TYPE_PAIRS = {
-    False: (  # client instantiation of a model with client data
-        # (dict, ModelComposed),
-        # (list, ModelComposed),
-        # (dict, ModelNormal),
-        # (list, ModelNormal),
-        # (str, ModelSimple),
-        # (int, ModelSimple),
-        # (float, ModelSimple),
-        # (list, ModelSimple),
-        # (str, int),
-        # (str, float),
-        # (str, datetime),
-        # (str, date),
-        # (int, str),
-        # (float, str),
-    ),
-    True: (  # server -> client data
-        (dict, ModelComposed),
-        (list, ModelComposed),
-        (dict, ModelNormal),
-        (list, ModelNormal),
-        (str, ModelSimple),
-        (int, ModelSimple),
-        (float, ModelSimple),
-        (list, ModelSimple),
-        # (str, int),
-        # (str, float),
-        (str, datetime),
-        (str, date),
-        # (int, str),
-        # (float, str),
-        (str, file_type)
-    ),
-}
-
-
-def get_simple_class(input_value):
-    """Returns an input_value's simple class that we will use for type checking
-    Python2:
-    float and int will return int, where int is the python3 int backport
-    str and unicode will return str, where str is the python3 str backport
-    Note: float and int ARE both instances of int backport
-    Note: str_py2 and unicode_py2 are NOT both instances of str backport
-
-    Args:
-        input_value (class/class_instance): the item for which we will return
-                                            the simple class
-    """
-    if isinstance(input_value, type):
-        # input_value is a class
-        return input_value
-    elif isinstance(input_value, tuple):
-        return tuple
-    elif isinstance(input_value, list):
-        return list
-    elif isinstance(input_value, dict):
-        return dict
-    elif isinstance(input_value, none_type):
-        return none_type
-    elif isinstance(input_value, file_type):
-        return file_type
-    elif isinstance(input_value, bool):
-        # this must be higher than the int check because
-        # isinstance(True, int) == True
-        return bool
-    elif isinstance(input_value, int):
-        return int
-    elif isinstance(input_value, datetime):
-        # this must be higher than the date check because
-        # isinstance(datetime_instance, date) == True
-        return datetime
-    elif isinstance(input_value, date):
-        return date
-    elif isinstance(input_value, str):
-        return str
-    return type(input_value)
-
-
-def check_allowed_values(allowed_values, input_variable_path, input_values):
-    """Raises an exception if the input_values are not allowed
-
-    Args:
-        allowed_values (dict): the allowed_values dict
-        input_variable_path (tuple): the path to the input variable
-        input_values (list/str/int/float/date/datetime): the values that we
-            are checking to see if they are in allowed_values
-    """
-    these_allowed_values = list(allowed_values[input_variable_path].values())
-    if (isinstance(input_values, list)
-            and not set(input_values).issubset(
-                set(these_allowed_values))):
-        invalid_values = ", ".join(
-            map(str, set(input_values) - set(these_allowed_values))),
-        raise ApiValueError(
-            "Invalid values for `%s` [%s], must be a subset of [%s]" %
-            (
-                input_variable_path[0],
-                invalid_values,
-                ", ".join(map(str, these_allowed_values))
-            )
-        )
-    elif (isinstance(input_values, dict)
-            and not set(
-                input_values.keys()).issubset(set(these_allowed_values))):
-        invalid_values = ", ".join(
-            map(str, set(input_values.keys()) - set(these_allowed_values)))
-        raise ApiValueError(
-            "Invalid keys in `%s` [%s], must be a subset of [%s]" %
-            (
-                input_variable_path[0],
-                invalid_values,
-                ", ".join(map(str, these_allowed_values))
-            )
-        )
-    elif (not isinstance(input_values, (list, dict))
-            and input_values not in these_allowed_values):
-        raise ApiValueError(
-            "Invalid value for `%s` (%s), must be one of %s" %
-            (
-                input_variable_path[0],
-                input_values,
-                these_allowed_values
-            )
-        )
-
-
-def is_json_validation_enabled(schema_keyword, configuration=None):
-    """Returns true if JSON schema validation is enabled for the specified
-    validation keyword. This can be used to skip JSON schema structural validation
-    as requested in the configuration.
-
-    Args:
-        schema_keyword (string): the name of a JSON schema validation keyword.
-        configuration (Configuration): the configuration class.
-    """
-
-    return (configuration is None or
-            not hasattr(configuration, '_disabled_client_side_validations') or
-            schema_keyword not in configuration._disabled_client_side_validations)
-
-
-def check_validations(
-        validations, input_variable_path, input_values,
-        configuration=None):
-    """Raises an exception if the input_values are invalid
-
-    Args:
-        validations (dict): the validation dictionary.
-        input_variable_path (tuple): the path to the input variable.
-        input_values (list/str/int/float/date/datetime): the values that we
-            are checking.
-        configuration (Configuration): the configuration class.
-    """
-
-    if input_values is None:
-        return
-
-    current_validations = validations[input_variable_path]
-    if (is_json_validation_enabled('multipleOf', configuration) and
-            'multiple_of' in current_validations and
-            isinstance(input_values, (int, float)) and
-            not (float(input_values) / current_validations['multiple_of']).is_integer()):
-        # Note 'multipleOf' will be as good as the floating point arithmetic.
-        raise ApiValueError(
-            "Invalid value for `%s`, value must be a multiple of "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['multiple_of']
-            )
-        )
-
-    if (is_json_validation_enabled('maxLength', configuration) and
-            'max_length' in current_validations and
-            len(input_values) > current_validations['max_length']):
-        raise ApiValueError(
-            "Invalid value for `%s`, length must be less than or equal to "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['max_length']
-            )
-        )
-
-    if (is_json_validation_enabled('minLength', configuration) and
-            'min_length' in current_validations and
-            len(input_values) < current_validations['min_length']):
-        raise ApiValueError(
-            "Invalid value for `%s`, length must be greater than or equal to "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['min_length']
-            )
-        )
-
-    if (is_json_validation_enabled('maxItems', configuration) and
-            'max_items' in current_validations and
-            len(input_values) > current_validations['max_items']):
-        raise ApiValueError(
-            "Invalid value for `%s`, number of items must be less than or "
-            "equal to `%s`" % (
-                input_variable_path[0],
-                current_validations['max_items']
-            )
-        )
-
-    if (is_json_validation_enabled('minItems', configuration) and
-            'min_items' in current_validations and
-            len(input_values) < current_validations['min_items']):
-        raise ValueError(
-            "Invalid value for `%s`, number of items must be greater than or "
-            "equal to `%s`" % (
-                input_variable_path[0],
-                current_validations['min_items']
-            )
-        )
-
-    items = ('exclusive_maximum', 'inclusive_maximum', 'exclusive_minimum',
-             'inclusive_minimum')
-    if (any(item in current_validations for item in items)):
-        if isinstance(input_values, list):
-            max_val = max(input_values)
-            min_val = min(input_values)
-        elif isinstance(input_values, dict):
-            max_val = max(input_values.values())
-            min_val = min(input_values.values())
-        else:
-            max_val = input_values
-            min_val = input_values
-
-    if (is_json_validation_enabled('exclusiveMaximum', configuration) and
-            'exclusive_maximum' in current_validations and
-            max_val >= current_validations['exclusive_maximum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value less than `%s`" % (
-                input_variable_path[0],
-                current_validations['exclusive_maximum']
-            )
-        )
-
-    if (is_json_validation_enabled('maximum', configuration) and
-            'inclusive_maximum' in current_validations and
-            max_val > current_validations['inclusive_maximum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value less than or equal to "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['inclusive_maximum']
-            )
-        )
-
-    if (is_json_validation_enabled('exclusiveMinimum', configuration) and
-            'exclusive_minimum' in current_validations and
-            min_val <= current_validations['exclusive_minimum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value greater than `%s`" %
-            (
-                input_variable_path[0],
-                current_validations['exclusive_maximum']
-            )
-        )
-
-    if (is_json_validation_enabled('minimum', configuration) and
-            'inclusive_minimum' in current_validations and
-            min_val < current_validations['inclusive_minimum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value greater than or equal "
-            "to `%s`" % (
-                input_variable_path[0],
-                current_validations['inclusive_minimum']
-            )
-        )
-    flags = current_validations.get('regex', {}).get('flags', 0)
-    if (is_json_validation_enabled('pattern', configuration) and
-            'regex' in current_validations and
-            not re.search(current_validations['regex']['pattern'],
-                          input_values, flags=flags)):
-        err_msg = r"Invalid value for `%s`, must match regular expression `%s`" % (
-            input_variable_path[0],
-            current_validations['regex']['pattern']
-        )
-        if flags != 0:
-            # Don't print the regex flags if the flags are not
-            # specified in the OAS document.
-            err_msg = r"%s with flags=`%s`" % (err_msg, flags)
-        raise ApiValueError(err_msg)
-
-
-def order_response_types(required_types):
-    """Returns the required types sorted in coercion order
-
-    Args:
-        required_types (list/tuple): collection of classes or instance of
-            list or dict with class information inside it.
-
-    Returns:
-        (list): coercion order sorted collection of classes or instance
-            of list or dict with class information inside it.
-    """
-
-    def index_getter(class_or_instance):
-        if isinstance(class_or_instance, list):
-            return COERCION_INDEX_BY_TYPE[list]
-        elif isinstance(class_or_instance, dict):
-            return COERCION_INDEX_BY_TYPE[dict]
-        elif (inspect.isclass(class_or_instance)
-                and issubclass(class_or_instance, ModelComposed)):
-            return COERCION_INDEX_BY_TYPE[ModelComposed]
-        elif (inspect.isclass(class_or_instance)
-                and issubclass(class_or_instance, ModelNormal)):
-            return COERCION_INDEX_BY_TYPE[ModelNormal]
-        elif (inspect.isclass(class_or_instance)
-                and issubclass(class_or_instance, ModelSimple)):
-            return COERCION_INDEX_BY_TYPE[ModelSimple]
-        elif class_or_instance in COERCION_INDEX_BY_TYPE:
-            return COERCION_INDEX_BY_TYPE[class_or_instance]
-        raise ApiValueError("Unsupported type: %s" % class_or_instance)
-
-    sorted_types = sorted(
-        required_types,
-        key=lambda class_or_instance: index_getter(class_or_instance)
-    )
-    return sorted_types
-
-
-def remove_uncoercible(required_types_classes, current_item, spec_property_naming,
-                       must_convert=True):
-    """Only keeps the type conversions that are possible
-
-    Args:
-        required_types_classes (tuple): tuple of classes that are required
-                          these should be ordered by COERCION_INDEX_BY_TYPE
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-        current_item (any): the current item (input data) to be converted
-
-    Keyword Args:
-        must_convert (bool): if True the item to convert is of the wrong
-                          type and we want a big list of coercibles
-                          if False, we want a limited list of coercibles
-
-    Returns:
-        (list): the remaining coercible required types, classes only
-    """
-    current_type_simple = get_simple_class(current_item)
-
-    results_classes = []
-    for required_type_class in required_types_classes:
-        # convert our models to OpenApiModel
-        required_type_class_simplified = required_type_class
-        if isinstance(required_type_class_simplified, type):
-            if issubclass(required_type_class_simplified, ModelComposed):
-                required_type_class_simplified = ModelComposed
-            elif issubclass(required_type_class_simplified, ModelNormal):
-                required_type_class_simplified = ModelNormal
-            elif issubclass(required_type_class_simplified, ModelSimple):
-                required_type_class_simplified = ModelSimple
-
-        if required_type_class_simplified == current_type_simple:
-            # don't consider converting to one's own class
-            continue
-
-        class_pair = (current_type_simple, required_type_class_simplified)
-        if must_convert and class_pair in COERCIBLE_TYPE_PAIRS[spec_property_naming]:
-            results_classes.append(required_type_class)
-        elif class_pair in UPCONVERSION_TYPE_PAIRS:
-            results_classes.append(required_type_class)
-    return results_classes
-
-
-def get_discriminated_classes(cls):
-    """
-    Returns all the classes that a discriminator converts to
-    TODO: lru_cache this
-    """
-    possible_classes = []
-    key = list(cls.discriminator.keys())[0]
-    if is_type_nullable(cls):
-        possible_classes.append(cls)
-    for discr_cls in cls.discriminator[key].values():
-        if hasattr(discr_cls, 'discriminator') and discr_cls.discriminator is not None:
-            possible_classes.extend(get_discriminated_classes(discr_cls))
-        else:
-            possible_classes.append(discr_cls)
-    return possible_classes
-
-
-def get_possible_classes(cls, from_server_context):
-    # TODO: lru_cache this
-    possible_classes = [cls]
-    if from_server_context:
-        return possible_classes
-    if hasattr(cls, 'discriminator') and cls.discriminator is not None:
-        possible_classes = []
-        possible_classes.extend(get_discriminated_classes(cls))
-    elif issubclass(cls, ModelComposed):
-        possible_classes.extend(composed_model_input_classes(cls))
-    return possible_classes
-
-
-def get_required_type_classes(required_types_mixed, spec_property_naming):
-    """Converts the tuple required_types into a tuple and a dict described
-    below
-
-    Args:
-        required_types_mixed (tuple/list): will contain either classes or
-            instance of list or dict
-        spec_property_naming (bool): if True these values came from the
-            server, and we use the data types in our endpoints.
-            If False, we are client side and we need to include
-            oneOf and discriminator classes inside the data types in our endpoints
-
-    Returns:
-        (valid_classes, dict_valid_class_to_child_types_mixed):
-            valid_classes (tuple): the valid classes that the current item
-                                   should be
-            dict_valid_class_to_child_types_mixed (dict):
-                valid_class (class): this is the key
-                child_types_mixed (list/dict/tuple): describes the valid child
-                    types
-    """
-    valid_classes = []
-    child_req_types_by_current_type = {}
-    for required_type in required_types_mixed:
-        if isinstance(required_type, list):
-            valid_classes.append(list)
-            child_req_types_by_current_type[list] = required_type
-        elif isinstance(required_type, tuple):
-            valid_classes.append(tuple)
-            child_req_types_by_current_type[tuple] = required_type
-        elif isinstance(required_type, dict):
-            valid_classes.append(dict)
-            child_req_types_by_current_type[dict] = required_type[str]
-        else:
-            valid_classes.extend(get_possible_classes(required_type, spec_property_naming))
-    return tuple(valid_classes), child_req_types_by_current_type
-
-
-def change_keys_js_to_python(input_dict, model_class):
-    """
-    Converts from javascript_key keys in the input_dict to python_keys in
-    the output dict using the mapping in model_class.
-    If the input_dict contains a key which does not declared in the model_class,
-    the key is added to the output dict as is. The assumption is the model_class
-    may have undeclared properties (additionalProperties attribute in the OAS
-    document).
-    """
-
-    if getattr(model_class, 'attribute_map', None) is None:
-        return input_dict
-    output_dict = {}
-    reversed_attr_map = {value: key for key, value in
-                         model_class.attribute_map.items()}
-    for javascript_key, value in input_dict.items():
-        python_key = reversed_attr_map.get(javascript_key)
-        if python_key is None:
-            # if the key is unknown, it is in error or it is an
-            # additionalProperties variable
-            python_key = javascript_key
-        output_dict[python_key] = value
-    return output_dict
-
-
-def get_type_error(var_value, path_to_item, valid_classes, key_type=False):
-    error_msg = type_error_message(
-        var_name=path_to_item[-1],
-        var_value=var_value,
-        valid_classes=valid_classes,
-        key_type=key_type
-    )
-    return ApiTypeError(
-        error_msg,
-        path_to_item=path_to_item,
-        valid_classes=valid_classes,
-        key_type=key_type
-    )
-
-
-def deserialize_primitive(data, klass, path_to_item):
-    """Deserializes string to primitive type.
-
-    :param data: str/int/float
-    :param klass: str/class the class to convert to
-
-    :return: int, float, str, bool, date, datetime
-    """
-    additional_message = ""
-    try:
-        if klass in {datetime, date}:
-            additional_message = (
-                "If you need your parameter to have a fallback "
-                "string value, please set its type as `type: {}` in your "
-                "spec. That allows the value to be any type. "
-            )
-            if klass == datetime:
-                if len(data) < 8:
-                    raise ValueError("This is not a datetime")
-                # The string should be in iso8601 datetime format.
-                parsed_datetime = parse(data)
-                date_only = (
-                    parsed_datetime.hour == 0 and
-                    parsed_datetime.minute == 0 and
-                    parsed_datetime.second == 0 and
-                    parsed_datetime.tzinfo is None and
-                    8 <= len(data) <= 10
-                )
-                if date_only:
-                    raise ValueError("This is a date, not a datetime")
-                return parsed_datetime
-            elif klass == date:
-                if len(data) < 8:
-                    raise ValueError("This is not a date")
-                return parse(data).date()
-        else:
-            converted_value = klass(data)
-            if isinstance(data, str) and klass == float:
-                if str(converted_value) != data:
-                    # '7' -> 7.0 -> '7.0' != '7'
-                    raise ValueError('This is not a float')
-            return converted_value
-    except (OverflowError, ValueError) as ex:
-        # parse can raise OverflowError
-        raise ApiValueError(
-            "{0}Failed to parse {1} as {2}".format(
-                additional_message, repr(data), klass.__name__
-            ),
-            path_to_item=path_to_item
-        ) from ex
-
-
-def get_discriminator_class(model_class,
-                            discr_name,
-                            discr_value, cls_visited):
-    """Returns the child class specified by the discriminator.
-
-    Args:
-        model_class (OpenApiModel): the model class.
-        discr_name (string): the name of the discriminator property.
-        discr_value (any): the discriminator value.
-        cls_visited (list): list of model classes that have been visited.
-            Used to determine the discriminator class without
-            visiting circular references indefinitely.
-
-    Returns:
-        used_model_class (class/None): the chosen child class that will be used
-            to deserialize the data, for example dog.Dog.
-            If a class is not found, None is returned.
-    """
-
-    if model_class in cls_visited:
-        # The class has already been visited and no suitable class was found.
-        return None
-    cls_visited.append(model_class)
-    used_model_class = None
-    if discr_name in model_class.discriminator:
-        class_name_to_discr_class = model_class.discriminator[discr_name]
-        used_model_class = class_name_to_discr_class.get(discr_value)
-    if used_model_class is None:
-        # We didn't find a discriminated class in class_name_to_discr_class.
-        # So look in the ancestor or descendant discriminators
-        # The discriminator mapping may exist in a descendant (anyOf, oneOf)
-        # or ancestor (allOf).
-        # Ancestor example: in the GrandparentAnimal -> ParentPet -> ChildCat
-        #   hierarchy, the discriminator mappings may be defined at any level
-        #   in the hierarchy.
-        # Descendant example:  mammal -> whale/zebra/Pig -> BasquePig/DanishPig
-        #   if we try to make BasquePig from mammal, we need to travel through
-        #   the oneOf descendant discriminators to find BasquePig
-        descendant_classes = model_class._composed_schemas.get('oneOf', ()) + \
-            model_class._composed_schemas.get('anyOf', ())
-        ancestor_classes = model_class._composed_schemas.get('allOf', ())
-        possible_classes = descendant_classes + ancestor_classes
-        for cls in possible_classes:
-            # Check if the schema has inherited discriminators.
-            if hasattr(cls, 'discriminator') and cls.discriminator is not None:
-                used_model_class = get_discriminator_class(
-                    cls, discr_name, discr_value, cls_visited)
-                if used_model_class is not None:
-                    return used_model_class
-    return used_model_class
-
-
-def deserialize_model(model_data, model_class, path_to_item, check_type,
-                      configuration, spec_property_naming):
-    """Deserializes model_data to model instance.
-
-    Args:
-        model_data (int/str/float/bool/none_type/list/dict): data to instantiate the model
-        model_class (OpenApiModel): the model class
-        path_to_item (list): path to the model in the received data
-        check_type (bool): whether to check the data tupe for the values in
-            the model
-        configuration (Configuration): the instance to use to convert files
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-
-    Returns:
-        model instance
-
-    Raise:
-        ApiTypeError
-        ApiValueError
-        ApiKeyError
-    """
-
-    kw_args = dict(_check_type=check_type,
-                   _path_to_item=path_to_item,
-                   _configuration=configuration,
-                   _spec_property_naming=spec_property_naming)
-
-    if issubclass(model_class, ModelSimple):
-        return model_class._new_from_openapi_data(model_data, **kw_args)
-    elif isinstance(model_data, list):
-        return model_class._new_from_openapi_data(*model_data, **kw_args)
-    if isinstance(model_data, dict):
-        kw_args.update(model_data)
-        return model_class._new_from_openapi_data(**kw_args)
-    elif isinstance(model_data, PRIMITIVE_TYPES):
-        return model_class._new_from_openapi_data(model_data, **kw_args)
-
-
-def deserialize_file(response_data, configuration, content_disposition=None):
-    """Deserializes body to file
-
-    Saves response body into a file in a temporary folder,
-    using the filename from the `Content-Disposition` header if provided.
-
-    Args:
-        param response_data (str):  the file data to write
-        configuration (Configuration): the instance to use to convert files
-
-    Keyword Args:
-        content_disposition (str):  the value of the Content-Disposition
-            header
-
-    Returns:
-        (file_type): the deserialized file which is open
-            The user is responsible for closing and reading the file
-    """
-    fd, path = tempfile.mkstemp(dir=configuration.temp_folder_path)
-    os.close(fd)
-    os.remove(path)
-
-    if content_disposition:
-        filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?',
-                             content_disposition,
-                             flags=re.I)
-        if filename is not None:
-            filename = filename.group(1)
-        else:
-            filename = "default_" + str(uuid.uuid4())
-
-        path = os.path.join(os.path.dirname(path), filename)
-
-    with open(path, "wb") as f:
-        if isinstance(response_data, str):
-            # change str to bytes so we can write it
-            response_data = response_data.encode('utf-8')
-        f.write(response_data)
-
-    f = open(path, "rb")
-    return f
-
-
-def attempt_convert_item(input_value, valid_classes, path_to_item,
-                         configuration, spec_property_naming, key_type=False,
-                         must_convert=False, check_type=True):
-    """
-    Args:
-        input_value (any): the data to convert
-        valid_classes (any): the classes that are valid
-        path_to_item (list): the path to the item to convert
-        configuration (Configuration): the instance to use to convert files
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-        key_type (bool): if True we need to convert a key type (not supported)
-        must_convert (bool): if True we must convert
-        check_type (bool): if True we check the type or the returned data in
-            ModelComposed/ModelNormal/ModelSimple instances
-
-    Returns:
-        instance (any) the fixed item
-
-    Raises:
-        ApiTypeError
-        ApiValueError
-        ApiKeyError
-    """
-    valid_classes_ordered = order_response_types(valid_classes)
-    valid_classes_coercible = remove_uncoercible(
-        valid_classes_ordered, input_value, spec_property_naming)
-    if not valid_classes_coercible or key_type:
-        # we do not handle keytype errors, json will take care
-        # of this for us
-        if configuration is None or not configuration.discard_unknown_keys:
-            raise get_type_error(input_value, path_to_item, valid_classes,
-                                 key_type=key_type)
-    for valid_class in valid_classes_coercible:
-        try:
-            if issubclass(valid_class, OpenApiModel):
-                return deserialize_model(input_value, valid_class,
-                                         path_to_item, check_type,
-                                         configuration, spec_property_naming)
-            elif valid_class == file_type:
-                return deserialize_file(input_value, configuration)
-            return deserialize_primitive(input_value, valid_class,
-                                         path_to_item)
-        except (ApiTypeError, ApiValueError, ApiKeyError) as conversion_exc:
-            if must_convert:
-                raise conversion_exc
-            # if we have conversion errors when must_convert == False
-            # we ignore the exception and move on to the next class
-            continue
-    # we were unable to convert, must_convert == False
-    return input_value
-
-
-def is_type_nullable(input_type):
-    """
-    Returns true if None is an allowed value for the specified input_type.
-
-    A type is nullable if at least one of the following conditions is true:
-    1. The OAS 'nullable' attribute has been specified,
-    1. The type is the 'null' type,
-    1. The type is a anyOf/oneOf composed schema, and a child schema is
-       the 'null' type.
-    Args:
-        input_type (type): the class of the input_value that we are
-            checking
-    Returns:
-        bool
-    """
-    if input_type is none_type:
-        return True
-    if issubclass(input_type, OpenApiModel) and input_type._nullable:
-        return True
-    if issubclass(input_type, ModelComposed):
-        # If oneOf/anyOf, check if the 'null' type is one of the allowed types.
-        for t in input_type._composed_schemas.get('oneOf', ()):
-            if is_type_nullable(t):
-                return True
-        for t in input_type._composed_schemas.get('anyOf', ()):
-            if is_type_nullable(t):
-                return True
-    return False
-
-
-def is_valid_type(input_class_simple, valid_classes):
-    """
-    Args:
-        input_class_simple (class): the class of the input_value that we are
-            checking
-        valid_classes (tuple): the valid classes that the current item
-            should be
-    Returns:
-        bool
-    """
-    if issubclass(input_class_simple, OpenApiModel) and \
-            valid_classes == (bool, date, datetime, dict, float, int, list, str, none_type,):
-        return True
-    valid_type = input_class_simple in valid_classes
-    if not valid_type and (
-            issubclass(input_class_simple, OpenApiModel) or
-            input_class_simple is none_type):
-        for valid_class in valid_classes:
-            if input_class_simple is none_type and is_type_nullable(valid_class):
-                # Schema is oneOf/anyOf and the 'null' type is one of the allowed types.
-                return True
-            if not (issubclass(valid_class, OpenApiModel) and valid_class.discriminator):
-                continue
-            discr_propertyname_py = list(valid_class.discriminator.keys())[0]
-            discriminator_classes = (
-                valid_class.discriminator[discr_propertyname_py].values()
-            )
-            valid_type = is_valid_type(input_class_simple, discriminator_classes)
-            if valid_type:
-                return True
-    return valid_type
-
-
-def validate_and_convert_types(input_value, required_types_mixed, path_to_item,
-                               spec_property_naming, _check_type, configuration=None):
-    """Raises a TypeError is there is a problem, otherwise returns value
-
-    Args:
-        input_value (any): the data to validate/convert
-        required_types_mixed (list/dict/tuple): A list of
-            valid classes, or a list tuples of valid classes, or a dict where
-            the value is a tuple of value classes
-        path_to_item: (list) the path to the data being validated
-            this stores a list of keys or indices to get to the data being
-            validated
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-        _check_type: (boolean) if true, type will be checked and conversion
-            will be attempted.
-        configuration: (Configuration): the configuration class to use
-            when converting file_type items.
-            If passed, conversion will be attempted when possible
-            If not passed, no conversions will be attempted and
-            exceptions will be raised
-
-    Returns:
-        the correctly typed value
-
-    Raises:
-        ApiTypeError
-    """
-    results = get_required_type_classes(required_types_mixed, spec_property_naming)
-    valid_classes, child_req_types_by_current_type = results
-
-    input_class_simple = get_simple_class(input_value)
-    valid_type = is_valid_type(input_class_simple, valid_classes)
-    if not valid_type:
-        if (configuration
-                or (input_class_simple == dict
-                    and dict not in valid_classes)):
-            # if input_value is not valid_type try to convert it
-            converted_instance = attempt_convert_item(
-                input_value,
-                valid_classes,
-                path_to_item,
-                configuration,
-                spec_property_naming,
-                key_type=False,
-                must_convert=True,
-                check_type=_check_type
-            )
-            return converted_instance
-        else:
-            raise get_type_error(input_value, path_to_item, valid_classes,
-                                 key_type=False)
-
-    # input_value's type is in valid_classes
-    if len(valid_classes) > 1 and configuration:
-        # there are valid classes which are not the current class
-        valid_classes_coercible = remove_uncoercible(
-            valid_classes, input_value, spec_property_naming, must_convert=False)
-        if valid_classes_coercible:
-            converted_instance = attempt_convert_item(
-                input_value,
-                valid_classes_coercible,
-                path_to_item,
-                configuration,
-                spec_property_naming,
-                key_type=False,
-                must_convert=False,
-                check_type=_check_type
-            )
-            return converted_instance
-
-    if child_req_types_by_current_type == {}:
-        # all types are of the required types and there are no more inner
-        # variables left to look at
-        return input_value
-    inner_required_types = child_req_types_by_current_type.get(
-        type(input_value)
-    )
-    if inner_required_types is None:
-        # for this type, there are not more inner variables left to look at
-        return input_value
-    if isinstance(input_value, list):
-        if input_value == []:
-            # allow an empty list
-            return input_value
-        for index, inner_value in enumerate(input_value):
-            inner_path = list(path_to_item)
-            inner_path.append(index)
-            input_value[index] = validate_and_convert_types(
-                inner_value,
-                inner_required_types,
-                inner_path,
-                spec_property_naming,
-                _check_type,
-                configuration=configuration
-            )
-    elif isinstance(input_value, dict):
-        if input_value == {}:
-            # allow an empty dict
-            return input_value
-        for inner_key, inner_val in input_value.items():
-            inner_path = list(path_to_item)
-            inner_path.append(inner_key)
-            if get_simple_class(inner_key) != str:
-                raise get_type_error(inner_key, inner_path, valid_classes,
-                                     key_type=True)
-            input_value[inner_key] = validate_and_convert_types(
-                inner_val,
-                inner_required_types,
-                inner_path,
-                spec_property_naming,
-                _check_type,
-                configuration=configuration
-            )
-    return input_value
-
-
-def model_to_dict(model_instance, serialize=True):
-    """Returns the model properties as a dict
-
-    Args:
-        model_instance (one of your model instances): the model instance that
-            will be converted to a dict.
-
-    Keyword Args:
-        serialize (bool): if True, the keys in the dict will be values from
-            attribute_map
-    """
-    result = {}
-
-    def extract_item(item): return (
-        item[0], model_to_dict(
-            item[1], serialize=serialize)) if hasattr(
-        item[1], '_data_store') else item
-
-    model_instances = [model_instance]
-    if model_instance._composed_schemas:
-        model_instances.extend(model_instance._composed_instances)
-    seen_json_attribute_names = set()
-    used_fallback_python_attribute_names = set()
-    py_to_json_map = {}
-    for model_instance in model_instances:
-        for attr, value in model_instance._data_store.items():
-            if serialize:
-                # we use get here because additional property key names do not
-                # exist in attribute_map
-                try:
-                    attr = model_instance.attribute_map[attr]
-                    py_to_json_map.update(model_instance.attribute_map)
-                    seen_json_attribute_names.add(attr)
-                except KeyError:
-                    used_fallback_python_attribute_names.add(attr)
-            if isinstance(value, list):
-                if not value:
-                    # empty list or None
-                    result[attr] = value
-                else:
-                    res = []
-                    for v in value:
-                        if isinstance(v, PRIMITIVE_TYPES) or v is None:
-                            res.append(v)
-                        elif isinstance(v, ModelSimple):
-                            res.append(v.value)
-                        elif isinstance(v, dict):
-                            res.append(dict(map(
-                                extract_item,
-                                v.items()
-                            )))
-                        else:
-                            res.append(model_to_dict(v, serialize=serialize))
-                    result[attr] = res
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    extract_item,
-                    value.items()
-                ))
-            elif isinstance(value, ModelSimple):
-                result[attr] = value.value
-            elif hasattr(value, '_data_store'):
-                result[attr] = model_to_dict(value, serialize=serialize)
-            else:
-                result[attr] = value
-    if serialize:
-        for python_key in used_fallback_python_attribute_names:
-            json_key = py_to_json_map.get(python_key)
-            if json_key is None:
-                continue
-            if python_key == json_key:
-                continue
-            json_key_assigned_no_need_for_python_key = json_key in seen_json_attribute_names
-            if json_key_assigned_no_need_for_python_key:
-                del result[python_key]
-
-    return result
-
-
-def type_error_message(var_value=None, var_name=None, valid_classes=None,
-                       key_type=None):
-    """
-    Keyword Args:
-        var_value (any): the variable which has the type_error
-        var_name (str): the name of the variable which has the typ error
-        valid_classes (tuple): the accepted classes for current_item's
-                                  value
-        key_type (bool): False if our value is a value in a dict
-                         True if it is a key in a dict
-                         False if our item is an item in a list
-    """
-    key_or_value = 'value'
-    if key_type:
-        key_or_value = 'key'
-    valid_classes_phrase = get_valid_classes_phrase(valid_classes)
-    msg = (
-        "Invalid type for variable '{0}'. Required {1} type {2} and "
-        "passed type was {3}".format(
-            var_name,
-            key_or_value,
-            valid_classes_phrase,
-            type(var_value).__name__,
-        )
-    )
-    return msg
-
-
-def get_valid_classes_phrase(input_classes):
-    """Returns a string phrase describing what types are allowed
-    """
-    all_classes = list(input_classes)
-    all_classes = sorted(all_classes, key=lambda cls: cls.__name__)
-    all_class_names = [cls.__name__ for cls in all_classes]
-    if len(all_class_names) == 1:
-        return 'is {0}'.format(all_class_names[0])
-    return "is one of [{0}]".format(", ".join(all_class_names))
-
-
-def get_allof_instances(self, model_args, constant_args):
-    """
-    Args:
-        self: the class we are handling
-        model_args (dict): var_name to var_value
-            used to make instances
-        constant_args (dict):
-            metadata arguments:
-            _check_type
-            _path_to_item
-            _spec_property_naming
-            _configuration
-            _visited_composed_classes
-
-    Returns
-        composed_instances (list)
-    """
-    composed_instances = []
-    for allof_class in self._composed_schemas['allOf']:
-
-        try:
-            if constant_args.get('_spec_property_naming'):
-                allof_instance = allof_class._from_openapi_data(**model_args, **constant_args)
-            else:
-                allof_instance = allof_class(**model_args, **constant_args)
-            composed_instances.append(allof_instance)
-        except Exception as ex:
-            raise ApiValueError(
-                "Invalid inputs given to generate an instance of '%s'. The "
-                "input data was invalid for the allOf schema '%s' in the composed "
-                "schema '%s'. Error=%s" % (
-                    allof_class.__name__,
-                    allof_class.__name__,
-                    self.__class__.__name__,
-                    str(ex)
-                )
-            ) from ex
-    return composed_instances
-
-
-def get_oneof_instance(cls, model_kwargs, constant_kwargs, model_arg=None):
-    """
-    Find the oneOf schema that matches the input data (e.g. payload).
-    If exactly one schema matches the input data, an instance of that schema
-    is returned.
-    If zero or more than one schema match the input data, an exception is raised.
-    In OAS 3.x, the payload MUST, by validation, match exactly one of the
-    schemas described by oneOf.
-
-    Args:
-        cls: the class we are handling
-        model_kwargs (dict): var_name to var_value
-            The input data, e.g. the payload that must match a oneOf schema
-            in the OpenAPI document.
-        constant_kwargs (dict): var_name to var_value
-            args that every model requires, including configuration, server
-            and path to item.
-
-    Kwargs:
-        model_arg: (int, float, bool, str, date, datetime, ModelSimple, None):
-            the value to assign to a primitive class or ModelSimple class
-            Notes:
-            - this is only passed in when oneOf includes types which are not object
-            - None is used to suppress handling of model_arg, nullable models are handled in __new__
-
-    Returns
-        oneof_instance (instance)
-    """
-    if len(cls._composed_schemas['oneOf']) == 0:
-        return None
-
-    oneof_instances = []
-    # Iterate over each oneOf schema and determine if the input data
-    # matches the oneOf schemas.
-    for oneof_class in cls._composed_schemas['oneOf']:
-        # The composed oneOf schema allows the 'null' type and the input data
-        # is the null value. This is a OAS >= 3.1 feature.
-        if oneof_class is none_type:
-            # skip none_types because we are deserializing dict data.
-            # none_type deserialization is handled in the __new__ method
-            continue
-
-        single_value_input = allows_single_value_input(oneof_class)
-
-        try:
-            if not single_value_input:
-                if constant_kwargs.get('_spec_property_naming'):
-                    oneof_instance = oneof_class._from_openapi_data(
-                        **model_kwargs, **constant_kwargs)
-                else:
-                    oneof_instance = oneof_class(**model_kwargs, **constant_kwargs)
-            else:
-                if issubclass(oneof_class, ModelSimple):
-                    if constant_kwargs.get('_spec_property_naming'):
-                        oneof_instance = oneof_class._from_openapi_data(
-                            model_arg, **constant_kwargs)
-                    else:
-                        oneof_instance = oneof_class(model_arg, **constant_kwargs)
-                elif oneof_class in PRIMITIVE_TYPES:
-                    oneof_instance = validate_and_convert_types(
-                        model_arg,
-                        (oneof_class,),
-                        constant_kwargs['_path_to_item'],
-                        constant_kwargs['_spec_property_naming'],
-                        constant_kwargs['_check_type'],
-                        configuration=constant_kwargs['_configuration']
-                    )
-            oneof_instances.append(oneof_instance)
-        except Exception:
-            pass
-    if len(oneof_instances) == 0:
-        raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. None "
-            "of the oneOf schemas matched the input data." %
-            cls.__name__
-        )
-    elif len(oneof_instances) > 1:
-        raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. Multiple "
-            "oneOf schemas matched the inputs, but a max of one is allowed." %
-            cls.__name__
-        )
-    return oneof_instances[0]
-
-
-def get_anyof_instances(self, model_args, constant_args):
-    """
-    Args:
-        self: the class we are handling
-        model_args (dict): var_name to var_value
-            The input data, e.g. the payload that must match at least one
-            anyOf child schema in the OpenAPI document.
-        constant_args (dict): var_name to var_value
-            args that every model requires, including configuration, server
-            and path to item.
-
-    Returns
-        anyof_instances (list)
-    """
-    anyof_instances = []
-    if len(self._composed_schemas['anyOf']) == 0:
-        return anyof_instances
-
-    for anyof_class in self._composed_schemas['anyOf']:
-        # The composed oneOf schema allows the 'null' type and the input data
-        # is the null value. This is a OAS >= 3.1 feature.
-        if anyof_class is none_type:
-            # skip none_types because we are deserializing dict data.
-            # none_type deserialization is handled in the __new__ method
-            continue
-
-        try:
-            if constant_args.get('_spec_property_naming'):
-                anyof_instance = anyof_class._from_openapi_data(**model_args, **constant_args)
-            else:
-                anyof_instance = anyof_class(**model_args, **constant_args)
-            anyof_instances.append(anyof_instance)
-        except Exception:
-            pass
-    if len(anyof_instances) == 0:
-        raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. None of the "
-            "anyOf schemas matched the inputs." %
-            self.__class__.__name__
-        )
-    return anyof_instances
-
-
-def get_discarded_args(self, composed_instances, model_args):
-    """
-    Gathers the args that were discarded by configuration.discard_unknown_keys
-    """
-    model_arg_keys = model_args.keys()
-    discarded_args = set()
-    # arguments passed to self were already converted to python names
-    # before __init__ was called
-    for instance in composed_instances:
-        if instance.__class__ in self._composed_schemas['allOf']:
-            try:
-                keys = instance.to_dict().keys()
-                discarded_keys = model_args - keys
-                discarded_args.update(discarded_keys)
-            except Exception:
-                # allOf integer schema will throw exception
-                pass
-        else:
-            try:
-                all_keys = set(model_to_dict(instance, serialize=False).keys())
-                js_keys = model_to_dict(instance, serialize=True).keys()
-                all_keys.update(js_keys)
-                discarded_keys = model_arg_keys - all_keys
-                discarded_args.update(discarded_keys)
-            except Exception:
-                # allOf integer schema will throw exception
-                pass
-    return discarded_args
-
-
-def validate_get_composed_info(constant_args, model_args, self):
-    """
-    For composed schemas, generate schema instances for
-    all schemas in the oneOf/anyOf/allOf definition. If additional
-    properties are allowed, also assign those properties on
-    all matched schemas that contain additionalProperties.
-    Openapi schemas are python classes.
-
-    Exceptions are raised if:
-    - 0 or > 1 oneOf schema matches the model_args input data
-    - no anyOf schema matches the model_args input data
-    - any of the allOf schemas do not match the model_args input data
-
-    Args:
-        constant_args (dict): these are the args that every model requires
-        model_args (dict): these are the required and optional spec args that
-            were passed in to make this model
-        self (class): the class that we are instantiating
-            This class contains self._composed_schemas
-
-    Returns:
-        composed_info (list): length three
-            composed_instances (list): the composed instances which are not
-                self
-            var_name_to_model_instances (dict): a dict going from var_name
-                to the model_instance which holds that var_name
-                the model_instance may be self or an instance of one of the
-                classes in self.composed_instances()
-            additional_properties_model_instances (list): a list of the
-                model instances which have the property
-                additional_properties_type. This list can include self
-    """
-    # create composed_instances
-    composed_instances = []
-    allof_instances = get_allof_instances(self, model_args, constant_args)
-    composed_instances.extend(allof_instances)
-    oneof_instance = get_oneof_instance(self.__class__, model_args, constant_args)
-    if oneof_instance is not None:
-        composed_instances.append(oneof_instance)
-    anyof_instances = get_anyof_instances(self, model_args, constant_args)
-    composed_instances.extend(anyof_instances)
-    """
-    set additional_properties_model_instances
-    additional properties must be evaluated at the schema level
-    so self's additional properties are most important
-    If self is a composed schema with:
-    - no properties defined in self
-    - additionalProperties: False
-    Then for object payloads every property is an additional property
-    and they are not allowed, so only empty dict is allowed
-
-    Properties must be set on all matching schemas
-    so when a property is assigned toa composed instance, it must be set on all
-    composed instances regardless of additionalProperties presence
-    keeping it to prevent breaking changes in v5.0.1
-    TODO remove cls._additional_properties_model_instances in 6.0.0
-    """
-    additional_properties_model_instances = []
-    if self.additional_properties_type is not None:
-        additional_properties_model_instances = [self]
-
-    """
-    no need to set properties on self in here, they will be set in __init__
-    By here all composed schema oneOf/anyOf/allOf instances have their properties set using
-    model_args
-    """
-    discarded_args = get_discarded_args(self, composed_instances, model_args)
-
-    # map variable names to composed_instances
-    var_name_to_model_instances = {}
-    for prop_name in model_args:
-        if prop_name not in discarded_args:
-            var_name_to_model_instances[prop_name] = [self] + composed_instances
-
-    return [
-        composed_instances,
-        var_name_to_model_instances,
-        additional_properties_model_instances,
-        discarded_args
-    ]
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+from datetime import date, datetime  # noqa: F401
+from copy import deepcopy
+import inspect
+import io
+import os
+import pprint
+import re
+import tempfile
+import uuid
+
+from dateutil.parser import parse
+
+from code_size_analyzer_client.exceptions import (
+    ApiKeyError,
+    ApiAttributeError,
+    ApiTypeError,
+    ApiValueError,
+)
+
+none_type = type(None)
+file_type = io.IOBase
+
+
+def convert_js_args_to_python_args(fn):
+    from functools import wraps
+    @wraps(fn)
+    def wrapped_init(_self, *args, **kwargs):
+        """
+        An attribute named `self` received from the api will conflicts with the reserved `self`
+        parameter of a class method. During generation, `self` attributes are mapped
+        to `_self` in models. Here, we name `_self` instead of `self` to avoid conflicts.
+        """
+        spec_property_naming = kwargs.get('_spec_property_naming', False)
+        if spec_property_naming:
+            kwargs = change_keys_js_to_python(
+                kwargs, _self if isinstance(
+                    _self, type) else _self.__class__)
+        return fn(_self, *args, **kwargs)
+    return wrapped_init
+
+
+class cached_property(object):
+    # this caches the result of the function call for fn with no inputs
+    # use this as a decorator on function methods that you want converted
+    # into cached properties
+    result_key = '_results'
+
+    def __init__(self, fn):
+        self._fn = fn
+
+    def __get__(self, instance, cls=None):
+        if self.result_key in vars(self):
+            return vars(self)[self.result_key]
+        else:
+            result = self._fn()
+            setattr(self, self.result_key, result)
+            return result
+
+
+PRIMITIVE_TYPES = (list, float, int, bool, datetime, date, str, file_type)
+
+
+def allows_single_value_input(cls):
+    """
+    This function returns True if the input composed schema model or any
+    descendant model allows a value only input
+    This is true for cases where oneOf contains items like:
+    oneOf:
+      - float
+      - NumberWithValidation
+      - StringEnum
+      - ArrayModel
+      - null
+    TODO: lru_cache this
+    """
+    if (
+        issubclass(cls, ModelSimple) or
+        cls in PRIMITIVE_TYPES
+    ):
+        return True
+    elif issubclass(cls, ModelComposed):
+        if not cls._composed_schemas['oneOf']:
+            return False
+        return any(allows_single_value_input(c) for c in cls._composed_schemas['oneOf'])
+    return False
+
+
+def composed_model_input_classes(cls):
+    """
+    This function returns a list of the possible models that can be accepted as
+    inputs.
+    TODO: lru_cache this
+    """
+    if issubclass(cls, ModelSimple) or cls in PRIMITIVE_TYPES:
+        return [cls]
+    elif issubclass(cls, ModelNormal):
+        if cls.discriminator is None:
+            return [cls]
+        else:
+            return get_discriminated_classes(cls)
+    elif issubclass(cls, ModelComposed):
+        if not cls._composed_schemas['oneOf']:
+            return []
+        if cls.discriminator is None:
+            input_classes = []
+            for c in cls._composed_schemas['oneOf']:
+                input_classes.extend(composed_model_input_classes(c))
+            return input_classes
+        else:
+            return get_discriminated_classes(cls)
+    return []
+
+
+class OpenApiModel(object):
+    """The base class for all OpenAPIModels"""
+
+    def set_attribute(self, name, value):
+        # this is only used to set properties on self
+
+        path_to_item = []
+        if self._path_to_item:
+            path_to_item.extend(self._path_to_item)
+        path_to_item.append(name)
+
+        if name in self.openapi_types:
+            required_types_mixed = self.openapi_types[name]
+        elif self.additional_properties_type is None:
+            raise ApiAttributeError(
+                "{0} has no attribute '{1}'".format(
+                    type(self).__name__, name),
+                path_to_item
+            )
+        elif self.additional_properties_type is not None:
+            required_types_mixed = self.additional_properties_type
+
+        if get_simple_class(name) != str:
+            error_msg = type_error_message(
+                var_name=name,
+                var_value=name,
+                valid_classes=(str,),
+                key_type=True
+            )
+            raise ApiTypeError(
+                error_msg,
+                path_to_item=path_to_item,
+                valid_classes=(str,),
+                key_type=True
+            )
+
+        if self._check_type:
+            value = validate_and_convert_types(
+                value, required_types_mixed, path_to_item, self._spec_property_naming,
+                self._check_type, configuration=self._configuration)
+        if (name,) in self.allowed_values:
+            check_allowed_values(
+                self.allowed_values,
+                (name,),
+                value
+            )
+        if (name,) in self.validations:
+            check_validations(
+                self.validations,
+                (name,),
+                value,
+                self._configuration
+            )
+        self.__dict__['_data_store'][name] = value
+
+    def __repr__(self):
+        """For `print` and `pprint`"""
+        return self.to_str()
+
+    def __ne__(self, other):
+        """Returns true if both objects are not equal"""
+        return not self == other
+
+    def __setattr__(self, attr, value):
+        """set the value of an attribute using dot notation: `instance.attr = val`"""
+        self[attr] = value
+
+    def __getattr__(self, attr):
+        """get the value of an attribute using dot notation: `instance.attr`"""
+        return self.__getitem__(attr)
+
+    def __copy__(self):
+        cls = self.__class__
+        if self.get("_spec_property_naming", False):
+            return cls._new_from_openapi_data(**self.__dict__)
+        else:
+            return cls.__new__(cls, **self.__dict__)
+
+    def __deepcopy__(self, memo):
+        cls = self.__class__
+
+        if self.get("_spec_property_naming", False):
+            new_inst = cls._new_from_openapi_data()
+        else:
+            new_inst = cls.__new__(cls)
+
+        for k, v in self.__dict__.items():
+            setattr(new_inst, k, deepcopy(v, memo))
+        return new_inst
+
+
+    def __new__(cls, *args, **kwargs):
+        # this function uses the discriminator to
+        # pick a new schema/class to instantiate because a discriminator
+        # propertyName value was passed in
+
+        if len(args) == 1:
+            arg = args[0]
+            if arg is None and is_type_nullable(cls):
+                # The input data is the 'null' value and the type is nullable.
+                return None
+
+            if issubclass(cls, ModelComposed) and allows_single_value_input(cls):
+                model_kwargs = {}
+                oneof_instance = get_oneof_instance(cls, model_kwargs, kwargs, model_arg=arg)
+                return oneof_instance
+
+        visited_composed_classes = kwargs.get('_visited_composed_classes', ())
+        if (
+            cls.discriminator is None or
+            cls in visited_composed_classes
+        ):
+            # Use case 1: this openapi schema (cls) does not have a discriminator
+            # Use case 2: we have already visited this class before and are sure that we
+            # want to instantiate it this time. We have visited this class deserializing
+            # a payload with a discriminator. During that process we traveled through
+            # this class but did not make an instance of it. Now we are making an
+            # instance of a composed class which contains cls in it, so this time make an instance of cls.
+            #
+            # Here's an example of use case 2: If Animal has a discriminator
+            # petType and we pass in "Dog", and the class Dog
+            # allOf includes Animal, we move through Animal
+            # once using the discriminator, and pick Dog.
+            # Then in the composed schema dog Dog, we will make an instance of the
+            # Animal class (because Dal has allOf: Animal) but this time we won't travel
+            # through Animal's discriminator because we passed in
+            # _visited_composed_classes = (Animal,)
+
+            return super(OpenApiModel, cls).__new__(cls)
+
+        # Get the name and value of the discriminator property.
+        # The discriminator name is obtained from the discriminator meta-data
+        # and the discriminator value is obtained from the input data.
+        discr_propertyname_py = list(cls.discriminator.keys())[0]
+        discr_propertyname_js = cls.attribute_map[discr_propertyname_py]
+        if discr_propertyname_js in kwargs:
+            discr_value = kwargs[discr_propertyname_js]
+        elif discr_propertyname_py in kwargs:
+            discr_value = kwargs[discr_propertyname_py]
+        else:
+            # The input data does not contain the discriminator property.
+            path_to_item = kwargs.get('_path_to_item', ())
+            raise ApiValueError(
+                "Cannot deserialize input data due to missing discriminator. "
+                "The discriminator property '%s' is missing at path: %s" %
+                (discr_propertyname_js, path_to_item)
+            )
+
+        # Implementation note: the last argument to get_discriminator_class
+        # is a list of visited classes. get_discriminator_class may recursively
+        # call itself and update the list of visited classes, and the initial
+        # value must be an empty list. Hence not using 'visited_composed_classes'
+        new_cls = get_discriminator_class(
+            cls, discr_propertyname_py, discr_value, [])
+        if new_cls is None:
+            path_to_item = kwargs.get('_path_to_item', ())
+            disc_prop_value = kwargs.get(
+                discr_propertyname_js, kwargs.get(discr_propertyname_py))
+            raise ApiValueError(
+                "Cannot deserialize input data due to invalid discriminator "
+                "value. The OpenAPI document has no mapping for discriminator "
+                "property '%s'='%s' at path: %s" %
+                (discr_propertyname_js, disc_prop_value, path_to_item)
+            )
+
+        if new_cls in visited_composed_classes:
+            # if we are making an instance of a composed schema Descendent
+            # which allOf includes Ancestor, then Ancestor contains
+            # a discriminator that includes Descendent.
+            # So if we make an instance of Descendent, we have to make an
+            # instance of Ancestor to hold the allOf properties.
+            # This code detects that use case and makes the instance of Ancestor
+            # For example:
+            # When making an instance of Dog, _visited_composed_classes = (Dog,)
+            # then we make an instance of Animal to include in dog._composed_instances
+            # so when we are here, cls is Animal
+            # cls.discriminator != None
+            # cls not in _visited_composed_classes
+            # new_cls = Dog
+            # but we know we know that we already have Dog
+            # because it is in visited_composed_classes
+            # so make Animal here
+            return super(OpenApiModel, cls).__new__(cls)
+
+        # Build a list containing all oneOf and anyOf descendants.
+        oneof_anyof_classes = None
+        if cls._composed_schemas is not None:
+            oneof_anyof_classes = (
+                cls._composed_schemas.get('oneOf', ()) +
+                cls._composed_schemas.get('anyOf', ()))
+        oneof_anyof_child = new_cls in oneof_anyof_classes
+        kwargs['_visited_composed_classes'] = visited_composed_classes + (cls,)
+
+        if cls._composed_schemas.get('allOf') and oneof_anyof_child:
+            # Validate that we can make self because when we make the
+            # new_cls it will not include the allOf validations in self
+            self_inst = super(OpenApiModel, cls).__new__(cls)
+            self_inst.__init__(*args, **kwargs)
+
+        if kwargs.get("_spec_property_naming", False):
+            # when true, implies new is from deserialization
+            new_inst = new_cls._new_from_openapi_data(*args, **kwargs)
+        else:
+            new_inst = new_cls.__new__(new_cls, *args, **kwargs)
+            new_inst.__init__(*args, **kwargs)
+
+        return new_inst
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _new_from_openapi_data(cls, *args, **kwargs):
+        # this function uses the discriminator to
+        # pick a new schema/class to instantiate because a discriminator
+        # propertyName value was passed in
+
+        if len(args) == 1:
+            arg = args[0]
+            if arg is None and is_type_nullable(cls):
+                # The input data is the 'null' value and the type is nullable.
+                return None
+
+            if issubclass(cls, ModelComposed) and allows_single_value_input(cls):
+                model_kwargs = {}
+                oneof_instance = get_oneof_instance(cls, model_kwargs, kwargs, model_arg=arg)
+                return oneof_instance
+
+        visited_composed_classes = kwargs.get('_visited_composed_classes', ())
+        if (
+            cls.discriminator is None or
+            cls in visited_composed_classes
+        ):
+            # Use case 1: this openapi schema (cls) does not have a discriminator
+            # Use case 2: we have already visited this class before and are sure that we
+            # want to instantiate it this time. We have visited this class deserializing
+            # a payload with a discriminator. During that process we traveled through
+            # this class but did not make an instance of it. Now we are making an
+            # instance of a composed class which contains cls in it, so this time make an instance of cls.
+            #
+            # Here's an example of use case 2: If Animal has a discriminator
+            # petType and we pass in "Dog", and the class Dog
+            # allOf includes Animal, we move through Animal
+            # once using the discriminator, and pick Dog.
+            # Then in the composed schema dog Dog, we will make an instance of the
+            # Animal class (because Dal has allOf: Animal) but this time we won't travel
+            # through Animal's discriminator because we passed in
+            # _visited_composed_classes = (Animal,)
+
+            return cls._from_openapi_data(*args, **kwargs)
+
+        # Get the name and value of the discriminator property.
+        # The discriminator name is obtained from the discriminator meta-data
+        # and the discriminator value is obtained from the input data.
+        discr_propertyname_py = list(cls.discriminator.keys())[0]
+        discr_propertyname_js = cls.attribute_map[discr_propertyname_py]
+        if discr_propertyname_js in kwargs:
+            discr_value = kwargs[discr_propertyname_js]
+        elif discr_propertyname_py in kwargs:
+            discr_value = kwargs[discr_propertyname_py]
+        else:
+            # The input data does not contain the discriminator property.
+            path_to_item = kwargs.get('_path_to_item', ())
+            raise ApiValueError(
+                "Cannot deserialize input data due to missing discriminator. "
+                "The discriminator property '%s' is missing at path: %s" %
+                (discr_propertyname_js, path_to_item)
+            )
+
+        # Implementation note: the last argument to get_discriminator_class
+        # is a list of visited classes. get_discriminator_class may recursively
+        # call itself and update the list of visited classes, and the initial
+        # value must be an empty list. Hence not using 'visited_composed_classes'
+        new_cls = get_discriminator_class(
+            cls, discr_propertyname_py, discr_value, [])
+        if new_cls is None:
+            path_to_item = kwargs.get('_path_to_item', ())
+            disc_prop_value = kwargs.get(
+                discr_propertyname_js, kwargs.get(discr_propertyname_py))
+            raise ApiValueError(
+                "Cannot deserialize input data due to invalid discriminator "
+                "value. The OpenAPI document has no mapping for discriminator "
+                "property '%s'='%s' at path: %s" %
+                (discr_propertyname_js, disc_prop_value, path_to_item)
+            )
+
+        if new_cls in visited_composed_classes:
+            # if we are making an instance of a composed schema Descendent
+            # which allOf includes Ancestor, then Ancestor contains
+            # a discriminator that includes Descendent.
+            # So if we make an instance of Descendent, we have to make an
+            # instance of Ancestor to hold the allOf properties.
+            # This code detects that use case and makes the instance of Ancestor
+            # For example:
+            # When making an instance of Dog, _visited_composed_classes = (Dog,)
+            # then we make an instance of Animal to include in dog._composed_instances
+            # so when we are here, cls is Animal
+            # cls.discriminator != None
+            # cls not in _visited_composed_classes
+            # new_cls = Dog
+            # but we know we know that we already have Dog
+            # because it is in visited_composed_classes
+            # so make Animal here
+            return cls._from_openapi_data(*args, **kwargs)
+
+        # Build a list containing all oneOf and anyOf descendants.
+        oneof_anyof_classes = None
+        if cls._composed_schemas is not None:
+            oneof_anyof_classes = (
+                cls._composed_schemas.get('oneOf', ()) +
+                cls._composed_schemas.get('anyOf', ()))
+        oneof_anyof_child = new_cls in oneof_anyof_classes
+        kwargs['_visited_composed_classes'] = visited_composed_classes + (cls,)
+
+        if cls._composed_schemas.get('allOf') and oneof_anyof_child:
+            # Validate that we can make self because when we make the
+            # new_cls it will not include the allOf validations in self
+            self_inst = cls._from_openapi_data(*args, **kwargs)
+
+        new_inst = new_cls._new_from_openapi_data(*args, **kwargs)
+        return new_inst
+
+
+class ModelSimple(OpenApiModel):
+    """the parent class of models whose type != object in their
+    swagger/openapi"""
+
+    def __setitem__(self, name, value):
+        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
+        if name in self.required_properties:
+            self.__dict__[name] = value
+            return
+
+        self.set_attribute(name, value)
+
+    def get(self, name, default=None):
+        """returns the value of an attribute or some default value if the attribute was not set"""
+        if name in self.required_properties:
+            return self.__dict__[name]
+
+        return self.__dict__['_data_store'].get(name, default)
+
+    def __getitem__(self, name):
+        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
+        if name in self:
+            return self.get(name)
+
+        raise ApiAttributeError(
+            "{0} has no attribute '{1}'".format(
+                type(self).__name__, name),
+            [e for e in [self._path_to_item, name] if e]
+        )
+
+    def __contains__(self, name):
+        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
+        if name in self.required_properties:
+            return name in self.__dict__
+
+        return name in self.__dict__['_data_store']
+
+    def to_str(self):
+        """Returns the string representation of the model"""
+        return str(self.value)
+
+    def __eq__(self, other):
+        """Returns true if both objects are equal"""
+        if not isinstance(other, self.__class__):
+            return False
+
+        this_val = self._data_store['value']
+        that_val = other._data_store['value']
+        types = set()
+        types.add(this_val.__class__)
+        types.add(that_val.__class__)
+        vals_equal = this_val == that_val
+        return vals_equal
+
+
+class ModelNormal(OpenApiModel):
+    """the parent class of models whose type == object in their
+    swagger/openapi"""
+
+    def __setitem__(self, name, value):
+        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
+        if name in self.required_properties:
+            self.__dict__[name] = value
+            return
+
+        self.set_attribute(name, value)
+
+    def get(self, name, default=None):
+        """returns the value of an attribute or some default value if the attribute was not set"""
+        if name in self.required_properties:
+            return self.__dict__[name]
+
+        return self.__dict__['_data_store'].get(name, default)
+
+    def __getitem__(self, name):
+        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
+        if name in self:
+            return self.get(name)
+
+        raise ApiAttributeError(
+            "{0} has no attribute '{1}'".format(
+                type(self).__name__, name),
+            [e for e in [self._path_to_item, name] if e]
+        )
+
+    def __contains__(self, name):
+        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
+        if name in self.required_properties:
+            return name in self.__dict__
+
+        return name in self.__dict__['_data_store']
+
+    def to_dict(self):
+        """Returns the model properties as a dict"""
+        return model_to_dict(self, serialize=False)
+
+    def to_str(self):
+        """Returns the string representation of the model"""
+        return pprint.pformat(self.to_dict())
+
+    def __eq__(self, other):
+        """Returns true if both objects are equal"""
+        if not isinstance(other, self.__class__):
+            return False
+
+        if not set(self._data_store.keys()) == set(other._data_store.keys()):
+            return False
+        for _var_name, this_val in self._data_store.items():
+            that_val = other._data_store[_var_name]
+            types = set()
+            types.add(this_val.__class__)
+            types.add(that_val.__class__)
+            vals_equal = this_val == that_val
+            if not vals_equal:
+                return False
+        return True
+
+
+class ModelComposed(OpenApiModel):
+    """the parent class of models whose type == object in their
+    swagger/openapi and have oneOf/allOf/anyOf
+
+    When one sets a property we use var_name_to_model_instances to store the value in
+    the correct class instances + run any type checking + validation code.
+    When one gets a property we use var_name_to_model_instances to get the value
+    from the correct class instances.
+    This allows multiple composed schemas to contain the same property with additive
+    constraints on the value.
+
+    _composed_schemas (dict) stores the anyOf/allOf/oneOf classes
+    key (str): allOf/oneOf/anyOf
+    value (list): the classes in the XOf definition.
+        Note: none_type can be included when the openapi document version >= 3.1.0
+    _composed_instances (list): stores a list of instances of the composed schemas
+    defined in _composed_schemas. When properties are accessed in the self instance,
+    they are returned from the self._data_store or the data stores in the instances
+    in self._composed_schemas
+    _var_name_to_model_instances (dict): maps between a variable name on self and
+    the composed instances (self included) which contain that data
+    key (str): property name
+    value (list): list of class instances, self or instances in _composed_instances
+    which contain the value that the key is referring to.
+    """
+
+    def __setitem__(self, name, value):
+        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
+        if name in self.required_properties:
+            self.__dict__[name] = value
+            return
+
+        """
+        Use cases:
+        1. additional_properties_type is None (additionalProperties == False in spec)
+            Check for property presence in self.openapi_types
+            if not present then throw an error
+            if present set in self, set attribute
+            always set on composed schemas
+        2.  additional_properties_type exists
+            set attribute on self
+            always set on composed schemas
+        """
+        if self.additional_properties_type is None:
+            """
+            For an attribute to exist on a composed schema it must:
+            - fulfill schema_requirements in the self composed schema not considering oneOf/anyOf/allOf schemas AND
+            - fulfill schema_requirements in each oneOf/anyOf/allOf schemas
+
+            schema_requirements:
+            For an attribute to exist on a schema it must:
+            - be present in properties at the schema OR
+            - have additionalProperties unset (defaults additionalProperties = any type) OR
+            - have additionalProperties set
+            """
+            if name not in self.openapi_types:
+                raise ApiAttributeError(
+                    "{0} has no attribute '{1}'".format(
+                        type(self).__name__, name),
+                    [e for e in [self._path_to_item, name] if e]
+                )
+        # attribute must be set on self and composed instances
+        self.set_attribute(name, value)
+        for model_instance in self._composed_instances:
+            setattr(model_instance, name, value)
+        if name not in self._var_name_to_model_instances:
+            # we assigned an additional property
+            self.__dict__['_var_name_to_model_instances'][name] = self._composed_instances + [self]
+        return None
+
+    __unset_attribute_value__ = object()
+
+    def get(self, name, default=None):
+        """returns the value of an attribute or some default value if the attribute was not set"""
+        if name in self.required_properties:
+            return self.__dict__[name]
+
+        # get the attribute from the correct instance
+        model_instances = self._var_name_to_model_instances.get(name)
+        values = []
+        # A composed model stores self and child (oneof/anyOf/allOf) models under
+        # self._var_name_to_model_instances.
+        # Any property must exist in self and all model instances
+        # The value stored in all model instances must be the same
+        if model_instances:
+            for model_instance in model_instances:
+                if name in model_instance._data_store:
+                    v = model_instance._data_store[name]
+                    if v not in values:
+                        values.append(v)
+        len_values = len(values)
+        if len_values == 0:
+            return default
+        elif len_values == 1:
+            return values[0]
+        elif len_values > 1:
+            raise ApiValueError(
+                "Values stored for property {0} in {1} differ when looking "
+                "at self and self's composed instances. All values must be "
+                "the same".format(name, type(self).__name__),
+                [e for e in [self._path_to_item, name] if e]
+            )
+
+    def __getitem__(self, name):
+        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
+        value = self.get(name, self.__unset_attribute_value__)
+        if value is self.__unset_attribute_value__:
+            raise ApiAttributeError(
+                "{0} has no attribute '{1}'".format(
+                    type(self).__name__, name),
+                    [e for e in [self._path_to_item, name] if e]
+            )
+        return value
+
+    def __contains__(self, name):
+        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
+
+        if name in self.required_properties:
+            return name in self.__dict__
+
+        model_instances = self._var_name_to_model_instances.get(
+            name, self._additional_properties_model_instances)
+
+        if model_instances:
+            for model_instance in model_instances:
+                if name in model_instance._data_store:
+                    return True
+
+        return False
+
+    def to_dict(self):
+        """Returns the model properties as a dict"""
+        return model_to_dict(self, serialize=False)
+
+    def to_str(self):
+        """Returns the string representation of the model"""
+        return pprint.pformat(self.to_dict())
+
+    def __eq__(self, other):
+        """Returns true if both objects are equal"""
+        if not isinstance(other, self.__class__):
+            return False
+
+        if not set(self._data_store.keys()) == set(other._data_store.keys()):
+            return False
+        for _var_name, this_val in self._data_store.items():
+            that_val = other._data_store[_var_name]
+            types = set()
+            types.add(this_val.__class__)
+            types.add(that_val.__class__)
+            vals_equal = this_val == that_val
+            if not vals_equal:
+                return False
+        return True
+
+
+COERCION_INDEX_BY_TYPE = {
+    ModelComposed: 0,
+    ModelNormal: 1,
+    ModelSimple: 2,
+    none_type: 3,    # The type of 'None'.
+    list: 4,
+    dict: 5,
+    float: 6,
+    int: 7,
+    bool: 8,
+    datetime: 9,
+    date: 10,
+    str: 11,
+    file_type: 12,   # 'file_type' is an alias for the built-in 'file' or 'io.IOBase' type.
+}
+
+# these are used to limit what type conversions we try to do
+# when we have a valid type already and we want to try converting
+# to another type
+UPCONVERSION_TYPE_PAIRS = (
+    (str, datetime),
+    (str, date),
+    # A float may be serialized as an integer, e.g. '3' is a valid serialized float.
+    (int, float),
+    (list, ModelComposed),
+    (dict, ModelComposed),
+    (str, ModelComposed),
+    (int, ModelComposed),
+    (float, ModelComposed),
+    (list, ModelComposed),
+    (list, ModelNormal),
+    (dict, ModelNormal),
+    (str, ModelSimple),
+    (int, ModelSimple),
+    (float, ModelSimple),
+    (list, ModelSimple),
+)
+
+COERCIBLE_TYPE_PAIRS = {
+    False: (  # client instantiation of a model with client data
+        # (dict, ModelComposed),
+        # (list, ModelComposed),
+        # (dict, ModelNormal),
+        # (list, ModelNormal),
+        # (str, ModelSimple),
+        # (int, ModelSimple),
+        # (float, ModelSimple),
+        # (list, ModelSimple),
+        # (str, int),
+        # (str, float),
+        # (str, datetime),
+        # (str, date),
+        # (int, str),
+        # (float, str),
+    ),
+    True: (  # server -> client data
+        (dict, ModelComposed),
+        (list, ModelComposed),
+        (dict, ModelNormal),
+        (list, ModelNormal),
+        (str, ModelSimple),
+        (int, ModelSimple),
+        (float, ModelSimple),
+        (list, ModelSimple),
+        # (str, int),
+        # (str, float),
+        (str, datetime),
+        (str, date),
+        # (int, str),
+        # (float, str),
+        (str, file_type)
+    ),
+}
+
+
+def get_simple_class(input_value):
+    """Returns an input_value's simple class that we will use for type checking
+    Python2:
+    float and int will return int, where int is the python3 int backport
+    str and unicode will return str, where str is the python3 str backport
+    Note: float and int ARE both instances of int backport
+    Note: str_py2 and unicode_py2 are NOT both instances of str backport
+
+    Args:
+        input_value (class/class_instance): the item for which we will return
+                                            the simple class
+    """
+    if isinstance(input_value, type):
+        # input_value is a class
+        return input_value
+    elif isinstance(input_value, tuple):
+        return tuple
+    elif isinstance(input_value, list):
+        return list
+    elif isinstance(input_value, dict):
+        return dict
+    elif isinstance(input_value, none_type):
+        return none_type
+    elif isinstance(input_value, file_type):
+        return file_type
+    elif isinstance(input_value, bool):
+        # this must be higher than the int check because
+        # isinstance(True, int) == True
+        return bool
+    elif isinstance(input_value, int):
+        return int
+    elif isinstance(input_value, datetime):
+        # this must be higher than the date check because
+        # isinstance(datetime_instance, date) == True
+        return datetime
+    elif isinstance(input_value, date):
+        return date
+    elif isinstance(input_value, str):
+        return str
+    return type(input_value)
+
+
+def check_allowed_values(allowed_values, input_variable_path, input_values):
+    """Raises an exception if the input_values are not allowed
+
+    Args:
+        allowed_values (dict): the allowed_values dict
+        input_variable_path (tuple): the path to the input variable
+        input_values (list/str/int/float/date/datetime): the values that we
+            are checking to see if they are in allowed_values
+    """
+    these_allowed_values = list(allowed_values[input_variable_path].values())
+    if (isinstance(input_values, list)
+            and not set(input_values).issubset(
+                set(these_allowed_values))):
+        invalid_values = ", ".join(
+            map(str, set(input_values) - set(these_allowed_values))),
+        raise ApiValueError(
+            "Invalid values for `%s` [%s], must be a subset of [%s]" %
+            (
+                input_variable_path[0],
+                invalid_values,
+                ", ".join(map(str, these_allowed_values))
+            )
+        )
+    elif (isinstance(input_values, dict)
+            and not set(
+                input_values.keys()).issubset(set(these_allowed_values))):
+        invalid_values = ", ".join(
+            map(str, set(input_values.keys()) - set(these_allowed_values)))
+        raise ApiValueError(
+            "Invalid keys in `%s` [%s], must be a subset of [%s]" %
+            (
+                input_variable_path[0],
+                invalid_values,
+                ", ".join(map(str, these_allowed_values))
+            )
+        )
+    elif (not isinstance(input_values, (list, dict))
+            and input_values not in these_allowed_values):
+        raise ApiValueError(
+            "Invalid value for `%s` (%s), must be one of %s" %
+            (
+                input_variable_path[0],
+                input_values,
+                these_allowed_values
+            )
+        )
+
+
+def is_json_validation_enabled(schema_keyword, configuration=None):
+    """Returns true if JSON schema validation is enabled for the specified
+    validation keyword. This can be used to skip JSON schema structural validation
+    as requested in the configuration.
+
+    Args:
+        schema_keyword (string): the name of a JSON schema validation keyword.
+        configuration (Configuration): the configuration class.
+    """
+
+    return (configuration is None or
+            not hasattr(configuration, '_disabled_client_side_validations') or
+            schema_keyword not in configuration._disabled_client_side_validations)
+
+
+def check_validations(
+        validations, input_variable_path, input_values,
+        configuration=None):
+    """Raises an exception if the input_values are invalid
+
+    Args:
+        validations (dict): the validation dictionary.
+        input_variable_path (tuple): the path to the input variable.
+        input_values (list/str/int/float/date/datetime): the values that we
+            are checking.
+        configuration (Configuration): the configuration class.
+    """
+
+    if input_values is None:
+        return
+
+    current_validations = validations[input_variable_path]
+    if (is_json_validation_enabled('multipleOf', configuration) and
+            'multiple_of' in current_validations and
+            isinstance(input_values, (int, float)) and
+            not (float(input_values) / current_validations['multiple_of']).is_integer()):
+        # Note 'multipleOf' will be as good as the floating point arithmetic.
+        raise ApiValueError(
+            "Invalid value for `%s`, value must be a multiple of "
+            "`%s`" % (
+                input_variable_path[0],
+                current_validations['multiple_of']
+            )
+        )
+
+    if (is_json_validation_enabled('maxLength', configuration) and
+            'max_length' in current_validations and
+            len(input_values) > current_validations['max_length']):
+        raise ApiValueError(
+            "Invalid value for `%s`, length must be less than or equal to "
+            "`%s`" % (
+                input_variable_path[0],
+                current_validations['max_length']
+            )
+        )
+
+    if (is_json_validation_enabled('minLength', configuration) and
+            'min_length' in current_validations and
+            len(input_values) < current_validations['min_length']):
+        raise ApiValueError(
+            "Invalid value for `%s`, length must be greater than or equal to "
+            "`%s`" % (
+                input_variable_path[0],
+                current_validations['min_length']
+            )
+        )
+
+    if (is_json_validation_enabled('maxItems', configuration) and
+            'max_items' in current_validations and
+            len(input_values) > current_validations['max_items']):
+        raise ApiValueError(
+            "Invalid value for `%s`, number of items must be less than or "
+            "equal to `%s`" % (
+                input_variable_path[0],
+                current_validations['max_items']
+            )
+        )
+
+    if (is_json_validation_enabled('minItems', configuration) and
+            'min_items' in current_validations and
+            len(input_values) < current_validations['min_items']):
+        raise ValueError(
+            "Invalid value for `%s`, number of items must be greater than or "
+            "equal to `%s`" % (
+                input_variable_path[0],
+                current_validations['min_items']
+            )
+        )
+
+    items = ('exclusive_maximum', 'inclusive_maximum', 'exclusive_minimum',
+             'inclusive_minimum')
+    if (any(item in current_validations for item in items)):
+        if isinstance(input_values, list):
+            max_val = max(input_values)
+            min_val = min(input_values)
+        elif isinstance(input_values, dict):
+            max_val = max(input_values.values())
+            min_val = min(input_values.values())
+        else:
+            max_val = input_values
+            min_val = input_values
+
+    if (is_json_validation_enabled('exclusiveMaximum', configuration) and
+            'exclusive_maximum' in current_validations and
+            max_val >= current_validations['exclusive_maximum']):
+        raise ApiValueError(
+            "Invalid value for `%s`, must be a value less than `%s`" % (
+                input_variable_path[0],
+                current_validations['exclusive_maximum']
+            )
+        )
+
+    if (is_json_validation_enabled('maximum', configuration) and
+            'inclusive_maximum' in current_validations and
+            max_val > current_validations['inclusive_maximum']):
+        raise ApiValueError(
+            "Invalid value for `%s`, must be a value less than or equal to "
+            "`%s`" % (
+                input_variable_path[0],
+                current_validations['inclusive_maximum']
+            )
+        )
+
+    if (is_json_validation_enabled('exclusiveMinimum', configuration) and
+            'exclusive_minimum' in current_validations and
+            min_val <= current_validations['exclusive_minimum']):
+        raise ApiValueError(
+            "Invalid value for `%s`, must be a value greater than `%s`" %
+            (
+                input_variable_path[0],
+                current_validations['exclusive_maximum']
+            )
+        )
+
+    if (is_json_validation_enabled('minimum', configuration) and
+            'inclusive_minimum' in current_validations and
+            min_val < current_validations['inclusive_minimum']):
+        raise ApiValueError(
+            "Invalid value for `%s`, must be a value greater than or equal "
+            "to `%s`" % (
+                input_variable_path[0],
+                current_validations['inclusive_minimum']
+            )
+        )
+    flags = current_validations.get('regex', {}).get('flags', 0)
+    if (is_json_validation_enabled('pattern', configuration) and
+            'regex' in current_validations and
+            not re.search(current_validations['regex']['pattern'],
+                          input_values, flags=flags)):
+        err_msg = r"Invalid value for `%s`, must match regular expression `%s`" % (
+            input_variable_path[0],
+            current_validations['regex']['pattern']
+        )
+        if flags != 0:
+            # Don't print the regex flags if the flags are not
+            # specified in the OAS document.
+            err_msg = r"%s with flags=`%s`" % (err_msg, flags)
+        raise ApiValueError(err_msg)
+
+
+def order_response_types(required_types):
+    """Returns the required types sorted in coercion order
+
+    Args:
+        required_types (list/tuple): collection of classes or instance of
+            list or dict with class information inside it.
+
+    Returns:
+        (list): coercion order sorted collection of classes or instance
+            of list or dict with class information inside it.
+    """
+
+    def index_getter(class_or_instance):
+        if isinstance(class_or_instance, list):
+            return COERCION_INDEX_BY_TYPE[list]
+        elif isinstance(class_or_instance, dict):
+            return COERCION_INDEX_BY_TYPE[dict]
+        elif (inspect.isclass(class_or_instance)
+                and issubclass(class_or_instance, ModelComposed)):
+            return COERCION_INDEX_BY_TYPE[ModelComposed]
+        elif (inspect.isclass(class_or_instance)
+                and issubclass(class_or_instance, ModelNormal)):
+            return COERCION_INDEX_BY_TYPE[ModelNormal]
+        elif (inspect.isclass(class_or_instance)
+                and issubclass(class_or_instance, ModelSimple)):
+            return COERCION_INDEX_BY_TYPE[ModelSimple]
+        elif class_or_instance in COERCION_INDEX_BY_TYPE:
+            return COERCION_INDEX_BY_TYPE[class_or_instance]
+        raise ApiValueError("Unsupported type: %s" % class_or_instance)
+
+    sorted_types = sorted(
+        required_types,
+        key=lambda class_or_instance: index_getter(class_or_instance)
+    )
+    return sorted_types
+
+
+def remove_uncoercible(required_types_classes, current_item, spec_property_naming,
+                       must_convert=True):
+    """Only keeps the type conversions that are possible
+
+    Args:
+        required_types_classes (tuple): tuple of classes that are required
+                          these should be ordered by COERCION_INDEX_BY_TYPE
+        spec_property_naming (bool): True if the variable names in the input
+            data are serialized names as specified in the OpenAPI document.
+            False if the variables names in the input data are python
+            variable names in PEP-8 snake case.
+        current_item (any): the current item (input data) to be converted
+
+    Keyword Args:
+        must_convert (bool): if True the item to convert is of the wrong
+                          type and we want a big list of coercibles
+                          if False, we want a limited list of coercibles
+
+    Returns:
+        (list): the remaining coercible required types, classes only
+    """
+    current_type_simple = get_simple_class(current_item)
+
+    results_classes = []
+    for required_type_class in required_types_classes:
+        # convert our models to OpenApiModel
+        required_type_class_simplified = required_type_class
+        if isinstance(required_type_class_simplified, type):
+            if issubclass(required_type_class_simplified, ModelComposed):
+                required_type_class_simplified = ModelComposed
+            elif issubclass(required_type_class_simplified, ModelNormal):
+                required_type_class_simplified = ModelNormal
+            elif issubclass(required_type_class_simplified, ModelSimple):
+                required_type_class_simplified = ModelSimple
+
+        if required_type_class_simplified == current_type_simple:
+            # don't consider converting to one's own class
+            continue
+
+        class_pair = (current_type_simple, required_type_class_simplified)
+        if must_convert and class_pair in COERCIBLE_TYPE_PAIRS[spec_property_naming]:
+            results_classes.append(required_type_class)
+        elif class_pair in UPCONVERSION_TYPE_PAIRS:
+            results_classes.append(required_type_class)
+    return results_classes
+
+
+def get_discriminated_classes(cls):
+    """
+    Returns all the classes that a discriminator converts to
+    TODO: lru_cache this
+    """
+    possible_classes = []
+    key = list(cls.discriminator.keys())[0]
+    if is_type_nullable(cls):
+        possible_classes.append(cls)
+    for discr_cls in cls.discriminator[key].values():
+        if hasattr(discr_cls, 'discriminator') and discr_cls.discriminator is not None:
+            possible_classes.extend(get_discriminated_classes(discr_cls))
+        else:
+            possible_classes.append(discr_cls)
+    return possible_classes
+
+
+def get_possible_classes(cls, from_server_context):
+    # TODO: lru_cache this
+    possible_classes = [cls]
+    if from_server_context:
+        return possible_classes
+    if hasattr(cls, 'discriminator') and cls.discriminator is not None:
+        possible_classes = []
+        possible_classes.extend(get_discriminated_classes(cls))
+    elif issubclass(cls, ModelComposed):
+        possible_classes.extend(composed_model_input_classes(cls))
+    return possible_classes
+
+
+def get_required_type_classes(required_types_mixed, spec_property_naming):
+    """Converts the tuple required_types into a tuple and a dict described
+    below
+
+    Args:
+        required_types_mixed (tuple/list): will contain either classes or
+            instance of list or dict
+        spec_property_naming (bool): if True these values came from the
+            server, and we use the data types in our endpoints.
+            If False, we are client side and we need to include
+            oneOf and discriminator classes inside the data types in our endpoints
+
+    Returns:
+        (valid_classes, dict_valid_class_to_child_types_mixed):
+            valid_classes (tuple): the valid classes that the current item
+                                   should be
+            dict_valid_class_to_child_types_mixed (dict):
+                valid_class (class): this is the key
+                child_types_mixed (list/dict/tuple): describes the valid child
+                    types
+    """
+    valid_classes = []
+    child_req_types_by_current_type = {}
+    for required_type in required_types_mixed:
+        if isinstance(required_type, list):
+            valid_classes.append(list)
+            child_req_types_by_current_type[list] = required_type
+        elif isinstance(required_type, tuple):
+            valid_classes.append(tuple)
+            child_req_types_by_current_type[tuple] = required_type
+        elif isinstance(required_type, dict):
+            valid_classes.append(dict)
+            child_req_types_by_current_type[dict] = required_type[str]
+        else:
+            valid_classes.extend(get_possible_classes(required_type, spec_property_naming))
+    return tuple(valid_classes), child_req_types_by_current_type
+
+
+def change_keys_js_to_python(input_dict, model_class):
+    """
+    Converts from javascript_key keys in the input_dict to python_keys in
+    the output dict using the mapping in model_class.
+    If the input_dict contains a key which does not declared in the model_class,
+    the key is added to the output dict as is. The assumption is the model_class
+    may have undeclared properties (additionalProperties attribute in the OAS
+    document).
+    """
+
+    if getattr(model_class, 'attribute_map', None) is None:
+        return input_dict
+    output_dict = {}
+    reversed_attr_map = {value: key for key, value in
+                         model_class.attribute_map.items()}
+    for javascript_key, value in input_dict.items():
+        python_key = reversed_attr_map.get(javascript_key)
+        if python_key is None:
+            # if the key is unknown, it is in error or it is an
+            # additionalProperties variable
+            python_key = javascript_key
+        output_dict[python_key] = value
+    return output_dict
+
+
+def get_type_error(var_value, path_to_item, valid_classes, key_type=False):
+    error_msg = type_error_message(
+        var_name=path_to_item[-1],
+        var_value=var_value,
+        valid_classes=valid_classes,
+        key_type=key_type
+    )
+    return ApiTypeError(
+        error_msg,
+        path_to_item=path_to_item,
+        valid_classes=valid_classes,
+        key_type=key_type
+    )
+
+
+def deserialize_primitive(data, klass, path_to_item):
+    """Deserializes string to primitive type.
+
+    :param data: str/int/float
+    :param klass: str/class the class to convert to
+
+    :return: int, float, str, bool, date, datetime
+    """
+    additional_message = ""
+    try:
+        if klass in {datetime, date}:
+            additional_message = (
+                "If you need your parameter to have a fallback "
+                "string value, please set its type as `type: {}` in your "
+                "spec. That allows the value to be any type. "
+            )
+            if klass == datetime:
+                if len(data) < 8:
+                    raise ValueError("This is not a datetime")
+                # The string should be in iso8601 datetime format.
+                parsed_datetime = parse(data)
+                date_only = (
+                    parsed_datetime.hour == 0 and
+                    parsed_datetime.minute == 0 and
+                    parsed_datetime.second == 0 and
+                    parsed_datetime.tzinfo is None and
+                    8 <= len(data) <= 10
+                )
+                if date_only:
+                    raise ValueError("This is a date, not a datetime")
+                return parsed_datetime
+            elif klass == date:
+                if len(data) < 8:
+                    raise ValueError("This is not a date")
+                return parse(data).date()
+        else:
+            converted_value = klass(data)
+            if isinstance(data, str) and klass == float:
+                if str(converted_value) != data:
+                    # '7' -> 7.0 -> '7.0' != '7'
+                    raise ValueError('This is not a float')
+            return converted_value
+    except (OverflowError, ValueError) as ex:
+        # parse can raise OverflowError
+        raise ApiValueError(
+            "{0}Failed to parse {1} as {2}".format(
+                additional_message, repr(data), klass.__name__
+            ),
+            path_to_item=path_to_item
+        ) from ex
+
+
+def get_discriminator_class(model_class,
+                            discr_name,
+                            discr_value, cls_visited):
+    """Returns the child class specified by the discriminator.
+
+    Args:
+        model_class (OpenApiModel): the model class.
+        discr_name (string): the name of the discriminator property.
+        discr_value (any): the discriminator value.
+        cls_visited (list): list of model classes that have been visited.
+            Used to determine the discriminator class without
+            visiting circular references indefinitely.
+
+    Returns:
+        used_model_class (class/None): the chosen child class that will be used
+            to deserialize the data, for example dog.Dog.
+            If a class is not found, None is returned.
+    """
+
+    if model_class in cls_visited:
+        # The class has already been visited and no suitable class was found.
+        return None
+    cls_visited.append(model_class)
+    used_model_class = None
+    if discr_name in model_class.discriminator:
+        class_name_to_discr_class = model_class.discriminator[discr_name]
+        used_model_class = class_name_to_discr_class.get(discr_value)
+    if used_model_class is None:
+        # We didn't find a discriminated class in class_name_to_discr_class.
+        # So look in the ancestor or descendant discriminators
+        # The discriminator mapping may exist in a descendant (anyOf, oneOf)
+        # or ancestor (allOf).
+        # Ancestor example: in the GrandparentAnimal -> ParentPet -> ChildCat
+        #   hierarchy, the discriminator mappings may be defined at any level
+        #   in the hierarchy.
+        # Descendant example:  mammal -> whale/zebra/Pig -> BasquePig/DanishPig
+        #   if we try to make BasquePig from mammal, we need to travel through
+        #   the oneOf descendant discriminators to find BasquePig
+        descendant_classes = model_class._composed_schemas.get('oneOf', ()) + \
+            model_class._composed_schemas.get('anyOf', ())
+        ancestor_classes = model_class._composed_schemas.get('allOf', ())
+        possible_classes = descendant_classes + ancestor_classes
+        for cls in possible_classes:
+            # Check if the schema has inherited discriminators.
+            if hasattr(cls, 'discriminator') and cls.discriminator is not None:
+                used_model_class = get_discriminator_class(
+                    cls, discr_name, discr_value, cls_visited)
+                if used_model_class is not None:
+                    return used_model_class
+    return used_model_class
+
+
+def deserialize_model(model_data, model_class, path_to_item, check_type,
+                      configuration, spec_property_naming):
+    """Deserializes model_data to model instance.
+
+    Args:
+        model_data (int/str/float/bool/none_type/list/dict): data to instantiate the model
+        model_class (OpenApiModel): the model class
+        path_to_item (list): path to the model in the received data
+        check_type (bool): whether to check the data tupe for the values in
+            the model
+        configuration (Configuration): the instance to use to convert files
+        spec_property_naming (bool): True if the variable names in the input
+            data are serialized names as specified in the OpenAPI document.
+            False if the variables names in the input data are python
+            variable names in PEP-8 snake case.
+
+    Returns:
+        model instance
+
+    Raise:
+        ApiTypeError
+        ApiValueError
+        ApiKeyError
+    """
+
+    kw_args = dict(_check_type=check_type,
+                   _path_to_item=path_to_item,
+                   _configuration=configuration,
+                   _spec_property_naming=spec_property_naming)
+
+    if issubclass(model_class, ModelSimple):
+        return model_class._new_from_openapi_data(model_data, **kw_args)
+    elif isinstance(model_data, list):
+        return model_class._new_from_openapi_data(*model_data, **kw_args)
+    if isinstance(model_data, dict):
+        kw_args.update(model_data)
+        return model_class._new_from_openapi_data(**kw_args)
+    elif isinstance(model_data, PRIMITIVE_TYPES):
+        return model_class._new_from_openapi_data(model_data, **kw_args)
+
+
+def deserialize_file(response_data, configuration, content_disposition=None):
+    """Deserializes body to file
+
+    Saves response body into a file in a temporary folder,
+    using the filename from the `Content-Disposition` header if provided.
+
+    Args:
+        param response_data (str):  the file data to write
+        configuration (Configuration): the instance to use to convert files
+
+    Keyword Args:
+        content_disposition (str):  the value of the Content-Disposition
+            header
+
+    Returns:
+        (file_type): the deserialized file which is open
+            The user is responsible for closing and reading the file
+    """
+    fd, path = tempfile.mkstemp(dir=configuration.temp_folder_path)
+    os.close(fd)
+    os.remove(path)
+
+    if content_disposition:
+        filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?',
+                             content_disposition,
+                             flags=re.I)
+        if filename is not None:
+            filename = filename.group(1)
+        else:
+            filename = "default_" + str(uuid.uuid4())
+
+        path = os.path.join(os.path.dirname(path), filename)
+
+    with open(path, "wb") as f:
+        if isinstance(response_data, str):
+            # change str to bytes so we can write it
+            response_data = response_data.encode('utf-8')
+        f.write(response_data)
+
+    f = open(path, "rb")
+    return f
+
+
+def attempt_convert_item(input_value, valid_classes, path_to_item,
+                         configuration, spec_property_naming, key_type=False,
+                         must_convert=False, check_type=True):
+    """
+    Args:
+        input_value (any): the data to convert
+        valid_classes (any): the classes that are valid
+        path_to_item (list): the path to the item to convert
+        configuration (Configuration): the instance to use to convert files
+        spec_property_naming (bool): True if the variable names in the input
+            data are serialized names as specified in the OpenAPI document.
+            False if the variables names in the input data are python
+            variable names in PEP-8 snake case.
+        key_type (bool): if True we need to convert a key type (not supported)
+        must_convert (bool): if True we must convert
+        check_type (bool): if True we check the type or the returned data in
+            ModelComposed/ModelNormal/ModelSimple instances
+
+    Returns:
+        instance (any) the fixed item
+
+    Raises:
+        ApiTypeError
+        ApiValueError
+        ApiKeyError
+    """
+    valid_classes_ordered = order_response_types(valid_classes)
+    valid_classes_coercible = remove_uncoercible(
+        valid_classes_ordered, input_value, spec_property_naming)
+    if not valid_classes_coercible or key_type:
+        # we do not handle keytype errors, json will take care
+        # of this for us
+        if configuration is None or not configuration.discard_unknown_keys:
+            raise get_type_error(input_value, path_to_item, valid_classes,
+                                 key_type=key_type)
+    for valid_class in valid_classes_coercible:
+        try:
+            if issubclass(valid_class, OpenApiModel):
+                return deserialize_model(input_value, valid_class,
+                                         path_to_item, check_type,
+                                         configuration, spec_property_naming)
+            elif valid_class == file_type:
+                return deserialize_file(input_value, configuration)
+            return deserialize_primitive(input_value, valid_class,
+                                         path_to_item)
+        except (ApiTypeError, ApiValueError, ApiKeyError) as conversion_exc:
+            if must_convert:
+                raise conversion_exc
+            # if we have conversion errors when must_convert == False
+            # we ignore the exception and move on to the next class
+            continue
+    # we were unable to convert, must_convert == False
+    return input_value
+
+
+def is_type_nullable(input_type):
+    """
+    Returns true if None is an allowed value for the specified input_type.
+
+    A type is nullable if at least one of the following conditions is true:
+    1. The OAS 'nullable' attribute has been specified,
+    1. The type is the 'null' type,
+    1. The type is a anyOf/oneOf composed schema, and a child schema is
+       the 'null' type.
+    Args:
+        input_type (type): the class of the input_value that we are
+            checking
+    Returns:
+        bool
+    """
+    if input_type is none_type:
+        return True
+    if issubclass(input_type, OpenApiModel) and input_type._nullable:
+        return True
+    if issubclass(input_type, ModelComposed):
+        # If oneOf/anyOf, check if the 'null' type is one of the allowed types.
+        for t in input_type._composed_schemas.get('oneOf', ()):
+            if is_type_nullable(t):
+                return True
+        for t in input_type._composed_schemas.get('anyOf', ()):
+            if is_type_nullable(t):
+                return True
+    return False
+
+
+def is_valid_type(input_class_simple, valid_classes):
+    """
+    Args:
+        input_class_simple (class): the class of the input_value that we are
+            checking
+        valid_classes (tuple): the valid classes that the current item
+            should be
+    Returns:
+        bool
+    """
+    if issubclass(input_class_simple, OpenApiModel) and \
+            valid_classes == (bool, date, datetime, dict, float, int, list, str, none_type,):
+        return True
+    valid_type = input_class_simple in valid_classes
+    if not valid_type and (
+            issubclass(input_class_simple, OpenApiModel) or
+            input_class_simple is none_type):
+        for valid_class in valid_classes:
+            if input_class_simple is none_type and is_type_nullable(valid_class):
+                # Schema is oneOf/anyOf and the 'null' type is one of the allowed types.
+                return True
+            if not (issubclass(valid_class, OpenApiModel) and valid_class.discriminator):
+                continue
+            discr_propertyname_py = list(valid_class.discriminator.keys())[0]
+            discriminator_classes = (
+                valid_class.discriminator[discr_propertyname_py].values()
+            )
+            valid_type = is_valid_type(input_class_simple, discriminator_classes)
+            if valid_type:
+                return True
+    return valid_type
+
+
+def validate_and_convert_types(input_value, required_types_mixed, path_to_item,
+                               spec_property_naming, _check_type, configuration=None):
+    """Raises a TypeError is there is a problem, otherwise returns value
+
+    Args:
+        input_value (any): the data to validate/convert
+        required_types_mixed (list/dict/tuple): A list of
+            valid classes, or a list tuples of valid classes, or a dict where
+            the value is a tuple of value classes
+        path_to_item: (list) the path to the data being validated
+            this stores a list of keys or indices to get to the data being
+            validated
+        spec_property_naming (bool): True if the variable names in the input
+            data are serialized names as specified in the OpenAPI document.
+            False if the variables names in the input data are python
+            variable names in PEP-8 snake case.
+        _check_type: (boolean) if true, type will be checked and conversion
+            will be attempted.
+        configuration: (Configuration): the configuration class to use
+            when converting file_type items.
+            If passed, conversion will be attempted when possible
+            If not passed, no conversions will be attempted and
+            exceptions will be raised
+
+    Returns:
+        the correctly typed value
+
+    Raises:
+        ApiTypeError
+    """
+    results = get_required_type_classes(required_types_mixed, spec_property_naming)
+    valid_classes, child_req_types_by_current_type = results
+
+    input_class_simple = get_simple_class(input_value)
+    valid_type = is_valid_type(input_class_simple, valid_classes)
+    if not valid_type:
+        if (configuration
+                or (input_class_simple == dict
+                    and dict not in valid_classes)):
+            # if input_value is not valid_type try to convert it
+            converted_instance = attempt_convert_item(
+                input_value,
+                valid_classes,
+                path_to_item,
+                configuration,
+                spec_property_naming,
+                key_type=False,
+                must_convert=True,
+                check_type=_check_type
+            )
+            return converted_instance
+        else:
+            raise get_type_error(input_value, path_to_item, valid_classes,
+                                 key_type=False)
+
+    # input_value's type is in valid_classes
+    if len(valid_classes) > 1 and configuration:
+        # there are valid classes which are not the current class
+        valid_classes_coercible = remove_uncoercible(
+            valid_classes, input_value, spec_property_naming, must_convert=False)
+        if valid_classes_coercible:
+            converted_instance = attempt_convert_item(
+                input_value,
+                valid_classes_coercible,
+                path_to_item,
+                configuration,
+                spec_property_naming,
+                key_type=False,
+                must_convert=False,
+                check_type=_check_type
+            )
+            return converted_instance
+
+    if child_req_types_by_current_type == {}:
+        # all types are of the required types and there are no more inner
+        # variables left to look at
+        return input_value
+    inner_required_types = child_req_types_by_current_type.get(
+        type(input_value)
+    )
+    if inner_required_types is None:
+        # for this type, there are not more inner variables left to look at
+        return input_value
+    if isinstance(input_value, list):
+        if input_value == []:
+            # allow an empty list
+            return input_value
+        for index, inner_value in enumerate(input_value):
+            inner_path = list(path_to_item)
+            inner_path.append(index)
+            input_value[index] = validate_and_convert_types(
+                inner_value,
+                inner_required_types,
+                inner_path,
+                spec_property_naming,
+                _check_type,
+                configuration=configuration
+            )
+    elif isinstance(input_value, dict):
+        if input_value == {}:
+            # allow an empty dict
+            return input_value
+        for inner_key, inner_val in input_value.items():
+            inner_path = list(path_to_item)
+            inner_path.append(inner_key)
+            if get_simple_class(inner_key) != str:
+                raise get_type_error(inner_key, inner_path, valid_classes,
+                                     key_type=True)
+            input_value[inner_key] = validate_and_convert_types(
+                inner_val,
+                inner_required_types,
+                inner_path,
+                spec_property_naming,
+                _check_type,
+                configuration=configuration
+            )
+    return input_value
+
+
+def model_to_dict(model_instance, serialize=True):
+    """Returns the model properties as a dict
+
+    Args:
+        model_instance (one of your model instances): the model instance that
+            will be converted to a dict.
+
+    Keyword Args:
+        serialize (bool): if True, the keys in the dict will be values from
+            attribute_map
+    """
+    result = {}
+
+    def extract_item(item): return (
+        item[0], model_to_dict(
+            item[1], serialize=serialize)) if hasattr(
+        item[1], '_data_store') else item
+
+    model_instances = [model_instance]
+    if model_instance._composed_schemas:
+        model_instances.extend(model_instance._composed_instances)
+    seen_json_attribute_names = set()
+    used_fallback_python_attribute_names = set()
+    py_to_json_map = {}
+    for model_instance in model_instances:
+        for attr, value in model_instance._data_store.items():
+            if serialize:
+                # we use get here because additional property key names do not
+                # exist in attribute_map
+                try:
+                    attr = model_instance.attribute_map[attr]
+                    py_to_json_map.update(model_instance.attribute_map)
+                    seen_json_attribute_names.add(attr)
+                except KeyError:
+                    used_fallback_python_attribute_names.add(attr)
+            if isinstance(value, list):
+                if not value:
+                    # empty list or None
+                    result[attr] = value
+                else:
+                    res = []
+                    for v in value:
+                        if isinstance(v, PRIMITIVE_TYPES) or v is None:
+                            res.append(v)
+                        elif isinstance(v, ModelSimple):
+                            res.append(v.value)
+                        elif isinstance(v, dict):
+                            res.append(dict(map(
+                                extract_item,
+                                v.items()
+                            )))
+                        else:
+                            res.append(model_to_dict(v, serialize=serialize))
+                    result[attr] = res
+            elif isinstance(value, dict):
+                result[attr] = dict(map(
+                    extract_item,
+                    value.items()
+                ))
+            elif isinstance(value, ModelSimple):
+                result[attr] = value.value
+            elif hasattr(value, '_data_store'):
+                result[attr] = model_to_dict(value, serialize=serialize)
+            else:
+                result[attr] = value
+    if serialize:
+        for python_key in used_fallback_python_attribute_names:
+            json_key = py_to_json_map.get(python_key)
+            if json_key is None:
+                continue
+            if python_key == json_key:
+                continue
+            json_key_assigned_no_need_for_python_key = json_key in seen_json_attribute_names
+            if json_key_assigned_no_need_for_python_key:
+                del result[python_key]
+
+    return result
+
+
+def type_error_message(var_value=None, var_name=None, valid_classes=None,
+                       key_type=None):
+    """
+    Keyword Args:
+        var_value (any): the variable which has the type_error
+        var_name (str): the name of the variable which has the typ error
+        valid_classes (tuple): the accepted classes for current_item's
+                                  value
+        key_type (bool): False if our value is a value in a dict
+                         True if it is a key in a dict
+                         False if our item is an item in a list
+    """
+    key_or_value = 'value'
+    if key_type:
+        key_or_value = 'key'
+    valid_classes_phrase = get_valid_classes_phrase(valid_classes)
+    msg = (
+        "Invalid type for variable '{0}'. Required {1} type {2} and "
+        "passed type was {3}".format(
+            var_name,
+            key_or_value,
+            valid_classes_phrase,
+            type(var_value).__name__,
+        )
+    )
+    return msg
+
+
+def get_valid_classes_phrase(input_classes):
+    """Returns a string phrase describing what types are allowed
+    """
+    all_classes = list(input_classes)
+    all_classes = sorted(all_classes, key=lambda cls: cls.__name__)
+    all_class_names = [cls.__name__ for cls in all_classes]
+    if len(all_class_names) == 1:
+        return 'is {0}'.format(all_class_names[0])
+    return "is one of [{0}]".format(", ".join(all_class_names))
+
+
+def get_allof_instances(self, model_args, constant_args):
+    """
+    Args:
+        self: the class we are handling
+        model_args (dict): var_name to var_value
+            used to make instances
+        constant_args (dict):
+            metadata arguments:
+            _check_type
+            _path_to_item
+            _spec_property_naming
+            _configuration
+            _visited_composed_classes
+
+    Returns
+        composed_instances (list)
+    """
+    composed_instances = []
+    for allof_class in self._composed_schemas['allOf']:
+
+        try:
+            if constant_args.get('_spec_property_naming'):
+                allof_instance = allof_class._from_openapi_data(**model_args, **constant_args)
+            else:
+                allof_instance = allof_class(**model_args, **constant_args)
+            composed_instances.append(allof_instance)
+        except Exception as ex:
+            raise ApiValueError(
+                "Invalid inputs given to generate an instance of '%s'. The "
+                "input data was invalid for the allOf schema '%s' in the composed "
+                "schema '%s'. Error=%s" % (
+                    allof_class.__name__,
+                    allof_class.__name__,
+                    self.__class__.__name__,
+                    str(ex)
+                )
+            ) from ex
+    return composed_instances
+
+
+def get_oneof_instance(cls, model_kwargs, constant_kwargs, model_arg=None):
+    """
+    Find the oneOf schema that matches the input data (e.g. payload).
+    If exactly one schema matches the input data, an instance of that schema
+    is returned.
+    If zero or more than one schema match the input data, an exception is raised.
+    In OAS 3.x, the payload MUST, by validation, match exactly one of the
+    schemas described by oneOf.
+
+    Args:
+        cls: the class we are handling
+        model_kwargs (dict): var_name to var_value
+            The input data, e.g. the payload that must match a oneOf schema
+            in the OpenAPI document.
+        constant_kwargs (dict): var_name to var_value
+            args that every model requires, including configuration, server
+            and path to item.
+
+    Kwargs:
+        model_arg: (int, float, bool, str, date, datetime, ModelSimple, None):
+            the value to assign to a primitive class or ModelSimple class
+            Notes:
+            - this is only passed in when oneOf includes types which are not object
+            - None is used to suppress handling of model_arg, nullable models are handled in __new__
+
+    Returns
+        oneof_instance (instance)
+    """
+    if len(cls._composed_schemas['oneOf']) == 0:
+        return None
+
+    oneof_instances = []
+    # Iterate over each oneOf schema and determine if the input data
+    # matches the oneOf schemas.
+    for oneof_class in cls._composed_schemas['oneOf']:
+        # The composed oneOf schema allows the 'null' type and the input data
+        # is the null value. This is a OAS >= 3.1 feature.
+        if oneof_class is none_type:
+            # skip none_types because we are deserializing dict data.
+            # none_type deserialization is handled in the __new__ method
+            continue
+
+        single_value_input = allows_single_value_input(oneof_class)
+
+        try:
+            if not single_value_input:
+                if constant_kwargs.get('_spec_property_naming'):
+                    oneof_instance = oneof_class._from_openapi_data(
+                        **model_kwargs, **constant_kwargs)
+                else:
+                    oneof_instance = oneof_class(**model_kwargs, **constant_kwargs)
+            else:
+                if issubclass(oneof_class, ModelSimple):
+                    if constant_kwargs.get('_spec_property_naming'):
+                        oneof_instance = oneof_class._from_openapi_data(
+                            model_arg, **constant_kwargs)
+                    else:
+                        oneof_instance = oneof_class(model_arg, **constant_kwargs)
+                elif oneof_class in PRIMITIVE_TYPES:
+                    oneof_instance = validate_and_convert_types(
+                        model_arg,
+                        (oneof_class,),
+                        constant_kwargs['_path_to_item'],
+                        constant_kwargs['_spec_property_naming'],
+                        constant_kwargs['_check_type'],
+                        configuration=constant_kwargs['_configuration']
+                    )
+            oneof_instances.append(oneof_instance)
+        except Exception:
+            pass
+    if len(oneof_instances) == 0:
+        raise ApiValueError(
+            "Invalid inputs given to generate an instance of %s. None "
+            "of the oneOf schemas matched the input data." %
+            cls.__name__
+        )
+    elif len(oneof_instances) > 1:
+        raise ApiValueError(
+            "Invalid inputs given to generate an instance of %s. Multiple "
+            "oneOf schemas matched the inputs, but a max of one is allowed." %
+            cls.__name__
+        )
+    return oneof_instances[0]
+
+
+def get_anyof_instances(self, model_args, constant_args):
+    """
+    Args:
+        self: the class we are handling
+        model_args (dict): var_name to var_value
+            The input data, e.g. the payload that must match at least one
+            anyOf child schema in the OpenAPI document.
+        constant_args (dict): var_name to var_value
+            args that every model requires, including configuration, server
+            and path to item.
+
+    Returns
+        anyof_instances (list)
+    """
+    anyof_instances = []
+    if len(self._composed_schemas['anyOf']) == 0:
+        return anyof_instances
+
+    for anyof_class in self._composed_schemas['anyOf']:
+        # The composed oneOf schema allows the 'null' type and the input data
+        # is the null value. This is a OAS >= 3.1 feature.
+        if anyof_class is none_type:
+            # skip none_types because we are deserializing dict data.
+            # none_type deserialization is handled in the __new__ method
+            continue
+
+        try:
+            if constant_args.get('_spec_property_naming'):
+                anyof_instance = anyof_class._from_openapi_data(**model_args, **constant_args)
+            else:
+                anyof_instance = anyof_class(**model_args, **constant_args)
+            anyof_instances.append(anyof_instance)
+        except Exception:
+            pass
+    if len(anyof_instances) == 0:
+        raise ApiValueError(
+            "Invalid inputs given to generate an instance of %s. None of the "
+            "anyOf schemas matched the inputs." %
+            self.__class__.__name__
+        )
+    return anyof_instances
+
+
+def get_discarded_args(self, composed_instances, model_args):
+    """
+    Gathers the args that were discarded by configuration.discard_unknown_keys
+    """
+    model_arg_keys = model_args.keys()
+    discarded_args = set()
+    # arguments passed to self were already converted to python names
+    # before __init__ was called
+    for instance in composed_instances:
+        if instance.__class__ in self._composed_schemas['allOf']:
+            try:
+                keys = instance.to_dict().keys()
+                discarded_keys = model_args - keys
+                discarded_args.update(discarded_keys)
+            except Exception:
+                # allOf integer schema will throw exception
+                pass
+        else:
+            try:
+                all_keys = set(model_to_dict(instance, serialize=False).keys())
+                js_keys = model_to_dict(instance, serialize=True).keys()
+                all_keys.update(js_keys)
+                discarded_keys = model_arg_keys - all_keys
+                discarded_args.update(discarded_keys)
+            except Exception:
+                # allOf integer schema will throw exception
+                pass
+    return discarded_args
+
+
+def validate_get_composed_info(constant_args, model_args, self):
+    """
+    For composed schemas, generate schema instances for
+    all schemas in the oneOf/anyOf/allOf definition. If additional
+    properties are allowed, also assign those properties on
+    all matched schemas that contain additionalProperties.
+    Openapi schemas are python classes.
+
+    Exceptions are raised if:
+    - 0 or > 1 oneOf schema matches the model_args input data
+    - no anyOf schema matches the model_args input data
+    - any of the allOf schemas do not match the model_args input data
+
+    Args:
+        constant_args (dict): these are the args that every model requires
+        model_args (dict): these are the required and optional spec args that
+            were passed in to make this model
+        self (class): the class that we are instantiating
+            This class contains self._composed_schemas
+
+    Returns:
+        composed_info (list): length three
+            composed_instances (list): the composed instances which are not
+                self
+            var_name_to_model_instances (dict): a dict going from var_name
+                to the model_instance which holds that var_name
+                the model_instance may be self or an instance of one of the
+                classes in self.composed_instances()
+            additional_properties_model_instances (list): a list of the
+                model instances which have the property
+                additional_properties_type. This list can include self
+    """
+    # create composed_instances
+    composed_instances = []
+    allof_instances = get_allof_instances(self, model_args, constant_args)
+    composed_instances.extend(allof_instances)
+    oneof_instance = get_oneof_instance(self.__class__, model_args, constant_args)
+    if oneof_instance is not None:
+        composed_instances.append(oneof_instance)
+    anyof_instances = get_anyof_instances(self, model_args, constant_args)
+    composed_instances.extend(anyof_instances)
+    """
+    set additional_properties_model_instances
+    additional properties must be evaluated at the schema level
+    so self's additional properties are most important
+    If self is a composed schema with:
+    - no properties defined in self
+    - additionalProperties: False
+    Then for object payloads every property is an additional property
+    and they are not allowed, so only empty dict is allowed
+
+    Properties must be set on all matching schemas
+    so when a property is assigned toa composed instance, it must be set on all
+    composed instances regardless of additionalProperties presence
+    keeping it to prevent breaking changes in v5.0.1
+    TODO remove cls._additional_properties_model_instances in 6.0.0
+    """
+    additional_properties_model_instances = []
+    if self.additional_properties_type is not None:
+        additional_properties_model_instances = [self]
+
+    """
+    no need to set properties on self in here, they will be set in __init__
+    By here all composed schema oneOf/anyOf/allOf instances have their properties set using
+    model_args
+    """
+    discarded_args = get_discarded_args(self, composed_instances, model_args)
+
+    # map variable names to composed_instances
+    var_name_to_model_instances = {}
+    for prop_name in model_args:
+        if prop_name not in discarded_args:
+            var_name_to_model_instances[prop_name] = [self] + composed_instances
+
+    return [
+        composed_instances,
+        var_name_to_model_instances,
+        additional_properties_model_instances,
+        discarded_args
+    ]
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/models/__init__.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-# flake8: noqa
-
-# import all models into this package
-# if you have many models here with many references from one model to another this may
-# raise a RecursionError
-# to avoid this, import only the models that you directly need like:
-# from from code_size_analyzer_client.model.pet import Pet
-# or import this package, but before doing it, use:
-# import sys
-# sys.setrecursionlimit(n)
-
-from code_size_analyzer_client.model.application_combination import ApplicationCombination
-from code_size_analyzer_client.model.classification_rule import ClassificationRule
-from code_size_analyzer_client.model.data_record import DataRecord
-from code_size_analyzer_client.model.http_validation_error import HTTPValidationError
-from code_size_analyzer_client.model.map_file_memory_config import MapFileMemoryConfig
-from code_size_analyzer_client.model.map_file_parse_request import MapFileParseRequest
-from code_size_analyzer_client.model.map_file_parse_response import MapFileParseResponse
-from code_size_analyzer_client.model.map_file_request import MapFileRequest
-from code_size_analyzer_client.model.map_file_response import MapFileResponse
-from code_size_analyzer_client.model.map_file_section import MapFileSection
-from code_size_analyzer_client.model.map_file_summary import MapFileSummary
-from code_size_analyzer_client.model.module import Module
-from code_size_analyzer_client.model.module_group import ModuleGroup
-from code_size_analyzer_client.model.summary_record import SummaryRecord
-from code_size_analyzer_client.model.symbol import Symbol
-from code_size_analyzer_client.model.target_info import TargetInfo
-from code_size_analyzer_client.model.validation_error import ValidationError
+# flake8: noqa
+
+# import all models into this package
+# if you have many models here with many references from one model to another this may
+# raise a RecursionError
+# to avoid this, import only the models that you directly need like:
+# from from code_size_analyzer_client.model.pet import Pet
+# or import this package, but before doing it, use:
+# import sys
+# sys.setrecursionlimit(n)
+
+from code_size_analyzer_client.model.application_analysis_result_with_detail import ApplicationAnalysisResultWithDetail
+from code_size_analyzer_client.model.application_combination import ApplicationCombination
+from code_size_analyzer_client.model.classification_rule import ClassificationRule
+from code_size_analyzer_client.model.data_record import DataRecord
+from code_size_analyzer_client.model.file_data import FileData
+from code_size_analyzer_client.model.http_validation_error import HTTPValidationError
+from code_size_analyzer_client.model.map_file_memory_config import MapFileMemoryConfig
+from code_size_analyzer_client.model.map_file_parse_request import MapFileParseRequest
+from code_size_analyzer_client.model.map_file_parse_response import MapFileParseResponse
+from code_size_analyzer_client.model.map_file_request import MapFileRequest
+from code_size_analyzer_client.model.map_file_response import MapFileResponse
+from code_size_analyzer_client.model.map_file_section import MapFileSection
+from code_size_analyzer_client.model.map_file_summary import MapFileSummary
+from code_size_analyzer_client.model.module import Module
+from code_size_analyzer_client.model.module_group import ModuleGroup
+from code_size_analyzer_client.model.response_get_app_analysis_details_results_get_app_analysis_details_get import ResponseGetAppAnalysisDetailsResultsGetAppAnalysisDetailsGet
+from code_size_analyzer_client.model.section_summary import SectionSummary
+from code_size_analyzer_client.model.summary_record import SummaryRecord
+from code_size_analyzer_client.model.symbol import Symbol
+from code_size_analyzer_client.model.target_info import TargetInfo
+from code_size_analyzer_client.model.validation_error import ValidationError
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client/rest.py` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client/rest.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,352 +1,352 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import io
-import json
-import logging
-import re
-import ssl
-from urllib.parse import urlencode
-from urllib.parse import urlparse
-from urllib.request import proxy_bypass_environment
-import urllib3
-import ipaddress
-
-from code_size_analyzer_client.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
-
-
-logger = logging.getLogger(__name__)
-
-
-class RESTResponse(io.IOBase):
-
-    def __init__(self, resp):
-        self.urllib3_response = resp
-        self.status = resp.status
-        self.reason = resp.reason
-        self.data = resp.data
-
-    def getheaders(self):
-        """Returns a dictionary of the response headers."""
-        return self.urllib3_response.getheaders()
-
-    def getheader(self, name, default=None):
-        """Returns a given response header."""
-        return self.urllib3_response.getheader(name, default)
-
-
-class RESTClientObject(object):
-
-    def __init__(self, configuration, pools_size=4, maxsize=None):
-        # urllib3.PoolManager will pass all kw parameters to connectionpool
-        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
-        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
-        # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
-        # Custom SSL certificates and client certificates: http://urllib3.readthedocs.io/en/latest/advanced-usage.html  # noqa: E501
-
-        # cert_reqs
-        if configuration.verify_ssl:
-            cert_reqs = ssl.CERT_REQUIRED
-        else:
-            cert_reqs = ssl.CERT_NONE
-
-        addition_pool_args = {}
-        if configuration.assert_hostname is not None:
-            addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
-
-        if configuration.retries is not None:
-            addition_pool_args['retries'] = configuration.retries
-
-        if configuration.socket_options is not None:
-            addition_pool_args['socket_options'] = configuration.socket_options
-
-        if maxsize is None:
-            if configuration.connection_pool_maxsize is not None:
-                maxsize = configuration.connection_pool_maxsize
-            else:
-                maxsize = 4
-
-        # https pool manager
-        if configuration.proxy and not should_bypass_proxies(
-                configuration.host, no_proxy=configuration.no_proxy or ''):
-            self.pool_manager = urllib3.ProxyManager(
-                num_pools=pools_size,
-                maxsize=maxsize,
-                cert_reqs=cert_reqs,
-                ca_certs=configuration.ssl_ca_cert,
-                cert_file=configuration.cert_file,
-                key_file=configuration.key_file,
-                proxy_url=configuration.proxy,
-                proxy_headers=configuration.proxy_headers,
-                **addition_pool_args
-            )
-        else:
-            self.pool_manager = urllib3.PoolManager(
-                num_pools=pools_size,
-                maxsize=maxsize,
-                cert_reqs=cert_reqs,
-                ca_certs=configuration.ssl_ca_cert,
-                cert_file=configuration.cert_file,
-                key_file=configuration.key_file,
-                **addition_pool_args
-            )
-
-    def request(self, method, url, query_params=None, headers=None,
-                body=None, post_params=None, _preload_content=True,
-                _request_timeout=None):
-        """Perform requests.
-
-        :param method: http request method
-        :param url: http request url
-        :param query_params: query parameters in the url
-        :param headers: http request headers
-        :param body: request json body, for `application/json`
-        :param post_params: request post parameters,
-                            `application/x-www-form-urlencoded`
-                            and `multipart/form-data`
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        """
-        method = method.upper()
-        assert method in ['GET', 'HEAD', 'DELETE', 'POST', 'PUT',
-                          'PATCH', 'OPTIONS']
-
-        if post_params and body:
-            raise ApiValueError(
-                "body parameter cannot be used with post_params parameter."
-            )
-
-        post_params = post_params or {}
-        headers = headers or {}
-
-        timeout = None
-        if _request_timeout:
-            if isinstance(_request_timeout, (int, float)):  # noqa: E501,F821
-                timeout = urllib3.Timeout(total=_request_timeout)
-            elif (isinstance(_request_timeout, tuple) and
-                  len(_request_timeout) == 2):
-                timeout = urllib3.Timeout(
-                    connect=_request_timeout[0], read=_request_timeout[1])
-
-        try:
-            # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
-            if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
-                # Only set a default Content-Type for POST, PUT, PATCH and OPTIONS requests
-                if (method != 'DELETE') and ('Content-Type' not in headers):
-                    headers['Content-Type'] = 'application/json'
-                if query_params:
-                    url += '?' + urlencode(query_params)
-                if ('Content-Type' not in headers) or (re.search('json',
-                                                                 headers['Content-Type'], re.IGNORECASE)):
-                    request_body = None
-                    if body is not None:
-                        request_body = json.dumps(body)
-                    r = self.pool_manager.request(
-                        method, url,
-                        body=request_body,
-                        preload_content=_preload_content,
-                        timeout=timeout,
-                        headers=headers)
-                elif headers['Content-Type'] == 'application/x-www-form-urlencoded':  # noqa: E501
-                    r = self.pool_manager.request(
-                        method, url,
-                        fields=post_params,
-                        encode_multipart=False,
-                        preload_content=_preload_content,
-                        timeout=timeout,
-                        headers=headers)
-                elif headers['Content-Type'] == 'multipart/form-data':
-                    # must del headers['Content-Type'], or the correct
-                    # Content-Type which generated by urllib3 will be
-                    # overwritten.
-                    del headers['Content-Type']
-                    r = self.pool_manager.request(
-                        method, url,
-                        fields=post_params,
-                        encode_multipart=True,
-                        preload_content=_preload_content,
-                        timeout=timeout,
-                        headers=headers)
-                # Pass a `string` parameter directly in the body to support
-                # other content types than Json when `body` argument is
-                # provided in serialized form
-                elif isinstance(body, str) or isinstance(body, bytes):
-                    request_body = body
-                    r = self.pool_manager.request(
-                        method, url,
-                        body=request_body,
-                        preload_content=_preload_content,
-                        timeout=timeout,
-                        headers=headers)
-                else:
-                    # Cannot generate the request from given parameters
-                    msg = """Cannot prepare a request message for provided
-                             arguments. Please check that your arguments match
-                             declared content type."""
-                    raise ApiException(status=0, reason=msg)
-            # For `GET`, `HEAD`
-            else:
-                r = self.pool_manager.request(method, url,
-                                              fields=query_params,
-                                              preload_content=_preload_content,
-                                              timeout=timeout,
-                                              headers=headers)
-        except urllib3.exceptions.SSLError as e:
-            msg = "{0}\n{1}".format(type(e).__name__, str(e))
-            raise ApiException(status=0, reason=msg)
-
-        if _preload_content:
-            r = RESTResponse(r)
-
-            # log response body
-            logger.debug("response body: %s", r.data)
-
-        if not 200 <= r.status <= 299:
-            if r.status == 401:
-                raise UnauthorizedException(http_resp=r)
-
-            if r.status == 403:
-                raise ForbiddenException(http_resp=r)
-
-            if r.status == 404:
-                raise NotFoundException(http_resp=r)
-
-            if 500 <= r.status <= 599:
-                raise ServiceException(http_resp=r)
-
-            raise ApiException(http_resp=r)
-
-        return r
-
-    def GET(self, url, headers=None, query_params=None, _preload_content=True,
-            _request_timeout=None):
-        return self.request("GET", url,
-                            headers=headers,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            query_params=query_params)
-
-    def HEAD(self, url, headers=None, query_params=None, _preload_content=True,
-             _request_timeout=None):
-        return self.request("HEAD", url,
-                            headers=headers,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            query_params=query_params)
-
-    def OPTIONS(self, url, headers=None, query_params=None, post_params=None,
-                body=None, _preload_content=True, _request_timeout=None):
-        return self.request("OPTIONS", url,
-                            headers=headers,
-                            query_params=query_params,
-                            post_params=post_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
-
-    def DELETE(self, url, headers=None, query_params=None, body=None,
-               _preload_content=True, _request_timeout=None):
-        return self.request("DELETE", url,
-                            headers=headers,
-                            query_params=query_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
-
-    def POST(self, url, headers=None, query_params=None, post_params=None,
-             body=None, _preload_content=True, _request_timeout=None):
-        return self.request("POST", url,
-                            headers=headers,
-                            query_params=query_params,
-                            post_params=post_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
-
-    def PUT(self, url, headers=None, query_params=None, post_params=None,
-            body=None, _preload_content=True, _request_timeout=None):
-        return self.request("PUT", url,
-                            headers=headers,
-                            query_params=query_params,
-                            post_params=post_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
-
-    def PATCH(self, url, headers=None, query_params=None, post_params=None,
-              body=None, _preload_content=True, _request_timeout=None):
-        return self.request("PATCH", url,
-                            headers=headers,
-                            query_params=query_params,
-                            post_params=post_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
-
-# end of class RESTClientObject
-
-
-def is_ipv4(target):
-    """ Test if IPv4 address or not
-    """
-    try:
-        chk = ipaddress.IPv4Address(target)
-        return True
-    except ipaddress.AddressValueError:
-        return False
-
-
-def in_ipv4net(target, net):
-    """ Test if target belongs to given IPv4 network
-    """
-    try:
-        nw = ipaddress.IPv4Network(net)
-        ip = ipaddress.IPv4Address(target)
-        if ip in nw:
-            return True
-        return False
-    except ipaddress.AddressValueError:
-        return False
-    except ipaddress.NetmaskValueError:
-        return False
-
-
-def should_bypass_proxies(url, no_proxy=None):
-    """ Yet another requests.should_bypass_proxies
-    Test if proxies should not be used for a particular url.
-    """
-
-    parsed = urlparse(url)
-
-    # special cases
-    if parsed.hostname in [None, '']:
-        return True
-
-    # special cases
-    if no_proxy in [None, '']:
-        return False
-    if no_proxy == '*':
-        return True
-
-    no_proxy = no_proxy.lower().replace(' ', '');
-    entries = (
-        host for host in no_proxy.split(',') if host
-    )
-
-    if is_ipv4(parsed.hostname):
-        for item in entries:
-            if in_ipv4net(parsed.hostname, item):
-                return True
-    return proxy_bypass_environment(parsed.hostname, {'no': no_proxy})
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import io
+import json
+import logging
+import re
+import ssl
+from urllib.parse import urlencode
+from urllib.parse import urlparse
+from urllib.request import proxy_bypass_environment
+import urllib3
+import ipaddress
+
+from code_size_analyzer_client.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
+
+
+logger = logging.getLogger(__name__)
+
+
+class RESTResponse(io.IOBase):
+
+    def __init__(self, resp):
+        self.urllib3_response = resp
+        self.status = resp.status
+        self.reason = resp.reason
+        self.data = resp.data
+
+    def getheaders(self):
+        """Returns a dictionary of the response headers."""
+        return self.urllib3_response.getheaders()
+
+    def getheader(self, name, default=None):
+        """Returns a given response header."""
+        return self.urllib3_response.getheader(name, default)
+
+
+class RESTClientObject(object):
+
+    def __init__(self, configuration, pools_size=4, maxsize=None):
+        # urllib3.PoolManager will pass all kw parameters to connectionpool
+        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
+        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
+        # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
+        # Custom SSL certificates and client certificates: http://urllib3.readthedocs.io/en/latest/advanced-usage.html  # noqa: E501
+
+        # cert_reqs
+        if configuration.verify_ssl:
+            cert_reqs = ssl.CERT_REQUIRED
+        else:
+            cert_reqs = ssl.CERT_NONE
+
+        addition_pool_args = {}
+        if configuration.assert_hostname is not None:
+            addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
+
+        if configuration.retries is not None:
+            addition_pool_args['retries'] = configuration.retries
+
+        if configuration.socket_options is not None:
+            addition_pool_args['socket_options'] = configuration.socket_options
+
+        if maxsize is None:
+            if configuration.connection_pool_maxsize is not None:
+                maxsize = configuration.connection_pool_maxsize
+            else:
+                maxsize = 4
+
+        # https pool manager
+        if configuration.proxy and not should_bypass_proxies(
+                configuration.host, no_proxy=configuration.no_proxy or ''):
+            self.pool_manager = urllib3.ProxyManager(
+                num_pools=pools_size,
+                maxsize=maxsize,
+                cert_reqs=cert_reqs,
+                ca_certs=configuration.ssl_ca_cert,
+                cert_file=configuration.cert_file,
+                key_file=configuration.key_file,
+                proxy_url=configuration.proxy,
+                proxy_headers=configuration.proxy_headers,
+                **addition_pool_args
+            )
+        else:
+            self.pool_manager = urllib3.PoolManager(
+                num_pools=pools_size,
+                maxsize=maxsize,
+                cert_reqs=cert_reqs,
+                ca_certs=configuration.ssl_ca_cert,
+                cert_file=configuration.cert_file,
+                key_file=configuration.key_file,
+                **addition_pool_args
+            )
+
+    def request(self, method, url, query_params=None, headers=None,
+                body=None, post_params=None, _preload_content=True,
+                _request_timeout=None):
+        """Perform requests.
+
+        :param method: http request method
+        :param url: http request url
+        :param query_params: query parameters in the url
+        :param headers: http request headers
+        :param body: request json body, for `application/json`
+        :param post_params: request post parameters,
+                            `application/x-www-form-urlencoded`
+                            and `multipart/form-data`
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        """
+        method = method.upper()
+        assert method in ['GET', 'HEAD', 'DELETE', 'POST', 'PUT',
+                          'PATCH', 'OPTIONS']
+
+        if post_params and body:
+            raise ApiValueError(
+                "body parameter cannot be used with post_params parameter."
+            )
+
+        post_params = post_params or {}
+        headers = headers or {}
+
+        timeout = None
+        if _request_timeout:
+            if isinstance(_request_timeout, (int, float)):  # noqa: E501,F821
+                timeout = urllib3.Timeout(total=_request_timeout)
+            elif (isinstance(_request_timeout, tuple) and
+                  len(_request_timeout) == 2):
+                timeout = urllib3.Timeout(
+                    connect=_request_timeout[0], read=_request_timeout[1])
+
+        try:
+            # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
+            if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
+                # Only set a default Content-Type for POST, PUT, PATCH and OPTIONS requests
+                if (method != 'DELETE') and ('Content-Type' not in headers):
+                    headers['Content-Type'] = 'application/json'
+                if query_params:
+                    url += '?' + urlencode(query_params)
+                if ('Content-Type' not in headers) or (re.search('json',
+                                                                 headers['Content-Type'], re.IGNORECASE)):
+                    request_body = None
+                    if body is not None:
+                        request_body = json.dumps(body)
+                    r = self.pool_manager.request(
+                        method, url,
+                        body=request_body,
+                        preload_content=_preload_content,
+                        timeout=timeout,
+                        headers=headers)
+                elif headers['Content-Type'] == 'application/x-www-form-urlencoded':  # noqa: E501
+                    r = self.pool_manager.request(
+                        method, url,
+                        fields=post_params,
+                        encode_multipart=False,
+                        preload_content=_preload_content,
+                        timeout=timeout,
+                        headers=headers)
+                elif headers['Content-Type'] == 'multipart/form-data':
+                    # must del headers['Content-Type'], or the correct
+                    # Content-Type which generated by urllib3 will be
+                    # overwritten.
+                    del headers['Content-Type']
+                    r = self.pool_manager.request(
+                        method, url,
+                        fields=post_params,
+                        encode_multipart=True,
+                        preload_content=_preload_content,
+                        timeout=timeout,
+                        headers=headers)
+                # Pass a `string` parameter directly in the body to support
+                # other content types than Json when `body` argument is
+                # provided in serialized form
+                elif isinstance(body, str) or isinstance(body, bytes):
+                    request_body = body
+                    r = self.pool_manager.request(
+                        method, url,
+                        body=request_body,
+                        preload_content=_preload_content,
+                        timeout=timeout,
+                        headers=headers)
+                else:
+                    # Cannot generate the request from given parameters
+                    msg = """Cannot prepare a request message for provided
+                             arguments. Please check that your arguments match
+                             declared content type."""
+                    raise ApiException(status=0, reason=msg)
+            # For `GET`, `HEAD`
+            else:
+                r = self.pool_manager.request(method, url,
+                                              fields=query_params,
+                                              preload_content=_preload_content,
+                                              timeout=timeout,
+                                              headers=headers)
+        except urllib3.exceptions.SSLError as e:
+            msg = "{0}\n{1}".format(type(e).__name__, str(e))
+            raise ApiException(status=0, reason=msg)
+
+        if _preload_content:
+            r = RESTResponse(r)
+
+            # log response body
+            logger.debug("response body: %s", r.data)
+
+        if not 200 <= r.status <= 299:
+            if r.status == 401:
+                raise UnauthorizedException(http_resp=r)
+
+            if r.status == 403:
+                raise ForbiddenException(http_resp=r)
+
+            if r.status == 404:
+                raise NotFoundException(http_resp=r)
+
+            if 500 <= r.status <= 599:
+                raise ServiceException(http_resp=r)
+
+            raise ApiException(http_resp=r)
+
+        return r
+
+    def GET(self, url, headers=None, query_params=None, _preload_content=True,
+            _request_timeout=None):
+        return self.request("GET", url,
+                            headers=headers,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            query_params=query_params)
+
+    def HEAD(self, url, headers=None, query_params=None, _preload_content=True,
+             _request_timeout=None):
+        return self.request("HEAD", url,
+                            headers=headers,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            query_params=query_params)
+
+    def OPTIONS(self, url, headers=None, query_params=None, post_params=None,
+                body=None, _preload_content=True, _request_timeout=None):
+        return self.request("OPTIONS", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def DELETE(self, url, headers=None, query_params=None, body=None,
+               _preload_content=True, _request_timeout=None):
+        return self.request("DELETE", url,
+                            headers=headers,
+                            query_params=query_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def POST(self, url, headers=None, query_params=None, post_params=None,
+             body=None, _preload_content=True, _request_timeout=None):
+        return self.request("POST", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def PUT(self, url, headers=None, query_params=None, post_params=None,
+            body=None, _preload_content=True, _request_timeout=None):
+        return self.request("PUT", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def PATCH(self, url, headers=None, query_params=None, post_params=None,
+              body=None, _preload_content=True, _request_timeout=None):
+        return self.request("PATCH", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+# end of class RESTClientObject
+
+
+def is_ipv4(target):
+    """ Test if IPv4 address or not
+    """
+    try:
+        chk = ipaddress.IPv4Address(target)
+        return True
+    except ipaddress.AddressValueError:
+        return False
+
+
+def in_ipv4net(target, net):
+    """ Test if target belongs to given IPv4 network
+    """
+    try:
+        nw = ipaddress.IPv4Network(net)
+        ip = ipaddress.IPv4Address(target)
+        if ip in nw:
+            return True
+        return False
+    except ipaddress.AddressValueError:
+        return False
+    except ipaddress.NetmaskValueError:
+        return False
+
+
+def should_bypass_proxies(url, no_proxy=None):
+    """ Yet another requests.should_bypass_proxies
+    Test if proxies should not be used for a particular url.
+    """
+
+    parsed = urlparse(url)
+
+    # special cases
+    if parsed.hostname in [None, '']:
+        return True
+
+    # special cases
+    if no_proxy in [None, '']:
+        return False
+    if no_proxy == '*':
+        return True
+
+    no_proxy = no_proxy.lower().replace(' ', '');
+    entries = (
+        host for host in no_proxy.split(',') if host
+    )
+
+    if is_ipv4(parsed.hostname):
+        for item in entries:
+            if in_ipv4net(parsed.hostname, item):
+                return True
+    return proxy_bypass_environment(parsed.hostname, {'no': no_proxy})
```

### Comparing `code_size_analyzer_client-python-0.6.2/code_size_analyzer_client_python.egg-info/SOURCES.txt` & `code_size_analyzer_client_python-0.7.0/code_size_analyzer_client_python.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 README.md
 code_size_analyzer_cli.py
+code_size_results_cli.py
 setup.cfg
 setup.py
 code_size_analyzer_client/__init__.py
 code_size_analyzer_client/api_client.py
 code_size_analyzer_client/client_wrapper.py
 code_size_analyzer_client/configuration.py
 code_size_analyzer_client/exceptions.py
@@ -12,52 +13,60 @@
 code_size_analyzer_client/api/__init__.py
 code_size_analyzer_client/api/analyzer_api.py
 code_size_analyzer_client/api/default_api.py
 code_size_analyzer_client/api/parser_api.py
 code_size_analyzer_client/api/results_api.py
 code_size_analyzer_client/apis/__init__.py
 code_size_analyzer_client/model/__init__.py
+code_size_analyzer_client/model/application_analysis_result_with_detail.py
 code_size_analyzer_client/model/application_combination.py
 code_size_analyzer_client/model/classification_rule.py
 code_size_analyzer_client/model/data_record.py
+code_size_analyzer_client/model/file_data.py
 code_size_analyzer_client/model/http_validation_error.py
 code_size_analyzer_client/model/map_file_memory_config.py
 code_size_analyzer_client/model/map_file_parse_request.py
 code_size_analyzer_client/model/map_file_parse_response.py
 code_size_analyzer_client/model/map_file_request.py
 code_size_analyzer_client/model/map_file_response.py
 code_size_analyzer_client/model/map_file_section.py
 code_size_analyzer_client/model/map_file_summary.py
 code_size_analyzer_client/model/module.py
 code_size_analyzer_client/model/module_group.py
+code_size_analyzer_client/model/response_get_app_analysis_details_results_get_app_analysis_details_get.py
+code_size_analyzer_client/model/section_summary.py
 code_size_analyzer_client/model/summary_record.py
 code_size_analyzer_client/model/symbol.py
 code_size_analyzer_client/model/target_info.py
 code_size_analyzer_client/model/validation_error.py
 code_size_analyzer_client/models/__init__.py
 code_size_analyzer_client_python.egg-info/PKG-INFO
 code_size_analyzer_client_python.egg-info/SOURCES.txt
 code_size_analyzer_client_python.egg-info/dependency_links.txt
 code_size_analyzer_client_python.egg-info/entry_points.txt
 code_size_analyzer_client_python.egg-info/requires.txt
 code_size_analyzer_client_python.egg-info/top_level.txt
 test/test_analyzer_api.py
+test/test_application_analysis_result_with_detail.py
 test/test_application_combination.py
 test/test_classification_rule.py
 test/test_data_record.py
 test/test_default_api.py
+test/test_file_data.py
 test/test_http_validation_error.py
 test/test_map_file_memory_config.py
 test/test_map_file_parse_request.py
 test/test_map_file_parse_response.py
 test/test_map_file_request.py
 test/test_map_file_response.py
 test/test_map_file_section.py
 test/test_map_file_summary.py
 test/test_module.py
 test/test_module_group.py
 test/test_parser_api.py
+test/test_response_get_app_analysis_details_results_get_app_analysis_details_get.py
 test/test_results_api.py
+test/test_section_summary.py
 test/test_summary_record.py
 test/test_symbol.py
 test/test_target_info.py
 test/test_validation_error.py
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_analyzer_api.py` & `code_size_analyzer_client_python-0.7.0/test/test_summary_record.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.api.analyzer_api import AnalyzerApi  # noqa: E501
-
-
-class TestAnalyzerApi(unittest.TestCase):
-    """AnalyzerApi unit test stubs"""
-
-    def setUp(self):
-        self.api = AnalyzerApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    def test_analyze_map_file(self):
-        """Test case for analyze_map_file
-
-        Analyze Map File Post  # noqa: E501
-        """
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.summary_record import SummaryRecord
+
+
+class TestSummaryRecord(unittest.TestCase):
+    """SummaryRecord unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testSummaryRecord(self):
+        """Test SummaryRecord"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = SummaryRecord()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_application_combination.py` & `code_size_analyzer_client_python-0.7.0/test/test_application_combination.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.model.application_combination import ApplicationCombination
-
-
-class TestApplicationCombination(unittest.TestCase):
-    """ApplicationCombination unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testApplicationCombination(self):
-        """Test ApplicationCombination"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ApplicationCombination()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.application_combination import ApplicationCombination
+
+
+class TestApplicationCombination(unittest.TestCase):
+    """ApplicationCombination unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testApplicationCombination(self):
+        """Test ApplicationCombination"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = ApplicationCombination()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_data_record.py` & `code_size_analyzer_client_python-0.7.0/test/test_module.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.model.data_record import DataRecord
-
-
-class TestDataRecord(unittest.TestCase):
-    """DataRecord unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testDataRecord(self):
-        """Test DataRecord"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = DataRecord()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.symbol import Symbol
+globals()['Symbol'] = Symbol
+from code_size_analyzer_client.model.module import Module
+
+
+class TestModule(unittest.TestCase):
+    """Module unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testModule(self):
+        """Test Module"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = Module()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_default_api.py` & `code_size_analyzer_client_python-0.7.0/test/test_map_file_parse_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.api.default_api import DefaultApi  # noqa: E501
-
-
-class TestDefaultApi(unittest.TestCase):
-    """DefaultApi unit test stubs"""
-
-    def setUp(self):
-        self.api = DefaultApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    def test_metrics_metrics_get(self):
-        """Test case for metrics_metrics_get
-
-        Metrics  # noqa: E501
-        """
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.map_file_parse_request import MapFileParseRequest
+
+
+class TestMapFileParseRequest(unittest.TestCase):
+    """MapFileParseRequest unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testMapFileParseRequest(self):
+        """Test MapFileParseRequest"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = MapFileParseRequest()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_http_validation_error.py` & `code_size_analyzer_client_python-0.7.0/test/test_http_validation_error.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.model.validation_error import ValidationError
-globals()['ValidationError'] = ValidationError
-from code_size_analyzer_client.model.http_validation_error import HTTPValidationError
-
-
-class TestHTTPValidationError(unittest.TestCase):
-    """HTTPValidationError unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testHTTPValidationError(self):
-        """Test HTTPValidationError"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = HTTPValidationError()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.validation_error import ValidationError
+globals()['ValidationError'] = ValidationError
+from code_size_analyzer_client.model.http_validation_error import HTTPValidationError
+
+
+class TestHTTPValidationError(unittest.TestCase):
+    """HTTPValidationError unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testHTTPValidationError(self):
+        """Test HTTPValidationError"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = HTTPValidationError()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_map_file_memory_config.py` & `code_size_analyzer_client_python-0.7.0/test/test_map_file_memory_config.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.model.map_file_section import MapFileSection
-globals()['MapFileSection'] = MapFileSection
-from code_size_analyzer_client.model.map_file_memory_config import MapFileMemoryConfig
-
-
-class TestMapFileMemoryConfig(unittest.TestCase):
-    """MapFileMemoryConfig unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testMapFileMemoryConfig(self):
-        """Test MapFileMemoryConfig"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = MapFileMemoryConfig()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.map_file_section import MapFileSection
+globals()['MapFileSection'] = MapFileSection
+from code_size_analyzer_client.model.map_file_memory_config import MapFileMemoryConfig
+
+
+class TestMapFileMemoryConfig(unittest.TestCase):
+    """MapFileMemoryConfig unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testMapFileMemoryConfig(self):
+        """Test MapFileMemoryConfig"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = MapFileMemoryConfig()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_map_file_parse_request.py` & `code_size_analyzer_client_python-0.7.0/test/test_map_file_section.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.model.map_file_parse_request import MapFileParseRequest
-
-
-class TestMapFileParseRequest(unittest.TestCase):
-    """MapFileParseRequest unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testMapFileParseRequest(self):
-        """Test MapFileParseRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = MapFileParseRequest()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.map_file_section import MapFileSection
+
+
+class TestMapFileSection(unittest.TestCase):
+    """MapFileSection unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testMapFileSection(self):
+        """Test MapFileSection"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = MapFileSection()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_map_file_parse_response.py` & `code_size_analyzer_client_python-0.7.0/test/test_map_file_parse_response.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.model.map_file_memory_config import MapFileMemoryConfig
-from code_size_analyzer_client.model.map_file_summary import MapFileSummary
-globals()['MapFileMemoryConfig'] = MapFileMemoryConfig
-globals()['MapFileSummary'] = MapFileSummary
-from code_size_analyzer_client.model.map_file_parse_response import MapFileParseResponse
-
-
-class TestMapFileParseResponse(unittest.TestCase):
-    """MapFileParseResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testMapFileParseResponse(self):
-        """Test MapFileParseResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = MapFileParseResponse()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.map_file_memory_config import MapFileMemoryConfig
+from code_size_analyzer_client.model.map_file_summary import MapFileSummary
+globals()['MapFileMemoryConfig'] = MapFileMemoryConfig
+globals()['MapFileSummary'] = MapFileSummary
+from code_size_analyzer_client.model.map_file_parse_response import MapFileParseResponse
+
+
+class TestMapFileParseResponse(unittest.TestCase):
+    """MapFileParseResponse unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testMapFileParseResponse(self):
+        """Test MapFileParseResponse"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = MapFileParseResponse()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_map_file_request.py` & `code_size_analyzer_client_python-0.7.0/test/test_classification_rule.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.model.classification_rule import ClassificationRule
-globals()['ClassificationRule'] = ClassificationRule
-from code_size_analyzer_client.model.map_file_request import MapFileRequest
-
-
-class TestMapFileRequest(unittest.TestCase):
-    """MapFileRequest unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testMapFileRequest(self):
-        """Test MapFileRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = MapFileRequest()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.classification_rule import ClassificationRule
+
+
+class TestClassificationRule(unittest.TestCase):
+    """ClassificationRule unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testClassificationRule(self):
+        """Test ClassificationRule"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = ClassificationRule()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_map_file_section.py` & `code_size_analyzer_client_python-0.7.0/test/test_file_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.model.map_file_section import MapFileSection
-
-
-class TestMapFileSection(unittest.TestCase):
-    """MapFileSection unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testMapFileSection(self):
-        """Test MapFileSection"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = MapFileSection()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.file_data import FileData
+
+
+class TestFileData(unittest.TestCase):
+    """FileData unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testFileData(self):
+        """Test FileData"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = FileData()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_module.py` & `code_size_analyzer_client_python-0.7.0/test/test_map_file_summary.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.model.symbol import Symbol
-globals()['Symbol'] = Symbol
-from code_size_analyzer_client.model.module import Module
-
-
-class TestModule(unittest.TestCase):
-    """Module unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testModule(self):
-        """Test Module"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Module()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.module_group import ModuleGroup
+globals()['ModuleGroup'] = ModuleGroup
+from code_size_analyzer_client.model.map_file_summary import MapFileSummary
+
+
+class TestMapFileSummary(unittest.TestCase):
+    """MapFileSummary unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testMapFileSummary(self):
+        """Test MapFileSummary"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = MapFileSummary()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_module_group.py` & `code_size_analyzer_client_python-0.7.0/test/test_module_group.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.model.module import Module
-globals()['Module'] = Module
-from code_size_analyzer_client.model.module_group import ModuleGroup
-
-
-class TestModuleGroup(unittest.TestCase):
-    """ModuleGroup unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testModuleGroup(self):
-        """Test ModuleGroup"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ModuleGroup()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.module import Module
+globals()['Module'] = Module
+from code_size_analyzer_client.model.module_group import ModuleGroup
+
+
+class TestModuleGroup(unittest.TestCase):
+    """ModuleGroup unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testModuleGroup(self):
+        """Test ModuleGroup"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = ModuleGroup()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_parser_api.py` & `code_size_analyzer_client_python-0.7.0/test/test_default_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.api.parser_api import ParserApi  # noqa: E501
-
-
-class TestParserApi(unittest.TestCase):
-    """ParserApi unit test stubs"""
-
-    def setUp(self):
-        self.api = ParserApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    def test_parse_map_file(self):
-        """Test case for parse_map_file
-
-        Analyze Map File Post  # noqa: E501
-        """
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.api.default_api import DefaultApi  # noqa: E501
+
+
+class TestDefaultApi(unittest.TestCase):
+    """DefaultApi unit test stubs"""
+
+    def setUp(self):
+        self.api = DefaultApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_metrics_health_get(self):
+        """Test case for metrics_health_get
+
+        Metrics  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_results_api.py` & `code_size_analyzer_client_python-0.7.0/test/test_results_api.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.api.results_api import ResultsApi  # noqa: E501
-
-
-class TestResultsApi(unittest.TestCase):
-    """ResultsApi unit test stubs"""
-
-    def setUp(self):
-        self.api = ResultsApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    def test_get_app_analysis_details(self):
-        """Test case for get_app_analysis_details
-
-        Get App Analysis Details  # noqa: E501
-        """
-        pass
-
-    def test_get_app_combinations(self):
-        """Test case for get_app_combinations
-
-        Get App Combinations  # noqa: E501
-        """
-        pass
-
-    def test_get_app_stack_names(self):
-        """Test case for get_app_stack_names
-
-        Get App Stack Names  # noqa: E501
-        """
-        pass
-
-    def test_get_app_summary_records(self):
-        """Test case for get_app_summary_records
-
-        Get App Summary Records  # noqa: E501
-        """
-        pass
-
-    def test_get_branch_builds(self):
-        """Test case for get_branch_builds
-
-        Get Branch Builds  # noqa: E501
-        """
-        pass
-
-    def test_get_target_info(self):
-        """Test case for get_target_info
-
-        Get Target Info  # noqa: E501
-        """
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.api.results_api import ResultsApi  # noqa: E501
+
+
+class TestResultsApi(unittest.TestCase):
+    """ResultsApi unit test stubs"""
+
+    def setUp(self):
+        self.api = ResultsApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_get_app_analysis_details(self):
+        """Test case for get_app_analysis_details
+
+        Get App Analysis Details  # noqa: E501
+        """
+        pass
+
+    def test_get_app_combinations(self):
+        """Test case for get_app_combinations
+
+        Get App Combinations  # noqa: E501
+        """
+        pass
+
+    def test_get_app_stack_names(self):
+        """Test case for get_app_stack_names
+
+        Get App Stack Names  # noqa: E501
+        """
+        pass
+
+    def test_get_app_summary_records(self):
+        """Test case for get_app_summary_records
+
+        Get App Summary Records  # noqa: E501
+        """
+        pass
+
+    def test_get_branch_builds(self):
+        """Test case for get_branch_builds
+
+        Get Branch Builds  # noqa: E501
+        """
+        pass
+
+    def test_get_target_info(self):
+        """Test case for get_target_info
+
+        Get Target Info  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_target_info.py` & `code_size_analyzer_client_python-0.7.0/test/test_target_info.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.model.target_info import TargetInfo
-
-
-class TestTargetInfo(unittest.TestCase):
-    """TargetInfo unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testTargetInfo(self):
-        """Test TargetInfo"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = TargetInfo()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.target_info import TargetInfo
+
+
+class TestTargetInfo(unittest.TestCase):
+    """TargetInfo unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testTargetInfo(self):
+        """Test TargetInfo"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = TargetInfo()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `code_size_analyzer_client-python-0.6.2/test/test_validation_error.py` & `code_size_analyzer_client_python-0.7.0/test/test_validation_error.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-"""
-    FastAPI
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import sys
-import unittest
-
-import code_size_analyzer_client
-from code_size_analyzer_client.model.validation_error import ValidationError
-
-
-class TestValidationError(unittest.TestCase):
-    """ValidationError unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testValidationError(self):
-        """Test ValidationError"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ValidationError()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+    FastAPI
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+
+    The version of the OpenAPI document: 0.1.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import code_size_analyzer_client
+from code_size_analyzer_client.model.validation_error import ValidationError
+
+
+class TestValidationError(unittest.TestCase):
+    """ValidationError unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testValidationError(self):
+        """Test ValidationError"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = ValidationError()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

