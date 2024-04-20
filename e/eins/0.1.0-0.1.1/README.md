# Comparing `tmp/eins-0.1.0.tar.gz` & `tmp/eins-0.1.1.tar.gz`

## Comparing `eins-0.1.0.tar` & `eins-0.1.1.tar`

### file list

```diff
@@ -1,49 +1,51 @@
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 eins-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 eins-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 eins-0.1.0/algorithm.md
--rw-r--r--   0        0        0    12443 2020-02-02 00:00:00.000000 eins-0.1.0/benchmarking.ipynb
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 eins-0.1.0/examples.ipynb
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 eins-0.1.0/examples.md
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 eins-0.1.0/examples.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 eins-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0    16996 2020-02-02 00:00:00.000000 eins-0.1.0/network.ipynb
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 eins-0.1.0/parsing.md
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 eins-0.1.0/perf.ipynb
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 eins-0.1.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 eins-0.1.0/docs/in-depth.md
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 eins-0.1.0/docs/index.md
--rw-r--r--   0        0        0    16072 2020-02-02 00:00:00.000000 eins-0.1.0/docs/tutorial.md
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 eins-0.1.0/docs/javascripts/katex.js
--rw-r--r--   0        0        0   201364 2020-02-02 00:00:00.000000 eins-0.1.0/docs/stylesheets/CascadiaCode.woff2
--rw-r--r--   0        0        0   143760 2020-02-02 00:00:00.000000 eins-0.1.0/docs/stylesheets/CascadiaCodeItalic.woff2
--rw-r--r--   0        0        0   202128 2020-02-02 00:00:00.000000 eins-0.1.0/docs/stylesheets/InstrumentSans-Italic[wdth,wght].ttf
--rw-r--r--   0        0        0   194336 2020-02-02 00:00:00.000000 eins-0.1.0/docs/stylesheets/InstrumentSans[wdth,wght].ttf
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 eins-0.1.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 eins-0.1.0/docs/stylesheets/readme.md
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 eins-0.1.0/examples/README.md
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 eins-0.1.0/examples/multi_head_attention.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 eins-0.1.0/examples/vit_encoder.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/__about__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/__init__.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/combination.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/common_types.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/concrete.py
--rw-r--r--   0        0        0     9104 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/constraint.py
--rw-r--r--   0        0        0    19810 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/einsop.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/elementwise.py
--rw-r--r--   0        0        0     7537 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/namespaces.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/parsing.py
--rw-r--r--   0        0        0    14784 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/program.py
--rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/reduction.py
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/strategy.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/symbolic.py
--rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/transformation.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/utils.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 eins-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 eins-0.1.0/tests/test_basic.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 eins-0.1.0/tests/test_parsing.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 eins-0.1.0/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 eins-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 eins-0.1.0/README.md
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 eins-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 eins-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 eins-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 eins-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 eins-0.1.1/algorithm.md
+-rw-r--r--   0        0        0    12443 2020-02-02 00:00:00.000000 eins-0.1.1/benchmarking.ipynb
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 eins-0.1.1/examples.ipynb
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 eins-0.1.1/examples.md
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 eins-0.1.1/examples.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 eins-0.1.1/mkdocs.yml
+-rw-r--r--   0        0        0    16996 2020-02-02 00:00:00.000000 eins-0.1.1/network.ipynb
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 eins-0.1.1/parsing.md
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 eins-0.1.1/perf.ipynb
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 eins-0.1.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 eins-0.1.1/development_docs/README.md
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 eins-0.1.1/development_docs/ordering.md
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 eins-0.1.1/docs/in-depth.md
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 eins-0.1.1/docs/index.md
+-rw-r--r--   0        0        0    16072 2020-02-02 00:00:00.000000 eins-0.1.1/docs/tutorial.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 eins-0.1.1/docs/javascripts/katex.js
+-rw-r--r--   0        0        0   201364 2020-02-02 00:00:00.000000 eins-0.1.1/docs/stylesheets/CascadiaCode.woff2
+-rw-r--r--   0        0        0   143760 2020-02-02 00:00:00.000000 eins-0.1.1/docs/stylesheets/CascadiaCodeItalic.woff2
+-rw-r--r--   0        0        0   202128 2020-02-02 00:00:00.000000 eins-0.1.1/docs/stylesheets/InstrumentSans-Italic[wdth,wght].ttf
+-rw-r--r--   0        0        0   194336 2020-02-02 00:00:00.000000 eins-0.1.1/docs/stylesheets/InstrumentSans[wdth,wght].ttf
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 eins-0.1.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 eins-0.1.1/docs/stylesheets/readme.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 eins-0.1.1/examples/README.md
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 eins-0.1.1/examples/multi_head_attention.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 eins-0.1.1/examples/vit_encoder.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/__about__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/__init__.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/combination.py
+-rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/common_types.py
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/concrete.py
+-rw-r--r--   0        0        0     9104 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/constraint.py
+-rw-r--r--   0        0        0    19949 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/einsop.py
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/elementwise.py
+-rw-r--r--   0        0        0     7537 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/namespaces.py
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/parsing.py
+-rw-r--r--   0        0        0    14802 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/program.py
+-rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/reduction.py
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/strategy.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/symbolic.py
+-rw-r--r--   0        0        0    10981 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/transformation.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 eins-0.1.1/src/eins/utils.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 eins-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 eins-0.1.1/tests/test_basic.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 eins-0.1.1/tests/test_parsing.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 eins-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 eins-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 eins-0.1.1/README.md
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 eins-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 eins-0.1.1/PKG-INFO
```

### Comparing `eins-0.1.0/CODE_OF_CONDUCT.md` & `eins-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/CONTRIBUTING.md` & `eins-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/algorithm.md` & `eins-0.1.1/algorithm.md`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/benchmarking.ipynb` & `eins-0.1.1/benchmarking.ipynb`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/examples.ipynb` & `eins-0.1.1/examples.ipynb`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/examples.md` & `eins-0.1.1/examples.md`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/examples.py` & `eins-0.1.1/examples.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 # type: ignore
 
 from typing import cast
 
 from eins import EinsOp
 from eins import Reductions as R  # noqa: N817
-from eins import Transformations as T
-from eins.common_types import Array
+from eins import Transformations as T  # noqa: N817
+from eins.common_types import Array, ArrayBackend
 from eins.namespaces import ElementwiseOps
 
 # Set this to 'jax', 'numpy', or 'torch'
 BACKEND = 'jax'
 
 if BACKEND == 'jax':
     import jax.numpy as jnp
 
-    xp = jnp
+    xp: ArrayBackend[jnp.array] = jnp
     arr = jnp.array
 elif BACKEND == 'numpy':
     import numpy as np
 
-    xp = np
+    xp: ArrayBackend[np.ndarray] = np
     arr = np.array
 elif BACKEND == 'torch':
     import torch
 
-    xp = torch
+    xp: ArrayBackend[torch.Tensor] = torch
     arr = torch.tensor
 else:
     raise ValueError
 
 
 def randn(*shape) -> Array:
     if BACKEND == 'jax':
         import jax.numpy as jnp
         import numpy as np
 
         # TODO debug why bfloat16 doesn't work here
-        return jnp.asarray(np.random.randn(*shape))
+        return jnp.asarray(np.random.randn(*shape), dtype=jnp.bfloat16)
     elif BACKEND == 'numpy':
         import numpy as np
 
         return np.array(np.random.randn(*shape))
     elif BACKEND == 'torch':
         import torch
 
@@ -53,15 +53,24 @@
 
 
 def test_close(a: Array, b: Array):
     if a.shape != b.shape:
         msg = f'{a.shape} != {b.shape}'
         raise ValueError(msg)
     diffs = xp.mean(xp.abs(a - b))  # type: ignore
-    assert diffs.max() < EPSILON, f'{a.shape} != {b.shape}, {R.mean(a)}, {R.mean(b)}, {diffs.max()}'  # noqa: S101
+    assert (  # noqa: S101
+        diffs.max() < EPSILON
+    ), f'{a.shape} != {b.shape}, {R.mean(a.reshape(-1))}, {R.mean(b.reshape(-1))}, {diffs.max()}'
+
+
+# Unit axis
+x = randn(5)
+
+op = EinsOp('a -> ()', reduce='sum')
+test_close(op(x), xp.sum(x))
 
 
 # Softmax
 x = randn(5, 4)
 
 op = EinsOp('a b', transform={'b': ('softmax', ElementwiseOps.from_func(lambda x: x + 2))})
 y = op(x)
@@ -69,15 +78,15 @@
 y2 = T.Softmax(temperature=1)(x, axis=1)
 test_close(y, y2)
 
 # Splitting
 x, y = randn(3, 4), randn(5, 4)
 z2 = xp.concatenate((x, y), axis=0)
 
-x1 = EinsOp('α+β γ -> α γ', symbol_values={'α': x.shape[0]})(z2)
+x1 = EinsOp('λ+β Δ -> λ Δ', symbol_values={'λ': x.shape[0]})(z2)
 test_close(x1, x)
 
 # Concatenation
 
 # z1 = EinsOp('a c, b c -> a+b c')(x, y)
 # test_close(z1, z2)
```

### Comparing `eins-0.1.0/mkdocs.yml` & `eins-0.1.1/mkdocs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 nav:
   - Home: index.md
   - Tutorial: tutorial.md
   - Advanced Eins: in-depth.md
   - API Reference: $api/eins.***
 
 plugins:
-- search
-- exclude-search:
-    exclude:
-      - src/eins/*
-- mkapi
-- social
-- privacy
+  - search
+  - exclude-search:
+      exclude:
+        - src/eins/*
+  - mkapi
+  - social:
+      cards_layout: default
+  - privacy
 
 theme:
   name: material
   palette:
     - scheme: default
       primary: pink
       accent: red
```

### Comparing `eins-0.1.0/network.ipynb` & `eins-0.1.1/network.ipynb`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/parsing.md` & `eins-0.1.1/parsing.md`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/perf.ipynb` & `eins-0.1.1/perf.ipynb`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/.github/workflows/main.yml` & `eins-0.1.1/.github/workflows/main.yml`

 * *Files 12% similar despite different names*

```diff
@@ -21,10 +21,11 @@
       - run: echo "cache_id=$(date --utc '+%V')" >> $GITHUB_ENV
       - uses: actions/cache@v4
         with:
           key: mkdocs-material-${{ env.cache_id }}
           path: .cache
           restore-keys: |
             mkdocs-material-
-      - run: pip install mkdocs-material
+      - run: pip install "mkdocs-material[imaging]"
       - run: pip install mkapi
+      - run: pip install mkdocs-exclude-search
       - run: mkdocs gh-deploy --force
```

### Comparing `eins-0.1.0/docs/in-depth.md` & `eins-0.1.1/docs/in-depth.md`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/docs/index.md` & `eins-0.1.1/docs/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # Eins Documentation
-## Introduction: one tensor operation is all you need
+## Introduction: One Tensor Operation is All You Need
 
 What if most of your machine learning model code could be replaced by a single operation? Eins gives
 you a powerful language to describe array manipulation, making it a one-stop shop for all of your AI
 needs.
 
-For a sample of what Eins does, let's do [the patch embedding from a vision
+Let's say you want to compute batched pairwise distance between two batches of arrays of points:
+
+```python
+from eins import EinsOp
+EinsOp('batch n1 d, batch n2 d -> batch n1 n2',
+       combine='add', reduce='l2_norm')(pts1, -pts2)
+```
+
+If you're more interested in deep learning, here is [the patch embedding from a vision
 transformer](https://nn.labml.ai/transformers/vit/index.html#PatchEmbeddings). That means breaking
 up an image into patches and then linearly embedding each patch.
 
 ```python
 from eins import EinsOp
-patchify = EinsOp([
-    'b (n_p patch) (n_p patch) c',
-    '(patch patch c) emb',
-    'b (n_p n_p) emb'
-])
-
-kernel = randn(5 * 5 * 3, 12)
-images = randn(4, 55, 55, 3)
-patches = linear(images, kernel)
-print(patches.shape)  # (4, 121, 12)
+patchify = EinsOp('''b (n_p patch) (n_p patch) c, (patch patch c) emb -> b (n_p n_p) emb''')
+patches = patchify(images, kernel)
 ```
 
 ## Installation
 
 Eins just has a few pure Python dependencies, and installation should be as easy as:
 
 ```console
```

### Comparing `eins-0.1.0/docs/tutorial.md` & `eins-0.1.1/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/docs/stylesheets/CascadiaCode.woff2` & `eins-0.1.1/docs/stylesheets/CascadiaCode.woff2`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/docs/stylesheets/CascadiaCodeItalic.woff2` & `eins-0.1.1/docs/stylesheets/CascadiaCodeItalic.woff2`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/docs/stylesheets/InstrumentSans-Italic[wdth,wght].ttf` & `eins-0.1.1/docs/stylesheets/InstrumentSans-Italic[wdth,wght].ttf`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/docs/stylesheets/InstrumentSans[wdth,wght].ttf` & `eins-0.1.1/docs/stylesheets/InstrumentSans[wdth,wght].ttf`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/docs/stylesheets/extra.css` & `eins-0.1.1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/docs/stylesheets/readme.md` & `eins-0.1.1/docs/stylesheets/readme.md`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/examples/README.md` & `eins-0.1.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/examples/multi_head_attention.py` & `eins-0.1.1/examples/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/examples/vit_encoder.py` & `eins-0.1.1/examples/vit_encoder.py`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/src/eins/combination.py` & `eins-0.1.1/src/eins/combination.py`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/src/eins/concrete.py` & `eins-0.1.1/src/eins/concrete.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,18 @@
                 tiles = []
                 if len(op.new_shape) != len(x[0].shape):
                     msg = f'Shape {x[0].shape} cannot be tiled to{op.new_shape}: shapes must match.'
                     raise ValueError(msg)
 
                 for out_ax, in_len in zip(op.new_shape, x[0].shape):
                     out_len = self.constr.value_of(out_ax)
+                    if out_len is None:
+                        msg = f'Could not compute value of {out_ax} for tile operation.'
+                        raise ValueError(msg)
+
                     if out_len % in_len != 0:
                         msg = f'Cannot tile: {in_len} does not divide {out_len}'
                         msg += f': {x[0]}, {op.new_shape}'
                         raise ValueError(msg)
                     tiles.append(out_len // in_len)
 
                 if hasattr(xp, 'tile'):
```

### Comparing `eins-0.1.0/src/eins/constraint.py` & `eins-0.1.1/src/eins/constraint.py`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/src/eins/einsop.py` & `eins-0.1.1/src/eins/einsop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """User-facing API."""
 
 import typing
 from itertools import chain
 from string import ascii_uppercase
-from typing import AnyStr, Callable, Mapping, MutableMapping, Optional, Sequence, Union
+from typing import AnyStr, Callable, List, Mapping, MutableMapping, Optional, Sequence, Union, cast
 
 from eins.combination import (
     Combination,
     CombineLiteral,
     CompositeCombination,
     CustomCombination,
     parse_combination,
@@ -125,15 +125,17 @@
     elif isinstance(transform, Callable):
         return CustomTransformation(transform)
     elif isinstance(transform, str):
         combo_parse = parse_transformation(transform)
         if combo_parse is not None:
             return combo_parse
 
-        msg = f'Cannot parse transformation {transform}. Valid literals: {", ".join(_transformation_ops)}'
+        msg = f'Cannot parse transformation {transform}. Valid literals: ' + ', '.join(
+            _transformation_ops
+        )
         raise ValueError(msg)
     else:
         ops = []
         for op in transform:
             if isinstance(op, (ElementwiseOp, Transformation)):
                 ops.append(op)
                 continue
@@ -210,15 +212,15 @@
 
 
 class EinsOp:
     """A computation on tensors, defined abstractly without specific inputs."""
 
     def __init__(
         self,
-        op: str,
+        op: Union[str, Sequence[str]],
         /,
         *,
         reduce: ReduceArg = 'sum',
         combine: CombineArg = 'multiply',
         transform: Optional[Mapping[str, TransformArg]] = None,
         symbol_values: Optional[Mapping[str, int]] = None,
     ):
@@ -419,15 +421,17 @@
             for op, children in src.children:
                 if len(children) == 1:
                     # could be a many-to-one op
                     child = children[0]
                     concrete_parents = [self.concrete.get(id(parent)) for parent in child.parents]
                     if all(p is not None for p in concrete_parents):
                         # we can fill in this operation
-                        result = self.backend.do(concrete_parents, op, child.parents, [child])[0]
+                        result = self.backend.do(
+                            cast(List[Array], concrete_parents), op, child.parents, [child]
+                        )[0]
                         instructions.append((op, list(map(id, child.parents)), [id(child)]))
                         # type: ignore
                         res = fill_from(child, result)
                         leaves.extend(res)
 
                 else:
                     # no many-to-many ops: we can fill in all of these
@@ -444,15 +448,15 @@
             for src, arr in zip(self.program.sources, tensors):
                 ans = fill_from(src, arr)
                 leaves.extend(ans)
 
             self.out_shape = [
                 self.program.constr.value_of(ax) for ax in self.program.orig_sink.axes
             ]
-            potential_returns = [l for l in leaves if list(l.shape) == self.out_shape]
+            potential_returns = [leaf for leaf in leaves if list(leaf.shape) == self.out_shape]
             if potential_returns:
                 ans = potential_returns[-1]
                 self.abstract[id(ans)] = self.program.orig_sink
                 # the concrete arrays are large: we don't want to store them indefinitely
                 self.concrete.clear()
                 return ans
         except ValueError as err:
```

### Comparing `eins-0.1.0/src/eins/elementwise.py` & `eins-0.1.1/src/eins/elementwise.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Elementwise operations, for use in combination with reduction operations."""
 
-import math
 import typing
 from dataclasses import dataclass
-from typing import Callable, Literal, Optional, Sequence, Union
+from typing import Callable, Literal, Optional, Union
 
 import array_api_compat
 
 from eins.common_types import Array, ElementwiseFunc, ElementwiseOp
 from eins.utils import array_backend
 
 # https://data-apis.org/array-api/latest/API_specification/elementwise_functions.html Every method
@@ -116,15 +115,15 @@
     specific performance-optimized versions we'd like to use, but we can implement it ourselves if
     we need to (e.g., in numpy).
 
     Strings are members of a submodule of the overarching module for each array API, which helps
     avoid requiring any of the individual backends.
     """
 
-    generic: Callable
+    generic: ElementwiseFunc
     numpy: Union[Callable, str, None]
     jax: Union[Callable, str, None]
     torch: Union[Callable, str, None]
 
     @staticmethod
     def get_method(func_or_name: Union[Callable, str], module: str):
         if isinstance(func_or_name, str):
@@ -143,15 +142,15 @@
         if array_api_compat.is_torch_array(arr):
             module = 'torch'
         elif array_api_compat.is_jax_array(arr):
             module = 'jax'
         elif array_api_compat.is_numpy_array(arr):
             module = 'numpy'
         else:
-            return self.generic(arr, axis=axis)
+            return self.generic(arr)
 
         func = getattr(self, module)
         if func is None:
             func = self.generic
 
         try:
             return self.get_method(func, module)(arr)
```

### Comparing `eins-0.1.0/src/eins/namespaces.py` & `eins-0.1.1/src/eins/namespaces.py`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/src/eins/parsing.py` & `eins-0.1.1/src/eins/parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 pows_paren = re.compile(r'(\{[^{}]+\})\^(\d+)')
 pows_atomic = re.compile(r'([^{} +*/-]+)\^(\d+)')
 
 
 def unpack_parens(m: re.Match):
     body = m.group()[1:-1]
     exprs = body.split(' ')
-    return lparen + '*'.join(f'{lparen}{expr}{rparen}' for expr in exprs) + rparen
+    return lparen + '*'.join(f'{lparen}{expr}{rparen}' for expr in exprs if expr) + rparen
 
 
 def unpack_index(m: re.Match):
     ind, *rest = m.groups()
     return ' '.join(rest) + f' @ {ind}'
 
 
@@ -42,15 +42,14 @@
         num_times += 1
         if num_times > MAX_NESTED_PARENS:
             msg = 'Stack overflow'
             raise ValueError(msg)
         new_expr, expr = re.sub(parens, unpack_parens, new_expr), new_expr
 
     expr = re.sub(index, unpack_index, new_expr)
-
     return expr
 
 
 # parse = parse_einop('b (d=(n p) d) c, b p*p*c h, h[k] -> b n n k') parse = parse_einop('b k=(a a)
 # a -> a b') pprint.pprint(parse)
 
 # b ((d=((n)*(p)))*(d)) c, b p*p*c h, h[] k -> b n n k
@@ -63,23 +62,24 @@
 comma_op = spaces + pp.Literal(',') + spaces
 seq_op = pp.Literal(' ')
 add_op = pp.one_of('+ -')
 mul_op = pp.one_of('* /')
 pow_op = pp.one_of('^')
 arrow = spaces + pp.Literal('->') + spaces
 index_op = spaces + pp.one_of('@') + spaces
+unit = pp.Literal('()')
 
 symbol = pp.Word(
     pp.pyparsing_unicode.identchars,
     pp.pyparsing_unicode.identbodychars,
     exclude_chars='+-*/^()[] ->',
 )
 literal = pp.Word(pp.nums)
 
-operand = symbol | literal
+operand = symbol | literal | unit
 
 expr = pp.infix_notation(
     operand,
     [
         (pow_op, 2, pp.OpAssoc.LEFT),
         (mul_op, 2, pp.OpAssoc.LEFT),
         (add_op, 2, pp.OpAssoc.LEFT),
@@ -132,14 +132,16 @@
         return f'({self.op} ' + ' '.join(map(str, self.children)) + ')'
 
 
 def make_expr(parsed: Union[list, str]) -> Node:
     if isinstance(parsed, str):
         if parsed.isdigit():
             return Constant(int(parsed))
+        elif parsed == '()':
+            return Expr(' ', [])
         else:
             return Symbol(parsed)
     else:
         if len(parsed) == 1:
             return make_expr(parsed[0])
 
         lhs, op, *rhs = parsed
```

### Comparing `eins-0.1.0/src/eins/program.py` & `eins-0.1.1/src/eins/program.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Ruff *really* does not like magic numbers!
 import pprint
 from collections import defaultdict
 from copy import deepcopy
 from itertools import chain
-from typing import Mapping, MutableSequence, Sequence, Tuple, Union, cast
+from typing import Mapping, MutableSequence, Sequence, Union, cast
 
 from eins.combination import ArrayCombination
 from eins.common_types import Combination, Reduction, Transformation
 from eins.constraint import Constraints, postprocess_ast
 from eins.parsing import Constant, Expr, Node, Symbol, make_expr, unpack_shorthands
 from eins.parsing import expr as expr_parser
 from eins.reduction import ArrayReduction
@@ -154,15 +154,15 @@
 
         for t in self.current + self.sinks:
             self.constr.add_variables(t.axes_list())
 
         self.combine = combine
 
         if isinstance(reduce, Reduction):
-            self.reduce = defaultdict(lambda: reduce)
+            self.reduce: Mapping[str, Reduction] = defaultdict(lambda: reduce)
         else:
             self.reduce = dict(reduce)
             # we may have already renamed axes, but the user is passing in the old names
             # e.g., a b b, c b b -> a, reduce={'b': 'mean', 'c': 'sum'}
             # b now is b-1 and b-2
             for lhs, rhs in self.constr.equations:
                 if isinstance(rhs, Symbol) and isinstance(lhs, Symbol):
```

### Comparing `eins-0.1.0/src/eins/reduction.py` & `eins-0.1.1/src/eins/reduction.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 from dataclasses import dataclass
 from functools import reduce
 from itertools import chain
 from math import isnan
 from typing import Literal, Optional, Sequence, Union
 
 from eins.combination import Combination, parse_combination
-from eins.common_types import Array, ElementwiseOp, Reduction, ReductionFunc, Transformation
+from eins.common_types import (
+    Array,
+    ElementwiseOp,
+    Reduction,
+    ReductionFunc,
+    Transformation,
+    call_axis_func,
+)
 from eins.utils import array_backend
 
 # https://data-apis.org/array-api/latest/API_specification/statistical_functions.html
 ArrayReductionLiteral = Literal['max', 'mean', 'min', 'prod', 'std', 'sum', 'var']
 
 ARRAY_REDUCE_OPS = [str(x) for x in typing.get_args(ArrayReductionLiteral)]
 
@@ -218,15 +225,15 @@
     """Reduction using a user-defined function.
 
     func must take in an array and an axis argument, returning an array with that axis removed."""
 
     func: ReductionFunc
 
     def __call__(self, arr: Array, axis: int = 0) -> Array:
-        return self.func(arr, axis=axis)
+        return call_axis_func(self.func, arr, axis=axis)
 
 
 def parse_reduction(name: str) -> Optional[Reduction]:
     for cls in (ArrayReduction, Fold, PowerNorm, Range):
         parse = cls.parse(name)
         if parse is not None:
             return parse
```

### Comparing `eins-0.1.0/src/eins/strategy.py` & `eins-0.1.1/src/eins/strategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Abstraction of different algorithmic choices made during program execution."""
 
 from collections import defaultdict
 from typing import Sequence, Union
 
-from eins.common_types import Transformation
-from eins.parsing import Constant, Symbol
+from eins.parsing import Symbol
 from eins.program import Program
-from eins.symbolic import Combine, ExpandTo, Reduce, ShapeOp, Tensor, Tile, Transform, Transpose
+from eins.symbolic import Combine, ExpandTo, Reduce, ShapeOp, Tensor, Tile, Transpose
 
 
 class BaseStrategy:
     """Base strategy: implements simple defaults and implements higher-order logic that doesn't
     usually need to change."""
 
     def __init__(self, prog: Program, reduce_early: bool = True) -> None:  # noqa: FBT001, FBT002
```

### Comparing `eins-0.1.0/src/eins/symbolic.py` & `eins-0.1.1/src/eins/symbolic.py`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/src/eins/transformation.py` & `eins-0.1.1/src/eins/transformation.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,16 +95,26 @@
             return cls(combo)
         else:
             return None
 
     def __call__(self, arr: Array, axis: int = 0) -> Array:
         xp = array_backend(arr)
         if xp is not None:
-            slices = xp.unstack(arr, axis=axis)
-            return cast(Array, accumulate(slices, self.combination))
+            # the array API *should* have unstack, but that's not in every version.
+            # So we implement it a worse way.
+            if hasattr(xp, 'unstack'):
+                stacks = xp.unstack(arr, axis=axis)  # type: ignore
+            else:
+                slc: list[Union[slice, int]] = [slice(None)] * arr.ndim
+                stacks = []
+                for i in range(arr.shape[axis]):
+                    slc[axis] = i
+                    stacks.append(arr[tuple(slc)])
+                    slc[axis] = slice(None)
+            return cast(Array, accumulate(stacks, self.combination))
         else:
             msg = f'Cannot scan over non-Array {arr} of type {type(arr)}'
             raise ValueError(msg)
 
 
 DEFAULT_NORM = PowerNorm()
 NormalizeLiteral = Literal['normalize', 'l2_normalize', 'l1_normalize', 'inf_normalize']
```

### Comparing `eins-0.1.0/tests/test_basic.py` & `eins-0.1.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/LICENSE.txt` & `eins-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eins-0.1.0/README.md` & `eins-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,30 @@
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
 
 What if most of your machine learning model code could be replaced by a single operation? Eins gives
 you a powerful language to describe array manipulation, making it a one-stop shop for all of your AI
 needs.
 
-For a sample of what Eins does, let's do [the patch embedding from a vision
+Let's say you want to compute batched pairwise distance between two batches of arrays of points:
+
+```python
+from eins import EinsOp
+EinsOp('batch n1 d, batch n2 d -> batch n1 n2',
+       combine='add', reduce='l2_norm')(pts1, -pts2)
+```
+
+If you're more interested in deep learning, here is [the patch embedding from a vision
 transformer](https://nn.labml.ai/transformers/vit/index.html#PatchEmbeddings). That means breaking
 up an image into patches and then linearly embedding each patch.
 
 ```python
 from eins import EinsOp
 patchify = EinsOp('''b (n_p patch) (n_p patch) c, (patch patch c) emb -> b (n_p n_p) emb''')
-
-kernel = randn(5 * 5 * 3, 12)
-images = randn(4, 55, 55, 3)
-patches = linear(images, kernel)
-print(patches.shape)  # (4, 121, 12)
+patches = patchify(images, kernel)
 ```
 
 You input the shapes and Eins will figure out what to do.
 
 If you've used [`einops`](https://github.com/arogozhnikov/einops), then think of Eins as `einops`
 with a more ambitious goal—being the only operation you should need for your next deep learning
 project.
```

### Comparing `eins-0.1.0/pyproject.toml` & `eins-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Typing :: Typed",
 ]
-dependencies = ["array-api-compat", "pyparsing"]
+dependencies = ["array-api-compat", "pyparsing", "typing-extensions"]
 
 [project.urls]
 Documentation = "https://github.com/nicholas-miklaucic/eins#readme"
 Issues = "https://github.com/nicholas-miklaucic/eins/issues"
 Source = "https://github.com/nicholas-miklaucic/eins"
 
 [tool.hatch.version]
```

### Comparing `eins-0.1.0/PKG-INFO` & `eins-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: eins
-Version: 0.1.0
+Version: 0.1.1
 Summary: One tensor operation is all you need
 Project-URL: Documentation, https://github.com/nicholas-miklaucic/eins#readme
 Project-URL: Issues, https://github.com/nicholas-miklaucic/eins/issues
 Project-URL: Source, https://github.com/nicholas-miklaucic/eins
 Author-email: Nicholas Miklaucic <nicholas.miklaucic@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -23,14 +23,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: array-api-compat
 Requires-Dist: pyparsing
+Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # eins
 
 ## One tensor operation is all you need
 
 [![PyPI - Version](https://img.shields.io/pypi/v/eins.svg)](https://pypi.org/project/eins)
@@ -38,26 +39,30 @@
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
 
 What if most of your machine learning model code could be replaced by a single operation? Eins gives
 you a powerful language to describe array manipulation, making it a one-stop shop for all of your AI
 needs.
 
-For a sample of what Eins does, let's do [the patch embedding from a vision
+Let's say you want to compute batched pairwise distance between two batches of arrays of points:
+
+```python
+from eins import EinsOp
+EinsOp('batch n1 d, batch n2 d -> batch n1 n2',
+       combine='add', reduce='l2_norm')(pts1, -pts2)
+```
+
+If you're more interested in deep learning, here is [the patch embedding from a vision
 transformer](https://nn.labml.ai/transformers/vit/index.html#PatchEmbeddings). That means breaking
 up an image into patches and then linearly embedding each patch.
 
 ```python
 from eins import EinsOp
 patchify = EinsOp('''b (n_p patch) (n_p patch) c, (patch patch c) emb -> b (n_p n_p) emb''')
-
-kernel = randn(5 * 5 * 3, 12)
-images = randn(4, 55, 55, 3)
-patches = linear(images, kernel)
-print(patches.shape)  # (4, 121, 12)
+patches = patchify(images, kernel)
 ```
 
 You input the shapes and Eins will figure out what to do.
 
 If you've used [`einops`](https://github.com/arogozhnikov/einops), then think of Eins as `einops`
 with a more ambitious goal—being the only operation you should need for your next deep learning
 project.
```

