# Comparing `tmp/grabberlib-0.0.7.tar.gz` & `tmp/grabberlib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.0.7.tar", max compression
+gzip compressed data, was "grabberlib-0.0.8.tar", max compression
```

## Comparing `grabberlib-0.0.7.tar` & `grabberlib-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.755675 grabberlib-0.0.7/README.md
--rw-r--r--   0        0        0        1 2024-04-20 14:47:15.755675 grabberlib-0.0.7/assets/pages.txt
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/__main__.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/controllers/__init__.py
--rw-r--r--   0        0        0     3798 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/controllers/base.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/core/__init__.py
--rw-r--r--   0        0        0       65 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/core/exc.py
--rw-r--r--   0        0        0      446 2024-04-20 15:06:51.092892 grabberlib-0.0.7/grabber/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/core/sources/__init__.py
--rw-r--r--   0        0        0     3400 2024-04-20 15:08:46.386081 grabberlib-0.0.7/grabber/core/sources/graph.py
--rw-r--r--   0        0        0     4008 2024-04-20 15:09:05.377639 grabberlib-0.0.7/grabber/core/sources/khd.py
--rw-r--r--   0        0        0     3610 2024-04-20 15:09:24.729188 grabberlib-0.0.7/grabber/core/sources/xasiat.py
--rw-r--r--   0        0        0     3740 2024-04-20 15:09:41.284801 grabberlib-0.0.7/grabber/core/sources/xiuren.py
--rw-r--r--   0        0        0        1 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/core/sources/yellow.py
--rw-r--r--   0        0        0    13127 2024-04-20 15:12:16.745134 grabberlib-0.0.7/grabber/core/utils.py
--rw-r--r--   0        0        0      175 2024-04-20 15:10:47.699240 grabberlib-0.0.7/grabber/core/version.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/templates/__init__.py
--rw-r--r--   0        0        0     1017 2024-04-20 15:10:40.347413 grabberlib-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.755675 grabberlib-0.0.8/README.md
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.755675 grabberlib-0.0.8/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     4026 2024-04-20 15:37:09.641442 grabberlib-0.0.8/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/core/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/core/exc.py
+-rw-r--r--   0        0        0      446 2024-04-20 15:06:51.092892 grabberlib-0.0.8/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0     3400 2024-04-20 15:08:46.386081 grabberlib-0.0.8/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     4008 2024-04-20 15:09:05.377639 grabberlib-0.0.8/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     3610 2024-04-20 15:09:24.729188 grabberlib-0.0.8/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     3871 2024-04-20 15:32:13.229448 grabberlib-0.0.8/grabber/core/sources/xiuren.py
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0    13127 2024-04-20 15:12:16.745134 grabberlib-0.0.8/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-04-20 15:32:24.269170 grabberlib-0.0.8/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.8/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1017 2024-04-20 15:32:18.045327 grabberlib-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.8/PKG-INFO
```

### Comparing `grabberlib-0.0.7/grabber/__main__.py` & `grabberlib-0.0.8/grabber/__main__.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.7/grabber/controllers/base.py` & `grabberlib-0.0.8/grabber/controllers/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from cement import Controller, ex
-from cement.utils.version import get_version_banner
 
 from grabber.core.sources.graph import get_for_telegraph
 from grabber.core.sources.khd import get_sources_for_4khd
 from grabber.core.sources.xiuren import get_sources_for_xiuren
 from grabber.core.utils import upload_folders_to_telegraph
 
 from ..core.version import get_version
 
-VERSION_BANNER = """
-A beautiful CLI utility to download images from the web! %s
-%s
-""" % (get_version(), get_version_banner())
+VERSION_BANNER = f"""
+A beautiful CLI utility to download images from the web! {get_version()}
+"""
 
 
 class Base(Controller):
     class Meta:
         label = "base"
 
         # text displayed at the top of --help output
@@ -29,15 +27,15 @@
             ### add a version banner
             (
                 ["-e", "--entity"],
                 {
                     "dest": "entity",
                     "type": str,
                     "help": "Webtsite name from where it will be download",
-                },
+               },
             ),
             (
                 ["-s", "--sources"],
                 {
                     "dest": "sources",
                     "type": str,
                     "help": "List of links",
@@ -82,27 +80,38 @@
                 ["-t", "--tag"],
                 {
                     "dest": "is_tag",
                     "action": "store_true",
                     "help": "Indicates that the link(s) passed is a tag in which the posts are paginated",
                 },
             ),
+            (
+                ["-v", "--version"],
+                {
+                    "action": "version",
+                    "version": VERSION_BANNER,
+                },
+            ),
         ]
 
     @ex(hide=True)
     def _default(self):
         """Default action if no sub-command is passed."""
 
         entity = self.app.pargs.entity
         sources = self.app.pargs.sources
         folder = self.app.pargs.folder
         publish = self.app.pargs.publish
         upload = self.app.pargs.upload
         is_tag = self.app.pargs.is_tag
         limit = self.app.pargs.limit
+        version = self.app.pargs.version
+        if version:
+            self.app.args.print_help()
+            return
 
         getter_mapping = {
             "4khd": get_sources_for_4khd,
             "telegraph": get_for_telegraph,
             "xiuren": get_sources_for_xiuren,
         }
```

### Comparing `grabberlib-0.0.7/grabber/core/sources/graph.py` & `grabberlib-0.0.8/grabber/core/sources/graph.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.7/grabber/core/sources/khd.py` & `grabberlib-0.0.8/grabber/core/sources/khd.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.7/grabber/core/sources/xasiat.py` & `grabberlib-0.0.8/grabber/core/sources/xasiat.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.7/grabber/core/sources/xiuren.py` & `grabberlib-0.0.8/grabber/core/sources/xiuren.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,14 +110,16 @@
     ):
         future.result()
 
     if save_to_telegraph:
         for title, (_, folder_dest) in title_folder_mapping.items():
             upload_to_telegraph(folder_dest, page_title=title)
 
-    albums_message = "".join([f"- {title}\n" for title in titles])
+    albums_file = pathlib.Path(get_media_root() / "assets/pages.txt")
+    albums_links = albums_file.read_text().split("\n")
+    albums_message = "".join([f"- {album}\n" for album in albums_links])
     message = f"""
-    All images have been downloaded and saved to the specified folder.
+    All albums have been downloaded and saved to the specified folder.
     Albums saved are the following:
         {albums_message}
     """
     print(message)
```

### Comparing `grabberlib-0.0.7/grabber/core/utils.py` & `grabberlib-0.0.8/grabber/core/utils.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.7/pyproject.toml` & `grabberlib-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
     { include = "assets/pages.txt" },
 ]
```

### Comparing `grabberlib-0.0.7/PKG-INFO` & `grabberlib-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

