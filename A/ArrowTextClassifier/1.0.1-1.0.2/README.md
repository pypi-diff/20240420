# Comparing `tmp/ArrowTextClassifier-1.0.1.tar.gz` & `tmp/ArrowTextClassifier-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ArrowTextClassifier-1.0.1.tar", last modified: Sat Apr 20 13:39:17 2024, max compression
+gzip compressed data, was "ArrowTextClassifier-1.0.2.tar", last modified: Sat Apr 20 14:04:54 2024, max compression
```

## Comparing `ArrowTextClassifier-1.0.1.tar` & `ArrowTextClassifier-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 13:39:17.136318 ArrowTextClassifier-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-20 13:39:17.108240 ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/
--rw-rw-rw-   0        0        0     3835 2024-04-20 13:39:16.000000 ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-04-20 13:39:17.000000 ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 13:39:16.000000 ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-04-20 13:39:16.000000 ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-20 13:39:16.000000 ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2024-04-15 12:47:46.000000 ArrowTextClassifier-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3835 2024-04-20 13:39:17.134753 ArrowTextClassifier-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2623 2024-04-20 13:28:04.000000 ArrowTextClassifier-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-20 13:39:17.136318 ArrowTextClassifier-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1783 2024-04-20 13:33:59.000000 ArrowTextClassifier-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 13:39:17.131500 ArrowTextClassifier-1.0.1/src/
--rw-rw-rw-   0        0        0      307 2024-04-20 13:01:37.000000 ArrowTextClassifier-1.0.1/src/__init__.py
--rw-rw-rw-   0        0        0     2505 2024-04-20 12:36:05.000000 ArrowTextClassifier-1.0.1/src/classify_text.py
--rw-rw-rw-   0        0        0     1772 2024-04-20 13:01:26.000000 ArrowTextClassifier-1.0.1/src/main.py
--rw-rw-rw-   0        0        0     1317 2024-04-15 12:53:00.000000 ArrowTextClassifier-1.0.1/src/model.py
--rw-rw-rw-   0        0        0     1628 2024-04-20 10:43:28.000000 ArrowTextClassifier-1.0.1/src/summarize_model.py
--rw-rw-rw-   0        0        0      718 2024-04-15 12:53:00.000000 ArrowTextClassifier-1.0.1/src/tokenizer.py
--rw-rw-rw-   0        0        0     6955 2024-04-20 11:33:27.000000 ArrowTextClassifier-1.0.1/src/train.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:04:54.901948 ArrowTextClassifier-1.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-20 14:04:54.846707 ArrowTextClassifier-1.0.2/ArrowTextClassifier/
+-rw-rw-rw-   0        0        0      307 2024-04-20 13:01:37.000000 ArrowTextClassifier-1.0.2/ArrowTextClassifier/__init__.py
+-rw-rw-rw-   0        0        0     2505 2024-04-20 12:36:05.000000 ArrowTextClassifier-1.0.2/ArrowTextClassifier/classify_text.py
+-rw-rw-rw-   0        0        0     1772 2024-04-20 13:01:26.000000 ArrowTextClassifier-1.0.2/ArrowTextClassifier/main.py
+-rw-rw-rw-   0        0        0     1317 2024-04-15 12:53:00.000000 ArrowTextClassifier-1.0.2/ArrowTextClassifier/model.py
+-rw-rw-rw-   0        0        0     1628 2024-04-20 10:43:28.000000 ArrowTextClassifier-1.0.2/ArrowTextClassifier/summarize_model.py
+-rw-rw-rw-   0        0        0      718 2024-04-15 12:53:00.000000 ArrowTextClassifier-1.0.2/ArrowTextClassifier/tokenizer.py
+-rw-rw-rw-   0        0        0     6955 2024-04-20 11:33:27.000000 ArrowTextClassifier-1.0.2/ArrowTextClassifier/train.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:04:54.897242 ArrowTextClassifier-1.0.2/ArrowTextClassifier.egg-info/
+-rw-rw-rw-   0        0        0     3835 2024-04-20 14:04:54.000000 ArrowTextClassifier-1.0.2/ArrowTextClassifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2024-04-20 14:04:54.000000 ArrowTextClassifier-1.0.2/ArrowTextClassifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 14:04:54.000000 ArrowTextClassifier-1.0.2/ArrowTextClassifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-04-20 14:04:54.000000 ArrowTextClassifier-1.0.2/ArrowTextClassifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-20 14:04:54.000000 ArrowTextClassifier-1.0.2/ArrowTextClassifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2024-04-15 12:47:46.000000 ArrowTextClassifier-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3835 2024-04-20 14:04:54.900962 ArrowTextClassifier-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2623 2024-04-20 13:28:04.000000 ArrowTextClassifier-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 14:04:54.902856 ArrowTextClassifier-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1783 2024-04-20 14:04:47.000000 ArrowTextClassifier-1.0.2/setup.py
```

### Comparing `ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/PKG-INFO` & `ArrowTextClassifier-1.0.2/ArrowTextClassifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArrowTextClassifier
-Version: 1.0.1
+Version: 1.0.2
 Summary: ArrowTextClassifier is a simple text classification tool written in pytorch that allows you to train, summarize, and use text classification models for various tasks.
 Home-page: https://github.com/Bhargav230m/ArrowTextClassifier.git
 Author: techpowerb
 Author-email: technologypower24@gmail.com
 Keywords: text classification,natural language processing,NLP,PyTorch,machine learning,deep learning,text summarization,preprocessing,data science,artificial intelligence,dataset,discord
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ArrowTextClassifier-1.0.1/LICENSE` & `ArrowTextClassifier-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ArrowTextClassifier-1.0.1/PKG-INFO` & `ArrowTextClassifier-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArrowTextClassifier
-Version: 1.0.1
+Version: 1.0.2
 Summary: ArrowTextClassifier is a simple text classification tool written in pytorch that allows you to train, summarize, and use text classification models for various tasks.
 Home-page: https://github.com/Bhargav230m/ArrowTextClassifier.git
 Author: techpowerb
 Author-email: technologypower24@gmail.com
 Keywords: text classification,natural language processing,NLP,PyTorch,machine learning,deep learning,text summarization,preprocessing,data science,artificial intelligence,dataset,discord
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ArrowTextClassifier-1.0.1/README.md` & `ArrowTextClassifier-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ArrowTextClassifier-1.0.1/setup.py` & `ArrowTextClassifier-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="ArrowTextClassifier",
-    version="1.0.1",
+    version="1.0.2",
     author="techpowerb",
     author_email="technologypower24@gmail.com",
     description="ArrowTextClassifier is a simple text classification tool written in pytorch that allows you to train, summarize, and use text classification models for various tasks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bhargav230m/ArrowTextClassifier.git",
     packages=find_packages(),
```

### Comparing `ArrowTextClassifier-1.0.1/src/classify_text.py` & `ArrowTextClassifier-1.0.2/ArrowTextClassifier/classify_text.py`

 * *Files identical despite different names*

### Comparing `ArrowTextClassifier-1.0.1/src/main.py` & `ArrowTextClassifier-1.0.2/ArrowTextClassifier/main.py`

 * *Files identical despite different names*

### Comparing `ArrowTextClassifier-1.0.1/src/model.py` & `ArrowTextClassifier-1.0.2/ArrowTextClassifier/model.py`

 * *Files identical despite different names*

### Comparing `ArrowTextClassifier-1.0.1/src/summarize_model.py` & `ArrowTextClassifier-1.0.2/ArrowTextClassifier/summarize_model.py`

 * *Files identical despite different names*

### Comparing `ArrowTextClassifier-1.0.1/src/tokenizer.py` & `ArrowTextClassifier-1.0.2/ArrowTextClassifier/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ArrowTextClassifier-1.0.1/src/train.py` & `ArrowTextClassifier-1.0.2/ArrowTextClassifier/train.py`

 * *Files identical despite different names*

