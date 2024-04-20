# Comparing `tmp/ring-attention-pytorch-0.3.9.tar.gz` & `tmp/ring_attention_pytorch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ring-attention-pytorch-0.3.9.tar", last modified: Wed Apr 10 13:59:20 2024, max compression
+gzip compressed data, was "ring_attention_pytorch-0.4.0.tar", last modified: Sat Apr 20 14:08:41 2024, max compression
```

## Comparing `ring-attention-pytorch-0.3.9.tar` & `ring_attention_pytorch-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:59:20.484446 ring-attention-pytorch-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-10 13:59:20.484446 ring-attention-pytorch-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:59:20.480446 ring-attention-pytorch-0.3.9/ring_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring.py
--rw-r--r--   0 runner    (1001) docker     (127)    18780 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12278 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    25569 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring_flash_attention_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:59:20.480446 ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-10 13:59:20.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 13:59:20.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:59:20.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-10 13:59:20.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 13:59:20.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:59:20.484446 ring-attention-pytorch-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:08:41.599834 ring_attention_pytorch-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-20 14:08:31.000000 ring_attention_pytorch-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-20 14:08:41.599834 ring_attention_pytorch-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-20 14:08:31.000000 ring_attention_pytorch-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:08:41.599834 ring_attention_pytorch-0.4.0/ring_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-20 14:08:31.000000 ring_attention_pytorch-0.4.0/ring_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-20 14:08:31.000000 ring_attention_pytorch-0.4.0/ring_attention_pytorch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-20 14:08:31.000000 ring_attention_pytorch-0.4.0/ring_attention_pytorch/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19610 2024-04-20 14:08:31.000000 ring_attention_pytorch-0.4.0/ring_attention_pytorch/ring_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-04-20 14:08:31.000000 ring_attention_pytorch-0.4.0/ring_attention_pytorch/ring_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-04-20 14:08:31.000000 ring_attention_pytorch-0.4.0/ring_attention_pytorch/ring_flash_attention_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33543 2024-04-20 14:08:31.000000 ring_attention_pytorch-0.4.0/ring_attention_pytorch/triton_flash_attn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:08:41.599834 ring_attention_pytorch-0.4.0/ring_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-20 14:08:41.000000 ring_attention_pytorch-0.4.0/ring_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-20 14:08:41.000000 ring_attention_pytorch-0.4.0/ring_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 14:08:41.000000 ring_attention_pytorch-0.4.0/ring_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-20 14:08:41.000000 ring_attention_pytorch-0.4.0/ring_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 14:08:41.000000 ring_attention_pytorch-0.4.0/ring_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 14:08:41.599834 ring_attention_pytorch-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-20 14:08:31.000000 ring_attention_pytorch-0.4.0/setup.py
```

### Comparing `ring-attention-pytorch-0.3.9/LICENSE` & `ring_attention_pytorch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.9/PKG-INFO` & `ring_attention_pytorch-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.9
+Version: 0.4.0
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.9/README.md` & `ring_attention_pytorch-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 It basically splits the data across the sequence dimension (instead of batch) and applies ring reduce to the processing of the tiles of the attention matrix, flash attention style.
 
 I believe this is being used for the 1-10 million tokens for the latest Gemini. At least some form of it; the other possibility would be unpublished improvements on top of <a href="https://github.com/lucidrains/recurrent-memory-transformer-pytorch">RMT</a>.
 
 In addition, the repository also contains the logic for <a href="https://arxiv.org/abs/2311.09431">Striped Attention</a>, a follow up paper that permutes the sequence for better workload balancing for autoregressive transformers.
 
+It also contains support for <a href="https://arxiv.org/abs/2305.13245">grouped query attention</a>, popularized by Llama series of attention models. This will further save on communication costs during the ring reduce.
+
 ## Appreciation
 
 - <a href="https://a16z.com/supporting-the-open-source-ai-community/">A16Z Open Source AI Grant Program</a> for the generous sponsorship, as well as my other sponsors, for affording me the independence to open source current artificial intelligence research
 
 - <a href="https://tridao.me/">Tri Dao</a> for all his tremendous hard work maintaining <a href="https://github.com/Dao-AILab/flash-attention">Flash Attention</a> over the last year or two, from which the CUDA version in this repository depends on
 
 - Phil Tillet for <a href="https://github.com/openai/triton">Triton</a>, without which the forward ring flash attention CUDA kernel would have taken a magnitude of order more work.
@@ -94,20 +96,21 @@
     - [x] prevent an unnecessary `tl.load` on the first ring pass
     - [x] cuda backwards pass must have same dq, dk, dv as naive
 - [x] fix naive flash attention backwards
 - [x] validate cuda causal and striped ring attention works
 - [x] make sure cuda striped attention works for multiple buckets, otherwise flash attention is ineffective
 - [x] for cuda striped attention, for backwards hack, pad the extra token once and index out when passing into Tri's cuda kernel
 - [x] find a machine with 8 GPUs and test with a quarter million tokens first
+- [x] see for cuda version whether softmax_D can be computed once and cached over the ring reduce. go for modified triton backwards if not
 
-- [ ] see for cuda version whether softmax_D can be computed once and cached over the ring reduce. go for modified triton backwards if not
 - [ ] think about how to craft a special `Dataset` that shards across sequence length (take into account labels for cross entropy loss) for ring transformer training
 - [ ] add ring attention to Tri's flash attention implementation. find some cuda ring reduce impl
 - [ ] figure out how to pytest distributed pytorch
 - [ ] use sdp context manager to validate when it is possible to use `ring_flash_attn_cuda`, otherwise assert out
+- [ ] improvise a variant where each machine keeps compressed summary tokens, and one only ring pass those summary token for some given distance
 
 ## Citations
 
 ```bibtex
 @article{Liu2023RingAW,
     title    = {Ring Attention with Blockwise Transformers for Near-Infinite Context},
     author   = {Hao Liu and Matei Zaharia and Pieter Abbeel},
@@ -152,7 +155,19 @@
     title   = {Triton: an intermediate language and compiler for tiled neural network computations},
     author  = {Philippe Tillet and H. Kung and D. Cox},
     journal = {Proceedings of the 3rd ACM SIGPLAN International Workshop on Machine Learning and Programming Languages},
     year    = {2019}
 }
 ```
 
+```bibtex
+@article{Ainslie2023GQATG,
+    title   = {GQA: Training Generalized Multi-Query Transformer Models from Multi-Head Checkpoints},
+    author  = {Joshua Ainslie and James Lee-Thorp and Michiel de Jong and Yury Zemlyanskiy and Federico Lebr'on and Sumit K. Sanghai},
+    journal = {ArXiv},
+    year    = {2023},
+    volume  = {abs/2305.13245},
+    url     = {https://api.semanticscholar.org/CorpusID:258833177}
+}
+```
+
+*<a href="http://www.incompleteideas.net/IncIdeas/BitterLesson.html">The Bitter Lesson</a>* - Richard Sutton
```

#### html2text {}

```diff
@@ -2,21 +2,23 @@
 _L_i_u et al. at Berkeley AI, in Pytorch. It basically splits the data across the
 sequence dimension (instead of batch) and applies ring reduce to the processing
 of the tiles of the attention matrix, flash attention style. I believe this is
 being used for the 1-10 million tokens for the latest Gemini. At least some
 form of it; the other possibility would be unpublished improvements on top of
 _R_M_T. In addition, the repository also contains the logic for _S_t_r_i_p_e_d_ _A_t_t_e_n_t_i_o_n,
 a follow up paper that permutes the sequence for better workload balancing for
-autoregressive transformers. ## Appreciation - _A_1_6_Z_ _O_p_e_n_ _S_o_u_r_c_e_ _A_I_ _G_r_a_n_t
-_P_r_o_g_r_a_m for the generous sponsorship, as well as my other sponsors, for
-affording me the independence to open source current artificial intelligence
-research - _T_r_i_ _D_a_o for all his tremendous hard work maintaining _F_l_a_s_h_ _A_t_t_e_n_t_i_o_n
-over the last year or two, from which the CUDA version in this repository
-depends on - Phil Tillet for _T_r_i_t_o_n, without which the forward ring flash
-attention CUDA kernel would have taken a magnitude of order more work. ##
+autoregressive transformers. It also contains support for _g_r_o_u_p_e_d_ _q_u_e_r_y
+_a_t_t_e_n_t_i_o_n, popularized by Llama series of attention models. This will further
+save on communication costs during the ring reduce. ## Appreciation - _A_1_6_Z_ _O_p_e_n
+_S_o_u_r_c_e_ _A_I_ _G_r_a_n_t_ _P_r_o_g_r_a_m for the generous sponsorship, as well as my other
+sponsors, for affording me the independence to open source current artificial
+intelligence research - _T_r_i_ _D_a_o for all his tremendous hard work maintaining
+_F_l_a_s_h_ _A_t_t_e_n_t_i_o_n over the last year or two, from which the CUDA version in this
+repository depends on - Phil Tillet for _T_r_i_t_o_n, without which the forward ring
+flash attention CUDA kernel would have taken a magnitude of order more work. ##
 Install ```bash $ pip install ring-attention-pytorch ``` ## Usage ```python
 import torch from ring_attention_pytorch import RingAttention attn =
 RingAttention( dim = 512, dim_head = 64, heads = 8, causal = True,
 auto_shard_seq = True, ring_attn = True, ring_seq_size = 512 ) tokens =
 torch.randn(1, 1024, 512) attended = attn(tokens) assert attended.shape ==
 tokens.shape ``` ## Test First install requirements ```bash $ pip install -
 r requirements.txt ``` Then say testing autoregressive striped ring attention
@@ -54,22 +56,24 @@
 float16 - [x] prevent an unnecessary `tl.load` on the first ring pass - [x]
 cuda backwards pass must have same dq, dk, dv as naive - [x] fix naive flash
 attention backwards - [x] validate cuda causal and striped ring attention works
 - [x] make sure cuda striped attention works for multiple buckets, otherwise
 flash attention is ineffective - [x] for cuda striped attention, for backwards
 hack, pad the extra token once and index out when passing into Tri's cuda
 kernel - [x] find a machine with 8 GPUs and test with a quarter million tokens
-first - [ ] see for cuda version whether softmax_D can be computed once and
+first - [x] see for cuda version whether softmax_D can be computed once and
 cached over the ring reduce. go for modified triton backwards if not - [ ]
 think about how to craft a special `Dataset` that shards across sequence length
 (take into account labels for cross entropy loss) for ring transformer training
 - [ ] add ring attention to Tri's flash attention implementation. find some
 cuda ring reduce impl - [ ] figure out how to pytest distributed pytorch - [ ]
 use sdp context manager to validate when it is possible to use
-`ring_flash_attn_cuda`, otherwise assert out ## Citations ```bibtex @article
+`ring_flash_attn_cuda`, otherwise assert out - [ ] improvise a variant where
+each machine keeps compressed summary tokens, and one only ring pass those
+summary token for some given distance ## Citations ```bibtex @article
 {Liu2023RingAW, title = {Ring Attention with Blockwise Transformers for Near-
 Infinite Context}, author = {Hao Liu and Matei Zaharia and Pieter Abbeel},
 journal = {ArXiv}, year = {2023}, volume = {abs/2310.01889}, url = {https://
 api.semanticscholar.org/CorpusID:263608461} } ``` ```bibtex @article
 {Brandon2023StripedAF, title = {Striped Attention: Faster Ring Attention for
 Causal Transformers}, author = {William Brandon and Aniruddha Nrusimha and
 Kevin Qian and Zachary Ankner and Tian Jin and Zhiye Song and Jonathan Ragan-
@@ -81,8 +85,13 @@
 {2022}, volume = {abs/2205.14135} } ``` ```bibtex @article
 {dao2023flashattention2, title = {Flash{A}ttention-2: Faster Attention with
 Better Parallelism and Work Partitioning, author = {Dao, Tri}, year = {2023} }
 ``` ```bibtex @article{Tillet2019TritonAI, title = {Triton: an intermediate
 language and compiler for tiled neural network computations}, author =
 {Philippe Tillet and H. Kung and D. Cox}, journal = {Proceedings of the 3rd ACM
 SIGPLAN International Workshop on Machine Learning and Programming Languages},
-year = {2019} } ```
+year = {2019} } ``` ```bibtex @article{Ainslie2023GQATG, title = {GQA: Training
+Generalized Multi-Query Transformer Models from Multi-Head Checkpoints}, author
+= {Joshua Ainslie and James Lee-Thorp and Michiel de Jong and Yury Zemlyanskiy
+and Federico Lebr'on and Sumit K. Sanghai}, journal = {ArXiv}, year = {2023},
+volume = {abs/2305.13245}, url = {https://api.semanticscholar.org/CorpusID:
+258833177} } ``` *_T_h_e_ _B_i_t_t_e_r_ _L_e_s_s_o_n* - Richard Sutton
```

### Comparing `ring-attention-pytorch-0.3.9/ring_attention_pytorch/distributed.py` & `ring_attention_pytorch-0.4.0/ring_attention_pytorch/distributed.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,17 +62,26 @@
     gathered_tensors = gathered_tensors.index_select(dim, indices)
 
     return gathered_tensors, sizes
 
 class AllGatherFunction(Function):
     @staticmethod
     def forward(ctx, x, dim, sizes):
+        is_bool = x.dtype == torch.bool
+
+        if is_bool:
+            x = x.int()
+
         x, batch_sizes = all_gather_variable_dim(x, dim = dim, sizes = sizes)
         ctx.batch_sizes = batch_sizes.tolist()
         ctx.dim = dim
+
+        if is_bool:
+            x = x.bool()
+
         return x, batch_sizes
 
     @staticmethod
     def backward(ctx, grads, _):
         batch_sizes, rank = ctx.batch_sizes, dist.get_rank()
         grads_by_rank = grads.split(batch_sizes, dim = ctx.dim)
         return grads_by_rank[rank], None, None
```

### Comparing `ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring.py` & `ring_attention_pytorch-0.4.0/ring_attention_pytorch/ring.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring_attention.py` & `ring_attention_pytorch-0.4.0/ring_attention_pytorch/ring_attention.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 def cast_tuple(t, length = 1):
     return t if isinstance(t, tuple) else ((t,) * length)
 
 def divisible_by(num, den):
     return (num % den) == 0
 
+@beartype
 def default_attention(
     q: Tensor,
     k: Tensor,
     v: Tensor,
     mask: Optional[Tensor] = None,
     causal: bool = False
 ):
@@ -76,14 +77,15 @@
     out = einsum('b h i j, b j h d -> b i h d', attn, v)
 
     return out
 
 # rotary embeddings with modifications to support striped attention
 
 class RingRotaryEmbedding(Module):
+    @beartype
     def __init__(
         self,
         dim,
         ring: bool = False,
         striped: bool = False,
         buckets: int = 1,        # in striped attention with flash buckets > 1, one needs to specify the number of buckets per machine
         theta = 10000
@@ -101,14 +103,15 @@
         return self.inv_freq.device
 
     @property
     def is_cuda(self):
         return self.inv_freq.is_cuda
 
     @autocast(enabled = False)
+    @beartype
     def forward(
         self,
         seq_len: int
     ):
         device = self.device
 
         pos = None
@@ -172,26 +175,26 @@
     return pad_at_dim(x, (0, pad_length), value = pad_value, dim = 1), pad_length
 
 def maybe_pad_seq_and_mask(
     x: Tensor,
     mask: Optional[Tensor],
     seq_size: int
 ):
-    orig_x, shape = x, x.shape[:2]
+    orig_x, device, shape = x, x.device, x.shape[:2]
     seq_len = shape[-1]
 
     # auto pad sequence and mask, as ring passing makes assumption tensor is all same shape
 
     x, pad_length = pad_to_multiple(x, seq_size)
 
     if pad_length == 0:
         return x, mask
 
     if not exists(mask):
-        mask = torch.ones(shape).bool()
+        mask = torch.ones(shape, device = device).bool()
 
     mask, _ = pad_to_multiple(mask, seq_size, pad_value = False)
 
     return x, mask
 
 def sharded_batch_to_sharded_seq(
     x: Tensor,
@@ -257,14 +260,15 @@
     @beartype
     def __init__(
         self,
         dim: int,
         *,
         dim_head: int = 64,
         heads: int = 8,
+        num_grouped_query_heads: int = 1,
         causal: bool = False,
         eps: float = 1e-10,
         bucket_size: int = 512,
         ring_attn: bool = False,
         ring_seq_size: int = 512,
         max_lookback_seq_len: Optional[int] = None,
         striped_ring_attn: bool = False,
@@ -280,14 +284,22 @@
 
         use_cuda_kernel = default(use_cuda_kernel, torch.cuda.is_available())
         assert not (use_cuda_kernel and not torch.cuda.is_available())
         self.use_cuda_kernel = use_cuda_kernel
 
         self.eps = eps
         self.heads = heads
+        self.dim_head = dim_head
+
+        assert divisible_by(heads, num_grouped_query_heads), f'number of query heads ({heads}) must be divisible by the groups ({num_grouped_query_heads})'
+
+        kv_heads = heads // num_grouped_query_heads
+        self.num_grouped_query_heads = num_grouped_query_heads
+        self.qkv_head_breakdown = (heads, kv_heads, kv_heads)
+
         self.scale = dim_head ** -0.5
         self.causal = causal
 
         assert (not ring_attn) or divisible_by(ring_seq_size, bucket_size), f'ring seq size {ring_seq_size} is not divisible by bucket size {bucket_size}'
 
         self.ring_attn = ring_attn
         self.max_lookback_seq_len = max_lookback_seq_len
@@ -314,18 +326,21 @@
                 theta = rotary_embed_theta,
                 buckets = ring_seq_size // bucket_size
             )
 
         # projections
 
         dim_inner = dim_head * heads
+        dim_kv_inner = dim_head * kv_heads
+
+        self.to_qkv_split = (dim_inner, dim_kv_inner, dim_kv_inner)
 
         self.to_qkv = nn.Sequential(
             RMSNorm(dim) if prenorm else nn.Identity(),
-            nn.Linear(dim, dim_inner * 3, bias = False)
+            nn.Linear(dim, dim_inner + (dim_kv_inner * 2), bias = False)
         )
 
         self.to_out = nn.Linear(dim_inner, dim, bias = False)
 
     def forward(
         self,
         x,
@@ -362,15 +377,16 @@
                     mask = rearrange(mask, 'b (i j) -> b (j i)', i = striped_bucket_size)
 
             (x, mask), batch_sizes, num_sharded_batches = sharded_batch_to_sharded_seq(x, mask, self.ring_seq_size)
 
         device = x.device
 
         qkv = self.to_qkv(x)
-        q, k, v = rearrange(qkv, 'b n (qkv h d) -> qkv b n h d', qkv = 3, h = self.heads)
+
+        q, k, v = rearrange(qkv, 'b n (h d) -> b n h d', d = self.dim_head).split(self.qkv_head_breakdown, dim = -2)
 
         # rotary relative positions
 
         if not exists(rotary_emb) and exists(self.rotary_embed):
             rotary_emb = self.rotary_embed(q.shape[-2])
 
         if exists(rotary_emb):
@@ -453,14 +469,15 @@
         num_tokens: int,
         dim: int,
         depth: int,
         causal: bool = False,
         dim_head: int = 64,
         heads: int = 8,
         ff_mult: int = 4,
+        num_grouped_query_heads: int = 1,   # grouped query attention - kv heads = (heads // num_grouped_query_heads)
         bucket_size: int = 512,
         ring_attn: bool = False,
         striped_ring_attn: bool = False,
         ring_seq_size: int = 512,
         auto_shard_seq: Optional[bool] = None,
         max_lookback_seq_len: Optional[Union[Tuple[int, ...], int]] = None,
         rotary_embed_theta: int = 10000,    # will need to be changed for the million token context
@@ -509,14 +526,15 @@
 
             self.layers.append(ModuleList([
                 RingAttention(
                     dim = dim,
                     causal = causal,
                     dim_head = dim_head,
                     heads = heads,
+                    num_grouped_query_heads = num_grouped_query_heads,
                     bucket_size = bucket_size,
                     ring_attn = ring_attn,
                     ring_seq_size = ring_seq_size,
                     max_lookback_seq_len = layer_max_lookback_seq_len,
                     striped_ring_attn = striped_ring_attn,
                     force_regular_attn = force_regular_attn,
                     use_cuda_kernel = self.use_cuda_kernel,
```

### Comparing `ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring_flash_attention.py` & `ring_attention_pytorch-0.4.0/ring_attention_pytorch/ring_flash_attention.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import partial
 from typing import Optional
 
 import torch
 from torch import nn, einsum, Tensor
 from torch.autograd.function import Function
 
-from einops import rearrange
+from einops import rearrange, repeat, reduce
 
 from ring_attention_pytorch.ring import (
     ring_pass,
     all_ring_pass,
     null_ring_pass,
     one_ring_pass,
     get_rank,
@@ -69,15 +69,19 @@
     ):
         ring_size = default(ring_size, get_world_size())
 
         cross_attn = q.shape[-2] != k.shape[-2]
         ring_reduce_col &= not cross_attn
         striped_ring_attn &= not cross_attn
 
-        assert k.shape[-1] == v.shape[-1]
+        assert k.shape[-2:] == v.shape[-2:]
+        q_heads, kv_heads = q.shape[-2], k.shape[-2]
+
+        assert divisible_by(q_heads, kv_heads)
+        q_head_groups = q_heads // kv_heads
 
         per_machine_seq_size = k.shape[1]
 
         # calculate max ring passes
 
         max_ring_passes = None
         num_lookback_buckets = float('inf')
@@ -120,14 +124,16 @@
         receive_kv = None
         receive_mask = None
 
         for (ring_rank, _), ((kv, mask), (receive_kv, receive_mask)) in ring_pass_fn(kv, mask, receive_buffers = (receive_kv, receive_mask), max_iters = max_ring_passes, ring_size = ring_size):
 
             k, v = kv
 
+            k, v = map(lambda t: repeat(t, '... h d -> ... (g h) d', g = q_head_groups), (k, v))
+
             col_splits = zip(
                 k.split(bucket_size, dim = -3),
                 v.split(bucket_size, dim = -3),
                 maybe_split(mask, bucket_size, dim = -1)
             )
 
             for k_ind, (kc, vc, col_mask) in enumerate(col_splits):
@@ -202,15 +208,16 @@
             scale,
             orig_mask,
             bucket_size,
             ring_reduce_col,
             max_ring_passes,
             num_lookback_buckets,
             striped_ring_attn,
-            ring_size
+            ring_size,
+            q_head_groups
         )
 
         ctx.save_for_backward(q, orig_k, orig_v, o, lse)
 
         return o
 
     @staticmethod
@@ -223,15 +230,16 @@
             scale,
             mask,
             bucket_size,
             ring_reduce_col,
             max_ring_passes,
             num_lookback_buckets,
             striped_ring_attn,
-            ring_size
+            ring_size,
+            q_head_groups
         ) = ctx.args
 
         q, k, v, o, lse = ctx.saved_tensors
 
         row_ring_rank = (get_rank() % ring_size) if ring_reduce_col else 0
 
         per_machine_seq_size = k.shape[1]
@@ -264,14 +272,18 @@
         # ring reduce key / values
 
         for (ring_rank, _), ((kv_and_dkv, mask), (receive_kv_and_dkv, receive_mask)) in ring_pass_fn(kv_and_dkv, mask, receive_buffers = (receive_kv_and_dkv, receive_mask), max_iters = max_ring_passes, ring_size = ring_size):
             k_ring_rank = ring_rank % ring_size
 
             k, v, dk, dv = kv_and_dkv
 
+            # account for grouped query attention
+
+            k, v = map(lambda t: repeat(t, '... h d -> ... (g h) d', g = q_head_groups), (k, v))
+
             col_splits = zip(
                 k.split(bucket_size, dim = 1),
                 v.split(bucket_size, dim = 1),
                 dk.split(bucket_size, dim = 1),
                 dv.split(bucket_size, dim = 1),
                 maybe_split(mask, bucket_size, dim = -1)
             )
@@ -319,14 +331,19 @@
                     dp = einsum('b i h d, b j h d -> b h i j', doc, vc)
 
                     ds = p * scale * (dp - Dc)
 
                     dq_chunk = einsum('b h i j, b j h d -> b i h d', ds, kc)
                     dk_chunk = einsum('b h i j, b i h d -> b j h d', ds, qc)
 
+                    # account for grouped query attention
+
+                    dk_chunk = reduce(dk_chunk, '... (g h) d -> ... h d', g = q_head_groups, reduction = 'sum')
+                    dv_chunk = reduce(dv_chunk, '... (g h) d -> ... h d', g = q_head_groups, reduction = 'sum')
+
                     dqc.add_(dq_chunk)
                     dkc.add_(dk_chunk)
                     dvc.add_(dv_chunk)
 
             if not ring_reduce_col:
                 continue
```

### Comparing `ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/PKG-INFO` & `ring_attention_pytorch-0.4.0/ring_attention_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.9
+Version: 0.4.0
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.9/setup.py` & `ring_attention_pytorch-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'ring-attention-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.9',
+  version = '0.4.0',
   license='MIT',
   description = 'Ring Attention - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/ring-attention-pytorch',
   keywords = [
```

