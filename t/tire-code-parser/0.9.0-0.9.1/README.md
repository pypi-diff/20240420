# Comparing `tmp/tire-code-parser-0.9.0.tar.gz` & `tmp/tire-code-parser-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tire-code-parser-0.9.0.tar", last modified: Sat Apr 20 18:10:13 2024, max compression
+gzip compressed data, was "tire-code-parser-0.9.1.tar", last modified: Sat Apr 20 18:17:15 2024, max compression
```

## Comparing `tire-code-parser-0.9.0.tar` & `tire-code-parser-0.9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 18:10:13.366527 tire-code-parser-0.9.0/
--rw-rw-rw-   0        0        0     1090 2024-03-18 15:02:29.000000 tire-code-parser-0.9.0/LICENSE
--rw-rw-rw-   0        0        0      372 2024-04-20 18:10:13.366527 tire-code-parser-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0       95 2024-03-18 16:01:52.000000 tire-code-parser-0.9.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-20 18:10:13.367527 tire-code-parser-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      500 2024-04-20 18:10:01.000000 tire-code-parser-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 18:10:13.343527 tire-code-parser-0.9.0/tire_code_parser/
--rw-rw-rw-   0        0        0       37 2024-04-20 18:00:43.000000 tire-code-parser-0.9.0/tire_code_parser/__init__.py
--rw-rw-rw-   0        0        0     2330 2024-01-19 01:35:13.000000 tire-code-parser-0.9.0/tire_code_parser/parser.py
-drwxrwxrwx   0        0        0        0 2024-04-20 18:10:13.364526 tire-code-parser-0.9.0/tire_code_parser.egg-info/
--rw-rw-rw-   0        0        0      372 2024-04-20 18:10:13.000000 tire-code-parser-0.9.0/tire_code_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-20 18:10:13.000000 tire-code-parser-0.9.0/tire_code_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 18:10:13.000000 tire-code-parser-0.9.0/tire_code_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-20 18:10:13.000000 tire-code-parser-0.9.0/tire_code_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 18:17:15.879726 tire-code-parser-0.9.1/
+-rw-rw-rw-   0        0        0     1090 2024-03-18 15:02:29.000000 tire-code-parser-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0      532 2024-04-20 18:17:15.878726 tire-code-parser-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      117 2024-04-20 18:16:40.000000 tire-code-parser-0.9.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 18:17:15.879726 tire-code-parser-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      682 2024-04-20 18:16:22.000000 tire-code-parser-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:17:15.860534 tire-code-parser-0.9.1/tire_code_parser/
+-rw-rw-rw-   0        0        0       37 2024-04-20 18:00:43.000000 tire-code-parser-0.9.1/tire_code_parser/__init__.py
+-rw-rw-rw-   0        0        0     2330 2024-01-19 01:35:13.000000 tire-code-parser-0.9.1/tire_code_parser/parser.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:17:15.877713 tire-code-parser-0.9.1/tire_code_parser.egg-info/
+-rw-rw-rw-   0        0        0      532 2024-04-20 18:17:15.000000 tire-code-parser-0.9.1/tire_code_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-04-20 18:17:15.000000 tire-code-parser-0.9.1/tire_code_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 18:17:15.000000 tire-code-parser-0.9.1/tire_code_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-20 18:17:15.000000 tire-code-parser-0.9.1/tire_code_parser.egg-info/top_level.txt
```

### Comparing `tire-code-parser-0.9.0/LICENSE` & `tire-code-parser-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tire-code-parser-0.9.0/tire_code_parser/parser.py` & `tire-code-parser-0.9.1/tire_code_parser/parser.py`

 * *Files identical despite different names*

