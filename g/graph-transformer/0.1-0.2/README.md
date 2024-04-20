# Comparing `tmp/graph-transformer-0.1.tar.gz` & `tmp/graph-transformer-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph-transformer-0.1.tar", last modified: Mon Jan 30 16:09:51 2023, max compression
+gzip compressed data, was "graph-transformer-0.2.tar", last modified: Sat Apr 20 10:31:04 2024, max compression
```

## Comparing `graph-transformer-0.1.tar` & `graph-transformer-0.2.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0 pc        (1000) pc        (1000)        0 2023-01-30 16:09:51.198157 graph-transformer-0.1/
--rwxrwxrwx   0 pc        (1000) pc        (1000)      752 2023-01-30 16:09:51.198316 graph-transformer-0.1/PKG-INFO
--rwxrwxrwx   0 pc        (1000) pc        (1000)     1260 2023-01-30 16:07:05.000000 graph-transformer-0.1/README.md
-drwxrwxrwx   0 pc        (1000) pc        (1000)        0 2023-01-30 16:09:51.195466 graph-transformer-0.1/graph_transformer/
--rwxrwxrwx   0 pc        (1000) pc        (1000)       75 2023-01-30 14:37:03.000000 graph-transformer-0.1/graph_transformer/__init__.py
--rwxrwxrwx   0 pc        (1000) pc        (1000)     6810 2023-01-30 14:15:34.000000 graph-transformer-0.1/graph_transformer/graph_transformer_model.py
-drwxrwxrwx   0 pc        (1000) pc        (1000)        0 2023-01-30 16:09:51.197828 graph-transformer-0.1/graph_transformer.egg-info/
--rwxrwxrwx   0 pc        (1000) pc        (1000)      752 2023-01-30 16:09:51.000000 graph-transformer-0.1/graph_transformer.egg-info/PKG-INFO
--rwxrwxrwx   0 pc        (1000) pc        (1000)      307 2023-01-30 16:09:51.000000 graph-transformer-0.1/graph_transformer.egg-info/SOURCES.txt
--rwxrwxrwx   0 pc        (1000) pc        (1000)        1 2023-01-30 16:09:51.000000 graph-transformer-0.1/graph_transformer.egg-info/dependency_links.txt
--rwxrwxrwx   0 pc        (1000) pc        (1000)       22 2023-01-30 16:09:51.000000 graph-transformer-0.1/graph_transformer.egg-info/requires.txt
--rwxrwxrwx   0 pc        (1000) pc        (1000)        1 2023-01-30 16:09:51.000000 graph-transformer-0.1/graph_transformer.egg-info/top_level.txt
--rwxrwxrwx   0 pc        (1000) pc        (1000)       79 2023-01-30 16:09:51.198657 graph-transformer-0.1/setup.cfg
--rwxrwxrwx   0 pc        (1000) pc        (1000)      940 2023-01-30 16:07:27.000000 graph-transformer-0.1/setup.py
+drwxrwxrwx   0 willy     (1000) willy     (1000)        0 2024-04-20 10:31:04.893285 graph-transformer-0.2/
+-rwxrwxrwx   0 willy     (1000) willy     (1000)     1071 2024-04-20 08:54:16.000000 graph-transformer-0.2/LICENSE.txt
+-rwxrwxrwx   0 willy     (1000) willy     (1000)      791 2024-04-20 10:31:04.892897 graph-transformer-0.2/PKG-INFO
+-rwxrwxrwx   0 willy     (1000) willy     (1000)     1652 2024-04-20 08:54:16.000000 graph-transformer-0.2/README.md
+drwxrwxrwx   0 willy     (1000) willy     (1000)        0 2024-04-20 10:31:04.891262 graph-transformer-0.2/graph_transformer.egg-info/
+-rwxrwxrwx   0 willy     (1000) willy     (1000)      791 2024-04-20 10:31:04.000000 graph-transformer-0.2/graph_transformer.egg-info/PKG-INFO
+-rwxrwxrwx   0 willy     (1000) willy     (1000)      244 2024-04-20 10:31:04.000000 graph-transformer-0.2/graph_transformer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 willy     (1000) willy     (1000)        1 2024-04-20 10:31:04.000000 graph-transformer-0.2/graph_transformer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 willy     (1000) willy     (1000)       22 2024-04-20 10:31:04.000000 graph-transformer-0.2/graph_transformer.egg-info/requires.txt
+-rwxrwxrwx   0 willy     (1000) willy     (1000)        1 2024-04-20 10:31:04.000000 graph-transformer-0.2/graph_transformer.egg-info/top_level.txt
+-rwxrwxrwx   0 willy     (1000) willy     (1000)       79 2024-04-20 10:31:04.895026 graph-transformer-0.2/setup.cfg
+-rwxrwxrwx   0 willy     (1000) willy     (1000)      940 2024-04-20 10:29:15.000000 graph-transformer-0.2/setup.py
```

### Comparing `graph-transformer-0.1/PKG-INFO` & `graph-transformer-0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: graph-transformer
-Version: 0.1
+Version: 0.2
 Summary: This is the implementation of Graph Transformer (https://www.ijcai.org/proceedings/2021/0214.pdf)
 Home-page: https://github.com/willyfh/graph-transformer
+Download-URL: https://github.com/willyfh/graph-transformer/archive/refs/tags/v0.1.tar.gz
 Author: Willy Fitra Hendria
 Author-email: willyfitrahendria@gmail.com
 License: MIT
-Download-URL: https://github.com/willyfh/graph-transformer/archive/refs/tags/v0.1.tar.gz
-Description: UNKNOWN
 Keywords: deep learning,transformers,graph neural networks
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE.txt
+Requires-Dist: torch>=1.6
+Requires-Dist: numpy>=1.8
```

### Comparing `graph-transformer-0.1/README.md` & `graph-transformer-0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # Graph Transformer (IJCAI 2021)
 
+[![python](https://img.shields.io/badge/python-3.8%2B-blue)]() [![pytorch](https://img.shields.io/badge/pytorch-1.6%2B-orange)]() [![Downloads](https://static.pepy.tech/personalized-badge/graph-transformer?period=total&units=international_system&left_color=grey&right_color=green&left_text=PyPI%20Downloads)](https://pepy.tech/project/graph-transformer)
+
 An unofficial implementation of Graph Transformer:<br/>
 Masked Label Prediction: Unified Message Passing Model for Semi-Supervised Classification) - IJCAI 2021 > https://www.ijcai.org/proceedings/2021/0214.pdf
 
 This GNN architecture is implemented based on Section 3.1 (Graph Transformer) in the paper.
 
-I implemented the code by referring to [this repository](https://github.com/lucidrains/graph-transformer-pytorch), but with some modifications to match with the original paper.
+I implemented the code by referring to [this repository](https://github.com/lucidrains/graph-transformer-pytorch), but with some modifications to match with the original published paper in IJCAI 2021.
 
 ![image](https://github.com/willyfh/graph-transformer/blob/main/graph-transformer-architecture.png?raw=true)
 
 ## Installation
 
 ```bash
 pip install graph-transformer
 ```
 ## Usage
 ```python
+import torch
 from graph_transformer import GraphTransformerModel
 
 model = GraphTransformerModel(
         node_dim = 512,
         edge_dim = 512,
         num_blocks = 3, # number of graph transformer blocks
         num_heads = 8,
```

### Comparing `graph-transformer-0.1/graph_transformer.egg-info/PKG-INFO` & `graph-transformer-0.2/graph_transformer.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: graph-transformer
-Version: 0.1
+Version: 0.2
 Summary: This is the implementation of Graph Transformer (https://www.ijcai.org/proceedings/2021/0214.pdf)
 Home-page: https://github.com/willyfh/graph-transformer
+Download-URL: https://github.com/willyfh/graph-transformer/archive/refs/tags/v0.1.tar.gz
 Author: Willy Fitra Hendria
 Author-email: willyfitrahendria@gmail.com
 License: MIT
-Download-URL: https://github.com/willyfh/graph-transformer/archive/refs/tags/v0.1.tar.gz
-Description: UNKNOWN
 Keywords: deep learning,transformers,graph neural networks
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE.txt
+Requires-Dist: torch>=1.6
+Requires-Dist: numpy>=1.8
```

### Comparing `graph-transformer-0.1/setup.py` & `graph-transformer-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 setup(
     name='graph-transformer',
     description='This is the implementation of Graph Transformer (https://www.ijcai.org/proceedings/2021/0214.pdf)',
     packages=find_packages(include=['graph-transformer']),
-    version='0.1',
+    version='0.2',
     author='Willy Fitra Hendria',
     author_email = 'willyfitrahendria@gmail.com',
     url = 'https://github.com/willyfh/graph-transformer',
     download_url = 'https://github.com/willyfh/graph-transformer/archive/refs/tags/v0.1.tar.gz',
     keywords = ['deep learning','transformers','graph neural networks'],
     license='MIT',
     install_requires=['torch>=1.6', 'numpy>=1.8'],
```

