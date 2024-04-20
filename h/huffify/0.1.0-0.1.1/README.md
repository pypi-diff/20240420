# Comparing `tmp/huffify-0.1.0.tar.gz` & `tmp/huffify-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huffify-0.1.0.tar", max compression
+gzip compressed data, was "huffify-0.1.1.tar", max compression
```

## Comparing `huffify-0.1.0.tar` & `huffify-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-04-07 11:32:50.153169 huffify-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2024-04-06 18:40:43.735422 huffify-0.1.0/README.md
--rw-r--r--   0        0        0      886 2024-04-20 15:29:53.223652 huffify-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       65 2024-04-07 09:48:05.662914 huffify-0.1.0/src/huffify/__init__.py
--rw-r--r--   0        0        0      654 2024-04-07 11:19:45.464909 huffify-0.1.0/src/huffify/abstract.py
--rw-r--r--   0        0        0      111 2024-04-14 19:07:11.514806 huffify-0.1.0/src/huffify/annotations.py
--rw-r--r--   0        0        0     2691 2024-04-20 13:22:48.579606 huffify-0.1.0/src/huffify/encoders.py
--rw-r--r--   0        0        0      765 2024-04-07 09:48:06.382903 huffify-0.1.0/src/huffify/fileManger.py
--rw-r--r--   0        0        0      909 2024-04-06 19:12:01.753211 huffify-0.1.0/src/huffify/heapNodes.py
--rw-r--r--   0        0        0     2578 2024-04-20 13:22:32.486829 huffify-0.1.0/src/huffify/huffify.py
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 huffify-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-20 16:45:06.233524 huffify-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-20 16:45:06.233524 huffify-0.1.1/README.md
+-rw-r--r--   0        0        0      846 2024-04-20 16:45:06.233524 huffify-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       65 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/abstract.py
+-rw-r--r--   0        0        0      111 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/annotations.py
+-rw-r--r--   0        0        0     2691 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/encoders.py
+-rw-r--r--   0        0        0      765 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/fileManger.py
+-rw-r--r--   0        0        0      909 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/heapNodes.py
+-rw-r--r--   0        0        0     2578 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/huffify.py
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 huffify-0.1.1/PKG-INFO
```

### Comparing `huffify-0.1.0/LICENSE` & `huffify-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `huffify-0.1.0/pyproject.toml` & `huffify-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 [tool.poetry]
 name = "huffify"
-version = "0.1.0"
+version = "0.1.1"
 description = "Simple Huffman algotithm implementation"
 authors = ["munwriter <glebvysokov3@gmail.com>"]
 keywords = ["huffman", "compression", "encoding", "decoding"]
 repository = "https://github.com/munwriter/Huffify"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
-setuptools = "^69.0.3"
-wheel = "^0.42.0"
-twine = "^4.0.2"
-pytest = "^8.0.0"
 
 [tool.poetry.group.dev.dependencies]
+pytest = "^8.0.0"
 black = "^23.12.1"
 mypy = "^1.8.0"
 isort = "^5.13.2"
 ruff = "^0.3.5"
 
 [tool.mypy]
 python_version = "3.12"
@@ -41,7 +38,8 @@
 line-length=95
 target-version = "py312"
 show-fixes = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+exclude = "/tests"
```

### Comparing `huffify-0.1.0/src/huffify/abstract.py` & `huffify-0.1.1/src/huffify/abstract.py`

 * *Files identical despite different names*

### Comparing `huffify-0.1.0/src/huffify/encoders.py` & `huffify-0.1.1/src/huffify/encoders.py`

 * *Files identical despite different names*

### Comparing `huffify-0.1.0/src/huffify/fileManger.py` & `huffify-0.1.1/src/huffify/fileManger.py`

 * *Files identical despite different names*

### Comparing `huffify-0.1.0/src/huffify/heapNodes.py` & `huffify-0.1.1/src/huffify/heapNodes.py`

 * *Files identical despite different names*

### Comparing `huffify-0.1.0/src/huffify/huffify.py` & `huffify-0.1.1/src/huffify/huffify.py`

 * *Files identical despite different names*

