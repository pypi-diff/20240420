# Comparing `tmp/hfutils-0.1.0.tar.gz` & `tmp/hfutils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfutils-0.1.0.tar", last modified: Thu Apr 18 13:40:57 2024, max compression
+gzip compressed data, was "hfutils-0.1.1.tar", last modified: Sat Apr 20 10:03:06 2024, max compression
```

## Comparing `hfutils-0.1.0.tar` & `hfutils-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.140425 hfutils-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-18 13:40:35.000000 hfutils-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-18 13:40:35.000000 hfutils-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-18 13:40:57.140425 hfutils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-18 13:40:35.000000 hfutils-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.132424 hfutils-0.1.0/hfutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.132424 hfutils-0.1.0/hfutils/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/archive/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/archive/rar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/archive/sevenz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/archive/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/archive/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.132424 hfutils-0.1.0/hfutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.132424 hfutils-0.1.0/hfutils/entry/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/entry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/entry/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/entry/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/entry/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/entry/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.132424 hfutils-0.1.0/hfutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/operate/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/operate/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/operate/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/operate/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.136424 hfutils-0.1.0/hfutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/utils/temp.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/utils/tqdm_.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/utils/walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.136424 hfutils-0.1.0/hfutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-18 13:40:57.000000 hfutils-0.1.0/hfutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-18 13:40:57.000000 hfutils-0.1.0/hfutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:40:57.000000 hfutils-0.1.0/hfutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 13:40:57.000000 hfutils-0.1.0/hfutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-18 13:40:57.000000 hfutils-0.1.0/hfutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 13:40:57.000000 hfutils-0.1.0/hfutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements-7z.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements-rar.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements-transfer.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:40:57.140425 hfutils-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-18 13:40:35.000000 hfutils-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.239896 hfutils-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-20 10:02:44.000000 hfutils-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 10:02:44.000000 hfutils-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-20 10:03:06.239896 hfutils-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-20 10:02:44.000000 hfutils-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.231896 hfutils-0.1.1/hfutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.231896 hfutils-0.1.1/hfutils/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/archive/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/archive/rar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/archive/sevenz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/archive/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/archive/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.231896 hfutils-0.1.1/hfutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.231896 hfutils-0.1.1/hfutils/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/entry/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/entry/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/entry/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.231896 hfutils-0.1.1/hfutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/operate/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/operate/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/operate/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/operate/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.235896 hfutils-0.1.1/hfutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/utils/temp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/utils/tqdm_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/utils/walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.235896 hfutils-0.1.1/hfutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-20 10:03:06.000000 hfutils-0.1.1/hfutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-20 10:03:06.000000 hfutils-0.1.1/hfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 10:03:06.000000 hfutils-0.1.1/hfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-20 10:03:06.000000 hfutils-0.1.1/hfutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-20 10:03:06.000000 hfutils-0.1.1/hfutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 10:03:06.000000 hfutils-0.1.1/hfutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements-7z.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements-rar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements-transfer.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 10:03:06.239896 hfutils-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-20 10:02:45.000000 hfutils-0.1.1/setup.py
```

### Comparing `hfutils-0.1.0/LICENSE` & `hfutils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/PKG-INFO` & `hfutils-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfutils-0.1.0/README.md` & `hfutils-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/archive/__init__.py` & `hfutils-0.1.1/hfutils/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/archive/base.py` & `hfutils-0.1.1/hfutils/archive/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/archive/rar.py` & `hfutils-0.1.1/hfutils/archive/rar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/archive/sevenz.py` & `hfutils-0.1.1/hfutils/archive/sevenz.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/archive/tar.py` & `hfutils-0.1.1/hfutils/archive/tar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/archive/zip.py` & `hfutils-0.1.1/hfutils/archive/zip.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/entry/base.py` & `hfutils-0.1.1/hfutils/entry/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/entry/dispatch.py` & `hfutils-0.1.1/hfutils/entry/dispatch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/entry/download.py` & `hfutils-0.1.1/hfutils/entry/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/entry/upload.py` & `hfutils-0.1.1/hfutils/entry/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/operate/base.py` & `hfutils-0.1.1/hfutils/operate/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/operate/download.py` & `hfutils-0.1.1/hfutils/operate/download.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,33 +109,36 @@
     :param hf_token: Huggingface token for API client, use ``HF_TOKEN`` variable if not assigned.
     :type hf_token: str, optional
     """
     files = list_files_in_repository(repo_id, repo_type, dir_in_repo, revision, ignore_patterns)
     progress = tqdm(files, silent=silent, desc=f'Downloading {dir_in_repo!r} ...')
 
     def _download_one_file(rel_file):
-        dst_file = os.path.join(local_directory, rel_file)
-        if os.path.exists(dst_file) and is_local_file_ready(
-                repo_id=repo_id,
-                repo_type=repo_type,
-                local_file=dst_file,
-                file_in_repo=f'{dir_in_repo}/{rel_file}',
-                revision=revision,
-                hf_token=hf_token,
-        ):
-            logging.info(f'Local file {rel_file} is ready, download skipped.')
-        else:
-            download_file_to_file(
-                local_file=dst_file,
-                repo_id=repo_id,
-                file_in_repo=f'{dir_in_repo}/{rel_file}',
-                repo_type=repo_type,
-                revision=revision,
-                resume_download=resume_download,
-                hf_token=hf_token,
-            )
-        progress.update()
+        try:
+            dst_file = os.path.join(local_directory, rel_file)
+            if os.path.exists(dst_file) and is_local_file_ready(
+                    repo_id=repo_id,
+                    repo_type=repo_type,
+                    local_file=dst_file,
+                    file_in_repo=f'{dir_in_repo}/{rel_file}',
+                    revision=revision,
+                    hf_token=hf_token,
+            ):
+                logging.info(f'Local file {rel_file} is ready, download skipped.')
+            else:
+                download_file_to_file(
+                    local_file=dst_file,
+                    repo_id=repo_id,
+                    file_in_repo=f'{dir_in_repo}/{rel_file}',
+                    repo_type=repo_type,
+                    revision=revision,
+                    resume_download=resume_download,
+                    hf_token=hf_token,
+                )
+            progress.update()
+        except Exception as err:
+            logging.error(f'Unexpected error when downloading {rel_file!r} - {err!r}')
 
     tp = ThreadPoolExecutor(max_workers=max_workers)
     for file in files:
         tp.submit(_download_one_file, file)
     tp.shutdown(wait=True)
```

### Comparing `hfutils-0.1.0/hfutils/operate/upload.py` & `hfutils-0.1.1/hfutils/operate/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/operate/validate.py` & `hfutils-0.1.1/hfutils/operate/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/utils/binary.py` & `hfutils-0.1.1/hfutils/utils/binary.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/utils/download.py` & `hfutils-0.1.1/hfutils/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/utils/temp.py` & `hfutils-0.1.1/hfutils/utils/temp.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/utils/tqdm_.py` & `hfutils-0.1.1/hfutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils/utils/walk.py` & `hfutils-0.1.1/hfutils/utils/walk.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils.egg-info/PKG-INFO` & `hfutils-0.1.1/hfutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfutils-0.1.0/hfutils.egg-info/SOURCES.txt` & `hfutils-0.1.1/hfutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/hfutils.egg-info/requires.txt` & `hfutils-0.1.1/hfutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.0/setup.py` & `hfutils-0.1.1/setup.py`

 * *Files identical despite different names*

