# Comparing `tmp/pysettrie-1.0.0.tar.gz` & `tmp/pysettrie-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysettrie-1.0.0.tar", last modified: Sat Apr 20 01:42:50 2024, max compression
+gzip compressed data, was "pysettrie-1.0.1.tar", last modified: Sat Apr 20 02:08:08 2024, max compression
```

## Comparing `pysettrie-1.0.0.tar` & `pysettrie-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 01:42:50.225393 pysettrie-1.0.0/
--rw-rw-rw-   0        0        0     7799 2024-04-20 01:00:57.000000 pysettrie-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3268 2024-04-20 01:42:50.225393 pysettrie-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2574 2024-04-20 01:00:57.000000 pysettrie-1.0.0/README.md
--rw-rw-rw-   0        0        0      709 2024-04-20 01:39:57.000000 pysettrie-1.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-20 01:42:50.224394 pysettrie-1.0.0/pysettrie.egg-info/
--rw-rw-rw-   0        0        0     3268 2024-04-20 01:42:50.000000 pysettrie-1.0.0/pysettrie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-20 01:42:50.000000 pysettrie-1.0.0/pysettrie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 01:42:50.000000 pysettrie-1.0.0/pysettrie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-20 01:42:50.000000 pysettrie-1.0.0/pysettrie.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-20 01:42:50.221393 pysettrie-1.0.0/settrie/
--rw-rw-rw-   0        0        0  1178156 2024-04-20 01:42:47.000000 pysettrie-1.0.0/settrie/settrie.cpp
--rw-rw-rw-   0        0        0    41270 2024-04-20 01:00:57.000000 pysettrie-1.0.0/settrie/settrie.pyx
--rw-rw-rw-   0        0        0       42 2024-04-20 01:42:50.226898 pysettrie-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1536 2024-04-20 01:42:37.000000 pysettrie-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 01:42:50.223400 pysettrie-1.0.0/tests/
--rw-rw-rw-   0        0        0    15751 2024-04-20 01:00:57.000000 pysettrie-1.0.0/tests/test_settrie.py
+drwxrwxrwx   0        0        0        0 2024-04-20 02:08:08.779713 pysettrie-1.0.1/
+-rw-rw-rw-   0        0        0     7799 2024-04-20 01:00:57.000000 pysettrie-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3244 2024-04-20 02:08:08.778709 pysettrie-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2550 2024-04-20 01:49:56.000000 pysettrie-1.0.1/README.md
+-rw-rw-rw-   0        0        0      709 2024-04-20 02:07:48.000000 pysettrie-1.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-20 02:08:08.777704 pysettrie-1.0.1/pysettrie.egg-info/
+-rw-rw-rw-   0        0        0     3244 2024-04-20 02:08:08.000000 pysettrie-1.0.1/pysettrie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-04-20 02:08:08.000000 pysettrie-1.0.1/pysettrie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 02:08:08.000000 pysettrie-1.0.1/pysettrie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-20 02:08:08.000000 pysettrie-1.0.1/pysettrie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 02:08:08.776198 pysettrie-1.0.1/settrie/
+-rw-rw-rw-   0        0        0  1178156 2024-04-20 02:08:05.000000 pysettrie-1.0.1/settrie/settrie.cpp
+-rw-rw-rw-   0        0        0    41270 2024-04-20 01:00:57.000000 pysettrie-1.0.1/settrie/settrie.pyx
+-rw-rw-rw-   0        0        0       42 2024-04-20 02:08:08.779713 pysettrie-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1536 2024-04-20 02:07:39.000000 pysettrie-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 02:08:08.776198 pysettrie-1.0.1/tests/
+-rw-rw-rw-   0        0        0    19667 2024-04-20 02:00:45.000000 pysettrie-1.0.1/tests/test_settrie.py
```

### Comparing `pysettrie-1.0.0/LICENSE` & `pysettrie-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysettrie-1.0.0/PKG-INFO` & `pysettrie-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysettrie
-Version: 1.0.0
+Version: 1.0.1
 Summary: pysettrie package
 Home-page: https://github.com/GregoryMorse/pysettrie
 Author: Gregory Morse and Márton Miháltz
 Author-email: Gregory Morse <gregory.morse@live.com>, Márton Miháltz <mihaltz.marton@nytud.mta.hu>
 Project-URL: Homepage, https://github.com/GregoryMorse/pysettrie
 Project-URL: Issues, https://github.com/GregoryMorse/pysettrie/issues
 Classifier: Programming Language :: Python :: 3
@@ -12,17 +12,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pysettrie
 =========
-[![Build Status](https://travis-ci.org/mmihaltz/pysettrie.svg)](https://travis-ci.org/mmihaltz/pysettrie)
+[![Build Status](https://travis-ci.org/GregoryMorse/pysettrie.svg)](https://travis-ci.org/GregoryMorse/pysettrie)
 
-https://github.com/mmihaltz/pysettrie
+https://github.com/GregoryMorse/pysettrie
 
 pysettrie is a python3 package that provides support for efficient storage and querying of sets of sets 
 using the trie data structure, supporting operations like finding all the supersets/subsets of a given set 
 from a collection of sets.
 The original motivation for this module was to provide efficient search for supersets of sets of feature-value pairs in our natural language parser project (e.g. matching nouns against verb argument positions).
 
 The following classes are included: 
@@ -30,22 +30,18 @@
 - SetTrieMap: mapping container using sets as keys; supports efficient operations like SetTrie but also stores values associated to the key sets.
 - SetTrieMultiMap: like SetTrieMap, but supports multiple values associated to each key.
 
 For further information, please see [documentation](docs/build/html/index.html)
 
 Module test_settrie.py contains unittests for all the containers.
 
-Author: Márton Miháltz 
+Authors: Gregory Morse and Márton Miháltz 
 [https://sites.google.com/site/mmihaltz/](https://sites.google.com/site/mmihaltz/)
 
-This package depends on the [sortedcollection](http://grantjenks.com/docs/sortedcontainers/) module.
 One recommended way to install (tested on Ubuntu):
-```
-sudo pip3 install sortedcontainers
-```
 If you don't have pip3:
 ```
 sudo apt-get install python3-setuptools
 sudo easy_install3 pip
 ```
 
 pysettrie is partly based on:
@@ -57,12 +53,14 @@
 - the descriptions of getAllSubSets and getAllSuperSets operations are wrong, would not produce all sub/supersets
 
 See also:
 - http://stackoverflow.com/questions/9353100/quickly-checking-if-set-is-superset-of-stored-sets
 - http://stackoverflow.com/questions/1263524/superset-search?rq=1
 
 Changes:
+* Version 1.0.0:
+  - Some bug fixes, complete Cython translation for improved performance.
 * Version 0.1.3:
   - SetTrieMultiMap.assign() returns number of values associated to key after assignment.
 
 Licensed under the [GNU LESSER GENERAL PUBLIC LICENSE, Version 3](https://www.gnu.org/licenses/lgpl.html).
```

### Comparing `pysettrie-1.0.0/README.md` & `pysettrie-1.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pysettrie
 =========
-[![Build Status](https://travis-ci.org/mmihaltz/pysettrie.svg)](https://travis-ci.org/mmihaltz/pysettrie)
+[![Build Status](https://travis-ci.org/GregoryMorse/pysettrie.svg)](https://travis-ci.org/GregoryMorse/pysettrie)
 
-https://github.com/mmihaltz/pysettrie
+https://github.com/GregoryMorse/pysettrie
 
 pysettrie is a python3 package that provides support for efficient storage and querying of sets of sets 
 using the trie data structure, supporting operations like finding all the supersets/subsets of a given set 
 from a collection of sets.
 The original motivation for this module was to provide efficient search for supersets of sets of feature-value pairs in our natural language parser project (e.g. matching nouns against verb argument positions).
 
 The following classes are included: 
@@ -14,22 +14,18 @@
 - SetTrieMap: mapping container using sets as keys; supports efficient operations like SetTrie but also stores values associated to the key sets.
 - SetTrieMultiMap: like SetTrieMap, but supports multiple values associated to each key.
 
 For further information, please see [documentation](docs/build/html/index.html)
 
 Module test_settrie.py contains unittests for all the containers.
 
-Author: Márton Miháltz 
+Authors: Gregory Morse and Márton Miháltz 
 [https://sites.google.com/site/mmihaltz/](https://sites.google.com/site/mmihaltz/)
 
-This package depends on the [sortedcollection](http://grantjenks.com/docs/sortedcontainers/) module.
 One recommended way to install (tested on Ubuntu):
-```
-sudo pip3 install sortedcontainers
-```
 If you don't have pip3:
 ```
 sudo apt-get install python3-setuptools
 sudo easy_install3 pip
 ```
 
 pysettrie is partly based on:
@@ -41,12 +37,14 @@
 - the descriptions of getAllSubSets and getAllSuperSets operations are wrong, would not produce all sub/supersets
 
 See also:
 - http://stackoverflow.com/questions/9353100/quickly-checking-if-set-is-superset-of-stored-sets
 - http://stackoverflow.com/questions/1263524/superset-search?rq=1
 
 Changes:
+* Version 1.0.0:
+  - Some bug fixes, complete Cython translation for improved performance.
 * Version 0.1.3:
   - SetTrieMultiMap.assign() returns number of values associated to key after assignment.
 
 Licensed under the [GNU LESSER GENERAL PUBLIC LICENSE, Version 3](https://www.gnu.org/licenses/lgpl.html).
```

### Comparing `pysettrie-1.0.0/pyproject.toml` & `pysettrie-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pysettrie"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Gregory Morse", email="gregory.morse@live.com" },
   { name="Márton Miháltz", email="mihaltz.marton@nytud.mta.hu" }
 ]
 description = "pysettrie package"
 readme = "README.md"
 requires-python = ">=3.5"
```

### Comparing `pysettrie-1.0.0/pysettrie.egg-info/PKG-INFO` & `pysettrie-1.0.1/pysettrie.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysettrie
-Version: 1.0.0
+Version: 1.0.1
 Summary: pysettrie package
 Home-page: https://github.com/GregoryMorse/pysettrie
 Author: Gregory Morse and Márton Miháltz
 Author-email: Gregory Morse <gregory.morse@live.com>, Márton Miháltz <mihaltz.marton@nytud.mta.hu>
 Project-URL: Homepage, https://github.com/GregoryMorse/pysettrie
 Project-URL: Issues, https://github.com/GregoryMorse/pysettrie/issues
 Classifier: Programming Language :: Python :: 3
@@ -12,17 +12,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pysettrie
 =========
-[![Build Status](https://travis-ci.org/mmihaltz/pysettrie.svg)](https://travis-ci.org/mmihaltz/pysettrie)
+[![Build Status](https://travis-ci.org/GregoryMorse/pysettrie.svg)](https://travis-ci.org/GregoryMorse/pysettrie)
 
-https://github.com/mmihaltz/pysettrie
+https://github.com/GregoryMorse/pysettrie
 
 pysettrie is a python3 package that provides support for efficient storage and querying of sets of sets 
 using the trie data structure, supporting operations like finding all the supersets/subsets of a given set 
 from a collection of sets.
 The original motivation for this module was to provide efficient search for supersets of sets of feature-value pairs in our natural language parser project (e.g. matching nouns against verb argument positions).
 
 The following classes are included: 
@@ -30,22 +30,18 @@
 - SetTrieMap: mapping container using sets as keys; supports efficient operations like SetTrie but also stores values associated to the key sets.
 - SetTrieMultiMap: like SetTrieMap, but supports multiple values associated to each key.
 
 For further information, please see [documentation](docs/build/html/index.html)
 
 Module test_settrie.py contains unittests for all the containers.
 
-Author: Márton Miháltz 
+Authors: Gregory Morse and Márton Miháltz 
 [https://sites.google.com/site/mmihaltz/](https://sites.google.com/site/mmihaltz/)
 
-This package depends on the [sortedcollection](http://grantjenks.com/docs/sortedcontainers/) module.
 One recommended way to install (tested on Ubuntu):
-```
-sudo pip3 install sortedcontainers
-```
 If you don't have pip3:
 ```
 sudo apt-get install python3-setuptools
 sudo easy_install3 pip
 ```
 
 pysettrie is partly based on:
@@ -57,12 +53,14 @@
 - the descriptions of getAllSubSets and getAllSuperSets operations are wrong, would not produce all sub/supersets
 
 See also:
 - http://stackoverflow.com/questions/9353100/quickly-checking-if-set-is-superset-of-stored-sets
 - http://stackoverflow.com/questions/1263524/superset-search?rq=1
 
 Changes:
+* Version 1.0.0:
+  - Some bug fixes, complete Cython translation for improved performance.
 * Version 0.1.3:
   - SetTrieMultiMap.assign() returns number of values associated to key after assignment.
 
 Licensed under the [GNU LESSER GENERAL PUBLIC LICENSE, Version 3](https://www.gnu.org/licenses/lgpl.html).
```

### Comparing `pysettrie-1.0.0/settrie/settrie.cpp` & `pysettrie-1.0.1/settrie/settrie.cpp`

 * *Files identical despite different names*

### Comparing `pysettrie-1.0.0/settrie/settrie.pyx` & `pysettrie-1.0.1/settrie/settrie.pyx`

 * *Files identical despite different names*

### Comparing `pysettrie-1.0.0/setup.py` & `pysettrie-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 except ImportError :
     raise ImportError("setuptools module required, please go to https://pypi.python.org/pypi/setuptools and follow the instructions for installing setuptools")
 from Cython.Build import cythonize
 
 setup(
     name='pysettrie',
     url='https://github.com/GregoryMorse/pysettrie',
-    version='1.0.0',
+    version='1.0.1',
     author='Gregory Morse and Márton Miháltz',
     description='Efficient storage and querying of sets of sets using the trie data structure',
     packages=['settrie'],
     #install_requires=['sortedcontainers'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

### Comparing `pysettrie-1.0.0/tests/test_settrie.py` & `pysettrie-1.0.1/tests/test_settrie.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Author: Márton Miháltz 
 https://sites.google.com/site/mmihaltz/
 """
 
 import unittest
 from settrie import SetTrie, SetTrieMap, SetTrieMultiMap
 
+#unittest.main(settrie.TestSetTrie())
 
 class TestSetTrie(unittest.TestCase):
   """
   UnitTest for SetTrie class
   """
 
   def setUp(self):
@@ -73,14 +74,15 @@
     self.assertFalse({1, 3, 5, 7} in self.t)
     
   def test_hassuperset(self):
     self.assertTrue(self.t.hassuperset({3, 5}))
     self.assertFalse(self.t.hassuperset({6}))
     self.assertTrue(self.t.hassuperset({1, 2, 4}))
     self.assertFalse(self.t.hassuperset({2, 4, 5} ))
+    self.assertFalse(SetTrie().hassuperset({}))
     
   def test_supersets(self):
     self.assertEqual(self.t.supersets({3, 5}), [{1, 3, 5}, {2, 3, 5}])
     self.assertEqual(self.t.supersets({1, 4}), [{1, 2, 4}, {1, 4}])
     self.assertEqual(self.t.supersets({1, 3, 5}),  [{1, 3, 5}])
     self.assertEqual(self.t.supersets({2}),  [{1, 2, 4}, {2, 3, 5}, {2, 4}])
     self.assertEqual(self.t.supersets({1}),  [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}])
@@ -105,242 +107,321 @@
     self.assertEqual(self.t.subsets({1, 2, 5}), [])
     self.assertEqual(self.t.subsets({1, 4}), [{1, 4}]) # :)   
     self.assertEqual(self.t.subsets({1, 3, 5}), [{1, 3}, {1, 3, 5}])
     self.assertEqual(self.t.subsets({1, 3, 5, 111}), [{1, 3}, {1, 3, 5}])
     self.assertEqual(self.t.subsets({1, 4, 8}), [{1, 4}])
     self.assertEqual(self.t.subsets({2, 3, 4, 5}), [{2, 3, 5}, {2, 4}])
     self.assertEqual(self.t.subsets({2, 3, 5, 6}), [{2, 3, 5}])
+  
+  def test_add_remove(self):
+    self.t.remove({1,3})
+    self.assertEqual(self.t.aslist(), [{1, 2, 4}, {1, 3, 5}, {1, 4}, {2, 3, 5}, {2, 4}])
+    self.t.remove({1,3,5})
+    self.assertEqual(self.t.aslist(), [{1, 2, 4}, {1, 4}, {2, 3, 5}, {2, 4}])
+    self.t.remove({1,4})
+    self.assertEqual(self.t.aslist(), [{1, 2, 4}, {2, 3, 5}, {2, 4}])
+    self.t.remove({1,2,4})
+    self.assertEqual(self.t.aslist(), [{2, 3, 5}, {2, 4}])
+    self.t.remove({2,4})
+    self.assertEqual(self.t.aslist(), [{2, 3, 5}])
+    self.t.remove({2,3,5})
+    self.assertEqual(self.t.aslist(), [])
+    self.assertTrue(self.t.empty())
+    self.t.add({1,3})
+    self.assertEqual(self.t.aslist(), [{1, 3}])
+    self.t.add({1,3,5})
+    self.assertEqual(self.t.aslist(), [{1, 3}, {1, 3, 5}])
+    self.t.add({1,4})
+    self.assertEqual(self.t.aslist(), [{1, 3}, {1, 3, 5}, {1, 4}])
+    self.t.add({1,2,4})
+    self.assertEqual(self.t.aslist(), [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}])
+    self.t.add({2,4})
+    self.assertEqual(self.t.aslist(), [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}, {2, 4}])
+    self.t.add({2,3,5})
+    self.assertEqual(self.t.aslist(), [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}, {2, 3, 5}, {2, 4}])
+  
+  def test_validity(self):
+    import numpy as np
+    r = np.arange(30)
+    t = SetTrie()
+    count = 0
+    for i in range(10000):
+        np.random.shuffle(r)
+        n = r[:np.random.randint(30)]
+        if not n in t: count += 1
+        t.add(n)
+        t.add(n)
+    self.assertEqual(count, len(list(t)))
+    for i in range(100):
+        np.random.shuffle(r)
+        n = r[:np.random.randint(30)]
+        ns, res = set(n), list()
+        for x in t:
+            if x.issubset(ns): res.append(x)
+        self.assertEqual(t.hassubset(ns), not not res)
+        self.assertEqual(list(t.itersubsets(ns)), res)
+        res = list()
+        for x in t:
+            if x.issuperset(ns): res.append(x)
+        self.assertEqual(t.hassuperset(ns), not not res)
+        self.assertEqual(list(t.itersupersets(ns)), res)
+        
+  def test_performance(self):
+    import numpy as np
+    rnd = np.random.RandomState(0)
+    r = np.arange(30)
+    t = SetTrie()
+    for i in range(10000):
+        rnd.shuffle(r)
+        n = r[:rnd.randint(30)]
+        t.add(n)
+        t.add(n)
+    for i in range(10): list(t)
+    for i in range(10000):
+        rnd.shuffle(r)
+        n = r[:rnd.randint(30)]
+        list(t.itersubsets(n))
+        t.hassubset(n)
+        list(t.itersupersets(n))
+        t.hassuperset(n)
+        
+class TestSetTrieRecursion(TestSetTrie):
+  def setUp(self):
+    self.t = SetTrie([{1, 3}, {1, 3, 5}, {1, 4}, {1, 2, 4}, {2, 4}, {2, 3, 5}], recursion=True)
 
-
-class TestSetTrieMap(unittest.TestCase):
-  """
-  UnitTest for SetTrieMap class
-  """
-
+class TestSetTrieItemStack(TestSetTrie):
   def setUp(self):
-    self.t = SetTrieMap([({1, 3}, 'A'), ({1, 3, 5}, 'B'), ({1, 4}, 'C'),
-                         ({1, 2, 4}, 'D'), ({2, 4}, 'E'), ({2, 3, 5}, 'F')])
-    #self.t.printtree()
+    self.t = SetTrie([{1, 3}, {1, 3, 5}, {1, 4}, {1, 2, 4}, {2, 4}, {2, 3, 5}], recursion=None)
 
-  def test_print(self):
-    expected = """None
+class TestSetTrieMap(unittest.TestCase):
+    """
+    UnitTest for SetTrieMap class
+    """
+
+    def setUp(self):
+        self.t = SetTrieMap([({1, 3}, 'A'), ({1, 3, 5}, 'B'), ({1, 4}, 'C'),
+                             ({1, 2, 4}, 'D'), ({2, 4}, 'E'), ({2, 3, 5}, 'F')])
+        # self.t.printtree()
+
+    def test_print(self):
+        expected = \
+            """None
   1
     2
       4: 'D'
     3: 'A'
       5: 'B'
     4: 'C'
   2
     3
       5: 'F'
     4: 'E'
 """
-    from io import StringIO
-    outp = StringIO()
-    self.t.printtree(stream=outp)
-    self.assertEqual(outp.getvalue(), expected)
-  
-  def test_contains(self):
-    self.assertTrue(self.t.contains( {1, 3} ))
-    self.assertFalse(self.t.contains( {1} ))
-    self.assertTrue(self.t.contains( {1, 3, 5} ))
-    self.assertFalse(self.t.contains( {1, 3, 5, 7} ))
-
-  def test_in(self):
-    self.assertTrue({1, 3} in self.t)
-    self.assertFalse({1} in self.t)
-    self.assertTrue({1, 3, 5} in self.t)
-    self.assertFalse({1, 3, 5, 7} in self.t)
-
-  def test_get(self):
-    self.assertEqual(self.t.get({1, 3}), 'A')
-    self.assertEqual(self.t.get({1, 3, 5}), 'B')
-    self.assertEqual(self.t.get({1, 4}), 'C')
-    self.assertEqual(self.t.get({1, 2, 4}), 'D')
-    self.assertEqual(self.t.get({2, 4}), 'E')
-    self.assertEqual(self.t.get({2, 3, 5}), 'F')
-    self.assertEqual(self.t.get({1, 2, 3}), None)
-    self.assertEqual(self.t.get({100, 101, 102}, 0xDEADBEEF), 0xDEADBEEF)
-    self.assertEqual(self.t.get({}), None)
-  
-  def test_assign(self):
-    self.assertEqual(self.t.get({1, 3}), 'A')
-    self.t.assign({1, 3}, 'AAA')
-    self.assertEqual(self.t.get({1, 3}), 'AAA')
-    self.assertEqual(self.t.get({100, 200}), None)
-    self.t.assign({100, 200}, 'FOO')
-    self.assertEqual(self.t.get({100, 200}), 'FOO')
-    self.setUp()
-
-  def test_hassuperset(self):
-    self.assertTrue(self.t.hassuperset({3, 5}))
-    self.assertFalse(self.t.hassuperset({6}))
-    self.assertTrue(self.t.hassuperset({1, 2, 4}))
-    self.assertFalse(self.t.hassuperset({2, 4, 5} ))
-  
-  def test_supersets(self):
-    self.assertEqual(self.t.supersets({3, 5}), [({1, 3, 5}, 'B'), ({2, 3, 5}, 'F')])
-    self.assertEqual(self.t.supersets({1}), [({1, 2, 4}, 'D'), ({1, 3}, 'A'), ({1, 3, 5}, 'B'), ({1, 4}, 'C')])
-    self.assertEqual(self.t.supersets({1, 2, 5}), [])
-    self.assertEqual(self.t.supersets({3, 5}, mode='keys'), [{1, 3, 5}, {2, 3, 5}])
-    self.assertEqual(self.t.supersets({1}, mode='keys'), [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}])
-    self.assertEqual(self.t.supersets({1, 2, 5}, mode='keys'), [])
-    self.assertEqual(self.t.supersets({3, 5}, mode='values'), ['B', 'F'])
-    self.assertEqual(self.t.supersets({1}, mode='values'), ['D', 'A', 'B', 'C'])
-    self.assertEqual(self.t.supersets({1, 2, 5}, mode='values'), [])
-    
-  def test_hassubset(self):
-    self.assertTrue(self.t.hassubset({1, 2, 3}))
-    self.assertTrue(self.t.hassubset({2, 3, 4, 5}))
-    self.assertTrue(self.t.hassubset({1, 4}))
-    self.assertTrue(self.t.hassubset({2, 3, 5}))
-    self.assertFalse(self.t.hassubset({3, 4, 5}))
-    self.assertFalse(self.t.hassubset({6, 7, 8, 9, 1000}))
-
-  def test_subsets(self):
-    self.assertEqual(self.t.subsets({1, 2, 4, 11}), [({1, 2, 4}, 'D'), ({1, 4}, 'C'), ({2, 4}, 'E')])
-    self.assertEqual(self.t.subsets({1, 2, 4}), [({1, 2, 4}, 'D'), ({1, 4}, 'C'), ({2, 4}, 'E')])
-    self.assertEqual(self.t.subsets({1, 2}), [])
-    self.assertEqual(self.t.subsets({1, 2, 3, 4, 5}), [({1, 2, 4}, 'D'),
-      ({1, 3}, 'A'),
-      ({1, 3, 5}, 'B'),
-      ({1, 4}, 'C'),
-      ({2, 3, 5}, 'F'),
-      ({2, 4}, 'E')] )
-    self.assertEqual(self.t.subsets({0, 1, 3, 5}), [({1, 3}, 'A'), ({1, 3, 5}, 'B')])
-    self.assertEqual(self.t.subsets({1, 2, 5}), [])
-    self.assertEqual(self.t.subsets({1, 2, 4, 11}, mode='keys'), [{1, 2, 4}, {1, 4}, {2, 4}])
-    self.assertEqual(self.t.subsets({1, 2, 4}, mode='keys'), [{1, 2, 4}, {1, 4}, {2, 4}])
-    self.assertEqual(self.t.subsets({1, 2}, mode='keys'), [])
-    self.assertEqual(self.t.subsets({1, 2, 3, 4, 5}, mode='keys'), [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}, {2, 3, 5}, {2, 4}])
-    self.assertEqual(self.t.subsets({0, 1, 3, 5}, mode='keys'), [{1, 3}, {1, 3, 5}])
-    self.assertEqual(self.t.subsets({1, 2, 5}, mode='keys'), [])
-    self.assertEqual(self.t.subsets({1, 2, 4, 11}, mode='values'), ['D', 'C', 'E'])
-    self.assertEqual(self.t.subsets({1, 2, 4}, mode='values'), ['D', 'C', 'E'])
-    self.assertEqual(self.t.subsets({1, 2}, mode='values'), [])
-    self.assertEqual(self.t.subsets({1, 2, 3, 4, 5}, mode='values'), ['D', 'A', 'B', 'C', 'F', 'E'])
-    self.assertEqual(self.t.subsets({0, 1, 3, 5}, mode='values'), ['A', 'B'])
-    self.assertEqual(self.t.subsets({1, 2, 5}, mode='values'), [])
-    self.assertEqual(self.t.subsets({1, 4}), [({1, 4}, 'C')])
-    self.assertEqual(self.t.subsets({1, 3, 5}), [({1, 3}, 'A'), ({1, 3, 5}, 'B')])
-    self.assertEqual(self.t.subsets({1, 3, 5, 111}), [({1, 3}, 'A'), ({1, 3, 5}, 'B')])
-    self.assertEqual(self.t.subsets({1, 4, 8}), [({1, 4}, 'C')])
-    self.assertEqual(self.t.subsets({2, 3, 4, 5}), [({2, 3, 5}, 'F'), ({2, 4}, 'E')])
-    self.assertEqual(self.t.subsets({2, 3, 5, 6}), [({2, 3, 5}, 'F')])    
-    
-    
-
-  def test_iters(self):
-    self.assertEqual(self.t.aslist(), 
-      [({1, 2, 4}, 'D'), ({1, 3}, 'A'), ({1, 3, 5}, 'B'), ({1, 4}, 'C'), ({2, 3, 5}, 'F'), ({2, 4}, 'E')] )
-    self.assertEqual(list(self.t.keys()), [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}, {2, 3, 5}, {2, 4}] )
-    self.assertEqual(list(self.t.values()), ['D', 'A', 'B', 'C', 'F', 'E'] )
-    self.assertEqual(list(self.t.__iter__()), list(self.t.keys()))
-
+        from io import StringIO
+        outp = StringIO()
+        self.t.printtree(stream=outp)
+        self.assertEqual(outp.getvalue(), expected)
+
+    def test_contains(self):
+        self.assertTrue(self.t.contains({1, 3}))
+        self.assertFalse(self.t.contains({1}))
+        self.assertTrue(self.t.contains({1, 3, 5}))
+        self.assertFalse(self.t.contains({1, 3, 5, 7}))
+
+    def test_in(self):
+        self.assertTrue({1, 3} in self.t)
+        self.assertFalse({1} in self.t)
+        self.assertTrue({1, 3, 5} in self.t)
+        self.assertFalse({1, 3, 5, 7} in self.t)
+
+    def test_get(self):
+        self.assertEqual(self.t.get({1, 3}), 'A')
+        self.assertEqual(self.t.get({1, 3, 5}), 'B')
+        self.assertEqual(self.t.get({1, 4}), 'C')
+        self.assertEqual(self.t.get({1, 2, 4}), 'D')
+        self.assertEqual(self.t.get({2, 4}), 'E')
+        self.assertEqual(self.t.get({2, 3, 5}), 'F')
+        self.assertEqual(self.t.get({1, 2, 3}), None)
+        self.assertEqual(self.t.get({100, 101, 102}, 0xDEADBEEF), 0xDEADBEEF)
+        self.assertEqual(self.t.get({}), None)
+
+    def test_assign(self):
+        self.assertEqual(self.t.get({1, 3}), 'A')
+        self.t.assign({1, 3}, 'AAA')
+        self.assertEqual(self.t.get({1, 3}), 'AAA')
+        self.assertEqual(self.t.get({100, 200}), None)
+        self.t.assign({100, 200}, 'FOO')
+        self.assertEqual(self.t.get({100, 200}), 'FOO')
+        self.setUp()
+
+    def test_hassuperset(self):
+        self.assertTrue(self.t.hassuperset({3, 5}))
+        self.assertFalse(self.t.hassuperset({6}))
+        self.assertTrue(self.t.hassuperset({1, 2, 4}))
+        self.assertFalse(self.t.hassuperset({2, 4, 5}))
+
+    def test_supersets(self):
+        self.assertEqual(self.t.supersets({3, 5}), [({1, 3, 5}, 'B'), ({2, 3, 5}, 'F')])
+        self.assertEqual(self.t.supersets({1}), [({1, 2, 4}, 'D'), ({1, 3}, 'A'), ({1, 3, 5}, 'B'), ({1, 4}, 'C')])
+        self.assertEqual(self.t.supersets({1, 2, 5}), [])
+        self.assertEqual(self.t.supersetskeys({3, 5}), [{1, 3, 5}, {2, 3, 5}])
+        self.assertEqual(self.t.supersetskeys({1}), [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}])
+        self.assertEqual(self.t.supersetskeys({1, 2, 5}), [])
+        self.assertEqual(self.t.supersetsvalues({3, 5}), ['B', 'F'])
+        self.assertEqual(self.t.supersetsvalues({1}), ['D', 'A', 'B', 'C'])
+        self.assertEqual(self.t.supersetsvalues({1, 2, 5}), [])
+
+    def test_hassubset(self):
+        self.assertTrue(self.t.hassubset({1, 2, 3}))
+        self.assertTrue(self.t.hassubset({2, 3, 4, 5}))
+        self.assertTrue(self.t.hassubset({1, 4}))
+        self.assertTrue(self.t.hassubset({2, 3, 5}))
+        self.assertFalse(self.t.hassubset({3, 4, 5}))
+        self.assertFalse(self.t.hassubset({6, 7, 8, 9, 1000}))
+
+    def test_subsets(self):
+        self.assertEqual(self.t.subsets({1, 2, 4, 11}), [({1, 2, 4}, 'D'), ({1, 4}, 'C'), ({2, 4}, 'E')])
+        self.assertEqual(self.t.subsets({1, 2, 4}), [({1, 2, 4}, 'D'), ({1, 4}, 'C'), ({2, 4}, 'E')])
+        self.assertEqual(self.t.subsets({1, 2}), [])
+        self.assertEqual(self.t.subsets({1, 2, 3, 4, 5}), [({1, 2, 4}, 'D'), ({1, 3}, 'A'), ({1, 3, 5}, 'B'),
+                                                           ({1, 4}, 'C'), ({2, 3, 5}, 'F'), ({2, 4}, 'E')])
+        self.assertEqual(self.t.subsets({0, 1, 3, 5}), [({1, 3}, 'A'), ({1, 3, 5}, 'B')])
+        self.assertEqual(self.t.subsets({1, 2, 5}), [])
+        self.assertEqual(self.t.subsetskeys({1, 2, 4, 11}), [{1, 2, 4}, {1, 4}, {2, 4}])
+        self.assertEqual(self.t.subsetskeys({1, 2, 4}), [{1, 2, 4}, {1, 4}, {2, 4}])
+        self.assertEqual(self.t.subsetskeys({1, 2}), [])
+        self.assertEqual(self.t.subsetskeys({1, 2, 3, 4, 5}), [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}, {2, 3, 5},
+                                                                        {2, 4}])
+        self.assertEqual(self.t.subsetskeys({0, 1, 3, 5}), [{1, 3}, {1, 3, 5}])
+        self.assertEqual(self.t.subsetskeys({1, 2, 5}), [])
+        self.assertEqual(self.t.subsetsvalues({1, 2, 4, 11}), ['D', 'C', 'E'])
+        self.assertEqual(self.t.subsetsvalues({1, 2, 4}), ['D', 'C', 'E'])
+        self.assertEqual(self.t.subsetsvalues({1, 2}), [])
+        self.assertEqual(self.t.subsetsvalues({1, 2, 3, 4, 5}), ['D', 'A', 'B', 'C', 'F', 'E'])
+        self.assertEqual(self.t.subsetsvalues({0, 1, 3, 5}), ['A', 'B'])
+        self.assertEqual(self.t.subsetsvalues({1, 2, 5}), [])
+        self.assertEqual(self.t.subsets({1, 4}), [({1, 4}, 'C')])
+        self.assertEqual(self.t.subsets({1, 3, 5}), [({1, 3}, 'A'), ({1, 3, 5}, 'B')])
+        self.assertEqual(self.t.subsets({1, 3, 5, 111}), [({1, 3}, 'A'), ({1, 3, 5}, 'B')])
+        self.assertEqual(self.t.subsets({1, 4, 8}), [({1, 4}, 'C')])
+        self.assertEqual(self.t.subsets({2, 3, 4, 5}), [({2, 3, 5}, 'F'), ({2, 4}, 'E')])
+        self.assertEqual(self.t.subsets({2, 3, 5, 6}), [({2, 3, 5}, 'F')])
+
+    def test_iters(self):
+        self.assertEqual(self.t.aslist(), [({1, 2, 4}, 'D'), ({1, 3}, 'A'), ({1, 3, 5}, 'B'), ({1, 4}, 'C'),
+                                           ({2, 3, 5}, 'F'), ({2, 4}, 'E')])
+        self.assertEqual(list(self.t.keys()), [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}, {2, 3, 5}, {2, 4}])
+        self.assertEqual(list(self.t.values()), ['D', 'A', 'B', 'C', 'F', 'E'])
+        self.assertEqual(list(self.t.__iter__()), list(self.t.keys()))
 
 class TestSetTrieMultiMap(unittest.TestCase):
-  """
-  UnitTest for SetTrieMultiMap class
-  """
-
-  def setUp(self):
-    self.t = SetTrieMultiMap([({1, 3}, 'A'), ({1, 3}, 'AA'), ({1, 3, 5}, 'B'), ({1, 4}, 'C'), ({1, 4}, 'CC'),
-                         ({1, 2, 4}, 'D'), ({1, 2, 4}, 'DD'), ({2, 4}, 'E'), ({2, 3, 5}, 'F'),
-                         ({2, 3, 5}, 'FF'), ({2, 3, 5}, 'FFF')])
-    
-  def test_aslist(self):
-    self.assertEqual(self.t.aslist(), 
-      [({1, 2, 4}, 'D'), ({1, 2, 4}, 'DD'), ({1, 3}, 'A'), ({1, 3}, 'AA'), ({1, 3, 5}, 'B'),
-       ({1, 4}, 'C'), ({1, 4}, 'CC'), ({2, 3, 5}, 'F'), ({2, 3, 5}, 'FF'), ({2, 3, 5}, 'FFF'), ({2, 4}, 'E')] )
-
-  def test_assign_returned_value(self):
-    x = SetTrieMultiMap()
-    self.assertEqual(x.assign({1, 3}, 'A'), 1)
-    self.assertEqual(x.assign({1, 3}, 'AA'), 2)
-    self.assertEqual(x.assign({1, 3}, 'A'), 3)
-    self.assertEqual(x.assign({2, 4, 5}, 'Y'), 1)
-
-  def test_count(self):
-    self.assertEqual(self.t.count({1, 3}), 2)
-    self.assertEqual(self.t.count({1, 3, 5}), 1)
-    self.assertEqual(self.t.count({1, 3, 4}), 0)
-    self.assertEqual(self.t.count({111, 222}), 0)
-    self.assertEqual(self.t.count({2, 3, 5}), 3)
-
-  def test_iterget(self):
-    self.assertEqual(list(self.t.iterget({1, 3})), ['A', 'AA'])
-    self.assertEqual(list(self.t.iterget({1, 3, 4})), [])
-    
-  def test_get(self):
-    self.assertEqual(self.t.get({1, 3}), ['A', 'AA'])
-    self.assertEqual(self.t.get({1, 2, 4}), ['D', 'DD'])
-    self.assertEqual(self.t.get({1, 3, 5}), ['B'])
-    self.assertEqual(self.t.get({2, 3, 5}), ['F', 'FF', 'FFF'])
-    self.assertEqual(self.t.get({2, 4}), ['E'])
-    self.assertEqual(self.t.get({1, 3, 4}), None)
-    self.assertEqual(self.t.get({44}, []), [])
-    
-  def test_hassuperset(self):
-    self.assertTrue(self.t.hassuperset({3, 5}))
-    self.assertFalse(self.t.hassuperset({6}))
-    self.assertTrue(self.t.hassuperset({1, 2, 4}))
-    self.assertFalse(self.t.hassuperset({2, 4, 5} ))
-
-  def test_supersets(self):
-    self.assertEqual(self.t.supersets({3, 5}), [({1, 3, 5}, 'B'), ({2, 3, 5}, 'F'), ({2, 3, 5}, 'FF'), ({2, 3, 5}, 'FFF')])
-    self.assertEqual(self.t.supersets({3, 5}, mode='values'), ['B', 'F', 'FF', 'FFF'])
-    self.assertEqual(self.t.supersets({3, 5}, mode='keys'), [{1, 3, 5}, {2, 3, 5}])
-    self.assertEqual(self.t.supersets({1}), [({1, 2, 4}, 'D'), ({1, 2, 4}, 'DD'), ({1, 3}, 'A'), 
-                                             ({1, 3}, 'AA'), ({1, 3, 5}, 'B'), ({1, 4}, 'C'), ({1, 4}, 'CC')] )
-    self.assertEqual(self.t.supersets({1}, mode='keys'), [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}])
-    self.assertEqual(self.t.supersets({1}, mode='values'), ['D', 'DD', 'A', 'AA', 'B', 'C', 'CC'])
-    self.assertEqual(self.t.supersets({1, 2, 5}), [])
-    self.assertEqual(self.t.supersets({1, 2, 5}, mode='keys'), [])
-    self.assertEqual(self.t.supersets({1, 2, 5}, mode='values'), [])
-
-  def test_hassubset(self):
-    self.assertTrue(self.t.hassubset({1, 2, 3}))
-    self.assertTrue(self.t.hassubset({2, 3, 4, 5}))
-    self.assertTrue(self.t.hassubset({1, 4}))
-    self.assertTrue(self.t.hassubset({2, 3, 5}))
-    self.assertFalse(self.t.hassubset({3, 4, 5}))
-    self.assertFalse(self.t.hassubset({6, 7, 8, 9, 1000}))
-
-  def test_subsets(self):
-    self.assertEqual(self.t.subsets({1, 2, 4, 11}), [({1, 2, 4}, 'D'), ({1, 2, 4}, 'DD'), ({1, 4}, 'C'), 
-                                                     ({1, 4}, 'CC'), ({2, 4}, 'E')] )
-    self.assertEqual(self.t.subsets({1, 2, 4, 11}, mode='keys'), [{1, 2, 4}, {1, 4}, {2, 4}])
-    self.assertEqual(self.t.subsets({1, 2, 4, 11}, mode='values'), ['D', 'DD', 'C', 'CC', 'E'])
-    self.assertEqual(self.t.subsets({1, 2, 4}), [({1, 2, 4}, 'D'), ({1, 2, 4}, 'DD'), ({1, 4}, 'C'), ({1, 4}, 'CC'),
-                                                 ({2, 4}, 'E')])
-    self.assertEqual(self.t.subsets({1, 2, 4}, mode='keys'), [{1, 2, 4}, {1, 4}, {2, 4}])
-    self.assertEqual(self.t.subsets({1, 2, 4}, mode='values'), ['D', 'DD', 'C', 'CC', 'E'])
-    self.assertEqual(self.t.subsets({1, 2}), [])
-    self.assertEqual(self.t.subsets({1, 2}, mode='keys'), [])
-    self.assertEqual(self.t.subsets({1, 2}, mode='values'), [])
-    self.assertEqual(self.t.subsets({1, 2, 3, 4, 5}), 
-      [({1, 2, 4}, 'D'), ({1, 2, 4}, 'DD'), ({1, 3}, 'A'), ({1, 3}, 'AA'), ({1, 3, 5}, 'B'), 
-       ({1, 4}, 'C'), ({1, 4}, 'CC'), ({2, 3, 5}, 'F'), ({2, 3, 5}, 'FF'), ({2, 3, 5}, 'FFF'), ({2, 4}, 'E')] )
-    self.assertEqual(self.t.subsets({1, 2, 3, 4, 5}), self.t.aslist())
-    self.assertEqual(self.t.subsets({1, 2, 3, 4, 5}, mode='keys'), list(self.t.keys()))
-    self.assertEqual(self.t.subsets({1, 2, 3, 4, 5}, mode='keys'), [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}, {2, 3, 5}, {2, 4}])
-    self.assertEqual(self.t.subsets({1, 2, 3, 4, 5}, mode='values'), 
-      ['D', 'DD', 'A', 'AA', 'B', 'C', 'CC', 'F', 'FF', 'FFF', 'E'])
-    self.assertEqual(self.t.subsets({1, 2, 3, 4, 5}, mode='values'), list(self.t.values()))
-    self.assertEqual(self.t.subsets({0, 1, 3, 5}), [({1, 3}, 'A'), ({1, 3}, 'AA'), ({1, 3, 5}, 'B')])
-    self.assertEqual(self.t.subsets({0, 1, 3, 5}, mode='keys'), [{1, 3}, {1, 3, 5}])
-    self.assertEqual(self.t.subsets({0, 1, 3, 5}, mode='values'), ['A', 'AA', 'B'])
-    self.assertEqual(self.t.subsets({1, 2, 5}), [])
-    self.assertEqual(self.t.subsets({1, 2, 5}, mode='keys'), [])
-    self.assertEqual(self.t.subsets({1, 2, 5}, mode='values'), [])
-    self.assertEqual(self.t.subsets({1, 4}), [({1, 4}, 'C'), ({1, 4}, 'CC')])
-    self.assertEqual(self.t.subsets({1, 3, 5}), [({1, 3}, 'A'), ({1, 3}, 'AA'), ({1, 3, 5}, 'B')])
-    self.assertEqual(self.t.subsets({1, 3, 5, 111}), [({1, 3}, 'A'), ({1, 3}, 'AA'), ({1, 3, 5}, 'B')])
-    self.assertEqual(self.t.subsets({1, 4, 8}), [({1, 4}, 'C'), ({1, 4}, 'CC')])
-    self.assertEqual(self.t.subsets({2, 3, 4, 5}), [({2, 3, 5}, 'F'), ({2, 3, 5}, 'FF'), ({2, 3, 5}, 'FFF'), ({2, 4}, 'E')])
-    self.assertEqual(self.t.subsets({2, 3, 5, 6}), [({2, 3, 5}, 'F'), ({2, 3, 5}, 'FF'), ({2, 3, 5}, 'FFF')])     
+    """
+    UnitTest for SetTrieMultiMap class
+    """
+
+    def setUp(self):
+        self.t = SetTrieMultiMap([({1, 3}, 'A'), ({1, 3}, 'AA'), ({1, 3, 5}, 'B'), ({1, 4}, 'C'), ({1, 4}, 'CC'),
+                                  ({1, 2, 4}, 'D'), ({1, 2, 4}, 'DD'), ({2, 4}, 'E'), ({2, 3, 5}, 'F'),
+                                  ({2, 3, 5}, 'FF'), ({2, 3, 5}, 'FFF')])
+
+    def test_aslist(self):
+        self.assertEqual(self.t.aslist(), [({1, 2, 4}, 'D'), ({1, 2, 4}, 'DD'), ({1, 3}, 'A'), ({1, 3}, 'AA'),
+                                           ({1, 3, 5}, 'B'), ({1, 4}, 'C'), ({1, 4}, 'CC'), ({2, 3, 5}, 'F'),
+                                           ({2, 3, 5}, 'FF'), ({2, 3, 5}, 'FFF'), ({2, 4}, 'E')])
+
+    def test_assign_returned_value(self):
+        x = SetTrieMultiMap()
+        self.assertEqual(x.assign({1, 3}, 'A'), 1)
+        self.assertEqual(x.assign({1, 3}, 'AA'), 2)
+        self.assertEqual(x.assign({1, 3}, 'A'), 3)
+        self.assertEqual(x.assign({2, 4, 5}, 'Y'), 1)
+
+    def test_count(self):
+        self.assertEqual(self.t.count({1, 3}), 2)
+        self.assertEqual(self.t.count({1, 3, 5}), 1)
+        self.assertEqual(self.t.count({1, 3, 4}), 0)
+        self.assertEqual(self.t.count({111, 222}), 0)
+        self.assertEqual(self.t.count({2, 3, 5}), 3)
+
+    def test_iterget(self):
+        self.assertEqual(list(self.t.iterget({1, 3})), ['A', 'AA'])
+        self.assertEqual(list(self.t.iterget({1, 3, 4})), [])
+
+    def test_get(self):
+        self.assertEqual(self.t.get({1, 3}), ['A', 'AA'])
+        self.assertEqual(self.t.get({1, 2, 4}), ['D', 'DD'])
+        self.assertEqual(self.t.get({1, 3, 5}), ['B'])
+        self.assertEqual(self.t.get({2, 3, 5}), ['F', 'FF', 'FFF'])
+        self.assertEqual(self.t.get({2, 4}), ['E'])
+        self.assertEqual(self.t.get({1, 3, 4}), None)
+        self.assertEqual(self.t.get({44}, []), [])
+
+    def test_hassuperset(self):
+        self.assertTrue(self.t.hassuperset({3, 5}))
+        self.assertFalse(self.t.hassuperset({6}))
+        self.assertTrue(self.t.hassuperset({1, 2, 4}))
+        self.assertFalse(self.t.hassuperset({2, 4, 5}))
+
+    def test_supersets(self):
+        self.assertEqual(self.t.supersets({3, 5}), [({1, 3, 5}, 'B'), ({2, 3, 5}, 'F'), ({2, 3, 5}, 'FF'),
+                                                    ({2, 3, 5}, 'FFF')])
+        self.assertEqual(self.t.supersetsvalues({3, 5}), ['B', 'F', 'FF', 'FFF'])
+        self.assertEqual(self.t.supersetskeys({3, 5}), [{1, 3, 5}, {2, 3, 5}])
+        self.assertEqual(self.t.supersets({1}), [({1, 2, 4}, 'D'), ({1, 2, 4}, 'DD'), ({1, 3}, 'A'),
+                                                 ({1, 3}, 'AA'), ({1, 3, 5}, 'B'), ({1, 4}, 'C'),
+                                                 ({1, 4}, 'CC')])
+        self.assertEqual(self.t.supersetskeys({1}), [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}])
+        self.assertEqual(self.t.supersetsvalues({1}), ['D', 'DD', 'A', 'AA', 'B', 'C', 'CC'])
+        self.assertEqual(self.t.supersets({1, 2, 5}), [])
+        self.assertEqual(self.t.supersetskeys({1, 2, 5}), [])
+        self.assertEqual(self.t.supersetsvalues({1, 2, 5}), [])
+
+    def test_hassubset(self):
+        self.assertTrue(self.t.hassubset({1, 2, 3}))
+        self.assertTrue(self.t.hassubset({2, 3, 4, 5}))
+        self.assertTrue(self.t.hassubset({1, 4}))
+        self.assertTrue(self.t.hassubset({2, 3, 5}))
+        self.assertFalse(self.t.hassubset({3, 4, 5}))
+        self.assertFalse(self.t.hassubset({6, 7, 8, 9, 1000}))
+
+    def test_subsets(self):
+        self.assertEqual(self.t.subsets({1, 2, 4, 11}), [({1, 2, 4}, 'D'), ({1, 2, 4}, 'DD'), ({1, 4}, 'C'),
+                                                         ({1, 4}, 'CC'), ({2, 4}, 'E')])
+        self.assertEqual(self.t.subsetskeys({1, 2, 4, 11}), [{1, 2, 4}, {1, 4}, {2, 4}])
+        self.assertEqual(self.t.subsetsvalues({1, 2, 4, 11}), ['D', 'DD', 'C', 'CC', 'E'])
+        self.assertEqual(self.t.subsets({1, 2, 4}), [({1, 2, 4}, 'D'), ({1, 2, 4}, 'DD'), ({1, 4}, 'C'), ({1, 4}, 'CC'),
+                                                     ({2, 4}, 'E')])
+        self.assertEqual(self.t.subsetskeys({1, 2, 4}), [{1, 2, 4}, {1, 4}, {2, 4}])
+        self.assertEqual(self.t.subsetsvalues({1, 2, 4}), ['D', 'DD', 'C', 'CC', 'E'])
+        self.assertEqual(self.t.subsets({1, 2}), [])
+        self.assertEqual(self.t.subsetskeys({1, 2}), [])
+        self.assertEqual(self.t.subsetsvalues({1, 2}), [])
+        self.assertEqual(self.t.subsets({1, 2, 3, 4, 5}), [({1, 2, 4}, 'D'), ({1, 2, 4}, 'DD'), ({1, 3}, 'A'),
+                                                           ({1, 3}, 'AA'), ({1, 3, 5}, 'B'), ({1, 4}, 'C'),
+                                                           ({1, 4}, 'CC'), ({2, 3, 5}, 'F'), ({2, 3, 5}, 'FF'),
+                                                           ({2, 3, 5}, 'FFF'), ({2, 4}, 'E')])
+        self.assertEqual(self.t.subsets({1, 2, 3, 4, 5}), self.t.aslist())
+        self.assertEqual(self.t.subsetskeys({1, 2, 3, 4, 5}), list(self.t.keys()))
+        self.assertEqual(self.t.subsetskeys({1, 2, 3, 4, 5}), [{1, 2, 4}, {1, 3}, {1, 3, 5}, {1, 4}, {2, 3, 5},
+                                                                        {2, 4}])
+        self.assertEqual(self.t.subsetsvalues({1, 2, 3, 4, 5}), ['D', 'DD', 'A', 'AA', 'B', 'C', 'CC', 'F',
+                                                                          'FF', 'FFF', 'E'])
+        self.assertEqual(self.t.subsetsvalues({1, 2, 3, 4, 5}), list(self.t.values()))
+        self.assertEqual(self.t.subsets({0, 1, 3, 5}), [({1, 3}, 'A'), ({1, 3}, 'AA'), ({1, 3, 5}, 'B')])
+        self.assertEqual(self.t.subsetskeys({0, 1, 3, 5}), [{1, 3}, {1, 3, 5}])
+        self.assertEqual(self.t.subsetsvalues({0, 1, 3, 5}), ['A', 'AA', 'B'])
+        self.assertEqual(self.t.subsets({1, 2, 5}), [])
+        self.assertEqual(self.t.subsetskeys({1, 2, 5}), [])
+        self.assertEqual(self.t.subsetsvalues({1, 2, 5}), [])
+        self.assertEqual(self.t.subsets({1, 4}), [({1, 4}, 'C'), ({1, 4}, 'CC')])
+        self.assertEqual(self.t.subsets({1, 3, 5}), [({1, 3}, 'A'), ({1, 3}, 'AA'), ({1, 3, 5}, 'B')])
+        self.assertEqual(self.t.subsets({1, 3, 5, 111}), [({1, 3}, 'A'), ({1, 3}, 'AA'), ({1, 3, 5}, 'B')])
+        self.assertEqual(self.t.subsets({1, 4, 8}), [({1, 4}, 'C'), ({1, 4}, 'CC')])
+        self.assertEqual(self.t.subsets({2, 3, 4, 5}), [({2, 3, 5}, 'F'), ({2, 3, 5}, 'FF'), ({2, 3, 5}, 'FFF'),
+                                                        ({2, 4}, 'E')])
+        self.assertEqual(self.t.subsets({2, 3, 5, 6}), [({2, 3, 5}, 'F'), ({2, 3, 5}, 'FF'), ({2, 3, 5}, 'FFF')])
 
-# - - - - - - -
+    # - - - - - - -
 
 # If module is executed from command line, perform tests:
-if __name__ == "__main__":
-  unittest.main(verbosity=2)
+if __name__ == '__main__':
+    unittest.main(verbosity=2)
```

