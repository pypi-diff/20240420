# Comparing `tmp/few_shot_learning_nlp-0.0.2.tar.gz` & `tmp/few_shot_learning_nlp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "few_shot_learning_nlp-0.0.2.tar", last modified: Sat Apr 20 13:24:02 2024, max compression
+gzip compressed data, was "few_shot_learning_nlp-0.0.3.tar", last modified: Sat Apr 20 13:36:01 2024, max compression
```

## Comparing `few_shot_learning_nlp-0.0.2.tar` & `few_shot_learning_nlp-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:24:02.016853 few_shot_learning_nlp-0.0.2/
--rw-r--r--   0 pedro.silva (10822) users    (30000)    35149 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.2/LICENSE
--rw-r--r--   0 pedro.silva (10822) users    (30000)      451 2024-04-20 13:24:02.014858 few_shot_learning_nlp-0.0.2/PKG-INFO
--rw-r--r--   0 pedro.silva (10822) users    (30000)       23 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.2/README.md
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:24:02.012858 few_shot_learning_nlp-0.0.2/few_shot_learning_nlp.egg-info/
--rw-r--r--   0 pedro.silva (10822) users    (30000)      451 2024-04-20 13:24:01.000000 few_shot_learning_nlp-0.0.2/few_shot_learning_nlp.egg-info/PKG-INFO
--rw-r--r--   0 pedro.silva (10822) users    (30000)      206 2024-04-20 13:24:01.000000 few_shot_learning_nlp-0.0.2/few_shot_learning_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-20 13:24:01.000000 few_shot_learning_nlp-0.0.2/few_shot_learning_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-20 13:24:01.000000 few_shot_learning_nlp-0.0.2/few_shot_learning_nlp.egg-info/top_level.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)       38 2024-04-20 13:24:02.016858 few_shot_learning_nlp-0.0.2/setup.cfg
--rw-r--r--   0 pedro.silva (10822) users    (30000)      636 2024-04-20 13:23:44.000000 few_shot_learning_nlp-0.0.2/setup.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:36:01.911853 few_shot_learning_nlp-0.0.3/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)    35149 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.3/LICENSE
+-rw-r--r--   0 pedro.silva (10822) users    (30000)      451 2024-04-20 13:36:01.909858 few_shot_learning_nlp-0.0.3/PKG-INFO
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       23 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.3/README.md
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:36:01.907857 few_shot_learning_nlp-0.0.3/few_shot_learning_nlp.egg-info/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)      451 2024-04-20 13:36:01.000000 few_shot_learning_nlp-0.0.3/few_shot_learning_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 pedro.silva (10822) users    (30000)      206 2024-04-20 13:36:01.000000 few_shot_learning_nlp-0.0.3/few_shot_learning_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-20 13:36:01.000000 few_shot_learning_nlp-0.0.3/few_shot_learning_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-20 13:36:01.000000 few_shot_learning_nlp-0.0.3/few_shot_learning_nlp.egg-info/top_level.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       38 2024-04-20 13:36:01.911858 few_shot_learning_nlp-0.0.3/setup.cfg
+-rw-r--r--   0 pedro.silva (10822) users    (30000)      636 2024-04-20 13:35:58.000000 few_shot_learning_nlp-0.0.3/setup.py
```

### Comparing `few_shot_learning_nlp-0.0.2/LICENSE` & `few_shot_learning_nlp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `few_shot_learning_nlp-0.0.2/setup.py` & `few_shot_learning_nlp-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="few-shot-learning-nlp",
-    version="0.0.2",
+    version="0.0.3",
     author="Pedro Silva",
     author_email="pedrolmssilva@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peulsilva/few-shot-learning-nlp",
     packages=setuptools.find_packages(),
```

