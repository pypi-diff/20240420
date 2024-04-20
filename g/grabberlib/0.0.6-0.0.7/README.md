# Comparing `tmp/grabberlib-0.0.6.tar.gz` & `tmp/grabberlib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.0.6.tar", max compression
+gzip compressed data, was "grabberlib-0.0.7.tar", max compression
```

## Comparing `grabberlib-0.0.6.tar` & `grabberlib-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2024-04-19 16:44:36.061439 grabberlib-0.0.6/README.md
--rw-r--r--   0        0        0        1 2024-04-19 21:08:54.051660 grabberlib-0.0.6/assets/pages.txt
--rw-r--r--   0        0        0        0 2024-04-19 16:44:36.031593 grabberlib-0.0.6/grabber/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-19 16:44:36.314458 grabberlib-0.0.6/grabber/__main__.py
--rw-r--r--   0        0        0        0 2024-04-19 16:44:36.314537 grabberlib-0.0.6/grabber/controllers/__init__.py
--rw-r--r--   0        0        0     3798 2024-04-19 21:11:49.668721 grabberlib-0.0.6/grabber/controllers/base.py
--rw-r--r--   0        0        0        0 2024-04-19 16:44:36.315102 grabberlib-0.0.6/grabber/core/__init__.py
--rw-r--r--   0        0        0       65 2024-04-19 16:44:36.315699 grabberlib-0.0.6/grabber/core/exc.py
--rw-r--r--   0        0        0      188 2024-04-19 16:50:32.400947 grabberlib-0.0.6/grabber/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-19 16:44:36.316024 grabberlib-0.0.6/grabber/core/sources/__init__.py
--rw-r--r--   0        0        0     3378 2024-04-19 17:11:11.625028 grabberlib-0.0.6/grabber/core/sources/graph.py
--rw-r--r--   0        0        0     3986 2024-04-19 17:48:30.254982 grabberlib-0.0.6/grabber/core/sources/khd.py
--rw-r--r--   0        0        0     3588 2024-04-19 17:11:18.798709 grabberlib-0.0.6/grabber/core/sources/xasiat.py
--rw-r--r--   0        0        0     3718 2024-04-19 21:24:29.005339 grabberlib-0.0.6/grabber/core/sources/xiuren.py
--rw-r--r--   0        0        0        1 2024-04-19 16:44:36.392872 grabberlib-0.0.6/grabber/core/sources/yellow.py
--rw-r--r--   0        0        0    13070 2024-04-19 21:25:00.367081 grabberlib-0.0.6/grabber/core/utils.py
--rw-r--r--   0        0        0      175 2024-04-19 21:25:25.122215 grabberlib-0.0.6/grabber/core/version.py
--rw-r--r--   0        0        0        0 2024-04-19 16:44:36.318014 grabberlib-0.0.6/grabber/templates/__init__.py
--rw-r--r--   0        0        0     1017 2024-04-19 21:25:18.090165 grabberlib-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.755675 grabberlib-0.0.7/README.md
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.755675 grabberlib-0.0.7/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     3798 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/core/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/core/exc.py
+-rw-r--r--   0        0        0      446 2024-04-20 15:06:51.092892 grabberlib-0.0.7/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0     3400 2024-04-20 15:08:46.386081 grabberlib-0.0.7/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     4008 2024-04-20 15:09:05.377639 grabberlib-0.0.7/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     3610 2024-04-20 15:09:24.729188 grabberlib-0.0.7/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     3740 2024-04-20 15:09:41.284801 grabberlib-0.0.7/grabber/core/sources/xiuren.py
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0    13127 2024-04-20 15:12:16.745134 grabberlib-0.0.7/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-04-20 15:10:47.699240 grabberlib-0.0.7/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.7/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1017 2024-04-20 15:10:40.347413 grabberlib-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.7/PKG-INFO
```

### Comparing `grabberlib-0.0.6/grabber/__main__.py` & `grabberlib-0.0.7/grabber/__main__.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.6/grabber/controllers/base.py` & `grabberlib-0.0.7/grabber/controllers/base.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.6/grabber/core/sources/graph.py` & `grabberlib-0.0.7/grabber/core/sources/xasiat.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 import pathlib
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from typing import List
 
 from tqdm import tqdm
 
-from grabber.core.settings import MEDIA_ROOT
+from grabber.core.settings import get_media_root
 from grabber.core.utils import (
     query_mapping,
     headers_mapping,
     get_tags,
     download_images,
     upload_to_telegraph,
 )
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 
 
-def get_for_telegraph(
+def get_for_xasiat(
     sources: List[str],
     entity: str,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
     **kwargs,
 ) -> None:
     titles = set()
@@ -33,54 +33,60 @@
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
     folders = set()
     titles_and_folders = set()
     title_folder_mapping = {}
 
     if final_dest:
-        final_dest_folder = MEDIA_ROOT / final_dest
+        final_dest_folder = get_media_root() / final_dest
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         folder_name = ""
+        tqdm_sources_iterable.set_description(f"Retrieving URLs from {source_url}")
         tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
 
         title_tag = soup.select("title")[0]  # type: ignore
         folder_name = title_tag.get_text().strip().rstrip()
         title = folder_name
         titles.add(title)
         titles_and_folders.add((title, folder_name))
 
         if final_dest:
-            new_folder = MEDIA_ROOT / final_dest / folder_name
+            new_folder = get_media_root() / final_dest / folder_name
         else:
-            new_folder = MEDIA_ROOT / folder_name
+            new_folder = get_media_root() / folder_name
 
         if not new_folder.exists():
             new_folder.mkdir(parents=True, exist_ok=True)
 
         folders.add(new_folder)
         unique_img_urls = set()
 
         for idx, img_tag in enumerate(tags or []):
             img_src = img_tag.attrs[src_attr]
-            img_name: str = img_src.split("/")[-1]
-            img_name = img_name.strip().rstrip()
-            if "images.hotgirl.asia" not in img_src:
-                unique_img_urls.add(
-                    (f"{idx + 1}-{img_name}", f"https://telegra.ph{img_src}")
-                )
+
+            if "xasiat" in img_src:
+                img_name: str = img_src.split("/")[-2]
+                img_name = img_name.strip().rstrip()
+                img_extension: str = img_name.split(".")[-1]
             else:
-                unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
+                img_name: str = img_src.split("/")[-1]
+                img_name = img_name.strip().rstrip()
+                img_extension: str = img_name.split(".")[-1]
+
+            unique_img_urls.add(
+                (title, f"{idx + 1}.{img_extension}", img_src),
+            )
 
         title_folder_mapping[title] = (unique_img_urls, new_folder)
 
     futures = []
     with ThreadPoolExecutor(max_workers=DEFAULT_THREADS_NUMBER) as executor:
         for title, (images_set, folder_dest) in title_folder_mapping.items():
             partial_download = partial(
```

### Comparing `grabberlib-0.0.6/grabber/core/sources/khd.py` & `grabberlib-0.0.7/grabber/core/sources/khd.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from functools import partial
 from typing import List, Optional
 
 from tqdm import tqdm
 
-from grabber.core.settings import MEDIA_ROOT
+from grabber.core.settings import get_media_root
 from grabber.core.utils import (
     query_mapping,
     headers_mapping,
     get_tags,
     download_images,
     upload_to_telegraph,
 )
@@ -40,15 +40,15 @@
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
     folders = set()
     titles_and_folders = set()
     title_folder_mapping = {}
 
     if final_dest:
-        final_dest_folder = MEDIA_ROOT / pathlib.Path(final_dest)
+        final_dest_folder = get_media_root() / pathlib.Path(final_dest)
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         current_folder = None
         current_title = None
@@ -71,17 +71,17 @@
                 folder_name = soup.select("title")[0].get_text()  # type: ignore
                 title = folder_name.strip().rstrip()
                 titles.add(title)
                 titles_and_folders.add((title, folder_name))
                 current_title = title
 
         if final_dest:
-            new_folder = MEDIA_ROOT / final_dest / folder_name
+            new_folder = get_media_root() / final_dest / folder_name
         else:
-            new_folder = MEDIA_ROOT / folder_name
+            new_folder = get_media_root() / folder_name
 
         if not new_folder.exists():
             new_folder.mkdir(parents=True, exist_ok=True)
 
         current_folder = new_folder
         folders.add(current_folder)
         unique_img_urls = set()
```

### Comparing `grabberlib-0.0.6/grabber/core/sources/xasiat.py` & `grabberlib-0.0.7/grabber/core/sources/xiuren.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,117 +2,121 @@
 import pathlib
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from typing import List
 
 from tqdm import tqdm
 
-from grabber.core.settings import MEDIA_ROOT
+from grabber.core.settings import get_media_root
 from grabber.core.utils import (
+    get_pages_from_pagination,
     query_mapping,
     headers_mapping,
     get_tags,
     download_images,
     upload_to_telegraph,
 )
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 
 
-def get_for_xasiat(
+def get_sources_for_xiuren(
     sources: List[str],
     entity: str,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
     **kwargs,
 ) -> None:
     titles = set()
+    is_tag: bool = kwargs.get("is_tag", False)
+    limit: int = kwargs.get("limit", 0)
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
+        desc="Retrieving URLs...",
     )
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
     folders = set()
     titles_and_folders = set()
     title_folder_mapping = {}
 
     if final_dest:
-        final_dest_folder = MEDIA_ROOT / final_dest
+        final_dest_folder = get_media_root() / final_dest
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         folder_name = ""
-        tqdm_sources_iterable.set_description(f"Retrieving URLs from {source_url}")
+
+        if is_tag:
+            urls = get_pages_from_pagination(url=source_url, target="xiuren")
+            targets = urls[:limit] if limit else urls
+            return get_sources_for_xiuren(
+                sources=targets,
+                entity=entity,
+                final_dest=final_dest,
+                save_to_telegraph=save_to_telegraph,
+                is_tag=False,
+            )
+
         tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
 
         title_tag = soup.select("title")[0]  # type: ignore
         folder_name = title_tag.get_text().strip().rstrip()
         title = folder_name
         titles.add(title)
         titles_and_folders.add((title, folder_name))
 
         if final_dest:
-            new_folder = MEDIA_ROOT / final_dest / folder_name
+            new_folder = get_media_root() / final_dest / folder_name
         else:
-            new_folder = MEDIA_ROOT / folder_name
+            new_folder = get_media_root() / folder_name
 
         if not new_folder.exists():
             new_folder.mkdir(parents=True, exist_ok=True)
 
         folders.add(new_folder)
         unique_img_urls = set()
 
         for idx, img_tag in enumerate(tags or []):
             img_src = img_tag.attrs[src_attr]
-
-            if "xasiat" in img_src:
-                img_name: str = img_src.split("/")[-2]
-                img_name = img_name.strip().rstrip()
-                img_extension: str = img_name.split(".")[-1]
-            else:
-                img_name: str = img_src.split("/")[-1]
-                img_name = img_name.strip().rstrip()
-                img_extension: str = img_name.split(".")[-1]
-
-            unique_img_urls.add(
-                (title, f"{idx + 1}.{img_extension}", img_src),
-            )
+            img_name: str = img_src.split("/")[-1]
+            img_name = img_name.strip().rstrip()
+            unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
 
         title_folder_mapping[title] = (unique_img_urls, new_folder)
 
     futures = []
     with ThreadPoolExecutor(max_workers=DEFAULT_THREADS_NUMBER) as executor:
         for title, (images_set, folder_dest) in title_folder_mapping.items():
             partial_download = partial(
                 download_images,
                 new_folder=folder_dest,
                 headers=headers,
                 title=title,
             )
-            future = executor.submit(partial_download, images_set, title=title)
+            future = executor.submit(partial_download, images_set)
             futures.append(future)
 
     for future in tqdm(
         futures,
         total=len(futures),
         desc="Finishing download...",
     ):
         future.result()
 
     if save_to_telegraph:
-        for folder in folders:
-            print(f"Uploading to telegraph {folder}")
-            upload_to_telegraph(folder)
+        for title, (_, folder_dest) in title_folder_mapping.items():
+            upload_to_telegraph(folder_dest, page_title=title)
 
     albums_message = "".join([f"- {title}\n" for title in titles])
     message = f"""
     All images have been downloaded and saved to the specified folder.
     Albums saved are the following:
         {albums_message}
     """
```

### Comparing `grabberlib-0.0.6/grabber/core/sources/xiuren.py` & `grabberlib-0.0.7/grabber/core/sources/graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,121 +2,111 @@
 import pathlib
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from typing import List
 
 from tqdm import tqdm
 
-from grabber.core.settings import MEDIA_ROOT
+from grabber.core.settings import get_media_root
 from grabber.core.utils import (
-    get_pages_from_pagination,
     query_mapping,
     headers_mapping,
     get_tags,
     download_images,
     upload_to_telegraph,
 )
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 
 
-def get_sources_for_xiuren(
+def get_for_telegraph(
     sources: List[str],
     entity: str,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
     **kwargs,
 ) -> None:
     titles = set()
-    is_tag: bool = kwargs.get("is_tag", False)
-    limit: int = kwargs.get("limit", 0)
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
-        desc="Retrieving URLs...",
     )
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
     folders = set()
     titles_and_folders = set()
     title_folder_mapping = {}
 
     if final_dest:
-        final_dest_folder = MEDIA_ROOT / final_dest
+        final_dest_folder = get_media_root() / final_dest
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         folder_name = ""
-
-        if is_tag:
-            urls = get_pages_from_pagination(url=source_url, target="xiuren")
-            targets = urls[:limit] if limit else urls
-            return get_sources_for_xiuren(
-                sources=targets,
-                entity=entity,
-                final_dest=final_dest,
-                save_to_telegraph=save_to_telegraph,
-                is_tag=False,
-            )
-
         tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
 
         title_tag = soup.select("title")[0]  # type: ignore
         folder_name = title_tag.get_text().strip().rstrip()
         title = folder_name
         titles.add(title)
         titles_and_folders.add((title, folder_name))
 
         if final_dest:
-            new_folder = MEDIA_ROOT / final_dest / folder_name
+            new_folder = get_media_root() / final_dest / folder_name
         else:
-            new_folder = MEDIA_ROOT / folder_name
+            new_folder = get_media_root() / folder_name
 
         if not new_folder.exists():
             new_folder.mkdir(parents=True, exist_ok=True)
 
         folders.add(new_folder)
         unique_img_urls = set()
 
         for idx, img_tag in enumerate(tags or []):
             img_src = img_tag.attrs[src_attr]
             img_name: str = img_src.split("/")[-1]
             img_name = img_name.strip().rstrip()
-            unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
+            if "images.hotgirl.asia" not in img_src:
+                unique_img_urls.add(
+                    (f"{idx + 1}-{img_name}", f"https://telegra.ph{img_src}")
+                )
+            else:
+                unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
 
         title_folder_mapping[title] = (unique_img_urls, new_folder)
 
     futures = []
     with ThreadPoolExecutor(max_workers=DEFAULT_THREADS_NUMBER) as executor:
         for title, (images_set, folder_dest) in title_folder_mapping.items():
             partial_download = partial(
                 download_images,
                 new_folder=folder_dest,
                 headers=headers,
                 title=title,
             )
-            future = executor.submit(partial_download, images_set)
+            future = executor.submit(partial_download, images_set, title=title)
             futures.append(future)
 
     for future in tqdm(
         futures,
         total=len(futures),
         desc="Finishing download...",
     ):
         future.result()
 
     if save_to_telegraph:
-        for title, (_, folder_dest) in title_folder_mapping.items():
-            upload_to_telegraph(folder_dest, page_title=title)
+        for folder in folders:
+            print(f"Uploading to telegraph {folder}")
+            upload_to_telegraph(folder)
 
     albums_message = "".join([f"- {title}\n" for title in titles])
     message = f"""
     All images have been downloaded and saved to the specified folder.
     Albums saved are the following:
         {albums_message}
     """
```

### Comparing `grabberlib-0.0.6/grabber/core/utils.py` & `grabberlib-0.0.7/grabber/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from lxml import etree
 from PIL import Image
 from telegraph import Telegraph
 from telegraph import exceptions
 from tenacity import retry, wait_chain, wait_fixed
 from tqdm import tqdm
 
-from grabber.core.settings import MEDIA_ROOT
+from grabber.core.settings import get_media_root
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 PAGINATION_QUERY = "div.jeg_navigation.jeg_pagination"
 PAGINATION_PAGES_COUNT_QUERY = f"{PAGINATION_QUERY} span.page_info"
 PAGINATION_BASE_URL_QUERY = "div.jeg_navigation.jeg_pagination a.page_number"
 POSTS_QUERY_XPATH = "/html/body/div[2]/div[5]/div/div[1]/div/div/div[2]/div/div/div[2]/div/div[1]/div/div/div/article/div/div/a"
 
@@ -286,31 +286,33 @@
     except exceptions.TelegraphException as exc:
         print(f"Error: {exc} - {title} - {folder}")
         if "None" not in content:
             with open(uploaded_files_url_path, "w") as f:
                 f.write("\n".join(files_urls))
         return
 
-    with open("assets/pages.txt", "a") as f:
+    with open(get_media_root() / "assets/pages.txt", "a") as f:
         f.write(f"{title} - {page_url}\n")
 
     return page_url
 
 
 def upload_folders_to_telegraph(
     folder_name: Optional[str] = "",
     limit: Optional[int] = 0,
 ) -> None:
     folders = []
 
     if folder_name:
-        root = MEDIA_ROOT / folder_name
+        root = get_media_root() / folder_name
         folders += [f for f in list(root.iterdir()) if f.is_dir()]
     else:
-        root_folders = [folder for folder in MEDIA_ROOT.iterdir() if folder.is_dir()]
+        root_folders = [
+            folder for folder in get_media_root().iterdir() if folder.is_dir()
+        ]
         for folder in root_folders:
             if folder.is_dir():
                 nested_folders = [f for f in folder.iterdir() if f.is_dir()]
                 if nested_folders:
                     folders += nested_folders
                 else:
                     folders = root_folders
```

### Comparing `grabberlib-0.0.6/pyproject.toml` & `grabberlib-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
     { include = "assets/pages.txt" },
 ]
```

### Comparing `grabberlib-0.0.6/PKG-INFO` & `grabberlib-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

