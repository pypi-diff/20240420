# Comparing `tmp/flatpack-3.3.5.tar.gz` & `tmp/flatpack-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.3.5.tar", last modified: Fri Apr 19 23:37:19 2024, max compression
+gzip compressed data, was "flatpack-3.3.6.tar", last modified: Fri Apr 19 23:45:37 2024, max compression
```

## Comparing `flatpack-3.3.5.tar` & `flatpack-3.3.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:37:19.330109 flatpack-3.3.5/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.5/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     5243 2024-04-19 23:37:19.329825 flatpack-3.3.5/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     4583 2024-04-19 13:23:47.000000 flatpack-3.3.5/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:37:19.327434 flatpack-3.3.5/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/datasets.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26872 2024-04-19 23:23:50.000000 flatpack-3.3.5/flatpack/main.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/models.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:37:19.329002 flatpack-3.3.5/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.5/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.5/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6293 2024-04-19 23:37:07.000000 flatpack-3.3.5/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:37:19.329431 flatpack-3.3.5/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     5243 2024-04-19 23:37:19.000000 flatpack-3.3.5/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-19 23:37:19.000000 flatpack-3.3.5/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-19 23:37:19.000000 flatpack-3.3.5/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-19 23:37:19.000000 flatpack-3.3.5/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      218 2024-04-19 23:37:19.000000 flatpack-3.3.5/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-19 23:37:19.000000 flatpack-3.3.5/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-19 23:37:19.330173 flatpack-3.3.5/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)      939 2024-04-19 23:37:12.000000 flatpack-3.3.5/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:45:37.754659 flatpack-3.3.6/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.6/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5243 2024-04-19 23:45:37.754373 flatpack-3.3.6/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4583 2024-04-19 13:23:47.000000 flatpack-3.3.6/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:45:37.751879 flatpack-3.3.6/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/datasets.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26884 2024-04-19 23:45:08.000000 flatpack-3.3.6/flatpack/main.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/models.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:45:37.753600 flatpack-3.3.6/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.6/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6394 2024-04-19 23:44:50.000000 flatpack-3.3.6/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:45:37.754047 flatpack-3.3.6/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5243 2024-04-19 23:45:37.000000 flatpack-3.3.6/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-19 23:45:37.000000 flatpack-3.3.6/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-19 23:45:37.000000 flatpack-3.3.6/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-19 23:45:37.000000 flatpack-3.3.6/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      218 2024-04-19 23:45:37.000000 flatpack-3.3.6/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-19 23:45:37.000000 flatpack-3.3.6/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-19 23:45:37.754733 flatpack-3.3.6/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      939 2024-04-19 23:45:29.000000 flatpack-3.3.6/setup.py
```

### Comparing `flatpack-3.3.5/LICENSE` & `flatpack-3.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.5/PKG-INFO` & `flatpack-3.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.5
+Version: 3.3.6
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.3.5/README.md` & `flatpack-3.3.6/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.5/flatpack/datasets.py` & `flatpack-3.3.6/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.5/flatpack/instructions.py` & `flatpack-3.3.6/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.5/flatpack/main.py` & `flatpack-3.3.6/flatpack/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -584,17 +584,17 @@
 
                 try:
                     results = vm.search_vectors(args.query)
                     if results:
                         print("Search results:")
                         for result in results:
                             id = result["id"]
-                            rank = result["rank"]
+                            distance = result["distance"]
                             text = result["text"]
-                            print(f"({rank}) {id}: {text}\n")
+                            print(f"({distance}) {id}: {text}\n")
                     else:
                         print("No results found.")
                 except ValueError as e:
                     print(f"Error: {e}")
                 except Exception as e:
                     print(f"❌ An unexpected error occurred.")
             elif args.command == 'vector-add-pdf':
```

### Comparing `flatpack-3.3.5/flatpack/modules/lstm.py` & `flatpack-3.3.6/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.5/flatpack/modules/rnn.py` & `flatpack-3.3.6/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.5/flatpack/parsers.py` & `flatpack-3.3.6/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.5/flatpack/vector_manager.py` & `flatpack-3.3.6/flatpack/vector_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,23 +77,26 @@
         if not hasattr(self, 'index') or self.index is None:
             raise ValueError("Vector index is not available.")
 
         query_embedding = self.model.encode([query_text])[0]
         query_np = np.array(query_embedding, dtype=np.float32).reshape(1, -1)
         extended_top_k = min(top_k * 3, len(self.metadata))
         distances, indices = self.index.search(query_np, extended_top_k)
+
+        ranked_results = sorted(zip(distances[0], indices[0]), key=lambda x: x[0])
+
         results = []
         seen_hashes = set()
-        for idx in indices.flatten():
+        for distance, idx in ranked_results:
             if idx < len(self.metadata):
                 metadata_entry = self.metadata[idx]
                 text_hash = metadata_entry["hash"]
                 text = metadata_entry["text"]
                 if text_hash not in seen_hashes:
-                    results.append({"id": text_hash, "rank": idx, "text": text})
+                    results.append({"id": text_hash, "distance": distance, "text": text})
                     seen_hashes.add(text_hash)
                 if len(results) == top_k:
                     break
         return results
 
     def _process_text_and_add(self, text):
         if not isinstance(text, str):
```

### Comparing `flatpack-3.3.5/flatpack.egg-info/PKG-INFO` & `flatpack-3.3.6/flatpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.5
+Version: 3.3.6
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.3.5/setup.py` & `flatpack-3.3.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.3.5",
+    version="3.3.6",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.1",
```

