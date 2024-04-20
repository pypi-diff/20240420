# Comparing `tmp/tire-code-parser-0.8.0.tar.gz` & `tmp/tire-code-parser-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tire-code-parser-0.8.0.tar", last modified: Sat Apr 20 18:02:24 2024, max compression
+gzip compressed data, was "tire-code-parser-0.9.0.tar", last modified: Sat Apr 20 18:10:13 2024, max compression
```

## Comparing `tire-code-parser-0.8.0.tar` & `tire-code-parser-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 18:02:24.564194 tire-code-parser-0.8.0/
--rw-rw-rw-   0        0        0     1090 2024-03-18 15:02:29.000000 tire-code-parser-0.8.0/LICENSE
--rw-rw-rw-   0        0        0      372 2024-04-20 18:02:24.563233 tire-code-parser-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0       95 2024-03-18 16:01:52.000000 tire-code-parser-0.8.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-20 18:02:24.564194 tire-code-parser-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0      504 2024-04-20 18:02:05.000000 tire-code-parser-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 18:02:24.535183 tire-code-parser-0.8.0/tire_code_parser/
--rw-rw-rw-   0        0        0       37 2024-04-20 18:00:43.000000 tire-code-parser-0.8.0/tire_code_parser/__init__.py
--rw-rw-rw-   0        0        0     2330 2024-01-19 01:35:13.000000 tire-code-parser-0.8.0/tire_code_parser/parser.py
-drwxrwxrwx   0        0        0        0 2024-04-20 18:02:24.561177 tire-code-parser-0.8.0/tire_code_parser.egg-info/
--rw-rw-rw-   0        0        0      372 2024-04-20 18:02:24.000000 tire-code-parser-0.8.0/tire_code_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-04-20 18:02:24.000000 tire-code-parser-0.8.0/tire_code_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 18:02:24.000000 tire-code-parser-0.8.0/tire_code_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-04-20 18:02:24.000000 tire-code-parser-0.8.0/tire_code_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-20 18:02:24.000000 tire-code-parser-0.8.0/tire_code_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 18:10:13.366527 tire-code-parser-0.9.0/
+-rw-rw-rw-   0        0        0     1090 2024-03-18 15:02:29.000000 tire-code-parser-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      372 2024-04-20 18:10:13.366527 tire-code-parser-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       95 2024-03-18 16:01:52.000000 tire-code-parser-0.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 18:10:13.367527 tire-code-parser-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      500 2024-04-20 18:10:01.000000 tire-code-parser-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:10:13.343527 tire-code-parser-0.9.0/tire_code_parser/
+-rw-rw-rw-   0        0        0       37 2024-04-20 18:00:43.000000 tire-code-parser-0.9.0/tire_code_parser/__init__.py
+-rw-rw-rw-   0        0        0     2330 2024-01-19 01:35:13.000000 tire-code-parser-0.9.0/tire_code_parser/parser.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:10:13.364526 tire-code-parser-0.9.0/tire_code_parser.egg-info/
+-rw-rw-rw-   0        0        0      372 2024-04-20 18:10:13.000000 tire-code-parser-0.9.0/tire_code_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-04-20 18:10:13.000000 tire-code-parser-0.9.0/tire_code_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 18:10:13.000000 tire-code-parser-0.9.0/tire_code_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-20 18:10:13.000000 tire-code-parser-0.9.0/tire_code_parser.egg-info/top_level.txt
```

### Comparing `tire-code-parser-0.8.0/LICENSE` & `tire-code-parser-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tire-code-parser-0.8.0/tire_code_parser/parser.py` & `tire-code-parser-0.9.0/tire_code_parser/parser.py`

 * *Files identical despite different names*

