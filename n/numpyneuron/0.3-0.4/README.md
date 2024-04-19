# Comparing `tmp/numpyneuron-0.3.tar.gz` & `tmp/numpyneuron-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpyneuron-0.3.tar", last modified: Fri Apr 19 22:18:29 2024, max compression
+gzip compressed data, was "numpyneuron-0.4.tar", last modified: Fri Apr 19 23:57:24 2024, max compression
```

## Comparing `numpyneuron-0.3.tar` & `numpyneuron-0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 22:18:29.369394 numpyneuron-0.3/
--rw-r--r--   0 jensen     (501) staff       (20)     2605 2024-04-19 22:18:29.369235 numpyneuron-0.3/PKG-INFO
--rw-r--r--   0 jensen     (501) staff       (20)     2469 2024-04-19 21:12:37.000000 numpyneuron-0.3/README.md
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 22:18:29.368250 numpyneuron-0.3/numpyneuron/
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 22:18:29.369092 numpyneuron-0.3/numpyneuron/numpyneuron.egg-info/
--rw-r--r--   0 jensen     (501) staff       (20)     2605 2024-04-19 22:18:29.000000 numpyneuron-0.3/numpyneuron/numpyneuron.egg-info/PKG-INFO
--rw-r--r--   0 jensen     (501) staff       (20)      206 2024-04-19 22:18:29.000000 numpyneuron-0.3/numpyneuron/numpyneuron.egg-info/SOURCES.txt
--rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 22:18:29.000000 numpyneuron-0.3/numpyneuron/numpyneuron.egg-info/dependency_links.txt
--rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 22:18:29.000000 numpyneuron-0.3/numpyneuron/numpyneuron.egg-info/top_level.txt
--rw-r--r--   0 jensen     (501) staff       (20)       38 2024-04-19 22:18:29.369433 numpyneuron-0.3/setup.cfg
--rw-r--r--   0 jensen     (501) staff       (20)      777 2024-04-19 22:18:21.000000 numpyneuron-0.3/setup.py
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 23:57:24.299379 numpyneuron-0.4/
+-rw-r--r--   0 jensen     (501) staff       (20)     2467 2024-04-19 23:57:24.299196 numpyneuron-0.4/PKG-INFO
+-rw-r--r--   0 jensen     (501) staff       (20)     2476 2024-04-19 23:52:58.000000 numpyneuron-0.4/README.md
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 23:57:24.298177 numpyneuron-0.4/numpyneuron/
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 23:57:24.299034 numpyneuron-0.4/numpyneuron/numpyneuron.egg-info/
+-rw-r--r--   0 jensen     (501) staff       (20)     2467 2024-04-19 23:57:24.000000 numpyneuron-0.4/numpyneuron/numpyneuron.egg-info/PKG-INFO
+-rw-r--r--   0 jensen     (501) staff       (20)      206 2024-04-19 23:57:24.000000 numpyneuron-0.4/numpyneuron/numpyneuron.egg-info/SOURCES.txt
+-rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 23:57:24.000000 numpyneuron-0.4/numpyneuron/numpyneuron.egg-info/dependency_links.txt
+-rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 23:57:24.000000 numpyneuron-0.4/numpyneuron/numpyneuron.egg-info/top_level.txt
+-rw-r--r--   0 jensen     (501) staff       (20)       38 2024-04-19 23:57:24.299414 numpyneuron-0.4/setup.cfg
+-rw-r--r--   0 jensen     (501) staff       (20)      634 2024-04-19 23:57:11.000000 numpyneuron-0.4/setup.py
```

### Comparing `numpyneuron-0.3/PKG-INFO` & `numpyneuron-0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: numpyneuron
-Version: 0.3
+Version: 0.4
 Summary: Simple, lightweight neural network framework built in numpy
 Home-page: https://github.com/Jensen-holm/Numpy-Neuron
 Author: Jensen Holm
 Author-email: jensen.dev.01@gmail.com
 Project-URL: Bug Tracker, https://github.com/Jensen-holm/Numpy-Neuron/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Numpy-Neuron
 
 A small, simple neural network framework built using only [numpy](https://numpy.org) and python (duh).
 
 ## Install
 
-`pip install numpy_neuron`
+`pip install numpyneuron`
 
 
 ## Example
 
 ```py
 from sklearn import datasets
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import accuracy_score, precision_score, recall_score
 import numpy as np
-from nn import (
+from numpyneuron import (
     NN,
     Relu,
     Sigmoid,
     CrossEntropyWithLogits,
 )
```

### Comparing `numpyneuron-0.3/README.md` & `numpyneuron-0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 pinned: false
 license: mit
 ---
 
 
 # Numpy-Neuron
 
-A small, simple neural network framework built using only [numpy](https://numpy.org) and python (duh). Check it out on [PyPI](https://pypi.org/project/numpy-neuron/)
+A small, simple neural network framework built using only [numpy](https://numpy.org) and python (duh). Check it out on [PyPI](https://pypi.org/project/numpyneuron/)
 
 ## Install
 
-`pip install numpy-neuron`
+`pip install numpyneuron`
 
 
 ## Example
 
 ```py
 from sklearn import datasets
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import accuracy_score, precision_score, recall_score
 import numpy as np
-from nn import (
+from numpyneuron import (
     NN,
     Relu,
     Sigmoid,
     CrossEntropyWithLogits,
 )
```

### Comparing `numpyneuron-0.3/numpyneuron/numpyneuron.egg-info/PKG-INFO` & `numpyneuron-0.4/numpyneuron/numpyneuron.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: numpyneuron
-Version: 0.3
+Version: 0.4
 Summary: Simple, lightweight neural network framework built in numpy
 Home-page: https://github.com/Jensen-holm/Numpy-Neuron
 Author: Jensen Holm
 Author-email: jensen.dev.01@gmail.com
 Project-URL: Bug Tracker, https://github.com/Jensen-holm/Numpy-Neuron/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Numpy-Neuron
 
 A small, simple neural network framework built using only [numpy](https://numpy.org) and python (duh).
 
 ## Install
 
-`pip install numpy_neuron`
+`pip install numpyneuron`
 
 
 ## Example
 
 ```py
 from sklearn import datasets
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import accuracy_score, precision_score, recall_score
 import numpy as np
-from nn import (
+from numpyneuron import (
     NN,
     Relu,
     Sigmoid,
     CrossEntropyWithLogits,
 )
```

