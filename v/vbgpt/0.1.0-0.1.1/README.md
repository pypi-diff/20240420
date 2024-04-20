# Comparing `tmp/vbgpt-0.1.0.tar.gz` & `tmp/vbgpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbgpt-0.1.0.tar", max compression
+gzip compressed data, was "vbgpt-0.1.1.tar", max compression
```

## Comparing `vbgpt-0.1.0.tar` & `vbgpt-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-15 14:36:32.022624 vbgpt-0.1.0/README.md
--rw-r--r--   0        0        0      337 2024-04-15 14:38:50.947670 vbgpt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 14:36:32.022576 vbgpt-0.1.0/vbgpt/__init__.py
--rw-r--r--   0        0        0       47 2024-04-15 14:40:31.385581 vbgpt-0.1.0/vbgpt/__main__.py
--rw-r--r--   0        0        0     8413 2024-04-15 15:50:09.418375 vbgpt-0.1.0/vbgpt/main.py
--rw-r--r--   0        0        0      327 1970-01-01 00:00:00.000000 vbgpt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 14:36:32.022624 vbgpt-0.1.1/README.md
+-rw-r--r--   0        0        0      337 2024-04-20 16:03:36.614730 vbgpt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 14:36:32.022576 vbgpt-0.1.1/vbgpt/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-15 14:40:31.385581 vbgpt-0.1.1/vbgpt/__main__.py
+-rw-r--r--   0        0        0     8412 2024-04-20 16:03:23.415079 vbgpt-0.1.1/vbgpt/main.py
+-rw-r--r--   0        0        0      327 1970-01-01 00:00:00.000000 vbgpt-0.1.1/PKG-INFO
```

### Comparing `vbgpt-0.1.0/vbgpt/main.py` & `vbgpt-0.1.1/vbgpt/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,16 +261,16 @@
             render(path_gpt_temp, question, bgcolor)
 
 
 def get_ans_gpt(prompt):
     client = OpenAI()
 
     response = client.chat.completions.create(
-        model="gpt-3.5-turbo",
-        # model="gpt-4",
+        #model="gpt-3.5-turbo",
+        model="gpt-4",
         messages=[
             {
                 "role": "user",
                 "content": prompt
             }
         ],
         temperature=1,
```

