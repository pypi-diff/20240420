# Comparing `tmp/kfsconfig-1.1.0.tar.gz` & `tmp/kfsconfig-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsconfig-1.1.0.tar", max compression
+gzip compressed data, was "kfsconfig-1.2.0.tar", max compression
```

## Comparing `kfsconfig-1.1.0.tar` & `kfsconfig-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     4195 2023-12-04 10:14:05.656015 kfsconfig-1.1.0/KFSconfig/KFSconfig.py
--rw-r--r--   0        0        0        0 2023-12-04 10:14:05.656015 kfsconfig-1.1.0/KFSconfig/__init__.py
--rw-r--r--   0        0        0      515 2023-12-04 10:14:05.656015 kfsconfig-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      668 2023-12-04 10:14:05.656015 kfsconfig-1.1.0/readme.md
--rw-r--r--   0        0        0     1236 1970-01-01 00:00:00.000000 kfsconfig-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7245 2024-04-20 12:50:38.852606 kfsconfig-1.2.0/KFSconfig/KFSconfig.py
+-rw-r--r--   0        0        0      515 2024-04-20 12:50:38.852606 kfsconfig-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-04-20 12:50:38.852606 kfsconfig-1.2.0/readme.md
+-rw-r--r--   0        0        0     1236 1970-01-01 00:00:00.000000 kfsconfig-1.2.0/PKG-INFO
```

### Comparing `kfsconfig-1.1.0/pyproject.toml` & `kfsconfig-1.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors     = ["9FS <pray4spam@googlemail.com>"]
 description = ""
 license     = "MIT"
 name        = "KFSconfig"
 packages    = [{ include = "KFSconfig" }]
 readme      = "readme.md"
 repository  = "https://github.com/9-FS/2023-09-20-KFSconfig"
-version     = "1.1.0"
+version     = "1.2.0"
 
 [tool.poetry.dependencies]
 KFSlog = "^1.0.0"
 python = "^3.11.0"
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "^6.87.0"
```

### Comparing `kfsconfig-1.1.0/readme.md` & `kfsconfig-1.2.0/readme.md`

 * *Files identical despite different names*

### Comparing `kfsconfig-1.1.0/PKG-INFO` & `kfsconfig-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KFSconfig
-Version: 1.1.0
+Version: 1.2.0
 Summary: 
 Home-page: https://github.com/9-FS/2023-09-20-KFSconfig
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

