# Comparing `tmp/npc-sync-0.1.8.tar.gz` & `tmp/npc-sync-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npc-sync-0.1.8.tar", last modified: Wed Mar 20 18:00:42 2024, max compression
+gzip compressed data, was "npc-sync-0.1.9.tar", last modified: Wed Mar 20 18:20:15 2024, max compression
```

## Comparing `npc-sync-0.1.8.tar` & `npc-sync-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:00:42.636779 npc-sync-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-20 18:00:14.000000 npc-sync-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-20 18:00:42.636779 npc-sync-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-20 18:00:14.000000 npc-sync-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-20 18:00:40.000000 npc-sync-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 18:00:42.636779 npc-sync-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:00:42.636779 npc-sync-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:00:42.636779 npc-sync-0.1.8/src/npc_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-20 18:00:14.000000 npc-sync-0.1.8/src/npc_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:00:14.000000 npc-sync-0.1.8/src/npc_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    62409 2024-03-20 18:00:37.000000 npc-sync-0.1.8/src/npc_sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:00:42.636779 npc-sync-0.1.8/src/npc_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-20 18:00:42.000000 npc-sync-0.1.8/src/npc_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-20 18:00:42.000000 npc-sync-0.1.8/src/npc_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 18:00:42.000000 npc-sync-0.1.8/src/npc_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-20 18:00:42.000000 npc-sync-0.1.8/src/npc_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 18:00:42.000000 npc-sync-0.1.8/src/npc_sync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:00:42.636779 npc-sync-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-20 18:00:14.000000 npc-sync-0.1.8/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-20 18:00:14.000000 npc-sync-0.1.8/tests/test_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:20:15.579693 npc-sync-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-20 18:19:49.000000 npc-sync-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-20 18:20:15.579693 npc-sync-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-20 18:19:49.000000 npc-sync-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-20 18:20:13.000000 npc-sync-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 18:20:15.579693 npc-sync-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:20:15.579693 npc-sync-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:20:15.579693 npc-sync-0.1.9/src/npc_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-20 18:19:49.000000 npc-sync-0.1.9/src/npc_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:19:49.000000 npc-sync-0.1.9/src/npc_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    62411 2024-03-20 18:20:09.000000 npc-sync-0.1.9/src/npc_sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:20:15.579693 npc-sync-0.1.9/src/npc_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-20 18:20:15.000000 npc-sync-0.1.9/src/npc_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-20 18:20:15.000000 npc-sync-0.1.9/src/npc_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 18:20:15.000000 npc-sync-0.1.9/src/npc_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-20 18:20:15.000000 npc-sync-0.1.9/src/npc_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 18:20:15.000000 npc-sync-0.1.9/src/npc_sync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:20:15.579693 npc-sync-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-20 18:19:49.000000 npc-sync-0.1.9/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-20 18:19:49.000000 npc-sync-0.1.9/tests/test_plots.py
```

### Comparing `npc-sync-0.1.8/LICENSE` & `npc-sync-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `npc-sync-0.1.8/PKG-INFO` & `npc-sync-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc-sync
-Version: 0.1.8
+Version: 0.1.9
 Summary: Repackaging of AllenSDK.SyncDataset with extra functionality, compatible with data in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_sync
 Project-URL: Issues, https://github.com/AllenInstitute/npc_sync/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `npc-sync-0.1.8/README.md` & `npc-sync-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `npc-sync-0.1.8/pyproject.toml` & `npc-sync-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "h5py>=3.10.0",
     "numpy>=1.26.3",
     "matplotlib>=3.8.2",
     "typing-extensions>=4.9.0",
     "npc-io>=0.1.26",
     "npc-session>=0.1.33",
 ]
-version = "0.1.8"
+version = "0.1.9"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `npc-sync-0.1.8/src/npc_sync/__init__.py` & `npc-sync-0.1.9/src/npc_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `npc-sync-0.1.8/src/npc_sync/sync.py` & `npc-sync-0.1.9/src/npc_sync/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 Allen Institute for Brain Science
 """
 
 from __future__ import annotations
 
 import datetime
+import io
 import logging
 from collections.abc import Iterable, Sequence
 from typing import TYPE_CHECKING, Any, Literal, Union
 
 import h5py
 import npc_io
 import npc_session
@@ -264,20 +265,20 @@
         if isinstance(path, h5py.File):
             self.dfile = path
         else:
             try:
                 self.dfile = h5py.File(path, "r")
             except OSError:
                 path = npc_io.from_pathlike(path)
-                ffspec_storage_options = {}
-                if path.protocol not in ("", "file"):
-                    ffspec_storage_options["cache_type"] = "first"
-                self.dfile = h5py.File(
-                    path.open(mode="rb", **ffspec_storage_options), "r"
-                )
+                if path.protocol in ("", "file"):
+                    self.dfile = h5py.File(io.BytesIO(path.read_bytes()), "r")
+                else:
+                    self.dfile = h5py.File(
+                        path.open(mode="rb", cache_type="first"), "r"
+                    )
         return self.dfile
 
     @property
     def meta_data(self) -> dict[str, Any]:
         return eval(self.dfile["meta"][()])
 
     @property
```

### Comparing `npc-sync-0.1.8/src/npc_sync.egg-info/PKG-INFO` & `npc-sync-0.1.9/src/npc_sync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc-sync
-Version: 0.1.8
+Version: 0.1.9
 Summary: Repackaging of AllenSDK.SyncDataset with extra functionality, compatible with data in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_sync
 Project-URL: Issues, https://github.com/AllenInstitute/npc_sync/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

