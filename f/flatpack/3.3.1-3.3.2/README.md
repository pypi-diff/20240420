# Comparing `tmp/flatpack-3.3.1.tar.gz` & `tmp/flatpack-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.3.1.tar", last modified: Thu Apr 18 10:05:02 2024, max compression
+gzip compressed data, was "flatpack-3.3.2.tar", last modified: Fri Apr 19 09:07:02 2024, max compression
```

## Comparing `flatpack-3.3.1.tar` & `flatpack-3.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-18 10:05:02.500169 flatpack-3.3.1/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.1/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     5089 2024-04-18 10:05:02.499764 flatpack-3.3.1/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     4456 2024-04-16 19:54:33.000000 flatpack-3.3.1/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-18 10:05:02.496545 flatpack-3.3.1/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/datasets.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26139 2024-04-18 10:04:30.000000 flatpack-3.3.1/flatpack/main.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/models.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-18 10:05:02.498917 flatpack-3.3.1/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.1/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     3952 2024-04-16 19:15:27.000000 flatpack-3.3.1/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-18 10:05:02.499296 flatpack-3.3.1/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     5089 2024-04-18 10:05:02.000000 flatpack-3.3.1/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-18 10:05:02.000000 flatpack-3.3.1/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-18 10:05:02.000000 flatpack-3.3.1/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-18 10:05:02.000000 flatpack-3.3.1/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      206 2024-04-18 10:05:02.000000 flatpack-3.3.1/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-18 10:05:02.000000 flatpack-3.3.1/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-18 10:05:02.500378 flatpack-3.3.1/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)      916 2024-04-18 10:03:35.000000 flatpack-3.3.1/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 09:07:02.003759 flatpack-3.3.2/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.2/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5089 2024-04-19 09:07:02.003428 flatpack-3.3.2/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4456 2024-04-16 19:54:33.000000 flatpack-3.3.2/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 09:07:02.000175 flatpack-3.3.2/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/datasets.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26284 2024-04-19 09:06:10.000000 flatpack-3.3.2/flatpack/main.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/models.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 09:07:02.002647 flatpack-3.3.2/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.2/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4020 2024-04-19 09:03:52.000000 flatpack-3.3.2/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 09:07:02.003041 flatpack-3.3.2/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5089 2024-04-19 09:07:01.000000 flatpack-3.3.2/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-19 09:07:01.000000 flatpack-3.3.2/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-19 09:07:01.000000 flatpack-3.3.2/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-19 09:07:01.000000 flatpack-3.3.2/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      206 2024-04-19 09:07:01.000000 flatpack-3.3.2/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-19 09:07:01.000000 flatpack-3.3.2/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-19 09:07:02.003836 flatpack-3.3.2/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      916 2024-04-19 09:06:34.000000 flatpack-3.3.2/setup.py
```

### Comparing `flatpack-3.3.1/LICENSE` & `flatpack-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.1/PKG-INFO` & `flatpack-3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.1
+Version: 3.3.2
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.3.1/README.md` & `flatpack-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.1/flatpack/datasets.py` & `flatpack-3.3.2/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.1/flatpack/instructions.py` & `flatpack-3.3.2/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.1/flatpack/main.py` & `flatpack-3.3.2/flatpack/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -570,14 +570,18 @@
 
             fpk_get_api_key()
 
             if args.command == 'vector-add-texts':
                 vm.add_texts(args.texts)
                 print(f"Added {len(args.texts)} texts to the database.")
             elif args.command == 'vector-search':
+                if not vm.is_index_ready():
+                    print("Vector index is not ready. Skipping search.")
+                    return
+
                 try:
                     results = vm.search_vectors(args.query)
                     if results:
                         print("Search results:")
                         for result in results:
                             id = result["id"]
                             rank = result["rank"]
```

### Comparing `flatpack-3.3.1/flatpack/modules/lstm.py` & `flatpack-3.3.2/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.1/flatpack/modules/rnn.py` & `flatpack-3.3.2/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.1/flatpack/parsers.py` & `flatpack-3.3.2/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.1/flatpack/vector_manager.py` & `flatpack-3.3.2/flatpack/vector_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 
     def _initialize_index(self):
         index = faiss.IndexFlatL2(VECTOR_DIMENSION)
         if os.path.exists(INDEX_FILE):
             index = faiss.read_index(INDEX_FILE)
         return index
 
+    def is_index_ready(self):
+        return self.index.ntotal > 0
+
     def _load_metadata(self):
         if not os.path.exists(METADATA_FILE):
             return [], set()
         with open(METADATA_FILE, 'r') as file:
             metadata = [json.loads(line) for line in file]
         hash_set = {entry['hash'] for entry in metadata}
         return metadata, hash_set
```

### Comparing `flatpack-3.3.1/flatpack.egg-info/PKG-INFO` & `flatpack-3.3.2/flatpack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.1
+Version: 3.3.2
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.3.1/setup.py` & `flatpack-3.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.3.1",
+    version="3.3.2",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.1",
```

