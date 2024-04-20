# Comparing `tmp/dogma_data-0.2.6.tar.gz` & `tmp/dogma_data-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogma_data-0.2.6.tar", last modified: Thu Apr 18 18:38:42 2024, max compression
+gzip compressed data, was "dogma_data-0.2.7.tar", last modified: Sat Apr 20 02:47:21 2024, max compression
```

## Comparing `dogma_data-0.2.6.tar` & `dogma_data-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-18 18:38:42.025747 dogma_data-0.2.6/
--rw-r--r--   0 roed     (23269) root         (0)      628 2024-04-18 18:38:42.025747 dogma_data-0.2.6/PKG-INFO
--rw-r--r--   0 roed     (23269) root         (0)        0 2024-04-10 03:45:24.000000 dogma_data-0.2.6/README.md
-drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-18 18:38:42.025747 dogma_data-0.2.6/dogma_data/
--rw-r--r--   0 roed     (23269) root         (0)      235 2024-04-18 18:31:18.000000 dogma_data-0.2.6/dogma_data/__init__.py
--rw-r--r--   0 roed     (23269) root         (0)    11465 2024-04-18 18:37:22.000000 dogma_data-0.2.6/dogma_data/_dogma_data.py
--rw-r--r--   0 roed     (23269) root         (0)      450 2024-04-10 03:45:24.000000 dogma_data-0.2.6/dogma_data/dogma_torch.py
--rw-r--r--   0 roed     (23269) root         (0)     7292 2024-04-10 07:59:30.000000 dogma_data-0.2.6/dogma_data/fasta.py
--rw-r--r--   0 roed     (23269) root         (0)     3287 2024-04-18 18:25:24.000000 dogma_data-0.2.6/dogma_data/sharded_data.py
--rw-r--r--   0 roed     (23269) root         (0)      762 2024-04-10 03:45:24.000000 dogma_data-0.2.6/dogma_data/utils.py
-drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-18 18:38:42.025747 dogma_data-0.2.6/dogma_data.egg-info/
--rw-r--r--   0 roed     (23269) root         (0)      628 2024-04-18 18:38:42.000000 dogma_data-0.2.6/dogma_data.egg-info/PKG-INFO
--rw-r--r--   0 roed     (23269) root         (0)      335 2024-04-18 18:38:42.000000 dogma_data-0.2.6/dogma_data.egg-info/SOURCES.txt
--rw-r--r--   0 roed     (23269) root         (0)        1 2024-04-18 18:38:42.000000 dogma_data-0.2.6/dogma_data.egg-info/dependency_links.txt
--rw-r--r--   0 roed     (23269) root         (0)       93 2024-04-18 18:38:42.000000 dogma_data-0.2.6/dogma_data.egg-info/requires.txt
--rw-r--r--   0 roed     (23269) root         (0)       11 2024-04-18 18:38:42.000000 dogma_data-0.2.6/dogma_data.egg-info/top_level.txt
--rw-r--r--   0 roed     (23269) root         (0)     1067 2024-04-18 18:38:33.000000 dogma_data-0.2.6/pyproject.toml
--rw-r--r--   0 roed     (23269) root         (0)       38 2024-04-18 18:38:42.025747 dogma_data-0.2.6/setup.cfg
+drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-20 02:47:21.357833 dogma_data-0.2.7/
+-rw-r--r--   0 roed     (23269) root         (0)      628 2024-04-20 02:47:21.357833 dogma_data-0.2.7/PKG-INFO
+-rw-r--r--   0 roed     (23269) root         (0)        0 2024-04-10 03:45:24.000000 dogma_data-0.2.7/README.md
+drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-20 02:47:21.357833 dogma_data-0.2.7/dogma_data/
+-rw-r--r--   0 roed     (23269) root         (0)      235 2024-04-18 18:31:18.000000 dogma_data-0.2.7/dogma_data/__init__.py
+-rw-r--r--   0 roed     (23269) root         (0)    11807 2024-04-19 18:41:42.000000 dogma_data-0.2.7/dogma_data/_dogma_data.py
+-rw-r--r--   0 roed     (23269) root         (0)      450 2024-04-10 03:45:24.000000 dogma_data-0.2.7/dogma_data/dogma_torch.py
+-rw-r--r--   0 roed     (23269) root         (0)     7292 2024-04-10 07:59:30.000000 dogma_data-0.2.7/dogma_data/fasta.py
+-rw-r--r--   0 roed     (23269) root         (0)     3287 2024-04-18 18:25:24.000000 dogma_data-0.2.7/dogma_data/sharded_data.py
+-rw-r--r--   0 roed     (23269) root         (0)      762 2024-04-10 03:45:24.000000 dogma_data-0.2.7/dogma_data/utils.py
+drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-20 02:47:21.357833 dogma_data-0.2.7/dogma_data.egg-info/
+-rw-r--r--   0 roed     (23269) root         (0)      628 2024-04-20 02:47:21.000000 dogma_data-0.2.7/dogma_data.egg-info/PKG-INFO
+-rw-r--r--   0 roed     (23269) root         (0)      335 2024-04-20 02:47:21.000000 dogma_data-0.2.7/dogma_data.egg-info/SOURCES.txt
+-rw-r--r--   0 roed     (23269) root         (0)        1 2024-04-20 02:47:21.000000 dogma_data-0.2.7/dogma_data.egg-info/dependency_links.txt
+-rw-r--r--   0 roed     (23269) root         (0)       93 2024-04-20 02:47:21.000000 dogma_data-0.2.7/dogma_data.egg-info/requires.txt
+-rw-r--r--   0 roed     (23269) root         (0)       11 2024-04-20 02:47:21.000000 dogma_data-0.2.7/dogma_data.egg-info/top_level.txt
+-rw-r--r--   0 roed     (23269) root         (0)     1067 2024-04-20 02:46:13.000000 dogma_data-0.2.7/pyproject.toml
+-rw-r--r--   0 roed     (23269) root         (0)       38 2024-04-20 02:47:21.357833 dogma_data-0.2.7/setup.cfg
```

### Comparing `dogma_data-0.2.6/PKG-INFO` & `dogma_data-0.2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dogma-data
-Version: 0.2.6
+Version: 0.2.7
 Summary: Data processing for Dogma
 Author-email: Marcel Rød <roed@stanford.edu>
 Project-URL: Homepage, https://github.com/marcelroed/dogma-data
 Project-URL: Repository, https://github.com/marcelroed/dogma-data.git
 Keywords: single-cell,RNA-seq,embedding,pytorch,uce
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: lightning
 Requires-Dist: numpy
 Requires-Dist: awkward
 Requires-Dist: tqdm
 Requires-Dist: numba
 Requires-Dist: lightning_cloud
 Requires-Dist: blosc2
-Requires-Dist: dogma-rust>=0.2.4
+Requires-Dist: dogma-rust>=0.2.5
 Requires-Dist: smart-open
 Requires-Dist: click
```

### Comparing `dogma_data-0.2.6/dogma_data/_dogma_data.py` & `dogma_data-0.2.7/dogma_data/_dogma_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,31 +81,41 @@
             compressed = pickle.load(path_or_fileobj)
     else:
         raise ValueError(f'path_or_fileobj must be a Path, str, or IO object, not {type(path_or_fileobj)}')
     with timer('Decompressing'):
         return _decompress_leaves(compressed)
 
 
-def write_awkward(arr: ak.Array, path_or_fileobj: Path | str | IO):
+def write_awkward(arr: ak.Array, path_or_fileobj: Path | str | IO, nthreads: int | None = None):
     """
     Write any awkward array to file.
     Compresses the underlying buffers with Blosc2 blosclz for efficient storage and very fast reading/writing with multiple threads.
     """
-    blosc2.set_nthreads(64)
-    tree = ak.to_buffers(arr)
-    write_blosc_pickle(tree, path_or_fileobj)
+    try:
+        if nthreads:
+            prev_nthreads = blosc2.set_nthreads(nthreads)
+        tree = ak.to_buffers(arr)
+        write_blosc_pickle(tree, path_or_fileobj)
+    finally:
+        if nthreads:
+            blosc2.set_nthreads(prev_nthreads)
 
-def read_awkward(path_or_fileobj: Path | str | IO) -> ak.Array:
+def read_awkward(path_or_fileobj: Path | str | IO, nthreads=None) -> ak.Array:
     """
     Read any awkward array from file.
     Decompresses using Blosc2 blosclz for very fast reading with multiple threads.
     """
-    blosc2.set_nthreads(64)
-    tree = read_blosc_pickle(path_or_fileobj)
-    return ak.from_buffers(*tree)
+    try:
+        if nthreads:
+            prev_nthreads = blosc2.set_nthreads(nthreads)
+        tree = read_blosc_pickle(path_or_fileobj)
+        return ak.from_buffers(*tree)
+    finally:
+        if nthreads:
+            blosc2.set_nthreads(prev_nthreads)
 
 @njit(parallel=True)
 def _fast_pack(seqlens, starts, stops, content):
     """
     Helper function to quickly pack content into a new Awkward array buffer.
     """
     cu_seqlens = np.zeros((len(seqlens) + 1,), dtype=np.int64)
```

### Comparing `dogma_data-0.2.6/dogma_data/fasta.py` & `dogma_data-0.2.7/dogma_data/fasta.py`

 * *Files identical despite different names*

### Comparing `dogma_data-0.2.6/dogma_data/sharded_data.py` & `dogma_data-0.2.7/dogma_data/sharded_data.py`

 * *Files identical despite different names*

### Comparing `dogma_data-0.2.6/dogma_data/utils.py` & `dogma_data-0.2.7/dogma_data/utils.py`

 * *Files identical despite different names*

### Comparing `dogma_data-0.2.6/dogma_data.egg-info/PKG-INFO` & `dogma_data-0.2.7/dogma_data.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dogma-data
-Version: 0.2.6
+Version: 0.2.7
 Summary: Data processing for Dogma
 Author-email: Marcel Rød <roed@stanford.edu>
 Project-URL: Homepage, https://github.com/marcelroed/dogma-data
 Project-URL: Repository, https://github.com/marcelroed/dogma-data.git
 Keywords: single-cell,RNA-seq,embedding,pytorch,uce
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: lightning
 Requires-Dist: numpy
 Requires-Dist: awkward
 Requires-Dist: tqdm
 Requires-Dist: numba
 Requires-Dist: lightning_cloud
 Requires-Dist: blosc2
-Requires-Dist: dogma-rust>=0.2.4
+Requires-Dist: dogma-rust>=0.2.5
 Requires-Dist: smart-open
 Requires-Dist: click
```

### Comparing `dogma_data-0.2.6/pyproject.toml` & `dogma_data-0.2.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dogma-data"
 description = "Data processing for Dogma"
-version = "0.2.6"
+version = "0.2.7"
 requires-python = ">=3.11"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["single-cell", "RNA-seq", "embedding", "pytorch", "uce"]
 dependencies = [
     "lightning",
     "numpy",
     "awkward",
     "tqdm",
     "numba",
     "lightning_cloud",
     "blosc2",
-    "dogma-rust >= 0.2.4",
+    "dogma-rust >= 0.2.5",
     "smart-open",
     "click",
 ]
 
 authors = [
     {name = "Marcel Rød", email = "roed@stanford.edu"},
 ]
```

