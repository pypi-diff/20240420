# Comparing `tmp/local-attention-1.9.0.tar.gz` & `tmp/local_attention-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-attention-1.9.0.tar", last modified: Tue Oct 24 17:30:53 2023, max compression
+gzip compressed data, was "local_attention-1.9.1.tar", last modified: Sat Apr 20 19:32:59 2024, max compression
```

## Comparing `local-attention-1.9.0.tar` & `local_attention-1.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 17:30:53.760884 local-attention-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-10-24 17:30:39.000000 local-attention-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-10-24 17:30:53.756883 local-attention-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2023-10-24 17:30:39.000000 local-attention-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 17:30:53.756883 local-attention-1.9.0/local_attention/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-10-24 17:30:39.000000 local-attention-1.9.0/local_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2023-10-24 17:30:39.000000 local-attention-1.9.0/local_attention/local_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2023-10-24 17:30:39.000000 local-attention-1.9.0/local_attention/rotary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2023-10-24 17:30:39.000000 local-attention-1.9.0/local_attention/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 17:30:53.756883 local-attention-1.9.0/local_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-10-24 17:30:53.000000 local-attention-1.9.0/local_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-10-24 17:30:53.000000 local-attention-1.9.0/local_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 17:30:53.000000 local-attention-1.9.0/local_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 17:30:53.000000 local-attention-1.9.0/local_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-24 17:30:53.000000 local-attention-1.9.0/local_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-24 17:30:53.760884 local-attention-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-10-24 17:30:39.000000 local-attention-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:32:59.051707 local_attention-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-20 19:32:55.000000 local_attention-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-20 19:32:59.051707 local_attention-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-20 19:32:55.000000 local_attention-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:32:59.051707 local_attention-1.9.1/local_attention/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-20 19:32:55.000000 local_attention-1.9.1/local_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-20 19:32:55.000000 local_attention-1.9.1/local_attention/local_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-20 19:32:55.000000 local_attention-1.9.1/local_attention/rotary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-20 19:32:55.000000 local_attention-1.9.1/local_attention/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:32:59.051707 local_attention-1.9.1/local_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-20 19:32:59.000000 local_attention-1.9.1/local_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-20 19:32:59.000000 local_attention-1.9.1/local_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 19:32:59.000000 local_attention-1.9.1/local_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-20 19:32:59.000000 local_attention-1.9.1/local_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 19:32:59.000000 local_attention-1.9.1/local_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 19:32:59.051707 local_attention-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-20 19:32:55.000000 local_attention-1.9.1/setup.py
```

### Comparing `local-attention-1.9.0/LICENSE` & `local_attention-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `local-attention-1.9.0/PKG-INFO` & `local_attention-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local-attention
-Version: 1.9.0
+Version: 1.9.1
 Summary: Local attention, window with lookback, for language modeling
 Home-page: https://github.com/lucidrains/local-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: transformers,attention,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `local-attention-1.9.0/README.md` & `local_attention-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `local-attention-1.9.0/local_attention/local_attention.py` & `local_attention-1.9.1/local_attention/local_attention.py`

 * *Files identical despite different names*

### Comparing `local-attention-1.9.0/local_attention/rotary.py` & `local_attention-1.9.1/local_attention/rotary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import torch
 from torch import nn, einsum
+from torch.cuda.amp import autocast
 
 from einops import rearrange
 
 def exists(val):
     return val is not None
 
 class SinusoidalEmbeddings(nn.Module):
@@ -23,14 +24,15 @@
         self.scale_base = scale_base
 
         assert not (use_xpos and not exists(scale_base)), 'scale base must be defined if using xpos'
 
         scale = (torch.arange(0, dim, 2) + 0.4 * dim) / (1.4 * dim)
         self.register_buffer('scale', scale, persistent = False)
 
+    @autocast(enabled = False)
     def forward(self, x):
         seq_len, device = x.shape[-2], x.device
 
         t = torch.arange(seq_len, device = x.device).type_as(self.inv_freq)
         freqs = torch.einsum('i , j -> i j', t, self.inv_freq)
         freqs =  torch.cat((freqs, freqs), dim = -1)
 
@@ -44,14 +46,15 @@
         return freqs, scale
 
 def rotate_half(x):
     x = rearrange(x, 'b ... (r d) -> b ... r d', r = 2)
     x1, x2 = x.unbind(dim = -2)
     return torch.cat((-x2, x1), dim = -1)
 
+@autocast(enabled = False)
 def apply_rotary_pos_emb(q, k, freqs, scale = 1):
     q_len = q.shape[-2]
     q_freqs = freqs[..., -q_len:, :]
 
     inv_scale = scale ** -1
 
     if scale.ndim == 2:
```

### Comparing `local-attention-1.9.0/local_attention/transformer.py` & `local_attention-1.9.1/local_attention/transformer.py`

 * *Files identical despite different names*

### Comparing `local-attention-1.9.0/local_attention.egg-info/PKG-INFO` & `local_attention-1.9.1/local_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local-attention
-Version: 1.9.0
+Version: 1.9.1
 Summary: Local attention, window with lookback, for language modeling
 Home-page: https://github.com/lucidrains/local-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: transformers,attention,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `local-attention-1.9.0/setup.py` & `local_attention-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'local-attention',
   packages = find_packages(),
-  version = '1.9.0',
+  version = '1.9.1',
   license='MIT',
   description = 'Local attention, window with lookback, for language modeling',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/local-attention',
   keywords = [
```

