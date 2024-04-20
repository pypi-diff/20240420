# Comparing `tmp/personal_graph-0.1.6.tar.gz` & `tmp/personal_graph-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_graph-0.1.6.tar", max compression
+gzip compressed data, was "personal_graph-0.1.7.tar", max compression
```

## Comparing `personal_graph-0.1.6.tar` & `personal_graph-0.1.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1080 2024-03-13 05:55:36.893450 personal_graph-0.1.6/LICENSE
--rw-r--r--   0        0        0     8661 2024-03-30 12:39:30.387205 personal_graph-0.1.6/README.md
--rw-r--r--   0        0        0       54 2024-04-08 09:45:51.825318 personal_graph-0.1.6/personal_graph/__init__.py
--rw-r--r--   0        0        0    25676 2024-04-18 09:40:51.239348 personal_graph-0.1.6/personal_graph/database.py
--rw-r--r--   0        0        0      903 2024-04-08 05:20:20.734143 personal_graph-0.1.6/personal_graph/embeddings.py
--rw-r--r--   0        0        0     6031 2024-04-17 11:56:47.270908 personal_graph-0.1.6/personal_graph/graph.py
--rw-r--r--   0        0        0      142 2024-04-08 05:20:20.734143 personal_graph-0.1.6/personal_graph/ml.py
--rw-r--r--   0        0        0     1797 2024-04-12 11:09:18.207085 personal_graph-0.1.6/personal_graph/models.py
--rw-r--r--   0        0        0     4894 2024-04-18 09:40:51.239348 personal_graph-0.1.6/personal_graph/natural.py
--rw-r--r--   0        0        0     1161 2024-04-17 11:56:47.274908 personal_graph-0.1.6/personal_graph/retriever.py
--rw-r--r--   0        0        0       52 2024-04-08 05:20:20.734143 personal_graph-0.1.6/personal_graph/sql/delete-edge-embedding.sql
--rw-r--r--   0        0        0       48 2024-04-08 05:20:20.734143 personal_graph-0.1.6/personal_graph/sql/delete-edge.sql
--rw-r--r--   0        0        0       45 2024-04-08 05:20:20.734143 personal_graph-0.1.6/personal_graph/sql/delete-node-embedding.sql
--rw-r--r--   0        0        0       30 2024-04-08 05:20:20.734143 personal_graph-0.1.6/personal_graph/sql/delete-node.sql
--rw-r--r--   0        0        0       97 2024-04-12 11:09:18.207085 personal_graph-0.1.6/personal_graph/sql/existing-edge.sql
--rw-r--r--   0        0        0       39 2024-04-08 05:20:20.734143 personal_graph-0.1.6/personal_graph/sql/existing-node.sql
--rw-r--r--   0        0        0       72 2024-04-08 05:20:20.734143 personal_graph-0.1.6/personal_graph/sql/insert-edge-embedding.sql
--rw-r--r--   0        0        0       91 2024-04-12 11:09:18.207085 personal_graph-0.1.6/personal_graph/sql/insert-edge.sql
--rw-r--r--   0        0        0       62 2024-04-08 05:20:20.734143 personal_graph-0.1.6/personal_graph/sql/insert-node-embedding.sql
--rw-r--r--   0        0        0       70 2024-04-12 11:09:18.207085 personal_graph-0.1.6/personal_graph/sql/insert-node.sql
--rw-r--r--   0        0        0     1116 2024-04-12 11:09:18.207085 personal_graph-0.1.6/personal_graph/sql/schema.sql
--rw-r--r--   0        0        0       36 2024-04-08 05:20:20.738142 personal_graph-0.1.6/personal_graph/sql/search-edges-inbound.sql
--rw-r--r--   0        0        0       36 2024-04-08 05:20:20.738142 personal_graph-0.1.6/personal_graph/sql/search-edges-outbound.sql
--rw-r--r--   0        0        0       80 2024-04-08 05:20:20.738142 personal_graph-0.1.6/personal_graph/sql/search-edges.sql
--rw-r--r--   0        0        0      252 2024-04-12 11:09:18.207085 personal_graph-0.1.6/personal_graph/sql/search-node.template
--rw-r--r--   0        0        0      297 2024-04-12 11:09:18.207085 personal_graph-0.1.6/personal_graph/sql/search-where.template
--rw-r--r--   0        0        0      609 2024-04-12 11:09:18.207085 personal_graph-0.1.6/personal_graph/sql/traverse.template
--rw-r--r--   0        0        0       75 2024-04-12 11:09:18.207085 personal_graph-0.1.6/personal_graph/sql/update-node.sql
--rw-r--r--   0        0        0      283 2024-04-12 11:09:18.211085 personal_graph-0.1.6/personal_graph/sql/vector-search-edge.sql
--rw-r--r--   0        0        0      254 2024-04-12 11:09:18.211085 personal_graph-0.1.6/personal_graph/sql/vector-search-node.sql
--rw-r--r--   0        0        0        0 2024-04-08 05:20:20.742142 personal_graph-0.1.6/personal_graph/tests/__init__.py
--rw-r--r--   0        0        0     2455 2024-04-18 09:40:51.239348 personal_graph-0.1.6/personal_graph/tests/conftest.py
--rw-r--r--   0        0        0     3723 2024-04-08 05:20:20.742142 personal_graph-0.1.6/personal_graph/tests/test_database.py
--rw-r--r--   0        0        0     4551 2024-04-12 11:09:18.211085 personal_graph-0.1.6/personal_graph/tests/test_graph.py
--rw-r--r--   0        0        0        0 2024-04-08 05:20:20.746141 personal_graph-0.1.6/personal_graph/tests/test_ml.py
--rw-r--r--   0        0        0     1405 2024-04-12 11:09:18.211085 personal_graph-0.1.6/personal_graph/tests/test_natural.py
--rw-r--r--   0        0        0     1399 2024-04-08 05:20:20.746141 personal_graph-0.1.6/personal_graph/tests/test_visualizers.py
--rw-r--r--   0        0        0     4011 2024-04-17 11:56:47.274908 personal_graph-0.1.6/personal_graph/visualizers.py
--rw-r--r--   0        0        0      996 2024-04-18 09:40:51.243348 personal_graph-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     9864 1970-01-01 00:00:00.000000 personal_graph-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-03-13 05:55:36.893450 personal_graph-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5927 2024-04-20 12:33:56.682697 personal_graph-0.1.7/README.md
+-rw-r--r--   0        0        0       54 2024-04-08 09:45:51.825318 personal_graph-0.1.7/personal_graph/__init__.py
+-rw-r--r--   0        0        0    25676 2024-04-19 11:23:54.423395 personal_graph-0.1.7/personal_graph/database.py
+-rw-r--r--   0        0        0      903 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/embeddings.py
+-rw-r--r--   0        0        0     6031 2024-04-17 11:56:47.270908 personal_graph-0.1.7/personal_graph/graph.py
+-rw-r--r--   0        0        0      142 2024-04-20 09:29:58.161412 personal_graph-0.1.7/personal_graph/ml.py
+-rw-r--r--   0        0        0     1797 2024-04-19 18:12:33.056612 personal_graph-0.1.7/personal_graph/models.py
+-rw-r--r--   0        0        0     4899 2024-04-20 12:33:56.682697 personal_graph-0.1.7/personal_graph/natural.py
+-rw-r--r--   0        0        0     1161 2024-04-17 11:56:47.274908 personal_graph-0.1.7/personal_graph/retriever.py
+-rw-r--r--   0        0        0       52 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/delete-edge-embedding.sql
+-rw-r--r--   0        0        0       48 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/delete-edge.sql
+-rw-r--r--   0        0        0       45 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/delete-node-embedding.sql
+-rw-r--r--   0        0        0       30 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/delete-node.sql
+-rw-r--r--   0        0        0       97 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/existing-edge.sql
+-rw-r--r--   0        0        0       39 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/existing-node.sql
+-rw-r--r--   0        0        0       72 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/insert-edge-embedding.sql
+-rw-r--r--   0        0        0       91 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/insert-edge.sql
+-rw-r--r--   0        0        0       62 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/insert-node-embedding.sql
+-rw-r--r--   0        0        0       70 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/insert-node.sql
+-rw-r--r--   0        0        0     1116 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/schema.sql
+-rw-r--r--   0        0        0       36 2024-04-08 05:20:20.738142 personal_graph-0.1.7/personal_graph/sql/search-edges-inbound.sql
+-rw-r--r--   0        0        0       36 2024-04-08 05:20:20.738142 personal_graph-0.1.7/personal_graph/sql/search-edges-outbound.sql
+-rw-r--r--   0        0        0       80 2024-04-08 05:20:20.738142 personal_graph-0.1.7/personal_graph/sql/search-edges.sql
+-rw-r--r--   0        0        0      252 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/search-node.template
+-rw-r--r--   0        0        0      297 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/search-where.template
+-rw-r--r--   0        0        0      609 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/traverse.template
+-rw-r--r--   0        0        0       75 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/update-node.sql
+-rw-r--r--   0        0        0      283 2024-04-12 11:09:18.211085 personal_graph-0.1.7/personal_graph/sql/vector-search-edge.sql
+-rw-r--r--   0        0        0      254 2024-04-12 11:09:18.211085 personal_graph-0.1.7/personal_graph/sql/vector-search-node.sql
+-rw-r--r--   0        0        0        0 2024-04-08 05:20:20.742142 personal_graph-0.1.7/personal_graph/tests/__init__.py
+-rw-r--r--   0        0        0     2455 2024-04-18 09:40:51.239348 personal_graph-0.1.7/personal_graph/tests/conftest.py
+-rw-r--r--   0        0        0     3723 2024-04-08 05:20:20.742142 personal_graph-0.1.7/personal_graph/tests/test_database.py
+-rw-r--r--   0        0        0     4551 2024-04-12 11:09:18.211085 personal_graph-0.1.7/personal_graph/tests/test_graph.py
+-rw-r--r--   0        0        0        0 2024-04-08 05:20:20.746141 personal_graph-0.1.7/personal_graph/tests/test_ml.py
+-rw-r--r--   0        0        0     1405 2024-04-12 11:09:18.211085 personal_graph-0.1.7/personal_graph/tests/test_natural.py
+-rw-r--r--   0        0        0     1399 2024-04-08 05:20:20.746141 personal_graph-0.1.7/personal_graph/tests/test_visualizers.py
+-rw-r--r--   0        0        0     4011 2024-04-17 11:56:47.274908 personal_graph-0.1.7/personal_graph/visualizers.py
+-rw-r--r--   0        0        0      996 2024-04-20 12:33:56.682697 personal_graph-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     7130 1970-01-01 00:00:00.000000 personal_graph-0.1.7/PKG-INFO
```

### Comparing `personal_graph-0.1.6/LICENSE` & `personal_graph-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/personal_graph/database.py` & `personal_graph-0.1.7/personal_graph/database.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/personal_graph/embeddings.py` & `personal_graph-0.1.7/personal_graph/embeddings.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/personal_graph/graph.py` & `personal_graph-0.1.7/personal_graph/graph.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/personal_graph/models.py` & `personal_graph-0.1.7/personal_graph/models.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/personal_graph/natural.py` & `personal_graph-0.1.7/personal_graph/natural.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 def visualize_knowledge_graph(kg: KnowledgeGraph) -> Digraph:
     dot = Digraph(comment="Knowledge Graph")
 
     # Add nodes
     for node in kg.nodes:
-        dot.node(node.id, node.label, color="black")
+        dot.node(str(node.id), node.label, color="black")
 
     # Add edges
     for edge in kg.edges:
         dot.edge(str(edge.source), str(edge.target), edge.label, color="black")
 
     return dot
```

### Comparing `personal_graph-0.1.6/personal_graph/retriever.py` & `personal_graph-0.1.7/personal_graph/retriever.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/personal_graph/sql/schema.sql` & `personal_graph-0.1.7/personal_graph/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/personal_graph/sql/traverse.template` & `personal_graph-0.1.7/personal_graph/sql/traverse.template`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/personal_graph/tests/conftest.py` & `personal_graph-0.1.7/personal_graph/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/personal_graph/tests/test_database.py` & `personal_graph-0.1.7/personal_graph/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/personal_graph/tests/test_graph.py` & `personal_graph-0.1.7/personal_graph/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/personal_graph/tests/test_natural.py` & `personal_graph-0.1.7/personal_graph/tests/test_natural.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/personal_graph/tests/test_visualizers.py` & `personal_graph-0.1.7/personal_graph/tests/test_visualizers.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/personal_graph/visualizers.py` & `personal_graph-0.1.7/personal_graph/visualizers.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.6/pyproject.toml` & `personal_graph-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "personal-graph"
-version = "0.1.6"
+version = "0.1.7"
 description = "Graph database in LibSQL"
 authors = ["Anubhuti Bhardwaj <anubhutibhardwaj11@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 exclude = [
     { path = "examples/personal-graph.ipynb" }
 ]
```

