# Comparing `tmp/slicer_package_manager-0.8.0.tar.gz` & `tmp/slicer_package_manager-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slicer_package_manager-0.8.0.tar", last modified: Thu May 11 02:54:22 2023, max compression
+gzip compressed data, was "slicer_package_manager-0.9.0.tar", last modified: Sat Apr 20 04:49:25 2024, max compression
```

## Comparing `slicer_package_manager-0.8.0.tar` & `slicer_package_manager-0.9.0.tar`

### file list

```diff
@@ -1,58 +1,33 @@
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      148 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/AUTHORS.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      600 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/LICENSE
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      226 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/MANIFEST.in
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1982 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/PKG-INFO
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1109 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/README.rst
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.030357 slicer_package_manager-0.8.0/docs/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1130 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/Makefile
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       28 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/authors.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       28 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/changes.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    13624 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/commands_shell.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4774 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/concepts.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5473 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/conf.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.030357 slicer_package_manager-0.8.0/docs/developer_guide/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5732 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/develop.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      172 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/index.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2138 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/install.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      430 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/overview.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      378 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/slicer_package_manager.api.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      618 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/slicer_package_manager.models.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      636 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/slicer_package_manager.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      455 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/slicer_package_manager_client.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4756 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/faq.rst
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.030357 slicer_package_manager-0.8.0/docs/images/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)  1515244 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/images/slicer_package_manager_models.JPG
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      969 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/index.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1664 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/installation.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5300 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/make_a_release.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3359 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/overview.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2933 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/pyproject.toml
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      238 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/setup.cfg
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1480 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/slicer_package_manager/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     7267 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      497 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/slicer_package_manager/_version.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/slicer_package_manager/api/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/api/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    44559 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/api/app.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      302 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/constants.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/slicer_package_manager/models/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/models/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4975 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/models/extension.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3652 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/models/package.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     7461 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/utilities.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1982 2023-05-11 02:54:22.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/PKG-INFO
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1428 2023-05-11 02:54:22.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2023-05-11 02:54:22.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       77 2023-05-11 02:54:22.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/entry_points.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2023-05-11 02:54:21.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/not-zip-safe
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       49 2023-05-11 02:54:22.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/requires.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       29 2023-05-11 02:54:22.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/top_level.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/tests/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    14270 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/tests/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      396 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/tests/conftest.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      259 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/tests/test_load.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    47108 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/tests/test_slicer_package_manager.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    68603 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/versioneer.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2024-04-20 04:49:25.552881 slicer_package_manager-0.9.0/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      148 2022-04-18 17:25:05.000000 slicer_package_manager-0.9.0/AUTHORS.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      600 2022-04-18 17:25:05.000000 slicer_package_manager-0.9.0/LICENSE
+-rw-r--r--   0 jcfr      (1000) jcfr      (1000)     2341 2024-04-20 04:49:25.552881 slicer_package_manager-0.9.0/PKG-INFO
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1109 2022-05-20 21:48:20.000000 slicer_package_manager-0.9.0/README.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4980 2024-04-20 04:46:33.000000 slicer_package_manager-0.9.0/pyproject.toml
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       38 2024-04-20 04:49:25.552881 slicer_package_manager-0.9.0/setup.cfg
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      264 2024-04-18 06:44:19.000000 slicer_package_manager-0.9.0/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2024-04-20 04:49:25.548881 slicer_package_manager-0.9.0/slicer_package_manager/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     7000 2024-04-18 04:51:03.000000 slicer_package_manager-0.9.0/slicer_package_manager/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      497 2024-04-20 04:49:25.552881 slicer_package_manager-0.9.0/slicer_package_manager/_version.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2024-04-20 04:49:25.552881 slicer_package_manager-0.9.0/slicer_package_manager/api/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2022-05-20 20:46:19.000000 slicer_package_manager-0.9.0/slicer_package_manager/api/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    44683 2024-04-20 04:46:33.000000 slicer_package_manager-0.9.0/slicer_package_manager/api/app.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      302 2023-05-04 09:22:10.000000 slicer_package_manager-0.9.0/slicer_package_manager/constants.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2024-04-20 04:49:25.552881 slicer_package_manager-0.9.0/slicer_package_manager/models/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2022-05-20 20:46:19.000000 slicer_package_manager-0.9.0/slicer_package_manager/models/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4975 2024-04-18 04:51:03.000000 slicer_package_manager-0.9.0/slicer_package_manager/models/extension.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3652 2024-04-18 04:51:03.000000 slicer_package_manager-0.9.0/slicer_package_manager/models/package.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     7461 2024-04-18 04:51:03.000000 slicer_package_manager-0.9.0/slicer_package_manager/utilities.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2024-04-20 04:49:25.552881 slicer_package_manager-0.9.0/slicer_package_manager.egg-info/
+-rw-r--r--   0 jcfr      (1000) jcfr      (1000)     2341 2024-04-20 04:49:25.000000 slicer_package_manager-0.9.0/slicer_package_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      810 2024-04-20 04:49:25.000000 slicer_package_manager-0.9.0/slicer_package_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2024-04-20 04:49:25.000000 slicer_package_manager-0.9.0/slicer_package_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       77 2024-04-20 04:49:25.000000 slicer_package_manager-0.9.0/slicer_package_manager.egg-info/entry_points.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2024-04-18 06:57:58.000000 slicer_package_manager-0.9.0/slicer_package_manager.egg-info/not-zip-safe
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      153 2024-04-20 04:49:25.000000 slicer_package_manager-0.9.0/slicer_package_manager.egg-info/requires.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       29 2024-04-20 04:49:25.000000 slicer_package_manager-0.9.0/slicer_package_manager.egg-info/top_level.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2024-04-20 04:49:25.552881 slicer_package_manager-0.9.0/tests/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    14270 2024-04-18 04:51:03.000000 slicer_package_manager-0.9.0/tests/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      396 2023-05-05 00:56:18.000000 slicer_package_manager-0.9.0/tests/conftest.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      259 2024-04-18 04:51:03.000000 slicer_package_manager-0.9.0/tests/test_load.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    47862 2024-04-20 04:46:33.000000 slicer_package_manager-0.9.0/tests/test_slicer_package_manager.py
```

### Comparing `slicer_package_manager-0.8.0/LICENSE` & `slicer_package_manager-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.8.0/README.rst` & `slicer_package_manager-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.8.0/slicer_package_manager/__init__.py` & `slicer_package_manager-0.9.0/slicer_package_manager/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from girder import events, plugin
 from girder.constants import AccessType
 from girder.models.file import File
 from girder.models.item import Item
 from girder.models.folder import Folder
 from .api.app import App
 from . import constants, utilities
-from .models.extension import Extension as ExtensionModel
 from .models.package import Package as PackageModel
 
 from girder_hashsum_download import SUPPORTED_ALGORITHMS
 
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
@@ -105,17 +104,14 @@
 
     item = Item().load(file['itemId'], force=True)
 
     # Both application and extension packages are expected to have these metadata
     if not all(meta in item.get('meta', {}) for meta in ['app_id', 'os', 'arch', 'revision']):
         return
 
-    # ... but only extension packages have "app_revision"
-    is_extension_package = 'app_revision' in item
-
     if event.name == "model.file.save.after":
         if Item().childFiles(item).count() > 1:
             # If the update is not related to the first file, ignore
             return
 
         # Collect checksums associated if the file
         checksums = {algo: file[algo] for algo in SUPPORTED_ALGORITHMS if algo in file}
@@ -138,18 +134,15 @@
             # If after removing this file, there are no file left, set the checksum to empty string.
             # Collect checksums associated if the remaining file
             checksums = {algo: "" for algo in SUPPORTED_ALGORITHMS}
 
     # Update metadata overwriting existing checksum values if any
     meta = {**item['meta'], **checksums}
 
-    if is_extension_package:
-        ExtensionModel().setMetadata(item, meta)
-    else:
-        PackageModel().setMetadata(item, meta)
+    Item().setMetadata(item, meta)
 
 
 def _onReleaseFolderNameUpdated(event):
     """
     Update "release" metadata on all application package items in a release folder when its name is changed.
 
     See :func:`utilities.isReleaseFolder()`.
```

### Comparing `slicer_package_manager-0.8.0/slicer_package_manager/api/app.py` & `slicer_package_manager-0.9.0/slicer_package_manager/api/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 create new applications, new releases, and upload or download application and extensions
 packages.
 """
 import datetime
 import re
 
 from bson.objectid import ObjectId
+from html_sanitizer import Sanitizer
 
 from girder.api import access
 from girder.constants import TokenScope, AccessType, SortDir
 from girder.api.describe import Description, autoDescribeRoute
 from girder.api.rest import Resource
 from girder.exceptions import RestException
 from girder.models.folder import Folder
@@ -620,14 +621,17 @@
                 parentType='Folder',
                 public=release_folder['public'],
                 description='This directory contains all the extensions packages',
                 creator=creator)
         else:
             extensions_folder = extensions_folder[0]
 
+        sanitizer = Sanitizer()
+        description = sanitizer.sanitize(description)
+
         params = {
             'app_id': app_id,
             'baseName': baseName,
             'os': os,
             'arch': arch,
             'repository_type': repository_type,
             'repository_url': repository_url,
```

### Comparing `slicer_package_manager-0.8.0/slicer_package_manager/models/extension.py` & `slicer_package_manager-0.9.0/slicer_package_manager/models/extension.py`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.8.0/slicer_package_manager/models/package.py` & `slicer_package_manager-0.9.0/slicer_package_manager/models/package.py`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.8.0/slicer_package_manager/utilities.py` & `slicer_package_manager-0.9.0/slicer_package_manager/utilities.py`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.8.0/tests/__init__.py` & `slicer_package_manager-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.8.0/tests/test_slicer_package_manager.py` & `slicer_package_manager-0.9.0/tests/test_slicer_package_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -527,22 +527,30 @@
 @pytest.mark.plugin('slicer_package_manager')
 def testUpdateExtensions(server, user, app_folder, extensions):
     # Update the same extension
     newParams = EXTENSIONS[1]['meta'].copy()
     newParams.update({
         'revision': '0000',
         'repository_type': 'gitlab',
-        'description': 'Extension for Slicer 4 new version 2',
+        'description': (
+            'Extension for Slicer 4 new version 2<br>'
+            'with a new line and no script tag here:<script>alert(\'test\');</script>'
+        ),
     })
     updatedExtension = _createOrUpdatePackage(server, 'extension', newParams, _user=user, _app=app_folder)
     # Check the same extension has different metadata
     assert updatedExtension['_id'] == extensions[1]['_id']
     assert updatedExtension['name'] == constants.EXTENSION_PACKAGE_TEMPLATE_NAME.format(**newParams)
     assert updatedExtension['meta'] != extensions[1]['meta']
 
+    updatedExtensionMetadata = updatedExtension['meta']
+    assert updatedExtensionMetadata['description'] == (
+        'Extension for Slicer 4 new version 2<br>with a new line and no script tag here:'
+    )
+
 
 @pytest.mark.plugin('slicer_package_manager')
 def testGetExtensions(server, user, app_folder, release_folder, extensions):
     # Get all the extension of the application
     resp = server.request(
         path='/app/%s/extension' % app_folder['_id'],
         method='GET',
@@ -1006,34 +1014,42 @@
     for key in ['app_id', 'arch', 'baseName', 'os', 'revision']:
         assert item_after['meta'][key] == item['meta'][key]
 
     assert ObjectId(item_after['folderId']) == dest_folder['_id']
     assert item_after['meta'].get('release', None) == release_after
 
 
+@pytest.mark.parametrize("items", [
+    pytest.lazy_fixture('packages'),
+    pytest.lazy_fixture('extensions'),
+])
 @pytest.mark.plugin('slicer_package_manager')
-def testApplicationPackageMetadataChecksumUpdate_1(server, user, packages):
+def testPackageMetadataChecksumUpdate_1(server, user, items):
     """Replace existing file and verify checksum is updated."""
-    item = Item().load(packages[0]['_id'], force=True)
+    item = Item().load(items[0]['_id'], force=True)
     file = list(Item().childFiles(item))[0]
 
     # Replace file
     updated_contents = "you've changed!"
     _replaceFile(server, file["_id"], updated_contents, user)
 
     # Confirm item checksum was updated
     item_after = Item().load(item['_id'], force=True)
     expected_checksum = computeContentChecksum("SHA512", updated_contents.encode("utf8"))
     assert item_after["meta"]["sha512"] == expected_checksum
 
 
+@pytest.mark.parametrize("items", [
+    pytest.lazy_fixture('packages'),
+    pytest.lazy_fixture('extensions'),
+])
 @pytest.mark.plugin('slicer_package_manager')
-def testApplicationPackageMetadataChecksumUpdate_2(server, user, packages, tmpdir):
+def testPackageMetadataChecksumUpdate_2(server, user, items, tmpdir):
     """Upload an additional file and verify checksum remains the same."""
-    item = Item().load(packages[1]['_id'], force=True)
+    item = Item().load(items[1]['_id'], force=True)
     assert Item().childFiles(item).count() == 1
     item_first_file_sha512 = item["meta"]["sha512"]
 
     # Upload additional file
     filePath = tmpdir / "additional.tar.gz"
     with open(filePath, "w") as content:
         content.write("new file contents")
@@ -1046,20 +1062,24 @@
     item_after = Item().load(item['_id'], force=True)
     assert Item().childFiles(item_after).count() == 2
 
     # Confirm item checksum is unchanged
     assert item_first_file_sha512 == item_after["meta"]["sha512"]
 
 
+@pytest.mark.parametrize("items", [
+    pytest.lazy_fixture('packages'),
+    pytest.lazy_fixture('extensions'),
+])
 @pytest.mark.plugin('slicer_package_manager')
-def testApplicationPackageMetadataChecksumUpdate_3(server, user, packages, tmpdir):
+def testPackageMetadataChecksumUpdate_3(server, user, items, tmpdir):
     """Upload an additional file, remove the first one and verify the checksum matches
     the one of the additional file.
     """
-    item = Item().load(packages[2]['_id'], force=True)
+    item = Item().load(items[2]['_id'], force=True)
     assert Item().childFiles(item).count() == 1
     item_first_file_sha512 = item["meta"]["sha512"]
     item_first_file_id = list(Item().childFiles(item))[0]["_id"]
 
     # Upload additional file
     filePath = tmpdir / "additional.tar.gz"
     with open(filePath, "w") as content:
@@ -1084,18 +1104,22 @@
     assert Item().childFiles(item_after).count() == 1
 
     # Confirm the item checksum was updated
     assert item_after["meta"]["sha512"] != item_first_file_sha512
     assert item_after["meta"]["sha512"] == additional_file_sha512
 
 
+@pytest.mark.parametrize("items", [
+    pytest.lazy_fixture('packages'),
+    pytest.lazy_fixture('extensions'),
+])
 @pytest.mark.plugin('slicer_package_manager')
-def testApplicationPackageMetadataChecksumUpdate_4(server, user, packages):
+def testPackageMetadataChecksumUpdate_4(server, user, items):
     """Delete the last file and verify the checksum is set to an empty string."""
-    item = Item().load(packages[0]['_id'], force=True)
+    item = Item().load(items[0]['_id'], force=True)
     assert Item().childFiles(item).count() == 1
     item_file_id = list(Item().childFiles(item))[0]["_id"]
 
     # Remove the file
     resp = server.request(
         path='/file/%s' % item_file_id,
         method='DELETE',
@@ -1355,18 +1379,19 @@
     if status_code != 200:
         return None
 
     def _filtered(metadata):
         return {k: v for (k, v) in metadata.items() if k not in (
             'app_id',
             'build_date',
+            'description',
             'sha512',
         )}
 
-    # assert every other fields (besides unique or computed ones) are identical
+    # assert every other fields (besides unique, computed or sanitized ones) are identical
     assert _filtered(resp.json['meta']) == _filtered(params)
 
     if filePath:
         # Upload a package file
         item = resp.json
         with open(filePath, 'rb') as content:
             uploadedFile = server.uploadFile(
```

