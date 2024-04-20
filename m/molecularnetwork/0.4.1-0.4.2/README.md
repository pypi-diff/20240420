# Comparing `tmp/molecularnetwork-0.4.1.tar.gz` & `tmp/molecularnetwork-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecularnetwork-0.4.1.tar", last modified: Fri Apr 12 20:31:15 2024, max compression
+gzip compressed data, was "molecularnetwork-0.4.2.tar", last modified: Sat Apr 20 21:14:54 2024, max compression
```

## Comparing `molecularnetwork-0.4.1.tar` & `molecularnetwork-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,22 @@
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 20:31:15.167132 molecularnetwork-0.4.1/
--rw-r--r--   0 manasmahale   (501) staff       (20)     3096 2024-03-14 17:33:16.000000 molecularnetwork-0.4.1/.gitignore
--rw-r--r--   0 manasmahale   (501) staff       (20)     1069 2023-12-23 10:06:00.000000 molecularnetwork-0.4.1/LICENSE
--rw-r--r--   0 manasmahale   (501) staff       (20)     4767 2024-04-12 20:31:15.166875 molecularnetwork-0.4.1/PKG-INFO
--rw-r--r--   0 manasmahale   (501) staff       (20)     4344 2024-04-12 12:25:50.000000 molecularnetwork-0.4.1/README.md
--rw-r--r--   0 manasmahale   (501) staff       (20)   634211 2024-04-04 13:05:55.000000 molecularnetwork-0.4.1/banner.png
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 20:31:15.161643 molecularnetwork-0.4.1/molecularnetwork/
--rw-r--r--   0 manasmahale   (501) staff       (20)       36 2024-03-14 16:51:27.000000 molecularnetwork-0.4.1/molecularnetwork/__init__.py
--rw-r--r--   0 manasmahale   (501) staff       (20)      786 2024-04-12 20:30:01.000000 molecularnetwork-0.4.1/molecularnetwork/featurizer.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     2857 2024-04-12 19:00:24.000000 molecularnetwork-0.4.1/molecularnetwork/graph.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     1142 2024-03-14 16:51:27.000000 molecularnetwork-0.4.1/molecularnetwork/similarity.py
--rw-r--r--   0 manasmahale   (501) staff       (20)      222 2024-03-14 16:51:27.000000 molecularnetwork-0.4.1/molecularnetwork/utils.py
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 20:31:15.166410 molecularnetwork-0.4.1/molecularnetwork.egg-info/
--rw-r--r--   0 manasmahale   (501) staff       (20)     4767 2024-04-12 20:31:15.000000 molecularnetwork-0.4.1/molecularnetwork.egg-info/PKG-INFO
--rw-r--r--   0 manasmahale   (501) staff       (20)      460 2024-04-12 20:31:15.000000 molecularnetwork-0.4.1/molecularnetwork.egg-info/SOURCES.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)        1 2024-04-12 20:31:15.000000 molecularnetwork-0.4.1/molecularnetwork.egg-info/dependency_links.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       28 2024-04-12 20:31:15.000000 molecularnetwork-0.4.1/molecularnetwork.egg-info/requires.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       17 2024-04-12 20:31:15.000000 molecularnetwork-0.4.1/molecularnetwork.egg-info/top_level.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)    28978 2024-04-09 11:48:31.000000 molecularnetwork-0.4.1/net.png
--rw-r--r--   0 manasmahale   (501) staff       (20)       60 2024-03-14 16:49:26.000000 molecularnetwork-0.4.1/requirements.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       38 2024-04-12 20:31:15.167192 molecularnetwork-0.4.1/setup.cfg
--rw-r--r--   0 manasmahale   (501) staff       (20)      660 2024-04-12 20:30:30.000000 molecularnetwork-0.4.1/setup.py
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 20:31:15.166155 molecularnetwork-0.4.1/test/
--rw-rw-r--   0 manasmahale   (501) staff       (20)    86430 2023-03-09 05:52:27.000000 molecularnetwork-0.4.1/test/test.csv
--rw-r--r--   0 manasmahale   (501) staff       (20)   101028 2024-03-14 16:51:27.000000 molecularnetwork-0.4.1/test/test.gpickle
--rw-r--r--   0 manasmahale   (501) staff       (20)      278 2024-03-14 16:51:27.000000 molecularnetwork-0.4.1/test/test.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-20 21:14:54.888521 molecularnetwork-0.4.2/
+-rw-r--r--   0 manasmahale   (501) staff       (20)     3096 2024-03-14 17:33:16.000000 molecularnetwork-0.4.2/.gitignore
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1069 2023-12-23 10:06:00.000000 molecularnetwork-0.4.2/LICENSE
+-rw-r--r--   0 manasmahale   (501) staff       (20)     4767 2024-04-20 21:14:54.888323 molecularnetwork-0.4.2/PKG-INFO
+-rw-r--r--   0 manasmahale   (501) staff       (20)     4344 2024-04-12 12:25:50.000000 molecularnetwork-0.4.2/README.md
+-rw-r--r--   0 manasmahale   (501) staff       (20)   634211 2024-04-04 13:05:55.000000 molecularnetwork-0.4.2/banner.png
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-20 21:14:54.887344 molecularnetwork-0.4.2/molecularnetwork/
+-rw-r--r--   0 manasmahale   (501) staff       (20)       36 2024-03-14 16:51:27.000000 molecularnetwork-0.4.2/molecularnetwork/__init__.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)      820 2024-04-20 20:41:52.000000 molecularnetwork-0.4.2/molecularnetwork/featurizer.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     2625 2024-04-20 20:48:40.000000 molecularnetwork-0.4.2/molecularnetwork/graph.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1026 2024-04-20 21:06:03.000000 molecularnetwork-0.4.2/molecularnetwork/similarity.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)      222 2024-03-14 16:51:27.000000 molecularnetwork-0.4.2/molecularnetwork/utils.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-20 21:14:54.888079 molecularnetwork-0.4.2/molecularnetwork.egg-info/
+-rw-r--r--   0 manasmahale   (501) staff       (20)     4767 2024-04-20 21:14:54.000000 molecularnetwork-0.4.2/molecularnetwork.egg-info/PKG-INFO
+-rw-r--r--   0 manasmahale   (501) staff       (20)      415 2024-04-20 21:14:54.000000 molecularnetwork-0.4.2/molecularnetwork.egg-info/SOURCES.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)        1 2024-04-20 21:14:54.000000 molecularnetwork-0.4.2/molecularnetwork.egg-info/dependency_links.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       28 2024-04-20 21:14:54.000000 molecularnetwork-0.4.2/molecularnetwork.egg-info/requires.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       17 2024-04-20 21:14:54.000000 molecularnetwork-0.4.2/molecularnetwork.egg-info/top_level.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)    28978 2024-04-09 11:48:31.000000 molecularnetwork-0.4.2/net.png
+-rw-r--r--   0 manasmahale   (501) staff       (20)       60 2024-03-14 16:49:26.000000 molecularnetwork-0.4.2/requirements.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       38 2024-04-20 21:14:54.888563 molecularnetwork-0.4.2/setup.cfg
+-rw-r--r--   0 manasmahale   (501) staff       (20)      660 2024-04-20 19:02:40.000000 molecularnetwork-0.4.2/setup.py
```

### Comparing `molecularnetwork-0.4.1/.gitignore` & `molecularnetwork-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.4.1/LICENSE` & `molecularnetwork-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.4.1/PKG-INFO` & `molecularnetwork-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularnetwork
-Version: 0.4.1
+Version: 0.4.2
 Summary: A package for creating molecular networks based on molecular features and similarities.
 Home-page: https://github.com/Manas02/molecularnetwork
 Author: Manas Mahale
 Author-email: manas.m.mahale@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `molecularnetwork-0.4.1/README.md` & `molecularnetwork-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.4.1/banner.png` & `molecularnetwork-0.4.2/banner.png`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.4.1/molecularnetwork/graph.py` & `molecularnetwork-0.4.2/molecularnetwork/graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,30 +38,28 @@
         nodes = range(num_nodes)
         weighted_nodes = [
             (
                 node,
                 {
                     "smiles": smiles_list[node],
                     "categorical_label": str(value),
-                    "fp": np.array(model_fps[node])
+                    "fp": np.array(model_fps[node].ToList())
                 },
             )
             for node, value in zip(nodes, classes)
         ]
         self.graph.add_nodes_from(weighted_nodes)
 
     def _add_edges(self, fps):
         num_nodes = len(fps)
         for i in range(num_nodes):
             for j in range(i + 1, num_nodes):
                 sim_val = self._calculate_similarity(fps[i], fps[j])
                 if sim_val > self.sim_threshold:
-                    # Check if nodes are from same class or not (True if nodes are from same class)
-                    same_class = self.graph.nodes[i]['categorical_label'] == self.graph.nodes[j]['categorical_label']
-                    self.graph.add_edge(i, j, similarity=sim_val, same_class=same_class)
+                    self.graph.add_edge(i, j, similarity=sim_val)
 
     def _calculate_similarity(self, fp1, fp2):
         return self.similarity_calculator.calculate_similarity(fp1, fp2)
 
     def create_graph(self, smiles_list, classes=None):
         self._create_graph(smiles_list, classes)
         return self.graph
```

### Comparing `molecularnetwork-0.4.1/molecularnetwork/similarity.py` & `molecularnetwork-0.4.2/molecularnetwork/similarity.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,16 @@
         self.sim_metric = sim_metric
         self.metrics = {
             "asymmetric": DataStructs.AsymmetricSimilarity,
             "braunblanquet": DataStructs.BraunBlanquetSimilarity,
             "cosine": DataStructs.CosineSimilarity,
             "dice": DataStructs.DiceSimilarity,
             "kulczynski": DataStructs.KulczynskiSimilarity,
-            "mcconnaughey": DataStructs.McConnaugheySimilarity,
             "onbit": DataStructs.OnBitSimilarity,
             "rogotgoldberg": DataStructs.RogotGoldbergSimilarity,
-            "russel": DataStructs.RusselSimilarity,
             "sokal": DataStructs.SokalSimilarity,
             "tanimoto": DataStructs.TanimotoSimilarity,
             "tversky": lambda m1, m2: DataStructs.TverskySimilarity(
                 m1, m2, a=0.2, b=0.8
             ),
         }
```

### Comparing `molecularnetwork-0.4.1/molecularnetwork.egg-info/PKG-INFO` & `molecularnetwork-0.4.2/molecularnetwork.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularnetwork
-Version: 0.4.1
+Version: 0.4.2
 Summary: A package for creating molecular networks based on molecular features and similarities.
 Home-page: https://github.com/Manas02/molecularnetwork
 Author: Manas Mahale
 Author-email: manas.m.mahale@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `molecularnetwork-0.4.1/net.png` & `molecularnetwork-0.4.2/net.png`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.4.1/setup.py` & `molecularnetwork-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="molecularnetwork",
-    version="0.4.1",
+    version="0.4.2",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "networkx",
         "rdkit",
         "joblib",
     ],
```

