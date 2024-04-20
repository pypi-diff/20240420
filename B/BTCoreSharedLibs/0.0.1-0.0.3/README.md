# Comparing `tmp/BTCoreSharedLibs-0.0.1.tar.gz` & `tmp/btcoresharedlibs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTCoreSharedLibs-0.0.1.tar", last modified: Thu Apr 11 13:12:41 2024, max compression
+gzip compressed data, was "btcoresharedlibs-0.0.3.tar", last modified: Sat Apr 20 17:08:04 2024, max compression
```

## Comparing `BTCoreSharedLibs-0.0.1.tar` & `btcoresharedlibs-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:12:41.536607 BTCoreSharedLibs-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:12:41.536607 BTCoreSharedLibs-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:12:41.536607 BTCoreSharedLibs-0.0.1/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-11 13:12:34.000000 BTCoreSharedLibs-0.0.1/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:12:41.536607 BTCoreSharedLibs-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-11 13:12:34.000000 BTCoreSharedLibs-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-11 13:12:34.000000 BTCoreSharedLibs-0.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 13:12:34.000000 BTCoreSharedLibs-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 13:12:34.000000 BTCoreSharedLibs-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-11 13:12:41.536607 BTCoreSharedLibs-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-11 13:12:34.000000 BTCoreSharedLibs-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-11 13:12:34.000000 BTCoreSharedLibs-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 13:12:34.000000 BTCoreSharedLibs-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-11 13:12:41.536607 BTCoreSharedLibs-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:12:41.536607 BTCoreSharedLibs-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:12:41.536607 BTCoreSharedLibs-0.0.1/src/BTCoreSharedLibs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-11 13:12:41.000000 BTCoreSharedLibs-0.0.1/src/BTCoreSharedLibs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-11 13:12:41.000000 BTCoreSharedLibs-0.0.1/src/BTCoreSharedLibs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:12:41.000000 BTCoreSharedLibs-0.0.1/src/BTCoreSharedLibs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 13:12:41.000000 BTCoreSharedLibs-0.0.1/src/BTCoreSharedLibs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 13:12:41.000000 BTCoreSharedLibs-0.0.1/src/BTCoreSharedLibs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:12:41.536607 BTCoreSharedLibs-0.0.1/src/CoreSharedLibs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:12:34.000000 BTCoreSharedLibs-0.0.1/src/CoreSharedLibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-11 13:12:34.000000 BTCoreSharedLibs-0.0.1/src/CoreSharedLibs/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-11 13:12:34.000000 BTCoreSharedLibs-0.0.1/src/CoreSharedLibs/csl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.313963 btcoresharedlibs-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.309963 btcoresharedlibs-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.309963 btcoresharedlibs-0.0.3/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.309963 btcoresharedlibs-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-20 17:08:04.313963 btcoresharedlibs-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-20 17:08:04.313963 btcoresharedlibs-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.309963 btcoresharedlibs-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.313963 btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-20 17:08:04.000000 btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-20 17:08:04.000000 btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:08:04.000000 btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-20 17:08:04.000000 btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-20 17:08:04.000000 btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.313963 btcoresharedlibs-0.0.3/src/CoreSharedLibs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/src/CoreSharedLibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/src/CoreSharedLibs/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/src/CoreSharedLibs/csl.py
```

### Comparing `BTCoreSharedLibs-0.0.1/.github/scripts/release.py` & `btcoresharedlibs-0.0.3/.github/scripts/release.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 import json
 import subprocess
 
 
 def get_last_version() -> str:
     """Return the version number of the last release."""
     json_string = (
```

### Comparing `BTCoreSharedLibs-0.0.1/.github/workflows/publish.yml` & `btcoresharedlibs-0.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `BTCoreSharedLibs-0.0.1/LICENSE` & `btcoresharedlibs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BTCoreSharedLibs-0.0.1/PKG-INFO` & `btcoresharedlibs-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTCoreSharedLibs
-Version: 0.0.1
+Version: 0.0.3
 Summary: A package of functions that I keep writing over and over again, so I can stop doing that. Script based on seanh example.
 Home-page: https://github.com/Jtecx/Python-BTCoreSharedLibs
 Project-URL: Bug Tracker, https://github.com/Jtecx/Python-BTCoreSharedLibs/issues
 Project-URL: Changelog, https://github.com/Jtecx/Python-BTCoreSharedLibs/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
```

### Comparing `BTCoreSharedLibs-0.0.1/setup.cfg` & `btcoresharedlibs-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `BTCoreSharedLibs-0.0.1/src/BTCoreSharedLibs.egg-info/PKG-INFO` & `btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTCoreSharedLibs
-Version: 0.0.1
+Version: 0.0.3
 Summary: A package of functions that I keep writing over and over again, so I can stop doing that. Script based on seanh example.
 Home-page: https://github.com/Jtecx/Python-BTCoreSharedLibs
 Project-URL: Bug Tracker, https://github.com/Jtecx/Python-BTCoreSharedLibs/issues
 Project-URL: Changelog, https://github.com/Jtecx/Python-BTCoreSharedLibs/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
```

### Comparing `BTCoreSharedLibs-0.0.1/src/CoreSharedLibs/csl.py` & `btcoresharedlibs-0.0.3/src/CoreSharedLibs/csl.py`

 * *Files 22% similar despite different names*

```diff
@@ -102,7 +102,35 @@
 
     if match:
         # Return the matched filename
         return match.group(1)
     else:
         # If no match found, return None
         return None
+
+
+def pos_int_input():
+    verify = True
+    char_val = 0
+    while verify:
+        try:
+            char_val = int(input("Please input an integer. : "))
+            if char_val < 0:
+                raise ValueError("Negative integers are not allowed.")
+            else:
+                char_verify = input(f"{char_val} entered! Correct? Y/N: ").lower()[
+                              :1
+                              ]
+                while True:
+                    if char_verify in ["y", "n"]:
+                        if char_verify == "y":
+                            print("Understood. Moving on.")
+                            verify = False
+                        else:
+                            print("Understood. Trying again.")
+                            verify = True
+                        break
+                    else:
+                        print("Invalid input. Please enter Y or N.")
+        except ValueError:
+            logging.warning("Invalid entry. Integers only,")
+    return char_val
```

