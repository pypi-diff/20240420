# Comparing `tmp/trackhub-0.2.4.tar.gz` & `tmp/trackhub-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trackhub-0.2.4.tar", last modified: Thu Dec 21 15:53:28 2017, max compression
+gzip compressed data, was "trackhub-1.0.tar", last modified: Sat Apr 20 18:07:13 2024, max compression
```

## Comparing `trackhub-0.2.4.tar` & `trackhub-1.0.tar`

### file list

```diff
@@ -1,55 +1,64 @@
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-12-21 15:53:28.000000 trackhub-0.2.4/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       48 2017-09-20 20:59:18.000000 trackhub-0.2.4/MANIFEST.in
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-12-21 15:53:28.000000 trackhub-0.2.4/trackhub/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      556 2017-09-20 20:59:18.000000 trackhub-0.2.4/trackhub/compatibility.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5439 2017-12-20 23:03:28.000000 trackhub-0.2.4/trackhub/upload.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     7066 2017-12-20 23:07:34.000000 trackhub-0.2.4/trackhub/assembly.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3872 2017-12-20 23:07:34.000000 trackhub-0.2.4/trackhub/groups.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2090 2017-12-20 23:07:34.000000 trackhub-0.2.4/trackhub/genomes_file.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2126 2017-12-20 23:07:34.000000 trackhub-0.2.4/trackhub/genome.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    19827 2017-12-20 23:07:34.000000 trackhub-0.2.4/trackhub/constants.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     4378 2017-12-20 23:07:34.000000 trackhub-0.2.4/trackhub/base.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     4665 2017-12-20 23:03:28.000000 trackhub-0.2.4/trackhub/validate.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1515 2017-12-21 13:58:59.000000 trackhub-0.2.4/trackhub/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       16 2017-12-21 15:49:31.000000 trackhub-0.2.4/trackhub/version.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3121 2017-12-21 13:58:59.000000 trackhub-0.2.4/trackhub/trackdb.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-12-21 15:53:28.000000 trackhub-0.2.4/trackhub/test/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1358 2017-12-21 13:58:59.000000 trackhub-0.2.4/trackhub/test/test_example_data.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2503 2017-12-20 23:03:28.000000 trackhub-0.2.4/trackhub/test/upload_test.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-12-21 15:53:28.000000 trackhub-0.2.4/trackhub/test/data/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    19621 2017-12-20 23:35:40.000000 trackhub-0.2.4/trackhub/test/data/sine-no1-1000.bedgraph.bw
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    38999 2017-12-20 23:35:40.000000 trackhub-0.2.4/trackhub/test/data/random-no1-1.bigBed
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    13168 2017-12-20 23:35:39.000000 trackhub-0.2.4/trackhub/test/data/random-hg38-2.bigBed
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      142 2017-12-20 23:21:15.000000 trackhub-0.2.4/trackhub/test/data/__init__.pyc
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    36981 2017-12-20 23:35:40.000000 trackhub-0.2.4/trackhub/test/data/random-no1-2.bigBed
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    39319 2017-12-20 23:35:39.000000 trackhub-0.2.4/trackhub/test/data/sine-hg38-0.bedgraph.bw
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    13150 2017-12-20 23:35:39.000000 trackhub-0.2.4/trackhub/test/data/random-hg38-1.bigBed
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    45017 2017-12-20 23:35:40.000000 trackhub-0.2.4/trackhub/test/data/random-no1-0.bigBed
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    13160 2017-12-20 23:35:39.000000 trackhub-0.2.4/trackhub/test/data/random-hg38-0.bigBed
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    19618 2017-12-20 23:35:40.000000 trackhub-0.2.4/trackhub/test/data/sine-no1-100.bedgraph.bw
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2017-09-20 20:59:18.000000 trackhub-0.2.4/trackhub/test/data/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    55161 2017-12-21 13:59:03.000000 trackhub-0.2.4/trackhub/test/data/newOrg1.2bit
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    39311 2017-12-20 23:35:39.000000 trackhub-0.2.4/trackhub/test/data/sine-hg38-1.bedgraph.bw
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    39296 2017-12-20 23:35:39.000000 trackhub-0.2.4/trackhub/test/data/sine-hg38-2.bedgraph.bw
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     4321 2017-12-20 23:03:28.000000 trackhub-0.2.4/trackhub/test/test_components.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1670 2017-12-20 23:03:28.000000 trackhub-0.2.4/trackhub/test/construct_example_data.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1927 2017-12-20 23:03:28.000000 trackhub-0.2.4/trackhub/test/construct_example_genome.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2017-12-20 23:03:28.000000 trackhub-0.2.4/trackhub/test/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2417 2017-12-20 23:03:28.000000 trackhub-0.2.4/trackhub/test/deprecated_upload_test.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1047 2017-12-20 23:03:28.000000 trackhub-0.2.4/trackhub/test/test_assembly.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     4860 2017-12-20 23:07:34.000000 trackhub-0.2.4/trackhub/helpers.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    25104 2017-12-21 13:58:59.000000 trackhub-0.2.4/trackhub/track.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3295 2017-12-20 23:07:34.000000 trackhub-0.2.4/trackhub/hub.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        9 2017-12-20 22:35:28.000000 trackhub-0.2.4/requirements.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      130 2017-12-20 20:31:57.000000 trackhub-0.2.4/test-requirements.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1076 2017-09-20 20:59:18.000000 trackhub-0.2.4/LICENSE.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1291 2017-12-21 15:48:58.000000 trackhub-0.2.4/setup.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      761 2017-12-21 15:53:28.000000 trackhub-0.2.4/PKG-INFO
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2017-12-21 15:53:28.000000 trackhub-0.2.4/trackhub.egg-info/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2017-12-21 15:53:28.000000 trackhub-0.2.4/trackhub.egg-info/dependency_links.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        9 2017-12-21 15:53:28.000000 trackhub-0.2.4/trackhub.egg-info/top_level.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        9 2017-12-21 15:53:28.000000 trackhub-0.2.4/trackhub.egg-info/requires.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      761 2017-12-21 15:53:28.000000 trackhub-0.2.4/trackhub.egg-info/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1371 2017-12-21 15:53:28.000000 trackhub-0.2.4/trackhub.egg-info/SOURCES.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     6572 2017-12-21 13:58:59.000000 trackhub-0.2.4/README.rst
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       59 2017-12-21 15:53:28.000000 trackhub-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:13.821732 trackhub-1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-20 18:07:08.000000 trackhub-1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 18:07:08.000000 trackhub-1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-20 18:07:13.821732 trackhub-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-20 18:07:08.000000 trackhub-1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-20 18:07:08.000000 trackhub-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 18:07:08.000000 trackhub-1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:07:13.821732 trackhub-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-20 18:07:08.000000 trackhub-1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-20 18:07:08.000000 trackhub-1.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:13.817732 trackhub-1.0/trackhub/
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/genomes_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38438 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/parsed_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:13.817732 trackhub-1.0/trackhub/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/construct_example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/construct_example_genome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:13.821732 trackhub-1.0/trackhub/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/download_ucsc_examples.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    16736 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/example.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    55161 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/newOrg1.2bit
+-rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/random-hg38-0.bigBed
+-rw-r--r--   0 runner    (1001) docker     (127)    13150 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/random-hg38-1.bigBed
+-rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/random-hg38-2.bigBed
+-rw-r--r--   0 runner    (1001) docker     (127)    45017 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/random-no1-0.bigBed
+-rw-r--r--   0 runner    (1001) docker     (127)    38999 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/random-no1-1.bigBed
+-rw-r--r--   0 runner    (1001) docker     (127)    36981 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/random-no1-2.bigBed
+-rw-r--r--   0 runner    (1001) docker     (127)    39319 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/sine-hg38-0.bedgraph.bw
+-rw-r--r--   0 runner    (1001) docker     (127)    39311 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/sine-hg38-1.bedgraph.bw
+-rw-r--r--   0 runner    (1001) docker     (127)    39296 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/sine-hg38-2.bedgraph.bw
+-rw-r--r--   0 runner    (1001) docker     (127)    19618 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/sine-no1-100.bedgraph.bw
+-rw-r--r--   0 runner    (1001) docker     (127)    19621 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/data/sine-no1-1000.bedgraph.bw
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/deprecated_upload_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/test_add_tracks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/test_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/test_example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/test_supertrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/test/upload_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28254 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/trackdb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21982 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/trackhub_from_excel
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 18:07:08.000000 trackhub-1.0/trackhub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:13.821732 trackhub-1.0/trackhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-20 18:07:13.000000 trackhub-1.0/trackhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-20 18:07:13.000000 trackhub-1.0/trackhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:07:13.000000 trackhub-1.0/trackhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 18:07:13.000000 trackhub-1.0/trackhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 18:07:13.000000 trackhub-1.0/trackhub.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `trackhub-0.2.4/trackhub/upload.py` & `trackhub-1.0/trackhub/upload.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,35 @@
 import shlex
 import subprocess as sp
 import logging
 from . import track
 from . import genome
 from . import base
 from . import trackdb
+from . import compatibility
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
-RSYNC_OPTIONS = '--progress -rvL'
+RSYNC_OPTIONS = "--progress -rvL"
 
 
 def run(cmds, **kwargs):
     """
     Wrapper around subprocess.run, with unicode decoding of output.
 
     Additional kwargs are passed to subprocess.run.
     """
-    proc = sp.Popen(cmds, bufsize=-1, stdout=sp.PIPE, stderr=sp.STDOUT,
-                    close_fds=sys.platform != 'win32')
+    proc = sp.Popen(
+        cmds,
+        bufsize=-1,
+        stdout=sp.PIPE,
+        stderr=sp.STDOUT,
+        close_fds=sys.platform != "win32",
+    )
     for line in proc.stdout:
         print(line[:-1].decode())
     retcode = proc.wait()
     if retcode:
         raise sp.CalledProcessError(retcode, cmds)
 
 
@@ -35,22 +41,42 @@
     Create a symlink to `target` called `linkname`.
 
     Converts `target` and `linkname` to absolute paths; creates
     `dirname(linkname)` if needed.
     """
     target = os.path.abspath(target)
     linkname = os.path.abspath(linkname)
+
     if not os.path.exists(target):
         raise ValueError("target {} not found".format(target))
 
     link_dir = os.path.dirname(linkname)
     if not os.path.exists(link_dir):
         os.makedirs(link_dir)
 
-    run(['ln', '-s', '-f', target, linkname])
+    if os.path.exists(linkname):
+        if os.path.islink(linkname):
+            os.remove(linkname)
+
+    os.symlink(target, linkname)
+
+    # If possible, we modify the symlink's mtime to be that of the target.
+    mtime = os.stat(target).st_mtime
+
+    # Python 2.7 does not support modifying symlink modification time
+    if compatibility.PY == 3:
+        try:
+            os.utime(target, (mtime, mtime), follow_symlinks=False)
+
+        # In some cases (the reason is still unclear), in Python 3 we can still
+        # get a PermissionError. That's still OK, and we'll handle it as if it
+        # were Py27, that is, leave the symlink itself unchanged.
+        except (NotImplementedError, PermissionError):
+            pass
+
     return linkname
 
 
 def upload(host, user, local_dir, remote_dir, rsync_options=RSYNC_OPTIONS):
     """
     Upload a file or directory via rsync.
 
@@ -68,27 +94,27 @@
     remote_dir : str
         If a directory, a trailing "/" will be added.
     """
     if user is None:
         user = ""
     else:
         user = user + "@"
-    if host is None or host == 'localhost':
+    if host is None or host == "localhost":
         host = ""
     else:
         host = host + ":"
 
-    if not local_dir.endswith('/'):
-        local_dir = local_dir + '/'
+    if not local_dir.endswith("/"):
+        local_dir = local_dir + "/"
 
-    if not remote_dir.endswith('/'):
-        remote_dir = remote_dir + '/'
+    if not remote_dir.endswith("/"):
+        remote_dir = remote_dir + "/"
 
-    remote_string = '{user}{host}{remote_dir}'.format(**locals())
-    cmds = ['rsync']
+    remote_string = "{user}{host}{remote_dir}".format(**locals())
+    cmds = ["rsync"]
     cmds += shlex.split(rsync_options)
     cmds += [local_dir, remote_string]
     run(cmds)
     return [remote_string]
 
 
 def local_link(local_fn, remote_fn, staging):
@@ -142,62 +168,68 @@
         return linknames
 
     # If it's an object representing a file, then render it.
     #
     # Track objects don't represent files, but their documentation does
     linknames.append(x.render(staging))
 
-    if hasattr(x, 'source') and hasattr(x, 'filename'):
-        def _stg(x, ext=''):
+    if hasattr(x, "source") and hasattr(x, "filename"):
+
+        def _stg(x, ext=""):
             # A remote track hosted elsewhere does not need staging. This is
             # defined by a track with a url, but no source or filename.
             if (
                 x.source is None
                 and x.filename is None
-                and getattr(x, 'url', None) is not None
+                and getattr(x, "url", None) is not None
             ):
                 return
 
-            linknames.append(
-                local_link(x.source + ext, x.filename + ext, staging)
-            )
+            linknames.append(local_link(x.source + ext, x.filename + ext, staging))
 
         _stg(x)
 
         if isinstance(x, track.Track):
-            if x.tracktype == 'bam':
-                _stg(x, ext='.bai')
-            if x.tracktype == 'vcfTabix':
-                _stg(x, ext='.tbi')
+            if x.tracktype == "bam":
+                _stg(x, ext=".bai")
+            if x.tracktype == "vcfTabix":
+                _stg(x, ext=".tbi")
 
         if isinstance(x, track.CompositeTrack):
             if x._html:
                 _stg(x._html)
 
     return linknames
 
 
-
 def stage_hub(hub, staging=None):
     """
     Stage a hub by symlinking all its connected files to a local directory.
     """
     linknames = []
     if staging is None:
         staging = tempfile.mkdtemp()
     for obj, level in hub.leaves(base.HubComponent, intermediate=True):
         linknames.extend(stage(obj, staging))
 
     return staging, linknames
 
 
-def upload_hub(hub, host, remote_dir, user=None, port=22, rsync_options=RSYNC_OPTIONS, staging=None):
+def upload_hub(
+    hub, host, remote_dir, user=None, port=22, rsync_options=RSYNC_OPTIONS, staging=None
+):
     """
     Renders, stages, and uploads a hub.
     """
     hub.render()
     if staging is None:
         staging = tempfile.mkdtemp()
     staging, linknames = stage_hub(hub, staging=staging)
     local_dir = os.path.join(staging)
-    upload(host, user, local_dir=local_dir, remote_dir=remote_dir, rsync_options=rsync_options)
+    upload(
+        host,
+        user,
+        local_dir=local_dir,
+        remote_dir=remote_dir,
+        rsync_options=rsync_options,
+    )
     return linknames
```

### Comparing `trackhub-0.2.4/trackhub/assembly.py` & `trackhub-1.0/trackhub/assembly.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from collections import OrderedDict
 from .validate import ValidationError
 from .base import HubComponent, deprecation_handler
 from .genome import Genome
 from .genomes_file import GenomesFile
 from .groups import GroupsFile
 from .trackdb import TrackDb
-from .constants import assembly_fields
-from .track import HTMLDoc
+from . import constants
+from .track import HTMLDoc, ParameterError
 
 
 class TwoBitFile(HubComponent):
     def __init__(self, source, filename=None, assembly_obj=None, **kwargs):
         source, filename = deprecation_handler(source, filename, kwargs)
         HubComponent.__init__(self)
         self.source = source
@@ -49,42 +49,41 @@
         if not self.assembly:
             return None
         if not self.assembly.genomes_file:
             return None
         return os.path.join(
             os.path.dirname(self.assembly.genomes_file.filename),
             self.assembly.genome,
-            self.assembly.genome + '.2bit')
+            self.assembly.genome + ".2bit",
+        )
 
     def validate(self):
         if not os.path.exists(self.source):
             raise ValueError("Local filename {0} does not exist".format(self.source))
 
     @filename.setter
     def filename(self, fn):
         self._filename = fn
 
-    def _render(self, staging='staging'):
+    def _render(self, staging="staging"):
         pass
 
 
 class Assembly(Genome):
-
-    params = OrderedDict()
-    params.update(assembly_fields)
-
-    def __init__(self,
-                 genome,
-                 twobit_file=None,
-                 groups=None,
-                 trackdb=None,
-                 genome_file_obj=None,
-                 html_string=None,
-                 html_string_format='rst',
-                 **kwargs):
+    def __init__(
+        self,
+        genome,
+        twobit_file=None,
+        groups=None,
+        trackdb=None,
+        genome_file_obj=None,
+        html_string=None,
+        html_string_format="rst",
+        **kwargs
+    ):
         """
         Represents a genome stanza within a "genomes.txt" file for a non-UCSC genome.
 
         The file itself is represented by a :class:`GenomesFile` object.
 
         Parameters
         ----------
@@ -105,14 +104,18 @@
         if groups is not None:
             self.add_groups(groups)
         else:
             self.groups = None
 
         self._orig_kwargs = kwargs
 
+        self.track_field_order = []
+        self.track_field_order.extend(constants.track_fields["assembly"])
+        self.track_field_order.extend(constants.track_fields["all"])
+
         self.add_params(**kwargs)
 
     def add_twobit(self, twobit):
         self.children = [x for x in self.children if not isinstance(x, TwoBitFile)]
         self.add_child(twobit)
         self.twobit = twobit
 
@@ -139,19 +142,21 @@
         """
         Add [possibly many] parameters to the Assembly.
 
         Parameters will be checked against known UCSC parameters and their
         supported formats.
         """
         for k, v in kw.items():
-            if k not in self.params:
-                raise ValidationError(
-                    '"%s" is not a valid parameter for %s'
-                    % (k, self.__class__.__name__))
-            self.params[k].validate(v)
+            if k not in self.track_field_order:
+                raise ParameterError(
+                    '"{0}" is not a valid parameter for {1}'.format(
+                        k, self.__class__.__name__
+                    )
+                )
+            constants.param_dict[k].validate(v)
 
         self._orig_kwargs.update(kw)
         self.kwargs = self._orig_kwargs.copy()
 
     def remove_params(self, *args):
         """
         Remove [possibly many] parameters from the Assembly.
@@ -176,31 +181,31 @@
         try:
             self.validate()
         except ValidationError:
             return "Unconfigured <Assembly> object"
 
         s = []
 
-        s.append('genome %s' % self.genome)
-        s.append('trackDb %s' % self.trackdb.filename)
-        s.append('twoBitPath %s' % self.twobit.filename)
+        s.append("genome %s" % self.genome)
+        s.append("trackDb %s" % self.trackdb.filename)
+        s.append("twoBitPath %s" % self.twobit.filename)
         if self.groups is not None:
-            s.append('groups %s' % self.groups.filename)
+            s.append("groups %s" % self.groups.filename)
 
-        for name, parameter_obj in self.params.items():
+        for name in self.track_field_order:
             value = self.kwargs.pop(name, None)
             if value is not None:
-                if parameter_obj.validate(value):
+                if constants.param_dict[name].validate(value):
                     s.append("%s %s" % (name, value))
 
         if self._html is not None:
-            s.append('htmlDocumentation %s' % self._html.filename)
+            s.append("htmlDocumentation %s" % self._html.filename)
 
         self.kwargs = self._orig_kwargs.copy()
-        return '\n'.join(s) + '\n'
+        return "\n".join(s) + "\n"
 
     def validate(self):
         Genome.validate(self)
         # check for necessary params?
 
 
 class AssemblyHTMLDoc(HTMLDoc):
@@ -208,15 +213,16 @@
     @property
     def filename(self):
         if (self.genomes_file is None) or (self.genome is None):
             return None
         return os.path.join(
             os.path.dirname(self.genomes_file.filename),
             self.genome.genome,
-            '%s_info.html' % self.genome.genome)
+            "%s_info.html" % self.genome.genome,
+        )
 
     @property
     def genomes_file(self):
         obj, level = self.root(cls=GenomesFile)
         if level is None:
             return None
         if level != -2:
@@ -230,10 +236,11 @@
             return None
         if level != -1:
             raise ValueError("Assembly is level %s, not -1" % level)
         return obj
 
     def validate(self):
         if not self.genome:
-            raise ValueError("HTMLDoc object must be connected to an"
-                             "Assembly subclass instance")
+            raise ValueError(
+                "HTMLDoc object must be connected to an" "Assembly subclass instance"
+            )
         return True
```

### Comparing `trackhub-0.2.4/trackhub/groups.py` & `trackhub-1.0/trackhub/groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from .validate import ValidationError
 from .base import HubComponent
 from .genome import Genome
 from .genomes_file import GenomesFile
 
 
 class GroupDefinition(object):
-
     def __init__(self, name, label=None, priority=1, default_is_closed=0):
         """
         Represents a group of tracks in a trackhub.
 
         Instances of this class are provided to an assembly.
 
         Parameters
@@ -24,34 +23,35 @@
         label : str
             The label that will be displayed (e.g., "Mapping")
 
         priority : int
             Orders this track group with the other track groups
 
         default_is_closed : 0 | 1
-            Determines if this track group is expanded or closed by default. Values to use are 0 or 1
+            Determines if this track group is expanded or closed by default.
+            Values to use are 0 or 1
         """
         self.name = str(name)
         if label is None:
             label = name
         self.label = str(label)
         self.priority = int(priority)
         if default_is_closed in (0, 1):
             self.default_is_closed = default_is_closed
         else:
             raise ValueError("default_is_closed must be 1 or 0")
 
     def __str__(self):
         s = [
-            'name %s' % self.name,
-            'label %s' % self.label,
-            'priority %s' % self.priority,
-            'defaultIsClosed %d' % self.default_is_closed
+            "name %s" % self.name,
+            "label %s" % self.label,
+            "priority %s" % self.priority,
+            "defaultIsClosed %d" % self.default_is_closed,
         ]
-        return '\n'.join(s) + '\n'
+        return "\n".join(s) + "\n"
 
 
 class GroupsFile(HubComponent):
     def __init__(self, groups, filename=None):
         """
         Represents the groups file on disk, used for assembly hubs.
 
@@ -80,15 +80,15 @@
         """
         self.groups.extend(groups)
 
     def __str__(self):
         """
         Render groups.txt file.
         """
-        return '\n'.join(g.__str__() for g in self.groups)
+        return "\n".join(g.__str__() for g in self.groups)
 
     @property
     def genomes_file(self):
         genomes_file, level = self.root(GenomesFile)
         if level is None:
             return None
         if level != -2:
@@ -97,44 +97,50 @@
 
     @property
     def genome(self):
         genome, level = self.root(Genome)
         if level is None:
             return None
         if level != -1:
-            raise ValueError('Genome is level %s, not -1' % level)
+            raise ValueError("Genome is level %s, not -1" % level)
         return genome
 
     @property
     def filename(self):
         if self._filename is not None:
             return self._filename
 
         if self.genome is None:
             return None
 
         if self.genomes_file is None:
             return None
 
         else:
-            return os.path.join(os.path.dirname(self.genomes_file.filename),
-                                self.genome.genome, 'groups.txt')
+            return os.path.join(
+                os.path.dirname(self.genomes_file.filename),
+                self.genome.genome,
+                "groups.txt",
+            )
 
     @filename.setter
     def filename(self, fn):
         self._filename = fn
 
     def validate(self):
         if self.genome is None:
-            raise ValidationError("GroupsFile object must be attached to an Genome instance or subclass")
+            raise ValidationError(
+                "GroupsFile object must be attached to an Genome instance "
+                "or subclass"
+            )
         pass
 
-    def _render(self, staging='staging'):
+    def _render(self, staging="staging"):
         """
         Renders the children GroupDefinition objects to file
         """
         rendered_filename = os.path.join(staging, self.filename)
         self.makedirs(rendered_filename)
-        fout = open(rendered_filename, 'w')
+        fout = open(rendered_filename, "w")
         fout.write(str(self))
         fout.close()
         return fout.name
```

### Comparing `trackhub-0.2.4/trackhub/genomes_file.py` & `trackhub-1.0/trackhub/genomes_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,45 +33,45 @@
 
     @property
     def filename(self):
         if self._filename is not None:
             return self._filename
         if self.hub is None:
             return None
-        return os.path.join(os.path.dirname(self.hub.filename), self.hub.hub + '.genomes.txt')
+        return os.path.join(
+            os.path.dirname(self.hub.filename), self.hub.hub + ".genomes.txt"
+        )
 
     @filename.setter
     def filename(self, fn):
         self._filename = fn
 
     @property
     def hub(self):
         hub, level = self.root(Hub)
         if level is None:
             return None
         if level != -1:
-            raise ValueError(
-                "Found a hub at %s levels away -- needs to be -1" % level)
+            raise ValueError("Found a hub at %s levels away -- needs to be -1" % level)
         return hub
 
     def add_genome(self, genome):
         self.add_child(genome)
         self.genomes = self.children
 
     def __str__(self):
         s = []
         for genome in self.genomes:
             s.append(str(genome))
-        return '\n'.join(s) + '\n'
+        return "\n".join(s) + "\n"
 
-    def _render(self, staging='staging'):
+    def _render(self, staging="staging"):
         rendered_filename = os.path.join(staging, self.filename)
         self.makedirs(rendered_filename)
-        fout = open(rendered_filename, 'w')
+        fout = open(rendered_filename, "w")
         fout.write(str(self))
         fout.close()
         return fout.name
 
     def validate(self):
         if len(self.children) == 0:
-            raise ValueError(
-                "No defined Genome objects to use")
+            raise ValueError("No defined Genome objects to use")
```

### Comparing `trackhub-0.2.4/trackhub/genome.py` & `trackhub-1.0/trackhub/genome.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import absolute_import
 
 import os
 from .validate import ValidationError
 from .base import HubComponent
+from . import constants
 
 
 class Genome(HubComponent):
-    def __init__(self, genome, trackdb=None, genome_file_obj=None):
+    def __init__(self, genome, trackdb=None, genome_file_obj=None, **kwargs):
         """
         Represents a 2-line genome stanza within a "genomes.txt" file.
 
         The file itself is represented by a :class:`GenomesFile` object.
 
         Parameters
         ----------
-
         genome : str
             One of the UCSC-supported assembly names (e.g., "hg38")
 
         trackdb : TrackDb object
             If not None, this object will be attached as the child track db
 
         genome_file : GenomesFile object
@@ -28,48 +28,92 @@
         self.genome = genome
         self.trackdb = None
         if trackdb is not None:
             self.add_trackdb(trackdb)
         if genome_file_obj:
             self.add_parent(genome_file_obj)
 
+        self._orig_kwargs = kwargs
+
+        self.track_field_order = []
+        self.track_field_order.extend(constants.track_fields["genome"])
+
+        self.add_params(**kwargs)
+
     @property
     def genome_file_obj(self):
         try:
             return self.parent
         except AttributeError:
             return None
 
     def add_trackdb(self, trackdb):
         self.children = []
         self.add_child(trackdb)
         self.trackdb = self.children[0]
 
+    def add_params(self, **kw):
+        """
+        Add [possibly many] parameters to the Genome.
+
+        Parameters will be checked against known UCSC parameters and their
+        supported formats.
+        """
+        for k, v in kw.items():
+            if k not in self.track_field_order:
+                raise ParameterError(
+                    '"{0}" is not a valid parameter for {1} with '
+                    "tracktype {2}".format(k, self.__class__.__name__, self.tracktype)
+                )
+            constants.param_dict[k].validate(v)
+
+        self._orig_kwargs.update(kw)
+        self.kwargs = self._orig_kwargs.copy()
+
+    def remove_params(self, *args):
+        """
+        Remove [possibly many] parameters from the Genome.
+
+        E.g.,
+
+        remove_params('color', 'visibility')
+        """
+        for a in args:
+            self._orig_kwargs.pop(a)
+        self.kwargs = self._orig_kwargs.copy()
+
     def __str__(self):
         try:
             self.validate()
         except ValidationError:
             return "Unconfigured <Genome> object"
         s = []
-        s.append('genome %s' % self.genome)
+        s.append("genome %s" % self.genome)
         s.append(
-            'trackDb %s'
+            "trackDb %s"
             % os.path.relpath(
-                self.trackdb.filename,
-                os.path.dirname(self.genome_file_obj.filename)
+                self.trackdb.filename, os.path.dirname(self.genome_file_obj.filename)
             )
         )
-        return '\n'.join(s) + '\n'
+
+        for name in self.track_field_order:
+            value = self.kwargs.pop(name, None)
+            if value is not None:
+                if constants.param_dict[name].validate(value):
+                    s.append("%s %s" % (name, value))
+
+        self.kwargs = self._orig_kwargs.copy()
+
+        return "\n".join(s) + "\n"
 
     def validate(self):
         if len(self.children) == 0:
-            raise ValidationError(
-                "No TrackDb objects provided")
+            raise ValidationError("No TrackDb objects provided")
         if self.trackdb is None:
             raise ValidationError("No TrackDb objects provided")
 
-    def _render(self, staging='staging'):
+    def _render(self, staging="staging"):
         """
         No file is created from a Genome object -- only from its parent
         GenomesFile object.
         """
         pass
```

### Comparing `trackhub-0.2.4/trackhub/base.py` & `trackhub-1.0/trackhub/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,63 +2,69 @@
 import os
 import warnings
 import tempfile
 from collections import OrderedDict
 
 
 def deprecation_handler(source, filename, kwargs):
-    if 'local_fn' in kwargs:
+    if "local_fn" in kwargs:
         warnings.warn(
-            'Please use the argument "source" instead of "local_fn"',
-            DeprecationWarning)
+            'Please use the argument "source" instead of "local_fn"', DeprecationWarning
+        )
         if source is not None:
             raise ValueError(
                 'Both "source" and "local_fn" are specified. Please use '
-                'just "source"')
-        source = kwargs.pop('local_fn')
+                'just "source"'
+            )
+        source = kwargs.pop("local_fn")
 
-    if 'remote_fn' in kwargs:
+    if "remote_fn" in kwargs:
         warnings.warn(
             'Please use the argument "source" instead of "remote_fn"',
-            DeprecationWarning)
+            DeprecationWarning,
+        )
         if filename is not None:
             raise ValueError(
                 'Both "filename" and "remote_fn" are specified. Please use '
-                'just "filename"')
-        filename = kwargs.pop('remote_fn')
+                'just "filename"'
+            )
+        filename = kwargs.pop("remote_fn")
     return source, filename
 
 
 class HubComponent(object):
     """
     Base class for various track hub components.  Several methods must be
     overridden by subclasses.
     """
+
     def __init__(self):
         self.children = []
         self.parent = None
 
-    def _render(self, staging='staging'):
+    def _render(self, staging="staging"):
         """
         Renders the object to file.  Must be overridden by subclass.
 
         Can return None if nothing to be done for the subclass.
         """
         raise NotImplementedError(
             "%s: subclasses must define their own _render() method"
-            % self.__class__.__name__)
+            % self.__class__.__name__
+        )
 
     def validate(self):
         """
         Runs validation, raising exceptions as needed.  Must be overridden by
         subclass.
         """
         raise NotImplementedError(
             "%s: subclasses must define their own validate() method"
-            % self.__class__.__name__)
+            % self.__class__.__name__
+        )
 
     def add_child(self, child):
         """
         Adds self as parent to child, and then adds child.
         """
         child.parent = self
         self.children.append(child)
@@ -109,15 +115,15 @@
             if isinstance(self, cls):
                 yield self, level
             else:
                 raise StopIteration
 
         for child in self.children:
             for leaf, _level in child.leaves(cls, level + 1, intermediate=intermediate):
-                    yield leaf, _level
+                yield leaf, _level
 
     def render(self, staging=None):
         """
         Renders the object to file, returning a list of created files.
 
         Calls validation code, and, as long as each child is also a subclass of
         :class:`HubComponent`, the rendering is recursive.
```

### Comparing `trackhub-0.2.4/trackhub/trackdb.py` & `trackhub-1.0/trackhub/trackdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,31 +46,34 @@
 
     @property
     def genome(self):
         genome, level = self.root(Genome)
         if level is None:
             return None
         if level != -1:
-            raise ValueError('Genome is level %s, not -1' % level)
+            raise ValueError("Genome is level %s, not -1" % level)
         return genome
 
     @property
     def filename(self):
         if self._filename is not None:
             return self._filename
 
         if self.genome is None:
             return None
 
         if self.genomes_file is None:
             return None
 
         else:
-            return os.path.join(os.path.dirname(self.genomes_file.filename),
-                                self.genome.genome, 'trackDb.txt')
+            return os.path.join(
+                os.path.dirname(self.genomes_file.filename),
+                self.genome.genome,
+                "trackDb.txt",
+            )
 
     @filename.setter
     def filename(self, fn):
         self._filename = fn
 
     def add_tracks(self, track):
         """
@@ -80,40 +83,47 @@
         ----------
 
         track : iterable or Track
             Iterable of :class:`Track` objects, or a single :class:`Track`
             object.
         """
         from trackhub import BaseTrack
+
         if isinstance(track, BaseTrack):
             self.add_child(track)
             self._tracks.append(track)
         else:
             for t in track:
                 self.add_child(t)
                 self._tracks.append(t)
 
     @property
     def tracks(self):
         from trackhub import Track
+
         return [i for i, level in self.leaves(Track)]
 
     def add_genome(self, genome):
         self.add_parent(genome)
 
     def __str__(self):
+        self.validate()
         s = []
         for track in self._tracks:
-            s.append(str(track) + '\n')
-        return '\n'.join(s)
+            for line in str(track).splitlines(False):
+                line = line.rstrip()
+                s.append(line)
+            s.append("")
+
+        return "\n".join(s)
 
     def validate(self):
         if len(self.children) == 0:
             raise ValueError("No Track objects specified")
 
-    def _render(self, staging='staging'):
+    def _render(self, staging="staging"):
         rendered_filename = os.path.join(staging, self.filename)
         self.makedirs(rendered_filename)
-        fout = open(rendered_filename, 'w')
+        fout = open(rendered_filename, "w")
         fout.write(str(self))
         fout.close()
         return fout.name
```

### Comparing `trackhub-0.2.4/trackhub/test/test_example_data.py` & `trackhub-1.0/trackhub/test/test_example_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 import os
 import sys
 import hashlib
 from trackhub import helpers
 
+
 def test_example_data_md5s():
     data_dir = helpers.data_dir()
 
-    data = [i.strip().split() for i in '''
+    data = [
+        i.strip().split()
+        for i in """
     3735b696b3a416a59f8755eaf5664e5a  sine-hg38-0.bedgraph.bw
     73ad8ba3590d0895810d069599b0e443  sine-hg38-1.bedgraph.bw
     85478d1ecc5906405ccb43d1ca426d29  sine-hg38-2.bedgraph.bw
     55ac2603c31b232dacfdaba07d8a25eb  sine-no1-1000.bedgraph.bw
     b8c983862c58fee6afa99382634ab2d8  sine-no1-100.bedgraph.bw
     35fa6ac3453e2bbd503c40a1d15afc65  random-hg38-0.bigBed
     3c94c294f8376f625f3701dee7641997  random-hg38-1.bigBed
     3bed0726e452d677f33979b2ed1c65d6  random-hg38-2.bigBed
     72934b760f1f5ee8f99d596536ef8b4c  random-no1-0.bigBed
     19116a3295e5679cb79ffc8904fa5abe  random-no1-1.bigBed
     d628cd0d3b91d8426bb9d0f99b39be52  random-no1-2.bigBed
-    '''.splitlines(False) if not i.strip().startswith('#') and len(i.strip()) > 0]
+    """.splitlines(
+            False
+        )
+        if not i.strip().startswith("#") and len(i.strip()) > 0
+    ]
 
     # for some reason, only faToTwoBit under py27 results in a different md5 than under py3.
     if sys.version_info[0] == 3:
-        data.append(('ba2fd8b22bcad65bb6583da937ff5222', 'newOrg1.2bit'))
+        data.append(("ba2fd8b22bcad65bb6583da937ff5222", "newOrg1.2bit"))
 
     success = True
     for md5, fn in data:
         fn = os.path.join(data_dir, fn)
-        obs = hashlib.md5(open(fn, 'rb').read()).hexdigest()
+        obs = hashlib.md5(open(fn, "rb").read()).hexdigest()
         success = success and (obs == md5)
         print(obs, md5, fn)
     assert success
```

### Comparing `trackhub-0.2.4/trackhub/test/upload_test.py` & `trackhub-1.0/trackhub/test/deprecated_upload_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,101 @@
 import os
 from textwrap import dedent
+import warnings
 import pytest
 import tempfile
 from trackhub import upload
 from trackhub.helpers import data_dir
-from trackhub import Hub, GenomesFile, Genome, Track, CompositeTrack, \
-    TrackDb, ViewTrack, SuperTrack, AggregateTrack
+from trackhub import (
+    Hub,
+    GenomesFile,
+    Genome,
+    Track,
+    CompositeTrack,
+    TrackDb,
+    ViewTrack,
+    SuperTrack,
+    AggregateTrack,
+)
 
 d = data_dir()
 
-class TestUpload(object):
-    def setup(self):
-        self.hub = Hub(
-            hub='example_hub',
-            short_label='example hub',
-            long_label='an example hub for testing',
-            email='none@example.com')
-        self.genomes_file = GenomesFile()
-        self.genome = Genome('dm3')
-        self.trackdb = TrackDb()
-
-        self.tracks = [
-            Track(
-                name='track1',
-                tracktype='bigBed',
-                source=os.path.join(d, 'random-hg38-0.bigBed')
-            ),
-            Track(
-                name='track2',
-                tracktype='bigWig',
-                source=os.path.join(d, 'sine-hg38-0.bedgraph.bw'),
-            ),
-            Track(
-                name='track3',
-                tracktype='bigWig',
-                source=os.path.join(d, 'sine-hg38-1.bedgraph.bw'),
-                filename='3.bw',
+
+class Upload(object):
+    def __init__(self):
+        with pytest.warns(DeprecationWarning):
+            self.hub = Hub(
+                hub="example_hub",
+                short_label="example hub",
+                long_label="an example hub for testing",
+                email="none@example.com",
             )
-        ]
-        self.hub.add_genomes_file(self.genomes_file)
-        self.genomes_file.add_genome(self.genome)
-        self.genome.add_trackdb(self.trackdb)
-        self.trackdb.add_tracks(self.tracks)
-
-    def test_staging(self):
-        staging_dir, linknames = upload.stage_hub(self.hub)
-
-        assert open(os.path.join(staging_dir, 'example_hub.genomes.txt')).read() == dedent(
-            """\
-            genome dm3
-            trackDb dm3/trackDb.txt
-
-            """)
-
-        assert open(os.path.join(staging_dir, 'example_hub.hub.txt')).read() == dedent(
-            """\
-            hub hub
-            shortLabel example hub
-            longLabel an example hub for testing
-            genomesFile example_hub.genomes.txt
-            email none@example.com""")
-
-    #@unittest.skipUnless(os.path.exists('data/track1.bam'), 'No test data')
-    def test_upload(self):
-        d = tempfile.mkdtemp()
-        print(d)
-        upload.upload_hub(
-            hub=self.hub,
-            remote_dir=d,
-            user=None,
-            host=None,
-        )
-
-    def test_render(self):
-        trackdb = str(self.trackdb)
-        # make sure some of the trackdb rendered correctly
-        assert 'track track1' in trackdb
-        assert 'bigDataUrl track1.bigBed' in trackdb
-        assert 'bigDataUrl ../3.bw' in trackdb
+            self.genomes_file = GenomesFile()
+            self.genome = Genome("dm3")
+            self.trackdb = TrackDb()
+
+            self.tracks = [
+                Track(
+                    name="track1",
+                    tracktype="bigBed",
+                    local_fn=os.path.join(d, "random-hg38-0.bigBed"),
+                    remote_fn="1.bigbed",
+                ),
+                Track(
+                    name="track2",
+                    tracktype="bigWig",
+                    local_fn=os.path.join(d, "sine-hg38-0.bedgraph.bw"),
+                    remote_fn="2.bw",
+                ),
+            ]
+            self.hub.add_genomes_file(self.genomes_file)
+            self.genomes_file.add_genome(self.genome)
+            self.genome.add_trackdb(self.trackdb)
+            self.trackdb.add_tracks(self.tracks)
+
+
+@pytest.fixture
+def upload_obj():
+    return Upload()
+
+
+def test_staging(upload_obj):
+    staging_dir, linknames = upload.stage_hub(upload_obj.hub)
+
+    assert open(os.path.join(staging_dir, "example_hub.genomes.txt")).read() == dedent(
+        """\
+        genome dm3
+        trackDb dm3/trackDb.txt
+
+        """
+    )
+
+    assert open(os.path.join(staging_dir, "example_hub.hub.txt")).read() == dedent(
+        """\
+        hub hub
+        shortLabel example hub
+        longLabel an example hub for testing
+        genomesFile example_hub.genomes.txt
+        email none@example.com"""
+    )
+
+    print(staging_dir)
+
+
+# @unittest.skipUnless(os.path.exists('data/track1.bam'), 'No test data')
+def test_upload(upload_obj):
+    d = tempfile.mkdtemp()
+    upload.upload_hub(
+        hub=upload_obj.hub,
+        remote_dir=d,
+        user=None,
+        host=None,
+    )
+
+
+def test_render(upload_obj):
+    trackdb = str(upload_obj.trackdb)
+    print(upload_obj.trackdb)
+    # make sure some of the trackdb rendered correctly
+    assert "track track1" in trackdb
+    assert "bigDataUrl ../1.bigbed" in trackdb
+    assert "bigDataUrl ../2.bw" in trackdb
```

### Comparing `trackhub-0.2.4/trackhub/test/data/sine-no1-1000.bedgraph.bw` & `trackhub-1.0/trackhub/test/data/sine-no1-1000.bedgraph.bw`

 * *Files identical despite different names*

### Comparing `trackhub-0.2.4/trackhub/test/data/random-no1-1.bigBed` & `trackhub-1.0/trackhub/test/data/random-no1-1.bigBed`

 * *Files identical despite different names*

### Comparing `trackhub-0.2.4/trackhub/test/data/random-hg38-2.bigBed` & `trackhub-1.0/trackhub/test/data/random-hg38-2.bigBed`

 * *Files identical despite different names*

### Comparing `trackhub-0.2.4/trackhub/test/data/random-no1-2.bigBed` & `trackhub-1.0/trackhub/test/data/random-no1-2.bigBed`

 * *Files identical despite different names*

### Comparing `trackhub-0.2.4/trackhub/test/data/sine-hg38-0.bedgraph.bw` & `trackhub-1.0/trackhub/test/data/sine-hg38-0.bedgraph.bw`

 * *Files identical despite different names*

### Comparing `trackhub-0.2.4/trackhub/test/data/random-hg38-1.bigBed` & `trackhub-1.0/trackhub/test/data/random-hg38-1.bigBed`

 * *Files identical despite different names*

### Comparing `trackhub-0.2.4/trackhub/test/data/random-no1-0.bigBed` & `trackhub-1.0/trackhub/test/data/random-no1-0.bigBed`

 * *Files identical despite different names*

### Comparing `trackhub-0.2.4/trackhub/test/data/random-hg38-0.bigBed` & `trackhub-1.0/trackhub/test/data/random-hg38-0.bigBed`

 * *Files identical despite different names*

### Comparing `trackhub-0.2.4/trackhub/test/data/sine-no1-100.bedgraph.bw` & `trackhub-1.0/trackhub/test/data/sine-no1-100.bedgraph.bw`

 * *Files identical despite different names*

### Comparing `trackhub-0.2.4/trackhub/test/data/newOrg1.2bit` & `trackhub-1.0/trackhub/test/data/newOrg1.2bit`

 * *Files identical despite different names*

### Comparing `trackhub-0.2.4/trackhub/test/data/sine-hg38-1.bedgraph.bw` & `trackhub-1.0/trackhub/test/data/sine-hg38-1.bedgraph.bw`

 * *Files identical despite different names*

### Comparing `trackhub-0.2.4/trackhub/test/data/sine-hg38-2.bedgraph.bw` & `trackhub-1.0/trackhub/test/data/sine-hg38-2.bedgraph.bw`

 * *Files identical despite different names*

### Comparing `trackhub-0.2.4/trackhub/test/construct_example_data.py` & `trackhub-1.0/trackhub/test/construct_example_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,79 @@
 import os
 import subprocess
 import pybedtools
 import numpy as np
 from trackhub import helpers
 
-np.random.seed(0)
 
-data_dir = helpers.data_dir()
+def make_files():
+    np.random.seed(0)
 
-with open('chromsizes', 'w') as fout:
-    fout.write('chr1\t10000\n')
+    data_dir = helpers.data_dir()
 
-# First, make some example BED files to convert to bigBed
+    with open("chromsizes", "w") as fout:
+        fout.write("chr1\t10000\n")
 
+    # First, make some example BED files to convert to bigBed
+
+    for i, x in enumerate(
+        [
+            pybedtools.BedTool(
+                """
+            chr1 10 50
+            chr1 100 125
+            chr1 300 400
+            """,
+                from_string=True,
+            ),
+            pybedtools.BedTool(
+                """
+            chr1 500 600
+            """,
+                from_string=True,
+            ),
+            pybedtools.BedTool(
+                """
+            chr1 20 60
+            chr1 40 100
+            chr1 80 90
+            chr1 250 300
+            """,
+                from_string=True,
+            ),
+        ]
+    ):
+        out = os.path.join(data_dir, "random-hg38-%s.bigBed" % i)
+        cmds = ["bedToBigBed", x.fn, "chromsizes", out]
+        subprocess.check_call(cmds)
+
+    # make some sine waves for bigWigs
+
+    def sine(resolution=10, power=2):
+        resolution = 10
+        x = np.arange(0, 10000, resolution)
+        y = np.sin(x / resolution ** power) + np.random.random(x.shape[0])
+        for xi, yi in zip(x, y):
+            yield pybedtools.create_interval_from_list(
+                ["chr1", str(xi), str(xi + resolution), "{0:.3f}".format(yi)]
+            )
+
+    for i, x in enumerate(
+        [
+            sine(resolution=10, power=2.0),
+            sine(resolution=10, power=2.5),
+            sine(resolution=10, power=3.0),
+        ]
+    ):
+        x = pybedtools.BedTool(x).saveas(
+            os.path.join(data_dir, "sine-hg38-%d.bedgraph" % i)
+        )
+        out = x.fn + ".bw"
+        cmds = ["bedGraphToBigWig", x.fn, "chromsizes", out]
+        subprocess.check_call(cmds)
+        os.unlink(x.fn)
 
-for i, x in enumerate([
-    pybedtools.BedTool(
-        """
-        chr1 10 50
-        chr1 100 125
-        chr1 300 400
-        """, from_string=True),
-    pybedtools.BedTool(
-        """
-        chr1 500 600
-        """, from_string=True),
-    pybedtools.BedTool(
-        """
-        chr1 20 60
-        chr1 40 100
-        chr1 80 90
-        chr1 250 300
-        """, from_string=True)
-]):
-    out = os.path.join(data_dir, 'random-hg38-%s.bigBed' % i)
-    cmds = [
-        'bedToBigBed',
-        x.fn,
-        'chromsizes',
-        out]
-    subprocess.check_call(cmds)
-
-# make some sine waves for bigWigs
-
-
-
-def sine(resolution=10, power=2):
-    resolution = 10
-    x = np.arange(0, 10000, resolution)
-    y = np.sin(x / resolution ** power) + np.random.random(x.shape[0])
-    for xi, yi in zip(x, y):
-        yield pybedtools.create_interval_from_list([
-            'chr1',
-            str(xi),
-            str(xi + resolution),
-            '{0:.3f}'.format(yi)
-        ])
-
-
-for i, x in enumerate([
-    sine(resolution=10, power=2.0),
-    sine(resolution=10, power=2.5),
-    sine(resolution=10, power=3.0),
-]):
-    x = pybedtools.BedTool(x).saveas(os.path.join(data_dir, 'sine-hg38-%d.bedgraph' % i))
-    out = x.fn + '.bw'
-    cmds = [
-        'bedGraphToBigWig',
-        x.fn,
-        'chromsizes',
-        out]
-    subprocess.check_call(cmds)
-    os.unlink(x.fn)
+    os.unlink("chromsizes")
 
-os.unlink('chromsizes')
+
+if __name__ == "__main__":
+    make_files()
```

### Comparing `trackhub-0.2.4/trackhub/test/construct_example_genome.py` & `trackhub-1.0/trackhub/test/construct_example_genome.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,84 +2,78 @@
 import random
 import subprocess
 from collections import OrderedDict
 import pybedtools
 import numpy as np
 from trackhub import helpers
 
-random.seed(0)
-np.random.seed(0)
 
-data_dir = helpers.data_dir()
+def make_files():
+    random.seed(0)
+    np.random.seed(0)
 
-chromsizes = OrderedDict([
-    ("chr1", (0, 100000)),
-    ("chr2", (0, 75000)),
-    ("chr3", (0, 50000))
-])
-
-
-def random_dna(length, chars="ATGC"):
-    return ''.join(random.choice(chars) for _ in range(length)) + "\n"
-
-fasta = open(os.path.join(data_dir, "newOrg1.fa"), "w")
-
-for chrom, size in chromsizes.items():
-    fasta.write(">" + chrom + "\n")
-    n, r = divmod(size[1], 80)
-    for _ in range(n):
-        fasta.write(random_dna(80))
-    fasta.write(random_dna(r))
-
-cmds = [
-    "faToTwoBit",
-    fasta.name,
-    fasta.name[0:-2] + "2bit"
-]
-
-p = subprocess.check_call(cmds)
-
-fasta.close()
-os.unlink(fasta.name)
-
-g = pybedtools.chromsizes_to_file(chromsizes)
-
-# Make some randomized bigBed files
-for i in range(3):
-    x = pybedtools.BedTool(
-        "chr1 0 100000", from_string=True)\
-        .window_maker(g=g, w=100 * (i + 1))\
-        .shuffle(g=g, seed=i)\
-        .sort()
-
-    out = os.path.join(data_dir, 'random-no1-%s.bigBed' % i)
-
-    cmds = [
-        'bedToBigBed',
-        x.fn,
-        g,
-        out]
-    p = subprocess.check_call(cmds)
+    data_dir = helpers.data_dir()
+
+    chromsizes = OrderedDict(
+        [("chr1", (0, 100000)), ("chr2", (0, 75000)), ("chr3", (0, 50000))]
+    )
 
+    def random_dna(length, chars="ATGC"):
+        return "".join(random.choice(chars) for _ in range(length)) + "\n"
 
-# make some sine waves for bigWigs
-def sine(factor):
+    fasta = open(os.path.join(data_dir, "newOrg1.fa"), "w")
 
     for chrom, size in chromsizes.items():
-        _, size = size
-        x = np.arange(0, size, 10000)
-        y = np.sin(x / factor / np.pi) + np.random.random(len(x)) / 3
-        for xi, yi in zip(x, y):
-            yield pybedtools.create_interval_from_list(list(map(str, [
-                chrom, xi, xi + 1000, yi])))
-
-for f in [100., 1000.]:
-    x = pybedtools.BedTool(sine(f)).saveas(os.path.join(data_dir, 'sine-no1-%d.bedgraph' % f))
-    out = x.fn + '.bw'
-
-    cmds = [
-        'bedGraphToBigWig',
-        x.fn,
-        g,
-        out]
+        fasta.write(">" + chrom + "\n")
+        n, r = divmod(size[1], 80)
+        for _ in range(n):
+            fasta.write(random_dna(80))
+        fasta.write(random_dna(r))
+
+    cmds = ["faToTwoBit", fasta.name, fasta.name[0:-2] + "2bit"]
+
     p = subprocess.check_call(cmds)
-    os.unlink(x.fn)
+
+    fasta.close()
+    os.unlink(fasta.name)
+
+    g = pybedtools.chromsizes_to_file(chromsizes)
+
+    # Make some randomized bigBed files
+    for i in range(3):
+        x = (
+            pybedtools.BedTool("chr1 0 100000", from_string=True)
+            .window_maker(g=g, w=100 * (i + 1))
+            .shuffle(g=g, seed=i)
+            .sort()
+        )
+
+        out = os.path.join(data_dir, "random-no1-%s.bigBed" % i)
+
+        cmds = ["bedToBigBed", x.fn, g, out]
+        p = subprocess.check_call(cmds)
+
+    # make some sine waves for bigWigs
+    def sine(factor):
+
+        for chrom, size in chromsizes.items():
+            _, size = size
+            x = np.arange(0, size, 10000)
+            y = np.sin(x / factor / np.pi) + np.random.random(len(x)) / 3
+            for xi, yi in zip(x, y):
+                yield pybedtools.create_interval_from_list(
+                    list(map(str, [chrom, xi, xi + 1000, yi]))
+                )
+
+    for f in [100.0, 1000.0]:
+        x = pybedtools.BedTool(sine(f)).saveas(
+            os.path.join(data_dir, "sine-no1-%d.bedgraph" % f)
+        )
+        out = x.fn + ".bw"
+
+        cmds = ["bedGraphToBigWig", x.fn, g, out]
+        p = subprocess.check_call(cmds)
+        os.unlink(x.fn)
+
+
+if __name__ == "__main__":
+    make_files()
```

### Comparing `trackhub-0.2.4/trackhub/test/deprecated_upload_test.py` & `trackhub-1.0/trackhub/test/upload_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,100 @@
 import os
 from textwrap import dedent
 import pytest
 import tempfile
 from trackhub import upload
 from trackhub.helpers import data_dir
-from trackhub import Hub, GenomesFile, Genome, Track, CompositeTrack, \
-    TrackDb, ViewTrack, SuperTrack, AggregateTrack
+from trackhub import (
+    Hub,
+    GenomesFile,
+    Genome,
+    Track,
+    CompositeTrack,
+    TrackDb,
+    ViewTrack,
+    SuperTrack,
+    AggregateTrack,
+)
 
 d = data_dir()
 
-class TestUpload(object):
-    def setup(self):
+
+class Upload(object):
+    def __init__(self):
         self.hub = Hub(
-            hub='example_hub',
-            short_label='example hub',
-            long_label='an example hub for testing',
-            email='none@example.com')
+            hub="example_hub",
+            short_label="example hub",
+            long_label="an example hub for testing",
+            email="none@example.com",
+        )
         self.genomes_file = GenomesFile()
-        self.genome = Genome('dm3')
+        self.genome = Genome("dm3")
         self.trackdb = TrackDb()
 
         self.tracks = [
             Track(
-                name='track1',
-                tracktype='bigBed',
-                local_fn=os.path.join(d, 'random-hg38-0.bigBed'),
-                remote_fn='1.bigbed',
+                name="track1",
+                tracktype="bigBed",
+                source=os.path.join(d, "random-hg38-0.bigBed"),
+            ),
+            Track(
+                name="track2",
+                tracktype="bigWig",
+                source=os.path.join(d, "sine-hg38-0.bedgraph.bw"),
             ),
             Track(
-                name='track2',
-                tracktype='bigWig',
-                local_fn=os.path.join(d, 'sine-hg38-0.bedgraph.bw'),
-                remote_fn='2.bw',
+                name="track3",
+                tracktype="bigWig",
+                source=os.path.join(d, "sine-hg38-1.bedgraph.bw"),
+                filename="3.bw",
             ),
         ]
         self.hub.add_genomes_file(self.genomes_file)
         self.genomes_file.add_genome(self.genome)
         self.genome.add_trackdb(self.trackdb)
         self.trackdb.add_tracks(self.tracks)
 
-    def test_staging(self):
-        staging_dir, linknames = upload.stage_hub(self.hub)
-
-        assert open(os.path.join(staging_dir, 'example_hub.genomes.txt')).read() == dedent(
-            """\
-            genome dm3
-            trackDb dm3/trackDb.txt
-
-            """)
-
-        assert open(os.path.join(staging_dir, 'example_hub.hub.txt')).read() == dedent(
-            """\
-            hub hub
-            shortLabel example hub
-            longLabel an example hub for testing
-            genomesFile example_hub.genomes.txt
-            email none@example.com""")
-
-        print(staging_dir)
-
-    #@unittest.skipUnless(os.path.exists('data/track1.bam'), 'No test data')
-    def test_upload(self):
-        d = tempfile.mkdtemp()
-        upload.upload_hub(
-            hub=self.hub,
-            remote_dir=d,
-            user=None,
-            host=None,
-        )
 
-    def test_render(self):
-        trackdb = str(self.trackdb)
-        print(self.trackdb)
-        # make sure some of the trackdb rendered correctly
-        assert 'track track1' in trackdb
-        assert 'bigDataUrl ../1.bigbed' in trackdb
-        assert 'bigDataUrl ../2.bw' in trackdb
+@pytest.fixture
+def upload_obj():
+    return Upload()
+
+
+def test_staging(upload_obj):
+    staging_dir, linknames = upload.stage_hub(upload_obj.hub)
+
+    assert open(os.path.join(staging_dir, "example_hub.genomes.txt")).read() == dedent(
+        """\
+        genome dm3
+        trackDb dm3/trackDb.txt
+
+        """
+    )
+
+    assert open(os.path.join(staging_dir, "example_hub.hub.txt")).read() == dedent(
+        """\
+        hub hub
+        shortLabel example hub
+        longLabel an example hub for testing
+        genomesFile example_hub.genomes.txt
+        email none@example.com"""
+    )
+
+
+def test_upload(upload_obj):
+    d = tempfile.mkdtemp()
+    print(d)
+    upload.upload_hub(
+        hub=upload_obj.hub,
+        remote_dir=d,
+        user=None,
+        host=None,
+    )
+
+
+def test_render(upload_obj):
+    trackdb = str(upload_obj.trackdb)
+    # make sure some of the trackdb rendered correctly
+    assert "track track1" in trackdb
+    assert "bigDataUrl track1.bigBed" in trackdb
+    assert "bigDataUrl ../3.bw" in trackdb
```

### Comparing `trackhub-0.2.4/trackhub/test/test_assembly.py` & `trackhub-1.0/trackhub/test/test_assembly.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 import os
 import glob
 
 hub = trackhub.Hub(
     "assembly_hub",
     short_label="assembly_hub",
     long_label="an example of an assembly hub",
-    email="none@example.com")
+    email="none@example.com",
+)
 
 genome = trackhub.Assembly(
     genome="newOrg1",
     twobit_file=os.path.join(trackhub.helpers.data_dir(), "newOrg1.2bit"),
     organism="Big Foot",
     defaultPos="chr1:0-1000000",
     scientificName="Biggus Footus",
     description="BigFoot V4",
     html_string="BIGFOOT V4 INFO\n",
-    orderKey=4800
+    orderKey=4800,
 )
 
 genomes_file = trackhub.GenomesFile()
 genomes_file.add_genome(genome)
 trackdb = trackhub.TrackDb()
 hub.add_genomes_file(genomes_file)
 
@@ -30,13 +31,13 @@
 genome.add_trackdb(trackdb)
 
 for bw in glob.glob(os.path.join(trackhub.helpers.data_dir(), "*no1*.bw")):
     name, _, _ = os.path.basename(bw).split(".")
     track = trackhub.Track(
         name=trackhub.helpers.sanitize(name),
         source=bw,
-        tracktype='bigWig',
-        autoScale="on")
+        tracktype="bigWig",
+        autoScale="on",
+    )
     trackdb.add_tracks(track)
 
 trackhub.upload.stage_hub(hub)
-
```

### Comparing `trackhub-0.2.4/trackhub/helpers.py` & `trackhub-1.0/trackhub/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     Given a sorted list of subgroups, return a string appropriate to provide as
     a composite track's `dimensions` arg.
 
     Parameters
     ----------
     s : list of SubGroup objects (or anything with a `name` attribute)
     """
-    letters = 'XYABCDEFGHIJKLMNOPQRSTUVWZ'
-    return ' '.join(['dim{0}={1}'.format(dim, sg.name) for dim, sg in zip(letters, s)])
+    letters = "XYABCDEFGHIJKLMNOPQRSTUVWZ"
+    return " ".join(["dim{0}={1}".format(dim, sg.name) for dim, sg in zip(letters, s)])
 
 
 def filter_composite_from_subgroups(s):
     """
     Given a sorted list of subgroups, return a string appropriate to provide as
     the a composite track's `filterComposite` argument
 
@@ -35,39 +35,44 @@
     ----------
     s : list
         A list representing the ordered subgroups, ideally the same list
         provided to `dimensions_from_subgroups`. The values are not actually
         used, just the number of items.
     """
     dims = []
-    for letter, sg in zip('ABCDEFGHIJKLMNOPQRSTUVWZ', s[2:]):
-        dims.append('dim{0}'.format(letter))
+    for letter, sg in zip("ABCDEFGHIJKLMNOPQRSTUVWZ", s[2:]):
+        dims.append("dim{0}".format(letter))
     if dims:
-        return ' '.join(dims)
+        return " ".join(dims)
 
 
 def hex2rgb(h):
     """
     Convert hex colors to RGB tuples
 
     Parameters
     ----------
     h : str
         String hex color value
 
     >>> hex2rgb("#ff0033")
     '255,0,51'
     """
-    if not h.startswith('#') or len(h) != 7:
+    if not h.startswith("#") or len(h) != 7:
         raise ValueError("Does not look like a hex color: '{0}'".format(h))
-    return ','.join(map(str, (
-        int(h[1:3], 16),
-        int(h[3:5], 16),
-        int(h[5:7], 16),
-    )))
+    return ",".join(
+        map(
+            str,
+            (
+                int(h[1:3], 16),
+                int(h[3:5], 16),
+                int(h[5:7], 16),
+            ),
+        )
+    )
 
 
 def sanitize(s, strict=True):
     """
     Sanitize a string.
 
     Spaces are converted to underscore; if strict=True they are then removed.
@@ -77,28 +82,28 @@
     s : str
         String to sanitize
 
     strict : bool
         If True, only alphanumeric characters are allowed. If False, a limited
         set of additional characters (-._) will be allowed.
     """
-    allowed = ''.join(
+    allowed = "".join(
         [
-            'ABCDEFGHIJKLMNOPQRSTUVWXYZ',
-            'abcdefghijklmnopqrstuvwxyz',
-            '0123456789',
+            "ABCDEFGHIJKLMNOPQRSTUVWXYZ",
+            "abcdefghijklmnopqrstuvwxyz",
+            "0123456789",
         ]
     )
 
     if not strict:
-        allowed += '-_.'
+        allowed += "-_."
 
-    s = str(s).replace(' ', '_')
+    s = str(s).replace(" ", "_")
 
-    return ''.join([i for i in s if i in allowed])
+    return "".join([i for i in s if i in allowed])
 
 
 def auto_track_url(track):
     """
     Automatically sets the bigDataUrl for `track`.
 
     Requirements:
@@ -107,15 +112,16 @@
         * the root Hub object must have the Hub.url attribute set
         * the track must have the `source` attribute set
     """
     hub = track.root(cls=Hub)
 
     if hub is None:
         raise ValueError(
-            "track is not fully connected because the root is %s" % repr(hub))
+            "track is not fully connected because the root is %s" % repr(hub)
+        )
     if hub.url is None:
         raise ValueError("hub.url is not set")
     if track.source is None:
         raise ValueError("track.source is not set")
 
 
 def show_rendered_files(results_dict):
@@ -134,51 +140,53 @@
 def print_rendered_results(results_dict):
     """
     Pretty-prints the rendered results dictionary.
 
     Rendered results can be multiply-nested dictionaries; this uses JSON
     serialization to print a nice representation.
     """
+
     class _HubComponentEncoder(json.JSONEncoder):
         def default(self, o):
             if isinstance(o, base.HubComponent):
                 return repr(o)
             return json.JSONEncoder.default(self, o)
+
     formatted = json.dumps(results_dict, indent=4, cls=_HubComponentEncoder)
     # the returned string contains lines with trailing spaces, which causes
     # doctests to fail.  So fix that here.
     for s in formatted.splitlines():
         print(s.rstrip())
 
 
 def data_dir():
     """
     Returns the data directory that contains example files for tests and
     documentation.
     """
-    return os.path.join(os.path.dirname(_here), 'test', 'data')
+    return os.path.join(os.path.dirname(_here), "test", "data")
 
 
 def example_bigbeds():
     """
     Returns list of example bigBed files
     """
     hits = []
     d = data_dir()
     for fn in os.listdir(d):
         fn = os.path.join(d, fn)
-        if os.path.splitext(fn)[-1] == '.bigBed':
+        if os.path.splitext(fn)[-1] == ".bigBed":
             hits.append(os.path.abspath(fn))
     return hits
 
 
 def example_bigwigs():
     """
     Returns list of bigWig example files
     """
     hits = []
     d = data_dir()
     for fn in os.listdir(d):
         fn = os.path.join(d, fn)
-        if os.path.splitext(fn)[-1] == '.bw':
+        if os.path.splitext(fn)[-1] == ".bw":
             hits.append(os.path.abspath(fn))
     return hits
```

### Comparing `trackhub-0.2.4/trackhub/track.py` & `trackhub-1.0/trackhub/track.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,74 @@
 from __future__ import absolute_import
 
 import os
 import re
-from collections import OrderedDict
+import warnings
 from docutils.core import publish_parts
 from trackhub.base import HubComponent, deprecation_handler
 from trackhub import hub
 from trackhub import constants
+from trackhub import settings
 
 
-TRACKTYPES = ['bigWig', 'bam', 'bigBed', 'vcfTabix', None]
+TRACKTYPES = [
+    "bigWig",
+    "bam",
+    "bigBed",
+    "vcfTabix",
+    "bigNarrowPeak",
+    None,
+    "bigBarChart",
+    "bigChain",
+    "bigGenePred",
+    "bigNarrowPeak",
+    "bigMaf",
+    "bigPsl",
+    "halSnake",
+]
 
 
 def _check_name(name):
-    regex = re.compile('[^a-zA-Z0-9-_]')
+    regex = re.compile("[^a-zA-Z0-9-_]")
     if regex.search(name):
         raise ValueError('Non-alphanumeric character in name "%s"' % name)
 
 
 class ParameterError(Exception):
     pass
 
 
+def update_list(existing, new, first=constants.initial_params):
+    """
+    Extend a list, but with constraints.
+
+    Returned list is sorted alphabetically, except for any items that are in
+    `first`, which will come first regardless of sorting.
+
+    Parameters
+    ----------
+    existing : list
+        List to extend
+
+    new : list
+        Update `existing` with this
+
+    first : list or None
+        If provided, ensure that this list occurs at the beginning. Items must
+        already be in `existing` or `new`, others are ignored.
+    """
+    if first is None:
+        first = []
+
+    combined = set(existing + new)
+    beginning = [i for i in first if i in combined]
+    end = sorted(combined.difference(first))
+    return beginning + end
+
+
 class SubGroupDefinition(object):
     def __init__(self, name, label, mapping, default="none"):
         """
         Represents a subgroup line in a composite track.
 
         Instances of this class are provided to a composite track in order to
         define options for the subtracks' groups.
@@ -68,35 +111,32 @@
         self.mapping = mapping
         self.default = default
 
     def __str__(self):
         s = []
         s.append(self.name)
         s.append(self.label)
-        s.extend('%s=%s' % (k, v) for k, v in self.mapping.items())
-        return ' '.join(s)
+        s.extend("%s=%s" % (k, v) for k, v in self.mapping.items())
+        return " ".join(s)
 
 
 class BaseTrack(HubComponent):
-
-    # Dictionary where keys are parameter names (e.g., "color") and values are
-    # Parameter objects.  These are defined in the constants module.
-    params = OrderedDict()
-    params.update(constants.track_field_order)
-    params.update(constants.track_fields)
-
-    # For a plain 'ol Track, there's nothing specific.  But CompositeTracks and
-    # ViewTracks can have addtional specific parameters (e.g., filterComposite
-    # for CompositeTracks) that need to be handled separately.  Make some space
-    # for that here.
-    specific_params = OrderedDict()
-
-    def __init__(self, name, tracktype=None, short_label=None,
-                 long_label=None, parentonoff="on", subgroups=None, source=None,
-                 filename=None, html_string=None, html_string_format="rst", **kwargs):
+    def __init__(
+        self,
+        name,
+        tracktype=None,
+        short_label=None,
+        long_label=None,
+        subgroups=None,
+        source=None,
+        filename=None,
+        html_string=None,
+        html_string_format="rst",
+        **kwargs
+    ):
         """
         Represents a single track stanza, base class for other track types.
 
         Parameters
         ----------
 
         name : str
@@ -111,17 +151,14 @@
             Used for the left-hand side track label; alias for UCSC parameter
             "shortLabel"
 
         long_label : str
             Used for the longer middle labels; if None will copy
             short_label. Alias for UCSC parameter "longLabel".
 
-        parentonoff : 'on' | 'off'
-            Used to determine individual track status on or off
-
         subgroups : dict
             A dictionary of `{name: tag}` where each `name` is the name of
             a SubGroupDefinition in a parent :class:`CompositeTrack` and each
             `tag` is a key in the SubGroupDefinition.mapping dictionary. The
             dictionary `{'celltype': 'ES'}` would end up looking like this in
             the string representation::
 
@@ -149,42 +186,55 @@
             is assumed to be ReStructured Text format, use
             `html_string_format="html"` if the documentation is already in HTML
             format.
 
         html_string_format : 'html' or 'rst'
             Indicates the format of `html_string`. If `"html"`, then use as-is;
             if `"rst"` then convert ReST to HTML.
-
-
         """
         source, filename = deprecation_handler(source, filename, kwargs)
         HubComponent.__init__(self)
         _check_name(name)
         self.name = name
+
+        # Dictionary where keys are parameter names (e.g., "color") and values
+        # are Param objects.  These are defined in the constants module. To
+        # start, we add the params valid for all tracks.
+        #
+        # The Track subclass will add its own parameters when the track type is
+        # set. Other subclasses (Composite and View) will add their own special
+        # params in the class definition.
+        self.track_field_order = []
+        self.track_field_order = update_list(
+            self.track_field_order, constants.track_fields["all"]
+        )
+
+        # NOTE: when setting track type, it will update the track field order
+        # according to the known params for that track...so
+        # self.track_field_order needs to exist first.
         self.tracktype = tracktype
         if short_label is None:
             short_label = name
         self.short_label = short_label
         if long_label is None:
             long_label = short_label
         self.long_label = long_label
-        self.parentonoff = parentonoff
 
         self._source = source
         self._filename = filename
         self.html_string = html_string
         self.html_string_format = html_string_format
         self.subgroups = {}
         self.add_subgroups(subgroups)
 
         # Convert pythonic strings to UCSC versions
-        kwargs['track'] = name
-        kwargs['type'] = tracktype
-        kwargs['longLabel'] = kwargs.get('longLabel', long_label)
-        kwargs['shortLabel'] = kwargs.get('shortLabel', short_label)
+        kwargs["track"] = name
+        kwargs["type"] = tracktype
+        kwargs["longLabel"] = kwargs.get("longLabel", long_label)
+        kwargs["shortLabel"] = kwargs.get("shortLabel", short_label)
 
         self.kwargs = kwargs
 
         self._orig_kwargs = kwargs.copy()
 
     @property
     def _html(self):
@@ -193,14 +243,15 @@
         _html = HTMLDoc(self.html_string, self.html_string_format)
         _html.add_parent(self)
         return _html
 
     @property
     def trackdb(self):
         from trackhub import TrackDb
+
         return self.root(TrackDb)[0]
 
     @property
     def hub(self):
         return self.root(hub.Hub)[0]
 
     @property
@@ -226,15 +277,16 @@
         # However, if source is None and URL is set, then this is an
         # already-existing remote file and so should not have a filename.
         if self.trackdb:
             if self.source is None and self._url is not None:
                 return None
             return os.path.join(
                 os.path.dirname(self.trackdb.filename),
-                self.name + '.' + self.tracktype.split(' ')[0])
+                self.name + "." + self.tracktype.split(" ")[0],
+            )
         return None
 
     @filename.setter
     def filename(self, fn):
         self._filename = fn
 
     @property
@@ -244,20 +296,21 @@
     @tracktype.setter
     def tracktype(self, tracktype):
         """
         When setting the track type, the valid parameters for this track type
         need to be set as well.
         """
         self._tracktype = tracktype
-        if tracktype is not None:
-            if 'bed' in tracktype.lower():
-                tracktype = 'bigBed'
-            elif 'wig' in tracktype.lower():
-                tracktype = 'bigWig'
-        self.params.update(constants.track_typespecific_fields[tracktype])
+
+        # E.g., bigBed 6+3
+        base_tracktype = tracktype.split()[0]
+
+        fields = []
+        fields.extend(constants.track_fields[base_tracktype])
+        self.track_field_order = update_list(self.track_field_order, fields)
 
     def add_trackdb(self, trackdb):
         """
         Attach this track to a parent TrackDb object.
         """
         self.add_parent(trackdb)
 
@@ -270,21 +323,23 @@
 
         E.g.::
 
             add_params(color='128,0,0', visibility='dense')
 
         """
         for k, v in kw.items():
-            if (k not in self.params) and (k not in self.specific_params):
-                raise ParameterError('"%s" is not a valid parameter for %s'
-                                     % (k, self.__class__.__name__))
-            try:
-                self.params[k].validate(v)
-            except KeyError:
-                self.specific_params[k].validate(v)
+            if k not in self.track_field_order and constants.VALIDATE:
+                raise ParameterError(
+                    '"{0}" is not a valid parameter for {1} with '
+                    "tracktype {2}".format(k, self.__class__.__name__, self.tracktype)
+                )
+            if not constants.param_dict[k].validate(v) and constants.VALIDATE:
+                raise ParameterError(
+                    'value "{0}" did not validate for parameter "{1}"'.format(k, v)
+                )
 
         self._orig_kwargs.update(kw)
         self.kwargs = self._orig_kwargs.copy()
 
     def remove_params(self, *args):
         """
         Remove [possibly many] parameters from the track.
@@ -318,71 +373,81 @@
         if subgroups is None:
             subgroups = {}
         assert isinstance(subgroups, dict)
         self.subgroups.update(subgroups)
 
     def __str__(self):
         s = []
+        kwargs = self.kwargs.copy()
+        for name in self.track_field_order:
+            value = kwargs.pop(name, None)
+            if name == "parent":
+                if isinstance(self.parent, BaseTrack):
+                    if value is not None:
+                        s.append("parent {0} {1}".format(self.parent.name, value))
+                    else:
+                        s.append("parent {0}".format(self.parent.name))
+                continue
+
+            if name == "bigDataUrl" and value is None:
+                # fall back to `url` if set
+                value = getattr(self, "url", None)
 
-        specific = []
-        for name, parameter_obj in self.specific_params.items():
-            value = self.kwargs.pop(name, None)
             if value is not None:
-                if parameter_obj.validate(value):
-                    specific.append("%s %s" % (name, value))
-
-        for name, parameter_obj in self.params.items():
-            value = self.kwargs.pop(name, None)
-            if name == 'bigDataUrl':
-                value = getattr(self, 'url', None)
-            if value is not None:
-                if parameter_obj.validate(value):
+                if constants.param_dict[name].validate(value) or not settings.VALIDATE:
                     s.append("%s %s" % (name, value))
 
-        s.extend(specific)
-
+                else:
+                    raise ParameterError(
+                        "The value '{0}' did not validate for parameter '{1}'".format(
+                            value, name
+                        )
+                    )
         # Handle subgroups differently depending on if this is a composite
         # track or not.
         s.extend(self._str_subgroups())
 
-        if self.parent is not None:
-            if isinstance(self.parent, BaseTrack):
-                s.append('parent %s' % self.parent.name + ' ' + self.parentonoff)
-
-        if len(self.kwargs) > 0:
-            raise ParameterError(
-                "Unhandled keyword arguments: %s" % self.kwargs)
+        if settings.VALIDATE:
+            if len(kwargs) > 0:
+                raise ParameterError(
+                    "The following parameters are unknown for track type {0}: "
+                    "{1}".format(self.tracktype, kwargs)
+                )
+        else:
+            for k, v in kwargs.items():
+                s.append("%s %s" % (k, v))
 
         self.kwargs = self._orig_kwargs.copy()
 
-        return '\n'.join(s)
+        return "\n".join(s)
 
-    def _render(self, staging='staging'):
+    def _render(self, staging="staging"):
         if self._html:
             self._html.render(staging)
 
     def _str_subgroups(self):
         """
         helper function to render subgroups as a string
         """
         if not self.subgroups:
             return ""
-        return ['subGroups %s'
-                % ' '.join(['%s=%s' % (k, v) for (k, v) in
-                           self.subgroups.items()])]
+        return [
+            "subGroups %s"
+            % " ".join(["%s=%s" % (k, v) for (k, v) in self.subgroups.items()])
+        ]
 
     def validate(self):
         pass
 
     @property
     def html_fn(self):
         if self.filename and self.trackdb:
             return os.path.join(
-                os.path.dirname(self.trackdb.filename),
-                self.name + '.html')
+                os.path.dirname(self.trackdb.filename), self.name + ".html"
+            )
         else:
             raise ValueError(self.filename)
 
 
 class Track(BaseTrack):
     def __init__(self, url=None, *args, **kwargs):
         """
@@ -399,56 +464,61 @@
             used when using a remote track from some other provider or when you
             need lots of control over the URL. Otherwise the url will be
             automatically created based on `filename`.
 
 
         See :class:`BaseTrack` for details on other arguments.
         """
-        kwargs['bigDataUrl'] = kwargs.get('bigDataUrl', url)
+
+        if "bigDataUrl" in kwargs and url is not None:
+            raise ValueError("Only one of bigDataUrl or url should be specified")
+
+        kwargs["bigDataUrl"] = kwargs.get("bigDataUrl", url)
         super(Track, self).__init__(*args, **kwargs)
-        self._url = url
+        self._url = kwargs["bigDataUrl"]
 
     @property
     def url(self):
         if self._url is not None:
             return self._url
         if self.filename is None:
             return None
         return os.path.relpath(
-            self.filename,
-            start=os.path.dirname(self.trackdb.filename)
+            self.filename, start=os.path.dirname(self.trackdb.filename)
         )
 
     @url.setter
     def url(self, fn):
         self._url = fn
 
 
 class CompositeTrack(BaseTrack):
-
     def __init__(self, *args, **kwargs):
         """
         Represents a composite track.  Subclasses :class:`BaseTrack`, and adds
         some extras.
 
-        Add a view to this composite with :meth:`add_view`.
-
-        Add a subtrack with :meth:`add_track`.
+        Add a view or subtrack to this composite with :meth:`add_tracks`.
 
         Eventually, you'll need to make a :class:`trackdb.TrackDb` instance and
         add this composite to it with :meth:`trackdb.TrackDb.add_tracks()`. If
         you're using subgroups, use the :meth:`CompositeTrack.add_subgroups()`
         method.
 
         See :class:`BaseTrack` for details on arguments. There are no
         additional arguments supported by this class.
         """
         super(CompositeTrack, self).__init__(*args, **kwargs)
 
-        self.specific_params.update(constants.composite_track_fields)
+        self.track_field_order = update_list(
+            self.track_field_order, constants.track_fields["compositeTrack"]
+        )
+        self.track_field_order = update_list(
+            self.track_field_order, constants.track_fields["subGroups"]
+        )
 
         # TODO: are subtracks and views mutually exclusive, or can a composite
         # have both "view-ed" and "non-view-ed" subtracks?
         self.subtracks = []
         self.views = []
 
     def add_subgroups(self, subgroups):
@@ -470,69 +540,96 @@
             assert isinstance(sg, SubGroupDefinition)
             _subgroups[sg.name] = sg
         self.subgroups = _subgroups
 
     def add_subtrack(self, subtrack):
         """
         Add a child :class:`Track`.
+
+        Deprecated in favor of the more generic `add_tracks` method, but
+        maintained for backwards compatibility.
         """
-        self.add_child(subtrack)
-        self.subtracks.append(subtrack)
+        self.add_tracks(subtrack)
 
     def add_view(self, view):
         """
         Add a ViewTrack object to this composite.
 
+        Deprecated in favor of the more generic `add_tracks` method, but
+        maintained for backwards compatibility.
+
         :param view:
             A ViewTrack object.
         """
+        self.add_tracks(view)
 
-        self.add_child(view)
-        self.views.append(view)
+    def add_tracks(self, *args):
+        """
+        This method allows for both view and subtracks to be added to
+        a composite at the same time. `args` can be arbitrary BaseTrack objects
+        (typically Track or View objects), either singly or as a list. For
+        example any of the following are supported::
+
+            add_tracks(view)
+
+            add_tracks(view, [track1, track2])
+
+            add_tracks(track1, track2)
+        """
+        for arg in args:
+            if isinstance(arg, BaseTrack):
+                arg = [arg]
+
+            for track in arg:
+                if isinstance(track, ViewTrack):
+                    self.add_child(track)
+                    self.views.append(track)
+                if isinstance(track, Track):
+                    self.add_child(track)
+                    self.subtracks.append(track)
 
     def _str_subgroups(self):
         """
         renders subgroups to a list of strings
         """
         s = []
 
         i = 0
 
         # if there are any views, there must be a subGroup1 view View tag=val
         # as the first one.  So create it automatically here
         if len(self.views) > 0:
             mapping = dict((i.view, i.view) for i in self.views)
             view_subgroup = SubGroupDefinition(
-                name='view',
-                label='Views',
-                mapping=mapping)
+                name="view", label="Views", mapping=mapping
+            )
             i += 1
-            s.append('subGroup%s %s' % (i, view_subgroup))
+            s.append("subGroup%s %s" % (i, view_subgroup))
 
         for subgroup in self.subgroups.values():
             i += 1
-            s.append('subGroup%s %s' % (i, subgroup))
+            s.append("subGroup%s %s" % (i, subgroup))
         return s
 
     def __str__(self):
 
         s = []
 
         s.append(super(CompositeTrack, self).__str__())
-        s.append('compositeTrack on')
+        s.append("compositeTrack on")
 
         for view in self.views:
             s.append("")
             for line in str(view).splitlines(False):
-                s.append('    ' + line)
+                s.append(constants.INDENT + line)
 
         for subtrack in self.subtracks:
             s.append("")
             for line in str(subtrack).splitlines(False):
-                s.append('    ' + line)
+                s.append(constants.INDENT + line)
         return "\n".join(s)
 
 
 class ViewTrack(BaseTrack):
     def __init__(self, view, *args, **kwargs):
         """
         Represents a View track.  Subclasses :class:`BaseTrack`, and adds some
@@ -553,104 +650,101 @@
             Unique name to use for the view.
 
 
         See :class:`BaseTrack` for details on other arguments.
 
         """
         self.view = view
-        kwargs['view'] = view
+        kwargs["view"] = view
         super(ViewTrack, self).__init__(*args, **kwargs)
+        self.track_field_order = update_list(
+            self.track_field_order, constants.track_fields["view"]
+        )
         self.subtracks = []
 
-    def add_subgroups(self, subgroups):
-        if subgroups is None:
-            subgroups = {}
-        else:
-            raise ValueError('not sure if Views can have subgroups?')
-
-    def add_tracks(self, subtracks):
+    def add_tracks(self, *args):
         """
         Add one or more tracks to this view.
 
-        subtracks : Track or iterable of Tracks
-            A single Track instance or an iterable of them.
-        """
-        if isinstance(subtracks, Track):
-            subtracks = [subtracks]
-        for subtrack in subtracks:
-            subtrack.subgroups['view'] = self.view
-            self.add_child(subtrack)
-            self.subtracks.append(subtrack)
+        Parameters
+        ----------
 
-    def _str_subgroups(self):
-        return ""
+        args : Track or iterable of Tracks
+
+        """
+        for arg in args:
+            if isinstance(arg, BaseTrack):
+                arg = [arg]
+            for track in arg:
+                track.subgroups["view"] = self.view
+                self.add_child(track)
+                self.subtracks.append(track)
 
     def __str__(self):
         s = []
-        view_specific = []
-        for name, parameter_obj in constants.view_track_fields.items():
-            value = self.kwargs.pop(name, None)
-            if value is not None:
-                if parameter_obj.validate(value):
-                    view_specific.append("%s %s" % (name, value))
-
         s.append(super(ViewTrack, self).__str__())
-        s.extend(view_specific)
 
         for subtrack in self.subtracks:
             s.append("")
             for line in str(subtrack).splitlines(False):
-                s.append('        ' + line)
-        return '\n'.join(s)
+                s.append(constants.INDENT + line)
+        return "\n".join(s)
 
 
 class SuperTrack(BaseTrack):
     def __init__(self, *args, **kwargs):
         """
         Represents a Super track. Subclasses :class:`Track`, and adds some
         extras.
 
-        Super tracks are container tracks (Folders) that group tracks. They are
+        Super tracks are container tracks (folders) that group tracks. They are
         used to control visualization of a set of related data.
 
         Eventually, you'll need to make a :class:`trackdb.TrackDb` instance and
         add this supertrack to it with that instance's :meth:`add_tracks`
         method.
 
         See :class:`BaseTrack` for details on arguments.
         """
-        super(SuperTrack, self).__init__(*args, **kwargs)
+        super(SuperTrack, self).__init__(tracktype="superTrack", *args, **kwargs)
+        self.track_field_order = update_list(
+            self.track_field_order, constants.track_fields["superTrack"]
+        )
+
         self.subtracks = []
 
-    def add_tracks(self, subtracks):
+    def add_tracks(self, *args):
         """
         Add one or more tracks.
 
-        subtrack : Track or iterable of Tracks
+        Parameters
+        ----------
+
+        args : Track or iterable of Tracks
+
         """
-        if isinstance(subtracks, BaseTrack):
-            subtracks = [subtracks]
-        for subtrack in subtracks:
-            self.add_child(subtrack)
-            self.subtracks.append(subtrack)
+        for arg in args:
+            if isinstance(arg, BaseTrack):
+                arg = [arg]
+            for track in arg:
+                self.add_child(track)
+                self.subtracks.append(track)
 
     def __str__(self):
 
         s = []
 
         s.append(super(SuperTrack, self).__str__())
-        s.append('superTrack on')
+        s.append("superTrack on")
 
-        # Removed subtracks for Supertrack because composite tracks can be
-        # within the supertrack.  This is also the recommendation from UCSC
         for subtrack in self.subtracks:
             s.append("")
             for line in str(subtrack).splitlines(False):
-                s.append(line)
-        return '\n'.join(s)
+                s.append(constants.INDENT + line)
+        return "\n".join(s)
 
 
 class AggregateTrack(BaseTrack):
     def __init__(self, aggregate, *args, **kwargs):
         """
         Represents an Aggregate or Overlay track. Subclasses :class:`Track`,
         adds some extras.
@@ -672,37 +766,56 @@
             for details.
 
 
         See :class:`BaseTrack` for details on other arguments.
         """
 
         self.aggregate = aggregate
-        kwargs['aggregate'] = aggregate
+        kwargs["aggregate"] = aggregate
         super(AggregateTrack, self).__init__(*args, **kwargs)
-        self.specific_params.update(constants.aggregate_track_fields)
+        self.track_field_order = update_list(
+            self.track_field_order, constants.track_fields["multiWig"]
+        )
         self.subtracks = []
 
     def add_subtrack(self, subtrack):
         """
-        Add a child :class:`SubTrack` to this aggregrate.
+        Add a child :class:`SubTrack` to this aggregate.
+        """
+        self.add_tracks(subtrack)
+
+    def add_tracks(self, *args):
+        """
+        Add one or more tracks.
+
+        Parameters
+        ----------
+
+        args : Track or iterable of Tracks
+
         """
-        self.add_child(subtrack)
-        self.subtracks.append(subtrack)
+
+        for arg in args:
+            if isinstance(arg, BaseTrack):
+                arg = [arg]
+            for track in arg:
+                self.add_child(track)
+                self.subtracks.append(track)
 
     def __str__(self):
 
         s = []
 
         s.append(super(AggregateTrack, self).__str__())
-        s.append('container multiWig')
+        s.append("container multiWig")
 
         for subtrack in self.subtracks:
             s.append("")
             for line in str(subtrack).splitlines(False):
-                s.append('    ' + line)
+                s.append(constants.INDENT + line)
         return "\n".join(s)
 
 
 class HTMLDoc(HubComponent):
     def __init__(self, contents, html_string_format, filename=None):
         """
         Represents an HTML file used for documentation.
@@ -735,55 +848,63 @@
     @property
     def filename(self):
         if self._filename is not None:
             return self._filename
         if self.trackdb is None or self.track is None:
             return None
         return os.path.join(
-            os.path.dirname(self.trackdb.filename),
-            self.track.name + '.html')
+            os.path.dirname(self.trackdb.filename), self.track.name + ".html"
+        )
 
     @filename.setter
     def filename(self, fn):
         self._filename = fn
 
     @property
     def trackdb(self):
         from trackhub import TrackDb
+
         obj, level = self.root(cls=TrackDb)
         return obj
 
     @property
     def track(self):
         return self.parent
 
-    def _render(self, staging='staging'):
+    def _render(self, staging="staging"):
         self.validate()
         dirname = os.path.dirname(self.filename)
         if not os.path.exists(dirname):
             os.makedirs(dirname)
-        fout = open(os.path.join(staging, self.filename), 'w')
+        fout = open(os.path.join(staging, self.filename), "w")
         fout.write(str(self))
         fout.close()
         return fout.name
 
     def validate(self):
         if not self.trackdb:
-            raise ValueError("HTMLDoc object must be connected to a "
-                             "BaseTrack subclass instance and a TrackDb "
-                             "instance")
+            raise ValueError(
+                "HTMLDoc object must be connected to a "
+                "BaseTrack subclass instance and a TrackDb "
+                "instance"
+            )
         return True
 
     def __str__(self):
-        if self.html_string_format == 'html':
+        if self.html_string_format == "html":
             return self.contents
-        elif self.html_string_format == 'rst':
-            parts = publish_parts(
-                self.contents, writer_name='html',
-                settings_overrides={'output_encoding': 'unicode'}
-            )
-            return parts['html_body']
+        elif self.html_string_format == "rst":
+
+            # docutils still internally uses a "U" mode for opening files.
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+                parts = publish_parts(
+                    self.contents,
+                    writer_name="html",
+                    settings_overrides={"output_encoding": "unicode"},
+                )
+            return parts["html_body"]
         else:
             raise ValueError(
                 "html_string_format '{}' not supported".format(self.html_string_format)
             )
         return self.contents
```

### Comparing `trackhub-0.2.4/trackhub/hub.py` & `trackhub-1.0/trackhub/hub.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 from __future__ import absolute_import
 
 import os
+import warnings
 from .validate import ValidationError
 from .base import HubComponent
 
 
 class Hub(HubComponent):
     # map proper track hub stanza field names to pythonic attribute names in
     # this class.
 
-    def __init__(self, hub, short_label=None, long_label=None,
-                 genomes_file=None, genomes_filename=None, email="",
-                 url=None, filename=None):
+    def __init__(
+        self,
+        hub,
+        short_label=None,
+        long_label=None,
+        genomes_file=None,
+        genomes_filename=None,
+        email="",
+        url=None,
+        filename=None,
+    ):
         """
         Represents a top-level track hub container.
 
         hub : str
             Top-level name of the hub.
 
         short_label : str
@@ -39,36 +48,37 @@
         filename : str
             If None, defaults to the value of `hub` plus ".hub.txt". When
             uploaded, the filename is relative to the uploaded location.
         """
         HubComponent.__init__(self)
         if url is not None:
             self.url = url
-            warnings.DeprecationWarning('url is no longer used for Hub objects')
+            warnings.DeprecationWarning("url is no longer used for Hub objects")
         self.hub = hub
         if not short_label:
             short_label = hub
         self.short_label = short_label
         if not long_label:
             long_label = short_label
         self.long_label = long_label
         self.email = email
 
         self.genomes_file = None
         if genomes_file is not None:
             self.add_genomes_file(genomes_file)
 
         if filename is None:
-            filename = hub + '.hub.txt'
+            filename = hub + ".hub.txt"
         self.filename = filename
 
     def validate(self):
         if self.genomes_file is None:
             raise ValidationError(
-                'No GenomesFile attached to Hub (use add_genomes_file())')
+                "No GenomesFile attached to Hub (use add_genomes_file())"
+            )
         self.genomes_file.validate()
         return True
 
     def add_genomes_file(self, genomes_file):
         """
         If a GenomesFile object was not provided upon instantiating this
         object, attach one now
@@ -77,27 +87,27 @@
 
     def __str__(self):
         s = []
         genomes_file = None
         if self.genomes_file:
             genomes_file = self.genomes_file.filename
         for label, value in [
-            ('hub', 'hub'),
-            ('shortLabel', self.short_label),
-            ('longLabel', self.long_label),
-            ('genomesFile', genomes_file),
-            ('email', self.email),
+            ("hub", "hub"),
+            ("shortLabel", self.short_label),
+            ("longLabel", self.long_label),
+            ("genomesFile", genomes_file),
+            ("email", self.email),
         ]:
-            s.append('{0} {1}'.format(label, value))
-        return '\n'.join(s)
+            s.append("{0} {1}".format(label, value))
+        return "\n".join(s)
 
-    def _render(self, staging='staging'):
+    def _render(self, staging="staging"):
         """
         Render just this object, and not all the underlying GenomeFiles and
         their TrackDb.
         """
         rendered_filename = os.path.join(staging, self.filename)
         self.makedirs(rendered_filename)
-        fout = open(rendered_filename, 'w')
+        fout = open(rendered_filename, "w")
         fout.write(str(self))
         fout.close()
         return fout.name
```

### Comparing `trackhub-0.2.4/LICENSE.txt` & `trackhub-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trackhub-0.2.4/setup.py` & `trackhub-1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,22 +17,27 @@
               'trackhub.test',
               'trackhub.test.data',
              ],
     author="Ryan Dale",
     description=long_description,
     long_description=long_description,
     url="http://github.com/daler/trackhub",
+    include_package_data=True,
     package_data = {'trackhub':["test/data/*"]},
     package_dir = {"trackhub": "trackhub"},
+    scripts=["trackhub/trackhub_from_excel"],
     license = 'MIT',
-    author_email="dalerr@niddk.nih.gov",
+    author_email="ryan.dale@nih.gov",
     classifiers=[
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License (GPL)',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 )
```

### Comparing `trackhub-0.2.4/trackhub.egg-info/SOURCES.txt` & `trackhub-1.0/trackhub.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 requirements.txt
 setup.py
 test-requirements.txt
 trackhub/__init__.py
 trackhub/assembly.py
 trackhub/base.py
 trackhub/compatibility.py
 trackhub/constants.py
 trackhub/genome.py
 trackhub/genomes_file.py
 trackhub/groups.py
 trackhub/helpers.py
 trackhub/hub.py
+trackhub/parse.py
+trackhub/parsed_params.py
+trackhub/settings.py
 trackhub/track.py
 trackhub/trackdb.py
+trackhub/trackhub_from_excel
 trackhub/upload.py
 trackhub/validate.py
 trackhub/version.py
 trackhub.egg-info/PKG-INFO
 trackhub.egg-info/SOURCES.txt
 trackhub.egg-info/dependency_links.txt
 trackhub.egg-info/requires.txt
 trackhub.egg-info/top_level.txt
 trackhub/test/__init__.py
 trackhub/test/construct_example_data.py
 trackhub/test/construct_example_genome.py
 trackhub/test/deprecated_upload_test.py
+trackhub/test/test_add_tracks.py
 trackhub/test/test_assembly.py
 trackhub/test/test_components.py
 trackhub/test/test_example_data.py
+trackhub/test/test_supertrack.py
 trackhub/test/upload_test.py
+trackhub/test/data/.gitignore
 trackhub/test/data/__init__.py
-trackhub/test/data/__init__.pyc
+trackhub/test/data/download_ucsc_examples.sh
+trackhub/test/data/example.xlsx
 trackhub/test/data/newOrg1.2bit
 trackhub/test/data/random-hg38-0.bigBed
 trackhub/test/data/random-hg38-1.bigBed
 trackhub/test/data/random-hg38-2.bigBed
 trackhub/test/data/random-no1-0.bigBed
 trackhub/test/data/random-no1-1.bigBed
 trackhub/test/data/random-no1-2.bigBed
```

### Comparing `trackhub-0.2.4/README.rst` & `trackhub-1.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 trackhub
 ========
 
+.. image:: https://github.com/daler/trackhub/workflows/main/badge.svg
+    :target: https://github.com/daler/trackhub/actions?query=workflow%3Amain
+
+See the documentation at https://daler.github.io/trackhub for more details.
+
 Data visualization is critical at all steps of genomic data analysis, from QC
 through final figure preparation.  A `track hub
 <https://genome.ucsc.edu/goldenPath/help/hgTrackHubHelp.html>`_ is way of
 organizing large numbers of of genomic data "tracks" (data files in a supported
 format), configured with a set of plain-text files that determine the
 organization, UI, labels, color, and other details. The files comprising
 a track hub are uploaded to a server, and a genome browser (e.g., UCSC Genome
@@ -18,23 +23,21 @@
 `trackhub` is a Python package that enables the programmatic construction and
 upload of arbitrarily complex track hubs. It has no dependencies besides Python
 itself, the common Python package `docutils`, and the availability of ``rsync``
 (a standard Unix command-line tool for remotely transferring files). It is
 availabe on PyPI, bioconda, and GitHub; an automated test suite and tested
 documentation ensure high-quality code and help.
 
-See the documentation at https://daler.github.io/trackhub for more details.
-
 Installation
 ------------
 
-Using `bioconda <https://bioconda.github.io>`_: ``conda install trackhub``
-
 Using pip: ``pip install trackhub``
 
+Using `bioconda <https://bioconda.github.io>`_: ``conda install trackhub``
+
 Features
 --------
 
 Validation
 ~~~~~~~~~~
 `trackhub` validates parameters against UCSC's documented options, so errors
 are caught early and less time is spent debugging in the Genome Browser.
@@ -72,64 +75,75 @@
 
 .. _basic-example:
 
 Basic example
 -------------
 The following code demonstrates a track hub built out of all bigWig files found
 in a directory. It is relatively simple; see these other examples from the
-documentation for more advanced usage:
-
-- `grouping example <https://daler.github.io/trackhub/grouping.html>`_ (`load the grouping example hub in UCSC <http://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&hubUrl=https://raw.githubusercontent.com/daler/trackhub-demo/master/example_grouping_hub/grouping.hub.txt&position=chr1%3A1-5000>`_)
-- `html documentation example <https://daler.github.io/trackhub/html_doc.html>`_ (`load the HTML documentation example hub in UCSC <http://genome.ucsc.edu/cgi-bin/hgHubConnect?hgHub_do_redirect=on&hgHubConnect.remakeTrackHub=on&hgHub_do_firstDb=1&hubUrl=https://raw.githubusercontent.com/daler/trackhub-demo/master/example_htmldoc_hub/htmldoc.hub.txt>`_)
-- `assembly example <https://daler.github.io/trackhub/assembly_example.html>`_ (`load the assembly example hub in UCSC <http://genome.ucsc.edu/cgi-bin/hgHubConnect?hgHub_do_redirect=on&hgHubConnect.remakeTrackHub=on&hgHub_do_firstDb=1&hubUrl=https://raw.githubusercontent.com/daler/trackhub-demo/master/example_assembly_hub/assembly_hub.hub.txt>`_)
+documentation for complex usage.
 
-This basis example is run automatically when the documentation is re-generated.
+This basic example is run automatically when the documentation is re-generated.
 You can view the uploaded files in the `trackhub-demo
 <https://github.com/daler/trackhub-demo>`_ GitHub repository, and `load the hub
-<http://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&hubUrl=https://raw.githubusercontent.com/daler/trackhub-demo/total-refactor/example_hub/myhub.hub.txt&position=chr1%3A1-5000>`_
+<http://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&hubUrl=https://raw.githubusercontent.com/daler/trackhub-demo/master/example_hub/myhub.hub.txt&position=chr1%3A1-5000>`_
 directly into UCSC to see what it looks like.
 
 .. code-block:: python
 
     import glob, os
     import trackhub
 
     # First we initialize the components of a track hub
+
     hub, genomes_file, genome, trackdb = trackhub.default_hub(
         hub_name="myhub",
         short_label='myhub',
         long_label='myhub',
         genome="hg38",
-        email="dalerr@niddk.nih.gov")
+        email="ryan.dale@nih.gov")
 
-    # Next, we add a track for every bigwig found.  In practice, you would
-    # point to your own files. In this example we use the path to the data
-    # included with trackhub.
+    # Next we add tracks for some bigWigs. These can be anywhere on the
+    # filesystem; symlinks will be made to them. Here we use some example data
+    # included with the trackhub package; in practice you'd point to your own
+    # data.
+
+    for bigwig in glob.glob('trackhub/test/data/sine-hg38-*.bw'):
+
+        # track names can't have any spaces or special characters. Since we'll
+        # be using filenames as names, and filenames have non-alphanumeric
+        # characters, we use the sanitize() function to remove them.
 
-    for bigwig in glob.glob('../trackhub/test/data/sine-hg38-*.bw'):
         name = trackhub.helpers.sanitize(os.path.basename(bigwig))
+
+        # We're keeping this relatively simple, but arguments can be
+        # programmatically determined (color tracks based on sample; change scale
+        # based on criteria, etc).
+
         track = trackhub.Track(
             name=name,          # track names can't have any spaces or special chars.
             source=bigwig,      # filename to build this track from
             visibility='full',  # shows the full signal
             color='128,0,5',    # brick red
             autoScale='on',     # allow the track to autoscale
             tracktype='bigWig', # required when making a track
         )
 
         # Each track is added to the trackdb
+
         trackdb.add_tracks(track)
 
     # In this example we "upload" the hub locally. Files are created in the
     # "example_hub" directory, along with symlinks to the tracks' data files.
     # This directory can then be pushed to GitHub or rsynced to a server.
-    trackhub.upload.upload_hub(hub=hub, host='localhost', remote_dir='example_hub')
+
+    trackhub.upload.upload_hub(hub=hub, host='localhost', remote_dir='example_hubs/example_hub')
 
     # Alternatively, we could upload directly to a web server (not run in this
     # example):
+
     if 0:
         trackhub.upload.upload_hub(
             hub=hub, host='example.com', user='username',
             remote_dir='/var/www/example_hub')
 
 
-Copyright 2012-2017 Ryan Dale; MIT license.
+Copyright 2012-2020 Ryan Dale; MIT license.
```

