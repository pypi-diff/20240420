# Comparing `tmp/szurubooru_toolkit-1.0.0.tar.gz` & `tmp/szurubooru_toolkit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "szurubooru_toolkit-1.0.0.tar", max compression
+gzip compressed data, was "szurubooru_toolkit-1.0.1.tar", max compression
```

## Comparing `szurubooru_toolkit-1.0.0.tar` & `szurubooru_toolkit-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2024-02-10 12:00:31.327259 szurubooru_toolkit-1.0.0/LICENSE
--rw-r--r--   0        0        0     8055 2024-02-10 12:00:31.327259 szurubooru_toolkit-1.0.0/README.md
--rw-r--r--   0        0        0     1404 2024-02-10 12:00:31.327259 szurubooru_toolkit-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2467 2024-02-10 12:00:31.327259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/__init__.py
--rw-r--r--   0        0        0    12401 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/config.py
--rw-r--r--   0        0        0    10890 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/danbooru.py
--rw-r--r--   0        0        0     4859 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/deepbooru.py
--rw-r--r--   0        0        0     6118 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/pixiv.py
--rw-r--r--   0        0        0     8022 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/saucenao.py
--rw-r--r--   0        0        0        0 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/__init__.py
--rw-r--r--   0        0        0    13042 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/auto_tagger.py
--rw-r--r--   0        0        0     7795 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/create_relations.py
--rw-r--r--   0        0        0     3230 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/create_tags.py
--rw-r--r--   0        0        0     1702 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/delete_posts.py
--rw-r--r--   0        0        0     2214 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/import_from_booru.py
--rw-r--r--   0        0        0     8307 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/import_from_url.py
--rw-r--r--   0        0        0     1715 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/reset_posts.py
--rw-r--r--   0        0        0    23490 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/szuru_toolkit.py
--rw-r--r--   0        0        0     2442 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/tag_posts.py
--rw-r--r--   0        0        0    15804 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/upload_media.py
--rw-r--r--   0        0        0    15342 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/szurubooru.py
--rw-r--r--   0        0        0    20233 2024-02-10 12:00:31.331259 szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/utils.py
--rw-r--r--   0        0        0     9410 1970-01-01 00:00:00.000000 szurubooru_toolkit-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-20 10:43:58.758032 szurubooru_toolkit-1.0.1/LICENSE
+-rw-r--r--   0        0        0     9682 2024-04-20 10:43:58.758032 szurubooru_toolkit-1.0.1/README.md
+-rw-r--r--   0        0        0     1404 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2467 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/__init__.py
+-rw-r--r--   0        0        0    12464 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/config.py
+-rw-r--r--   0        0        0    10890 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/danbooru.py
+-rw-r--r--   0        0        0     4859 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/deepbooru.py
+-rw-r--r--   0        0        0     6118 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/pixiv.py
+-rw-r--r--   0        0        0     8022 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/saucenao.py
+-rw-r--r--   0        0        0        0 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/__init__.py
+-rw-r--r--   0        0        0    13042 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/auto_tagger.py
+-rw-r--r--   0        0        0     7795 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/create_relations.py
+-rw-r--r--   0        0        0     3230 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/create_tags.py
+-rw-r--r--   0        0        0     1702 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/delete_posts.py
+-rw-r--r--   0        0        0     2214 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/import_from_booru.py
+-rw-r--r--   0        0        0     8307 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/import_from_url.py
+-rw-r--r--   0        0        0     1715 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/reset_posts.py
+-rw-r--r--   0        0        0    23849 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/szuru_toolkit.py
+-rw-r--r--   0        0        0     2862 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/tag_posts.py
+-rw-r--r--   0        0        0    16586 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/upload_media.py
+-rw-r--r--   0        0        0    15313 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/szurubooru.py
+-rw-r--r--   0        0        0    20233 2024-04-20 10:43:58.762032 szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/utils.py
+-rw-r--r--   0        0        0    11037 1970-01-01 00:00:00.000000 szurubooru_toolkit-1.0.1/PKG-INFO
```

### Comparing `szurubooru_toolkit-1.0.0/LICENSE` & `szurubooru_toolkit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/README.md` & `szurubooru_toolkit-1.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -2,19 +2,50 @@
 <img src="https://cdn-icons-png.flaticon.com/512/2581/2581053.png"
   alt="szurubooru-toolkit icon"
   width="128" height="128">
 </p>
 
 # szurubooru-toolkit
 Python package and script collection to manage your [szurubooru](https://github.com/rr-/szurubooru) image board.
+```
+Usage: szuru-toolkit [OPTIONS] COMMAND [ARGS]...
 
+  Toolkit to manage your szurubooru image board.
+
+  Defaults can also be set in a config file.
+
+  Visit https://github.com/reluce/szurubooru-toolkit for more information.
+
+Options:
+  --url TEXT                      Base URL to your szurubooru instance.
+  --username TEXT                 Username which will be used to authenticate with the szurubooru API.
+  --api-token TEXT                API token for the user which will be used to authenticate with the szurubooru API.
+  --public                        If your szurubooru instance is reachable from the internet (default: False).
+  --log-enabled                   Create a log file (default: False).
+  --log-colorized                 Colorize the log output (default: True).
+  --log-file TEXT                 Output file for the log (default: szurubooru_toolkit.log)
+  --log-level [DEBUG|INFO|WARNING|ERROR|CRITICAL]
+                                  Set the log level (default: INFO).
+  --hide-progress                 Hides the progress bar (default: False).
+  -h, --help                      Show this message and exit.
+
+Commands:
+  auto-tagger        Tag posts automatically
+  create-relations   Create relations between character and parody tag categories
+  create-tags        Create tags based on a tag file or query
+  delete-posts       Delete posts
+  import-from-booru  Download and tag posts from various Boorus
+  import-from-url    Download images from URLS or file containing URLs
+  reset-posts        Remove tags and sources
+  tag-posts          Tag posts manually
+  upload-media       Upload media files
+```
 ## :ballot_box_with_check: Requirements
 In order to run `szuru-toolkit`, Python `3.11` is required.
 
-
 ## :hammer_and_wrench: Installation
 This package is available on [PyPI](https://pypi.org/project/szurubooru-toolkit/) and can be installed with pip:
 `pip install szurubooru-toolkit`
 
 Alternatively, you can clone the package from GitHub and set everything up with [Poetry](https://python-poetry.org/docs/). In the root directory of this repository, execute `poetry install`.
 
 ### Docker Instructions
```

### Comparing `szurubooru_toolkit-1.0.0/pyproject.toml` & `szurubooru_toolkit-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 known_first_party = ["szurubooru_toolkit"]
 known_local_folder = ["src/szurubooru_toolkit"]
 multi_line_output = 3
 force_single_line = true
 
 [tool.poetry]
 name = "szurubooru-toolkit"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python package and script collection to manage szurubooru."
 authors = ["reluce <reluce@fkosquad.moe>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/reluce/szurubooru-toolkit"
 documentation = "https://github.com/reluce/szurubooru-toolkit"
 keywords = ["szurubooru", "szuru", "booru", "saucenao", "deepbooru"]
```

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/__init__.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/config.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,22 +72,24 @@
     'deepbooru': False,
     'hide_progress': False,
     'md5_search': False,
     'range': ':100',
     'saucenao': False,
     'tmp_path': './tmp/gallery-dl',
     'use_twitter_artist': False,
+    'update_tags_if_exists': False,
 }
 
 RESET_POSTS_DEFAULTS = {'hide_progress': False}
 
 TAG_POSTS_DEFAULTS = {
     'hide_progress': False,
     'update_implications': False,
     'mode': 'append',
+    'silence_info': False,
 }
 
 UPLOAD_MEDIA_DEFAULTS = {
     'src_path': None,
     'hide_progress': False,
     'cleanup': False,
     'tags': ['tagme'],
```

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/danbooru.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/danbooru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/deepbooru.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/deepbooru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/pixiv.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/pixiv.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/saucenao.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/saucenao.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/auto_tagger.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/auto_tagger.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/create_relations.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/create_relations.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/create_tags.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/create_tags.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/delete_posts.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/delete_posts.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/import_from_booru.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/import_from_booru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/import_from_url.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/import_from_url.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/reset_posts.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/reset_posts.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/szuru_toolkit.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/szuru_toolkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,14 +443,19 @@
     type=int,
     help=f'Images which total pixel count exceeds this value will be shrunk (default: {config.UPLOAD_MEDIA_DEFAULTS["shrink_threshold"]}).',
 )
 @click.option(
     '--shrink-dimensions',
     help=f'Maximum width and height of the shrunken image (default: {config.UPLOAD_MEDIA_DEFAULTS["shrink_dimensions"]}).',
 )
+@click.option(
+    '--update-tags-if-exists/--dont-update-tags-if-exists',
+    is_flag=True,
+    help=f'Append new tags, if any, to already uploaded posts (default: {config.IMPORT_FROM_URL_DEFAULTS["update_tags_if_exists"]}).',
+)
 @click.option('--verbose', is_flag=True, help='Show download progress of gallery-dl script.')
 @click.pass_context
 def click_import_from_url(
     ctx,
     urls,
     input_file,
     range,
@@ -462,14 +467,15 @@
     convert_to_jpg,
     convert_threshold,
     default_safety,
     max_similarity,
     shrink,
     shrink_threshold,
     shrink_dimensions,
+    update_tags_if_exists,
     verbose,
 ):
     """
     Download images from URLS or file containing URLs
 
     URLS is a comma-separated list of URLs to download images from.
     """
@@ -522,37 +528,38 @@
     module.main(query, except_ids, add_tags)
 
 
 @cli.command('tag-posts', epilog='Example: szuru-toolkit tag-posts --add-tags "foo,bar" --remove-tags "baz" "foo"')
 @click.argument('query')
 @click.option('--add-tags', help='Specify tags, separated by a comma, which will be added to all posts matching your query.')
 @click.option('--remove-tags', help='Specify tags, separated by a comma, which will be removed from all posts matching your query.')
+@click.option('--source', help='Set the source of the post')
 @click.option(
     '--mode',
     type=click.Choice(['overwrite', 'append'], case_sensitive=False),
     help=f'Set mode to overwrite to remove already set tags, set append to keep them (default: {config.TAG_POSTS_DEFAULTS["mode"]}).',
 )
 @click.option(
     '--update-implications/--dont-update-implications',
     help=(
         'Fetches all tags from the posts matching the query and updates them if tag implications are missing (default:'
         f' {config.TAG_POSTS_DEFAULTS["update_implications"]}).'
     ),
 )
 @click.pass_context
-def click_tag_posts(ctx, query, add_tags, remove_tags, mode, update_implications):
+def click_tag_posts(ctx, query, add_tags, remove_tags, source, mode, update_implications):
     """
     Tag posts manually
 
     QUERY is a szurubooru query for posts to tag.
     """
 
-    if not add_tags and not remove_tags and not update_implications:
+    if not add_tags and not remove_tags and not source and not update_implications:
         print(ctx.get_help())
-        click.echo('\nYou need to specify either --add-tags, --remove-tags or --update-implications as an argument!')
+        click.echo('\nYou need to specify either --add-tags, --remove-tags, --source or --update-implications as an argument!')
         exit(1)
 
     module = setup_module('tag_posts', ctx)
 
     from loguru import logger
 
     for param in ctx.command.params:
@@ -563,15 +570,15 @@
     if add_tags:
         add_tags = add_tags.replace(' ', '').split(',')
         logger.debug(f'add_tags = {add_tags}')
     if remove_tags:
         remove_tags = remove_tags.replace(' ', '').split(',')
         logger.debug(f'remove_tags = {remove_tags}')
 
-    module.main(query, add_tags, remove_tags)
+    module.main(query, add_tags, remove_tags, source)
 
 
 @cli.command('upload-media', epilog='Example: szuru-toolkit upload-media --auto-tag --cleanup --tags "foo,bar"')
 @click.argument('src-path', required=False)
 @click.option('--auto-tag/--no-auto-tag', help=f'Tag posts automatically (default: {config.UPLOAD_MEDIA_DEFAULTS["auto_tag"]}).')
 @click.option(
     '--cleanup/--no-cleanup',
```

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/tag_posts.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/tag_posts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from loguru import logger
 from tqdm import tqdm
 
 from szurubooru_toolkit import config
 from szurubooru_toolkit import szuru
+from szurubooru_toolkit.utils import collect_sources
 
 
 @logger.catch
-def main(query: str, add_tags: list = [], remove_tags: list = []) -> None:
+def main(query: str, add_tags: list = [], remove_tags: list = [], source: str = '') -> None:
     """
     Retrieve the posts from input query, set post.tags based on mode and update them in szurubooru.
 
     Args:
         query (str): The query to use for retrieving posts.
         add_tags (list, optional): A list of tags to add to the posts. Defaults to [].
         remove_tags (list, optional): A list of tags to remove from the posts. Defaults to [].
+        source (str, optional): The source of the posts. Defaults to ''.
 
     Returns:
         None
     """
 
     try:
         try:
@@ -30,33 +32,39 @@
         logger.debug(f'update_implications = {str(update_implications)}')
 
         posts = szuru.get_posts(query, videos=True)
 
         try:
             total_posts = next(posts)
         except StopIteration:
-            logger.info(f'Found no posts for your query: {query}')
+            if not config.tag_posts['silence_info']:
+                logger.info(f'Found no posts for your query: {query}')
             exit()
 
-        logger.info(f'Found {total_posts} posts. Start tagging...')
+        if not config.tag_posts['silence_info']:
+            logger.info(f'Found {total_posts} posts. Start tagging...')
 
         for post in tqdm(
             posts,
             ncols=80,
             position=0,
             leave=False,
             total=int(total_posts),
             disable=hide_progress,
         ):
             if mode == 'append':
                 if add_tags:
                     post.tags = list(set().union(post.tags, add_tags))
+                if source:
+                    post.source = collect_sources(post.source, source)
             elif mode == 'overwrite':
                 if add_tags:
                     post.tags = add_tags
+                if source:
+                    post.source = source
 
             if remove_tags:
                 post.tags = [tag for tag in post.tags if tag not in remove_tags]
 
             if update_implications:
                 for tag in post.tags:
                     szuru_tag = szuru.api.getTag(tag)
```

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/scripts/upload_media.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/scripts/upload_media.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import requests
 from loguru import logger
 from tqdm import tqdm
 
 from szurubooru_toolkit import config
 from szurubooru_toolkit import szuru
 from szurubooru_toolkit.scripts import auto_tagger
+from szurubooru_toolkit.scripts import tag_posts
 from szurubooru_toolkit.szurubooru import Post
 from szurubooru_toolkit.szurubooru import Szurubooru
 from szurubooru_toolkit.utils import get_md5sum
 from szurubooru_toolkit.utils import shrink_img
 
 
 def get_files(upload_dir: str) -> list:
@@ -189,15 +190,15 @@
                 shutil.rmtree(os.path.join(root, name))
             try:
                 os.rmdir(os.path.join(root, name))
             except OSError:
                 pass
 
 
-def eval_convert_image(file: bytes, file_ext: str, file_to_upload: str = None) -> tuple(bytes | str):
+def eval_convert_image(file: bytes, file_ext: str, file_to_upload: str = None) -> tuple[bytes | str]:
     """
     Evaluate if the image should be converted or shrunk and if so, do so.
 
     This function checks if the image file should be converted to a different format or shrunk based on the global
     configuration settings. If the image is a PNG and its size is greater than the conversion threshold, it will be
     converted to a JPG. If the 'shrink' setting is enabled, the image will also be shrunk.
 
@@ -330,14 +331,31 @@
             saucenao_limit_reached = auto_tagger.main(
                 post_id=str(post_id),
                 file_to_upload=post.media,
                 limit_reached=saucenao_limit_reached,
                 md5=original_md5,
             )
 
+    else:
+        logger.debug('File is already uploaded')
+        if config.import_from_url['update_tags_if_exists'] and metadata:
+            logger.debug(f'Trying to update tags for post {post.exact_post["id"]}...')
+
+            id = str(post.exact_post['id']) if 'id' in post.exact_post else str(post.exact_post['post']['id'])
+            config.tag_posts['mode'] = 'append'
+
+            try:
+                if not metadata['tags'] and metadata['tag_string']:
+                    metadata['tags'] = metadata['tag_string'].split(' ')
+            except KeyError:
+                pass
+
+            config.tag_posts['silence_info'] = True
+            tag_posts.main(query=id, add_tags=metadata['tags'], source=metadata['source'])
+
     return True, saucenao_limit_reached
 
 
 def main(
     src_path: str = '',
     file_to_upload: bytes = None,
     file_ext: str = None,
```

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/szurubooru.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/szurubooru.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
             query_url = self.szuru_api_url + '/posts/?' + urllib.parse.urlencode(query_params)
             logger.debug(f'Getting post from query_url: {query_url}')
 
             response_json = requests.get(query_url, headers=self.headers)
             response = response_json.json()
             # logger.debug(f'Got following response: {response}')
 
-            if 'name' in response and response['name'] in ['SearchError', 'UserNotFoundError']:
+            if 'name' in response and 'Error' in response['name']:
                 logger.critical(f'{response["name"]}: {response["description"]}')
                 raise UnknownTokenError(response['description'])
 
             total = str(response['total'])
             logger.debug(f'Got a total of {total} results')
 
             results = response['results']
```

### Comparing `szurubooru_toolkit-1.0.0/src/szurubooru_toolkit/utils.py` & `szurubooru_toolkit-1.0.1/src/szurubooru_toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-1.0.0/PKG-INFO` & `szurubooru_toolkit-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: szurubooru-toolkit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python package and script collection to manage szurubooru.
 Home-page: https://github.com/reluce/szurubooru-toolkit
 License: GPL-3.0-only
 Keywords: szurubooru,szuru,booru,saucenao,deepbooru
 Author: reluce
 Author-email: reluce@fkosquad.moe
 Requires-Python: >=3.11,<3.12
@@ -35,19 +35,50 @@
 <img src="https://cdn-icons-png.flaticon.com/512/2581/2581053.png"
   alt="szurubooru-toolkit icon"
   width="128" height="128">
 </p>
 
 # szurubooru-toolkit
 Python package and script collection to manage your [szurubooru](https://github.com/rr-/szurubooru) image board.
+```
+Usage: szuru-toolkit [OPTIONS] COMMAND [ARGS]...
 
+  Toolkit to manage your szurubooru image board.
+
+  Defaults can also be set in a config file.
+
+  Visit https://github.com/reluce/szurubooru-toolkit for more information.
+
+Options:
+  --url TEXT                      Base URL to your szurubooru instance.
+  --username TEXT                 Username which will be used to authenticate with the szurubooru API.
+  --api-token TEXT                API token for the user which will be used to authenticate with the szurubooru API.
+  --public                        If your szurubooru instance is reachable from the internet (default: False).
+  --log-enabled                   Create a log file (default: False).
+  --log-colorized                 Colorize the log output (default: True).
+  --log-file TEXT                 Output file for the log (default: szurubooru_toolkit.log)
+  --log-level [DEBUG|INFO|WARNING|ERROR|CRITICAL]
+                                  Set the log level (default: INFO).
+  --hide-progress                 Hides the progress bar (default: False).
+  -h, --help                      Show this message and exit.
+
+Commands:
+  auto-tagger        Tag posts automatically
+  create-relations   Create relations between character and parody tag categories
+  create-tags        Create tags based on a tag file or query
+  delete-posts       Delete posts
+  import-from-booru  Download and tag posts from various Boorus
+  import-from-url    Download images from URLS or file containing URLs
+  reset-posts        Remove tags and sources
+  tag-posts          Tag posts manually
+  upload-media       Upload media files
+```
 ## :ballot_box_with_check: Requirements
 In order to run `szuru-toolkit`, Python `3.11` is required.
 
-
 ## :hammer_and_wrench: Installation
 This package is available on [PyPI](https://pypi.org/project/szurubooru-toolkit/) and can be installed with pip:
 `pip install szurubooru-toolkit`
 
 Alternatively, you can clone the package from GitHub and set everything up with [Poetry](https://python-poetry.org/docs/). In the root directory of this repository, execute `poetry install`.
 
 ### Docker Instructions
```

