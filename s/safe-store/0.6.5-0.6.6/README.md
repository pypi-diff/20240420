# Comparing `tmp/safe_store-0.6.5.tar.gz` & `tmp/safe_store-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_store-0.6.5.tar", last modified: Sun Apr 14 23:43:44 2024, max compression
+gzip compressed data, was "safe_store-0.6.6.tar", last modified: Fri Apr 19 19:55:29 2024, max compression
```

## Comparing `safe_store-0.6.5.tar` & `safe_store-0.6.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 23:43:44.338821 safe_store-0.6.5/
--rw-rw-rw-   0        0        0    11558 2024-01-25 22:10:12.000000 safe_store-0.6.5/LICENSE
--rw-rw-rw-   0        0        0     7438 2024-04-14 23:43:44.337820 safe_store-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     6333 2024-02-10 19:31:37.000000 safe_store-0.6.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 23:43:44.305801 safe_store-0.6.5/safe_store/
--rw-rw-rw-   0        0        0     3941 2024-01-25 22:10:12.000000 safe_store-0.6.5/safe_store/BM25Vectorizer.py
--rw-rw-rw-   0        0        0      203 2024-01-25 22:10:12.000000 safe_store-0.6.5/safe_store/__init__.py
--rw-rw-rw-   0        0        0     3113 2024-01-25 22:10:12.000000 safe_store-0.6.5/safe_store/document_decomposer.py
--rw-rw-rw-   0        0        0    10902 2024-04-10 19:55:07.000000 safe_store-0.6.5/safe_store/generic_data_loader.py
--rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.6.5/safe_store/knowledge_base.py
--rw-rw-rw-   0        0        0    32144 2024-04-14 23:14:39.000000 safe_store-0.6.5/safe_store/text_vectorizer.py
--rw-rw-rw-   0        0        0      899 2024-01-25 22:10:12.000000 safe_store-0.6.5/safe_store/tfidf_loader.py
--rw-rw-rw-   0        0        0      502 2024-01-25 22:10:12.000000 safe_store-0.6.5/safe_store/utils.py
--rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.6.5/safe_store/word2vec.py
-drwxrwxrwx   0        0        0        0 2024-04-14 23:43:44.335899 safe_store-0.6.5/safe_store.egg-info/
--rw-rw-rw-   0        0        0     7438 2024-04-14 23:43:44.000000 safe_store-0.6.5/safe_store.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2024-04-14 23:43:44.000000 safe_store-0.6.5/safe_store.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 23:43:44.000000 safe_store-0.6.5/safe_store.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2024-04-14 23:43:44.000000 safe_store-0.6.5/safe_store.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-14 23:43:44.000000 safe_store-0.6.5/safe_store.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 23:43:44.338821 safe_store-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1601 2024-04-14 23:43:37.000000 safe_store-0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 19:55:29.257962 safe_store-0.6.6/
+-rw-rw-rw-   0        0        0    11558 2024-01-25 22:10:12.000000 safe_store-0.6.6/LICENSE
+-rw-rw-rw-   0        0        0     7438 2024-04-19 19:55:29.256961 safe_store-0.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6333 2024-02-10 19:31:37.000000 safe_store-0.6.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 19:55:29.235927 safe_store-0.6.6/safe_store/
+-rw-rw-rw-   0        0        0     3941 2024-01-25 22:10:12.000000 safe_store-0.6.6/safe_store/BM25Vectorizer.py
+-rw-rw-rw-   0        0        0      203 2024-01-25 22:10:12.000000 safe_store-0.6.6/safe_store/__init__.py
+-rw-rw-rw-   0        0        0     3113 2024-01-25 22:10:12.000000 safe_store-0.6.6/safe_store/document_decomposer.py
+-rw-rw-rw-   0        0        0    10902 2024-04-10 19:55:07.000000 safe_store-0.6.6/safe_store/generic_data_loader.py
+-rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.6.6/safe_store/knowledge_base.py
+-rw-rw-rw-   0        0        0    32340 2024-04-19 19:54:06.000000 safe_store-0.6.6/safe_store/text_vectorizer.py
+-rw-rw-rw-   0        0        0      907 2024-04-19 19:53:32.000000 safe_store-0.6.6/safe_store/tfidf_loader.py
+-rw-rw-rw-   0        0        0      502 2024-01-25 22:10:12.000000 safe_store-0.6.6/safe_store/utils.py
+-rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.6.6/safe_store/word2vec.py
+drwxrwxrwx   0        0        0        0 2024-04-19 19:55:29.255962 safe_store-0.6.6/safe_store.egg-info/
+-rw-rw-rw-   0        0        0     7438 2024-04-19 19:55:28.000000 safe_store-0.6.6/safe_store.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2024-04-19 19:55:29.000000 safe_store-0.6.6/safe_store.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 19:55:28.000000 safe_store-0.6.6/safe_store.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2024-04-19 19:55:28.000000 safe_store-0.6.6/safe_store.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-19 19:55:28.000000 safe_store-0.6.6/safe_store.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 19:55:29.258957 safe_store-0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2024-04-19 19:54:50.000000 safe_store-0.6.6/setup.py
```

### Comparing `safe_store-0.6.5/LICENSE` & `safe_store-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_store-0.6.5/PKG-INFO` & `safe_store-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe_store
-Version: 0.6.5
+Version: 0.6.6
 Summary: A library for safe document storage and vectorization.
 Home-page: https://github.com/ParisNeo/safe_store
 Author: ALOUI Saifeddine (ParisNeo)
 Author-email: aloui.seifeddine@email.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `safe_store-0.6.5/README.md` & `safe_store-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `safe_store-0.6.5/safe_store/BM25Vectorizer.py` & `safe_store-0.6.6/safe_store/BM25Vectorizer.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.6.5/safe_store/document_decomposer.py` & `safe_store-0.6.6/safe_store/document_decomposer.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.6.5/safe_store/generic_data_loader.py` & `safe_store-0.6.6/safe_store/generic_data_loader.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.6.5/safe_store/text_vectorizer.py` & `safe_store-0.6.6/safe_store/text_vectorizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from pipmaster import PackageManager
 pm = PackageManager()
-from sklearn.feature_extraction.text import TfidfVectorizer
 from ascii_colors import ASCIIColors, trace_exception
-from sklearn.metrics.pairwise import cosine_similarity
 from safe_store.BM25Vectorizer import BM25Vectorizer, split_string  # Import BM25Vectorizer
 import numpy as np
 from pathlib import Path
 import json
 from safe_store.document_decomposer import DocumentDecomposer
 from safe_store.tfidf_loader import TFIDFLoader
 from safe_store.utils import NumpyEncoderDecoder
@@ -113,26 +111,30 @@
             if Path(self.database_file).exists():
                 ASCIIColors.success(f"Database file found : {self.database_file}")
                 try:
                     self.load_from_json()
                 except Exception as ex:
                     ASCIIColors.error("Couldn't load vectorized db.\nMoving to safe mode")
                     if self.vectorization_method==VectorizationMethod.TFIDF_VECTORIZER:
+                        from sklearn.feature_extraction.text import TfidfVectorizer
+
                         self.vectorizer = TfidfVectorizer()
                     elif self.vectorization_method == VectorizationMethod.BM25_VECTORIZER:
                         self.vectorizer = BM25Vectorizer()
                 self.ready = True
             else:
                 ASCIIColors.info(f"No database file found : {self.database_file}")
                 if self.vectorization_method==VectorizationMethod.TFIDF_VECTORIZER:
+                    from sklearn.feature_extraction.text import TfidfVectorizer
                     self.vectorizer = TfidfVectorizer()
                 elif self.vectorization_method == VectorizationMethod.BM25_VECTORIZER:
                     self.vectorizer = BM25Vectorizer()
         else:
             if self.vectorization_method==VectorizationMethod.TFIDF_VECTORIZER:
+                from sklearn.feature_extraction.text import TfidfVectorizer
                 self.vectorizer = TfidfVectorizer()
             elif self.vectorization_method == VectorizationMethod.BM25_VECTORIZER:
                 self.vectorizer = BM25Vectorizer()
 
 
     def show_document(self, query_text: str = None, save_fig_path: str = None, show_interactive_form: bool = False, add_hover_detection: bool = False, add_click_detection: bool = False):
         """
@@ -531,14 +533,15 @@
         Args:
             query (str): The query text.
             top_k (int, optional): The number of most similar texts to retrieve. Default is 3.
         Returns:
             Tuple[List[str], np.ndarray]: A tuple containing a list of the most similar texts and an array of the corresponding similarity scores.
         """
         if self.vectorization_method==VectorizationMethod.TFIDF_VECTORIZER or self.vectorization_method==VectorizationMethod.MODEL_EMBEDDING:
+            from sklearn.metrics.pairwise import cosine_similarity
             similarities = {}
             query_embedding = self.embed_query(query)
             for chunk_id, chunk in self.chunks.items():
                 if type(chunk["embeddings"])==np.ndarray:
                     similarity = cosine_similarity(query_embedding, chunk["embeddings"])
                     similarities[chunk_id] = similarity
                 else:
```

### Comparing `safe_store-0.6.5/safe_store/tfidf_loader.py` & `safe_store-0.6.6/safe_store/tfidf_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from sklearn.feature_extraction.text import TfidfVectorizer
 import numpy
 
 class TFIDFLoader:
     @staticmethod
     def create_vectorizer_from_dict(tfidf_info):
+        from sklearn.feature_extraction.text import TfidfVectorizer
         vectorizer = TfidfVectorizer(**tfidf_info['params'])
         vectorizer.ngram_range = tuple(vectorizer.ngram_range)
         vectorizer.vocabulary_ = tfidf_info['vocabulary']
         vectorizer.idf_ = tfidf_info['idf_values']
         dt = vectorizer.dtype[8:-2]
         vectorizer.dtype = eval(dt)
         return vectorizer
```

### Comparing `safe_store-0.6.5/safe_store.egg-info/PKG-INFO` & `safe_store-0.6.6/safe_store.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe_store
-Version: 0.6.5
+Version: 0.6.6
 Summary: A library for safe document storage and vectorization.
 Home-page: https://github.com/ParisNeo/safe_store
 Author: ALOUI Saifeddine (ParisNeo)
 Author-email: aloui.seifeddine@email.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `safe_store-0.6.5/setup.py` & `safe_store-0.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Package metadata
 NAME = 'safe_store'
 DESCRIPTION = 'A library for safe document storage and vectorization.'
 URL = 'https://github.com/ParisNeo/safe_store'
 AUTHOR = 'ALOUI Saifeddine (ParisNeo)'
 AUTHOR_EMAIL = 'aloui.seifeddine@email.com'
 LICENSE = 'Apache 2.0'
-VERSION = '0.6.5'
+VERSION = '0.6.6'
 
 # Read dependencies from requirements.txt
 with open('requirements.txt', 'r') as req_file:
     INSTALL_REQUIRES = req_file.read().splitlines()
 
 # Packages to include (find_packages() automatically discovers and includes sub-packages)
 PACKAGES = find_packages()
```

