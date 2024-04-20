# Comparing `tmp/llm_offset-0.4.0.tar.gz` & `tmp/llm_offset-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_offset-0.4.0.tar", last modified: Sat Apr 20 04:47:59 2024, max compression
+gzip compressed data, was "llm_offset-0.5.0.tar", last modified: Sat Apr 20 05:00:48 2024, max compression
```

## Comparing `llm_offset-0.4.0.tar` & `llm_offset-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:47:59.896219 llm_offset-0.4.0/
--rw-r--r--   0 adityakakarla   (501) staff       (20)      187 2024-04-20 04:47:59.896055 llm_offset-0.4.0/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)       91 2024-04-20 04:01:32.000000 llm_offset-0.4.0/README.md
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:47:59.894720 llm_offset-0.4.0/llm_offset/
--rw-r--r--   0 adityakakarla   (501) staff       (20)       33 2024-04-20 04:47:54.000000 llm_offset-0.4.0/llm_offset/__init__.py
--rw-r--r--   0 adityakakarla   (501) staff       (20)      414 2024-04-20 04:45:52.000000 llm_offset-0.4.0/llm_offset/interceptor.py
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:47:59.895811 llm_offset-0.4.0/llm_offset.egg-info/
--rw-r--r--   0 adityakakarla   (501) staff       (20)      187 2024-04-20 04:47:59.000000 llm_offset-0.4.0/llm_offset.egg-info/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)      236 2024-04-20 04:47:59.000000 llm_offset-0.4.0/llm_offset.egg-info/SOURCES.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-20 04:47:59.000000 llm_offset-0.4.0/llm_offset.egg-info/dependency_links.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)        7 2024-04-20 04:47:59.000000 llm_offset-0.4.0/llm_offset.egg-info/requires.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       11 2024-04-20 04:47:59.000000 llm_offset-0.4.0/llm_offset.egg-info/top_level.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-20 04:47:59.896263 llm_offset-0.4.0/setup.cfg
--rw-r--r--   0 adityakakarla   (501) staff       (20)      322 2024-04-20 04:46:46.000000 llm_offset-0.4.0/setup.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 05:00:48.102571 llm_offset-0.5.0/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      187 2024-04-20 05:00:48.102453 llm_offset-0.5.0/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       91 2024-04-20 04:01:32.000000 llm_offset-0.5.0/README.md
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 05:00:48.101478 llm_offset-0.5.0/llm_offset/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       44 2024-04-20 05:00:31.000000 llm_offset-0.5.0/llm_offset/__init__.py
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      414 2024-04-20 04:45:52.000000 llm_offset-0.5.0/llm_offset/interceptor.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 05:00:48.102301 llm_offset-0.5.0/llm_offset.egg-info/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      187 2024-04-20 05:00:48.000000 llm_offset-0.5.0/llm_offset.egg-info/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      236 2024-04-20 05:00:48.000000 llm_offset-0.5.0/llm_offset.egg-info/SOURCES.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-20 05:00:48.000000 llm_offset-0.5.0/llm_offset.egg-info/dependency_links.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)        7 2024-04-20 05:00:48.000000 llm_offset-0.5.0/llm_offset.egg-info/requires.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       11 2024-04-20 05:00:48.000000 llm_offset-0.5.0/llm_offset.egg-info/top_level.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-20 05:00:48.102613 llm_offset-0.5.0/setup.cfg
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      322 2024-04-20 05:00:39.000000 llm_offset-0.5.0/setup.py
```

