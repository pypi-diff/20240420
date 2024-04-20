# Comparing `tmp/llm_offset-0.1.tar.gz` & `tmp/llm_offset-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_offset-0.1.tar", last modified: Sat Apr 20 04:00:38 2024, max compression
+gzip compressed data, was "llm_offset-0.2.0.tar", last modified: Sat Apr 20 04:24:56 2024, max compression
```

## Comparing `llm_offset-0.1.tar` & `llm_offset-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:00:38.610623 llm_offset-0.1/
--rw-r--r--   0 adityakakarla   (501) staff       (20)       52 2024-04-20 04:00:38.610491 llm_offset-0.1/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)       12 2024-04-20 03:51:10.000000 llm_offset-0.1/README.md
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:00:38.609757 llm_offset-0.1/llm_offset/
--rw-r--r--   0 adityakakarla   (501) staff       (20)       25 2024-04-20 03:55:27.000000 llm_offset-0.1/llm_offset/__init__.py
--rw-r--r--   0 adityakakarla   (501) staff       (20)       47 2024-04-20 03:54:44.000000 llm_offset-0.1/llm_offset/main.py
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:00:38.610343 llm_offset-0.1/llm_offset.egg-info/
--rw-r--r--   0 adityakakarla   (501) staff       (20)       52 2024-04-20 04:00:38.000000 llm_offset-0.1/llm_offset.egg-info/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)      196 2024-04-20 04:00:38.000000 llm_offset-0.1/llm_offset.egg-info/SOURCES.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-20 04:00:38.000000 llm_offset-0.1/llm_offset.egg-info/dependency_links.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       11 2024-04-20 04:00:38.000000 llm_offset-0.1/llm_offset.egg-info/top_level.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-20 04:00:38.610660 llm_offset-0.1/setup.cfg
--rw-r--r--   0 adityakakarla   (501) staff       (20)      156 2024-04-20 04:00:15.000000 llm_offset-0.1/setup.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:24:56.132465 llm_offset-0.2.0/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      187 2024-04-20 04:24:56.132338 llm_offset-0.2.0/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       91 2024-04-20 04:01:32.000000 llm_offset-0.2.0/README.md
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:24:56.131448 llm_offset-0.2.0/llm_offset/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       25 2024-04-20 03:55:27.000000 llm_offset-0.2.0/llm_offset/__init__.py
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       47 2024-04-20 03:54:44.000000 llm_offset-0.2.0/llm_offset/main.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:24:56.132164 llm_offset-0.2.0/llm_offset.egg-info/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      187 2024-04-20 04:24:56.000000 llm_offset-0.2.0/llm_offset.egg-info/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      196 2024-04-20 04:24:56.000000 llm_offset-0.2.0/llm_offset.egg-info/SOURCES.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-20 04:24:56.000000 llm_offset-0.2.0/llm_offset.egg-info/dependency_links.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       11 2024-04-20 04:24:56.000000 llm_offset-0.2.0/llm_offset.egg-info/top_level.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-20 04:24:56.132503 llm_offset-0.2.0/setup.cfg
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      306 2024-04-20 04:24:50.000000 llm_offset-0.2.0/setup.py
```

