# Comparing `tmp/few_shot_learning_nlp-0.0.4.tar.gz` & `tmp/few_shot_learning_nlp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "few_shot_learning_nlp-0.0.4.tar", last modified: Sat Apr 20 13:55:31 2024, max compression
+gzip compressed data, was "few_shot_learning_nlp-0.0.5.tar", last modified: Sat Apr 20 14:02:59 2024, max compression
```

## Comparing `few_shot_learning_nlp-0.0.4.tar` & `few_shot_learning_nlp-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:55:31.598729 few_shot_learning_nlp-0.0.4/
--rw-r--r--   0 pedro.silva (10822) users    (30000)    35149 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.4/LICENSE
--rw-r--r--   0 pedro.silva (10822) users    (30000)      451 2024-04-20 13:55:31.597727 few_shot_learning_nlp-0.0.4/PKG-INFO
--rw-r--r--   0 pedro.silva (10822) users    (30000)       23 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.4/README.md
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:55:31.594737 few_shot_learning_nlp-0.0.4/few_shot_learning_nlp.egg-info/
--rw-r--r--   0 pedro.silva (10822) users    (30000)      451 2024-04-20 13:55:31.000000 few_shot_learning_nlp-0.0.4/few_shot_learning_nlp.egg-info/PKG-INFO
--rw-r--r--   0 pedro.silva (10822) users    (30000)      222 2024-04-20 13:55:31.000000 few_shot_learning_nlp-0.0.4/few_shot_learning_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-20 13:55:31.000000 few_shot_learning_nlp-0.0.4/few_shot_learning_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)        4 2024-04-20 13:55:31.000000 few_shot_learning_nlp-0.0.4/few_shot_learning_nlp.egg-info/top_level.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)       38 2024-04-20 13:55:31.598734 few_shot_learning_nlp-0.0.4/setup.cfg
--rw-r--r--   0 pedro.silva (10822) users    (30000)      636 2024-04-20 13:55:15.000000 few_shot_learning_nlp-0.0.4/setup.py
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:55:31.593729 few_shot_learning_nlp-0.0.4/src/
--rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:54:41.000000 few_shot_learning_nlp-0.0.4/src/__init__.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:02:59.689712 few_shot_learning_nlp-0.0.5/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)    35149 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.5/LICENSE
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:02:59.687713 few_shot_learning_nlp-0.0.5/PKG-INFO
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       23 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.5/README.md
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:02:59.676718 few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:02:59.000000 few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 pedro.silva (10822) users    (30000)      266 2024-04-20 14:02:59.000000 few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-20 14:02:59.000000 few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     2914 2024-04-20 14:02:59.000000 few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/requires.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        4 2024-04-20 14:02:59.000000 few_shot_learning_nlp-0.0.5/few_shot_learning_nlp.egg-info/top_level.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       38 2024-04-20 14:02:59.689717 few_shot_learning_nlp-0.0.5/setup.cfg
+-rw-r--r--   0 pedro.silva (10822) users    (30000)      721 2024-04-20 14:02:15.000000 few_shot_learning_nlp-0.0.5/setup.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:02:59.675713 few_shot_learning_nlp-0.0.5/src/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:54:41.000000 few_shot_learning_nlp-0.0.5/src/__init__.py
```

### Comparing `few_shot_learning_nlp-0.0.4/LICENSE` & `few_shot_learning_nlp-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `few_shot_learning_nlp-0.0.4/setup.py` & `few_shot_learning_nlp-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import setuptools
+from requirements import REQUIRED_PACKAGES
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="few-shot-learning-nlp",
-    version="0.0.4",
+    version="0.0.5",
     author="Pedro Silva",
     author_email="pedrolmssilva@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peulsilva/few-shot-learning-nlp",
     packages=setuptools.find_packages(),
+    install_requires = REQUIRED_PACKAGES,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

