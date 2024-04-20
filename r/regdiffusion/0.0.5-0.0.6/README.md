# Comparing `tmp/regdiffusion-0.0.5.tar.gz` & `tmp/regdiffusion-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regdiffusion-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "regdiffusion-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `regdiffusion-0.0.5.tar` & `regdiffusion-0.0.6.tar`

### file list

```diff
@@ -1,47 +1,30 @@
--rw-r--r--   0        0        0     8196 2024-03-29 03:21:54.348168 regdiffusion-0.0.5/.DS_Store
--rw-r--r--   0        0        0     1081 2024-03-27 21:49:00.320451 regdiffusion-0.0.5/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      160 2024-03-28 20:56:06.258360 regdiffusion-0.0.5/.gitignore
--rw-r--r--   0        0        0    11341 2024-03-17 14:05:11.179073 regdiffusion-0.0.5/LICENSE
--rw-r--r--   0        0        0      831 2024-03-27 02:27:52.639756 regdiffusion-0.0.5/README.md
--rw-r--r--   0        0        0       32 2024-03-27 03:45:27.579114 regdiffusion-0.0.5/docs/.gitignore
--rw-r--r--   0        0        0      634 2024-03-22 02:27:01.393418 regdiffusion-0.0.5/docs/Makefile
--rw-r--r--   0        0        0    41866 2024-03-29 03:20:00.202421 regdiffusion-0.0.5/docs/_static/regdiffusion.png
--rw-r--r--   0        0        0   104704 2024-03-29 03:20:00.225785 regdiffusion-0.0.5/docs/_static/regdiffusion@2x.png
--rw-r--r--   0        0        0      227 2024-03-27 03:05:34.619510 regdiffusion-0.0.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      203 2024-03-27 03:06:25.177685 regdiffusion-0.0.5/docs/_templates/autosummary/classnoinheritance.rst
--rw-r--r--   0        0        0     1469 2024-03-29 03:21:43.715202 regdiffusion-0.0.5/docs/conf.py
--rw-r--r--   0        0        0      401 2024-03-28 21:26:12.637302 regdiffusion-0.0.5/docs/data_module.rst
--rw-r--r--   0        0        0     3707 2024-03-28 21:24:19.645072 regdiffusion-0.0.5/docs/index.rst
--rw-r--r--   0        0        0      160 2024-03-29 03:23:36.146801 regdiffusion-0.0.5/docs/main_api.rst
--rw-r--r--   0        0        0      800 2024-03-22 02:27:01.393639 regdiffusion-0.0.5/docs/make.bat
--rw-r--r--   0        0        0       94 2024-03-28 21:23:41.136317 regdiffusion-0.0.5/docs/models.rst
--rw-r--r--   0        0        0    10157 2024-03-27 02:59:31.919041 regdiffusion-0.0.5/docs/quick_tour.md
--rw-r--r--   0        0        0     1222 2024-03-27 11:40:19.763362 regdiffusion-0.0.5/docs/supplements.rst
--rw-r--r--   0        0        0    34931 2024-03-27 05:00:56.441859 regdiffusion-0.0.5/docs/supplements/rd_hammond_Cx3cr1.html
--rw-r--r--   0        0        0    27882 2024-03-27 05:00:56.441959 regdiffusion-0.0.5/docs/supplements/rd_hammond_Fcrls.html
--rw-r--r--   0        0        0    22085 2024-03-27 05:00:56.442103 regdiffusion-0.0.5/docs/supplements/rd_hammond_Hexb.html
--rw-r--r--   0        0        0    41477 2024-03-27 05:00:56.442208 regdiffusion-0.0.5/docs/supplements/rd_hammond_Mertk.html
--rw-r--r--   0        0        0    29160 2024-03-27 05:00:56.442356 regdiffusion-0.0.5/docs/supplements/rd_hammond_P2ry12.html
--rw-r--r--   0        0        0    30894 2024-03-27 05:00:56.442493 regdiffusion-0.0.5/docs/supplements/rd_hammond_Pros1.html
--rw-r--r--   0        0        0    50781 2024-03-27 05:00:56.442678 regdiffusion-0.0.5/docs/supplements/rd_hammond_Sall1.html
--rw-r--r--   0        0        0    27402 2024-03-27 05:00:56.442908 regdiffusion-0.0.5/docs/supplements/rd_hammond_Siglech.html
--rw-r--r--   0        0        0    21649 2024-03-27 05:00:56.443024 regdiffusion-0.0.5/docs/supplements/rd_hammond_Tmem119.html
--rw-r--r--   0        0        0    20696 2024-03-27 05:00:56.443153 regdiffusion-0.0.5/docs/supplements/rd_hammond_Trem2.html
--rw-r--r--   0        0        0    13682 2024-03-22 02:27:01.393826 regdiffusion-0.0.5/example.ipynb
--rw-r--r--   0        0        0      786 2024-03-22 02:27:01.395713 regdiffusion-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      396 2024-03-22 03:24:56.295692 regdiffusion-0.0.5/regdiffusion/__init__.py
--rw-r--r--   0        0        0      366 2024-03-28 21:12:32.210141 regdiffusion-0.0.5/regdiffusion/data/__init__.py
--rw-r--r--   0        0        0     3697 2024-03-28 21:01:09.698055 regdiffusion-0.0.5/regdiffusion/data/beeline.py
--rw-r--r--   0        0        0     4278 2024-03-28 02:52:23.196646 regdiffusion-0.0.5/regdiffusion/data/microglia.py
--rw-r--r--   0        0        0      567 2024-03-22 03:03:28.782637 regdiffusion-0.0.5/regdiffusion/data/utils.py
--rw-r--r--   0        0        0     3350 2024-03-22 02:27:01.395858 regdiffusion-0.0.5/regdiffusion/evaluator.py
--rw-r--r--   0        0        0    16924 2024-03-28 02:51:31.529942 regdiffusion-0.0.5/regdiffusion/grn.py
--rw-r--r--   0        0        0     5906 2024-03-22 03:40:01.507266 regdiffusion-0.0.5/regdiffusion/logger.py
--rw-r--r--   0        0        0       39 2024-03-17 14:05:11.190775 regdiffusion-0.0.5/regdiffusion/models/__init__.py
--rw-r--r--   0        0        0     6331 2024-03-28 02:59:41.717194 regdiffusion-0.0.5/regdiffusion/models/regdiffusion.py
--rw-r--r--   0        0        0    17058 2024-03-27 21:11:04.107791 regdiffusion-0.0.5/regdiffusion/trainer.py
--rw-r--r--   0        0        0   953971 2024-03-26 19:43:13.353093 regdiffusion-0.0.5/resources/apoe_reg.png
--rw-r--r--   0        0        0   374861 2024-03-17 14:05:11.193301 regdiffusion-0.0.5/resources/mecs.png
--rw-r--r--   0        0        0   323230 2024-03-17 14:05:11.195618 regdiffusion-0.0.5/resources/mecs_cluster.png
--rw-r--r--   0        0        0   288128 2024-03-17 14:05:11.197567 regdiffusion-0.0.5/resources/shinygo.png
--rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 regdiffusion-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-11-05 15:52:36.085365 regdiffusion-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3809 2024-03-29 20:40:52.313815 regdiffusion-0.0.6/README.md
+-rw-r--r--   0        0        0      786 2024-04-20 04:02:47.110287 regdiffusion-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      423 2024-04-16 15:21:41.073897 regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     3350 2024-03-21 21:26:05.086388 regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/evaluator-checkpoint.py
+-rw-r--r--   0        0        0    18237 2024-04-05 04:43:37.672632 regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/grn-checkpoint.py
+-rw-r--r--   0        0        0     5120 2024-01-25 21:19:10.168299 regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/logger-checkpoint.py
+-rw-r--r--   0        0        0    11432 2024-03-14 17:20:42.308017 regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/trainer-checkpoint.py
+-rw-r--r--   0        0        0      423 2024-04-16 15:21:41.073897 regdiffusion-0.0.6/regdiffusion/__init__.py
+-rw-r--r--   0        0        0      149 2024-03-02 14:07:24.969670 regdiffusion-0.0.6/regdiffusion/data/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     4272 2024-02-01 03:02:39.297276 regdiffusion-0.0.6/regdiffusion/data/.ipynb_checkpoints/beeline-checkpoint.py
+-rw-r--r--   0        0        0     2654 2024-03-07 17:17:15.538130 regdiffusion-0.0.6/regdiffusion/data/.ipynb_checkpoints/microglia-checkpoint.py
+-rw-r--r--   0        0        0      567 2024-01-25 21:19:10.293030 regdiffusion-0.0.6/regdiffusion/data/.ipynb_checkpoints/utils-checkpoint.py
+-rw-r--r--   0        0        0      366 2024-03-29 20:40:52.511868 regdiffusion-0.0.6/regdiffusion/data/__init__.py
+-rw-r--r--   0        0        0     3697 2024-03-29 20:40:52.521726 regdiffusion-0.0.6/regdiffusion/data/beeline.py
+-rw-r--r--   0        0        0     4278 2024-03-29 20:40:52.535236 regdiffusion-0.0.6/regdiffusion/data/microglia.py
+-rw-r--r--   0        0        0      567 2024-01-25 21:19:10.333274 regdiffusion-0.0.6/regdiffusion/data/utils.py
+-rw-r--r--   0        0        0     3350 2024-03-21 21:26:05.086388 regdiffusion-0.0.6/regdiffusion/evaluator.py
+-rw-r--r--   0        0        0    18097 2024-04-16 15:03:49.420584 regdiffusion-0.0.6/regdiffusion/grn.py
+-rw-r--r--   0        0        0     5906 2024-03-27 03:46:34.074272 regdiffusion-0.0.6/regdiffusion/logger.py
+-rw-r--r--   0        0        0       39 2024-03-07 16:35:41.777169 regdiffusion-0.0.6/regdiffusion/models/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     6363 2024-03-22 04:52:28.581539 regdiffusion-0.0.6/regdiffusion/models/.ipynb_checkpoints/regdiffusion-checkpoint.py
+-rw-r--r--   0        0        0       39 2024-03-07 16:35:41.777169 regdiffusion-0.0.6/regdiffusion/models/__init__.py
+-rw-r--r--   0        0        0     6331 2024-03-29 20:40:52.560257 regdiffusion-0.0.6/regdiffusion/models/regdiffusion.py
+-rw-r--r--   0        0        0       30 2024-04-16 15:03:49.428592 regdiffusion-0.0.6/regdiffusion/plot/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     2218 2024-04-16 15:24:20.971807 regdiffusion-0.0.6/regdiffusion/plot/.ipynb_checkpoints/pyvis-checkpoint.py
+-rw-r--r--   0        0        0       30 2024-04-16 15:03:49.428592 regdiffusion-0.0.6/regdiffusion/plot/__init__.py
+-rw-r--r--   0        0        0     2218 2024-04-16 15:24:20.971807 regdiffusion-0.0.6/regdiffusion/plot/pyvis.py
+-rw-r--r--   0        0        0    17126 2024-04-16 15:03:49.445516 regdiffusion-0.0.6/regdiffusion/trainer.py
+-rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 regdiffusion-0.0.6/PKG-INFO
```

### Comparing `regdiffusion-0.0.5/LICENSE` & `regdiffusion-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.5/docs/index.rst` & `regdiffusion-0.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,232 +1,239 @@
-00000000: 5265 6744 6966 6675 7369 6f6e 0a3d 3d3d  RegDiffusion.===
-00000010: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 5265 6744  ==========..RegD
-00000020: 6966 6675 7369 6f6e 2069 7320 6120 7665  iffusion is a ve
-00000030: 7279 2066 6173 7420 7265 6775 6c61 746f  ry fast regulato
-00000040: 7279 206e 6574 776f 726b 2069 6e66 6572  ry network infer
-00000050: 656e 6365 2061 6c67 6f72 6974 686d 2062  ence algorithm b
-00000060: 6173 6564 206f 6e20 0a70 726f 6261 6269  ased on .probabi
-00000070: 6c69 7374 6963 2064 6966 6675 7369 6f6e  listic diffusion
-00000080: 206d 6f64 656c 2e20 4974 2077 6f72 6b73   model. It works
-00000090: 2077 656c 6c20 6f6e 2067 656e 6573 2061   well on genes a
-000000a0: 6e64 2069 7320 6361 7061 626c 6520 746f  nd is capable to
-000000b0: 2072 6170 6964 6c79 0a70 7265 6469 6374   rapidly.predict
-000000c0: 2062 696f 6c6f 6769 6361 6c6c 7920 7665   biologically ve
-000000d0: 7269 6669 6162 6c65 206c 696e 6b73 2066  rifiable links f
-000000e0: 726f 6d20 6c61 7267 6520 7369 6e67 6c65  rom large single
-000000f0: 2063 656c 6c20 524e 412d 7365 7120 6461   cell RNA-seq da
-00000100: 7461 2077 6974 6820 0a31 302c 3030 302b  ta with .10,000+
-00000110: 2067 656e 6573 2e0a 0a49 6e73 7461 6c6c   genes...Install
-00000120: 6174 696f 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d  ation.----------
-00000130: 2d2d 0a0a 6060 7265 6764 6966 6675 7369  --..``regdiffusi
-00000140: 6f6e 6060 2069 7320 6176 6169 6c61 626c  on`` is availabl
-00000150: 6520 6f6e 2070 7970 693a 0a0a 2020 2020  e on pypi:..    
-00000160: 7069 7020 696e 7374 616c 6c20 7265 6764  pip install regd
-00000170: 6966 6675 7369 6f6e 0a0a 5175 6963 6b20  iffusion..Quick 
-00000180: 546f 7572 0a2d 2d2d 2d2d 2d2d 2d2d 2d0a  Tour.----------.
-00000190: 5468 6973 2070 6163 6b61 6765 2060 6072  This package ``r
-000001a0: 6567 6469 6666 7573 696f 6e60 6020 7072  egdiffusion`` pr
-000001b0: 6f76 6964 6573 2074 6865 206f 6666 6963  ovides the offic
-000001c0: 6961 6c20 696d 706c 656d 656e 7461 7469  ial implementati
-000001d0: 6f6e 206f 6620 7468 650a 5265 6744 6966  on of the.RegDif
-000001e0: 6675 7369 6f6e 2061 6c67 6f72 6974 686d  fusion algorithm
-000001f0: 2061 6e64 2061 2073 6574 206f 6620 6561   and a set of ea
-00000200: 7379 2d74 6f2d 7573 6520 636f 6d70 616e  sy-to-use compan
-00000210: 696f 6e20 746f 6f6c 7320 746f 2065 7661  ion tools to eva
-00000220: 6c75 6174 652c 0a61 6e61 6c79 7a65 2c20  luate,.analyze, 
-00000230: 616e 6420 7669 7375 616c 697a 6520 7468  and visualize th
-00000240: 6520 696e 6665 7272 6564 206e 6574 776f  e inferred netwo
-00000250: 726b 2e20 5765 2061 6c73 6f20 7072 6f76  rk. We also prov
-00000260: 6964 6520 6163 6365 7373 2074 6f6f 6c73  ide access tools
-00000270: 2074 6f20 0a47 524e 2062 656e 6368 6d61   to .GRN benchma
-00000280: 726b 7320 616e 6420 7072 6570 726f 6365  rks and preproce
-00000290: 7373 6564 2073 696e 676c 6520 6365 6c6c  ssed single cell
-000002a0: 2064 6174 6173 6574 7320 666f 7220 6576   datasets for ev
-000002b0: 616c 7561 7469 6f6e 2e20 0a0a 5765 2074  aluation. ..We t
-000002c0: 7269 6564 2074 6f20 6b65 6570 2074 6865  ried to keep the
-000002d0: 2074 6f70 206c 6576 656c 2069 6e74 6572   top level inter
-000002e0: 6661 6365 2073 7472 6169 6768 7466 6f72  face straightfor
-000002f0: 7761 7264 2e20 5269 6768 7420 6e6f 772c  ward. Right now,
-00000300: 2069 7420 6f6e 6c79 200a 636f 6e73 6973   it only .consis
-00000310: 7473 206f 6620 3420 636f 6d70 6f6e 656e  ts of 4 componen
-00000320: 7473 3a20 7468 6520 6060 5265 6744 6966  ts: the ``RegDif
-00000330: 6675 7369 6f6e 5472 6169 6e65 7260 6020  fusionTrainer`` 
-00000340: 636c 6173 732c 2074 6865 2060 6047 524e  class, the ``GRN
-00000350: 6060 2063 6c61 7373 2c20 7468 6520 0a60  `` class, the .`
-00000360: 6047 524e 4576 616c 7561 746f 7260 6020  `GRNEvaluator`` 
-00000370: 636c 6173 732c 2061 6e64 2074 6865 2060  class, and the `
-00000380: 6064 6174 6160 6020 6d6f 6475 6c65 2e20  `data`` module. 
-00000390: 0a0a 2d20 6060 5265 6744 6966 6675 7369  ..- ``RegDiffusi
-000003a0: 6f6e 5472 6169 6e65 7260 603a 2059 6f75  onTrainer``: You
-000003b0: 2063 616e 2075 7365 2069 7420 746f 2074   can use it to t
-000003c0: 7261 696e 2061 2060 6052 6567 4469 6666  rain a ``RegDiff
-000003d0: 7573 696f 6e60 6020 6d6f 6465 6c20 6279  usion`` model by
-000003e0: 200a 2020 7072 6f76 6964 696e 6720 6c6f   .  providing lo
-000003f0: 6720 7472 616e 7366 6f72 6d65 6420 6578  g transformed ex
-00000400: 7072 6573 7369 6f6e 2064 6174 6120 696e  pression data in
-00000410: 2061 2060 606e 756d 7079 6060 2061 7272   a ``numpy`` arr
-00000420: 6179 2e20 5468 6520 7472 6169 6e69 6e67  ay. The training
-00000430: 0a20 2070 726f 6365 7373 2063 6f75 6c64  .  process could
-00000440: 2062 6520 6569 7468 6572 2073 7461 7274   be either start
-00000450: 6564 206f 7220 636f 6e74 696e 7565 6420  ed or continued 
-00000460: 7573 696e 6720 7468 6520 6060 2e74 7261  using the ``.tra
-00000470: 696e 2829 6060 206d 6574 686f 642e 2059  in()`` method. Y
-00000480: 6f75 200a 2020 6361 6e20 6578 706f 7274  ou .  can export
-00000490: 2074 6865 2069 6e66 6572 7265 6420 6060   the inferred ``
-000004a0: 4752 4e60 6020 7573 696e 6720 7468 6520  GRN`` using the 
-000004b0: 6060 2e67 6574 5f67 726e 2829 6060 206d  ``.get_grn()`` m
-000004c0: 6574 686f 642e 0a2d 2060 6047 524e 6060  ethod..- ``GRN``
-000004d0: 3a20 5468 6520 6060 4752 4e60 6020 636c  : The ``GRN`` cl
-000004e0: 6173 7320 7072 6f76 6964 6573 2061 2063  ass provides a c
-000004f0: 6f6e 7461 696e 6572 2074 6f20 7361 7665  ontainer to save
-00000500: 2074 6865 2069 6e66 6572 7265 6420 6164   the inferred ad
-00000510: 6a61 6365 6e63 790a 2020 6d61 7472 6978  jacency.  matrix
-00000520: 2061 6e64 2074 6865 2063 6f72 7265 7370   and the corresp
-00000530: 6f6e 6469 6e67 2067 656e 6520 6e61 6d65  onding gene name
-00000540: 732e 2059 6f75 2063 616e 2073 6176 6520  s. You can save 
-00000550: 7468 6520 6060 4752 4e60 6020 6f62 6a65  the ``GRN`` obje
-00000560: 6374 2074 6f20 0a20 2061 206c 6f63 616c  ct to .  a local
-00000570: 2060 6048 4446 3560 6020 6669 6c65 2075   ``HDF5`` file u
-00000580: 7369 6e67 2074 6865 2060 602e 746f 5f68  sing the ``.to_h
-00000590: 6466 3528 2960 6020 6d65 7468 6f64 2061  df5()`` method a
-000005a0: 6e64 2072 656c 6f61 6420 7468 6520 7361  nd reload the sa
-000005b0: 7665 6420 6669 6c65 200a 2020 7573 696e  ved file .  usin
-000005c0: 6720 7468 6520 6060 7265 6164 5f68 6466  g the ``read_hdf
-000005d0: 3528 2960 6020 6675 6e63 7469 6f6e 2e20  5()`` function. 
-000005e0: 4974 2061 6c73 6f20 636f 6d65 7320 7769  It also comes wi
-000005f0: 7468 2066 756e 6374 696f 6e61 6c69 7469  th functionaliti
-00000600: 6573 2074 6f20 0a20 2065 7870 6f72 7420  es to .  export 
-00000610: 6f72 2076 6973 7561 6c69 7a65 206c 6f63  or visualize loc
-00000620: 616c 2072 6567 696f 6e73 2e20 466f 7220  al regions. For 
-00000630: 6578 616d 706c 652c 2079 6f75 2063 616e  example, you can
-00000640: 2075 7365 2074 6865 200a 2020 6060 2e76   use the .  ``.v
-00000650: 6973 7561 6c69 7a65 5f6c 6f63 616c 5f6e  isualize_local_n
-00000660: 6569 6768 626f 7268 6f6f 6428 2960 6020  eighborhood()`` 
-00000670: 746f 2067 656e 6572 6174 6520 6120 7369  to generate a si
-00000680: 6d69 6c61 7220 706c 6f74 2061 7320 7573  milar plot as us
-00000690: 6564 2069 6e20 0a20 2074 6865 2052 6567  ed in .  the Reg
-000006a0: 4469 6666 7573 696f 6e20 7061 7065 722e  Diffusion paper.
-000006b0: 2059 6f75 2063 616e 2061 6c73 6f20 6578   You can also ex
-000006c0: 7472 6163 7420 7468 6520 756e 6465 726c  tract the underl
-000006d0: 7969 6e67 2061 646a 6163 656e 6379 206c  ying adjacency l
-000006e0: 6973 7420 0a20 2075 7369 6e67 2074 6865  ist .  using the
-000006f0: 2060 602e 6578 7472 6163 745f 6e6f 6465   ``.extract_node
-00000700: 5f32 686f 705f 6e65 6967 6862 6f72 686f  _2hop_neighborho
-00000710: 6f64 2829 6060 206d 6574 686f 642e 0a2d  od()`` method..-
-00000720: 2060 6047 524e 4576 616c 7561 746f 7260   ``GRNEvaluator`
-00000730: 603a 2054 6865 2067 726f 756e 6420 7472  `: The ground tr
-00000740: 7574 6820 6f66 2072 6567 756c 6174 6f72  uth of regulator
-00000750: 7920 7265 6c61 7469 6f6e 7368 6970 206f  y relationship o
-00000760: 6674 656e 2065 7869 7374 2061 7320 0a20  ften exist as . 
-00000770: 206c 6973 7420 6f66 2065 6467 6573 2062   list of edges b
-00000780: 7574 2074 6865 2076 616c 7565 7320 746f  ut the values to
-00000790: 2062 6520 6576 616c 7561 7465 6420 6172   be evaluated ar
-000007a0: 6520 6f66 7465 6e20 696e 2061 646a 6163  e often in adjac
-000007b0: 656e 6379 206d 6174 7269 782e 200a 2020  ency matrix. .  
-000007c0: 5468 6520 6060 4752 4e45 7661 6c75 6174  The ``GRNEvaluat
-000007d0: 6f72 6060 2063 6c61 7373 2069 7320 6465  or`` class is de
-000007e0: 7369 676e 6564 2074 6f20 6669 6c6c 2074  signed to fill t
-000007f0: 6865 2067 6170 2e20 5269 6768 7420 6e6f  he gap. Right no
-00000800: 7720 6974 2073 7570 706f 7274 730a 2020  w it supports.  
-00000810: 636f 6d6d 6f6e 206d 6574 7269 6373 2073  common metrics s
-00000820: 7563 6820 6173 2041 5552 4f43 2c20 4155  uch as AUROC, AU
-00000830: 5052 2c20 4155 5052 2052 6174 696f 2c20  PR, AUPR Ratio, 
-00000840: 4550 2c20 616e 6420 4550 522e 200a 2d20  EP, and EPR. .- 
-00000850: 6060 6461 7461 6060 206d 6f64 756c 653a  ``data`` module:
-00000860: 2052 6967 6874 206e 6f77 2c20 7468 6520   Right now, the 
-00000870: 6060 6461 7461 6060 206d 6f64 756c 6520  ``data`` module 
-00000880: 696e 636c 7564 6573 2071 7569 636b 2061  includes quick a
-00000890: 6363 6573 7320 746f 2042 4545 4c49 4e45  ccess to BEELINE
-000008a0: 200a 2020 6265 6e63 686d 6172 6b73 2061   .  benchmarks a
-000008b0: 6e64 206f 7572 2070 7265 7072 6f63 6573  nd our preproces
-000008c0: 7365 6420 7369 6e67 6c65 2063 656c 6c20  sed single cell 
-000008d0: 6461 7461 7365 7473 206f 6e20 6d6f 7573  datasets on mous
-000008e0: 6520 6d69 6372 6f67 6c69 612e 200a 0a55  e microglia. ..U
-000008f0: 6e64 6572 7374 616e 6469 6e67 2074 6865  nderstanding the
-00000900: 2049 6e66 6572 7265 6420 4e65 7477 6f72   Inferred Networ
-00000910: 6b73 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ks.-------------
-00000920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000930: 2d2d 2d2d 2d2d 0a41 6674 6572 2074 6865  ------.After the
-00000940: 2060 6052 6567 4469 6666 7573 696f 6e60   ``RegDiffusion`
-00000950: 6020 6d6f 6465 6c20 636f 6e76 6572 6765  ` model converge
-00000960: 732c 2077 6861 7420 796f 7520 6765 7420  s, what you get 
-00000970: 6973 2073 696d 706c 7920 616e 200a 6061  is simply an .`a
-00000980: 646a 6163 656e 6379 6020 6d61 7472 6978  djacency` matrix
-00000990: 2e20 5768 656e 2079 6f75 2068 6176 6520  . When you have 
-000009a0: 7468 6f75 7361 6e64 7320 6f72 2074 656e  thousands or ten
-000009b0: 7320 6f66 2074 686f 7573 616e 6473 206f  s of thousands o
-000009c0: 6620 6765 6e65 732c 200a 6974 2773 2067  f genes, .it's g
-000009d0: 6574 7469 6e67 2064 6966 6669 6375 6c74  etting difficult
-000009e0: 2074 6f20 616e 616c 797a 6520 6d61 7472   to analyze matr
-000009f0: 6978 2061 7420 7468 6174 2073 6361 6c65  ix at that scale
-00000a00: 2e20 496e 206f 7572 2070 6170 6572 2c20  . In our paper, 
-00000a10: 7765 200a 7072 6f70 6f73 6520 6120 7761  we .propose a wa
-00000a20: 7920 746f 2061 6e61 6c79 7a65 2074 6865  y to analyze the
-00000a30: 206c 6f63 616c 206e 6574 776f 726b 2062   local network b
-00000a40: 7920 666f 6375 7369 6e67 206f 6e20 7468  y focusing on th
-00000a50: 6520 6765 6e65 7320 796f 7520 6361 7265  e genes you care
-00000a60: 200a 7468 6520 6d6f 7374 2e20 4368 6563   .the most. Chec
-00000a70: 6b20 6f75 7420 7468 6520 7475 746f 7269  k out the tutori
-00000a80: 616c 7320 6f6e 2074 6865 206c 6566 7420  als on the left 
-00000a90: 7369 6465 2066 6f72 2068 6f77 2074 6f20  side for how to 
-00000aa0: 7065 7266 6f72 6d20 6120 7369 6d69 6c61  perform a simila
-00000ab0: 7220 0a6e 6574 776f 726b 2061 6e61 6c79  r .network analy
-00000ac0: 7369 7320 6c69 6b65 2074 6865 206f 6e65  sis like the one
-00000ad0: 2077 6520 6469 6420 696e 2074 6865 2070   we did in the p
-00000ae0: 6170 6572 2e20 5765 2061 7265 2061 6c73  aper. We are als
-00000af0: 6f20 776f 726b 696e 6720 6f6e 2061 6e20  o working on an 
-00000b00: 0a69 6e74 6572 6163 7469 7665 2074 6f6f  .interactive too
-00000b10: 6c20 746f 2061 6e61 6c79 7a65 2073 6176  l to analyze sav
-00000b20: 6564 2047 524e 206f 626a 6563 742e 200a  ed GRN object. .
-00000b30: 0a2e 2e20 696d 6167 653a 3a20 6874 7470  ... image:: http
-00000b40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-00000b50: 7566 7473 4243 422f 5265 6744 6966 6675  uftsBCB/RegDiffu
-00000b60: 7369 6f6e 2f62 6c6f 622f 6d61 7374 6572  sion/blob/master
-00000b70: 2f72 6573 6f75 7263 6573 2f61 706f 655f  /resources/apoe_
-00000b80: 7265 672e 706e 673f 7261 773d 7472 7565  reg.png?raw=true
-00000b90: 0a20 2020 203a 7769 6474 683a 2037 3030  .    :width: 700
-00000ba0: 0a20 2020 203a 616c 743a 2049 6e66 6572  .    :alt: Infer
-00000bb0: 7265 6420 6e65 7477 6f72 6b20 6172 6f75  red network arou
-00000bc0: 6e64 2041 706f 450a 0a49 6e66 6572 656e  nd ApoE..Inferen
-00000bd0: 6365 2053 7065 6564 0a2d 2d2d 2d2d 2d2d  ce Speed.-------
-00000be0: 2d2d 2d2d 2d2d 2d2d 0a49 6e66 6572 656e  --------.Inferen
-00000bf0: 6365 206f 6e20 6e65 7477 6f72 6b73 2077  ce on networks w
-00000c00: 6974 6820 3135 2c30 3030 2067 656e 6573  ith 15,000 genes
-00000c10: 2074 616b 6573 2075 6e64 6572 2035 206d   takes under 5 m
-00000c20: 696e 7574 6573 206f 6e20 616e 2041 3130  inutes on an A10
-00000c30: 3020 4750 552e 200a 496e 2063 6f6e 7472  0 GPU. .In contr
-00000c40: 6173 742c 2070 7265 7669 6f75 7320 5641  ast, previous VA
-00000c50: 4520 6261 7365 6420 6d6f 6465 6c73 2077  E based models w
-00000c60: 6f75 6c64 2074 616b 6520 6d6f 7265 2074  ould take more t
-00000c70: 6861 6e20 3420 686f 7572 7320 6f6e 2074  han 4 hours on t
-00000c80: 6865 2073 616d 6520 0a64 6576 6963 652e  he same .device.
-00000c90: 2045 7665 6e20 6966 2079 6f75 2064 6f6e   Even if you don
-00000ca0: 2774 2068 6176 6520 6163 6365 7373 2074  't have access t
-00000cb0: 6f20 7468 6f73 6520 6661 6e63 7920 4750  o those fancy GP
-00000cc0: 5520 6361 7264 732c 2052 6567 4469 6666  U cards, RegDiff
-00000cd0: 7573 696f 6e20 0a73 7469 6c6c 2077 6f72  usion .still wor
-00000ce0: 6b73 2e20 496e 6665 7265 6e63 6520 6f6e  ks. Inference on
-00000cf0: 2074 6865 2073 616d 6520 6c61 7267 6520   the same large 
-00000d00: 6e65 7477 6f72 6b20 7461 6b65 7320 726f  network takes ro
-00000d10: 7567 686c 7920 3320 686f 7572 7320 6f6e  ughly 3 hours on
-00000d20: 2061 200a 6d69 642d 7261 6e67 6520 3132   a .mid-range 12
-00000d30: 2d63 6f72 6520 4350 552e 200a 0a0a 4369  -core CPU. ...Ci
-00000d40: 7461 7469 6f6e 0a2d 2d2d 2d2d 2d2d 2d0a  tation.--------.
-00000d50: 506c 6561 7365 2063 6f6e 7369 6465 7220  Please consider 
-00000d60: 6369 7465 206f 7572 2077 6f72 6b20 6966  cite our work if
-00000d70: 2079 6f75 2066 6f75 6e64 2069 7420 7573   you found it us
-00000d80: 6566 756c 2066 6f72 2079 6f75 7220 776f  eful for your wo
-00000d90: 726b 3a0a 0a0a 0a2e 2e20 746f 6374 7265  rk:...... toctre
-00000da0: 653a 3a0a 2020 203a 6361 7074 696f 6e3a  e::.   :caption:
-00000db0: 2047 6574 2053 7461 7274 6564 3a0a 2020   Get Started:.  
-00000dc0: 203a 6869 6464 656e 3a0a 0a20 2020 7175   :hidden:..   qu
-00000dd0: 6963 6b5f 746f 7572 0a0a 2e2e 2074 6f63  ick_tour.... toc
-00000de0: 7472 6565 3a3a 0a20 2020 3a63 6170 7469  tree::.   :capti
-00000df0: 6f6e 3a20 5265 6665 7265 6e63 6573 3a0a  on: References:.
-00000e00: 2020 203a 6869 6464 656e 3a0a 0a20 2020     :hidden:..   
-00000e10: 6d61 696e 5f61 7069 0a20 2020 6d6f 6465  main_api.   mode
-00000e20: 6c73 0a20 2020 6461 7461 5f6d 6f64 756c  ls.   data_modul
-00000e30: 650a 0a2e 2e20 746f 6374 7265 653a 3a0a  e.... toctree::.
-00000e40: 2020 203a 6361 7074 696f 6e3a 2050 6170     :caption: Pap
-00000e50: 6572 2053 7570 706c 656d 656e 7473 0a20  er Supplements. 
-00000e60: 2020 3a68 6964 6465 6e3a 0a0a 2020 2073    :hidden:..   s
-00000e70: 7570 706c 656d 656e 7473 0a              upplements.
+00000000: 2320 5265 6744 6966 6675 7369 6f6e 203c  # RegDiffusion <
+00000010: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000020: 7475 6674 7362 6362 2e67 6974 6875 622e  tuftsbcb.github.
+00000030: 696f 2f52 6567 4469 6666 7573 696f 6e2f  io/RegDiffusion/
+00000040: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000050: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000060: 6572 636f 6e74 656e 742e 636f 6d2f 5475  ercontent.com/Tu
+00000070: 6674 7342 4342 2f52 6567 4469 6666 7573  ftsBCB/RegDiffus
+00000080: 696f 6e2f 6d61 7374 6572 2f64 6f63 732f  ion/master/docs/
+00000090: 5f73 7461 7469 632f 7265 6764 6966 6675  _static/regdiffu
+000000a0: 7369 6f6e 2e70 6e67 2220 616c 6967 6e3d  sion.png" align=
+000000b0: 2272 6967 6874 2220 616c 743d 226c 6f67  "right" alt="log
+000000c0: 6f22 2077 6964 7468 3d22 3134 3022 2068  o" width="140" h
+000000d0: 6569 6768 7420 3d20 2231 3430 2220 7374  eight = "140" st
+000000e0: 796c 6520 3d20 2262 6f72 6465 723a 206e  yle = "border: n
+000000f0: 6f6e 653b 2066 6c6f 6174 3a20 7269 6768  one; float: righ
+00000100: 743b 223e 3c2f 613e 0a0a 5265 6744 6966  t;"></a>..RegDif
+00000110: 6675 7369 6f6e 2069 7320 6120 7665 7279  fusion is a very
+00000120: 2066 6173 7420 7265 6775 6c61 746f 7279   fast regulatory
+00000130: 206e 6574 776f 726b 2069 6e66 6572 656e   network inferen
+00000140: 6365 2061 6c67 6f72 6974 686d 2062 6173  ce algorithm bas
+00000150: 6564 206f 6e20 7072 6f62 6162 696c 6973  ed on probabilis
+00000160: 7469 6320 6469 6666 7573 696f 6e20 6d6f  tic diffusion mo
+00000170: 6465 6c2e 2049 7420 776f 726b 7320 7765  del. It works we
+00000180: 6c6c 206f 6e20 6765 6e65 7320 616e 6420  ll on genes and 
+00000190: 6973 2063 6170 6162 6c65 2074 6f20 7261  is capable to ra
+000001a0: 7069 646c 7920 283c 356d 696e 2920 7072  pidly (<5min) pr
+000001b0: 6564 6963 7420 6269 6f6c 6f67 6963 616c  edict biological
+000001c0: 6c79 2076 6572 6966 6961 626c 6520 6c69  ly verifiable li
+000001d0: 6e6b 7320 6672 6f6d 206c 6172 6765 2073  nks from large s
+000001e0: 696e 676c 6520 6365 6c6c 2052 4e41 2d73  ingle cell RNA-s
+000001f0: 6571 2064 6174 6120 7769 7468 2031 342c  eq data with 14,
+00000200: 3030 302b 2067 656e 6573 2e0a 0a60 6060  000+ genes...```
+00000210: 0a46 726f 6d20 4e6f 6973 6520 746f 204b  .From Noise to K
+00000220: 6e6f 776c 6564 6765 3a20 5072 6f62 6162  nowledge: Probab
+00000230: 696c 6973 7469 6320 4469 6666 7573 696f  ilistic Diffusio
+00000240: 6e2d 4261 7365 6420 4e65 7572 616c 2049  n-Based Neural I
+00000250: 6e66 6572 656e 6365 206f 6620 4765 6e65  nference of Gene
+00000260: 2052 6567 756c 6174 6f72 7920 4e65 7477   Regulatory Netw
+00000270: 6f72 6b73 0a48 616f 205a 6875 2c20 446f  orks.Hao Zhu, Do
+00000280: 6e6e 6120 4b2e 2053 6c6f 6e69 6d0a 6269  nna K. Slonim.bi
+00000290: 6f52 7869 7620 3230 3233 2e31 312e 3035  oRxiv 2023.11.05
+000002a0: 2e35 3635 3637 353b 2064 6f69 3a20 6874  .565675; doi: ht
+000002b0: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+000002c0: 2e31 3130 312f 3230 3233 2e31 312e 3035  .1101/2023.11.05
+000002d0: 2e35 3635 3637 350a 6060 600a 0a0a 2323  .565675.```...##
+000002e0: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a52   Installation..R
+000002f0: 6567 4469 6666 7573 696f 6e20 6973 206f  egDiffusion is o
+00000300: 6e20 7079 7069 2e0a 0a60 6060 0a70 6970  n pypi...```.pip
+00000310: 2069 6e73 7461 6c6c 2072 6567 6469 6666   install regdiff
+00000320: 7573 696f 6e0a 6060 600a 0a43 6865 636b  usion.```..Check
+00000330: 206f 7574 2074 6865 205b 7468 6973 2074   out the [this t
+00000340: 7574 6f72 6961 6c5d 2868 7474 7073 3a2f  utorial](https:/
+00000350: 2f74 7566 7473 6263 622e 6769 7468 7562  /tuftsbcb.github
+00000360: 2e69 6f2f 5265 6744 6966 6675 7369 6f6e  .io/RegDiffusion
+00000370: 2f71 7569 636b 5f74 6f75 722e 6874 6d6c  /quick_tour.html
+00000380: 2920 666f 7220 6120 7175 6963 6b20 746f  ) for a quick to
+00000390: 7572 206f 6620 686f 7720 746f 2075 7365  ur of how to use
+000003a0: 2052 6567 4469 6666 7573 696f 6e20 666f   RegDiffusion fo
+000003b0: 7220 796f 7572 2072 6573 6561 7263 6821  r your research!
+000003c0: 0a0a 2323 2051 7569 636b 2054 6f75 720a  ..## Quick Tour.
+000003d0: 5468 6973 2070 6163 6b61 6765 2060 7265  This package `re
+000003e0: 6764 6966 6675 7369 6f6e 6020 7072 6f76  gdiffusion` prov
+000003f0: 6964 6573 2074 6865 206f 6666 6963 6961  ides the officia
+00000400: 6c20 696d 706c 656d 656e 7461 7469 6f6e  l implementation
+00000410: 206f 6620 7468 650a 5265 6744 6966 6675   of the.RegDiffu
+00000420: 7369 6f6e 2061 6c67 6f72 6974 686d 2061  sion algorithm a
+00000430: 6e64 2061 2073 6574 206f 6620 6561 7379  nd a set of easy
+00000440: 2d74 6f2d 7573 6520 636f 6d70 616e 696f  -to-use companio
+00000450: 6e20 746f 6f6c 7320 746f 2065 7661 6c75  n tools to evalu
+00000460: 6174 652c 0a61 6e61 6c79 7a65 2c20 616e  ate,.analyze, an
+00000470: 6420 7669 7375 616c 697a 6520 7468 6520  d visualize the 
+00000480: 696e 6665 7272 6564 206e 6574 776f 726b  inferred network
+00000490: 2e20 5765 2061 6c73 6f20 7072 6f76 6964  . We also provid
+000004a0: 6520 6163 6365 7373 2074 6f6f 6c73 2074  e access tools t
+000004b0: 6f20 0a47 524e 2062 656e 6368 6d61 726b  o .GRN benchmark
+000004c0: 7320 616e 6420 7072 6570 726f 6365 7373  s and preprocess
+000004d0: 6564 2073 696e 676c 6520 6365 6c6c 2064  ed single cell d
+000004e0: 6174 6173 6574 7320 666f 7220 6576 616c  atasets for eval
+000004f0: 7561 7469 6f6e 2e20 0a0a 5765 2074 7269  uation. ..We tri
+00000500: 6564 2074 6f20 6b65 6570 2074 6865 2074  ed to keep the t
+00000510: 6f70 206c 6576 656c 2069 6e74 6572 6661  op level interfa
+00000520: 6365 2073 7472 6169 6768 7466 6f72 7761  ce straightforwa
+00000530: 7264 2e20 5269 6768 7420 6e6f 772c 2069  rd. Right now, i
+00000540: 7420 6f6e 6c79 200a 636f 6e73 6973 7473  t only .consists
+00000550: 206f 6620 3420 636f 6d70 6f6e 656e 7473   of 4 components
+00000560: 3a20 7468 6520 6052 6567 4469 6666 7573  : the `RegDiffus
+00000570: 696f 6e54 7261 696e 6572 6020 636c 6173  ionTrainer` clas
+00000580: 732c 2074 6865 2060 4752 4e60 2063 6c61  s, the `GRN` cla
+00000590: 7373 2c20 7468 6520 0a60 4752 4e45 7661  ss, the .`GRNEva
+000005a0: 6c75 6174 6f72 6020 636c 6173 732c 2061  luator` class, a
+000005b0: 6e64 2074 6865 2060 6461 7461 6020 6d6f  nd the `data` mo
+000005c0: 6475 6c65 2e20 0a0a 2d20 6052 6567 4469  dule. ..- `RegDi
+000005d0: 6666 7573 696f 6e54 7261 696e 6572 603a  ffusionTrainer`:
+000005e0: 2059 6f75 2063 616e 2075 7365 2069 7420   You can use it 
+000005f0: 746f 2074 7261 696e 2061 2060 5265 6744  to train a `RegD
+00000600: 6966 6675 7369 6f6e 6020 6d6f 6465 6c20  iffusion` model 
+00000610: 6279 200a 2020 7072 6f76 6964 696e 6720  by .  providing 
+00000620: 6c6f 6720 7472 616e 7366 6f72 6d65 6420  log transformed 
+00000630: 6578 7072 6573 7369 6f6e 2064 6174 6120  expression data 
+00000640: 696e 2061 2060 6e75 6d70 7960 2061 7272  in a `numpy` arr
+00000650: 6179 2e20 5468 6520 7472 6169 6e69 6e67  ay. The training
+00000660: 0a20 2070 726f 6365 7373 2063 6f75 6c64  .  process could
+00000670: 2062 6520 6569 7468 6572 2073 7461 7274   be either start
+00000680: 6564 206f 7220 636f 6e74 696e 7565 6420  ed or continued 
+00000690: 7573 696e 6720 7468 6520 602e 7472 6169  using the `.trai
+000006a0: 6e28 2960 206d 6574 686f 642e 2059 6f75  n()` method. You
+000006b0: 200a 2020 6361 6e20 6578 706f 7274 2074   .  can export t
+000006c0: 6865 2069 6e66 6572 7265 6420 6047 524e  he inferred `GRN
+000006d0: 6020 7573 696e 6720 7468 6520 602e 6765  ` using the `.ge
+000006e0: 745f 6772 6e28 2960 206d 6574 686f 642e  t_grn()` method.
+000006f0: 0a2d 2060 4752 4e60 3a20 5468 6520 6047  .- `GRN`: The `G
+00000700: 524e 6020 636c 6173 7320 7072 6f76 6964  RN` class provid
+00000710: 6573 2061 2063 6f6e 7461 696e 6572 2074  es a container t
+00000720: 6f20 7361 7665 2074 6865 2069 6e66 6572  o save the infer
+00000730: 7265 6420 6164 6a61 6365 6e63 790a 2020  red adjacency.  
+00000740: 6d61 7472 6978 2061 6e64 2074 6865 2063  matrix and the c
+00000750: 6f72 7265 7370 6f6e 6469 6e67 2067 656e  orresponding gen
+00000760: 6520 6e61 6d65 732e 2059 6f75 2063 616e  e names. You can
+00000770: 2073 6176 6520 7468 6520 6047 524e 6020   save the `GRN` 
+00000780: 6f62 6a65 6374 2074 6f20 0a20 2061 206c  object to .  a l
+00000790: 6f63 616c 2060 4844 4635 6020 6669 6c65  ocal `HDF5` file
+000007a0: 2075 7369 6e67 2074 6865 2060 2e74 6f5f   using the `.to_
+000007b0: 6864 6635 2829 6020 6d65 7468 6f64 2061  hdf5()` method a
+000007c0: 6e64 2072 656c 6f61 6420 7468 6520 7361  nd reload the sa
+000007d0: 7665 6420 6669 6c65 200a 2020 7573 696e  ved file .  usin
+000007e0: 6720 7468 6520 6072 6561 645f 6864 6635  g the `read_hdf5
+000007f0: 2829 6020 6675 6e63 7469 6f6e 2e20 4974  ()` function. It
+00000800: 2061 6c73 6f20 636f 6d65 7320 7769 7468   also comes with
+00000810: 2066 756e 6374 696f 6e61 6c69 7469 6573   functionalities
+00000820: 2074 6f20 0a20 2065 7870 6f72 7420 6f72   to .  export or
+00000830: 2076 6973 7561 6c69 7a65 206c 6f63 616c   visualize local
+00000840: 2072 6567 696f 6e73 2e20 466f 7220 6578   regions. For ex
+00000850: 616d 706c 652c 2079 6f75 2063 616e 2075  ample, you can u
+00000860: 7365 2074 6865 200a 2020 602e 7669 7375  se the .  `.visu
+00000870: 616c 697a 655f 6c6f 6361 6c5f 6e65 6967  alize_local_neig
+00000880: 6862 6f72 686f 6f64 2829 6020 746f 2067  hborhood()` to g
+00000890: 656e 6572 6174 6520 6120 7369 6d69 6c61  enerate a simila
+000008a0: 7220 706c 6f74 2061 7320 7573 6564 2069  r plot as used i
+000008b0: 6e20 0a20 2074 6865 2052 6567 4469 6666  n .  the RegDiff
+000008c0: 7573 696f 6e20 7061 7065 722e 2059 6f75  usion paper. You
+000008d0: 2063 616e 2061 6c73 6f20 6578 7472 6163   can also extrac
+000008e0: 7420 7468 6520 756e 6465 726c 7969 6e67  t the underlying
+000008f0: 2061 646a 6163 656e 6379 206c 6973 7420   adjacency list 
+00000900: 0a20 2075 7369 6e67 2074 6865 2060 2e65  .  using the `.e
+00000910: 7874 7261 6374 5f6e 6f64 655f 3268 6f70  xtract_node_2hop
+00000920: 5f6e 6569 6768 626f 7268 6f6f 6428 2960  _neighborhood()`
+00000930: 206d 6574 686f 642e 0a2d 2060 4752 4e45   method..- `GRNE
+00000940: 7661 6c75 6174 6f72 603a 2054 6865 2067  valuator`: The g
+00000950: 726f 756e 6420 7472 7574 6820 6f66 2072  round truth of r
+00000960: 6567 756c 6174 6f72 7920 7265 6c61 7469  egulatory relati
+00000970: 6f6e 7368 6970 206f 6674 656e 2065 7869  onship often exi
+00000980: 7374 2061 7320 0a20 206c 6973 7420 6f66  st as .  list of
+00000990: 2065 6467 6573 2062 7574 2074 6865 2076   edges but the v
+000009a0: 616c 7565 7320 746f 2062 6520 6576 616c  alues to be eval
+000009b0: 7561 7465 6420 6172 6520 6f66 7465 6e20  uated are often 
+000009c0: 696e 2061 646a 6163 656e 6379 206d 6174  in adjacency mat
+000009d0: 7269 782e 200a 2020 5468 6520 6047 524e  rix. .  The `GRN
+000009e0: 4576 616c 7561 746f 7260 2063 6c61 7373  Evaluator` class
+000009f0: 2069 7320 6465 7369 676e 6564 2074 6f20   is designed to 
+00000a00: 6669 6c6c 2074 6865 2067 6170 2e20 5269  fill the gap. Ri
+00000a10: 6768 7420 6e6f 7720 6974 2073 7570 706f  ght now it suppo
+00000a20: 7274 730a 2020 636f 6d6d 6f6e 206d 6574  rts.  common met
+00000a30: 7269 6373 2073 7563 6820 6173 2041 5552  rics such as AUR
+00000a40: 4f43 2c20 4155 5052 2c20 4155 5052 2052  OC, AUPR, AUPR R
+00000a50: 6174 696f 2c20 4550 2c20 616e 6420 4550  atio, EP, and EP
+00000a60: 522e 200a 2d20 6064 6174 6160 206d 6f64  R. .- `data` mod
+00000a70: 756c 653a 2052 6967 6874 206e 6f77 2c20  ule: Right now, 
+00000a80: 7468 6520 6064 6174 6160 206d 6f64 756c  the `data` modul
+00000a90: 6520 696e 636c 7564 6573 2071 7569 636b  e includes quick
+00000aa0: 2061 6363 6573 7320 746f 2042 4545 4c49   access to BEELI
+00000ab0: 4e45 200a 2020 6265 6e63 686d 6172 6b73  NE .  benchmarks
+00000ac0: 2061 6e64 206f 7572 2070 7265 7072 6f63   and our preproc
+00000ad0: 6573 7365 6420 7369 6e67 6c65 2063 656c  essed single cel
+00000ae0: 6c20 6461 7461 7365 7473 206f 6e20 6d6f  l datasets on mo
+00000af0: 7573 6520 6d69 6372 6f67 6c69 612e 200a  use microglia. .
+00000b00: 0a23 2320 556e 6465 7273 7461 6e64 696e  .## Understandin
+00000b10: 6720 7468 6520 496e 6665 7272 6564 204e  g the Inferred N
+00000b20: 6574 776f 726b 730a 4166 7465 7220 7468  etworks.After th
+00000b30: 6520 6052 6567 4469 6666 7573 696f 6e60  e `RegDiffusion`
+00000b40: 206d 6f64 656c 2063 6f6e 7665 7267 6573   model converges
+00000b50: 2c20 7768 6174 2079 6f75 2067 6574 2069  , what you get i
+00000b60: 7320 7369 6d70 6c79 2061 6e20 0a60 6164  s simply an .`ad
+00000b70: 6a61 6365 6e63 7960 206d 6174 7269 782e  jacency` matrix.
+00000b80: 2057 6865 6e20 796f 7520 6861 7665 2074   When you have t
+00000b90: 686f 7573 616e 6473 206f 7220 7465 6e73  housands or tens
+00000ba0: 206f 6620 7468 6f75 7361 6e64 7320 6f66   of thousands of
+00000bb0: 2067 656e 6573 2c20 0a69 7427 7320 6765   genes, .it's ge
+00000bc0: 7474 696e 6720 6469 6666 6963 756c 7420  tting difficult 
+00000bd0: 746f 2061 6e61 6c79 7a65 206d 6174 7269  to analyze matri
+00000be0: 7820 6174 2074 6861 7420 7363 616c 652e  x at that scale.
+00000bf0: 2049 6e20 6f75 7220 7061 7065 722c 2077   In our paper, w
+00000c00: 6520 0a70 726f 706f 7365 2061 2077 6179  e .propose a way
+00000c10: 2074 6f20 616e 616c 797a 6520 7468 6520   to analyze the 
+00000c20: 6c6f 6361 6c20 6e65 7477 6f72 6b20 6279  local network by
+00000c30: 2066 6f63 7573 696e 6720 6f6e 2074 6865   focusing on the
+00000c40: 2067 656e 6573 2079 6f75 2063 6172 6520   genes you care 
+00000c50: 0a74 6865 206d 6f73 742e 2043 6865 636b  .the most. Check
+00000c60: 206f 7574 2074 6865 2074 7574 6f72 6961   out the tutoria
+00000c70: 6c73 206f 6e20 7468 6520 6c65 6674 2073  ls on the left s
+00000c80: 6964 6520 666f 7220 686f 7720 746f 2070  ide for how to p
+00000c90: 6572 666f 726d 2061 2073 696d 696c 6172  erform a similar
+00000ca0: 200a 6e65 7477 6f72 6b20 616e 616c 7973   .network analys
+00000cb0: 6973 206c 696b 6520 7468 6520 6f6e 6520  is like the one 
+00000cc0: 7765 2064 6964 2069 6e20 7468 6520 7061  we did in the pa
+00000cd0: 7065 722e 2057 6520 6172 6520 616c 736f  per. We are also
+00000ce0: 2077 6f72 6b69 6e67 206f 6e20 616e 200a   working on an .
+00000cf0: 696e 7465 7261 6374 6976 6520 746f 6f6c  interactive tool
+00000d00: 2074 6f20 616e 616c 797a 6520 7361 7665   to analyze save
+00000d10: 6420 4752 4e20 6f62 6a65 6374 2e20 0a0a  d GRN object. ..
+00000d20: 215b 5d28 6874 7470 733a 2f2f 7261 772e  ![](https://raw.
+00000d30: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000d40: 742e 636f 6d2f 5475 6674 7342 4342 2f52  t.com/TuftsBCB/R
+00000d50: 6567 4469 6666 7573 696f 6e2f 6d61 7374  egDiffusion/mast
+00000d60: 6572 2f72 6573 6f75 7263 6573 2f61 706f  er/resources/apo
+00000d70: 655f 7265 672e 706e 6729 0a0a 2323 2049  e_reg.png)..## I
+00000d80: 6e66 6572 656e 6365 2053 7065 6564 0a49  nference Speed.I
+00000d90: 6e66 6572 656e 6365 206f 6e20 6e65 7477  nference on netw
+00000da0: 6f72 6b73 2077 6974 6820 3135 2c30 3030  orks with 15,000
+00000db0: 2067 656e 6573 2074 616b 6573 2075 6e64   genes takes und
+00000dc0: 6572 2035 206d 696e 7574 6573 206f 6e20  er 5 minutes on 
+00000dd0: 616e 2041 3130 3020 4750 552e 200a 496e  an A100 GPU. .In
+00000de0: 2063 6f6e 7472 6173 742c 2070 7265 7669   contrast, previ
+00000df0: 6f75 7320 5641 4520 6261 7365 6420 6d6f  ous VAE based mo
+00000e00: 6465 6c73 2077 6f75 6c64 2074 616b 6520  dels would take 
+00000e10: 6d6f 7265 2074 6861 6e20 3420 686f 7572  more than 4 hour
+00000e20: 7320 6f6e 2074 6865 2073 616d 6520 0a64  s on the same .d
+00000e30: 6576 6963 652e 2045 7665 6e20 6966 2079  evice. Even if y
+00000e40: 6f75 2064 6f6e 2774 2068 6176 6520 6163  ou don't have ac
+00000e50: 6365 7373 2074 6f20 7468 6f73 6520 6661  cess to those fa
+00000e60: 6e63 7920 4750 5520 6361 7264 732c 2052  ncy GPU cards, R
+00000e70: 6567 4469 6666 7573 696f 6e20 0a73 7469  egDiffusion .sti
+00000e80: 6c6c 2077 6f72 6b73 2e20 496e 6665 7265  ll works. Infere
+00000e90: 6e63 6520 6f6e 2074 6865 2073 616d 6520  nce on the same 
+00000ea0: 6c61 7267 6520 6e65 7477 6f72 6b20 7461  large network ta
+00000eb0: 6b65 7320 726f 7567 686c 7920 3320 686f  kes roughly 3 ho
+00000ec0: 7572 7320 6f6e 2061 200a 6d69 642d 7261  urs on a .mid-ra
+00000ed0: 6e67 6520 3132 2d63 6f72 6520 4350 552e  nge 12-core CPU.
+00000ee0: 20
```

### Comparing `regdiffusion-0.0.5/pyproject.toml` & `regdiffusion-0.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     { name = "Donna Slonim", email="donna.slonim@tufts.edu"}
 ]
 maintainers = [
     { name = "Hao Zhu", email = "haozhu233@gmail.com" }
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
-version = "0.0.5"
+version = "0.0.6"
 description = "Gene Regulatory Networks Inference using diffusion model"
 
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 
 dependencies = [
     "numpy>=1.16.5",
     "pandas>=1.1.1",
```

### Comparing `regdiffusion-0.0.5/regdiffusion/data/beeline.py` & `regdiffusion-0.0.6/regdiffusion/data/beeline.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.5/regdiffusion/data/microglia.py` & `regdiffusion-0.0.6/regdiffusion/data/microglia.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.5/regdiffusion/data/utils.py` & `regdiffusion-0.0.6/regdiffusion/data/.ipynb_checkpoints/utils-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.5/regdiffusion/evaluator.py` & `regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/evaluator-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.5/regdiffusion/grn.py` & `regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/grn-checkpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -257,26 +257,26 @@
         """
         if isinstance(genes, str):
             genes = [genes]
         hop0_genes = set(genes)
         hop1 = pd.concat([
             self.extract_node_neighbors(g, k=k) for g in hop0_genes
         ])
-        hop1['weight'] = 0
+        hop1['hop'] = 0
         hop1_genes = set()
         for g in hop1.source:
             if g not in hop0_genes:
                 hop1_genes.add(g)
         for g in hop1.target:
             if g not in hop0_genes:
                 hop1_genes.add(g)
         hop2s = pd.concat([
             self.extract_node_neighbors(g, k=k) for g in hop1_genes
         ])
-        hop2s['weight'] = 1
+        hop2s['hop'] = 1
         hop2_genes = set()
         for g in hop2s.source:
             if g not in hop0_genes and g not in hop1_genes:
                 hop2_genes.add(g)
         for g in hop2s.target:
             if g not in hop0_genes and g not in hop1_genes:
                 hop2_genes.add(g)
@@ -284,18 +284,56 @@
         for g in hop2_genes:
             hop3 = self.extract_node_neighbors(g, k=k)
             hop3 = hop3[
                 hop3.source.isin(hop2_genes) & hop3.target.isin(hop2_genes)
             ]
             hop3s.append(hop3)
         hop3s = pd.concat(hop3s)
-        hop3s['weight'] = 2
+        hop3s['hop'] = 2
         adj_table = pd.concat([hop1, hop2s, hop3s]).reset_index(drop=True)
         return adj_table
 
+    def extract_node_1hop_neighborhood(
+        self, genes: Union[str, List[str]], k: int = 20
+    ) -> pd.DataFrame:
+        """
+        Generate a pandas dataframe for the local neighborhood (1-hop) around 
+        selected gene(s). 
+
+        Args:
+            genes (str, List(str)): A single gene or a list of genes to inspect.
+            k (int): Top-k edges to inspect on each node.
+            node_size (int): The size of nodes in the visualization.
+        """
+        if isinstance(genes, str):
+            genes = [genes]
+        hop0_genes = set(genes)
+        hop1 = pd.concat([
+            self.extract_node_neighbors(g, k=k) for g in hop0_genes
+        ])
+        hop1['hop'] = 0
+        hop1_genes = set()
+        for g in hop1.source:
+            if g not in hop0_genes:
+                hop1_genes.add(g)
+        for g in hop1.target:
+            if g not in hop0_genes:
+                hop1_genes.add(g)
+        hop2s = []
+        for g in hop1_genes:
+            hop2 = self.extract_node_neighbors(g, k=k)
+            hop2 = hop2[
+                hop2.source.isin(hop1_genes) & hop2.target.isin(hop1_genes)
+            ]
+            hop2s.append(hop2)
+        hop2s = pd.concat(hop2s)
+        hop2s['hop'] = 1
+        adj_table = pd.concat([hop1, hop2s]).reset_index(drop=True)
+        return adj_table
+
     def visualize_local_neighborhood(
         self, genes: Union[str, List[str]], k: int = 20, 
         node_size: int = 8, edge_widths: List[int] = [2, 1, 0.5], 
         font_size: int = 30,
         node_group_dict: Dict = None, 
         cdn_resources: str = 'remote', notebook: bool = True):
         """
@@ -330,15 +368,15 @@
             node_shape = 'star' if node in genes else 'dot'
             node_group = None if node_group_dict is None else node_group_dict[node]
             g.add_node(node, label=node, size=node_size, 
                        shape=node_shape, group=node_group, 
                        font={"size": font_size})
         
         for _, row in local_adj_table.iterrows():
-            g.add_edge(row['source'], row['target'], width=row['weight'])
+            g.add_edge(row['source'], row['target'], width=row['hop'])
         
         g.repulsion()
         return g
 
     def to_hdf5(self, file_path: str, as_sparse: bool = False):
         """
         Save GRN into a HDF5 file. You have the option to save as a sparse
```

### Comparing `regdiffusion-0.0.5/regdiffusion/logger.py` & `regdiffusion-0.0.6/regdiffusion/logger.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.5/regdiffusion/models/regdiffusion.py` & `regdiffusion-0.0.6/regdiffusion/models/regdiffusion.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.5/regdiffusion/trainer.py` & `regdiffusion-0.0.6/regdiffusion/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from torch.utils.data import DataLoader
 from torch.utils.data.dataset import TensorDataset
 from .models import RegDiffusion
 from tqdm import tqdm
 from .logger import LightLogger
 from datetime import datetime
 from .grn import GRN
+from .evaluator import GRNEvaluator
+from .logger import LightLogger
 import matplotlib.pyplot as plt
 import warnings
 
 def linear_beta_schedule(timesteps, start_noise, end_noise):
     scale = 1000 / timesteps
     beta_start = scale * start_noise
     beta_end = scale * end_noise
```

