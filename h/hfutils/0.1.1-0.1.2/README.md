# Comparing `tmp/hfutils-0.1.1.tar.gz` & `tmp/hfutils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfutils-0.1.1.tar", last modified: Sat Apr 20 10:03:06 2024, max compression
+gzip compressed data, was "hfutils-0.1.2.tar", last modified: Sat Apr 20 11:18:35 2024, max compression
```

## Comparing `hfutils-0.1.1.tar` & `hfutils-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.239896 hfutils-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-20 10:02:44.000000 hfutils-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 10:02:44.000000 hfutils-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-20 10:03:06.239896 hfutils-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-20 10:02:44.000000 hfutils-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.231896 hfutils-0.1.1/hfutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.231896 hfutils-0.1.1/hfutils/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/archive/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/archive/rar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/archive/sevenz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/archive/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/archive/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.231896 hfutils-0.1.1/hfutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.231896 hfutils-0.1.1/hfutils/entry/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/entry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/entry/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/entry/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/entry/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/entry/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.231896 hfutils-0.1.1/hfutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/operate/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/operate/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/operate/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/operate/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.235896 hfutils-0.1.1/hfutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/utils/temp.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/utils/tqdm_.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-20 10:02:45.000000 hfutils-0.1.1/hfutils/utils/walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:03:06.235896 hfutils-0.1.1/hfutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-20 10:03:06.000000 hfutils-0.1.1/hfutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-20 10:03:06.000000 hfutils-0.1.1/hfutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 10:03:06.000000 hfutils-0.1.1/hfutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-20 10:03:06.000000 hfutils-0.1.1/hfutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-20 10:03:06.000000 hfutils-0.1.1/hfutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 10:03:06.000000 hfutils-0.1.1/hfutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements-7z.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements-rar.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements-transfer.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-20 10:02:45.000000 hfutils-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 10:03:06.239896 hfutils-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-20 10:02:45.000000 hfutils-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.254774 hfutils-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-20 11:18:15.000000 hfutils-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 11:18:15.000000 hfutils-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-20 11:18:35.254774 hfutils-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-20 11:18:15.000000 hfutils-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.246775 hfutils-0.1.2/hfutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.246775 hfutils-0.1.2/hfutils/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/archive/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/archive/rar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/archive/sevenz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/archive/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/archive/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.246775 hfutils-0.1.2/hfutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.246775 hfutils-0.1.2/hfutils/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/entry/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/entry/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/entry/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.246775 hfutils-0.1.2/hfutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/operate/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/operate/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/operate/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/operate/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.246775 hfutils-0.1.2/hfutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/utils/temp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/utils/tqdm_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/utils/walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.250774 hfutils-0.1.2/hfutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-20 11:18:35.000000 hfutils-0.1.2/hfutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-20 11:18:35.000000 hfutils-0.1.2/hfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 11:18:35.000000 hfutils-0.1.2/hfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-20 11:18:35.000000 hfutils-0.1.2/hfutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-20 11:18:35.000000 hfutils-0.1.2/hfutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 11:18:35.000000 hfutils-0.1.2/hfutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements-7z.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements-rar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements-transfer.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 11:18:35.254774 hfutils-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-20 11:18:15.000000 hfutils-0.1.2/setup.py
```

### Comparing `hfutils-0.1.1/LICENSE` & `hfutils-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/PKG-INFO` & `hfutils-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfutils-0.1.1/README.md` & `hfutils-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/archive/__init__.py` & `hfutils-0.1.2/hfutils/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/archive/base.py` & `hfutils-0.1.2/hfutils/archive/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/archive/rar.py` & `hfutils-0.1.2/hfutils/archive/rar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/archive/sevenz.py` & `hfutils-0.1.2/hfutils/archive/sevenz.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/archive/tar.py` & `hfutils-0.1.2/hfutils/archive/tar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/archive/zip.py` & `hfutils-0.1.2/hfutils/archive/zip.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/entry/base.py` & `hfutils-0.1.2/hfutils/entry/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/entry/dispatch.py` & `hfutils-0.1.2/hfutils/entry/dispatch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/entry/download.py` & `hfutils-0.1.2/hfutils/entry/download.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import warnings
 from typing import Optional
 
 import click
 
 from .base import CONTEXT_SETTINGS, command_wrap, ClickErrorException
 from ..operate import download_file_to_file, download_archive_as_directory, download_directory_as_directory
@@ -42,18 +43,20 @@
                   help='Output path for download.')
     @click.option('-R', '--revision', 'revision', type=str, default='main',
                   help='Revision of repository.', show_default=True)
     @click.option('-n', '--max_workers', 'max_workers', type=int, default=8,
                   help='Max threads to download.', show_default=True)
     @click.option('-p', '--password', 'password', type=str, default=None,
                   help='Password for the archive file. Only applied when -a is used.', show_default=True)
+    @click.option('--tmpdir', 'tmpdir', type=str, default=None,
+                  help='Use custom temporary Directory.', show_default=True)
     @command_wrap()
     def download(repo_id: str, repo_type: RepoTypeTyping,
                  file_in_repo: Optional[str], archive_in_repo: Optional[str], dir_in_repo: Optional[str],
-                 output_path: str, revision: str, max_workers: int, password: Optional[str]):
+                 output_path: str, revision: str, max_workers: int, password: Optional[str], tmpdir: Optional[str]):
         """
         Download data from HuggingFace repositories.
 
         :param repo_id: Repository to download from.
         :type repo_id: str
         :param repo_type: Type of the HuggingFace repository.
         :type repo_type: RepoTypeTyping
@@ -67,15 +70,20 @@
         :type output_path: str
         :param revision: Revision of repository.
         :type revision: str
         :param max_workers: Max workers to download
         :type max_workers: int
         :param password: Password for the archive file. Only applied when -a is used.
         :type password: str, optional
+        :param tmpdir: Use custom temporary Directory.
+        :type tmpdir: str, optional
         """
+        if tmpdir:
+            os.environ['TMPDIR'] = tmpdir
+
         if not file_in_repo and not archive_in_repo and not dir_in_repo:
             raise NoRemotePathAssignedWithDownload('No remote path in repository assigned.\n'
                                                    'One of the -f, -a, or -d option is required.')
 
         if file_in_repo:
             if archive_in_repo:
                 warnings.warn('File in repository assigned, value of -a option will be ignored.')
```

### Comparing `hfutils-0.1.1/hfutils/entry/upload.py` & `hfutils-0.1.2/hfutils/entry/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/operate/base.py` & `hfutils-0.1.2/hfutils/operate/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/operate/download.py` & `hfutils-0.1.2/hfutils/operate/download.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import os.path
 import shutil
 from concurrent.futures import ThreadPoolExecutor
 from typing import List, Optional
 
+import requests.exceptions
+
 from .base import RepoTypeTyping, list_files_in_repository, _IGNORE_PATTERN_UNSET, get_hf_client
 from .validate import is_local_file_ready
 from ..archive import archive_unpack
 from ..utils import tqdm, TemporaryDirectory
 
 
 def download_file_to_file(local_file: str, repo_id: str, file_in_repo: str,
@@ -79,15 +81,15 @@
         download_file_to_file(archive_file, repo_id, file_in_repo, repo_type, revision, hf_token=hf_token)
         archive_unpack(archive_file, local_directory, password=password)
 
 
 def download_directory_as_directory(local_directory: str, repo_id: str, dir_in_repo: str = '.',
                                     repo_type: RepoTypeTyping = 'dataset', revision: str = 'main',
                                     silent: bool = False, ignore_patterns: List[str] = _IGNORE_PATTERN_UNSET,
-                                    resume_download: bool = True, max_workers: int = 8,
+                                    resume_download: bool = True, max_workers: int = 8, max_retries: int = 5,
                                     hf_token: Optional[str] = None):
     """
     Download all files in a directory from a Hugging Face repository to a local directory.
 
     :param local_directory: The local directory path to save the downloaded files.
     :type local_directory: str
     :param repo_id: The identifier of the repository.
@@ -100,44 +102,60 @@
     :type revision: str
     :param silent: If True, suppress progress bar output.
     :type silent: bool
     :param ignore_patterns: List of file patterns to ignore.
     :type ignore_patterns: List[str]
     :param max_workers: Max workers when downloading. Default is ``8``.
     :type max_workers: int
+    :param max_retries: Max retry times when downloading. Default is ``5``.
+    :type max_retries: int
     :param resume_download: Resume the existing download.
     :type resume_download: bool
     :param hf_token: Huggingface token for API client, use ``HF_TOKEN`` variable if not assigned.
     :type hf_token: str, optional
     """
-    files = list_files_in_repository(repo_id, repo_type, dir_in_repo, revision, ignore_patterns)
+    files = list_files_in_repository(repo_id, repo_type, dir_in_repo, revision, ignore_patterns, hf_token=hf_token)
     progress = tqdm(files, silent=silent, desc=f'Downloading {dir_in_repo!r} ...')
 
     def _download_one_file(rel_file):
+        current_resume_download = resume_download
         try:
             dst_file = os.path.join(local_directory, rel_file)
             if os.path.exists(dst_file) and is_local_file_ready(
                     repo_id=repo_id,
                     repo_type=repo_type,
                     local_file=dst_file,
                     file_in_repo=f'{dir_in_repo}/{rel_file}',
                     revision=revision,
                     hf_token=hf_token,
             ):
                 logging.info(f'Local file {rel_file} is ready, download skipped.')
             else:
-                download_file_to_file(
-                    local_file=dst_file,
-                    repo_id=repo_id,
-                    file_in_repo=f'{dir_in_repo}/{rel_file}',
-                    repo_type=repo_type,
-                    revision=revision,
-                    resume_download=resume_download,
-                    hf_token=hf_token,
-                )
+                tries = 0
+                while True:
+                    try:
+                        download_file_to_file(
+                            local_file=dst_file,
+                            repo_id=repo_id,
+                            file_in_repo=f'{dir_in_repo}/{rel_file}',
+                            repo_type=repo_type,
+                            revision=revision,
+                            resume_download=current_resume_download,
+                            hf_token=hf_token,
+                        )
+                    except requests.exceptions.RequestException as err:
+                        if tries < max_retries:
+                            tries += 1
+                            logging.warning(f'Download {rel_file!r} failed, retry ({tries}/{max_retries}) - {err!r}.')
+                            current_resume_download = True
+                        else:
+                            raise
+                    else:
+                        break
+
             progress.update()
         except Exception as err:
             logging.error(f'Unexpected error when downloading {rel_file!r} - {err!r}')
 
     tp = ThreadPoolExecutor(max_workers=max_workers)
     for file in files:
         tp.submit(_download_one_file, file)
```

### Comparing `hfutils-0.1.1/hfutils/operate/upload.py` & `hfutils-0.1.2/hfutils/operate/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     :param hf_token: Huggingface token for API client, use ``HF_TOKEN`` variable if not assigned.
     :type hf_token: str, optional
     """
     hf_client = get_hf_client(hf_token)
     if clear:
         pre_exist_files = {
             tuple(file.split('/')) for file in
-            list_files_in_repository(repo_id, repo_type, path_in_repo, revision, ignore_patterns)
+            list_files_in_repository(repo_id, repo_type, path_in_repo, revision, ignore_patterns, hf_token=hf_token)
         }
     else:
         pre_exist_files = set()
 
     operations = []
     for file in walk_files(local_directory):
         segments = tuple(seg for seg in _PATH_SEP.split(file) if seg)
```

### Comparing `hfutils-0.1.1/hfutils/operate/validate.py` & `hfutils-0.1.2/hfutils/operate/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/utils/binary.py` & `hfutils-0.1.2/hfutils/utils/binary.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/utils/download.py` & `hfutils-0.1.2/hfutils/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/utils/temp.py` & `hfutils-0.1.2/hfutils/utils/temp.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/utils/tqdm_.py` & `hfutils-0.1.2/hfutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils/utils/walk.py` & `hfutils-0.1.2/hfutils/utils/walk.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils.egg-info/PKG-INFO` & `hfutils-0.1.2/hfutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfutils-0.1.1/hfutils.egg-info/SOURCES.txt` & `hfutils-0.1.2/hfutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/hfutils.egg-info/requires.txt` & `hfutils-0.1.2/hfutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.1/setup.py` & `hfutils-0.1.2/setup.py`

 * *Files identical despite different names*

