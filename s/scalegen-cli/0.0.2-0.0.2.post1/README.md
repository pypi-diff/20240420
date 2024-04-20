# Comparing `tmp/scalegen-cli-0.0.2.tar.gz` & `tmp/scalegen-cli-0.0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalegen-cli-0.0.2.tar", last modified: Wed Mar 20 10:37:30 2024, max compression
+gzip compressed data, was "scalegen-cli-0.0.2.post1.tar", last modified: Wed Mar 20 10:44:23 2024, max compression
```

## Comparing `scalegen-cli-0.0.2.tar` & `scalegen-cli-0.0.2.post1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:37:30.649573 scalegen-cli-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-20 10:37:30.649573 scalegen-cli-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:37:30.649573 scalegen-cli-0.0.2/scalegen_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-20 10:37:30.000000 scalegen-cli-0.0.2/scalegen_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-20 10:37:30.000000 scalegen-cli-0.0.2/scalegen_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 10:37:30.000000 scalegen-cli-0.0.2/scalegen_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-20 10:37:30.000000 scalegen-cli-0.0.2/scalegen_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-20 10:37:30.000000 scalegen-cli-0.0.2/scalegen_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-20 10:37:30.000000 scalegen-cli-0.0.2/scalegen_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 10:37:30.649573 scalegen-cli-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:37:30.645573 scalegen-cli-0.0.2/st_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:37:30.649573 scalegen-cli-0.0.2/st_cli/datamodels/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/datamodels/.git
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/datamodels/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/datamodels/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:37:30.649573 scalegen-cli-0.0.2/st_cli/datamodels/datamodels/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/datamodels/datamodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:37:30.649573 scalegen-cli-0.0.2/st_cli/datamodels/datamodels/api/
--rw-r--r--   0 runner    (1001) docker     (127)    17733 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/datamodels/datamodels/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:37:30.649573 scalegen-cli-0.0.2/st_cli/datamodels/datamodels/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/datamodels/datamodels/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:37:30.649573 scalegen-cli-0.0.2/st_cli/datamodels/datamodels/common/
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/datamodels/datamodels/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:37:30.649573 scalegen-cli-0.0.2/st_cli/datamodels/datamodels/jc/
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/datamodels/datamodels/jc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/datamodels/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    12220 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/sg_finetune.py
--rw-r--r--   0 runner    (1001) docker     (127)    16319 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/sg_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/visualisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-03-20 10:37:23.000000 scalegen-cli-0.0.2/st_cli/workstation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.547638 scalegen-cli-0.0.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-20 10:44:23.000000 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-20 10:44:23.000000 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 10:44:23.000000 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-20 10:44:23.000000 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-20 10:44:23.000000 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-20 10:44:23.000000 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 10:44:23.547638 scalegen-cli-0.0.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/.git
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    17733 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/jc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/jc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12220 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/sg_finetune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16319 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/sg_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/workstation.py
```

### Comparing `scalegen-cli-0.0.2/PKG-INFO` & `scalegen-cli-0.0.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalegen-cli
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: ScaleTorch CLI
 Home-page: https://github.com/ScaleTorch/st-cli
 Requires-Python: >=3.6, <3.12
 Requires-Dist: certifi==2021.10.8
 Requires-Dist: charset-normalizer==2.0.11
 Requires-Dist: checksumdir==1.2.0
 Requires-Dist: click==8.0.3
```

### Comparing `scalegen-cli-0.0.2/scalegen_cli.egg-info/PKG-INFO` & `scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalegen-cli
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: ScaleTorch CLI
 Home-page: https://github.com/ScaleTorch/st-cli
 Requires-Python: >=3.6, <3.12
 Requires-Dist: certifi==2021.10.8
 Requires-Dist: charset-normalizer==2.0.11
 Requires-Dist: checksumdir==1.2.0
 Requires-Dist: click==8.0.3
```

### Comparing `scalegen-cli-0.0.2/scalegen_cli.egg-info/SOURCES.txt` & `scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/setup.py` & `scalegen-cli-0.0.2.post1/setup.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/client.py` & `scalegen-cli-0.0.2.post1/st_cli/client.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/datamodels/.gitignore` & `scalegen-cli-0.0.2.post1/st_cli/datamodels/.gitignore`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/datamodels/datamodels/api/__init__.py` & `scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/api/__init__.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/datamodels/datamodels/cli/__init__.py` & `scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/datamodels/datamodels/common/__init__.py` & `scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/common/__init__.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/datamodels/datamodels/jc/__init__.py` & `scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/jc/__init__.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/job.py` & `scalegen-cli-0.0.2.post1/st_cli/job.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/launch.py` & `scalegen-cli-0.0.2.post1/st_cli/launch.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/list.py` & `scalegen-cli-0.0.2.post1/st_cli/list.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/login.py` & `scalegen-cli-0.0.2.post1/st_cli/login.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/main.py` & `scalegen-cli-0.0.2.post1/st_cli/main.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/sg_finetune.py` & `scalegen-cli-0.0.2.post1/st_cli/sg_finetune.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/sg_inference.py` & `scalegen-cli-0.0.2.post1/st_cli/sg_inference.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/stop.py` & `scalegen-cli-0.0.2.post1/st_cli/stop.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/utils.py` & `scalegen-cli-0.0.2.post1/st_cli/utils.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/view.py` & `scalegen-cli-0.0.2.post1/st_cli/view.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/visualisation.py` & `scalegen-cli-0.0.2.post1/st_cli/visualisation.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2/st_cli/workstation.py` & `scalegen-cli-0.0.2.post1/st_cli/workstation.py`

 * *Files identical despite different names*

