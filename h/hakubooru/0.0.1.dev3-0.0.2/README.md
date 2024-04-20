# Comparing `tmp/hakubooru-0.0.1.dev3.tar.gz` & `tmp/hakubooru-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hakubooru-0.0.1.dev3.tar", last modified: Sat Feb  3 09:12:36 2024, max compression
+gzip compressed data, was "hakubooru-0.0.2.tar", last modified: Sat Apr 20 13:40:10 2024, max compression
```

## Comparing `hakubooru-0.0.1.dev3.tar` & `hakubooru-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-02-03 09:12:36.166833 hakubooru-0.0.1.dev3/
--rw-rw-rw-   0        0        0    11550 2024-01-27 15:29:18.000000 hakubooru-0.0.1.dev3/LICENSE
--rw-rw-rw-   0        0        0      347 2024-02-03 09:12:36.165834 hakubooru-0.0.1.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     2404 2024-01-29 09:27:58.000000 hakubooru-0.0.1.dev3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-03 09:12:36.158829 hakubooru-0.0.1.dev3/hakubooru/
--rw-rw-rw-   0        0        0       28 2024-01-27 15:10:36.000000 hakubooru-0.0.1.dev3/hakubooru/__init__.py
--rw-rw-rw-   0        0        0     3645 2024-02-03 09:11:16.000000 hakubooru-0.0.1.dev3/hakubooru/caption.py
-drwxrwxrwx   0        0        0        0 2024-02-03 09:12:36.165834 hakubooru-0.0.1.dev3/hakubooru/dataset/
--rw-rw-rw-   0        0        0      189 2024-02-02 05:01:19.000000 hakubooru-0.0.1.dev3/hakubooru/dataset/__init__.py
--rw-rw-rw-   0        0        0      181 2024-01-27 15:10:36.000000 hakubooru-0.0.1.dev3/hakubooru/dataset/__main__.py
--rw-rw-rw-   0        0        0     5669 2024-02-02 04:53:26.000000 hakubooru-0.0.1.dev3/hakubooru/dataset/db.py
--rw-rw-rw-   0        0        0      468 2024-02-02 05:00:59.000000 hakubooru-0.0.1.dev3/hakubooru/dataset/utils.py
--rw-rw-rw-   0        0        0     6393 2024-02-02 12:48:51.000000 hakubooru-0.0.1.dev3/hakubooru/export.py
--rw-rw-rw-   0        0        0     1024 2024-01-30 14:35:58.000000 hakubooru-0.0.1.dev3/hakubooru/logging.py
--rw-rw-rw-   0        0        0     3545 2024-01-27 15:07:11.000000 hakubooru-0.0.1.dev3/hakubooru/metainfo.py
--rw-rw-rw-   0        0        0     2029 2024-01-27 06:36:24.000000 hakubooru-0.0.1.dev3/hakubooru/tag_generator.py
-drwxrwxrwx   0        0        0        0 2024-02-03 09:12:36.163835 hakubooru-0.0.1.dev3/hakubooru.egg-info/
--rw-rw-rw-   0        0        0      347 2024-02-03 09:12:36.000000 hakubooru-0.0.1.dev3/hakubooru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2024-02-03 09:12:36.000000 hakubooru-0.0.1.dev3/hakubooru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-03 09:12:36.000000 hakubooru-0.0.1.dev3/hakubooru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-27 15:45:56.000000 hakubooru-0.0.1.dev3/hakubooru.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2024-02-03 09:12:36.000000 hakubooru-0.0.1.dev3/hakubooru.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-03 09:12:36.000000 hakubooru-0.0.1.dev3/hakubooru.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-03 09:12:36.166833 hakubooru-0.0.1.dev3/setup.cfg
--rw-rw-rw-   0        0        0      451 2024-02-03 09:12:26.000000 hakubooru-0.0.1.dev3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:40:10.939708 hakubooru-0.0.2/
+-rw-rw-rw-   0        0        0    11550 2024-01-27 15:29:18.000000 hakubooru-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      374 2024-04-20 13:40:10.938709 hakubooru-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5325 2024-02-21 13:06:46.000000 hakubooru-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 13:40:10.914152 hakubooru-0.0.2/hakubooru/
+-rw-rw-rw-   0        0        0       28 2024-01-27 15:10:36.000000 hakubooru-0.0.2/hakubooru/__init__.py
+-rw-rw-rw-   0        0        0     3790 2024-03-23 06:21:34.000000 hakubooru-0.0.2/hakubooru/caption.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:40:10.937702 hakubooru-0.0.2/hakubooru/dataset/
+-rw-rw-rw-   0        0        0      185 2024-02-25 09:46:22.000000 hakubooru-0.0.2/hakubooru/dataset/__init__.py
+-rw-rw-rw-   0        0        0      181 2024-01-27 15:10:36.000000 hakubooru-0.0.2/hakubooru/dataset/__main__.py
+-rw-rw-rw-   0        0        0     7901 2024-04-20 12:51:33.000000 hakubooru-0.0.2/hakubooru/dataset/db.py
+-rw-rw-rw-   0        0        0     1154 2024-04-20 13:33:21.000000 hakubooru-0.0.2/hakubooru/dataset/utils.py
+-rw-rw-rw-   0        0        0     5444 2024-02-25 09:33:53.000000 hakubooru-0.0.2/hakubooru/export.py
+-rw-rw-rw-   0        0        0     1024 2024-01-30 14:35:58.000000 hakubooru-0.0.2/hakubooru/logging.py
+-rw-rw-rw-   0        0        0     4387 2024-04-20 13:38:52.000000 hakubooru-0.0.2/hakubooru/metainfo.py
+-rw-rw-rw-   0        0        0     4631 2024-03-20 13:27:16.000000 hakubooru-0.0.2/hakubooru/source.py
+-rw-rw-rw-   0        0        0     3025 2024-03-20 13:29:53.000000 hakubooru-0.0.2/hakubooru/tag_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:40:10.938709 hakubooru-0.0.2/hakubooru.egg-info/
+-rw-rw-rw-   0        0        0      374 2024-04-20 13:40:10.000000 hakubooru-0.0.2/hakubooru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2024-04-20 13:40:10.000000 hakubooru-0.0.2/hakubooru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 13:40:10.000000 hakubooru-0.0.2/hakubooru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-27 15:45:56.000000 hakubooru-0.0.2/hakubooru.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2024-04-20 13:40:10.000000 hakubooru-0.0.2/hakubooru.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-20 13:40:10.000000 hakubooru-0.0.2/hakubooru.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 13:40:10.939708 hakubooru-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      500 2024-04-20 13:40:07.000000 hakubooru-0.0.2/setup.py
```

### Comparing `hakubooru-0.0.1.dev3/LICENSE` & `hakubooru-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hakubooru-0.0.1.dev3/hakubooru/caption.py` & `hakubooru-0.0.2/hakubooru/caption.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from hakubooru.metainfo import (
     meta_keywords_black_list,
     special_tags,
 )
 from hakubooru.tag_generator import (
     rating_tag,
     quality_tag,
+    quality_tag_new,
     year_tag,
 )
 from hakubooru.dataset.db import (
     Post,
     Tag,
 )
 
@@ -17,24 +18,25 @@
     return [
         tag.name.replace("_", tag_word_sep) if len(tag.name) > 3 else tag.name
         for tag in tag_list
         if tag.name.strip()
     ]
 
 
+def tags_filter(tag: Tag, black_list: list[str]) -> bool:
+    return not any(keyword in tag.name for keyword in black_list)
+
+
 def meta_tags_filter(tag: Tag) -> bool:
     if tag.type != "meta":
         return True
 
     # NOTE: we only filter out meta tags with these keywords
     # Which is definitely not related to the content of image
-    if any(keyword in tag.name for keyword in meta_keywords_black_list):
-        return False
-
-    return True
+    return tags_filter(tag, meta_keywords_black_list)
 
 
 def extract_special_tags(tag_list: list[Tag]) -> tuple[list[str], list[str]]:
     special = []
     general = []
     for tag in tag_list:
         if tag.name in special_tags:
@@ -52,15 +54,18 @@
     processor=[year_tag, rating_tag, quality_tag],
 ) -> str:
     special_tag_list, general_tag_list = extract_special_tags(post.tag_list_general)
     special_tag_list = tag_str_list(special_tag_list, tag_word_sep)
     general_tag_list = tag_str_list(general_tag_list, tag_word_sep)
     character_tag_list = tag_str_list(post.tag_list_character, tag_word_sep)
     copyright_tag_list = tag_str_list(post.tag_list_copyright, tag_word_sep)
-    artists_tag_list = tag_str_list(post.tag_list_artist, tag_word_sep)
+    artists_tag_list = tag_str_list(
+        [tag for tag in post.tag_list_artist if tags_filter(tag, ["banned"])],
+        tag_word_sep,
+    )
     meta_tag_list = tag_str_list(
         [tag for tag in post.tag_list_meta if meta_tags_filter(tag)], tag_word_sep
     )
 
     keep_tags = (
         special_tag_list + character_tag_list + copyright_tag_list + artists_tag_list
     )
@@ -79,15 +84,14 @@
     post_id: int,
     tag_word_sep: str = " ",
     tag_seperator: str = ", ",
     keep_seperator: str = "|||",
     processor=[year_tag, rating_tag, quality_tag],
 ) -> str:
     post = Post.get_by_id(post_id)
-    print(post.file_url)
     if post is None:
         raise Exception(f"Post with id {post_id} not found")
     return make_caption(post, tag_word_sep, tag_seperator, keep_seperator, processor)
 
 
 class BaseCaptioner:
     def caption(self, post: Post, img: bytes) -> str:
@@ -96,15 +100,15 @@
 
 class KohakuCaptioner(BaseCaptioner):
     def __init__(
         self,
         tag_word_sep=" ",
         tag_seperator=", ",
         keep_seperator="|||",
-        processors=[year_tag, rating_tag, quality_tag],
+        processors=[year_tag, rating_tag, quality_tag_new],
     ):
         self.processors = processors
         self.tag_word_sep = tag_word_sep
         self.tag_seperator = tag_seperator
         self.keep_seperator = keep_seperator
 
     def caption(self, post: Post, img: bytes) -> str:
```

### Comparing `hakubooru-0.0.1.dev3/hakubooru/export.py` & `hakubooru-0.0.2/hakubooru/export.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import os
 import re
+from threading import Lock
 from concurrent.futures import ThreadPoolExecutor
 
 import webdataset as wds
 from tqdm import tqdm
+from peewee import chunked
 
-from hakubooru.dataset.db import db, Post
 from hakubooru.caption import BaseCaptioner, KohakuCaptioner
+from hakubooru.dataset.db import db, Post
 from hakubooru.logging import logger
+from hakubooru.source import BaseSource
 
 
 file_id_regex = re.compile(r"data-(\d+)\.tar")
 
 
 class BaseSaver:
     def __init__(self, output_dir: str, caption_ext: str = "txt"):
@@ -57,35 +60,75 @@
         if caption is not None:
             with open(
                 os.path.join(self.output_dir, f"{img_id}.{self.caption_ext}"), "w"
             ) as f:
                 f.write(caption)
 
 
+class TextSaver(BaseSaver):
+    def __init__(
+        self, output_dir: str, caption_ext: str = "txt", one_file: bool = True
+    ):
+        super().__init__(output_dir, caption_ext)
+        self.one_file = one_file
+        if self.one_file:
+            self.cache = []
+            self.file_lock = Lock()
+            self.file = open(
+                os.path.join(self.output_dir, f"captions.{self.caption_ext}"), "w"
+            )
+
+    def __del__(self):
+        if self.one_file:
+            logger.info(f"Writing {len(self.cache)} captions")
+            self.file.write("\n".join(self.cache) + "\n")
+            self.file.close()
+
+    def __call__(self, img_id: int, img_data: bytes, img_ext: str, caption: str):
+        if self.one_file:
+            self.cache.append(caption)
+        else:
+            with open(
+                os.path.join(self.output_dir, f"{img_id}.{self.caption_ext}"), "w"
+            ) as f:
+                f.write(caption)
+
+
+class DummyPoolExecutor:
+    def map(self, func, args):
+        for arg in args:
+            yield func(arg)
+
+
 class Exporter:
     def __init__(
         self,
-        dataset_dir: str,
+        source: BaseSource,
         saver: BaseSaver = FileSaver("./out"),
         captioner: BaseCaptioner | None = KohakuCaptioner(),
+        process_batch_size=1000,
+        process_threads=16,
     ):
         # ThreadPool will speed up database query and saver
-        self.pool = ThreadPoolExecutor(16)
-        self.dataset_dir = dataset_dir
+        if process_threads:
+            self.pool = ThreadPoolExecutor(process_threads)
+        else:
+            self.pool = DummyPoolExecutor()
 
+        self.source = source
         self.saver = saver
         self.captioner = captioner
 
         self.do_caption = captioner is not None
+        self.batch_size = process_batch_size
 
     def process_data(self, args):
         fail = success = False
-        data_id, data, post = args
+        data_id, content, ext, post = args
         try:
-            ext, content = list(data.items())[-1]
             if self.do_caption:
                 caption = self.captioner.caption(post, content)
             else:
                 caption = None
 
             self.saver(
                 data_id,
@@ -98,100 +141,29 @@
                 f"Error occured when doing captioning and saving {data_id}: {e}"
             )
             fail = True
         if not fail:
             success = True
         return data_id, success, fail
 
-    def _export(self, tar_files, post_dict):
-        success = fail = 0
-        # Concat main and sub dataset together
-        dataset = wds.WebDataset(tar_files)
-        data_cache = {}
-
-        for data in iter(dataset):
-            data_id = int(data["__key__"])
-            if data_id in post_dict:
-                data_cache[data_id] = data
-                if len(data_cache) == len(post_dict):
-                    break
-
-        args = [
-            (data_id, data, post_dict[data_id]) for data_id, data in data_cache.items()
-        ]
-
-        for data_id, s, f in self.pool.map(self.process_data, args):
-            success += s
-            fail += f
-            if s:
-                del post_dict[data_id]
-        return success, fail
-
     def export_posts(self, choosed_posts: list[Post]):
-        dataset_dir = self.dataset_dir
-
-        # Read all tar files we have
-        existed_tar = {
-            int(file_id_regex.match(f).group(1)): [
-                os.path.join(dataset_dir, f).replace("\\", "/")
-            ]
-            for f in os.listdir(dataset_dir)
-            if f.endswith(".tar")
-        }
-        assert len(existed_tar), "Dataset is empty"
-
-        # Group posts by bucket
-        id_map = {}
-        for post in choosed_posts:
-            bucket_id = post.id % 1000
-            if bucket_id not in id_map:
-                id_map[bucket_id] = {}
-            id_map[bucket_id][post.id] = post
-        id_map = {k: id_map[k] for k in sorted(id_map)}
-
-        # Export
-        bucket_not_found = set()
-        success = 0
-        fail = 0
-        for bucket_id, post_dict in tqdm(
-            id_map.items(), desc="reading buckets", smoothing=0.1
-        ):
-            if bucket_id not in existed_tar and bucket_id + 1000 not in existed_tar:
-                bucket_not_found.add(bucket_id)
-                continue
-
-            # Concat main and sub dataset together
-            s, f = self._export(
-                existed_tar.get(bucket_id, []) + existed_tar.get(bucket_id + 1000, []),
-                post_dict,
-            )
-            success += s
-            fail += f
-
-        remains = {}
-        for _, post_dict in id_map.items():
-            remains.update(post_dict)
-
-        # Check addon dataset if needed
-        if remains and 2000 in existed_tar:
-            s, f = self._export(existed_tar[2000], post_dict)
-            success += s
-            fail += f
+        success = fail = 0
+        for datas in chunked(self.source.read(choosed_posts), self.batch_size):
+            for data_id, s, f in self.pool.map(self.process_data, datas):
+                success += s
+                fail += f
 
-        post_not_found = len(remains)
+        post_not_found = self.source.not_found
 
-        if bucket_not_found:
-            logger.warning(
-                f"{len(bucket_not_found)} posts are not exported"
-                "because the bucket doesn't exist"
-            )
+        del self.saver
+        del self.source
 
         if post_not_found:
             logger.warning(
-                f"{post_not_found} posts are not found in the dataset\n"
+                f"{len(post_not_found)} posts are not found in the dataset\n"
                 "Some of them are gif or mp4 or corrupted files so small number is normal\n"
                 "Lot of not found can be caused by missing/outdating dataset files or corrupted dataset files"
             )
 
         if fail:
             logger.warning(
                 f"{fail} images failed to captioning and save\n"
```

### Comparing `hakubooru-0.0.1.dev3/hakubooru/logging.py` & `hakubooru-0.0.2/hakubooru/logging.py`

 * *Files identical despite different names*

### Comparing `hakubooru-0.0.1.dev3/hakubooru/metainfo.py` & `hakubooru-0.0.2/hakubooru/metainfo.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,14 +39,37 @@
     "mismatch",
     "revision",
     "audio",
     "video",
 ]
 
 
+fav_count_percentile_full = {
+    "general": {
+        5: 1, 10: 1, 15: 2, 20: 3, 25: 3, 30: 4, 35: 5,
+        40: 6, 45: 7, 50: 8, 55: 9, 60: 10, 65: 12,
+        70: 14, 75: 16, 80: 18, 85: 22, 90: 27, 95: 37
+    },
+    "sensitive": {
+        5: 1, 10: 2, 15: 4, 20: 5, 25: 6, 30: 8, 35: 9,
+        40: 11, 45: 13, 50: 15, 55: 17, 60: 19, 65: 22,
+        70: 26, 75: 30, 80: 36, 85: 44, 90: 56, 95: 81
+    },
+    "questionable": {
+        5: 4, 10: 8, 15: 11, 20: 14, 25: 18, 30: 21, 35: 25,
+        40: 29, 45: 33, 50: 38, 55: 43, 60: 49, 65: 56,
+        70: 65, 75: 75, 80: 88, 85: 105, 90: 132, 95: 182
+    },
+    "explicit": {
+        5: 4, 10: 9, 15: 13, 20: 18, 25: 22, 30: 27, 35: 33,
+        40: 39, 45: 45, 50: 52, 55: 60, 60: 69, 65: 79,
+        70: 92, 75: 106, 80: 125, 85: 151, 90: 190, 95: 262
+    },
+}
+
 score_percentile_full = {
     "general": {
         5: 0,
         10: 1,
         15: 2,
         20: 3,
         25: 3,
```

### Comparing `hakubooru-0.0.1.dev3/hakubooru/tag_generator.py` & `hakubooru-0.0.2/hakubooru/tag_generator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import dateutil.parser
 
 from hakubooru.dataset.db import (
     Post,
 )
 from hakubooru.metainfo import (
     rating_map,
-    score_percentile_after_5m,
+    fav_count_percentile_full,
 )
 
 
 def year_tag(
     post: Post, keep_tags: list[str], general_tags: list[str]
 ) -> tuple[list[str], list[str]]:
     year = 0
@@ -42,21 +42,21 @@
     return keep_tags, general_tags
 
 
 def quality_tag(
     post: Post,
     keep_tags: list[str],
     general_tags: list[str],
-    percentile_map: dict[str, dict[int, int]] = score_percentile_after_5m,
+    percentile_map: dict[str, dict[int, int]] = fav_count_percentile_full,
 ) -> tuple[list[str], list[str]]:
-    if post.id > 6880000:
+    if post.id > 7000000:
         # Don't add quality tag for posts which are new.
         return keep_tags, general_tags
     rating = post.rating
-    score = post.score
+    score = post.fav_count
     percentile = percentile_map[rating]
 
     if score > percentile[95]:
         quality_tag = "masterpiece"
     elif score > percentile[85]:
         quality_tag = "best quality"
     elif score > percentile[75]:
@@ -67,9 +67,42 @@
         quality_tag = "normal quality"
     elif score > percentile[10]:
         quality_tag = "low quality"
     else:
         quality_tag = "worst quality"
 
     general_tags.append(quality_tag)
+
+    return keep_tags, general_tags
+
+
+def quality_tag_new(
+    post: Post,
+    keep_tags: list[str],
+    general_tags: list[str],
+    percentile_map: dict[str, dict[int, int]] = fav_count_percentile_full,
+) -> tuple[list[str], list[str]]:
+    if post.id > 7100000:
+        # Don't add quality tag for posts which are new.
+        return keep_tags, general_tags
+    rating = post.rating
+    score = post.fav_count
+    percentile = percentile_map[rating]
+
+    if score > percentile[90]:
+        quality_tag = "masterpiece"
+    elif score > percentile[75]:
+        quality_tag = "best quality"
+    elif score > percentile[60]:
+        quality_tag = "great quality"
+    elif score > percentile[45]:
+        quality_tag = "good quality"
+    elif score > percentile[30]:
+        quality_tag = "normal quality"
+    elif score > percentile[10]:
+        quality_tag = "low quality"
+    else:
+        quality_tag = "worst quality"
+
+    general_tags.append(quality_tag)
 
     return keep_tags, general_tags
```

