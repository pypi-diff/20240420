# Comparing `tmp/grabberlib-0.0.5.tar.gz` & `tmp/grabberlib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.0.5.tar", max compression
+gzip compressed data, was "grabberlib-0.0.6.tar", max compression
```

## Comparing `grabberlib-0.0.5.tar` & `grabberlib-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2024-04-19 16:44:36.061439 grabberlib-0.0.5/README.md
--rw-r--r--   0        0        0        1 2024-04-19 21:08:54.051660 grabberlib-0.0.5/assets/pages.txt
--rw-r--r--   0        0        0        0 2024-04-19 16:44:36.031593 grabberlib-0.0.5/grabber/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-19 16:44:36.314458 grabberlib-0.0.5/grabber/__main__.py
--rw-r--r--   0        0        0        0 2024-04-19 16:44:36.314537 grabberlib-0.0.5/grabber/controllers/__init__.py
--rw-r--r--   0        0        0     3798 2024-04-19 21:11:49.668721 grabberlib-0.0.5/grabber/controllers/base.py
--rw-r--r--   0        0        0        0 2024-04-19 16:44:36.315102 grabberlib-0.0.5/grabber/core/__init__.py
--rw-r--r--   0        0        0       65 2024-04-19 16:44:36.315699 grabberlib-0.0.5/grabber/core/exc.py
--rw-r--r--   0        0        0      188 2024-04-19 16:50:32.400947 grabberlib-0.0.5/grabber/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-19 16:44:36.316024 grabberlib-0.0.5/grabber/core/sources/__init__.py
--rw-r--r--   0        0        0     3378 2024-04-19 17:11:11.625028 grabberlib-0.0.5/grabber/core/sources/graph.py
--rw-r--r--   0        0        0     3986 2024-04-19 17:48:30.254982 grabberlib-0.0.5/grabber/core/sources/khd.py
--rw-r--r--   0        0        0     3588 2024-04-19 17:11:18.798709 grabberlib-0.0.5/grabber/core/sources/xasiat.py
--rw-r--r--   0        0        0     3717 2024-04-19 17:10:44.092619 grabberlib-0.0.5/grabber/core/sources/xiuren.py
--rw-r--r--   0        0        0        1 2024-04-19 16:44:36.392872 grabberlib-0.0.5/grabber/core/sources/yellow.py
--rw-r--r--   0        0        0    12856 2024-04-19 21:01:29.273811 grabberlib-0.0.5/grabber/core/utils.py
--rw-r--r--   0        0        0      175 2024-04-19 21:09:53.350881 grabberlib-0.0.5/grabber/core/version.py
--rw-r--r--   0        0        0        0 2024-04-19 16:44:36.318014 grabberlib-0.0.5/grabber/templates/__init__.py
--rw-r--r--   0        0        0     1017 2024-04-19 21:09:44.516801 grabberlib-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-19 16:44:36.061439 grabberlib-0.0.6/README.md
+-rw-r--r--   0        0        0        1 2024-04-19 21:08:54.051660 grabberlib-0.0.6/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-04-19 16:44:36.031593 grabberlib-0.0.6/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-19 16:44:36.314458 grabberlib-0.0.6/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:44:36.314537 grabberlib-0.0.6/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     3798 2024-04-19 21:11:49.668721 grabberlib-0.0.6/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:44:36.315102 grabberlib-0.0.6/grabber/core/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-19 16:44:36.315699 grabberlib-0.0.6/grabber/core/exc.py
+-rw-r--r--   0        0        0      188 2024-04-19 16:50:32.400947 grabberlib-0.0.6/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:44:36.316024 grabberlib-0.0.6/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0     3378 2024-04-19 17:11:11.625028 grabberlib-0.0.6/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     3986 2024-04-19 17:48:30.254982 grabberlib-0.0.6/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     3588 2024-04-19 17:11:18.798709 grabberlib-0.0.6/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     3718 2024-04-19 21:24:29.005339 grabberlib-0.0.6/grabber/core/sources/xiuren.py
+-rw-r--r--   0        0        0        1 2024-04-19 16:44:36.392872 grabberlib-0.0.6/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0    13070 2024-04-19 21:25:00.367081 grabberlib-0.0.6/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-04-19 21:25:25.122215 grabberlib-0.0.6/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:44:36.318014 grabberlib-0.0.6/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1017 2024-04-19 21:25:18.090165 grabberlib-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.6/PKG-INFO
```

### Comparing `grabberlib-0.0.5/grabber/__main__.py` & `grabberlib-0.0.6/grabber/__main__.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.5/grabber/controllers/base.py` & `grabberlib-0.0.6/grabber/controllers/base.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.5/grabber/core/sources/graph.py` & `grabberlib-0.0.6/grabber/core/sources/graph.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.5/grabber/core/sources/khd.py` & `grabberlib-0.0.6/grabber/core/sources/khd.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.5/grabber/core/sources/xasiat.py` & `grabberlib-0.0.6/grabber/core/sources/xasiat.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.5/grabber/core/sources/xiuren.py` & `grabberlib-0.0.6/grabber/core/sources/xiuren.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,31 +44,32 @@
         final_dest_folder = MEDIA_ROOT / final_dest
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         folder_name = ""
-        tags, soup = get_tags(
-            source_url,
-            headers=headers,
-            query=query,
-        )
 
         if is_tag:
             urls = get_pages_from_pagination(url=source_url, target="xiuren")
             targets = urls[:limit] if limit else urls
             return get_sources_for_xiuren(
                 sources=targets,
                 entity=entity,
                 final_dest=final_dest,
                 save_to_telegraph=save_to_telegraph,
                 is_tag=False,
             )
 
+        tags, soup = get_tags(
+            source_url,
+            headers=headers,
+            query=query,
+        )
+
         title_tag = soup.select("title")[0]  # type: ignore
         folder_name = title_tag.get_text().strip().rstrip()
         title = folder_name
         titles.add(title)
         titles_and_folders.add((title, folder_name))
 
         if final_dest:
```

### Comparing `grabberlib-0.0.5/grabber/core/utils.py` & `grabberlib-0.0.6/grabber/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,16 +340,20 @@
 
 def get_pages_from_pagination(url: str, target: str) -> List[str]:
     pagination_params = query_pagination_mapping[target]
     source_urls = []
     soup = get_soup(url)
     dom = etree.HTML(str(soup))
     pagination_set = soup.select(pagination_params.pages_count_query)
+
     if not pagination_set:
-        return []
+        for a_tag in dom.xpath(pagination_params.posts_query_xpath):
+            if a_tag is not None and a_tag.attrib["href"] not in source_urls:
+                source_urls.append(a_tag.attrib["href"])
+        return source_urls
 
     pagination = pagination_set[0]
     pagination_text = pagination.text
     first, last = pagination_text.split("Page")[-1].strip().split("of")
     first_page, last_page = int(first), int(last)
 
     first_link_pagination = soup.select(pagination_params.pagination_base_url_query)[0]
```

### Comparing `grabberlib-0.0.5/pyproject.toml` & `grabberlib-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
     { include = "assets/pages.txt" },
 ]
```

### Comparing `grabberlib-0.0.5/PKG-INFO` & `grabberlib-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

