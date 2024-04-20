# Comparing `tmp/few_shot_learning_nlp-0.0.7.tar.gz` & `tmp/few_shot_learning_nlp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "few_shot_learning_nlp-0.0.7.tar", last modified: Sat Apr 20 14:06:44 2024, max compression
+gzip compressed data, was "few_shot_learning_nlp-0.0.8.tar", last modified: Sat Apr 20 14:09:01 2024, max compression
```

## Comparing `few_shot_learning_nlp-0.0.7.tar` & `few_shot_learning_nlp-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:06:44.891687 few_shot_learning_nlp-0.0.7/
--rw-r--r--   0 pedro.silva (10822) users    (30000)    35149 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.7/LICENSE
--rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:06:44.890681 few_shot_learning_nlp-0.0.7/PKG-INFO
--rw-r--r--   0 pedro.silva (10822) users    (30000)       23 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.7/README.md
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:06:44.869682 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp/
--rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:54:41.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp/__init__.py
--rw-r--r--   0 pedro.silva (10822) users    (30000)        5 2024-04-20 14:05:17.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp/hello.py
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:06:44.880680 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/
--rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:06:44.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/PKG-INFO
--rw-r--r--   0 pedro.silva (10822) users    (30000)      315 2024-04-20 14:06:44.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-20 14:06:44.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)     2914 2024-04-20 14:06:44.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/requires.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)       22 2024-04-20 14:06:44.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/top_level.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)       38 2024-04-20 14:06:44.892684 few_shot_learning_nlp-0.0.7/setup.cfg
--rw-r--r--   0 pedro.silva (10822) users    (30000)      721 2024-04-20 14:06:07.000000 few_shot_learning_nlp-0.0.7/setup.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:09:01.000672 few_shot_learning_nlp-0.0.8/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)    35149 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.8/LICENSE
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:09:00.998673 few_shot_learning_nlp-0.0.8/PKG-INFO
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       23 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.8/README.md
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:09:00.971677 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:54:41.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/__init__.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:09:00.986673 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/fewShotTextClassification/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     8311 2024-04-20 13:32:48.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/fewShotTextClassification/SetFit.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     3454 2024-04-20 13:35:48.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/fewShotTextClassification/SetFitDataset.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:08:53.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/fewShotTextClassification/__init__.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        5 2024-04-20 14:05:17.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/hello.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:09:00.987681 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:09:00.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 pedro.silva (10822) users    (30000)      498 2024-04-20 14:09:00.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-20 14:09:00.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     2914 2024-04-20 14:09:00.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/requires.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       22 2024-04-20 14:09:00.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/top_level.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       38 2024-04-20 14:09:01.000677 few_shot_learning_nlp-0.0.8/setup.cfg
+-rw-r--r--   0 pedro.silva (10822) users    (30000)      721 2024-04-20 14:08:57.000000 few_shot_learning_nlp-0.0.8/setup.py
```

### Comparing `few_shot_learning_nlp-0.0.7/LICENSE` & `few_shot_learning_nlp-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `few_shot_learning_nlp-0.0.7/PKG-INFO` & `few_shot_learning_nlp-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: few-shot-learning-nlp
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Home-page: https://github.com/peulsilva/few-shot-learning-nlp
 Author: Pedro Silva
 Author-email: pedrolmssilva@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/PKG-INFO` & `few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: few-shot-learning-nlp
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Home-page: https://github.com/peulsilva/few-shot-learning-nlp
 Author: Pedro Silva
 Author-email: pedrolmssilva@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/requires.txt` & `few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `few_shot_learning_nlp-0.0.7/setup.py` & `few_shot_learning_nlp-0.0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from requirements import REQUIRED_PACKAGES
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="few-shot-learning-nlp",
-    version="0.0.7",
+    version="0.0.8",
     author="Pedro Silva",
     author_email="pedrolmssilva@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peulsilva/few-shot-learning-nlp",
     packages=setuptools.find_packages(),
```

