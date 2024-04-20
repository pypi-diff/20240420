# Comparing `tmp/datagouv_python-0.1.3.tar.gz` & `tmp/datagouv_python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagouv_python-0.1.3.tar", max compression
+gzip compressed data, was "datagouv_python-0.1.4.tar", max compression
```

## Comparing `datagouv_python-0.1.3.tar` & `datagouv_python-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2024-04-13 15:20:42.145253 datagouv_python-0.1.3/LICENSE
--rw-r--r--   0        0        0     2500 2024-04-16 19:53:04.995250 datagouv_python-0.1.3/README.md
--rw-r--r--   0        0        0      283 2024-04-15 06:43:06.307169 datagouv_python-0.1.3/datagouv/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 06:37:03.712875 datagouv_python-0.1.3/datagouv/api_client/__init__.py
--rw-r--r--   0        0        0     1373 2024-04-15 19:12:30.887035 datagouv_python-0.1.3/datagouv/api_client/_data_requestor.py
--rw-r--r--   0        0        0      350 2024-04-15 06:37:24.354131 datagouv_python-0.1.3/datagouv/api_client/_datagouv_client.py
--rw-r--r--   0        0        0     1607 2024-04-15 19:08:41.405368 datagouv_python-0.1.3/datagouv/api_client/_datasets_service.py
--rw-r--r--   0        0        0        0 2024-04-15 06:20:34.551164 datagouv_python-0.1.3/datagouv/downloader/__init__.py
--rw-r--r--   0        0        0     1821 2024-04-16 19:50:41.311593 datagouv_python-0.1.3/datagouv/downloader/_resources_downloader.py
--rw-r--r--   0        0        0     2294 2024-04-16 19:48:31.735868 datagouv_python-0.1.3/datagouv/downloader/_resources_downloader__test.py
--rw-r--r--   0        0        0      767 2024-04-15 07:00:51.087557 datagouv_python-0.1.3/datagouv/downloader/_utils.py
--rw-r--r--   0        0        0      131 2024-04-14 15:05:59.938086 datagouv_python-0.1.3/datagouv/main.py
--rw-r--r--   0        0        0      720 2024-04-16 19:53:11.529313 datagouv_python-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3440 1970-01-01 00:00:00.000000 datagouv_python-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-13 15:20:42.145253 datagouv_python-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2500 2024-04-16 19:53:04.995250 datagouv_python-0.1.4/README.md
+-rw-r--r--   0        0        0      283 2024-04-15 06:43:06.307169 datagouv_python-0.1.4/datagouv/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 06:37:03.712875 datagouv_python-0.1.4/datagouv/api_client/__init__.py
+-rw-r--r--   0        0        0     1373 2024-04-15 19:12:30.887035 datagouv_python-0.1.4/datagouv/api_client/_data_requestor.py
+-rw-r--r--   0        0        0      350 2024-04-15 06:37:24.354131 datagouv_python-0.1.4/datagouv/api_client/_datagouv_client.py
+-rw-r--r--   0        0        0     1607 2024-04-15 19:08:41.405368 datagouv_python-0.1.4/datagouv/api_client/_datasets_service.py
+-rw-r--r--   0        0        0        0 2024-04-15 06:20:34.551164 datagouv_python-0.1.4/datagouv/downloader/__init__.py
+-rw-r--r--   0        0        0     1879 2024-04-20 12:16:10.752147 datagouv_python-0.1.4/datagouv/downloader/_resources_downloader.py
+-rw-r--r--   0        0        0     2800 2024-04-20 12:22:07.394400 datagouv_python-0.1.4/datagouv/downloader/_resources_downloader__test.py
+-rw-r--r--   0        0        0      767 2024-04-15 07:00:51.087557 datagouv_python-0.1.4/datagouv/downloader/_utils.py
+-rw-r--r--   0        0        0      131 2024-04-14 15:05:59.938086 datagouv_python-0.1.4/datagouv/main.py
+-rw-r--r--   0        0        0      720 2024-04-20 12:37:21.147503 datagouv_python-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3440 1970-01-01 00:00:00.000000 datagouv_python-0.1.4/PKG-INFO
```

### Comparing `datagouv_python-0.1.3/LICENSE` & `datagouv_python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.1.3/README.md` & `datagouv_python-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.1.3/datagouv/api_client/_data_requestor.py` & `datagouv_python-0.1.4/datagouv/api_client/_data_requestor.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.1.3/datagouv/api_client/_datasets_service.py` & `datagouv_python-0.1.4/datagouv/api_client/_datasets_service.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.1.3/datagouv/downloader/_resources_downloader.py` & `datagouv_python-0.1.4/datagouv/downloader/_resources_downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class ResourcesDownloader(object):
     def __init__(
         self,
         dataset_id: str,
         resource_types: str | list[str] = "all",
-        url_regex: str = None,
+        title_regex: str = None,
         DatagouvClient=DatagouvClient,
     ) -> None:
         """
         resource_types: ["main", "documentation", "update", "api", "code", "other"]
         """
         self.dataset_id: str = dataset_id
 
@@ -25,15 +25,15 @@
         self.urls: list = []
 
         if resource_types == "all":
             self.resource_types: list = RESOURCE_TYPES
         elif isinstance(resource_types, list):
             self.resource_types = resource_types
 
-        self.url_regex = url_regex
+        self.title_regex = title_regex
 
         self.client = DatagouvClient()
 
         self.prepare()
 
     def prepare(self) -> None:
         """
@@ -42,18 +42,19 @@
         self.dataset = self.client.datasets.get(self.dataset_id)
         self.resources = self.dataset.get("resources")
         self.urls = []
 
         for resource in self.resources:
             # Add url if type is allowed
             type = resource.get("type")
-            url = resource.get("url")
+            title = resource.get("title")
             if type in self.resource_types and (
-                self.url_regex is None or re.search(self.url_regex, url) is not None
+                self.title_regex is None or re.search(self.title_regex, title) is not None
             ):
+                url = resource.get("url")
                 self.urls.append(url)
 
         return None
 
     def download(self, directory_path: str = None) -> list:
         """
         Download resources into `directory_path`
```

### Comparing `datagouv_python-0.1.3/datagouv/downloader/_resources_downloader__test.py` & `datagouv_python-0.1.4/datagouv/downloader/_resources_downloader__test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 import pytest
 
 from datagouv import ResourcesDownloader
 from datagouv.downloader._resources_downloader import RESOURCE_TYPES
 
-resource_1 = {"id": "r_1_id", "url": "r_1_url", "type": "main"}
-resource_2 = {"id": "r_2_id", "url": "r_2_url_2024", "type": "main"}
-resource_3 = {"id": "r_3_id", "url": "r_3_url_2024", "type": "documentation"}
-resource_4 = {"id": "r_4_id", "url": "r_4_url", "type": "other"}
+resource_1 = {"id": "r_1_id", "url": "r_1_url", "title": "1 Url", "type": "main"}
+resource_2 = {
+    "id": "r_2_id",
+    "url": "r_2_url_2024",
+    "title": "2 url_2024",
+    "type": "main",
+}
+resource_3 = {
+    "id": "r_3_id",
+    "url": "r_3_url_2024",
+    "title": "3 url_2024",
+    "type": "documentation",
+}
+resource_4 = {"id": "r_4_id", "url": "r_4_url", "title": "4 Url", "type": "other"}
 
 dataset_1_id = "id_d_1"
 dataset_1 = {
     "id": "dataset_1_id",
     "resources": [resource_1, resource_2, resource_3, resource_4],
 }
 
@@ -69,16 +79,31 @@
     )
     # Test files types
     assert d.resource_types == ["main", "documentation"]
     assert len(d.resources) == 4
     assert len(d.urls) == 3
 
 
-def test_regex_urls():
+def test_regex_titles():
+    title_regex = "_2024"
+    types = ["main"]
+    d = ResourcesDownloader(
+        dataset_1_id, types, title_regex, DatagouvClient=MockDatagouvClient
+    )
+    # Test files types
+    assert len(d.resources) == 4
+
+    # Only one url is type=main and contains '_2024'
+    assert len(d.urls) == 1
+
+
+def test_advanced_regex_titles():
+    title_regex = "_[0-9]{4}"
+    types = ["main"]
     d = ResourcesDownloader(
-        dataset_1_id, ["main"], "_2024", DatagouvClient=MockDatagouvClient
+        dataset_1_id, types, title_regex, DatagouvClient=MockDatagouvClient
     )
     # Test files types
     assert len(d.resources) == 4
 
     # Only one url is type=main and contains '_2024'
     assert len(d.urls) == 1
```

### Comparing `datagouv_python-0.1.3/datagouv/downloader/_utils.py` & `datagouv_python-0.1.4/datagouv/downloader/_utils.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.1.3/pyproject.toml` & `datagouv_python-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datagouv-python"
-version = "0.1.3"
+version = "0.1.4"
 description = "Unofficial python client for `data.gouv.fr`"
 authors = ["Maxime Pawlak <maxime.pawlak@amatek.fr>"]
 repository = "https://github.com/MaximePawlakFr/datagouv-python"
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "datagouv"}]
 keywords = ["open-data", "opendata", "government"]
```

### Comparing `datagouv_python-0.1.3/PKG-INFO` & `datagouv_python-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagouv-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: Unofficial python client for `data.gouv.fr`
 Home-page: https://github.com/MaximePawlakFr/datagouv-python
 License: GPL-3.0-or-later
 Keywords: open-data,opendata,government
 Author: Maxime Pawlak
 Author-email: maxime.pawlak@amatek.fr
 Requires-Python: >=3.9,<4.0
```

