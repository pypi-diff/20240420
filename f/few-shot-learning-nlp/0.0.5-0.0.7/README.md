# Comparing `tmp/few_shot_learning_nlp-0.0.5.tar.gz` & `tmp/few_shot_learning_nlp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "few_shot_learning_nlp-0.0.5.tar", last modified: Sat Apr 20 14:02:59 2024, max compression
+gzip compressed data, was "few_shot_learning_nlp-0.0.7.tar", last modified: Sat Apr 20 14:06:44 2024, max compression
```

## Comparing `few_shot_learning_nlp-0.0.5.tar` & `few_shot_learning_nlp-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:02:59.689712 few_shot_learning_nlp-0.0.5/
--rw-r--r--   0 pedro.silva (10822) users    (30000)    35149 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.5/LICENSE
--rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:02:59.687713 few_shot_learning_nlp-0.0.5/PKG-INFO
--rw-r--r--   0 pedro.silva (10822) users    (30000)       23 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.5/README.md
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:02:59.676718 few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/
--rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:02:59.000000 few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/PKG-INFO
--rw-r--r--   0 pedro.silva (10822) users    (30000)      266 2024-04-20 14:02:59.000000 few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-20 14:02:59.000000 few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)     2914 2024-04-20 14:02:59.000000 few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/requires.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)        4 2024-04-20 14:02:59.000000 few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/top_level.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)       38 2024-04-20 14:02:59.689717 few_shot_learning_nlp-0.0.5/setup.cfg
--rw-r--r--   0 pedro.silva (10822) users    (30000)      721 2024-04-20 14:02:15.000000 few_shot_learning_nlp-0.0.5/setup.py
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:02:59.675713 few_shot_learning_nlp-0.0.5/src/
--rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:54:41.000000 few_shot_learning_nlp-0.0.5/src/__init__.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:06:44.891687 few_shot_learning_nlp-0.0.7/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)    35149 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.7/LICENSE
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:06:44.890681 few_shot_learning_nlp-0.0.7/PKG-INFO
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       23 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.7/README.md
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:06:44.869682 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:54:41.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp/__init__.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        5 2024-04-20 14:05:17.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp/hello.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:06:44.880680 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:06:44.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 pedro.silva (10822) users    (30000)      315 2024-04-20 14:06:44.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-20 14:06:44.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     2914 2024-04-20 14:06:44.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/requires.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       22 2024-04-20 14:06:44.000000 few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/top_level.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       38 2024-04-20 14:06:44.892684 few_shot_learning_nlp-0.0.7/setup.cfg
+-rw-r--r--   0 pedro.silva (10822) users    (30000)      721 2024-04-20 14:06:07.000000 few_shot_learning_nlp-0.0.7/setup.py
```

### Comparing `few_shot_learning_nlp-0.0.5/LICENSE` & `few_shot_learning_nlp-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `few_shot_learning_nlp-0.0.5/PKG-INFO` & `few_shot_learning_nlp-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: few-shot-learning-nlp
-Version: 0.0.5
+Version: 0.0.7
 Summary: A small example package
 Home-page: https://github.com/peulsilva/few-shot-learning-nlp
 Author: Pedro Silva
 Author-email: pedrolmssilva@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/PKG-INFO` & `few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: few-shot-learning-nlp
-Version: 0.0.5
+Version: 0.0.7
 Summary: A small example package
 Home-page: https://github.com/peulsilva/few-shot-learning-nlp
 Author: Pedro Silva
 Author-email: pedrolmssilva@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/requires.txt` & `few_shot_learning_nlp-0.0.7/few_shot_learning_nlp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `few_shot_learning_nlp-0.0.5/setup.py` & `few_shot_learning_nlp-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from requirements import REQUIRED_PACKAGES
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="few-shot-learning-nlp",
-    version="0.0.5",
+    version="0.0.7",
     author="Pedro Silva",
     author_email="pedrolmssilva@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peulsilva/few-shot-learning-nlp",
     packages=setuptools.find_packages(),
```

