# Comparing `tmp/grabberlib-0.0.8.tar.gz` & `tmp/grabberlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.0.8.tar", max compression
+gzip compressed data, was "grabberlib-0.0.9.tar", max compression
```

## Comparing `grabberlib-0.0.8.tar` & `grabberlib-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.755675 grabberlib-0.0.8/README.md
--rw-r--r--   0        0        0        1 2024-04-20 14:47:15.755675 grabberlib-0.0.8/assets/pages.txt
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/__main__.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/controllers/__init__.py
--rw-r--r--   0        0        0     4026 2024-04-20 15:37:09.641442 grabberlib-0.0.8/grabber/controllers/base.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/core/__init__.py
--rw-r--r--   0        0        0       65 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/core/exc.py
--rw-r--r--   0        0        0      446 2024-04-20 15:06:51.092892 grabberlib-0.0.8/grabber/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/core/sources/__init__.py
--rw-r--r--   0        0        0     3400 2024-04-20 15:08:46.386081 grabberlib-0.0.8/grabber/core/sources/graph.py
--rw-r--r--   0        0        0     4008 2024-04-20 15:09:05.377639 grabberlib-0.0.8/grabber/core/sources/khd.py
--rw-r--r--   0        0        0     3610 2024-04-20 15:09:24.729188 grabberlib-0.0.8/grabber/core/sources/xasiat.py
--rw-r--r--   0        0        0     3871 2024-04-20 15:32:13.229448 grabberlib-0.0.8/grabber/core/sources/xiuren.py
--rw-r--r--   0        0        0        1 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/core/sources/yellow.py
--rw-r--r--   0        0        0    13127 2024-04-20 15:12:16.745134 grabberlib-0.0.8/grabber/core/utils.py
--rw-r--r--   0        0        0      175 2024-04-20 15:32:24.269170 grabberlib-0.0.8/grabber/core/version.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/templates/__init__.py
--rw-r--r--   0        0        0     1017 2024-04-20 15:32:18.045327 grabberlib-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.755675 grabberlib-0.0.9/README.md
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.755675 grabberlib-0.0.9/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     4066 2024-04-20 15:40:45.571619 grabberlib-0.0.9/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/core/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/core/exc.py
+-rw-r--r--   0        0        0      446 2024-04-20 15:06:51.092892 grabberlib-0.0.9/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0     3400 2024-04-20 15:08:46.386081 grabberlib-0.0.9/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     4008 2024-04-20 15:09:05.377639 grabberlib-0.0.9/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     3610 2024-04-20 15:09:24.729188 grabberlib-0.0.9/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     3871 2024-04-20 15:32:13.229448 grabberlib-0.0.9/grabber/core/sources/xiuren.py
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0    13127 2024-04-20 15:12:16.745134 grabberlib-0.0.9/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-04-20 15:40:55.979342 grabberlib-0.0.9/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1017 2024-04-20 15:40:50.431490 grabberlib-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.9/PKG-INFO
```

### Comparing `grabberlib-0.0.8/grabber/__main__.py` & `grabberlib-0.0.9/grabber/__main__.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.8/grabber/controllers/base.py` & `grabberlib-0.0.9/grabber/controllers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,17 @@
                     "action": "store_true",
                     "help": "Indicates that the link(s) passed is a tag in which the posts are paginated",
                 },
             ),
             (
                 ["-v", "--version"],
                 {
-                    "action": "version",
-                    "version": VERSION_BANNER,
+                    "action": "store_true",
+                    "dest": "version",
+                    "help": "Version of the lib",
                 },
             ),
         ]
 
     @ex(hide=True)
     def _default(self):
         """Default action if no sub-command is passed."""
@@ -102,15 +103,15 @@
         folder = self.app.pargs.folder
         publish = self.app.pargs.publish
         upload = self.app.pargs.upload
         is_tag = self.app.pargs.is_tag
         limit = self.app.pargs.limit
         version = self.app.pargs.version
         if version:
-            self.app.args.print_help()
+            print(VERSION_BANNER)
             return
 
         getter_mapping = {
             "4khd": get_sources_for_4khd,
             "telegraph": get_for_telegraph,
             "xiuren": get_sources_for_xiuren,
         }
```

### Comparing `grabberlib-0.0.8/grabber/core/sources/graph.py` & `grabberlib-0.0.9/grabber/core/sources/graph.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.8/grabber/core/sources/khd.py` & `grabberlib-0.0.9/grabber/core/sources/khd.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.8/grabber/core/sources/xasiat.py` & `grabberlib-0.0.9/grabber/core/sources/xasiat.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.8/grabber/core/sources/xiuren.py` & `grabberlib-0.0.9/grabber/core/sources/xiuren.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.8/grabber/core/utils.py` & `grabberlib-0.0.9/grabber/core/utils.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.8/pyproject.toml` & `grabberlib-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
     { include = "assets/pages.txt" },
 ]
```

### Comparing `grabberlib-0.0.8/PKG-INFO` & `grabberlib-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

