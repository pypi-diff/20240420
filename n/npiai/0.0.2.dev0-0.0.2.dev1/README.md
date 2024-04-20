# Comparing `tmp/npiai-0.0.2.dev0.tar.gz` & `tmp/npiai-0.0.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npiai-0.0.2.dev0.tar", max compression
+gzip compressed data, was "npiai-0.0.2.dev1.tar", max compression
```

## Comparing `npiai-0.0.2.dev0.tar` & `npiai-0.0.2.dev1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-18 05:31:48.474805 npiai-0.0.2.dev0/README.md
--rw-r--r--   0        0        0      151 2024-04-20 00:39:52.418936 npiai-0.0.2.dev0/npiai/__init__.py
--rw-r--r--   0        0        0      132 2024-04-20 00:26:15.294019 npiai-0.0.2.dev0/npiai/app/__init__.py
--rw-r--r--   0        0        0      510 2024-04-20 00:09:40.569381 npiai-0.0.2.dev0/npiai/app/google.py
--rw-r--r--   0        0        0     1090 2024-04-20 00:09:40.565760 npiai-0.0.2.dev0/npiai/app/human_feedback.py
--rw-r--r--   0        0        0       57 2024-04-20 00:26:15.289527 npiai-0.0.2.dev0/npiai/core/__init__.py
--rw-r--r--   0        0        0     6106 2024-04-20 00:09:40.560265 npiai-0.0.2.dev0/npiai/core/base.py
--rw-r--r--   0        0        0      367 2024-04-20 00:45:08.001682 npiai-0.0.2.dev0/pyproject.toml
--rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 npiai-0.0.2.dev0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 05:31:48.474805 npiai-0.0.2.dev1/README.md
+-rw-r--r--   0        0        0      151 2024-04-20 00:39:52.418936 npiai-0.0.2.dev1/npiai/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-20 00:26:15.294019 npiai-0.0.2.dev1/npiai/app/__init__.py
+-rw-r--r--   0        0        0      510 2024-04-20 00:09:40.569381 npiai-0.0.2.dev1/npiai/app/google.py
+-rw-r--r--   0        0        0     1090 2024-04-20 00:09:40.565760 npiai-0.0.2.dev1/npiai/app/human_feedback.py
+-rw-r--r--   0        0        0       57 2024-04-20 00:26:15.289527 npiai-0.0.2.dev1/npiai/core/__init__.py
+-rw-r--r--   0        0        0     6106 2024-04-20 00:09:40.560265 npiai-0.0.2.dev1/npiai/core/base.py
+-rw-r--r--   0        0        0      371 2024-04-20 00:57:24.762607 npiai-0.0.2.dev1/pyproject.toml
+-rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 npiai-0.0.2.dev1/PKG-INFO
```

### Comparing `npiai-0.0.2.dev0/npiai/app/human_feedback.py` & `npiai-0.0.2.dev1/npiai/app/human_feedback.py`

 * *Files identical despite different names*

### Comparing `npiai-0.0.2.dev0/npiai/core/base.py` & `npiai-0.0.2.dev1/npiai/core/base.py`

 * *Files identical despite different names*

