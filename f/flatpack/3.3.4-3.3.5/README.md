# Comparing `tmp/flatpack-3.3.4.tar.gz` & `tmp/flatpack-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.3.4.tar", last modified: Fri Apr 19 23:34:49 2024, max compression
+gzip compressed data, was "flatpack-3.3.5.tar", last modified: Fri Apr 19 23:37:19 2024, max compression
```

## Comparing `flatpack-3.3.4.tar` & `flatpack-3.3.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:34:49.109372 flatpack-3.3.4/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.4/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     5243 2024-04-19 23:34:49.108795 flatpack-3.3.4/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     4583 2024-04-19 13:23:47.000000 flatpack-3.3.4/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:34:49.104561 flatpack-3.3.4/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.4/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.4/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.4/flatpack/datasets.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.4/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26872 2024-04-19 23:23:50.000000 flatpack-3.3.4/flatpack/main.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.4/flatpack/models.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:34:49.107844 flatpack-3.3.4/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.4/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.4/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.4/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.4/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.4/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6293 2024-04-19 23:34:28.000000 flatpack-3.3.4/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:34:49.108286 flatpack-3.3.4/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     5243 2024-04-19 23:34:49.000000 flatpack-3.3.4/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-19 23:34:49.000000 flatpack-3.3.4/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-19 23:34:49.000000 flatpack-3.3.4/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-19 23:34:49.000000 flatpack-3.3.4/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      218 2024-04-19 23:34:49.000000 flatpack-3.3.4/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-19 23:34:49.000000 flatpack-3.3.4/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-19 23:34:49.109484 flatpack-3.3.4/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)      939 2024-04-19 23:34:39.000000 flatpack-3.3.4/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:37:19.330109 flatpack-3.3.5/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.5/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5243 2024-04-19 23:37:19.329825 flatpack-3.3.5/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4583 2024-04-19 13:23:47.000000 flatpack-3.3.5/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:37:19.327434 flatpack-3.3.5/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/datasets.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26872 2024-04-19 23:23:50.000000 flatpack-3.3.5/flatpack/main.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/models.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:37:19.329002 flatpack-3.3.5/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.5/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6293 2024-04-19 23:37:07.000000 flatpack-3.3.5/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:37:19.329431 flatpack-3.3.5/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5243 2024-04-19 23:37:19.000000 flatpack-3.3.5/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-19 23:37:19.000000 flatpack-3.3.5/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-19 23:37:19.000000 flatpack-3.3.5/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-19 23:37:19.000000 flatpack-3.3.5/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      218 2024-04-19 23:37:19.000000 flatpack-3.3.5/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-19 23:37:19.000000 flatpack-3.3.5/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-19 23:37:19.330173 flatpack-3.3.5/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      939 2024-04-19 23:37:12.000000 flatpack-3.3.5/setup.py
```

### Comparing `flatpack-3.3.4/LICENSE` & `flatpack-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.4/PKG-INFO` & `flatpack-3.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.4
+Version: 3.3.5
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.3.4/README.md` & `flatpack-3.3.5/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.4/flatpack/datasets.py` & `flatpack-3.3.5/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.4/flatpack/instructions.py` & `flatpack-3.3.5/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.4/flatpack/main.py` & `flatpack-3.3.5/flatpack/main.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.4/flatpack/modules/lstm.py` & `flatpack-3.3.5/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.4/flatpack/modules/rnn.py` & `flatpack-3.3.5/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.4/flatpack/parsers.py` & `flatpack-3.3.5/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.4/flatpack/vector_manager.py` & `flatpack-3.3.5/flatpack/vector_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
 nltk.download('punkt')
 
 VECTOR_DIMENSION = 384
 INDEX_FILE = "vector.index"
 METADATA_FILE = "metadata.json"
-SENTENCE_CHUNK_SIZE = 1
+SENTENCE_CHUNK_SIZE = 5
 
 
 class VectorManager:
     def __init__(self, model_name='all-MiniLM-L6-v2'):
         self.model = SentenceTransformer(model_name)
         self.index = self._initialize_index()
         self.metadata, self.hash_set = self._load_metadata()
```

### Comparing `flatpack-3.3.4/flatpack.egg-info/PKG-INFO` & `flatpack-3.3.5/flatpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.4
+Version: 3.3.5
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.3.4/setup.py` & `flatpack-3.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.3.4",
+    version="3.3.5",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.1",
```

