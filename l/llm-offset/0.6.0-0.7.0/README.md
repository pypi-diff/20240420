# Comparing `tmp/llm_offset-0.6.0.tar.gz` & `tmp/llm_offset-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_offset-0.6.0.tar", last modified: Sat Apr 20 20:38:00 2024, max compression
+gzip compressed data, was "llm_offset-0.7.0.tar", last modified: Sat Apr 20 20:41:05 2024, max compression
```

## Comparing `llm_offset-0.6.0.tar` & `llm_offset-0.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 20:38:00.489133 llm_offset-0.6.0/
--rw-r--r--   0 adityakakarla   (501) staff       (20)      188 2024-04-20 20:38:00.489015 llm_offset-0.6.0/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)       92 2024-04-20 20:35:51.000000 llm_offset-0.6.0/README.md
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 20:38:00.488050 llm_offset-0.6.0/llm_offset/
--rw-r--r--   0 adityakakarla   (501) staff       (20)       42 2024-04-20 05:05:02.000000 llm_offset-0.6.0/llm_offset/__init__.py
--rw-r--r--   0 adityakakarla   (501) staff       (20)      539 2024-04-20 20:32:50.000000 llm_offset-0.6.0/llm_offset/interceptor.py
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 20:38:00.488821 llm_offset-0.6.0/llm_offset.egg-info/
--rw-r--r--   0 adityakakarla   (501) staff       (20)      188 2024-04-20 20:38:00.000000 llm_offset-0.6.0/llm_offset.egg-info/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)      236 2024-04-20 20:38:00.000000 llm_offset-0.6.0/llm_offset.egg-info/SOURCES.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-20 20:38:00.000000 llm_offset-0.6.0/llm_offset.egg-info/dependency_links.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)        7 2024-04-20 20:38:00.000000 llm_offset-0.6.0/llm_offset.egg-info/requires.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       11 2024-04-20 20:38:00.000000 llm_offset-0.6.0/llm_offset.egg-info/top_level.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-20 20:38:00.489170 llm_offset-0.6.0/setup.cfg
--rw-r--r--   0 adityakakarla   (501) staff       (20)      322 2024-04-20 20:35:29.000000 llm_offset-0.6.0/setup.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 20:41:05.838641 llm_offset-0.7.0/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      188 2024-04-20 20:41:05.838521 llm_offset-0.7.0/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       92 2024-04-20 20:35:51.000000 llm_offset-0.7.0/README.md
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 20:41:05.837728 llm_offset-0.7.0/llm_offset/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       42 2024-04-20 05:05:02.000000 llm_offset-0.7.0/llm_offset/__init__.py
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      576 2024-04-20 20:40:34.000000 llm_offset-0.7.0/llm_offset/interceptor.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-20 20:41:05.838336 llm_offset-0.7.0/llm_offset.egg-info/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      188 2024-04-20 20:41:05.000000 llm_offset-0.7.0/llm_offset.egg-info/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      236 2024-04-20 20:41:05.000000 llm_offset-0.7.0/llm_offset.egg-info/SOURCES.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-20 20:41:05.000000 llm_offset-0.7.0/llm_offset.egg-info/dependency_links.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)        7 2024-04-20 20:41:05.000000 llm_offset-0.7.0/llm_offset.egg-info/requires.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       11 2024-04-20 20:41:05.000000 llm_offset-0.7.0/llm_offset.egg-info/top_level.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-20 20:41:05.838678 llm_offset-0.7.0/setup.cfg
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      322 2024-04-20 20:40:45.000000 llm_offset-0.7.0/setup.py
```

### Comparing `llm_offset-0.6.0/llm_offset/interceptor.py` & `llm_offset-0.7.0/llm_offset/interceptor.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,13 +3,13 @@
         def wrapper(*args, **kwargs):
             result = func(*args, **kwargs)
             print(f"Sending notification to {email}")
             return result
         return wrapper
     return decorator
 
-def log_call(openai, email):
-    original_text = openai.chat.completions.create
-    openai.chat.completions.create = llm_offset_decorator(email)(original_text)
+def log_call(openai_client, email):
+    original_text = openai_client.chat.completions.create
+    openai_client.chat.completions.create = llm_offset_decorator(email)(original_text)
 
-    original_image = openai.image.generate
-    openai.image.generate = llm_offset_decorator(email)(original_image)
+    original_image = openai_client.images.generate
+    openai_client.images.generate = llm_offset_decorator(email)(original_image)
```

