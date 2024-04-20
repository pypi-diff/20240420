# Comparing `tmp/safe_store-0.6.6.tar.gz` & `tmp/safe_store-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_store-0.6.6.tar", last modified: Fri Apr 19 19:55:29 2024, max compression
+gzip compressed data, was "safe_store-0.7.0.tar", last modified: Sat Apr 20 00:59:53 2024, max compression
```

## Comparing `safe_store-0.6.6.tar` & `safe_store-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 19:55:29.257962 safe_store-0.6.6/
--rw-rw-rw-   0        0        0    11558 2024-01-25 22:10:12.000000 safe_store-0.6.6/LICENSE
--rw-rw-rw-   0        0        0     7438 2024-04-19 19:55:29.256961 safe_store-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     6333 2024-02-10 19:31:37.000000 safe_store-0.6.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 19:55:29.235927 safe_store-0.6.6/safe_store/
--rw-rw-rw-   0        0        0     3941 2024-01-25 22:10:12.000000 safe_store-0.6.6/safe_store/BM25Vectorizer.py
--rw-rw-rw-   0        0        0      203 2024-01-25 22:10:12.000000 safe_store-0.6.6/safe_store/__init__.py
--rw-rw-rw-   0        0        0     3113 2024-01-25 22:10:12.000000 safe_store-0.6.6/safe_store/document_decomposer.py
--rw-rw-rw-   0        0        0    10902 2024-04-10 19:55:07.000000 safe_store-0.6.6/safe_store/generic_data_loader.py
--rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.6.6/safe_store/knowledge_base.py
--rw-rw-rw-   0        0        0    32340 2024-04-19 19:54:06.000000 safe_store-0.6.6/safe_store/text_vectorizer.py
--rw-rw-rw-   0        0        0      907 2024-04-19 19:53:32.000000 safe_store-0.6.6/safe_store/tfidf_loader.py
--rw-rw-rw-   0        0        0      502 2024-01-25 22:10:12.000000 safe_store-0.6.6/safe_store/utils.py
--rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.6.6/safe_store/word2vec.py
-drwxrwxrwx   0        0        0        0 2024-04-19 19:55:29.255962 safe_store-0.6.6/safe_store.egg-info/
--rw-rw-rw-   0        0        0     7438 2024-04-19 19:55:28.000000 safe_store-0.6.6/safe_store.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2024-04-19 19:55:29.000000 safe_store-0.6.6/safe_store.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 19:55:28.000000 safe_store-0.6.6/safe_store.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2024-04-19 19:55:28.000000 safe_store-0.6.6/safe_store.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-19 19:55:28.000000 safe_store-0.6.6/safe_store.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 19:55:29.258957 safe_store-0.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1601 2024-04-19 19:54:50.000000 safe_store-0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 00:59:53.928565 safe_store-0.7.0/
+-rw-rw-rw-   0        0        0    11558 2024-01-25 22:10:12.000000 safe_store-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     7438 2024-04-20 00:59:53.928043 safe_store-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6333 2024-02-10 19:31:37.000000 safe_store-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 00:59:53.905446 safe_store-0.7.0/safe_store/
+-rw-rw-rw-   0        0        0     3941 2024-01-25 22:10:12.000000 safe_store-0.7.0/safe_store/BM25Vectorizer.py
+-rw-rw-rw-   0        0        0      203 2024-01-25 22:10:12.000000 safe_store-0.7.0/safe_store/__init__.py
+-rw-rw-rw-   0        0        0     3113 2024-01-25 22:10:12.000000 safe_store-0.7.0/safe_store/document_decomposer.py
+-rw-rw-rw-   0        0        0    10919 2024-04-19 23:55:54.000000 safe_store-0.7.0/safe_store/generic_data_loader.py
+-rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.7.0/safe_store/knowledge_base.py
+-rw-rw-rw-   0        0        0    31936 2024-04-20 00:51:59.000000 safe_store-0.7.0/safe_store/text_vectorizer.py
+-rw-rw-rw-   0        0        0     2569 2024-04-20 00:44:17.000000 safe_store-0.7.0/safe_store/tf_idf_vectorizer.py
+-rw-rw-rw-   0        0        0      907 2024-04-19 19:53:32.000000 safe_store-0.7.0/safe_store/tfidf_loader.py
+-rw-rw-rw-   0        0        0      502 2024-01-25 22:10:12.000000 safe_store-0.7.0/safe_store/utils.py
+-rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.7.0/safe_store/word2vec.py
+drwxrwxrwx   0        0        0        0 2024-04-20 00:59:53.926535 safe_store-0.7.0/safe_store.egg-info/
+-rw-rw-rw-   0        0        0     7438 2024-04-20 00:59:53.000000 safe_store-0.7.0/safe_store.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2024-04-20 00:59:53.000000 safe_store-0.7.0/safe_store.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 00:59:53.000000 safe_store-0.7.0/safe_store.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2024-04-20 00:59:53.000000 safe_store-0.7.0/safe_store.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-20 00:59:53.000000 safe_store-0.7.0/safe_store.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 00:59:53.928565 safe_store-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2024-04-20 00:59:43.000000 safe_store-0.7.0/setup.py
```

### Comparing `safe_store-0.6.6/LICENSE` & `safe_store-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_store-0.6.6/PKG-INFO` & `safe_store-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe_store
-Version: 0.6.6
+Version: 0.7.0
 Summary: A library for safe document storage and vectorization.
 Home-page: https://github.com/ParisNeo/safe_store
 Author: ALOUI Saifeddine (ParisNeo)
 Author-email: aloui.seifeddine@email.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `safe_store-0.6.6/README.md` & `safe_store-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `safe_store-0.6.6/safe_store/BM25Vectorizer.py` & `safe_store-0.7.0/safe_store/BM25Vectorizer.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.6.6/safe_store/document_decomposer.py` & `safe_store-0.7.0/safe_store/document_decomposer.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.6.6/safe_store/generic_data_loader.py` & `safe_store-0.7.0/safe_store/generic_data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,11 +279,11 @@
         Args:
             file_path (Path): The path to the text file.
 
         Returns:
             str: The content of the text file.
         """
         # Implementation details omitted for brevity
-        with open(file_path, 'r', encoding='utf-8') as file:
+        with open(file_path, 'r', encoding='utf-8', errors='ignore') as file:
             content = file.read()
         return content
```

### Comparing `safe_store-0.6.6/safe_store/text_vectorizer.py` & `safe_store-0.7.0/safe_store/text_vectorizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pathlib import Path
 import json
 from safe_store.document_decomposer import DocumentDecomposer
 from safe_store.tfidf_loader import TFIDFLoader
 from safe_store.utils import NumpyEncoderDecoder
 from typing import Union, Tuple, List, Dict, Any
 from enum import Enum
+from safe_store.tf_idf_vectorizer import TfidfVectorizer
 
 class VectorizationMethod(Enum):
     MODEL_EMBEDDING = "model_embedding"
     TFIDF_VECTORIZER = "tfidf_vectorizer"
     BM25_VECTORIZER = "bm25_vectorizer"
     SENTENCE_TRANSFORMER_EMBEDDING = "sentense_transformer"
 class VisualizationMethod(Enum):
@@ -111,30 +112,26 @@
             if Path(self.database_file).exists():
                 ASCIIColors.success(f"Database file found : {self.database_file}")
                 try:
                     self.load_from_json()
                 except Exception as ex:
                     ASCIIColors.error("Couldn't load vectorized db.\nMoving to safe mode")
                     if self.vectorization_method==VectorizationMethod.TFIDF_VECTORIZER:
-                        from sklearn.feature_extraction.text import TfidfVectorizer
-
                         self.vectorizer = TfidfVectorizer()
                     elif self.vectorization_method == VectorizationMethod.BM25_VECTORIZER:
                         self.vectorizer = BM25Vectorizer()
                 self.ready = True
             else:
                 ASCIIColors.info(f"No database file found : {self.database_file}")
                 if self.vectorization_method==VectorizationMethod.TFIDF_VECTORIZER:
-                    from sklearn.feature_extraction.text import TfidfVectorizer
                     self.vectorizer = TfidfVectorizer()
                 elif self.vectorization_method == VectorizationMethod.BM25_VECTORIZER:
                     self.vectorizer = BM25Vectorizer()
         else:
             if self.vectorization_method==VectorizationMethod.TFIDF_VECTORIZER:
-                from sklearn.feature_extraction.text import TfidfVectorizer
                 self.vectorizer = TfidfVectorizer()
             elif self.vectorization_method == VectorizationMethod.BM25_VECTORIZER:
                 self.vectorizer = BM25Vectorizer()
 
 
     def show_document(self, query_text: str = None, save_fig_path: str = None, show_interactive_form: bool = False, add_hover_detection: bool = False, add_click_detection: bool = False):
         """
@@ -450,15 +447,15 @@
 
             
         # Generate embeddings for each chunk
         for chunk_id, chunk in self.chunks.items():
             # Store chunk ID, embeddings, and original text
             try:
                 if self.vectorization_method==VectorizationMethod.TFIDF_VECTORIZER:
-                    chunk["embeddings"] = self.vectorizer.transform([chunk["chunk_text"]]).toarray()
+                    chunk["embeddings"] = self.vectorizer.transform([chunk["chunk_text"]])
                 elif self.vectorization_method==VectorizationMethod.BM25_VECTORIZER:
                     chunk["BM25_data"] = (self.vectorizer.doc_term_freqs, self.vectorizer.doc_lengths) 
                 elif self.vectorization_method==VectorizationMethod.SENTENCE_TRANSFORMER_EMBEDDING:
                     chunk["embeddings"] = self.embed(chunk["chunk_text"])
                 else:
                     chunk["embeddings"] = self.model.embed(chunk["chunk_text"])
             except Exception as ex:
@@ -479,25 +476,25 @@
         Args:
             query_text (str): The query text to be embedded.
         Returns:
             Union[np.ndarray, None]: The embedded query text as a numpy array, or None if embedding is not supported.
         """
         # Generate query embeddings
         if self.vectorization_method == VectorizationMethod.TFIDF_VECTORIZER:
-            query_embedding = self.vectorizer.transform([query_text]).toarray()
+            query_embedding = self.vectorizer.transform([query_text])
         elif self.vectorization_method == VectorizationMethod.SENTENCE_TRANSFORMER_EMBEDDING:
             query_embedding = self.embed(query_text)
         elif self.vectorization_method == VectorizationMethod.BM25_VECTORIZER:
             raise Exception("BM25 doesn't use embedding")
         else:
             query_embedding = self.model.embed(query_text)
             if query_embedding is None:
                 ASCIIColors.warning("The model doesn't implement embeddings extraction")
                 self.vectorization_method = VectorizationMethod.TFIDF_VECTORIZER
-                query_embedding = self.vectorizer.transform([query_text]).toarray()
+                query_embedding = self.vectorizer.transform([query_text])
         return query_embedding
 
 
     def __len__(self) -> int:
         """
         Returns the number of chunks in the vector store.
         Returns:
@@ -533,23 +530,19 @@
         Args:
             query (str): The query text.
             top_k (int, optional): The number of most similar texts to retrieve. Default is 3.
         Returns:
             Tuple[List[str], np.ndarray]: A tuple containing a list of the most similar texts and an array of the corresponding similarity scores.
         """
         if self.vectorization_method==VectorizationMethod.TFIDF_VECTORIZER or self.vectorization_method==VectorizationMethod.MODEL_EMBEDDING:
-            from sklearn.metrics.pairwise import cosine_similarity
             similarities = {}
             query_embedding = self.embed_query(query)
             for chunk_id, chunk in self.chunks.items():
-                if type(chunk["embeddings"])==np.ndarray:
-                    similarity = cosine_similarity(query_embedding, chunk["embeddings"])
-                    similarities[chunk_id] = similarity
-                else:
-                    similarities[chunk_id] = 1e10
+                similarity = self.vectorizer.cosine_similarity(query_embedding[0], chunk["embeddings"][0])
+                similarities[chunk_id] = similarity
             # Sort the similarities and retrieve the top-k most similar embeddings
             sorted_similarities = sorted(similarities.items(), key=lambda x: x[1], reverse=True)[:top_k]
 
             # Retrieve the original text associated with the most similar embeddings
             texts = [self.chunks[chunk_id]["chunk_text"] for chunk_id, _ in sorted_similarities]
             document_ids = [self.chunks[chunk_id]["document_id"] for chunk_id, _ in sorted_similarities]
         elif self.vectorization_method==VectorizationMethod.SENTENCE_TRANSFORMER_EMBEDDING:
```

### Comparing `safe_store-0.6.6/safe_store/tfidf_loader.py` & `safe_store-0.7.0/safe_store/tfidf_loader.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.6.6/safe_store.egg-info/PKG-INFO` & `safe_store-0.7.0/safe_store.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe_store
-Version: 0.6.6
+Version: 0.7.0
 Summary: A library for safe document storage and vectorization.
 Home-page: https://github.com/ParisNeo/safe_store
 Author: ALOUI Saifeddine (ParisNeo)
 Author-email: aloui.seifeddine@email.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `safe_store-0.6.6/setup.py` & `safe_store-0.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Package metadata
 NAME = 'safe_store'
 DESCRIPTION = 'A library for safe document storage and vectorization.'
 URL = 'https://github.com/ParisNeo/safe_store'
 AUTHOR = 'ALOUI Saifeddine (ParisNeo)'
 AUTHOR_EMAIL = 'aloui.seifeddine@email.com'
 LICENSE = 'Apache 2.0'
-VERSION = '0.6.6'
+VERSION = '0.7.0'
 
 # Read dependencies from requirements.txt
 with open('requirements.txt', 'r') as req_file:
     INSTALL_REQUIRES = req_file.read().splitlines()
 
 # Packages to include (find_packages() automatically discovers and includes sub-packages)
 PACKAGES = find_packages()
```

