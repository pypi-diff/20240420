# Comparing `tmp/pg_podcast_toolkit-0.0.5.tar.gz` & `tmp/pg_podcast_toolkit-0.0.6.tar.gz`

## Comparing `pg_podcast_toolkit-0.0.5.tar` & `pg_podcast_toolkit-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0   273506 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/bballrss.xml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/buildpublish.sh
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/go_ssh_tunnel.sh
--rw-r--r--   0        0        0   261174 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/look.xml
--rw-r--r--   0        0        0   350044 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/output.xml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/requirements.txt
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/test_ssh_tunnel.sh
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/src/pg_podcast_toolkit/__init__.py
--rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/src/pg_podcast_toolkit/item.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/src/pg_podcast_toolkit/media_resource.py
--rw-r--r--   0        0        0    12361 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/src/pg_podcast_toolkit/podcast.py
--rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/src/pg_podcast_toolkit/podcast_ipfs_tools.py
--rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/src/pg_podcast_toolkit/podcast_tools.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/README.md
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0   273506 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/bballrss.xml
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/buildpublish.sh
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/go_ssh_tunnel.sh
+-rw-r--r--   0        0        0   261174 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/look.xml
+-rw-r--r--   0        0        0   350044 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/output.xml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/requirements.txt
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/test_ssh_tunnel.sh
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/__init__.py
+-rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/item.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/media_resource.py
+-rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/podcast.py
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/podcast_ipfs_tools.py
+-rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/podcast_tools.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/PKG-INFO
```

### Comparing `pg_podcast_toolkit-0.0.5/bballrss.xml` & `pg_podcast_toolkit-0.0.6/bballrss.xml`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.5/look.xml` & `pg_podcast_toolkit-0.0.6/look.xml`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.5/output.xml` & `pg_podcast_toolkit-0.0.6/output.xml`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.5/src/pg_podcast_toolkit/item.py` & `pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/item.py`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.5/src/pg_podcast_toolkit/media_resource.py` & `pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/media_resource.py`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.5/src/pg_podcast_toolkit/podcast.py` & `pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/podcast.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
 from bs4 import BeautifulSoup, Tag
 from datetime import datetime, date
 import email.utils
 from time import mktime
 import time
+from .item import Item
+import logging
 
 class InvalidPodcastFeed(ValueError):
     pass
 
 class Podcast():
     """Parses an xml rss feed
 
@@ -198,16 +200,17 @@
                 self.soup = BeautifulSoup(recovered_content, features="lxml-xml")
             except:
                 self.soup = BeautifulSoup(self.feed_content, features="lxml-xml")
 
 
     def add_item(self, tag):
         try:
-            item = item(tag, feed_url=self.feed_url)
+            item = Item(tag, feed_url=self.feed_url)
         except Exception as e:
+            logging.exception("error parsing item")
             return
 
         self.items.append(item)
 
     def set_copyright(self, tag):
         """Parses copyright and set value"""
         try:
```

### Comparing `pg_podcast_toolkit-0.0.5/src/pg_podcast_toolkit/podcast_ipfs_tools.py` & `pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/podcast_ipfs_tools.py`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.5/src/pg_podcast_toolkit/podcast_tools.py` & `pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/podcast_tools.py`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.5/.gitignore` & `pg_podcast_toolkit-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.5/LICENSE` & `pg_podcast_toolkit-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.5/pyproject.toml` & `pg_podcast_toolkit-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pg-podcast-toolkit"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Jason Mazza", email="jason@reallybadapps.com" },
 ]
 description = "Tools for managing podcasting 2.0 feeds"
 keywords = ["podcasting2.0", "ipfs", "rss", "podcast", "parser"]
 readme = "README.md"
 requires-python = ">=3.8"
@@ -20,8 +20,8 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project.urls]
 Homepage = "https://github.com/Really-Bad-Apps/pg-podcast-toolkit"
-Issues = "https://github.com/Really-Bad-Apps/pg-podcast-toolkit/issues"
+Issues = "https://github.com/Really-Bad-Apps/pg-podcast-toolkit/issues"
```

### Comparing `pg_podcast_toolkit-0.0.5/PKG-INFO` & `pg_podcast_toolkit-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pg-podcast-toolkit
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tools for managing podcasting 2.0 feeds
 Project-URL: Homepage, https://github.com/Really-Bad-Apps/pg-podcast-toolkit
 Project-URL: Issues, https://github.com/Really-Bad-Apps/pg-podcast-toolkit/issues
 Author-email: Jason Mazza <jason@reallybadapps.com>
 License: MIT License
 License-File: LICENSE
 Keywords: ipfs,parser,podcast,podcasting2.0,rss
```

