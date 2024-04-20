# Comparing `tmp/types-dateparser-1.1.4.9.tar.gz` & `tmp/types-dateparser-1.2.0.20240420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-dateparser-1.1.4.9.tar", last modified: Mon Mar 27 18:22:38 2023, max compression
+gzip compressed data, was "types-dateparser-1.2.0.20240420.tar", last modified: Sat Apr 20 02:14:53 2024, max compression
```

## Comparing `types-dateparser-1.1.4.9.tar` & `types-dateparser-1.2.0.20240420.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.122065 types-dateparser-1.1.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-27 18:22:37.000000 types-dateparser-1.1.4.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:22:37.000000 types-dateparser-1.1.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-27 18:22:38.122065 types-dateparser-1.1.4.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.118065 types-dateparser-1.1.4.9/dateparser-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-27 18:22:37.000000 types-dateparser-1.1.4.9/dateparser-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.118065 types-dateparser-1.1.4.9/dateparser-stubs/calendars/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/calendars/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/calendars/hijri.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/calendars/hijri_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/calendars/jalali.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/calendars/jalali_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/conf.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.118065 types-dateparser-1.1.4.9/dateparser-stubs/custom_language_detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/custom_language_detection/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/custom_language_detection/fasttext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/custom_language_detection/langdetect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/custom_language_detection/language_mapping.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.118065 types-dateparser-1.1.4.9/dateparser-stubs/data/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/data/languages_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/date.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/date_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/freshness_date_parser.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.118065 types-dateparser-1.1.4.9/dateparser-stubs/languages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/languages/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/languages/dictionary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/languages/loader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/languages/locale.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/languages/validation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/parser.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.118065 types-dateparser-1.1.4.9/dateparser-stubs/search/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/search/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/search/detection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/search/search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/search/text_detection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/timezone_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/timezones.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.122065 types-dateparser-1.1.4.9/dateparser-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/utils/strptime.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.122065 types-dateparser-1.1.4.9/dateparser_data-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-27 18:22:37.000000 types-dateparser-1.1.4.9/dateparser_data-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser_data-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser_data-stubs/settings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:22:38.122065 types-dateparser-1.1.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-03-27 18:22:37.000000 types-dateparser-1.1.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.122065 types-dateparser-1.1.4.9/types_dateparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-27 18:22:38.000000 types-dateparser-1.1.4.9/types_dateparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-27 18:22:38.000000 types-dateparser-1.1.4.9/types_dateparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:22:38.000000 types-dateparser-1.1.4.9/types_dateparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-27 18:22:38.000000 types-dateparser-1.1.4.9/types_dateparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:53.716172 types-dateparser-1.2.0.20240420/
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-20 02:14:51.000000 types-dateparser-1.2.0.20240420/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 02:14:51.000000 types-dateparser-1.2.0.20240420/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-20 02:14:53.716172 types-dateparser-1.2.0.20240420/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:53.712172 types-dateparser-1.2.0.20240420/dateparser-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-20 02:14:51.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:53.712172 types-dateparser-1.2.0.20240420/dateparser-stubs/calendars/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/calendars/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/calendars/hijri.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/calendars/hijri_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/calendars/jalali.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/calendars/jalali_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/conf.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:53.712172 types-dateparser-1.2.0.20240420/dateparser-stubs/custom_language_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/custom_language_detection/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/custom_language_detection/fasttext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/custom_language_detection/langdetect.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/custom_language_detection/language_mapping.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:53.712172 types-dateparser-1.2.0.20240420/dateparser-stubs/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/data/languages_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/date.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/date_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/freshness_date_parser.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:53.716172 types-dateparser-1.2.0.20240420/dateparser-stubs/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/languages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/languages/dictionary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/languages/loader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/languages/locale.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/languages/validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:51.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:53.716172 types-dateparser-1.2.0.20240420/dateparser-stubs/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/search/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/search/detection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/search/search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/search/text_detection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/timezone_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/timezones.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:53.716172 types-dateparser-1.2.0.20240420/dateparser-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser-stubs/utils/strptime.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:53.716172 types-dateparser-1.2.0.20240420/dateparser_data-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-20 02:14:51.000000 types-dateparser-1.2.0.20240420/dateparser_data-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser_data-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:51.000000 types-dateparser-1.2.0.20240420/dateparser_data-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-20 02:14:41.000000 types-dateparser-1.2.0.20240420/dateparser_data-stubs/settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 02:14:53.716172 types-dateparser-1.2.0.20240420/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-20 02:14:51.000000 types-dateparser-1.2.0.20240420/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:53.716172 types-dateparser-1.2.0.20240420/types_dateparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-20 02:14:53.000000 types-dateparser-1.2.0.20240420/types_dateparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-20 02:14:53.000000 types-dateparser-1.2.0.20240420/types_dateparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:14:53.000000 types-dateparser-1.2.0.20240420/types_dateparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-20 02:14:53.000000 types-dateparser-1.2.0.20240420/types_dateparser.egg-info/top_level.txt
```

### Comparing `types-dateparser-1.1.4.9/CHANGELOG.md` & `types-dateparser-1.2.0.20240420/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+## 1.2.0.20240420 (2024-04-20)
+
+Bump dateparser to 1.2.* (#11786)
+
+## 1.1.4.20240331 (2024-03-31)
+
+Remove bare Incomplete annotations in third-party stubs (#11671)
+
+## 1.1.4.20240106 (2024-01-06)
+
+Update typing_extensions imports in third-party stubs (#11245)
+
+## 1.1.4.10 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 1.1.4.9 (2023-03-27)
 
 Add defaults for third-party stubs A-D (#9952)
 
 ## 1.1.4.8 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-dateparser-1.1.4.9/PKG-INFO` & `types-dateparser-1.2.0.20240420/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 Metadata-Version: 2.1
 Name: types-dateparser
-Version: 1.1.4.9
+Version: 1.2.0.20240420
 Summary: Typing stubs for dateparser
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dateparser.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for dateparser
 
-This is a PEP 561 type stub package for the `dateparser` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`dateparser`](https://github.com/scrapinghub/dateparser) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`dateparser`. The source for this package can be found at
+`dateparser`.
+
+This version of `types-dateparser` aims to provide accurate annotations
+for `dateparser==1.2.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/dateparser. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `57f3dcac8dbed008479b251512975901a0206deb` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-dateparser-1.1.4.9/dateparser-stubs/__init__.pyi` & `types-dateparser-1.2.0.20240420/dateparser-stubs/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
-from typing_extensions import Literal, TypeAlias, TypedDict
+from typing import Literal, TypedDict
+from typing_extensions import TypeAlias
 
 from .date import DateDataParser, _DetectLanguagesFunction
 
 __version__: str
 
 _default_parser: DateDataParser
```

### Comparing `types-dateparser-1.1.4.9/dateparser-stubs/calendars/hijri_parser.pyi` & `types-dateparser-1.2.0.20240420/dateparser-stubs/calendars/hijri_parser.pyi`

 * *Files identical despite different names*

### Comparing `types-dateparser-1.1.4.9/dateparser-stubs/conf.pyi` & `types-dateparser-1.2.0.20240420/dateparser-stubs/conf.pyi`

 * *Files identical despite different names*

### Comparing `types-dateparser-1.1.4.9/dateparser-stubs/date.pyi` & `types-dateparser-1.2.0.20240420/dateparser-stubs/date.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import collections
 from collections.abc import Callable, Iterable, Iterator
 from datetime import datetime
 from re import Pattern
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from typing import ClassVar, Literal, overload
+from typing_extensions import TypeAlias
 
 from dateparser import _Settings
 from dateparser.conf import Settings
 from dateparser.languages.loader import LocaleDataLoader
 from dateparser.languages.locale import Locale
 
 _DetectLanguagesFunction: TypeAlias = Callable[[str, float], list[str]]
```

### Comparing `types-dateparser-1.1.4.9/dateparser-stubs/languages/dictionary.pyi` & `types-dateparser-1.2.0.20240420/dateparser-stubs/languages/dictionary.pyi`

 * *Files identical despite different names*

### Comparing `types-dateparser-1.1.4.9/dateparser-stubs/languages/loader.pyi` & `types-dateparser-1.2.0.20240420/dateparser-stubs/languages/loader.pyi`

 * *Files identical despite different names*

### Comparing `types-dateparser-1.1.4.9/dateparser-stubs/languages/locale.pyi` & `types-dateparser-1.2.0.20240420/dateparser-stubs/languages/locale.pyi`

 * *Files identical despite different names*

### Comparing `types-dateparser-1.1.4.9/dateparser-stubs/parser.pyi` & `types-dateparser-1.2.0.20240420/dateparser-stubs/parser.pyi`

 * *Files identical despite different names*

### Comparing `types-dateparser-1.1.4.9/dateparser-stubs/search/__init__.pyi` & `types-dateparser-1.2.0.20240420/dateparser-stubs/search/__init__.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from collections.abc import Mapping, Set as AbstractSet
 from datetime import datetime
-from typing import Any, overload
-from typing_extensions import Literal
+from typing import Any, Literal, overload
 
 from ..date import _DetectLanguagesFunction
 
 @overload
 def search_dates(
     text: str,
     languages: list[str] | tuple[str, ...] | AbstractSet[str] | None,
```

### Comparing `types-dateparser-1.1.4.9/dateparser-stubs/search/detection.pyi` & `types-dateparser-1.2.0.20240420/dateparser-stubs/search/detection.pyi`

 * *Files identical despite different names*

### Comparing `types-dateparser-1.1.4.9/dateparser-stubs/search/search.pyi` & `types-dateparser-1.2.0.20240420/dateparser-stubs/search/search.pyi`

 * *Files identical despite different names*

### Comparing `types-dateparser-1.1.4.9/dateparser-stubs/timezone_parser.pyi` & `types-dateparser-1.2.0.20240420/dateparser-stubs/timezone_parser.pyi`

 * *Files identical despite different names*

### Comparing `types-dateparser-1.1.4.9/dateparser-stubs/utils/__init__.pyi` & `types-dateparser-1.2.0.20240420/dateparser-stubs/utils/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -14,13 +14,14 @@
 def apply_dateparser_timezone(utc_datetime, offset_or_timezone_abb): ...
 def apply_timezone(date_time, tz_string): ...
 def apply_timezone_from_settings(date_obj, settings): ...
 def get_last_day_of_month(year, month): ...
 def get_previous_leap_year(year): ...
 def get_next_leap_year(year): ...
 def set_correct_day_from_settings(date_obj, settings, current_day: Incomplete | None = None): ...
+def set_correct_month_from_settings(date_obj, settings, current_month=None): ...
 def registry(cls): ...
 def get_logger() -> Any: ...
 def setup_logging() -> None: ...
 
 # TODO: this needs `types-pytz` and a type-alias
-def get_timezone_from_tz_string(tz_string: str) -> Incomplete: ...
+def get_timezone_from_tz_string(tz_string: str): ...
```

### Comparing `types-dateparser-1.1.4.9/setup.py` & `types-dateparser-1.2.0.20240420/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 from setuptools import setup
 
 name = "types-dateparser"
 description = "Typing stubs for dateparser"
 long_description = '''
 ## Typing stubs for dateparser
 
-This is a PEP 561 type stub package for the `dateparser` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`dateparser`](https://github.com/scrapinghub/dateparser) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`dateparser`. The source for this package can be found at
+`dateparser`.
+
+This version of `types-dateparser` aims to provide accurate annotations
+for `dateparser==1.2.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/dateparser. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `57f3dcac8dbed008479b251512975901a0206deb` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="1.1.4.9",
+      version="1.2.0.20240420",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dateparser.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['dateparser-stubs', 'dateparser_data-stubs'],
-      package_data={'dateparser-stubs': ['__init__.pyi', 'calendars/__init__.pyi', 'calendars/hijri.pyi', 'calendars/hijri_parser.pyi', 'calendars/jalali.pyi', 'calendars/jalali_parser.pyi', 'conf.pyi', 'custom_language_detection/__init__.pyi', 'custom_language_detection/fasttext.pyi', 'custom_language_detection/langdetect.pyi', 'custom_language_detection/language_mapping.pyi', 'data/__init__.pyi', 'data/languages_info.pyi', 'date.pyi', 'date_parser.pyi', 'freshness_date_parser.pyi', 'languages/__init__.pyi', 'languages/dictionary.pyi', 'languages/loader.pyi', 'languages/locale.pyi', 'languages/validation.pyi', 'parser.pyi', 'search/__init__.pyi', 'search/detection.pyi', 'search/search.pyi', 'search/text_detection.pyi', 'timezone_parser.pyi', 'timezones.pyi', 'utils/__init__.pyi', 'utils/strptime.pyi', 'METADATA.toml'], 'dateparser_data-stubs': ['__init__.pyi', 'settings.pyi', 'METADATA.toml']},
+      package_data={'dateparser-stubs': ['__init__.pyi', 'calendars/__init__.pyi', 'calendars/hijri.pyi', 'calendars/hijri_parser.pyi', 'calendars/jalali.pyi', 'calendars/jalali_parser.pyi', 'conf.pyi', 'custom_language_detection/__init__.pyi', 'custom_language_detection/fasttext.pyi', 'custom_language_detection/langdetect.pyi', 'custom_language_detection/language_mapping.pyi', 'data/__init__.pyi', 'data/languages_info.pyi', 'date.pyi', 'date_parser.pyi', 'freshness_date_parser.pyi', 'languages/__init__.pyi', 'languages/dictionary.pyi', 'languages/loader.pyi', 'languages/locale.pyi', 'languages/validation.pyi', 'parser.pyi', 'search/__init__.pyi', 'search/detection.pyi', 'search/search.pyi', 'search/text_detection.pyi', 'timezone_parser.pyi', 'timezones.pyi', 'utils/__init__.pyi', 'utils/strptime.pyi', 'METADATA.toml', 'py.typed'], 'dateparser_data-stubs': ['__init__.pyi', 'settings.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
+      python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-dateparser-1.1.4.9/types_dateparser.egg-info/PKG-INFO` & `types-dateparser-1.2.0.20240420/types_dateparser.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 Metadata-Version: 2.1
 Name: types-dateparser
-Version: 1.1.4.9
+Version: 1.2.0.20240420
 Summary: Typing stubs for dateparser
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dateparser.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for dateparser
 
-This is a PEP 561 type stub package for the `dateparser` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`dateparser`](https://github.com/scrapinghub/dateparser) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`dateparser`. The source for this package can be found at
+`dateparser`.
+
+This version of `types-dateparser` aims to provide accurate annotations
+for `dateparser==1.2.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/dateparser. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `57f3dcac8dbed008479b251512975901a0206deb` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-dateparser-1.1.4.9/types_dateparser.egg-info/SOURCES.txt` & `types-dateparser-1.2.0.20240420/types_dateparser.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 dateparser-stubs/METADATA.toml
 dateparser-stubs/__init__.pyi
 dateparser-stubs/conf.pyi
 dateparser-stubs/date.pyi
 dateparser-stubs/date_parser.pyi
 dateparser-stubs/freshness_date_parser.pyi
 dateparser-stubs/parser.pyi
+dateparser-stubs/py.typed
 dateparser-stubs/timezone_parser.pyi
 dateparser-stubs/timezones.pyi
 dateparser-stubs/calendars/__init__.pyi
 dateparser-stubs/calendars/hijri.pyi
 dateparser-stubs/calendars/hijri_parser.pyi
 dateparser-stubs/calendars/jalali.pyi
 dateparser-stubs/calendars/jalali_parser.pyi
@@ -30,12 +31,13 @@
 dateparser-stubs/search/detection.pyi
 dateparser-stubs/search/search.pyi
 dateparser-stubs/search/text_detection.pyi
 dateparser-stubs/utils/__init__.pyi
 dateparser-stubs/utils/strptime.pyi
 dateparser_data-stubs/METADATA.toml
 dateparser_data-stubs/__init__.pyi
+dateparser_data-stubs/py.typed
 dateparser_data-stubs/settings.pyi
 types_dateparser.egg-info/PKG-INFO
 types_dateparser.egg-info/SOURCES.txt
 types_dateparser.egg-info/dependency_links.txt
 types_dateparser.egg-info/top_level.txt
```

