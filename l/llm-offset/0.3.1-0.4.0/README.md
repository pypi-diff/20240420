# Comparing `tmp/llm_offset-0.3.1.tar.gz` & `tmp/llm_offset-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_offset-0.3.1.tar", last modified: Sat Apr 20 04:30:16 2024, max compression
+gzip compressed data, was "llm_offset-0.4.0.tar", last modified: Sat Apr 20 04:47:59 2024, max compression
```

## Comparing `llm_offset-0.3.1.tar` & `llm_offset-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:30:16.204460 llm_offset-0.3.1/
--rw-r--r--   0 adityakakarla   (501) staff       (20)      187 2024-04-20 04:30:16.204346 llm_offset-0.3.1/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)       91 2024-04-20 04:01:32.000000 llm_offset-0.3.1/README.md
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:30:16.203776 llm_offset-0.3.1/llm_offset/
--rw-r--r--   0 adityakakarla   (501) staff       (20)       25 2024-04-20 03:55:27.000000 llm_offset-0.3.1/llm_offset/__init__.py
--rw-r--r--   0 adityakakarla   (501) staff       (20)       47 2024-04-20 03:54:44.000000 llm_offset-0.3.1/llm_offset/main.py
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:30:16.204189 llm_offset-0.3.1/llm_offset.egg-info/
--rw-r--r--   0 adityakakarla   (501) staff       (20)      187 2024-04-20 04:30:16.000000 llm_offset-0.3.1/llm_offset.egg-info/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)      196 2024-04-20 04:30:16.000000 llm_offset-0.3.1/llm_offset.egg-info/SOURCES.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-20 04:30:16.000000 llm_offset-0.3.1/llm_offset.egg-info/dependency_links.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       11 2024-04-20 04:30:16.000000 llm_offset-0.3.1/llm_offset.egg-info/top_level.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-20 04:30:16.204497 llm_offset-0.3.1/setup.cfg
--rw-r--r--   0 adityakakarla   (501) staff       (20)      306 2024-04-20 04:30:13.000000 llm_offset-0.3.1/setup.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:47:59.896219 llm_offset-0.4.0/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      187 2024-04-20 04:47:59.896055 llm_offset-0.4.0/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       91 2024-04-20 04:01:32.000000 llm_offset-0.4.0/README.md
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:47:59.894720 llm_offset-0.4.0/llm_offset/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       33 2024-04-20 04:47:54.000000 llm_offset-0.4.0/llm_offset/__init__.py
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      414 2024-04-20 04:45:52.000000 llm_offset-0.4.0/llm_offset/interceptor.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 04:47:59.895811 llm_offset-0.4.0/llm_offset.egg-info/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      187 2024-04-20 04:47:59.000000 llm_offset-0.4.0/llm_offset.egg-info/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      236 2024-04-20 04:47:59.000000 llm_offset-0.4.0/llm_offset.egg-info/SOURCES.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-20 04:47:59.000000 llm_offset-0.4.0/llm_offset.egg-info/dependency_links.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)        7 2024-04-20 04:47:59.000000 llm_offset-0.4.0/llm_offset.egg-info/requires.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       11 2024-04-20 04:47:59.000000 llm_offset-0.4.0/llm_offset.egg-info/top_level.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-20 04:47:59.896263 llm_offset-0.4.0/setup.cfg
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      322 2024-04-20 04:46:46.000000 llm_offset-0.4.0/setup.py
```

