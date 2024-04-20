# Comparing `tmp/indexify_langchain-0.0.8.tar.gz` & `tmp/indexify_langchain-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexify_langchain-0.0.8.tar", max compression
+gzip compressed data, was "indexify_langchain-0.0.9.tar", max compression
```

## Comparing `indexify_langchain-0.0.8.tar` & `indexify_langchain-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2066 2024-02-17 00:13:15.580273 indexify_langchain-0.0.8/README.md
--rw-r--r--   0        0        0       92 2024-02-17 00:13:15.580273 indexify_langchain-0.0.8/indexify_langchain/__init__.py
--rw-r--r--   0        0        0     1893 2024-02-17 00:13:15.580273 indexify_langchain-0.0.8/indexify_langchain/retriever.py
--rw-r--r--   0        0        0      406 2024-02-17 00:13:15.580273 indexify_langchain-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2543 1970-01-01 00:00:00.000000 indexify_langchain-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2066 2024-02-17 20:26:27.826709 indexify_langchain-0.0.9/README.md
+-rw-r--r--   0        0        0       93 2024-02-17 20:26:27.826709 indexify_langchain-0.0.9/indexify_langchain/__init__.py
+-rw-r--r--   0        0        0     1863 2024-02-17 20:26:27.826709 indexify_langchain-0.0.9/indexify_langchain/retriever.py
+-rw-r--r--   0        0        0      406 2024-02-17 20:26:27.826709 indexify_langchain-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2543 1970-01-01 00:00:00.000000 indexify_langchain-0.0.9/PKG-INFO
```

### Comparing `indexify_langchain-0.0.8/README.md` & `indexify_langchain-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `indexify_langchain-0.0.8/indexify_langchain/retriever.py` & `indexify_langchain-0.0.9/indexify_langchain/retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,11 +52,9 @@
             "name": self.params["name"],
         }
 
         results = self.client.search_index(**args)
 
         final_results = []
         for r in results:
-            final_results.append(
-                Document(page_content=r["text"], metadata=r["labels"])
-            )
+            final_results.append(Document(page_content=r["text"], metadata=r["labels"]))
         return final_results
```

### Comparing `indexify_langchain-0.0.8/PKG-INFO` & `indexify_langchain-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indexify-langchain
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: Vijay Parthasarathy
 Author-email: vijay2win@gmail.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

