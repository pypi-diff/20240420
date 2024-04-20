# Comparing `tmp/browser-history-0.4.0.tar.gz` & `tmp/browser_history-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browser-history-0.4.0.tar", last modified: Sun Oct  1 13:08:17 2023, max compression
+gzip compressed data, was "browser_history-0.4.1.tar", last modified: Sat Apr 20 10:49:27 2024, max compression
```

## Comparing `browser-history-0.4.0.tar` & `browser_history-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 13:08:17.273157 browser-history-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11345 2023-10-01 13:08:06.000000 browser-history-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2023-10-01 13:08:17.273157 browser-history-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2023-10-01 13:08:06.000000 browser-history-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 13:08:17.269157 browser-history-0.4.0/browser_history/
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2023-10-01 13:08:06.000000 browser-history-0.4.0/browser_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2023-10-01 13:08:06.000000 browser-history-0.4.0/browser_history/browsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2023-10-01 13:08:06.000000 browser-history-0.4.0/browser_history/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    26814 2023-10-01 13:08:06.000000 browser-history-0.4.0/browser_history/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2023-10-01 13:08:06.000000 browser-history-0.4.0/browser_history/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 13:08:17.273157 browser-history-0.4.0/browser_history.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2023-10-01 13:08:17.000000 browser-history-0.4.0/browser_history.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-10-01 13:08:17.000000 browser-history-0.4.0/browser_history.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-01 13:08:17.000000 browser-history-0.4.0/browser_history.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-01 13:08:17.000000 browser-history-0.4.0/browser_history.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-01 13:08:17.000000 browser-history-0.4.0/browser_history.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-01 13:08:17.000000 browser-history-0.4.0/browser_history.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-10-01 13:08:17.273157 browser-history-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-10-01 13:08:06.000000 browser-history-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:49:27.796158 browser_history-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-04-20 10:49:15.000000 browser_history-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-20 10:49:27.796158 browser_history-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-20 10:49:15.000000 browser_history-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:49:27.792158 browser_history-0.4.1/browser_history/
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-20 10:49:15.000000 browser_history-0.4.1/browser_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-04-20 10:49:15.000000 browser_history-0.4.1/browser_history/browsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-20 10:49:15.000000 browser_history-0.4.1/browser_history/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-20 10:49:15.000000 browser_history-0.4.1/browser_history/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-04-20 10:49:15.000000 browser_history-0.4.1/browser_history/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:49:27.796158 browser_history-0.4.1/browser_history.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-20 10:49:27.000000 browser_history-0.4.1/browser_history.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-20 10:49:27.000000 browser_history-0.4.1/browser_history.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 10:49:27.000000 browser_history-0.4.1/browser_history.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-20 10:49:27.000000 browser_history-0.4.1/browser_history.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 10:49:27.000000 browser_history-0.4.1/browser_history.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 10:49:27.000000 browser_history-0.4.1/browser_history.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-20 10:49:27.796158 browser_history-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-20 10:49:15.000000 browser_history-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:49:27.796158 browser_history-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20948 2024-04-20 10:49:15.000000 browser_history-0.4.1/tests/test_browsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18455 2024-04-20 10:49:15.000000 browser_history-0.4.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-20 10:49:15.000000 browser_history-0.4.1/tests/test_default_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-04-20 10:49:15.000000 browser_history-0.4.1/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-20 10:49:15.000000 browser_history-0.4.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-20 10:49:15.000000 browser_history-0.4.1/tests/test_none_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-20 10:49:15.000000 browser_history-0.4.1/tests/test_utils.py
```

### Comparing `browser-history-0.4.0/LICENSE` & `browser_history-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `browser-history-0.4.0/PKG-INFO` & `browser_history-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browser-history
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python module to extract browser history
 Home-page: https://github.com/browser-history/browser-history
 Author: Samyak Sarnayak
 Author-email: samyak201@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://browser-history.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/browser-history/browser-history/
```

### Comparing `browser-history-0.4.0/README.md` & `browser_history-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `browser-history-0.4.0/browser_history/__init__.py` & `browser_history-0.4.1/browser_history/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from . import browsers, generic, utils  # noqa: F401
 
-
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 
 def get_history():
     """This method is used to obtain browser histories of all available and
     supported browsers for the system platform.
 
     :return: Object of class :py:class:`browser_history.generic.Outputs` with
@@ -19,15 +18,17 @@
     for browser_class in browser_classes:
         try:
             browser_object = browser_class()
             browser_output_object = browser_object.fetch_history()
             output_object.histories.extend(browser_output_object.histories)
         except AssertionError:
             utils.logger.info("%s browser is not supported", browser_class.name)
-    output_object.histories.sort()
+    # Can't sort tuples with None values, and some titles
+    # are None, so replace them with ''
+    output_object.histories.sort(key=lambda h: tuple(el or "" for el in h))
     return output_object
 
 
 def get_bookmarks():
     """This method is used to obtain browser bookmarks of all available and
     supported browsers for the system platform.
```

### Comparing `browser-history-0.4.0/browser_history/browsers.py` & `browser_history-0.4.1/browser_history/browsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module defines all supported browsers and their functionality.
 
 All browsers must inherit from :py:mod:`browser_history.generic.Browser`.
 """
+
 import datetime
 import sqlite3
 
 from browser_history.generic import Browser, ChromiumBasedBrowser
 
 
 class Chromium(ChromiumBasedBrowser):
@@ -141,14 +142,15 @@
     Supported platforms:
 
     * Linux
 
 
     Profile support: Yes
     """
+
     name = "LibreWolf"
     aliases = ("librewolfurl",)
 
     linux_path = ".librewolf"
 
 
 class Safari(Browser):
@@ -283,7 +285,26 @@
     aliases = ("vivaldi-stable", "vivaldistable")
 
     linux_path = ".config/vivaldi"
     mac_path = "Library/Application Support/Vivaldi"
     windows_path = "AppData/Local/Vivaldi/User Data"
 
     profile_support = True
+
+
+class Epic(ChromiumBasedBrowser):
+    """Epic Privacy Browser
+
+    Supported platforms (TODO: Add Mac OS support)
+
+    * Windows
+    * Mac OS
+
+    Profile support: No
+    """
+
+    name = "Epic Privacy Browser"
+
+    windows_path = "AppData/Local/Epic Privacy Browser/User Data/Default"
+    mac_path = "Library/Application Support/HiddenReflex/Epic/Default"
+
+    profile_support = False
```

### Comparing `browser-history-0.4.0/browser_history/cli.py` & `browser_history-0.4.1/browser_history/cli.py`

 * *Files identical despite different names*

### Comparing `browser-history-0.4.0/browser_history/generic.py` & `browser_history-0.4.1/browser_history/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module defines the generic base class and the functionality.
 
 All browsers from :py:mod:`browser_history.browsers` inherit this class.
 """
+
 import abc
 import csv
 import datetime
 import json
 import os
 import shutil
 import sqlite3
@@ -277,21 +278,25 @@
                 cursor.execute(self.history_SQL)
                 date_histories = [
                     (
                         datetime.datetime.strptime(d, "%Y-%m-%d %H:%M:%S").replace(
                             tzinfo=self._local_tz
                         ),
                         url,
-                        title
+                        title,
                     )
                     for d, url, title in cursor.fetchall()
                 ]
                 output_object.histories.extend(date_histories)
                 if sort:
-                    output_object.histories.sort(reverse=desc)
+                    # Can't sort tuples with None values, and some titles
+                    # are None, so replace them with ''
+                    output_object.histories.sort(
+                        key=lambda h: tuple(el or "" for el in h), reverse=desc
+                    )
                 conn.close()
         return output_object
 
     def fetch_bookmarks(self, bookmarks_paths=None, sort=True, desc=False):
         """Returns bookmarks of all available profiles stored in SQL or JSON
         or plist.
 
@@ -328,15 +333,16 @@
                 if not os.path.exists(bookmarks_path):
                     continue
                 if os.path.getsize(bookmarks_path.absolute()) == 0:
                     continue
                 copied_bookmark_path = shutil.copy2(
                     bookmarks_path.absolute(), tmpdirname
                 )
-                date_bookmarks = self.bookmarks_parser(copied_bookmark_path)  # pylint: disable=assignment-from-no-return
+                # pylint: disable=assignment-from-no-return
+                date_bookmarks = self.bookmarks_parser(copied_bookmark_path)
                 output_object.bookmarks.extend(date_bookmarks)
             if sort:
                 output_object.bookmarks.sort(reverse=desc)
         return output_object
 
     @classmethod
     def is_supported(cls):
@@ -427,15 +433,19 @@
 
         Examples:
 
         >>> from datetime import datetime
         ... from browser_history import generic
         ... entries = [
         ...     (datetime(2020, 1, 1), 'https://google.com', 'Google'),
-        ...     (datetime(2020, 1, 1), 'https://google.com/imghp?hl=EN', 'Google Images'),
+        ...     (
+        ...         datetime(2020, 1, 1),
+        ...         "https://google.com/imghp?hl=EN",
+        ...         "Google Images",
+        ...     ),
         ...     (datetime(2020, 1, 1), 'https://example.com', 'Example'),
         ... ]
         ... obj = generic.Outputs('history')
         ... obj.histories = entries
         ... obj.sort_domain()
         defaultdict(<class 'list'>, {
             'example.com': [
@@ -537,16 +547,24 @@
         ... entries = [
         ...     [datetime(2020, 1, 1), 'https://google.com', 'Google'],
         ...     [datetime(2020, 1, 1), 'https://example.com', 'Example Domain'],
         ... ]
         ... obj = generic.Outputs()
         ... obj.entries = entries
         ... print(obj.to_json(True))
-        {"Timestamp": "2020-01-01T00:00:00", "URL": "https://google.com", "Google"}
-        {"Timestamp": "2020-01-01T00:00:00", "URL": "https://example.com", "Example Domain"}
+        {
+            "Timestamp": "2020-01-01T00:00:00",
+            "URL": "https://google.com",
+            "Title": "Google",
+        }
+        {
+            "Timestamp": "2020-01-01T00:00:00",
+            "URL": "https://example.com",
+            "Title": "Example Domain",
+        }
         >>> print(obj.to_json())
         {
             "history": [
                 {
                     "Timestamp": "2020-01-01T00:00:00",
                     "URL": "https://google.com",
                     "Title", "Google"
@@ -555,14 +573,15 @@
                     "Timestamp": "2020-01-01T00:00:00",
                     "URL": "https://example.com",
                     "Title": "Example Domain"
                 }
             ]
         }
         """
+
         # custom json encoder for datetime objects
         class DateTimeEncoder(json.JSONEncoder):
             """Custom JSON encoder to encode datetime objects"""
 
             # Override the default method
             def default(self, o):
                 if isinstance(o, (datetime.date, datetime.datetime)):
```

### Comparing `browser-history-0.4.0/browser_history/utils.py` & `browser_history-0.4.1/browser_history/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Module defines Platform class enumerates the popular Operating Systems.
 
 """
+
 import enum
 import inspect
 import logging
 import platform
 import subprocess
 from typing import Optional
```

### Comparing `browser-history-0.4.0/browser_history.egg-info/PKG-INFO` & `browser_history-0.4.1/browser_history.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browser-history
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python module to extract browser history
 Home-page: https://github.com/browser-history/browser-history
 Author: Samyak Sarnayak
 Author-email: samyak201@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://browser-history.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/browser-history/browser-history/
```

### Comparing `browser-history-0.4.0/setup.cfg` & `browser_history-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `browser-history-0.4.0/setup.py` & `browser_history-0.4.1/setup.py`

 * *Files identical despite different names*

