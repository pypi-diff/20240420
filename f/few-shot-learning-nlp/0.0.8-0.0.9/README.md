# Comparing `tmp/few_shot_learning_nlp-0.0.8.tar.gz` & `tmp/few_shot_learning_nlp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "few_shot_learning_nlp-0.0.8.tar", last modified: Sat Apr 20 14:09:01 2024, max compression
+gzip compressed data, was "few_shot_learning_nlp-0.0.9.tar", last modified: Sat Apr 20 14:37:10 2024, max compression
```

## Comparing `few_shot_learning_nlp-0.0.8.tar` & `few_shot_learning_nlp-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:09:01.000672 few_shot_learning_nlp-0.0.8/
--rw-r--r--   0 pedro.silva (10822) users    (30000)    35149 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.8/LICENSE
--rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:09:00.998673 few_shot_learning_nlp-0.0.8/PKG-INFO
--rw-r--r--   0 pedro.silva (10822) users    (30000)       23 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.8/README.md
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:09:00.971677 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/
--rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:54:41.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/__init__.py
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:09:00.986673 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/fewShotTextClassification/
--rw-r--r--   0 pedro.silva (10822) users    (30000)     8311 2024-04-20 13:32:48.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/fewShotTextClassification/SetFit.py
--rw-r--r--   0 pedro.silva (10822) users    (30000)     3454 2024-04-20 13:35:48.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/fewShotTextClassification/SetFitDataset.py
--rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:08:53.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/fewShotTextClassification/__init__.py
--rw-r--r--   0 pedro.silva (10822) users    (30000)        5 2024-04-20 14:05:17.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/hello.py
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:09:00.987681 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/
--rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:09:00.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/PKG-INFO
--rw-r--r--   0 pedro.silva (10822) users    (30000)      498 2024-04-20 14:09:00.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-20 14:09:00.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)     2914 2024-04-20 14:09:00.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/requires.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)       22 2024-04-20 14:09:00.000000 few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/top_level.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)       38 2024-04-20 14:09:01.000677 few_shot_learning_nlp-0.0.8/setup.cfg
--rw-r--r--   0 pedro.silva (10822) users    (30000)      721 2024-04-20 14:08:57.000000 few_shot_learning_nlp-0.0.8/setup.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:37:10.546561 few_shot_learning_nlp-0.0.9/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)    35149 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.9/LICENSE
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:37:10.545556 few_shot_learning_nlp-0.0.9/PKG-INFO
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       23 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.9/README.md
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:37:10.518555 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:54:41.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/__init__.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:37:10.532561 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/fewShotTextClassification/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     8311 2024-04-20 13:32:48.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/fewShotTextClassification/SetFit.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     3454 2024-04-20 13:35:48.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/fewShotTextClassification/SetFitDataset.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:08:53.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/fewShotTextClassification/__init__.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     3163 2024-04-20 14:34:21.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/utils.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:37:10.534560 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:37:10.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 pedro.silva (10822) users    (30000)      498 2024-04-20 14:37:10.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-20 14:37:10.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     2914 2024-04-20 14:37:10.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/requires.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       22 2024-04-20 14:37:10.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/top_level.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       38 2024-04-20 14:37:10.547558 few_shot_learning_nlp-0.0.9/setup.cfg
+-rw-r--r--   0 pedro.silva (10822) users    (30000)      721 2024-04-20 14:37:02.000000 few_shot_learning_nlp-0.0.9/setup.py
```

### Comparing `few_shot_learning_nlp-0.0.8/LICENSE` & `few_shot_learning_nlp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `few_shot_learning_nlp-0.0.8/PKG-INFO` & `few_shot_learning_nlp-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: few-shot-learning-nlp
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Home-page: https://github.com/peulsilva/few-shot-learning-nlp
 Author: Pedro Silva
 Author-email: pedrolmssilva@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/fewShotTextClassification/SetFit.py` & `few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/fewShotTextClassification/SetFit.py`

 * *Files identical despite different names*

### Comparing `few_shot_learning_nlp-0.0.8/few_shot_learning_nlp/fewShotTextClassification/SetFitDataset.py` & `few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/fewShotTextClassification/SetFitDataset.py`

 * *Files identical despite different names*

### Comparing `few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/PKG-INFO` & `few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: few-shot-learning-nlp
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Home-page: https://github.com/peulsilva/few-shot-learning-nlp
 Author: Pedro Silva
 Author-email: pedrolmssilva@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `few_shot_learning_nlp-0.0.8/few_shot_learning_nlp.egg-info/requires.txt` & `few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `few_shot_learning_nlp-0.0.8/setup.py` & `few_shot_learning_nlp-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from requirements import REQUIRED_PACKAGES
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="few-shot-learning-nlp",
-    version="0.0.8",
+    version="0.0.9",
     author="Pedro Silva",
     author_email="pedrolmssilva@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peulsilva/few-shot-learning-nlp",
     packages=setuptools.find_packages(),
```

