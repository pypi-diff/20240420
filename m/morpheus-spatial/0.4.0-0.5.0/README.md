# Comparing `tmp/morpheus_spatial-0.4.0.tar.gz` & `tmp/morpheus_spatial-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morpheus_spatial-0.4.0.tar", max compression
+gzip compressed data, was "morpheus_spatial-0.5.0.tar", max compression
```

## Comparing `morpheus_spatial-0.4.0.tar` & `morpheus_spatial-0.5.0.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0     1465 2024-03-24 22:07:48.345779 morpheus_spatial-0.4.0/README.md
--rw-r--r--   0        0        0      611 2024-04-06 01:12:20.348217 morpheus_spatial-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      172 2024-03-24 20:40:40.558026 morpheus_spatial-0.4.0/src/morpheus/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 19:57:48.985646 morpheus_spatial-0.4.0/src/morpheus/api/__init__py
--rw-r--r--   0        0        0      535 2024-03-24 20:40:40.558500 morpheus_spatial-0.4.0/src/morpheus/api/__pycache__/defaults.cpython-39.pyc
--rw-r--r--   0        0        0     7022 2024-03-24 20:40:40.559130 morpheus_spatial-0.4.0/src/morpheus/api/__pycache__/interfaces.cpython-39.pyc
--rw-r--r--   0        0        0      453 2024-03-24 19:57:49.004227 morpheus_spatial-0.4.0/src/morpheus/api/defaults.py
--rw-r--r--   0        0        0     6889 2024-03-24 19:57:49.010975 morpheus_spatial-0.4.0/src/morpheus/api/interfaces.py
--rw-r--r--   0        0        0       77 2024-03-24 20:40:40.559608 morpheus_spatial-0.4.0/src/morpheus/classification/__init__.py
--rw-r--r--   0        0        0      276 2024-03-24 20:40:58.819685 morpheus_spatial-0.4.0/src/morpheus/classification/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4787 2024-03-24 20:40:58.763994 morpheus_spatial-0.4.0/src/morpheus/classification/__pycache__/classifier.cpython-39.pyc
--rw-r--r--   0        0        0     1728 2024-03-24 20:40:58.818768 morpheus_spatial-0.4.0/src/morpheus/classification/__pycache__/train.cpython-39.pyc
--rw-r--r--   0        0        0     5504 2024-03-24 20:40:40.561582 morpheus_spatial-0.4.0/src/morpheus/classification/classifier.py
--rw-r--r--   0        0        0     2058 2024-03-24 20:40:40.562027 morpheus_spatial-0.4.0/src/morpheus/classification/train.py
--rw-r--r--   0        0        0       35 2024-03-24 19:57:49.050136 morpheus_spatial-0.4.0/src/morpheus/confidence/__init__.py
--rw-r--r--   0        0        0      218 2024-03-24 20:40:40.562476 morpheus_spatial-0.4.0/src/morpheus/confidence/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6828 2024-03-24 20:40:40.562985 morpheus_spatial-0.4.0/src/morpheus/confidence/__pycache__/trustscore.cpython-39.pyc
--rw-r--r--   0        0        0     8238 2024-03-24 19:57:49.069331 morpheus_spatial-0.4.0/src/morpheus/confidence/trustscore.py
--rw-r--r--   0        0        0      679 2024-03-24 19:57:49.079309 morpheus_spatial-0.4.0/src/morpheus/configuration/Types.py
--rw-r--r--   0        0        0       21 2024-03-24 19:57:49.085704 morpheus_spatial-0.4.0/src/morpheus/configuration/__init__.py
--rw-r--r--   0        0        0      154 2024-03-24 19:57:49.093969 morpheus_spatial-0.4.0/src/morpheus/counterfactual/__init__.py
--rw-r--r--   0        0        0      316 2024-03-24 20:40:40.563441 morpheus_spatial-0.4.0/src/morpheus/counterfactual/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    26923 2024-04-06 01:07:40.040504 morpheus_spatial-0.4.0/src/morpheus/counterfactual/__pycache__/cf.cpython-39.pyc
--rw-r--r--   0        0        0    10429 2024-04-06 00:56:25.424106 morpheus_spatial-0.4.0/src/morpheus/counterfactual/__pycache__/generate.cpython-39.pyc
--rw-r--r--   0        0        0    48197 2024-04-06 01:05:26.035891 morpheus_spatial-0.4.0/src/morpheus/counterfactual/cf.py
--rw-r--r--   0        0        0    34031 2024-04-05 06:20:06.264699 morpheus_spatial-0.4.0/src/morpheus/counterfactual/cf_in_progress.py
--rw-r--r--   0        0        0    12218 2024-04-05 23:40:35.387029 morpheus_spatial-0.4.0/src/morpheus/counterfactual/generate.py
--rw-r--r--   0        0        0       44 2024-03-24 19:57:49.234244 morpheus_spatial-0.4.0/src/morpheus/datasets/__init__.py
--rw-r--r--   0        0        0    14299 2024-03-24 22:34:11.722417 morpheus_spatial-0.4.0/src/morpheus/datasets/__pycache__/spatial_dataset.cpython-39.pyc
--rw-r--r--   0        0        0     2874 2024-03-24 20:40:40.572611 morpheus_spatial-0.4.0/src/morpheus/datasets/__pycache__/torch_dataset.cpython-39.pyc
--rw-r--r--   0        0        0    18422 2024-03-24 22:30:27.333512 morpheus_spatial-0.4.0/src/morpheus/datasets/spatial_dataset.py
--rw-r--r--   0        0        0     3360 2024-03-24 19:57:49.314337 morpheus_spatial-0.4.0/src/morpheus/datasets/torch_dataset.py
--rw-r--r--   0        0        0        0 2024-03-24 19:57:49.315867 morpheus_spatial-0.4.0/src/morpheus/utils/__init__.py
--rw-r--r--   0        0        0      168 2024-03-24 20:40:40.573764 morpheus_spatial-0.4.0/src/morpheus/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      945 2024-03-24 20:40:40.574200 morpheus_spatial-0.4.0/src/morpheus/utils/__pycache__/saving.cpython-39.pyc
--rw-r--r--   0        0        0      188 2024-03-24 20:40:40.574625 morpheus_spatial-0.4.0/src/morpheus/utils/__pycache__/version.cpython-39.pyc
--rw-r--r--   0        0        0     2880 2024-04-05 06:18:14.436561 morpheus_spatial-0.4.0/src/morpheus/utils/gradients.py
--rw-r--r--   0        0        0     5862 2024-03-24 19:57:49.343166 morpheus_spatial-0.4.0/src/morpheus/utils/patchify.py
--rw-r--r--   0        0        0      893 2024-03-24 19:57:49.348980 morpheus_spatial-0.4.0/src/morpheus/utils/saving.py
--rw-r--r--   0        0        0      259 2024-03-24 19:57:49.352361 morpheus_spatial-0.4.0/src/morpheus/utils/set_seeds.py
--rw-r--r--   0        0        0      212 2024-03-24 19:57:49.358398 morpheus_spatial-0.4.0/src/morpheus/utils/version.py
--rw-r--r--   0        0        0     2180 1970-01-01 00:00:00.000000 morpheus_spatial-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1465 2024-04-06 21:01:32.002949 morpheus_spatial-0.5.0/README.md
+-rw-r--r--   0        0        0      660 2024-04-19 22:49:02.691745 morpheus_spatial-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      172 2024-04-06 21:01:32.171228 morpheus_spatial-0.5.0/src/morpheus/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:57:48.985646 morpheus_spatial-0.5.0/src/morpheus/api/__init__py
+-rw-r--r--   0        0        0      535 2024-04-06 21:01:32.183254 morpheus_spatial-0.5.0/src/morpheus/api/__pycache__/defaults.cpython-39.pyc
+-rw-r--r--   0        0        0     7022 2024-04-06 21:01:32.187773 morpheus_spatial-0.5.0/src/morpheus/api/__pycache__/interfaces.cpython-39.pyc
+-rw-r--r--   0        0        0      453 2024-03-24 19:57:49.004227 morpheus_spatial-0.5.0/src/morpheus/api/defaults.py
+-rw-r--r--   0        0        0     6889 2024-03-24 19:57:49.010975 morpheus_spatial-0.5.0/src/morpheus/api/interfaces.py
+-rw-r--r--   0        0        0       77 2024-04-06 21:01:32.192557 morpheus_spatial-0.5.0/src/morpheus/classification/__init__.py
+-rw-r--r--   0        0        0      276 2024-04-10 06:59:59.441169 morpheus_spatial-0.5.0/src/morpheus/classification/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4765 2024-04-19 04:33:38.040542 morpheus_spatial-0.5.0/src/morpheus/classification/__pycache__/classifier.cpython-39.pyc
+-rw-r--r--   0        0        0     1728 2024-04-10 06:59:59.444701 morpheus_spatial-0.5.0/src/morpheus/classification/__pycache__/train.cpython-39.pyc
+-rw-r--r--   0        0        0     5486 2024-04-19 04:33:38.043597 morpheus_spatial-0.5.0/src/morpheus/classification/classifier.py
+-rw-r--r--   0        0        0     2058 2024-04-06 21:01:32.249981 morpheus_spatial-0.5.0/src/morpheus/classification/train.py
+-rw-r--r--   0        0        0       35 2024-03-24 19:57:49.050136 morpheus_spatial-0.5.0/src/morpheus/confidence/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-06 21:01:32.290849 morpheus_spatial-0.5.0/src/morpheus/confidence/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6828 2024-04-06 21:01:32.298328 morpheus_spatial-0.5.0/src/morpheus/confidence/__pycache__/trustscore.cpython-39.pyc
+-rw-r--r--   0        0        0     8238 2024-03-24 19:57:49.069331 morpheus_spatial-0.5.0/src/morpheus/confidence/trustscore.py
+-rw-r--r--   0        0        0      679 2024-04-06 21:01:32.304450 morpheus_spatial-0.5.0/src/morpheus/configuration/Types.py
+-rw-r--r--   0        0        0       21 2024-03-24 19:57:49.085704 morpheus_spatial-0.5.0/src/morpheus/configuration/__init__.py
+-rw-r--r--   0        0        0      154 2024-03-24 19:57:49.093969 morpheus_spatial-0.5.0/src/morpheus/counterfactual/__init__.py
+-rw-r--r--   0        0        0      316 2024-04-06 21:01:32.309904 morpheus_spatial-0.5.0/src/morpheus/counterfactual/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    25561 2024-04-19 04:33:38.047299 morpheus_spatial-0.5.0/src/morpheus/counterfactual/__pycache__/cf.cpython-39.pyc
+-rw-r--r--   0        0        0    10955 2024-04-19 04:33:38.051569 morpheus_spatial-0.5.0/src/morpheus/counterfactual/__pycache__/generate.cpython-39.pyc
+-rw-r--r--   0        0        0    40837 2024-04-19 04:33:38.055755 morpheus_spatial-0.5.0/src/morpheus/counterfactual/cf.py
+-rw-r--r--   0        0        0    48270 2024-04-19 04:33:38.060209 morpheus_spatial-0.5.0/src/morpheus/counterfactual/cf_tf.py
+-rw-r--r--   0        0        0    14488 2024-04-19 04:33:38.065031 morpheus_spatial-0.5.0/src/morpheus/counterfactual/generate.py
+-rw-r--r--   0        0        0       44 2024-03-24 19:57:49.234244 morpheus_spatial-0.5.0/src/morpheus/datasets/__init__.py
+-rw-r--r--   0        0        0    14356 2024-04-12 21:21:41.456616 morpheus_spatial-0.5.0/src/morpheus/datasets/__pycache__/spatial_dataset.cpython-39.pyc
+-rw-r--r--   0        0        0     2874 2024-04-10 06:59:59.465923 morpheus_spatial-0.5.0/src/morpheus/datasets/__pycache__/torch_dataset.cpython-39.pyc
+-rw-r--r--   0        0        0    18516 2024-04-10 06:59:59.482213 morpheus_spatial-0.5.0/src/morpheus/datasets/spatial_dataset.py
+-rw-r--r--   0        0        0     3360 2024-04-06 21:01:32.713288 morpheus_spatial-0.5.0/src/morpheus/datasets/torch_dataset.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:57:49.315867 morpheus_spatial-0.5.0/src/morpheus/utils/__init__.py
+-rw-r--r--   0        0        0      168 2024-04-06 21:01:32.718919 morpheus_spatial-0.5.0/src/morpheus/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      945 2024-04-06 21:01:32.724637 morpheus_spatial-0.5.0/src/morpheus/utils/__pycache__/saving.cpython-39.pyc
+-rw-r--r--   0        0        0      188 2024-04-06 21:01:32.732206 morpheus_spatial-0.5.0/src/morpheus/utils/__pycache__/version.cpython-39.pyc
+-rw-r--r--   0        0        0     2880 2024-04-06 21:01:32.739861 morpheus_spatial-0.5.0/src/morpheus/utils/gradients.py
+-rw-r--r--   0        0        0     5862 2024-04-06 21:01:32.746763 morpheus_spatial-0.5.0/src/morpheus/utils/patchify.py
+-rw-r--r--   0        0        0      893 2024-03-24 19:57:49.348980 morpheus_spatial-0.5.0/src/morpheus/utils/saving.py
+-rw-r--r--   0        0        0      212 2024-03-24 19:57:49.358398 morpheus_spatial-0.5.0/src/morpheus/utils/version.py
+-rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 morpheus_spatial-0.5.0/PKG-INFO
```

### Comparing `morpheus_spatial-0.4.0/README.md` & `morpheus_spatial-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.4.0/src/morpheus/api/__pycache__/defaults.cpython-39.pyc` & `morpheus_spatial-0.5.0/src/morpheus/api/__pycache__/defaults.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.4.0/src/morpheus/api/__pycache__/interfaces.cpython-39.pyc` & `morpheus_spatial-0.5.0/src/morpheus/api/__pycache__/interfaces.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.4.0/src/morpheus/api/interfaces.py` & `morpheus_spatial-0.5.0/src/morpheus/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.4.0/src/morpheus/classification/__pycache__/classifier.cpython-39.pyc` & `morpheus_spatial-0.5.0/src/morpheus/classification/__pycache__/classifier.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Mar 24 20:40:40 2024 UTC, .py size: 5504 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 c88f 0066 8015 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 f1ec 2166 6e15 0000  a.........!fn...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 6d04 0200 0100 6d05 5a06 0100  d.l.m.....m.Z...
 00000050: 6400 6402 6c02 6d07 5a07 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c08 6d04 5a04 0100 4700 6404 6405 8400  l.m.Z...G.d.d...
 00000070: 6405 6501 6a09 8303 5a0a 640c 650b 650c  d.e.j...Z.d.e.e.
@@ -33,268 +33,266 @@
 00000200: 6573 da09 6f70 7469 6d69 7a65 72da 106f  es..optimizer..o
 00000210: 7074 696d 697a 6572 5f70 6172 616d 73da  ptimizer_params.
 00000220: 056c 6f77 6572 da04 6172 6368 da14 7361  .lower..arch..sa
 00000230: 7665 5f68 7970 6572 7061 7261 6d65 7465  ve_hyperparamete
 00000240: 7273 da0b 6275 696c 645f 6d6f 6465 6c29  rs..build_model)
 00000250: 07da 0473 656c 66da 0b69 6e5f 6368 616e  ...self..in_chan
 00000260: 6e65 6c73 da08 696d 675f 7369 7a65 7210  nels..img_sizer.
-00000270: 0000 00da 126e 756d 5f74 6172 6765 745f  .....num_target_
+00000270: 0000 005a 126e 756d 5f74 6172 6765 745f  ...Z.num_target_
 00000280: 636c 6173 7365 7372 0d00 0000 720e 0000  classesr....r...
 00000290: 00a9 01da 095f 5f63 6c61 7373 5f5f a900  .....__class__..
 000002a0: fa58 2f63 656e 7472 616c 2f68 6f6d 652f  .X/central/home/
 000002b0: 7a77 616e 6732 2f6d 6f72 7068 6575 732d  zwang2/morpheus-
 000002c0: 7370 6174 6961 6c2f 6d6f 7270 6865 7573  spatial/morpheus
 000002d0: 2f73 7263 2f6d 6f72 7068 6575 732f 636c  /src/morpheus/cl
 000002e0: 6173 7369 6669 6361 7469 6f6e 2f63 6c61  assification/cla
 000002f0: 7373 6966 6965 722e 7079 720a 0000 0009  ssifier.pyr.....
 00000300: 0000 0073 1400 0000 0009 0a01 0601 0801  ...s............
 00000310: 0801 0601 0601 0601 0a03 0803 7a18 5061  ............z.Pa
 00000320: 7463 6843 6c61 7373 6966 6965 722e 5f5f  tchClassifier.__
 00000330: 696e 6974 5f5f 6303 0000 0000 0000 0000  init__c.........
 00000340: 0000 0005 0000 000a 0000 0043 0000 0073  ...........C...s
-00000350: 0801 0000 7c00 6a00 6401 6b02 7282 7401  ....|.j.d.k.r.t.
+00000350: 0a01 0000 7c00 6a00 6401 6b02 7284 7401  ....|.j.d.k.r.t.
 00000360: 6a02 6a03 6402 6401 7c01 6403 7c01 6404  j.j.d.d.|.d.|.d.
-00000370: 8d05 7d03 7401 6a04 a005 a100 7d04 7c04  ..}.t.j.....}.|.
-00000380: a006 6405 7404 a007 a100 a102 0100 7c04  ..d.t.........|.
-00000390: a006 6406 7404 a008 7c02 6407 1900 7c02  ..d.t...|.d...|.
-000003a0: 6403 1900 1400 7c00 6a09 a102 a102 0100  d.....|.j.......
-000003b0: 7c04 a006 6408 7404 6a0a 6403 6409 8d01  |...d.t.j.d.d...
-000003c0: a102 0100 7404 6a05 7c03 7c04 6702 8e00  ....t.j.|.|.g...
-000003d0: 7c00 5f0b 6e82 7c00 6a00 640a 6b02 72ce  |._.n.|.j.d.k.r.
-000003e0: 7404 a005 7404 a008 7c01 640b a102 7404  t...t...|.d...t.
-000003f0: a00c a100 7404 a008 640b 640c a102 7404  ....t...d.d...t.
-00000400: a00c a100 7404 a008 640c 7c00 6a09 a102  ....t...d.|.j...
-00000410: 7404 6a0a 6403 6409 8d01 a106 7c00 5f0b  t.j.d.d.....|._.
-00000420: 6e36 7c00 6a00 640d 6b02 72f4 7404 a005  n6|.j.d.k.r.t...
-00000430: 7404 a008 7c01 6403 a102 7404 a00d a100  t...|.d...t.....
-00000440: a102 7c00 5f0b 6e10 740e 640e 7c00 6a0f  ..|._.n.t.d.|.j.
-00000450: 9b00 9d02 8301 8201 640f 5300 2910 7a43  ........d.S.).zC
-00000460: 0a20 2020 2020 2020 2053 656c 6563 7473  .        Selects
-00000470: 2061 6e64 2062 7569 6c64 7320 7468 6520   and builds the 
-00000480: 6368 6f73 656e 206d 6f64 656c 2061 7263  chosen model arc
-00000490: 6869 7465 6374 7572 652e 0a20 2020 2020  hitecture..     
-000004a0: 2020 2072 0500 0000 7a26 6d61 7465 7573     r....z&mateus
-000004b0: 7a62 7564 612f 6272 6169 6e2d 7365 676d  zbuda/brain-segm
-000004c0: 656e 7461 7469 6f6e 2d70 7974 6f72 6368  entation-pytorch
-000004d0: e901 0000 0029 0372 1400 0000 da0c 6f75  .....).r......ou
-000004e0: 745f 6368 616e 6e65 6c73 da0d 696e 6974  t_channels..init
-000004f0: 5f66 6561 7475 7265 73da 0766 6c61 7474  _features..flatt
-00000500: 656e da02 6663 7201 0000 00da 0361 6374  en..fcr......act
-00000510: a901 da03 6469 6dda 036d 6c70 e91e 0000  ....dim..mlp....
-00000520: 00e9 0a00 0000 7208 0000 007a 1c49 6e76  ......r....z.Inv
-00000530: 616c 6964 206d 6f64 656c 2061 7263 6869  alid model archi
-00000540: 7465 6374 7572 653a 204e 2910 7210 0000  tecture: N).r...
-00000550: 00da 0574 6f72 6368 da03 6875 62da 046c  ...torch..hub..l
-00000560: 6f61 6472 0200 0000 da0a 5365 7175 656e  oadr......Sequen
-00000570: 7469 616c da0a 6164 645f 6d6f 6475 6c65  tial..add_module
-00000580: da07 466c 6174 7465 6eda 064c 696e 6561  ..Flatten..Linea
-00000590: 7272 0c00 0000 da07 536f 6674 6d61 7872  rr......Softmaxr
-000005a0: 0b00 0000 da04 5265 4c55 da07 5369 676d  ......ReLU..Sigm
-000005b0: 6f69 64da 0a56 616c 7565 4572 726f 72da  oid..ValueError.
-000005c0: 0a6d 6f64 656c 5f61 7263 6829 0572 1300  .model_arch).r..
-000005d0: 0000 7214 0000 0072 1500 0000 da08 6261  ..r....r......ba
-000005e0: 636b 626f 6e65 da0a 636c 6173 7369 6669  ckbone..classifi
-000005f0: 6572 7219 0000 0072 1900 0000 721a 0000  err....r....r...
-00000600: 0072 1200 0000 2100 0000 7336 0000 0000  .r....!...s6....
-00000610: 040a 0106 0102 0102 0102 0102 0102 fb06  ................
-00000620: 070a 0110 0104 011a ff04 0314 0112 010a  ................
-00000630: 0104 010a 0106 010a 0106 010c 010a fa08  ................
-00000640: 080a 011c 027a 1b50 6174 6368 436c 6173  .....z.PatchClas
-00000650: 7369 6669 6572 2e62 7569 6c64 5f6d 6f64  sifier.build_mod
-00000660: 656c 6302 0000 0000 0000 0000 0000 0002  elc.............
-00000670: 0000 0003 0000 0043 0000 0073 1400 0000  .......C...s....
-00000680: 7c00 6a00 a001 a100 0100 7c00 a000 7c01  |.j.......|...|.
-00000690: a101 5300 2901 4e29 0272 0b00 0000 da04  ..S.).N).r......
-000006a0: 6576 616c 2902 7213 0000 00da 0178 7219  eval).r......xr.
-000006b0: 0000 0072 1900 0000 721a 0000 00da 0766  ...r....r......f
-000006c0: 6f72 7761 7264 4200 0000 7304 0000 0000  orwardB...s.....
-000006d0: 010a 017a 1750 6174 6368 436c 6173 7369  ...z.PatchClassi
-000006e0: 6669 6572 2e66 6f72 7761 7264 6301 0000  fier.forwardc...
-000006f0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00000700: 0043 0000 0073 2800 0000 7c00 6a00 6401  .C...s(...|.j.d.
-00000710: 6b02 7224 7401 6a02 6a03 7c00 a004 a100  k.r$t.j.j.|.....
-00000720: 6601 6900 7c00 6a05 a401 8e01 5300 6400  f.i.|.j.....S.d.
-00000730: 5300 2902 4e72 0700 0000 2906 720d 0000  S.).Nr....).r...
-00000740: 0072 2600 0000 da05 6f70 7469 6dda 0441  .r&.....optim..A
-00000750: 6461 6dda 0a70 6172 616d 6574 6572 7372  dam..parametersr
-00000760: 0e00 0000 2901 7213 0000 0072 1900 0000  ....).r....r....
-00000770: 7219 0000 0072 1a00 0000 da14 636f 6e66  r....r......conf
-00000780: 6967 7572 655f 6f70 7469 6d69 7a65 7273  igure_optimizers
-00000790: 4600 0000 7304 0000 0000 010a 017a 2450  F...s........z$P
-000007a0: 6174 6368 436c 6173 7369 6669 6572 2e63  atchClassifier.c
-000007b0: 6f6e 6669 6775 7265 5f6f 7074 696d 697a  onfigure_optimiz
-000007c0: 6572 7363 0300 0000 0000 0000 0000 0000  ersc............
-000007d0: 0600 0000 0500 0000 4300 0000 7334 0000  ........C...s4..
-000007e0: 007c 015c 027d 037d 0474 006a 017c 047c  .|.\.}.}.t.j.|.|
-000007f0: 006a 0264 018d 02a0 03a1 007d 047c 00a0  .j.d.......}.|..
-00000800: 047c 03a1 017d 057c 00a0 057c 027c 057c  .|...}.|...|.|.|
-00000810: 04a1 0353 0029 024e 2901 da0b 6e75 6d5f  ...S.).N)...num_
-00000820: 636c 6173 7365 7329 0672 0300 0000 da07  classes).r......
-00000830: 6f6e 655f 686f 7472 0c00 0000 da05 666c  one_hotr......fl
-00000840: 6f61 7472 0b00 0000 da0b 6c6f 675f 6d65  oatr......log_me
-00000850: 7472 6963 7329 0672 1300 0000 da05 6261  trics).r......ba
-00000860: 7463 68da 046d 6f64 6572 3500 0000 da06  tch..moder5.....
-00000870: 7461 7267 6574 720b 0000 0072 1900 0000  targetr....r....
-00000880: 7219 0000 0072 1a00 0000 da16 6578 6563  r....r......exec
-00000890: 7574 655f 616e 645f 6765 745f 6d65 7472  ute_and_get_metr
-000008a0: 6963 4a00 0000 7308 0000 0000 0108 0114  icJ...s.........
-000008b0: 010a 017a 2650 6174 6368 436c 6173 7369  ...z&PatchClassi
-000008c0: 6669 6572 2e65 7865 6375 7465 5f61 6e64  fier.execute_and
-000008d0: 5f67 6574 5f6d 6574 7269 6363 0300 0000  _get_metricc....
-000008e0: 0000 0000 0000 0000 0400 0000 0600 0000  ................
-000008f0: 4300 0000 7326 0000 007c 00a0 007c 0164  C...s&...|...|.d
-00000900: 01a1 027d 037c 006a 017c 0364 0264 0364  ...}.|.j.|.d.d.d
-00000910: 0264 048d 0401 007c 0364 0519 0053 0029  .d.....|.d...S.)
-00000920: 064e da05 7472 6169 6e46 54a9 03da 076f  .N..trainFT....o
-00000930: 6e5f 7374 6570 da08 6f6e 5f65 706f 6368  n_step..on_epoch
-00000940: da08 7072 6f67 5f62 6172 da09 7472 6169  ..prog_bar..trai
-00000950: 6e5f 6263 65a9 0272 4200 0000 da08 6c6f  n_bce..rB.....lo
-00000960: 675f 6469 6374 2904 7213 0000 00da 0b74  g_dict).r......t
-00000970: 7261 696e 5f62 6174 6368 da09 6261 7463  rain_batch..batc
-00000980: 685f 6964 78da 0b6d 6574 7269 635f 6469  h_idx..metric_di
-00000990: 6374 7219 0000 0072 1900 0000 721a 0000  ctr....r....r...
-000009a0: 00da 0d74 7261 696e 696e 675f 7374 6570  ...training_step
-000009b0: 5000 0000 7306 0000 0000 010c 0112 017a  P...s..........z
-000009c0: 1d50 6174 6368 436c 6173 7369 6669 6572  .PatchClassifier
-000009d0: 2e74 7261 696e 696e 675f 7374 6570 6303  .training_stepc.
-000009e0: 0000 0000 0000 0000 0000 0004 0000 0006  ................
-000009f0: 0000 0043 0000 0073 2200 0000 7c00 a000  ...C...s"...|...
-00000a00: 7c01 6401 a102 7d03 7c00 6a01 7c03 6402  |.d...}.|.j.|.d.
-00000a10: 6403 6403 6404 8d04 0100 6400 5300 2905  d.d.d.....d.S.).
-00000a20: 4eda 0376 616c 4654 7244 0000 0072 4900  N..valFTrD...rI.
-00000a30: 0000 2904 7213 0000 00da 0976 616c 5f62  ..).r......val_b
-00000a40: 6174 6368 724c 0000 0072 4d00 0000 7219  atchrL...rM...r.
-00000a50: 0000 0072 1900 0000 721a 0000 00da 0f76  ...r....r......v
-00000a60: 616c 6964 6174 696f 6e5f 7374 6570 5500  alidation_stepU.
-00000a70: 0000 7304 0000 0000 010c 017a 1f50 6174  ..s........z.Pat
-00000a80: 6368 436c 6173 7369 6669 6572 2e76 616c  chClassifier.val
-00000a90: 6964 6174 696f 6e5f 7374 6570 6303 0000  idation_stepc...
-00000aa0: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00000ab0: 0043 0000 0073 1e00 0000 7c00 a000 7c01  .C...s....|...|.
-00000ac0: 6401 a102 7d03 7c00 6a01 7c03 6402 6403  d...}.|.j.|.d.d.
-00000ad0: 8d02 0100 6400 5300 2904 4eda 0474 6573  ....d.S.).N..tes
-00000ae0: 7454 2901 7247 0000 0072 4900 0000 2904  tT).rG...rI...).
-00000af0: 7213 0000 00da 0a74 6573 745f 6261 7463  r......test_batc
-00000b00: 6872 4c00 0000 724d 0000 0072 1900 0000  hrL...rM...r....
-00000b10: 7219 0000 0072 1a00 0000 da09 7465 7374  r....r......test
-00000b20: 5f73 7465 7059 0000 0073 0400 0000 0001  _stepY...s......
-00000b30: 0c01 7a19 5061 7463 6843 6c61 7373 6966  ..z.PatchClassif
-00000b40: 6965 722e 7465 7374 5f73 7465 7063 0300  ier.test_stepc..
-00000b50: 0000 0000 0000 0000 0000 0c00 0000 0e00  ................
-00000b60: 0000 4300 0000 73f0 0000 007c 016a 0064  ..C...s....|.j.d
-00000b70: 0119 0064 016b 0272 3064 017c 0164 0064  ...d.k.r0d.|.d.d
-00000b80: 0085 0264 0266 0219 0018 007d 0374 01a0  ...d.f.....}.t..
-00000b90: 027c 017c 0366 02a1 017d 0174 03a0 047c  .|.|.f...}.t...|
-00000ba0: 017c 02a1 027d 0474 016a 057c 0164 0164  .|...}.t.j.|.d.d
-00000bb0: 038d 02a0 06a1 007d 0174 016a 057c 0264  .......}.t.j.|.d
-00000bc0: 0164 038d 02a0 06a1 007d 0274 07a0 087c  .d.......}.t...|
-00000bd0: 017c 02a1 027d 0574 07a0 097c 017c 02a1  .|...}.t...|.|..
-00000be0: 02a0 06a1 007d 0674 07a0 0a7c 017c 02a0  .....}.t...|.|..
-00000bf0: 0ba1 00a1 027d 0774 07a0 0c7c 017c 02a1  .....}.t...|.|..
-00000c00: 027d 0874 07a0 0d7c 017c 02a1 027d 0974  .}.t...|.|...}.t
-00000c10: 07a0 0e7c 017c 02a1 027d 0a7c 0064 0417  ...|.|...}.|.d..
-00000c20: 007c 047c 0064 0517 007c 097c 0064 0617  .|.|.d...|.|.d..
-00000c30: 007c 0a7c 0064 0717 007c 067c 0064 0817  .|.|.d...|.|.d..
-00000c40: 007c 077c 0064 0917 007c 087c 0064 0a17  .|.|.d...|.|.d..
-00000c50: 007c 0569 077d 0b7c 0b53 0029 0b4e 721b  .|.i.}.|.S.).Nr.
-00000c60: 0000 0072 0100 0000 7221 0000 00da 045f  ...r....r!....._
-00000c70: 6263 65da 0a5f 7072 6563 6973 696f 6eda  bce.._precision.
-00000c80: 075f 7265 6361 6c6c da04 5f62 6d63 da06  ._recall.._bmc..
-00000c90: 5f61 7572 6f63 da03 5f66 31da 045f 6163  _auroc.._f1.._ac
-00000ca0: 6329 0fda 0573 6861 7065 7226 0000 00da  c)...shaper&....
-00000cb0: 0c63 6f6c 756d 6e5f 7374 6163 6b72 0300  .column_stackr..
-00000cc0: 0000 da20 6269 6e61 7279 5f63 726f 7373  ... binary_cross
-00000cd0: 5f65 6e74 726f 7079 5f77 6974 685f 6c6f  _entropy_with_lo
-00000ce0: 6769 7473 da06 6172 676d 6178 723d 0000  gits..argmaxr=..
-00000cf0: 00da 0d74 665f 636c 6173 7369 6669 6572  ...tf_classifier
-00000d00: da0f 6269 6e61 7279 5f61 6363 7572 6163  ..binary_accurac
-00000d10: 79da 1862 696e 6172 795f 6d61 7474 6865  y..binary_matthe
-00000d20: 7773 5f63 6f72 7263 6f65 66da 0c62 696e  ws_corrcoef..bin
-00000d30: 6172 795f 6175 726f 63da 046c 6f6e 67da  ary_auroc..long.
-00000d40: 0f62 696e 6172 795f 6631 5f73 636f 7265  .binary_f1_score
-00000d50: da10 6269 6e61 7279 5f70 7265 6369 7369  ..binary_precisi
-00000d60: 6f6e da0d 6269 6e61 7279 5f72 6563 616c  on..binary_recal
-00000d70: 6c29 0c72 4000 0000 da05 7072 6564 7372  l).r@.....predsr
-00000d80: 4100 0000 da07 6e65 775f 636f 6cda 0362  A.....new_col..b
-00000d90: 6365 da08 7465 7374 5f61 6363 da03 626d  ce..test_acc..bm
-00000da0: 63da 0561 7572 6f63 da02 6631 da09 7072  c..auroc..f1..pr
-00000db0: 6563 6973 696f 6eda 0672 6563 616c 6c72  ecision..recallr
-00000dc0: 4d00 0000 7219 0000 0072 1900 0000 721a  M...r....r....r.
-00000dd0: 0000 0072 3e00 0000 5d00 0000 732a 0000  ...r>...]...s*..
-00000de0: 0000 030e 0214 020e 010c 0212 0112 010c  ................
-00000df0: 0110 0110 010c 010c 010c 0208 0108 0108  ................
-00000e00: 0108 0108 0108 0108 f904 097a 1b50 6174  ...........z.Pat
-00000e10: 6368 436c 6173 7369 6669 6572 2e6c 6f67  chClassifier.log
-00000e20: 5f6d 6574 7269 6373 2904 7205 0000 0072  _metrics).r....r
-00000e30: 0600 0000 7207 0000 004e 290e da08 5f5f  ....r....N)...__
-00000e40: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000e50: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000e60: 720a 0000 0072 1200 0000 7236 0000 0072  r....r....r6...r
-00000e70: 3a00 0000 7242 0000 0072 4e00 0000 7251  :...rB...rN...rQ
-00000e80: 0000 0072 5400 0000 da0c 7374 6174 6963  ...rT.....static
-00000e90: 6d65 7468 6f64 723e 0000 00da 0d5f 5f63  methodr>.....__c
-00000ea0: 6c61 7373 6365 6c6c 5f5f 7219 0000 0072  lasscell__r....r
-00000eb0: 1900 0000 7217 0000 0072 1a00 0000 7204  ....r....r....r.
-00000ec0: 0000 0008 0000 0073 1c00 0000 0805 0001  .......s........
-00000ed0: 0001 0001 00f9 0e18 0821 0804 0804 0806  .........!......
-00000ee0: 0805 0804 0804 0201 7204 0000 0054 2902  ........r....T).
-00000ef0: da0a 6d6f 6465 6c5f 7061 7468 7234 0000  ..model_pathr4..
-00000f00: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
-00000f10: 0000 0300 0000 4300 0000 7326 0000 0064  ......C...s&...d
-00000f20: 0164 026c 006d 017d 0201 007c 02a0 027c  .d.l.m.}...|...|
-00000f30: 00a1 017d 037c 0172 227c 03a0 03a1 0001  ...}.|.r"|......
-00000f40: 007c 0353 0029 037a 990a 2020 2020 4c6f  .|.S.).z..    Lo
-00000f50: 6164 2074 6865 2074 7261 696e 6564 206d  ad the trained m
-00000f60: 6f64 656c 2e0a 0a20 2020 2041 7267 733a  odel...    Args:
-00000f70: 0a20 2020 2020 2020 206d 6f64 656c 5f70  .        model_p
-00000f80: 6174 6820 2873 7472 293a 2050 6174 6820  ath (str): Path 
-00000f90: 746f 2074 6865 206d 6f64 656c 2063 6865  to the model che
-00000fa0: 636b 706f 696e 742e 0a0a 2020 2020 5265  ckpoint...    Re
-00000fb0: 7475 726e 733a 0a20 2020 2020 2020 2074  turns:.        t
-00000fc0: 6f72 6368 2e6e 6e2e 4d6f 6475 6c65 3a20  orch.nn.Module: 
-00000fd0: 4c6f 6164 6564 206d 6f64 656c 2e0a 2020  Loaded model..  
-00000fe0: 2020 7206 0000 0029 0172 0400 0000 2904    r....).r....).
-00000ff0: da0e 636c 6173 7369 6669 6361 7469 6f6e  ..classification
-00001000: 7204 0000 00da 146c 6f61 645f 6672 6f6d  r......load_from
-00001010: 5f63 6865 636b 706f 696e 7472 3400 0000  _checkpointr4...
-00001020: 2904 7276 0000 0072 3400 0000 7204 0000  ).rv...r4...r...
-00001030: 00da 056d 6f64 656c 7219 0000 0072 1900  ...modelr....r..
-00001040: 0000 721a 0000 00da 0a6c 6f61 645f 6d6f  ..r......load_mo
-00001050: 6465 6c7b 0000 0073 0e00 0000 000a 0c02  del{...s........
-00001060: 0401 02ff 0407 0401 0801 727a 0000 0063  ..........rz...c
-00001070: 0200 0000 0000 0000 0000 0000 0900 0000  ................
-00001080: 0600 0000 4300 0000 73a6 0000 0074 006a  ....C...s....t.j
-00001090: 0164 0164 028d 017d 0267 007d 0367 007d  .d.d...}.g.}.g.}
-000010a0: 0474 027c 0183 0144 005d 645c 027d 057d  .t.|...D.]d\.}.}
-000010b0: 067c 007c 0583 017d 077c 076a 0364 0119  .|.|...}.|.j.d..
-000010c0: 0064 016b 0272 5c64 017c 0764 0064 0085  .d.k.r\d.|.d.d..
-000010d0: 0264 0366 0219 0018 007d 0874 04a0 057c  .d.f.....}.t...|
-000010e0: 077c 0866 02a1 017d 077c 03a0 067c 027c  .|.f...}.|...|.|
-000010f0: 0783 0164 0064 0085 0264 0166 0219 00a1  ...d.d...d.f....
-00001100: 0101 007c 04a0 067c 06a1 0101 0071 1c74  ...|...|.....q.t
-00001110: 046a 077c 0364 0364 028d 027d 0374 046a  .j.|.d.d...}.t.j
-00001120: 077c 0464 0364 028d 027d 047c 037c 0466  .|.d.d...}.|.|.f
-00001130: 0253 0029 044e 721b 0000 0072 2100 0000  .S.).Nr....r!...
-00001140: 7201 0000 0029 0872 0200 0000 722d 0000  r....).r....r-..
-00001150: 00da 0469 7465 7272 5c00 0000 7226 0000  ...iterr\...r&..
-00001160: 0072 5d00 0000 da06 6170 7065 6e64 da03  .r].....append..
-00001170: 6361 7429 0972 7900 0000 da0b 6461 7461  cat).ry.....data
-00001180: 5f6c 6f61 6465 72da 016d 7268 0000 00da  _loader..mrh....
-00001190: 066c 6162 656c 7372 3500 0000 da01 79da  .labelsr5.....y.
-000011a0: 0470 7265 6472 6900 0000 7219 0000 0072  .predri...r....r
-000011b0: 1900 0000 721a 0000 00da 0e67 6574 5f70  ....r......get_p
-000011c0: 7265 6469 6374 696f 6e93 0000 0073 1a00  rediction....s..
-000011d0: 0000 0001 0c01 0401 0401 1001 0801 0e02  ................
-000011e0: 1402 0e01 1a01 0c01 0e01 0e01 7283 0000  ............r...
-000011f0: 0029 0154 290f da09 6c69 6768 746e 696e  .).T)...lightnin
-00001200: 67da 056c 6967 6874 7226 0000 00da 2674  g..lightr&....&t
-00001210: 6f72 6368 6d65 7472 6963 732e 6675 6e63  orchmetrics.func
-00001220: 7469 6f6e 616c 2e63 6c61 7373 6966 6963  tional.classific
-00001230: 6174 696f 6e72 0300 0000 7277 0000 0072  ationr....rw...r
-00001240: 6000 0000 7202 0000 00da 0874 6f72 6368  `...r......torch
-00001250: 2e6e 6eda 0f4c 6967 6874 6e69 6e67 4d6f  .nn..LightningMo
-00001260: 6475 6c65 7204 0000 00da 0373 7472 da04  duler......str..
-00001270: 626f 6f6c 727a 0000 0072 8300 0000 7219  boolrz...r....r.
-00001280: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00001290: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000012a0: 730e 0000 0008 0108 0112 010c 010c 0312  s...............
-000012b0: 7312 18                                  s..
+00000370: 6405 8d06 7d03 7401 6a04 a005 a100 7d04  d...}.t.j.....}.
+00000380: 7c04 a006 6406 7404 a007 a100 a102 0100  |...d.t.........
+00000390: 7c04 a006 6407 7404 a008 7c02 6408 1900  |...d.t...|.d...
+000003a0: 7c02 6403 1900 1400 7c00 6a09 a102 a102  |.d.....|.j.....
+000003b0: 0100 7c04 a006 6409 7404 6a0a 6403 640a  ..|...d.t.j.d.d.
+000003c0: 8d01 a102 0100 7404 6a05 7c03 7c04 6702  ......t.j.|.|.g.
+000003d0: 8e00 7c00 5f0b 6e82 7c00 6a00 640b 6b02  ..|._.n.|.j.d.k.
+000003e0: 72d0 7404 a005 7404 a008 7c01 640c a102  r.t...t...|.d...
+000003f0: 7404 a00c a100 7404 a008 640c 640d a102  t.....t...d.d...
+00000400: 7404 a00c a100 7404 a008 640d 7c00 6a09  t.....t...d.|.j.
+00000410: a102 7404 6a0a 6403 640a 8d01 a106 7c00  ..t.j.d.d.....|.
+00000420: 5f0b 6e36 7c00 6a00 640e 6b02 72f6 7404  _.n6|.j.d.k.r.t.
+00000430: a005 7404 a008 7c01 6403 a102 7404 a00d  ..t...|.d...t...
+00000440: a100 a102 7c00 5f0b 6e10 740e 640f 7c00  ....|._.n.t.d.|.
+00000450: 6a0f 9b00 9d02 8301 8201 6410 5300 2911  j.........d.S.).
+00000460: 7a43 0a20 2020 2020 2020 2053 656c 6563  zC.        Selec
+00000470: 7473 2061 6e64 2062 7569 6c64 7320 7468  ts and builds th
+00000480: 6520 6368 6f73 656e 206d 6f64 656c 2061  e chosen model a
+00000490: 7263 6869 7465 6374 7572 652e 0a20 2020  rchitecture..   
+000004a0: 2020 2020 2072 0500 0000 7a26 6d61 7465       r....z&mate
+000004b0: 7573 7a62 7564 612f 6272 6169 6e2d 7365  uszbuda/brain-se
+000004c0: 676d 656e 7461 7469 6f6e 2d70 7974 6f72  gmentation-pytor
+000004d0: 6368 e901 0000 0046 2904 7214 0000 00da  ch.....F).r.....
+000004e0: 0c6f 7574 5f63 6861 6e6e 656c 73da 0d69  .out_channels..i
+000004f0: 6e69 745f 6665 6174 7572 6573 da07 7665  nit_features..ve
+00000500: 7262 6f73 65da 0766 6c61 7474 656e da02  rbose..flatten..
+00000510: 6663 7201 0000 00da 0361 6374 a901 da03  fcr......act....
+00000520: 6469 6dda 036d 6c70 e91e 0000 00e9 0a00  dim..mlp........
+00000530: 0000 7208 0000 007a 1c49 6e76 616c 6964  ..r....z.Invalid
+00000540: 206d 6f64 656c 2061 7263 6869 7465 6374   model architect
+00000550: 7572 653a 204e 2910 7210 0000 00da 0574  ure: N).r......t
+00000560: 6f72 6368 da03 6875 62da 046c 6f61 6472  orch..hub..loadr
+00000570: 0200 0000 da0a 5365 7175 656e 7469 616c  ......Sequential
+00000580: da0a 6164 645f 6d6f 6475 6c65 da07 466c  ..add_module..Fl
+00000590: 6174 7465 6eda 064c 696e 6561 7272 0c00  atten..Linearr..
+000005a0: 0000 da07 536f 6674 6d61 7872 0b00 0000  ....Softmaxr....
+000005b0: da04 5265 4c55 da07 5369 676d 6f69 64da  ..ReLU..Sigmoid.
+000005c0: 0a56 616c 7565 4572 726f 72da 0a6d 6f64  .ValueError..mod
+000005d0: 656c 5f61 7263 6829 0572 1300 0000 7214  el_arch).r....r.
+000005e0: 0000 0072 1500 0000 da08 6261 636b 626f  ...r......backbo
+000005f0: 6e65 da0a 636c 6173 7369 6669 6572 7218  ne..classifierr.
+00000600: 0000 0072 1800 0000 7219 0000 0072 1200  ...r....r....r..
+00000610: 0000 2100 0000 7338 0000 0000 040a 0106  ..!...s8........
+00000620: 0102 0102 0102 0102 0102 0102 fa06 080a  ................
+00000630: 0110 0104 011a ff04 0314 0112 010a 0104  ................
+00000640: 010a 0106 010a 0106 010c 010a fa08 080a  ................
+00000650: 011c 027a 1b50 6174 6368 436c 6173 7369  ...z.PatchClassi
+00000660: 6669 6572 2e62 7569 6c64 5f6d 6f64 656c  fier.build_model
+00000670: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000680: 0003 0000 0043 0000 0073 1400 0000 7c00  .....C...s....|.
+00000690: 6a00 a001 a100 0100 7c00 a000 7c01 a101  j.......|...|...
+000006a0: 5300 2901 4e29 0272 0b00 0000 da04 6576  S.).N).r......ev
+000006b0: 616c 2902 7213 0000 00da 0178 7218 0000  al).r......xr...
+000006c0: 0072 1800 0000 7219 0000 00da 0766 6f72  .r....r......for
+000006d0: 7761 7264 4300 0000 7304 0000 0000 010a  wardC...s.......
+000006e0: 017a 1750 6174 6368 436c 6173 7369 6669  .z.PatchClassifi
+000006f0: 6572 2e66 6f72 7761 7264 6301 0000 0000  er.forwardc.....
+00000700: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
+00000710: 0000 0073 2800 0000 7c00 6a00 6401 6b02  ...s(...|.j.d.k.
+00000720: 7224 7401 6a02 6a03 7c00 a004 a100 6601  r$t.j.j.|.....f.
+00000730: 6900 7c00 6a05 a401 8e01 5300 6400 5300  i.|.j.....S.d.S.
+00000740: 2902 4e72 0700 0000 2906 720d 0000 0072  ).Nr....).r....r
+00000750: 2600 0000 da05 6f70 7469 6dda 0441 6461  &.....optim..Ada
+00000760: 6dda 0a70 6172 616d 6574 6572 7372 0e00  m..parametersr..
+00000770: 0000 2901 7213 0000 0072 1800 0000 7218  ..).r....r....r.
+00000780: 0000 0072 1900 0000 da14 636f 6e66 6967  ...r......config
+00000790: 7572 655f 6f70 7469 6d69 7a65 7273 4700  ure_optimizersG.
+000007a0: 0000 7304 0000 0000 010a 017a 2450 6174  ..s........z$Pat
+000007b0: 6368 436c 6173 7369 6669 6572 2e63 6f6e  chClassifier.con
+000007c0: 6669 6775 7265 5f6f 7074 696d 697a 6572  figure_optimizer
+000007d0: 7363 0300 0000 0000 0000 0000 0000 0600  sc..............
+000007e0: 0000 0500 0000 4300 0000 7334 0000 007c  ......C...s4...|
+000007f0: 015c 027d 037d 0474 006a 017c 047c 006a  .\.}.}.t.j.|.|.j
+00000800: 0264 018d 02a0 03a1 007d 047c 00a0 047c  .d.......}.|...|
+00000810: 03a1 017d 057c 00a0 057c 027c 057c 04a1  ...}.|...|.|.|..
+00000820: 0353 0029 024e 2901 da0b 6e75 6d5f 636c  .S.).N)...num_cl
+00000830: 6173 7365 7329 0672 0300 0000 da07 6f6e  asses).r......on
+00000840: 655f 686f 7472 0c00 0000 da05 666c 6f61  e_hotr......floa
+00000850: 7472 0b00 0000 da0b 6c6f 675f 6d65 7472  tr......log_metr
+00000860: 6963 7329 0672 1300 0000 da05 6261 7463  ics).r......batc
+00000870: 68da 046d 6f64 6572 3500 0000 da06 7461  h..moder5.....ta
+00000880: 7267 6574 720b 0000 0072 1800 0000 7218  rgetr....r....r.
+00000890: 0000 0072 1900 0000 da16 6578 6563 7574  ...r......execut
+000008a0: 655f 616e 645f 6765 745f 6d65 7472 6963  e_and_get_metric
+000008b0: 4b00 0000 7308 0000 0000 0108 0114 010a  K...s...........
+000008c0: 017a 2650 6174 6368 436c 6173 7369 6669  .z&PatchClassifi
+000008d0: 6572 2e65 7865 6375 7465 5f61 6e64 5f67  er.execute_and_g
+000008e0: 6574 5f6d 6574 7269 6363 0300 0000 0000  et_metricc......
+000008f0: 0000 0000 0000 0400 0000 0600 0000 4300  ..............C.
+00000900: 0000 7326 0000 007c 00a0 007c 0164 01a1  ..s&...|...|.d..
+00000910: 027d 037c 006a 017c 0364 0264 0364 0264  .}.|.j.|.d.d.d.d
+00000920: 048d 0401 007c 0364 0519 0053 0029 064e  .....|.d...S.).N
+00000930: da05 7472 6169 6e46 54a9 03da 076f 6e5f  ..trainFT....on_
+00000940: 7374 6570 da08 6f6e 5f65 706f 6368 da08  step..on_epoch..
+00000950: 7072 6f67 5f62 6172 5a09 7472 6169 6e5f  prog_barZ.train_
+00000960: 6263 65a9 0272 4200 0000 da08 6c6f 675f  bce..rB.....log_
+00000970: 6469 6374 2904 7213 0000 005a 0b74 7261  dict).r....Z.tra
+00000980: 696e 5f62 6174 6368 da09 6261 7463 685f  in_batch..batch_
+00000990: 6964 78da 0b6d 6574 7269 635f 6469 6374  idx..metric_dict
+000009a0: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
+000009b0: 0d74 7261 696e 696e 675f 7374 6570 5100  .training_stepQ.
+000009c0: 0000 7306 0000 0000 010c 0112 017a 1d50  ..s..........z.P
+000009d0: 6174 6368 436c 6173 7369 6669 6572 2e74  atchClassifier.t
+000009e0: 7261 696e 696e 675f 7374 6570 6303 0000  raining_stepc...
+000009f0: 0000 0000 0000 0000 0004 0000 0006 0000  ................
+00000a00: 0043 0000 0073 2200 0000 7c00 a000 7c01  .C...s"...|...|.
+00000a10: 6401 a102 7d03 7c00 6a01 7c03 6402 6403  d...}.|.j.|.d.d.
+00000a20: 6403 6404 8d04 0100 6400 5300 2905 4eda  d.d.....d.S.).N.
+00000a30: 0376 616c 4654 7244 0000 0072 4800 0000  .valFTrD...rH...
+00000a40: 2904 7213 0000 005a 0976 616c 5f62 6174  ).r....Z.val_bat
+00000a50: 6368 724a 0000 0072 4b00 0000 7218 0000  chrJ...rK...r...
+00000a60: 0072 1800 0000 7219 0000 00da 0f76 616c  .r....r......val
+00000a70: 6964 6174 696f 6e5f 7374 6570 5600 0000  idation_stepV...
+00000a80: 7304 0000 0000 010c 017a 1f50 6174 6368  s........z.Patch
+00000a90: 436c 6173 7369 6669 6572 2e76 616c 6964  Classifier.valid
+00000aa0: 6174 696f 6e5f 7374 6570 6303 0000 0000  ation_stepc.....
+00000ab0: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
+00000ac0: 0000 0073 1e00 0000 7c00 a000 7c01 6401  ...s....|...|.d.
+00000ad0: a102 7d03 7c00 6a01 7c03 6402 6403 8d02  ..}.|.j.|.d.d...
+00000ae0: 0100 6400 5300 2904 4eda 0474 6573 7454  ..d.S.).N..testT
+00000af0: 2901 7247 0000 0072 4800 0000 2904 7213  ).rG...rH...).r.
+00000b00: 0000 00da 0a74 6573 745f 6261 7463 6872  .....test_batchr
+00000b10: 4a00 0000 724b 0000 0072 1800 0000 7218  J...rK...r....r.
+00000b20: 0000 0072 1900 0000 da09 7465 7374 5f73  ...r......test_s
+00000b30: 7465 705a 0000 0073 0400 0000 0001 0c01  tepZ...s........
+00000b40: 7a19 5061 7463 6843 6c61 7373 6966 6965  z.PatchClassifie
+00000b50: 722e 7465 7374 5f73 7465 7063 0300 0000  r.test_stepc....
+00000b60: 0000 0000 0000 0000 0c00 0000 0e00 0000  ................
+00000b70: 4300 0000 73f0 0000 007c 016a 0064 0119  C...s....|.j.d..
+00000b80: 0064 016b 0272 3064 017c 0164 0064 0085  .d.k.r0d.|.d.d..
+00000b90: 0264 0266 0219 0018 007d 0374 01a0 027c  .d.f.....}.t...|
+00000ba0: 017c 0366 02a1 017d 0174 03a0 047c 017c  .|.f...}.t...|.|
+00000bb0: 02a1 027d 0474 016a 057c 0164 0164 038d  ...}.t.j.|.d.d..
+00000bc0: 02a0 06a1 007d 0174 016a 057c 0264 0164  .....}.t.j.|.d.d
+00000bd0: 038d 02a0 06a1 007d 0274 07a0 087c 017c  .......}.t...|.|
+00000be0: 02a1 027d 0574 07a0 097c 017c 02a1 02a0  ...}.t...|.|....
+00000bf0: 06a1 007d 0674 07a0 0a7c 017c 02a0 0ba1  ...}.t...|.|....
+00000c00: 00a1 027d 0774 07a0 0c7c 017c 02a1 027d  ...}.t...|.|...}
+00000c10: 0874 07a0 0d7c 017c 02a1 027d 0974 07a0  .t...|.|...}.t..
+00000c20: 0e7c 017c 02a1 027d 0a7c 0064 0417 007c  .|.|...}.|.d...|
+00000c30: 047c 0064 0517 007c 097c 0064 0617 007c  .|.d...|.|.d...|
+00000c40: 0a7c 0064 0717 007c 067c 0064 0817 007c  .|.d...|.|.d...|
+00000c50: 077c 0064 0917 007c 087c 0064 0a17 007c  .|.d...|.|.d...|
+00000c60: 0569 077d 0b7c 0b53 0029 0b4e 721a 0000  .i.}.|.S.).Nr...
+00000c70: 0072 0100 0000 7221 0000 005a 045f 6263  .r....r!...Z._bc
+00000c80: 65da 0a5f 7072 6563 6973 696f 6e5a 075f  e.._precisionZ._
+00000c90: 7265 6361 6c6c 5a04 5f62 6d63 5a06 5f61  recallZ._bmcZ._a
+00000ca0: 7572 6f63 5a03 5f66 315a 045f 6163 6329  urocZ._f1Z._acc)
+00000cb0: 0fda 0573 6861 7065 7226 0000 00da 0c63  ...shaper&.....c
+00000cc0: 6f6c 756d 6e5f 7374 6163 6b72 0300 0000  olumn_stackr....
+00000cd0: da20 6269 6e61 7279 5f63 726f 7373 5f65  . binary_cross_e
+00000ce0: 6e74 726f 7079 5f77 6974 685f 6c6f 6769  ntropy_with_logi
+00000cf0: 7473 da06 6172 676d 6178 723d 0000 00da  ts..argmaxr=....
+00000d00: 0d74 665f 636c 6173 7369 6669 6572 da0f  .tf_classifier..
+00000d10: 6269 6e61 7279 5f61 6363 7572 6163 79da  binary_accuracy.
+00000d20: 1862 696e 6172 795f 6d61 7474 6865 7773  .binary_matthews
+00000d30: 5f63 6f72 7263 6f65 66da 0c62 696e 6172  _corrcoef..binar
+00000d40: 795f 6175 726f 63da 046c 6f6e 67da 0f62  y_auroc..long..b
+00000d50: 696e 6172 795f 6631 5f73 636f 7265 da10  inary_f1_score..
+00000d60: 6269 6e61 7279 5f70 7265 6369 7369 6f6e  binary_precision
+00000d70: da0d 6269 6e61 7279 5f72 6563 616c 6c29  ..binary_recall)
+00000d80: 0c72 4000 0000 da05 7072 6564 7372 4100  .r@.....predsrA.
+00000d90: 0000 da07 6e65 775f 636f 6c5a 0362 6365  ....new_colZ.bce
+00000da0: 5a08 7465 7374 5f61 6363 5a03 626d 63da  Z.test_accZ.bmc.
+00000db0: 0561 7572 6f63 da02 6631 da09 7072 6563  .auroc..f1..prec
+00000dc0: 6973 696f 6eda 0672 6563 616c 6c72 4b00  ision..recallrK.
+00000dd0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000de0: 0072 3e00 0000 5e00 0000 732a 0000 0000  .r>...^...s*....
+00000df0: 030e 0214 020e 010c 0212 0112 010c 0110  ................
+00000e00: 0110 010c 010c 010c 0208 0108 0108 0108  ................
+00000e10: 0108 0108 0108 f904 097a 1b50 6174 6368  .........z.Patch
+00000e20: 436c 6173 7369 6669 6572 2e6c 6f67 5f6d  Classifier.log_m
+00000e30: 6574 7269 6373 2904 7205 0000 0072 0600  etrics).r....r..
+00000e40: 0000 7207 0000 004e 290e da08 5f5f 6e61  ..r....N)...__na
+00000e50: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000e60: da0c 5f5f 7175 616c 6e61 6d65 5f5f 720a  ..__qualname__r.
+00000e70: 0000 0072 1200 0000 7236 0000 0072 3a00  ...r....r6...r:.
+00000e80: 0000 7242 0000 0072 4c00 0000 724e 0000  ..rB...rL...rN..
+00000e90: 0072 5100 0000 da0c 7374 6174 6963 6d65  .rQ.....staticme
+00000ea0: 7468 6f64 723e 0000 00da 0d5f 5f63 6c61  thodr>.....__cla
+00000eb0: 7373 6365 6c6c 5f5f 7218 0000 0072 1800  sscell__r....r..
+00000ec0: 0000 7216 0000 0072 1900 0000 7204 0000  ..r....r....r...
+00000ed0: 0008 0000 0073 1c00 0000 0805 0001 0001  .....s..........
+00000ee0: 0001 00f9 0e18 0822 0804 0804 0806 0805  ......."........
+00000ef0: 0804 0804 0201 7204 0000 0054 2902 da0a  ......r....T)...
+00000f00: 6d6f 6465 6c5f 7061 7468 7234 0000 0063  model_pathr4...c
+00000f10: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00000f20: 0300 0000 4300 0000 731a 0000 0074 00a0  ....C...s....t..
+00000f30: 017c 00a1 017d 027c 0172 167c 02a0 02a1  .|...}.|.r.|....
+00000f40: 0001 007c 0253 0029 017a 990a 2020 2020  ...|.S.).z..    
+00000f50: 4c6f 6164 2074 6865 2074 7261 696e 6564  Load the trained
+00000f60: 206d 6f64 656c 2e0a 0a20 2020 2041 7267   model...    Arg
+00000f70: 733a 0a20 2020 2020 2020 206d 6f64 656c  s:.        model
+00000f80: 5f70 6174 6820 2873 7472 293a 2050 6174  _path (str): Pat
+00000f90: 6820 746f 2074 6865 206d 6f64 656c 2063  h to the model c
+00000fa0: 6865 636b 706f 696e 742e 0a0a 2020 2020  heckpoint...    
+00000fb0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00000fc0: 2074 6f72 6368 2e6e 6e2e 4d6f 6475 6c65   torch.nn.Module
+00000fd0: 3a20 4c6f 6164 6564 206d 6f64 656c 2e0a  : Loaded model..
+00000fe0: 2020 2020 2903 7204 0000 00da 146c 6f61      ).r......loa
+00000ff0: 645f 6672 6f6d 5f63 6865 636b 706f 696e  d_from_checkpoin
+00001000: 7472 3400 0000 2903 726a 0000 0072 3400  tr4...).rj...r4.
+00001010: 0000 da05 6d6f 6465 6c72 1800 0000 7218  ....modelr....r.
+00001020: 0000 0072 1900 0000 da0a 6c6f 6164 5f6d  ...r......load_m
+00001030: 6f64 656c 7c00 0000 730c 0000 0000 0b04  odel|...s.......
+00001040: 0102 ff04 0704 0108 0172 6d00 0000 6302  .........rm...c.
+00001050: 0000 0000 0000 0000 0000 0009 0000 0006  ................
+00001060: 0000 0043 0000 0073 a600 0000 7400 6a01  ...C...s....t.j.
+00001070: 6401 6402 8d01 7d02 6700 7d03 6700 7d04  d.d...}.g.}.g.}.
+00001080: 7402 7c01 8301 4400 5d64 5c02 7d05 7d06  t.|...D.]d\.}.}.
+00001090: 7c00 7c05 8301 7d07 7c07 6a03 6401 1900  |.|...}.|.j.d...
+000010a0: 6401 6b02 725c 6401 7c07 6400 6400 8502  d.k.r\d.|.d.d...
+000010b0: 6403 6602 1900 1800 7d08 7404 a005 7c07  d.f.....}.t...|.
+000010c0: 7c08 6602 a101 7d07 7c03 a006 7c02 7c07  |.f...}.|...|.|.
+000010d0: 8301 6400 6400 8502 6401 6602 1900 a101  ..d.d...d.f.....
+000010e0: 0100 7c04 a006 7c06 a101 0100 711c 7404  ..|...|.....q.t.
+000010f0: 6a07 7c03 6403 6402 8d02 7d03 7404 6a07  j.|.d.d...}.t.j.
+00001100: 7c04 6403 6402 8d02 7d04 7c03 7c04 6602  |.d.d...}.|.|.f.
+00001110: 5300 2904 4e72 1a00 0000 7221 0000 0072  S.).Nr....r!...r
+00001120: 0100 0000 2908 7202 0000 0072 2d00 0000  ....).r....r-...
+00001130: da04 6974 6572 7253 0000 0072 2600 0000  ..iterrS...r&...
+00001140: 7254 0000 00da 0661 7070 656e 64da 0363  rT.....append..c
+00001150: 6174 2909 726c 0000 005a 0b64 6174 615f  at).rl...Z.data_
+00001160: 6c6f 6164 6572 da01 6d72 5f00 0000 da06  loader..mr_.....
+00001170: 6c61 6265 6c73 7235 0000 00da 0179 da04  labelsr5.....y..
+00001180: 7072 6564 7260 0000 0072 1800 0000 7218  predr`...r....r.
+00001190: 0000 0072 1900 0000 da0e 6765 745f 7072  ...r......get_pr
+000011a0: 6564 6963 7469 6f6e 9300 0000 731a 0000  ediction....s...
+000011b0: 0000 010c 0104 0104 0110 0108 010e 0214  ................
+000011c0: 020e 011a 010c 010e 010e 0172 7500 0000  ...........ru...
+000011d0: 2901 5429 0fda 096c 6967 6874 6e69 6e67  ).T)...lightning
+000011e0: da05 6c69 6768 7472 2600 0000 da26 746f  ..lightr&....&to
+000011f0: 7263 686d 6574 7269 6373 2e66 756e 6374  rchmetrics.funct
+00001200: 696f 6e61 6c2e 636c 6173 7369 6669 6361  ional.classifica
+00001210: 7469 6f6e 7203 0000 00da 0e63 6c61 7373  tionr......class
+00001220: 6966 6963 6174 696f 6e72 5700 0000 7202  ificationrW...r.
+00001230: 0000 00da 0874 6f72 6368 2e6e 6eda 0f4c  .....torch.nn..L
+00001240: 6967 6874 6e69 6e67 4d6f 6475 6c65 7204  ightningModuler.
+00001250: 0000 00da 0373 7472 da04 626f 6f6c 726d  .....str..boolrm
+00001260: 0000 0072 7500 0000 7218 0000 0072 1800  ...ru...r....r..
+00001270: 0000 7218 0000 0072 1900 0000 da08 3c6d  ..r....r......<m
+00001280: 6f64 756c 653e 0100 0000 730e 0000 0008  odule>....s.....
+00001290: 0108 0112 010c 010c 0312 7412 17         ..........t..
```

### Comparing `morpheus_spatial-0.4.0/src/morpheus/classification/__pycache__/train.cpython-39.pyc` & `morpheus_spatial-0.5.0/src/morpheus/classification/__pycache__/train.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Mar 24 20:40:40 2024 UTC, .py size: 2058 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 c88f 0066 0a08 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 2cb8 1166 0a08 0000  a.......,..f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6404 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6406 6c09 6d0a 5a0a 0100 6407  ..d.d.l.m.Z...d.
 00000070: 6408 6c0b 6d0c 5a0c 0100 6404 6409 6c0d  d.l.m.Z...d.d.l.
@@ -39,70 +39,70 @@
 00000260: 0053 0029 1a4e e964 0000 00da 0461 7574  .S.).N.d.....aut
 00000270: 6f46 2904 da0a 6d61 785f 6570 6f63 6873  oF)...max_epochs
 00000280: da0b 6163 6365 6c65 7261 746f 72da 0764  ..accelerator..d
 00000290: 6576 6963 6573 da06 6c6f 6767 6572 e980  evices..logger..
 000002a0: 0000 00e9 0400 0000 5429 03da 0a62 6174  ........T)...bat
 000002b0: 6368 5f73 697a 65da 0b6e 756d 5f77 6f72  ch_size..num_wor
 000002c0: 6b65 7273 da0a 7069 6e5f 6d65 6d6f 7279  kers..pin_memory
-000002d0: 2903 720e 0000 00da 0a6d 6f64 656c 5f61  ).r......model_a
+000002d0: 2903 720e 0000 005a 0a6d 6f64 656c 5f61  ).r....Z.model_a
 000002e0: 7263 68da 0670 6172 616d 7372 0900 0000  rch..paramsr....
-000002f0: da07 7661 6c5f 626d 63da 036d 6178 2905  ..val_bmc..max).
+000002f0: 5a07 7661 6c5f 626d 63da 036d 6178 2905  Z.val_bmc..max).
 00000300: da07 6d6f 6e69 746f 72da 046d 6f64 65da  ..monitor..mode.
 00000310: 0a73 6176 655f 746f 705f 6bda 1173 6176  .save_top_k..sav
 00000320: 655f 7765 6967 6874 735f 6f6e 6c79 da07  e_weights_only..
 00000330: 7665 7262 6f73 6572 0100 0000 e90f 0000  verboser........
-00000340: 0029 0572 1e00 0000 da09 6d69 6e5f 6465  .).r......min_de
-00000350: 6c74 61da 0870 6174 6965 6e63 6572 2200  lta..patiencer".
-00000360: 0000 721f 0000 00e9 0a00 0000 2901 da0c  ..r.........)...
+00000340: 0029 0572 1c00 0000 da09 6d69 6e5f 6465  .).r......min_de
+00000350: 6c74 61da 0870 6174 6965 6e63 6572 2000  lta..patiencer .
+00000360: 0000 721d 0000 00e9 0a00 0000 2901 da0c  ..r.........)...
 00000370: 7265 6672 6573 685f 7261 7465 2903 7213  refresh_rate).r.
 00000380: 0000 00da 0963 616c 6c62 6163 6b73 da10  .....callbacks..
 00000390: 6465 6661 756c 745f 726f 6f74 5f64 6972  default_root_dir
 000003a0: 7a14 5472 6169 6e69 6e67 206d 6f64 656c  z.Training model
 000003b0: 2077 6974 6820 7a0d 2061 7263 6869 7465   with z. archite
 000003c0: 6374 7572 6529 0372 0c00 0000 da11 7472  cture).r......tr
 000003d0: 6169 6e5f 6461 7461 6c6f 6164 6572 73da  ain_dataloaders.
 000003e0: 0f76 616c 5f64 6174 616c 6f61 6465 7273  .val_dataloaders
 000003f0: 7a0f 6d6f 6465 6c20 7361 7665 6420 746f  z.model saved to
 00000400: 20da 0462 6573 7429 02da 0963 6b70 745f   ..best)...ckpt_
 00000410: 7061 7468 da0b 6461 7461 6c6f 6164 6572  path..dataloader
 00000420: 7329 12da 026f 73da 0470 6174 68da 046a  s)...os..path..j
 00000430: 6f69 6eda 0872 6f6f 745f 6469 7272 0b00  oin..root_dirr..
 00000440: 0000 720c 0000 00da 0576 616c 7565 7208  ..r......valuer.
-00000450: 0000 00da 0973 706c 6974 5f64 6972 da04  .....split_dir..
+00000450: 0000 005a 0973 706c 6974 5f64 6972 da04  ...Z.split_dir..
 00000460: 6172 6368 7202 0000 0072 0400 0000 7203  archr....r....r.
 00000470: 0000 0072 0500 0000 da05 7072 696e 74da  ...r......print.
 00000480: 0366 6974 da09 6d6f 6465 6c5f 6469 72da  .fit..model_dir.
 00000490: 0474 6573 7429 0a72 0c00 0000 720d 0000  .test).r....r...
-000004a0: 0072 0e00 0000 da0e 7361 7665 5f6d 6f64  .r......save_mod
-000004b0: 656c 5f64 6972 da11 6461 7461 6c6f 6164  el_dir..dataload
-000004c0: 6572 5f70 6172 616d 73da 0e74 7261 696e  er_params..train
-000004d0: 6572 5f70 6172 616d 73da 0c74 7261 696e  er_params..train
-000004e0: 5f6c 6f61 6465 72da 0a76 616c 5f6c 6f61  _loader..val_loa
-000004f0: 6465 72da 0b74 6573 745f 6c6f 6164 6572  der..test_loader
-00000500: da07 7472 6169 6e65 72a9 0072 4100 0000  ..trainer..rA...
+000004a0: 0072 0e00 0000 5a0e 7361 7665 5f6d 6f64  .r....Z.save_mod
+000004b0: 656c 5f64 6972 5a11 6461 7461 6c6f 6164  el_dirZ.dataload
+000004c0: 6572 5f70 6172 616d 735a 0e74 7261 696e  er_paramsZ.train
+000004d0: 6572 5f70 6172 616d 735a 0c74 7261 696e  er_paramsZ.train
+000004e0: 5f6c 6f61 6465 725a 0a76 616c 5f6c 6f61  _loaderZ.val_loa
+000004f0: 6465 725a 0b74 6573 745f 6c6f 6164 6572  derZ.test_loader
+00000500: da07 7472 6169 6e65 72a9 0072 3800 0000  ..trainer..r8...
 00000510: fa53 2f63 656e 7472 616c 2f68 6f6d 652f  .S/central/home/
 00000520: 7a77 616e 6732 2f6d 6f72 7068 6575 732d  zwang2/morpheus-
 00000530: 7370 6174 6961 6c2f 6d6f 7270 6865 7573  spatial/morpheus
 00000540: 2f73 7263 2f6d 6f72 7068 6575 732f 636c  /src/morpheus/cl
 00000550: 6173 7369 6669 6361 7469 6f6e 2f74 7261  assification/tra
 00000560: 696e 2e70 79da 0574 7261 696e 0c00 0000  in.py..train....
 00000570: 7350 0000 0000 0808 0202 0102 0102 0102  sP..............
 00000580: fc06 0608 010c 0108 0114 0302 0104 0102  ................
 00000590: 0104 0102 fc0c 0804 0102 0202 0102 0102  ................
 000005a0: 0102 0102 0102 fb04 0702 010a ff04 0308  ................
 000005b0: f502 0d02 f104 1002 f006 1412 0110 010e  ................
-000005c0: 0106 030e 0272 4300 0000 2903 4e4e 4e29  .....rC...).NNN)
-000005d0: 1172 2f00 0000 da09 6c69 6768 746e 696e  .r/.....lightnin
+000005c0: 0106 030e 0272 3a00 0000 2903 4e4e 4e29  .....r:...).NNN)
+000005d0: 1172 2d00 0000 da09 6c69 6768 746e 696e  .r-.....lightnin
 000005e0: 6772 0200 0000 da1b 6c69 6768 746e 696e  gr......lightnin
 000005f0: 672e 7079 746f 7263 682e 6361 6c6c 6261  g.pytorch.callba
 00000600: 636b 7372 0300 0000 7204 0000 0072 0500  cksr....r....r..
 00000610: 0000 da18 6461 7461 7365 7473 2e73 7061  ....datasets.spa
 00000620: 7469 616c 5f64 6174 6173 6574 7207 0000  tial_datasetr...
-00000630: 00da 1664 6174 6173 6574 732e 746f 7263  ...datasets.torc
+00000630: 005a 1664 6174 6173 6574 732e 746f 7263  .Z.datasets.torc
 00000640: 685f 6461 7461 7365 7472 0800 0000 da0a  h_datasetr......
 00000650: 636c 6173 7369 6669 6572 720a 0000 00da  classifierr.....
 00000660: 0d63 6f6e 6669 6775 7261 7469 6f6e 720b  .configurationr.
-00000670: 0000 00da 0373 7472 7243 0000 0072 4100  .....strrC...rA.
-00000680: 0000 7241 0000 0072 4100 0000 7242 0000  ..rA...rA...rB..
+00000670: 0000 00da 0373 7472 723a 0000 0072 3800  .....strr:...r8.
+00000680: 0000 7238 0000 0072 3800 0000 7239 0000  ..r8...r8...r9..
 00000690: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
 000006a0: 1c00 0000 0802 0c01 1402 0c01 0c01 0c01  ................
 000006b0: 0c07 0001 0001 00fa 0201 0201 0201 02fd  ................
```

### Comparing `morpheus_spatial-0.4.0/src/morpheus/classification/classifier.py` & `morpheus_spatial-0.5.0/src/morpheus/classification/classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         if self.arch == "unet":
             backbone = torch.hub.load(
                 "mateuszbuda/brain-segmentation-pytorch",
                 "unet",
                 in_channels=in_channels,
                 out_channels=1,
                 init_features=in_channels,
+                verbose=False,
             )
             classifier = torch.nn.Sequential()
             classifier.add_module("flatten", nn.Flatten())
             classifier.add_module(
                 "fc", nn.Linear(img_size[0] * img_size[1], self.classes)
             )
             classifier.add_module("act", nn.Softmax(dim=1))
@@ -126,15 +127,14 @@
 
     Args:
         model_path (str): Path to the model checkpoint.
 
     Returns:
         torch.nn.Module: Loaded model.
     """
-    from ..classification import PatchClassifier
 
     model = PatchClassifier.load_from_checkpoint(
         model_path,
         # in_channels=self.n_channels,
         # img_size=self.img_size,
         # arch=arch,
     )
```

### Comparing `morpheus_spatial-0.4.0/src/morpheus/classification/train.py` & `morpheus_spatial-0.5.0/src/morpheus/classification/train.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.4.0/src/morpheus/confidence/__pycache__/trustscore.cpython-39.pyc` & `morpheus_spatial-0.5.0/src/morpheus/confidence/__pycache__/trustscore.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.4.0/src/morpheus/confidence/trustscore.py` & `morpheus_spatial-0.5.0/src/morpheus/confidence/trustscore.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.4.0/src/morpheus/configuration/Types.py` & `morpheus_spatial-0.5.0/src/morpheus/configuration/Types.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.4.0/src/morpheus/counterfactual/__pycache__/cf.cpython-39.pyc` & `morpheus_spatial-0.5.0/src/morpheus/counterfactual/__pycache__/cf.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Apr  6 01:05:26 2024 UTC, .py size: 48197 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,1683 +1,1598 @@
-00000000: 610d 0d0a 0000 0000 d69f 1066 45bc 0000  a..........fE...
+00000000: 610d 0d0a 0000 0000 27f0 2166 859f 0000  a.......'.!f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
-00000050: 6401 6c04 5a05 6400 6402 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
-00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
-00000070: 0100 6400 6401 6c0c 5a0d 6400 6401 6c0e  ..d.d.l.Z.d.d.l.
-00000080: 6d0f 0200 0100 6d10 5a11 0100 6403 6404  m.....m.Z...d.d.
-00000090: 6c12 6d13 5a13 6d14 5a14 0100 6403 6405  l.m.Z.m.Z...d.d.
-000000a0: 6c15 6d16 5a16 6d17 5a17 6d18 5a18 0100  l.m.Z.m.Z.m.Z...
-000000b0: 6403 6406 6c19 6d1a 5a1a 0100 6400 6401  d.d.l.m.Z...d.d.
-000000c0: 6c1b 5a1b 6502 a01c 651d a101 5a1e 6511  l.Z.e...e...Z.e.
-000000d0: 6a02 a01f 6511 6a02 6a20 a101 0100 6511  j...e.j.j ....e.
-000000e0: 6a0f 6a10 a021 a100 0100 4700 6407 6408  j.j..!....G.d.d.
-000000f0: 8400 6408 6516 6518 8304 5a22 6409 640a  ..d.e.e...Z"d.d.
-00000100: 8400 5a23 640b 640c 8400 5a24 6401 5300  ..Z#d.d...Z$d.S.
-00000110: 290d e900 0000 004e 2905 da03 416e 79da  )......N)...Any.
-00000120: 0843 616c 6c61 626c 65da 084f 7074 696f  .Callable..Optio
-00000130: 6e61 6cda 0554 7570 6c65 da05 556e 696f  nal..Tuple..Unio
-00000140: 6ee9 0200 0000 2902 da0c 4445 4641 554c  n.....)...DEFAUL
-00000150: 545f 4441 5441 da0c 4445 4641 554c 545f  T_DATA..DEFAULT_
-00000160: 4d45 5441 2903 da09 4578 706c 6169 6e65  META)...Explaine
-00000170: 72da 0b45 7870 6c61 6e61 7469 6f6e da08  r..Explanation..
-00000180: 4669 744d 6978 696e 2901 da07 7065 7274  FitMixin)...pert
-00000190: 7572 6263 0000 0000 0000 0000 0000 0000  urbc............
-000001a0: 0000 0000 1900 0000 0000 0000 73ae 0100  ............s...
-000001b0: 0065 005a 0164 005a 0264 2565 0365 0465  .e.Z.d.Z.d%e.e.e
-000001c0: 056a 0667 0165 056a 0666 0219 0065 076a  .j.g.e.j.f...e.j
-000001d0: 086a 0966 0219 0065 0365 0465 056a 0667  .j.f...e.e.e.j.g
-000001e0: 0165 056a 0666 0219 0065 076a 086a 0966  .e.j.f...e.j.j.f
-000001f0: 0219 0065 0a65 0b65 0b65 0c65 0365 0b65  ...e.e.e.e.e.e.e
-00000200: 056a 0666 0219 0065 0365 0b65 056a 0666  .j.f...e.e.e.j.f
-00000210: 0219 0066 0219 0065 0b65 0d65 076a 086a  ...f...e.e.e.j.j
-00000220: 0919 0065 0d65 076a 086a 0919 0065 0b65  ...e.e.j.j...e.e
-00000230: 0e65 0b65 0f65 0b65 0f65 0a65 0a65 0f65  .e.e.e.e.e.e.e.e
-00000240: 0d65 1019 0065 0d65 1019 0065 0d65 076a  .e...e.e...e.e.j
-00000250: 1119 0065 0e64 0464 0d9c 1787 0066 0164  ...e.d.d.....f.d
-00000260: 0e64 0f84 0d5a 1265 05a0 1367 00a1 0165  .d...Z.e...g...e
-00000270: 05a0 1367 00a1 0164 0466 0365 056a 0665  ...g...d.f.e.j.e
-00000280: 056a 0665 0d65 1419 0064 0064 109c 0464  .j.e.e...d.d...d
-00000290: 1164 1284 055a 1565 056a 0665 056a 0665  .d...Z.e.j.e.j.e
-000002a0: 056a 0664 139c 0364 1464 1584 045a 1665  .j.d...d.d...Z.e
-000002b0: 056a 0665 056a 0665 0a65 056a 0664 169c  .j.e.j.e.e.j.d..
-000002c0: 0464 1764 1884 045a 1764 2665 056a 0665  .d.d...Z.d&e.j.e
-000002d0: 0f65 0f65 0b65 0b64 1a9c 0564 1b64 1c84  .e.e.e.d...d.d..
-000002e0: 055a 1864 2765 056a 0665 056a 0665 0d65  .Z.d'e.j.e.j.e.e
-000002f0: 1919 0065 0d65 0f19 0065 1065 0b65 0e65  ...e.e...e.e.e.e
-00000300: 0f65 0f65 0c65 056a 0665 0c65 056a 0665  .e.e.e.j.e.e.j.e
-00000310: 056a 0666 0219 0066 0219 0064 1f9c 0a64  .j.f...f...d...d
-00000320: 2064 2184 055a 1a64 2865 056a 0665 0d65   d!..Z.d(e.j.e.e
-00000330: 056a 0619 0065 0d65 1919 0065 0d65 0f19  .j...e.e...e.e..
-00000340: 0065 1065 0b65 0f65 0f65 1b64 229c 0964  .e.e.e.e.e.d"..d
-00000350: 2364 2484 055a 1c87 0004 005a 1d53 0029  #d$..Z.....Z.S.)
-00000360: 29da 0e43 6f75 6e74 6572 6661 6374 7561  )..Counterfactua
-00000370: 6ce7 0000 0000 0000 0000 e79a 9999 9999  l...............
-00000380: 99b9 3fa9 0267 0000 0020 5fa0 02c2 e700  ..?..g... _.....
-00000390: 0000 205f a002 424e 46e7 7b14 ae47 e17a  .. _..BNF.{..G.z
-000003a0: 843f e9e8 0300 00e7 0000 0000 0000 2440  .?............$@
-000003b0: e90a 0000 00a9 02e7 fca9 f1d2 4d62 503f  ............MbP?
-000003c0: 7218 0000 00a9 0267 0000 0000 0040 8fc0  r......g.....@..
-000003d0: 6700 0000 0000 408f 40e9 0100 0000 2917  g.....@.@.....).
-000003e0: da07 7072 6564 6963 74da 0f69 6e70 7574  ..predict..input
-000003f0: 5f74 7261 6e73 666f 726d da05 7368 6170  _transform..shap
-00000400: 65da 056b 6170 7061 da04 6265 7461 da0d  e..kappa..beta..
-00000410: 6665 6174 7572 655f 7261 6e67 65da 0567  feature_range..g
-00000420: 616d 6d61 da08 6165 5f6d 6f64 656c da09  amma..ae_model..
-00000430: 656e 635f 6d6f 6465 6cda 0574 6865 7461  enc_model..theta
-00000440: da0a 7573 655f 6b64 7472 6565 da12 6c65  ..use_kdtree..le
-00000450: 6172 6e69 6e67 5f72 6174 655f 696e 6974  arning_rate_init
-00000460: da0e 6d61 785f 6974 6572 6174 696f 6e73  ..max_iterations
-00000470: da06 635f 696e 6974 da07 635f 7374 6570  ..c_init..c_step
-00000480: 73da 0365 7073 da04 636c 6970 da0f 7570  s..eps..clip..up
-00000490: 6461 7465 5f6e 756d 5f67 7261 64da 0a74  date_num_grad..t
-000004a0: 7275 7374 7363 6f72 65da 0977 7269 7465  rustscore..write
-000004b0: 5f64 6972 da04 7365 7373 da07 7665 7262  _dir..sess..verb
-000004c0: 6f73 65da 0672 6574 7572 6e63 1700 0000  ose..returnc....
-000004d0: 0000 0000 0000 0000 2d00 0000 0c00 0000  ........-.......
-000004e0: 0300 0000 73a2 0c00 0074 0083 006a 0174  ....s....t...j.t
-000004f0: 02a0 0374 04a1 0164 018d 0101 0074 0588  ...t...d.....t..
-00000500: 0183 0164 026b 0472 3e88 0164 0364 0485  ...d.k.r>..d.d..
-00000510: 0219 007d 1788 0164 0519 0088 0164 0619  ...}...d.....d..
-00000520: 0066 0289 016e 0488 017d 1774 0683 007d  .f...n...}.t...}
-00000530: 1867 0064 07a2 017d 197c 1944 005d 0e7d  .g.d...}.|.D.].}
-00000540: 1a7c 18a0 077c 1aa1 0101 0071 547c 006a  .|...|.....qT|.j
-00000550: 0864 0819 00a0 097c 18a1 0101 007c 017c  .d.....|.....|.|
-00000560: 005f 0a7c 137c 005f 0b74 0c7c 0174 0d6a  ._.|.|._.t.|.t.j
-00000570: 0e6a 0f83 027d 1b74 0d6a 106a 116a 0e6a  .j...}.t.j.j.j.j
-00000580: 12a0 13a1 007d 1c74 0c7c 0874 0d6a 0e6a  .....}.t.|.t.j.j
-00000590: 0f83 027d 1d74 0c7c 0974 0d6a 0e6a 0f83  ...}.t.|.t.j.j..
-000005a0: 027d 1e7c 006a 0864 0819 006a 097c 1b7c  .}.|.j.d...j.|.|
-000005b0: 1d7c 1e64 098d 0301 0074 0c7c 1574 0d6a  .|.d.....t.|.t.j
-000005c0: 1483 0272 e47c 157c 005f 156e 067c 1c7c  ...r.|.|._.n.|.|
-000005d0: 005f 157c 1b90 0172 1264 0a7c 005f 167c  ._.|...r.d.|._.|
-000005e0: 006a 0aa0 0a74 17a0 1888 01a1 01a1 016a  .j...t.........j
-000005f0: 1964 0319 007c 005f 1a6e 3264 0b7c 005f  .d...|._.n2d.|._
-00000600: 167c 00a0 0a74 1b6a 1888 0164 0c8d 01a1  .|...t.j...d....
-00000610: 016a 1964 0319 007c 005f 1a74 1c64 0d7c  .j.d...|._.t.d.|
-00000620: 006a 1a9b 0064 0e9d 0383 0101 007c 1e90  .j...d.......|..
-00000630: 0172 5264 0a7c 005f 1d6e 0664 0b7c 005f  .rRd.|._.n.d.|._
-00000640: 1d7c 1d90 0172 6664 0a7c 005f 1e6e 0664  .|...rfd.|._.n.d
-00000650: 0b7c 005f 1e7c 0b90 0172 847c 006a 1d90  .|._.|...r.|.j..
-00000660: 0172 8474 1fa0 2064 0fa1 0101 007c 0b90  .r.t.. d.....|..
-00000670: 0173 927c 006a 1d90 0172 9a64 0a7c 005f  .s.|.j...r.d.|._
-00000680: 216e 0664 0b7c 005f 217c 006a 0864 0819  !n.d.|._!|.j.d..
-00000690: 006a 097c 006a 2164 108d 0101 007c 006a  .j.|.j!d.....|.j
-000006a0: 0864 0819 006a 0964 0b64 118d 0101 0088  .d...j.d.d......
-000006b0: 017c 005f 197c 177c 005f 227c 047c 005f  .|._.|.|._"|.|._
-000006c0: 237c 057c 005f 247c 077c 005f 257c 0a7c  #|.|._$|.|._%|.|
-000006d0: 005f 267c 087c 005f 277c 097c 005f 287c  ._&|.|._'|.|._(|
-000006e0: 0b7c 005f 2988 0164 0519 007c 005f 2a7c  .|._)..d...|._*|
-000006f0: 0d7c 005f 2b7c 0e7c 005f 2c7c 0f7c 005f  .|._+|.|._,|.|._
-00000700: 2d74 2e87 0087 0166 0264 1264 1384 0874  -t.....f.d.d...t
-00000710: 2f64 0283 0144 0083 0183 017c 005f 307c  /d...D.....|._0|
-00000720: 127c 005f 317c 107c 005f 327c 117c 005f  .|._1|.|._2|.|._
-00000730: 337c 027c 005f 347c 147c 005f 357c 167c  3|.|._4|.|._5|.|
-00000740: 005f 3674 0d6a 3774 17a0 1888 01a1 0174  ._6t.j7t.......t
-00000750: 0d6a 3864 1464 158d 037c 005f 3974 0d6a  .j8d.d...|._9t.j
-00000760: 3774 17a0 1888 01a1 0174 0d6a 3864 1664  7t.......t.j8d.d
-00000770: 158d 037c 005f 3a74 0d6a 3774 17a0 1888  ...|._:t.j7t....
-00000780: 01a1 0174 0d6a 3864 1764 158d 037c 005f  ...t.j8d.d...|._
-00000790: 3b74 0d6a 3774 17a0 187c 006a 2a7c 006a  ;t.j7t...|.j*|.j
-000007a0: 1a66 02a1 0174 0d6a 3864 1864 158d 037c  .f...t.j8d.d...|
-000007b0: 005f 3c7c 006a 1d90 0272 ec7c 006a 28a0  ._<|.j...r.|.j(.
-000007c0: 0a74 17a0 187c 006a 19a1 01a1 016a 197c  .t...|.j.....j.|
-000007d0: 005f 3d6e 087c 006a 197c 005f 3d74 0d6a  ._=n.|.j.|._=t.j
-000007e0: 3774 17a0 187c 006a 3da1 0174 0d6a 3864  7t...|.j=..t.j8d
-000007f0: 1964 158d 037c 005f 3e74 0d6a 3774 17a0  .d...|._>t.j7t..
-00000800: 187c 006a 2aa1 0174 0d6a 3864 1a64 158d  .|.j*..t.j8d.d..
-00000810: 037c 005f 3f74 0d6a 3764 1b64 0b64 1c64  .|._?t.j7d.d.d.d
-00000820: 1d8d 037c 005f 4074 0d6a 4174 0d6a 3888  ...|._@t.jAt.j8.
-00000830: 0164 1e64 1f8d 037c 005f 4274 0d6a 4174  .d.d...|._Bt.jAt
-00000840: 0d6a 3888 0164 2064 1f8d 037c 005f 4374  .j8..d d...|._Ct
-00000850: 0d6a 4174 0d6a 3888 0164 2164 1f8d 037c  .jAt.j8..d!d...|
-00000860: 005f 4474 0d6a 4174 0d6a 387c 006a 2a7c  ._Dt.jAt.j8|.j*|
-00000870: 006a 1a66 0264 2264 1f8d 037c 005f 4574  .j.f.d"d...|._Et
-00000880: 0d6a 4174 0d6a 387c 006a 2a67 0164 2364  .jAt.j8|.j*g.d#d
-00000890: 1f8d 037c 005f 4674 0d6a 4174 0d6a 387c  ...|._Ft.jAt.j8|
-000008a0: 006a 3d64 2464 1f8d 037c 005f 4774 0da0  .j=d$d...|._Gt..
-000008b0: 4864 25a1 0190 018f 067d 1f74 0da0 4974  Hd%......}.t..It
-000008c0: 0da0 4a74 0da0 4b7c 006a 3b7c 006a 39a1  ..Jt..K|.j;|.j9.
-000008d0: 027c 006a 24a1 0274 0d6a 38a1 0274 0da0  .|.j$..t.j8..t..
-000008e0: 4974 0da0 4c74 0da0 4d74 0da0 4b7c 006a  It..Lt..Mt..K|.j
-000008f0: 3b7c 006a 39a1 02a1 017c 006a 24a1 0274  ;|.j9....|.j$..t
-00000900: 0d6a 38a1 0274 0da0 4974 0da0 4e74 0da0  .j8..t..It..Nt..
-00000910: 4b7c 006a 3b7c 006a 39a1 0274 0da0 4f7c  K|.j;|.j9..t..O|
-00000920: 006a 24a1 01a1 0274 0d6a 38a1 0267 037d  .j$....t.j8..g.}
-00000930: 2074 0da0 5074 0da0 4b7c 006a 3b7c 006a   t..Pt..K|.j;|.j
-00000940: 24a1 0274 0da0 4988 0064 0319 0074 0d6a  $..t..I..d...t.j
-00000950: 38a1 02a1 027d 2174 0da0 5174 0da0 527c  8....}!t..Qt..R|
-00000960: 006a 3b7c 006a 24a1 0274 0da0 4988 0064  .j;|.j$..t..I..d
-00000970: 0519 0074 0d6a 38a1 02a1 027d 2274 0da0  ...t.j8....}"t..
-00000980: 537c 2064 0519 007c 21a1 0274 0da0 537c  S| d...|!..t..S|
-00000990: 2064 0319 007c 006a 39a1 0217 0074 0da0   d...|.j9....t..
-000009a0: 537c 2064 0219 007c 22a1 0217 007c 005f  S| d...|"....|._
-000009b0: 4357 0064 0404 0004 0083 0301 006e 1231  CW.d.........n.1
-000009c0: 0090 0473 de30 0001 0001 0001 0059 0001  ...s.0.......Y..
-000009d0: 0074 0da0 4864 26a1 018f 8a7d 1f74 0da0  .t..Hd&....}.t..
-000009e0: 547c 006a 407c 006a 4074 0da0 4964 2774  T|.j@|.j@t..Id't
-000009f0: 0d6a 38a1 0217 00a1 027c 005f 557c 006a  .j8......|._U|.j
-00000a00: 4374 0da0 537c 006a 557c 006a 437c 006a  Ct..S|.jU|.jC|.j
-00000a10: 3a18 00a1 0217 007c 005f 4474 0da0 507c  :......|._Dt..P|
-00000a20: 006a 4474 0da0 4988 0064 0319 0074 0d6a  .jDt..I..d...t.j
-00000a30: 38a1 02a1 027c 005f 4474 0da0 517c 006a  8....|._Dt..Q|.j
-00000a40: 4474 0da0 4988 0064 0519 0074 0d6a 38a1  Dt..I..d...t.j8.
-00000a50: 02a1 027c 005f 4457 0064 0404 0004 0083  ...|._DW.d......
-00000a60: 0301 006e 1231 0090 0573 8430 0001 0001  ...n.1...s.0....
-00000a70: 0001 0059 0001 0074 0da0 4864 28a1 018f  ...Y...t..Hd(...
-00000a80: 347d 1f74 0da0 567c 006a 3a7c 006a 43a1  4}.t..V|.j:|.jC.
-00000a90: 027c 005f 5774 0da0 567c 006a 3b7c 006a  .|._Wt..V|.j;|.j
-00000aa0: 44a1 027c 005f 5857 0064 0404 0004 0083  D..|._XW.d......
-00000ab0: 0301 006e 1231 0090 0573 d430 0001 0001  ...n.1...s.0....
-00000ac0: 0001 0059 0001 0074 0da0 4864 29a1 018f  ...Y...t..Hd)...
-00000ad0: 2c7d 1f7c 006a 397c 006a 3a18 007c 005f  ,}.|.j9|.j:..|._
-00000ae0: 597c 006a 397c 006a 3b18 007c 005f 5a57  Y|.j9|.j;..|._ZW
-00000af0: 0064 0404 0004 0083 0301 006e 1231 0090  .d.........n.1..
-00000b00: 0673 1c30 0001 0001 0001 0059 0001 0074  .s.0.......Y...t
-00000b10: 5b74 17a0 5c64 0374 0588 0183 01a1 0283  [t..\d.t........
-00000b20: 017d 2374 0da0 4864 2aa1 018f d87d 1f74  .}#t..Hd*....}.t
-00000b30: 0d6a 5d74 0da0 5e7c 006a 59a1 017c 2364  .j]t..^|.jY..|#d
-00000b40: 2b8d 027c 005f 5f74 0d6a 5d74 0da0 5e7c  +..|.__t.j]t..^|
-00000b50: 006a 5aa1 017c 2364 2b8d 027c 005f 6074  .jZ..|#d+..|._`t
-00000b60: 0d6a 5d74 0da0 4d7c 006a 59a1 017c 2364  .j]t..M|.jY..|#d
-00000b70: 2b8d 027c 005f 6174 0d6a 5d74 0da0 4d7c  +..|._at.j]t..M|
-00000b80: 006a 5aa1 017c 2364 2b8d 027c 005f 627c  .jZ..|#d+..|._b|
-00000b90: 006a 5f74 0da0 537c 006a 617c 006a 24a1  .j_t..S|.ja|.j$.
-00000ba0: 0217 007c 005f 637c 006a 6074 0da0 537c  ...|._c|.j`t..S|
-00000bb0: 006a 627c 006a 24a1 0217 007c 005f 6474  .jb|.j$....|._dt
-00000bc0: 0da0 5d7c 006a 61a1 017c 005f 6574 0da0  ..]|.ja..|._et..
-00000bd0: 5d7c 006a 62a1 017c 005f 6674 0da0 5d7c  ]|.jb..|._ft..]|
-00000be0: 006a 5fa1 017c 005f 6774 0da0 5d7c 006a  .j_..|._gt..]|.j
-00000bf0: 60a1 017c 005f 6857 0064 0404 0004 0083  `..|._hW.d......
-00000c00: 0301 006e 1231 0090 0773 2430 0001 0001  ...n.1...s$0....
-00000c10: 0001 0059 0001 007c 006a 3a7c 005f 697c  ...Y...|.j:|._i|
-00000c20: 006a 3b7c 005f 6a74 0da0 4864 2ca1 018f  .j;|._jt..Hd,...
-00000c30: 8e7d 1f7c 006a 1e90 0772 b07c 00a0 277c  .}.|.j...r.|..'|
-00000c40: 006a 69a1 017c 005f 6b7c 00a0 277c 006a  .ji..|._k|..'|.j
-00000c50: 6aa1 017c 005f 6c7c 006a 2574 0da0 5e74  j..|._l|.j%t..^t
-00000c60: 0da0 6d7c 006a 6b7c 006a 3a18 00a1 01a1  ..m|.jk|.j:.....
-00000c70: 0114 007c 005f 6e7c 006a 2574 0da0 5e74  ...|._n|.j%t..^t
-00000c80: 0da0 6d7c 006a 6c7c 006a 3b18 00a1 01a1  ..m|.jl|.j;.....
-00000c90: 0114 007c 005f 6f6e 1874 0da0 7064 1ba1  ...|._on.t..pd..
-00000ca0: 017c 005f 6e74 0da0 7064 1ba1 017c 005f  .|._nt..pd...|._
-00000cb0: 6f57 0064 0404 0004 0083 0301 006e 1231  oW.d.........n.1
-00000cc0: 0090 0773 de30 0001 0001 0001 0059 0001  ...s.0.......Y..
-00000cd0: 0074 0da0 4864 2da1 0190 018f 5c7d 1f7c  .t..Hd-.....\}.|
-00000ce0: 006a 1690 0873 1074 0da0 4174 0d6a 38a1  .j...s.t..At.j8.
-00000cf0: 017c 005f 7190 016e 327c 006a 2c64 1b6b  .|._q..n2|.j,d.k
-00000d00: 0290 0872 5e7c 006a 2d64 036b 0290 0872  ...r^|.j-d.k...r
-00000d10: 5e7c 00a0 0a7c 006a 69a1 017c 005f 727c  ^|...|.ji..|._r|
-00000d20: 00a0 0a7c 006a 6aa1 017c 005f 7374 0da0  ...|.jj..|._st..
-00000d30: 7064 1ba1 017c 005f 7174 0da0 7064 1ba1  pd...|._qt..pd..
-00000d40: 017c 005f 746e e47c 00a0 0a7c 006a 69a1  .|._tn.|...|.ji.
-00000d50: 017c 005f 727c 00a0 0a7c 006a 6aa1 017c  .|._r|...|.jj..|
-00000d60: 005f 7374 0da0 5d7c 006a 3c7c 006a 7214  ._st..]|.j<|.jr.
-00000d70: 0064 03a1 027c 005f 7574 0da0 5d7c 006a  .d...|._ut..]|.j
-00000d80: 3c7c 006a 7314 0064 03a1 027d 2474 0da0  <|.js..d...}$t..
-00000d90: 7664 037c 006a 3c18 007c 006a 7214 007c  vd.|.j<..|.jr..|
-00000da0: 006a 3c64 2e14 0018 0064 03a1 027c 005f  .j<d.....d...|._
-00000db0: 7774 0da0 7664 037c 006a 3c18 007c 006a  wt..vd.|.j<..|.j
-00000dc0: 7314 007c 006a 3c64 2e14 0018 0064 03a1  s..|.j<d.....d..
-00000dd0: 027d 2574 0da0 5164 1b7c 006a 770b 007c  .}%t..Qd.|.jw..|
-00000de0: 006a 7517 007c 006a 2317 00a1 027d 2674  .ju..|.j#....}&t
-00000df0: 0da0 5164 1b7c 250b 007c 2417 007c 006a  ..Qd.|%..|$..|.j
-00000e00: 2317 00a1 027d 2774 0da0 5d7c 006a 3f7c  #....}'t..]|.j?|
-00000e10: 2614 00a1 017c 005f 7174 0da0 5d7c 006a  &....|._qt..]|.j
-00000e20: 3f7c 2714 00a1 017c 005f 7457 0064 0404  ?|'....|._tW.d..
-00000e30: 0004 0083 0301 006e 1231 0090 0973 5830  .......n.1...sX0
-00000e40: 0001 0001 0001 0059 0001 0074 0da0 4864  .......Y...t..Hd
-00000e50: 2fa1 018f c87d 1f7c 006a 1d90 0972 c47c  /....}.|.j...r.|
-00000e60: 006a 2674 0da0 5e74 0da0 6d7c 00a0 287c  .j&t..^t..m|..(|
-00000e70: 006a 69a1 017c 006a 3e18 00a1 01a1 0114  .ji..|.j>.......
-00000e80: 007c 005f 787c 006a 2674 0da0 5e74 0da0  .|._x|.j&t..^t..
-00000e90: 6d7c 00a0 287c 006a 6aa1 017c 006a 3e18  m|..(|.jj..|.j>.
-00000ea0: 00a1 01a1 0114 007c 005f 796e 627c 006a  .......|._ynb|.j
-00000eb0: 2990 0a72 0e7c 006a 2674 0da0 5e74 0da0  )..r.|.j&t..^t..
-00000ec0: 6d7c 006a 3a7c 006a 3e18 00a1 01a1 0114  m|.j:|.j>.......
-00000ed0: 007c 005f 787c 006a 2674 0da0 5e74 0da0  .|._x|.j&t..^t..
-00000ee0: 6d7c 006a 3b7c 006a 3e18 00a1 01a1 0114  m|.j;|.j>.......
-00000ef0: 007c 005f 796e 1874 0da0 7064 1ba1 017c  .|._yn.t..pd...|
-00000f00: 005f 7874 0da0 7064 1ba1 017c 005f 7957  ._xt..pd...|._yW
-00000f10: 0064 0404 0004 0083 0301 006e 1231 0090  .d.........n.1..
-00000f20: 0a73 3c30 0001 0001 0001 0059 0001 0074  .s<0.......Y...t
-00000f30: 0da0 4864 30a1 018f 727d 1f7c 006a 1690  ..Hd0...r}.|.j..
-00000f40: 0a72 767c 006a 747c 006a 6817 007c 006a  .rv|.jt|.jh..|.j
-00000f50: 6f17 007c 006a 7917 007c 005f 7a6e 147c  o..|.jy..|._zn.|
-00000f60: 006a 687c 006a 6f17 007c 006a 7917 007c  .jh|.jo..|.jy..|
-00000f70: 005f 7a7c 006a 717c 006a 6717 007c 006a  ._z|.jq|.jg..|.j
-00000f80: 6e17 0074 0da0 537c 006a 247c 006a 65a1  n..t..S|.j$|.je.
-00000f90: 0217 007c 006a 7817 007c 005f 7b57 0064  ...|.jx..|._{W.d
-00000fa0: 0404 0004 0083 0301 006e 1231 0090 0a73  .........n.1...s
-00000fb0: ca30 0001 0001 0001 0059 0001 0074 0da0  .0.......Y...t..
-00000fc0: 4864 31a1 018f c67d 1f74 0d6a 7c6a 7d7c  Hd1....}.t.j|j}|
-00000fd0: 0c7c 006a 407c 006a 2b64 0564 3264 338d  .|.j@|.j+d.d2d3.
-00000fe0: 057c 005f 7e74 0d6a 7ca0 7f7c 006a 7ea1  .|._~t.j|..|.j~.
-00000ff0: 017d 2874 8064 3464 3584 0074 0da0 81a1  .}(t.d4d5..t....
-00001000: 0044 0083 0183 0189 027c 286a 827c 006a  .D.......|(j.|.j
-00001010: 7a7c 006a 3b67 0164 368d 027c 005f 8374  z|.j;g.d6..|._.t
-00001020: 0d6a 4174 0d6a 3864 3764 1f8d 027c 005f  .jAt.j8d7d...|._
-00001030: 8464 3864 1384 0074 0da0 85a1 0044 0083  .d8d...t.....D..
-00001040: 0164 0619 007d 297c 006a 847c 2966 0267  .d...})|.j.|)f.g
-00001050: 017d 2a7c 286a 867c 2a7c 006a 4064 398d  .}*|(j.|*|.j@d9.
-00001060: 027c 005f 8774 0da0 81a1 007d 2b87 0266  .|._.t.....}+..f
-00001070: 0164 3a64 1384 087c 2b44 0083 017d 2c57  .d:d...|+D...},W
-00001080: 0064 0404 0004 0083 0301 006e 1231 0090  .d.........n.1..
-00001090: 0b73 ac30 0001 0001 0001 0059 0001 0067  .s.0.......Y...g
-000010a0: 007c 005f 887c 006a 88a0 897c 006a 39a0  .|._.|.j...|.j9.
-000010b0: 567c 006a 42a1 01a1 0101 007c 006a 88a0  V|.jB......|.j..
-000010c0: 897c 006a 3ca0 567c 006a 45a1 01a1 0101  .|.j<.V|.jE.....
-000010d0: 007c 006a 88a0 897c 006a 3fa0 567c 006a  .|.j...|.j?.V|.j
-000010e0: 46a1 01a1 0101 007c 006a 88a0 897c 006a  F......|.j...|.j
-000010f0: 3aa0 567c 006a 43a1 01a1 0101 007c 006a  :.V|.jC......|.j
-00001100: 88a0 897c 006a 3ba0 567c 006a 44a1 01a1  ...|.j;.V|.jD...
-00001110: 0101 007c 006a 88a0 897c 006a 3ea0 567c  ...|.j...|.j>.V|
-00001120: 006a 47a1 01a1 0101 0074 0d6a 8a7c 006a  .jG......t.j.|.j
-00001130: 4067 017c 006a 3b67 0117 007c 006a 3a67  @g.|.j;g...|.j:g
-00001140: 0117 007c 2c17 0064 368d 017c 005f 8b7c  ...|,..d6..|._.|
-00001150: 006a 3564 0475 0190 0c72 9874 0d6a 8ca0  .j5d.u...r.t.j..
-00001160: 8d7c 1474 0da0 8ea1 00a1 027c 005f 8f7c  .|.t.......|._.|
-00001170: 006a 8fa0 9074 0da0 8ea1 00a1 0101 006e  .j...t.........n
-00001180: 0664 047c 005f 8f64 0453 0029 3b61 a609  .d.|._.d.S.);a..
-00001190: 0000 0a20 2020 2020 2020 2049 6e69 7469  ...        Initi
-000011a0: 616c 697a 6520 7072 6f74 6f74 7970 6963  alize prototypic
-000011b0: 616c 2063 6f75 6e74 6572 6661 6374 7561  al counterfactua
-000011c0: 6c20 6d65 7468 6f64 2e0a 0a20 2020 2020  l method...     
-000011d0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-000011e0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-000011f0: 0a20 2020 2020 2020 2070 7265 6469 6374  .        predict
-00001200: 0a20 2020 2020 2020 2020 2020 2060 7465  .            `te
-00001210: 6e73 6f72 666c 6f77 6020 6d6f 6465 6c20  nsorflow` model 
-00001220: 6f72 2061 6e79 206f 7468 6572 206d 6f64  or any other mod
-00001230: 656c 2773 2070 7265 6469 6374 696f 6e20  el's prediction 
-00001240: 6675 6e63 7469 6f6e 2072 6574 7572 6e69  function returni
-00001250: 6e67 2063 6c61 7373 2070 726f 6261 6269  ng class probabi
-00001260: 6c69 7469 6573 2e0a 2020 2020 2020 2020  lities..        
-00001270: 7368 6170 650a 2020 2020 2020 2020 2020  shape.          
-00001280: 2020 5368 6170 6520 6f66 2069 6e70 7574    Shape of input
-00001290: 2064 6174 6120 7374 6172 7469 6e67 2077   data starting w
-000012a0: 6974 6820 6261 7463 6820 7369 7a65 2e0a  ith batch size..
-000012b0: 2020 2020 2020 2020 6b61 7070 610a 2020          kappa.  
-000012c0: 2020 2020 2020 2020 2020 436f 6e66 6964            Confid
-000012d0: 656e 6365 2070 6172 616d 6574 6572 2066  ence parameter f
-000012e0: 6f72 2074 6865 2061 7474 6163 6b20 6c6f  or the attack lo
-000012f0: 7373 2074 6572 6d2e 0a20 2020 2020 2020  ss term..       
-00001300: 2062 6574 610a 2020 2020 2020 2020 2020   beta.          
-00001310: 2020 5265 6775 6c61 7269 7a61 7469 6f6e    Regularization
-00001320: 2063 6f6e 7374 616e 7420 666f 7220 4c31   constant for L1
-00001330: 206c 6f73 7320 7465 726d 2e0a 2020 2020   loss term..    
-00001340: 2020 2020 6665 6174 7572 655f 7261 6e67      feature_rang
-00001350: 650a 2020 2020 2020 2020 2020 2020 5475  e.            Tu
-00001360: 706c 6520 7769 7468 2060 6d69 6e60 2061  ple with `min` a
-00001370: 6e64 2060 6d61 7860 2072 616e 6765 7320  nd `max` ranges 
-00001380: 746f 2061 6c6c 6f77 2066 6f72 2070 6572  to allow for per
-00001390: 7475 7262 6564 2069 6e73 7461 6e63 6573  turbed instances
-000013a0: 2e20 604d 696e 6020 616e 6420 606d 6178  . `Min` and `max
-000013b0: 6020 7261 6e67 6573 2063 616e 2062 6520  ` ranges can be 
-000013c0: 6066 6c6f 6174 600a 2020 2020 2020 2020  `float`.        
-000013d0: 2020 2020 6f72 2060 6e75 6d70 7960 2061      or `numpy` a
-000013e0: 7272 6179 7320 7769 7468 2064 696d 656e  rrays with dimen
-000013f0: 7369 6f6e 2028 3178 206e 6220 6f66 2066  sion (1x nb of f
-00001400: 6561 7475 7265 7329 2066 6f72 2066 6561  eatures) for fea
-00001410: 7475 7265 2d77 6973 6520 7261 6e67 6573  ture-wise ranges
-00001420: 2e0a 2020 2020 2020 2020 6761 6d6d 610a  ..        gamma.
-00001430: 2020 2020 2020 2020 2020 2020 5265 6775              Regu
-00001440: 6c61 7269 7a61 7469 6f6e 2063 6f6e 7374  larization const
-00001450: 616e 7420 666f 7220 6f70 7469 6f6e 616c  ant for optional
-00001460: 2061 7574 6f2d 656e 636f 6465 7220 6c6f   auto-encoder lo
-00001470: 7373 2074 6572 6d2e 0a20 2020 2020 2020  ss term..       
-00001480: 2061 655f 6d6f 6465 6c0a 2020 2020 2020   ae_model.      
-00001490: 2020 2020 2020 4f70 7469 6f6e 616c 2061        Optional a
-000014a0: 7574 6f2d 656e 636f 6465 7220 6d6f 6465  uto-encoder mode
-000014b0: 6c20 7573 6564 2066 6f72 206c 6f73 7320  l used for loss 
-000014c0: 7265 6775 6c61 7269 7a61 7469 6f6e 2e0a  regularization..
-000014d0: 2020 2020 2020 2020 656e 635f 6d6f 6465          enc_mode
-000014e0: 6c0a 2020 2020 2020 2020 2020 2020 4f70  l.            Op
-000014f0: 7469 6f6e 616c 2065 6e63 6f64 6572 206d  tional encoder m
-00001500: 6f64 656c 2075 7365 6420 746f 2067 7569  odel used to gui
-00001510: 6465 2069 6e73 7461 6e63 6520 7065 7274  de instance pert
-00001520: 7572 6261 7469 6f6e 7320 746f 7761 7264  urbations toward
-00001530: 7320 6120 636c 6173 7320 7072 6f74 6f74  s a class protot
-00001540: 7970 652e 0a20 2020 2020 2020 2074 6865  ype..        the
-00001550: 7461 0a20 2020 2020 2020 2020 2020 2043  ta.            C
-00001560: 6f6e 7374 616e 7420 666f 7220 7468 6520  onstant for the 
-00001570: 7072 6f74 6f74 7970 6520 7365 6172 6368  prototype search
-00001580: 206c 6f73 7320 7465 726d 2e0a 2020 2020   loss term..    
-00001590: 2020 2020 7573 655f 6b64 7472 6565 0a20      use_kdtree. 
-000015a0: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
-000015b0: 6572 2074 6f20 7573 6520 6b2d 6420 7472  er to use k-d tr
-000015c0: 6565 7320 666f 7220 7468 6520 7072 6f74  ees for the prot
-000015d0: 6f74 7970 6520 6c6f 7373 2074 6572 6d20  otype loss term 
-000015e0: 6966 206e 6f20 656e 636f 6465 7220 6973  if no encoder is
-000015f0: 2061 7661 696c 6162 6c65 2e0a 2020 2020   available..    
-00001600: 2020 2020 6c65 6172 6e69 6e67 5f72 6174      learning_rat
-00001610: 655f 696e 6974 0a20 2020 2020 2020 2020  e_init.         
-00001620: 2020 2049 6e69 7469 616c 206c 6561 726e     Initial learn
-00001630: 696e 6720 7261 7465 206f 6620 6f70 7469  ing rate of opti
-00001640: 6d69 7a65 722e 0a20 2020 2020 2020 206d  mizer..        m
-00001650: 6178 5f69 7465 7261 7469 6f6e 730a 2020  ax_iterations.  
-00001660: 2020 2020 2020 2020 2020 4d61 7869 6d75            Maximu
-00001670: 6d20 6e75 6d62 6572 206f 6620 6974 6572  m number of iter
-00001680: 6174 696f 6e73 2066 6f72 2066 696e 6469  ations for findi
-00001690: 6e67 2061 2063 6f75 6e74 6572 6661 6374  ng a counterfact
-000016a0: 7561 6c2e 0a20 2020 2020 2020 2063 5f69  ual..        c_i
-000016b0: 6e69 740a 2020 2020 2020 2020 2020 2020  nit.            
-000016c0: 496e 6974 6961 6c20 7661 6c75 6520 746f  Initial value to
-000016d0: 2073 6361 6c65 2074 6865 2061 7474 6163   scale the attac
-000016e0: 6b20 6c6f 7373 2074 6572 6d2e 0a20 2020  k loss term..   
-000016f0: 2020 2020 2063 5f73 7465 7073 0a20 2020       c_steps.   
-00001700: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
-00001710: 6f66 2069 7465 7261 7469 6f6e 7320 746f  of iterations to
-00001720: 2061 646a 7573 7420 7468 6520 636f 6e73   adjust the cons
-00001730: 7461 6e74 2073 6361 6c69 6e67 2074 6865  tant scaling the
-00001740: 2061 7474 6163 6b20 6c6f 7373 2074 6572   attack loss ter
-00001750: 6d2e 0a20 2020 2020 2020 2065 7073 0a20  m..        eps. 
-00001760: 2020 2020 2020 2020 2020 2049 6620 6e75             If nu
-00001770: 6d65 7269 6361 6c20 6772 6164 6965 6e74  merical gradient
-00001780: 7320 6172 6520 7573 6564 2074 6f20 636f  s are used to co
-00001790: 6d70 7574 6520 6064 4c2f 6478 203d 2028  mpute `dL/dx = (
-000017a0: 644c 2f64 7029 202a 2028 6470 2f64 7829  dL/dp) * (dp/dx)
-000017b0: 602c 2074 6865 6e20 6065 7073 5b30 5d60  `, then `eps[0]`
-000017c0: 2069 7320 7573 6564 2074 6f0a 2020 2020   is used to.    
-000017d0: 2020 2020 2020 2020 6361 6c63 756c 6174          calculat
-000017e0: 6520 6064 4c2f 6470 6020 616e 6420 6065  e `dL/dp` and `e
-000017f0: 7073 5b31 5d60 2069 7320 7573 6564 2066  ps[1]` is used f
-00001800: 6f72 2060 6470 2f64 7860 2e20 6065 7073  or `dp/dx`. `eps
-00001810: 5b30 5d60 2061 6e64 2060 6570 735b 315d  [0]` and `eps[1]
-00001820: 6020 6361 6e20 6265 2061 2063 6f6d 6269  ` can be a combi
-00001830: 6e61 7469 6f6e 206f 6620 6066 6c6f 6174  nation of `float
-00001840: 600a 2020 2020 2020 2020 2020 2020 7661  `.            va
-00001850: 6c75 6573 2061 6e64 2060 6e75 6d70 7960  lues and `numpy`
-00001860: 2061 7272 6179 732e 2046 6f72 2060 6570   arrays. For `ep
-00001870: 735b 305d 602c 2074 6865 2061 7272 6179  s[0]`, the array
-00001880: 2064 696d 656e 7369 6f6e 2073 686f 756c   dimension shoul
-00001890: 6420 6265 2028 3178 206e 6220 6f66 2070  d be (1x nb of p
-000018a0: 7265 6469 6374 696f 6e20 6361 7465 676f  rediction catego
-000018b0: 7269 6573 290a 2020 2020 2020 2020 2020  ries).          
-000018c0: 2020 616e 6420 666f 7220 6065 7073 5b31    and for `eps[1
-000018d0: 5d60 2069 7420 7368 6f75 6c64 2062 6520  ]` it should be 
-000018e0: 2831 7820 6e62 206f 6620 6665 6174 7572  (1x nb of featur
-000018f0: 6573 292e 0a20 2020 2020 2020 2063 6c69  es)..        cli
-00001900: 700a 2020 2020 2020 2020 2020 2020 5475  p.            Tu
-00001910: 706c 6520 7769 7468 206d 696e 2061 6e64  ple with min and
-00001920: 206d 6178 2063 6c69 7020 7261 6e67 6573   max clip ranges
-00001930: 2066 6f72 2062 6f74 6820 7468 6520 6e75   for both the nu
-00001940: 6d65 7269 6361 6c20 6772 6164 6965 6e74  merical gradient
-00001950: 7320 616e 6420 7468 6520 6772 6164 6965  s and the gradie
-00001960: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-00001970: 6f62 7461 696e 6564 2066 726f 6d20 7468  obtained from th
-00001980: 6520 6074 656e 736f 7266 6c6f 7760 2067  e `tensorflow` g
-00001990: 7261 7068 2e0a 2020 2020 2020 2020 7570  raph..        up
-000019a0: 6461 7465 5f6e 756d 5f67 7261 640a 2020  date_num_grad.  
-000019b0: 2020 2020 2020 2020 2020 4966 206e 756d            If num
-000019c0: 6572 6963 616c 2067 7261 6469 656e 7473  erical gradients
-000019d0: 2061 7265 2075 7365 642c 2074 6865 7920   are used, they 
-000019e0: 7769 6c6c 2062 6520 7570 6461 7465 6420  will be updated 
-000019f0: 6576 6572 7920 6075 7064 6174 655f 6e75  every `update_nu
-00001a00: 6d5f 6772 6164 6020 6974 6572 6174 696f  m_grad` iteratio
-00001a10: 6e73 2e0a 2020 2020 2020 2020 7472 7573  ns..        trus
-00001a20: 7473 636f 7265 0a20 2020 2020 2020 2020  tscore.         
-00001a30: 2020 2044 6972 6563 746f 7279 2077 6865     Directory whe
-00001a40: 7265 2074 7275 7374 7363 6f72 6520 6f62  re trustscore ob
-00001a50: 6a65 6374 2069 7320 746f 2062 6520 7573  ject is to be us
-00001a60: 6564 0a20 2020 2020 2020 2077 7269 7465  ed.        write
-00001a70: 5f64 6972 0a20 2020 2020 2020 2020 2020  _dir.           
-00001a80: 2044 6972 6563 746f 7279 2074 6f20 7772   Directory to wr
-00001a90: 6974 6520 6074 656e 736f 7262 6f61 7264  ite `tensorboard
-00001aa0: 6020 6669 6c65 7320 746f 2e0a 2020 2020  ` files to..    
-00001ab0: 2020 2020 7365 7373 0a20 2020 2020 2020      sess.       
-00001ac0: 2020 2020 204f 7074 696f 6e61 6c20 6074       Optional `t
-00001ad0: 656e 736f 7266 6c6f 7760 2073 6573 7369  ensorflow` sessi
-00001ae0: 6f6e 2074 6861 7420 7769 6c6c 2062 6520  on that will be 
-00001af0: 7573 6564 2069 6620 7061 7373 6564 2069  used if passed i
-00001b00: 6e73 7465 6164 206f 6620 6372 6561 7469  nstead of creati
-00001b10: 6e67 206f 7220 696e 6665 7272 696e 6720  ng or inferring 
-00001b20: 6f6e 6520 696e 7465 726e 616c 6c79 2e0a  one internally..
-00001b30: 2020 2020 2020 2020 2901 da04 6d65 7461          )...meta
-00001b40: 7207 0000 0072 1a00 0000 4e72 0100 0000  r....r....Nr....
-00001b50: e9ff ffff ff29 07da 0473 656c 6672 1b00  .....)...selfr..
-00001b60: 0000 721c 0000 0072 2200 0000 7223 0000  ..r....r"...r#..
-00001b70: 0072 2f00 0000 da09 5f5f 636c 6173 735f  .r/.....__class_
-00001b80: 5fda 0670 6172 616d 7329 03da 0869 735f  _..params)...is_
-00001b90: 6d6f 6465 6cda 0569 735f 6165 da06 6973  model..is_ae..is
-00001ba0: 5f65 6e63 5446 2901 da04 7369 7a65 7a15  _encTF)...sizez.
-00001bb0: 426c 6163 6b20 626f 7820 6d6f 6465 6c20  Black box model 
-00001bc0: 7769 7468 207a 0820 636c 6173 7365 737a  with z. classesz
-00001bd0: 5542 6f74 6820 616e 2065 6e63 6f64 6572  UBoth an encoder
-00001be0: 2061 6e64 206b 2d64 2074 7265 6573 2065   and k-d trees e
-00001bf0: 6e61 626c 6564 2e20 5573 696e 6720 7468  nabled. Using th
-00001c00: 6520 656e 636f 6465 7220 666f 7220 7468  e encoder for th
-00001c10: 6520 7072 6f74 6f74 7970 6520 6c6f 7373  e prototype loss
-00001c20: 2074 6572 6d2e 2901 da0d 656e 635f 6f72   term.)...enc_or
-00001c30: 5f6b 6474 7265 6529 01da 0669 735f 6361  _kdtree)...is_ca
-00001c40: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
-00001c50: 0000 0700 0000 1300 0000 734e 0000 0067  ..........sN...g
-00001c60: 007c 005d 467d 0174 0088 007c 0119 0074  .|.]F}.t...|...t
-00001c70: 0183 0272 3c74 02a0 0388 0164 0064 0185  ...r<t.....d.d..
-00001c80: 0219 00a1 0188 007c 0119 0014 0064 0164  .......|.....d.d
-00001c90: 0164 0185 0266 0219 006e 0c74 02a0 0488  .d...f...n.t....
-00001ca0: 007c 0119 00a1 0191 0271 0453 0029 0272  .|.......q.S.).r
-00001cb0: 1a00 0000 4e29 05da 0a69 7369 6e73 7461  ....N)...isinsta
-00001cc0: 6e63 65da 0566 6c6f 6174 da02 6e70 da04  nce..float..np..
-00001cd0: 6f6e 6573 da05 6172 7261 7929 02da 022e  ones..array)....
-00001ce0: 30da 015f 2902 7220 0000 0072 1d00 0000  0.._).r ...r....
-00001cf0: a900 fa50 2f63 656e 7472 616c 2f68 6f6d  ...P/central/hom
-00001d00: 652f 7a77 616e 6732 2f6d 6f72 7068 6575  e/zwang2/morpheu
-00001d10: 732d 7370 6174 6961 6c2f 6d6f 7270 6865  s-spatial/morphe
-00001d20: 7573 2f73 7263 2f6d 6f72 7068 6575 732f  us/src/morpheus/
-00001d30: 636f 756e 7465 7266 6163 7475 616c 2f63  counterfactual/c
-00001d40: 662e 7079 da0a 3c6c 6973 7463 6f6d 703e  f.py..<listcomp>
-00001d50: bd00 0000 7308 0000 0006 0602 fd0c ff28  ....s..........(
-00001d60: 027a 2b43 6f75 6e74 6572 6661 6374 7561  .z+Counterfactua
-00001d70: 6c2e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  l.__init__.<loca
-00001d80: 6c73 3e2e 3c6c 6973 7463 6f6d 703e da04  ls>.<listcomp>..
-00001d90: 6f72 6967 2902 da05 6474 7970 65da 046e  orig)...dtype..n
-00001da0: 616d 65da 0361 6476 da05 6164 765f 73da  ame..adv..adv_s.
-00001db0: 0674 6172 6765 74da 0c74 6172 6765 745f  .target..target_
-00001dc0: 7072 6f74 6fda 0563 6f6e 7374 720f 0000  proto..constr...
-00001dd0: 00da 0b67 6c6f 6261 6c5f 7374 6570 2902  ...global_step).
-00001de0: 5a09 7472 6169 6e61 626c 6572 4900 0000  Z.trainablerI...
-00001df0: da0b 6173 7369 676e 5f6f 7269 67a9 0172  ..assign_orig..r
-00001e00: 4900 0000 da0a 6173 7369 676e 5f61 6476  I.....assign_adv
-00001e10: da0c 6173 7369 676e 5f61 6476 5f73 da0d  ..assign_adv_s..
-00001e20: 6173 7369 676e 5f74 6172 6765 74da 0c61  assign_target..a
-00001e30: 7373 6967 6e5f 636f 6e73 74da 1361 7373  ssign_const..ass
-00001e40: 6967 6e5f 7461 7267 6574 5f70 726f 746f  ign_target_proto
-00001e50: 5a16 7368 7269 6e6b 6167 655f 7468 7265  Z.shrinkage_thre
-00001e60: 7368 6f6c 6469 6e67 5a0e 7065 7274 7572  sholdingZ.pertur
-00001e70: 6261 7469 6f6e 5f79 e903 0000 005a 0a75  bation_y.....Z.u
-00001e80: 7064 6174 655f 6164 765a 0c75 7064 6174  pdate_advZ.updat
-00001e90: 655f 6465 6c74 61da 0a6c 6f73 735f 6c31  e_delta..loss_l1
-00001ea0: 5f6c 32a9 01da 0461 7869 73da 076c 6f73  _l2....axis..los
-00001eb0: 735f 6165 da0b 6c6f 7373 5f61 7474 6163  s_ae..loss_attac
-00001ec0: 6be9 1027 0000 5a0e 6c6f 7373 5f70 726f  k..'..Z.loss_pro
-00001ed0: 746f 7479 7065 5a0d 6c6f 7373 5f63 6f6d  totypeZ.loss_com
-00001ee0: 6269 6e65 64da 0874 7261 696e 696e 6767  bined..trainingg
-00001ef0: 0000 0000 0000 e03f 2901 da05 706f 7765  .......?)...powe
-00001f00: 7263 0100 0000 0000 0000 0000 0000 0200  rc..............
-00001f10: 0000 0200 0000 7300 0000 7314 0000 007c  ......s...s....|
-00001f20: 005d 0c7d 017c 016a 0056 0001 0071 0264  .].}.|.j.V...q.d
-00001f30: 0053 0029 014e 7251 0000 00a9 0272 4200  .S.).NrQ.....rB.
-00001f40: 0000 da01 7872 4400 0000 7244 0000 0072  ....xrD...rD...r
-00001f50: 4500 0000 da09 3c67 656e 6578 7072 3ea9  E.....<genexpr>.
-00001f60: 0100 00f3 0000 0000 7a2a 436f 756e 7465  ........z*Counte
-00001f70: 7266 6163 7475 616c 2e5f 5f69 6e69 745f  rfactual.__init_
-00001f80: 5f2e 3c6c 6f63 616c 733e 2e3c 6765 6e65  _.<locals>.<gene
-00001f90: 7870 723e 2901 da08 7661 725f 6c69 7374  xpr>)...var_list
-00001fa0: 5a0a 6772 6164 5f61 6476 5f73 6301 0000  Z.grad_adv_sc...
-00001fb0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00001fc0: 0053 0000 0073 1c00 0000 6700 7c00 5d14  .S...s....g.|.].
-00001fd0: 7d01 7c01 6a00 a001 6400 a101 7204 7c01  }.|.j...d...r.|.
-00001fe0: 9102 7104 5300 2901 724b 0000 0029 0272  ..q.S.).rK...).r
-00001ff0: 4900 0000 da0a 7374 6172 7473 7769 7468  I.....startswith
-00002000: 2902 7242 0000 005a 0474 7661 7272 4400  ).rB...Z.tvarrD.
-00002010: 0000 7244 0000 0072 4500 0000 7246 0000  ..rD...rE...rF..
-00002020: 00b0 0100 0073 0600 0000 0602 0201 0cfe  .....s..........
-00002030: 2901 724f 0000 0063 0100 0000 0000 0000  ).rO...c........
-00002040: 0000 0000 0200 0000 0400 0000 1300 0000  ................
-00002050: 731a 0000 0067 007c 005d 127d 017c 016a  s....g.|.].}.|.j
-00002060: 0088 0076 0172 047c 0191 0271 0453 0072  ...v.r.|...q.S.r
-00002070: 4400 0000 7251 0000 0072 6000 0000 2901  D...rQ...r`...).
-00002080: da0a 7374 6172 745f 7661 7273 7244 0000  ..start_varsrD..
-00002090: 0072 4500 0000 7246 0000 00bd 0100 0072  .rE...rF.......r
-000020a0: 6300 0000 2991 da05 7375 7065 72da 085f  c...)...super.._
-000020b0: 5f69 6e69 745f 5fda 0463 6f70 79da 0864  _init__..copy..d
-000020c0: 6565 7063 6f70 7972 0900 0000 da03 6c65  eepcopyr......le
-000020d0: 6eda 066c 6f63 616c 73da 0370 6f70 7232  n..locals..popr2
-000020e0: 0000 00da 0675 7064 6174 6572 1b00 0000  .....updater....
-000020f0: 722d 0000 0072 3d00 0000 da02 7466 da05  r-...r=.....tf..
-00002100: 6b65 7261 73da 054d 6f64 656c da06 636f  keras..Model..co
-00002110: 6d70 6174 da02 7631 da07 6261 636b 656e  mpat..v1..backen
-00002120: 645a 0b67 6574 5f73 6573 7369 6f6e da07  dZ.get_session..
-00002130: 5365 7373 696f 6e72 2f00 0000 da05 6d6f  Sessionr/.....mo
-00002140: 6465 6c72 3f00 0000 da05 7a65 726f 7372  delr?.....zerosr
-00002150: 1d00 0000 da07 636c 6173 7365 73da 0574  ......classes..t
-00002160: 6f72 6368 da05 7072 696e 7472 2300 0000  orch..printr#...
-00002170: 7222 0000 00da 066c 6f67 6765 72da 0777  r".....logger..w
-00002180: 6172 6e69 6e67 723b 0000 00da 0b70 6174  arningr;.....pat
-00002190: 6368 5f73 6861 7065 721e 0000 0072 1f00  ch_shaper....r..
-000021a0: 0000 7221 0000 0072 2400 0000 da02 6165  ..r!...r$.....ae
-000021b0: da03 656e 6372 2500 0000 da0a 6261 7463  ..encr%.....batc
-000021c0: 685f 7369 7a65 7227 0000 0072 2800 0000  h_sizer'...r(...
-000021d0: 7229 0000 00da 0574 7570 6c65 da05 7261  r).....tuple..ra
-000021e0: 6e67 6572 2000 0000 722c 0000 0072 2a00  nger ...r,...r*.
-000021f0: 0000 722b 0000 0072 1c00 0000 722e 0000  ..r+...r....r...
-00002200: 0072 3000 0000 da08 5661 7269 6162 6c65  .r0.....Variable
-00002210: da07 666c 6f61 7433 3272 4700 0000 724a  ..float32rG...rJ
-00002220: 0000 0072 4b00 0000 724c 0000 00da 0973  ...rK...rL.....s
-00002230: 6861 7065 5f65 6e63 724d 0000 0072 4e00  hape_encrM...rN.
-00002240: 0000 724f 0000 00da 0b70 6c61 6365 686f  ..rO.....placeho
-00002250: 6c64 6572 7250 0000 0072 5200 0000 7253  lderrP...rR...rS
-00002260: 0000 0072 5400 0000 7255 0000 0072 5600  ...rT...rU...rV.
-00002270: 0000 5a0a 6e61 6d65 5f73 636f 7065 da04  ..Z.name_scope..
-00002280: 6361 7374 da07 6772 6561 7465 72da 0873  cast..greater..s
-00002290: 7562 7472 6163 74da 0a6c 6573 735f 6571  ubtract..less_eq
-000022a0: 7561 6cda 0361 6273 da04 6c65 7373 da08  ual..abs..less..
-000022b0: 6e65 6761 7469 7665 da07 6d69 6e69 6d75  negative..minimu
-000022c0: 6dda 076d 6178 696d 756d da03 6164 64da  m..maximum..add.
-000022d0: 086d 756c 7469 706c 79da 0664 6976 6964  .multiply..divid
-000022e0: 65da 027a 74da 0661 7373 6967 6eda 0b61  e..zt..assign..a
-000022f0: 6476 5f75 7064 6174 6572 da0d 6164 765f  dv_updater..adv_
-00002300: 7570 6461 7465 725f 73da 0564 656c 7461  updater_s..delta
-00002310: da07 6465 6c74 615f 73da 046c 6973 74da  ..delta_s..list.
-00002320: 0661 7261 6e67 65da 0a72 6564 7563 655f  .arange..reduce_
-00002330: 7375 6dda 0673 7175 6172 65da 026c 325a  sum..square..l2Z
-00002340: 046c 325f 73da 026c 315a 046c 315f 73da  .l2_s..l1Z.l1_s.
-00002350: 056c 315f 6c32 5a07 6c31 5f6c 325f 73da  .l1_l2Z.l1_l2_s.
-00002360: 076c 6f73 735f 6c31 5a09 6c6f 7373 5f6c  .loss_l1Z.loss_l
-00002370: 315f 73da 076c 6f73 735f 6c32 5a09 6c6f  1_s..loss_l2Z.lo
-00002380: 7373 5f6c 325f 735a 0761 6476 5f63 6174  ss_l2_sZ.adv_cat
-00002390: 5a09 6164 765f 6361 745f 735a 0661 6476  Z.adv_cat_sZ.adv
-000023a0: 5f61 655a 0861 6476 5f61 655f 73da 046e  _aeZ.adv_ae_s..n
-000023b0: 6f72 6d72 5b00 0000 5a09 6c6f 7373 5f61  ormr[...Z.loss_a
-000023c0: 655f 73da 0863 6f6e 7374 616e 7472 5c00  e_s..constantr\.
-000023d0: 0000 da0a 7072 6564 5f70 726f 6261 5a0c  ....pred_probaZ.
-000023e0: 7072 6564 5f70 726f 6261 5f73 da0d 6c6f  pred_proba_s..lo
-000023f0: 7373 5f61 7474 6163 6b5f 73da 0c74 6172  ss_attack_s..tar
-00002400: 6765 745f 7072 6f62 615a 0a72 6564 7563  get_probaZ.reduc
-00002410: 655f 6d61 78da 136e 6f6e 7461 7267 6574  e_max..nontarget
-00002420: 5f70 726f 6261 5f6d 6178 da0a 6c6f 7373  _proba_max..loss
-00002430: 5f70 726f 746f 5a0c 6c6f 7373 5f70 726f  _protoZ.loss_pro
-00002440: 746f 5f73 da08 6c6f 7373 5f6f 7074 da0a  to_s..loss_opt..
-00002450: 6c6f 7373 5f74 6f74 616c da05 7472 6169  loss_total..trai
-00002460: 6e5a 1070 6f6c 796e 6f6d 6961 6c5f 6465  nZ.polynomial_de
-00002470: 6361 79da 0d6c 6561 726e 696e 675f 7261  cay..learning_ra
-00002480: 7465 5a18 4772 6164 6965 6e74 4465 7363  teZ.GradientDesc
-00002490: 656e 744f 7074 696d 697a 6572 da03 7365  entOptimizer..se
-000024a0: 745a 1067 6c6f 6261 6c5f 7661 7269 6162  tZ.global_variab
-000024b0: 6c65 735a 1163 6f6d 7075 7465 5f67 7261  lesZ.compute_gra
-000024c0: 6469 656e 7473 da0d 636f 6d70 7574 655f  dients..compute_
-000024d0: 6772 6164 73da 0767 7261 645f 7068 5a13  grads..grad_phZ.
-000024e0: 7472 6169 6e61 626c 655f 7661 7269 6162  trainable_variab
-000024f0: 6c65 735a 0f61 7070 6c79 5f67 7261 6469  lesZ.apply_gradi
-00002500: 656e 7473 da0b 6170 706c 795f 6772 6164  ents..apply_grad
-00002510: 73da 0573 6574 7570 da06 6170 7065 6e64  s..setup..append
-00002520: 5a15 7661 7269 6162 6c65 735f 696e 6974  Z.variables_init
-00002530: 6961 6c69 7a65 72da 0469 6e69 74da 0773  ializer..init..s
-00002540: 756d 6d61 7279 5a0a 4669 6c65 5772 6974  ummaryZ.FileWrit
-00002550: 6572 5a11 6765 745f 6465 6661 756c 745f  erZ.get_default_
-00002560: 6772 6170 68da 0677 7269 7465 72da 0961  graph..writer..a
-00002570: 6464 5f67 7261 7068 292d 7234 0000 0072  dd_graph)-r4...r
-00002580: 1b00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
-00002590: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
-000025a0: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
-000025b0: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
-000025c0: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
-000025d0: 2b00 0000 722c 0000 0072 2d00 0000 722e  +...r,...r-...r.
-000025e0: 0000 0072 2f00 0000 7230 0000 0072 7d00  ...r/...r0...r}.
-000025f0: 0000 7236 0000 00da 0672 656d 6f76 65da  ..r6.....remove.
-00002600: 036b 6579 7237 0000 005a 0a6d 6f64 656c  .keyr7...Z.model
-00002610: 5f73 6573 7372 3800 0000 7239 0000 00da  _sessr8...r9....
-00002620: 0573 636f 7065 da04 636f 6e64 da05 7570  .scope..cond..up
-00002630: 7065 72da 056c 6f77 6572 5a06 6178 5f73  per..lowerZ.ax_s
-00002640: 756d 5a0e 7461 7267 6574 5f70 726f 6261  umZ.target_proba
-00002650: 5f73 5a15 6e6f 6e74 6172 6765 745f 7072  _sZ.nontarget_pr
-00002660: 6f62 615f 6d61 785f 7372 5c00 0000 72a5  oba_max_sr\...r.
-00002670: 0000 00da 096f 7074 696d 697a 6572 da03  .....optimizer..
-00002680: 7661 725a 0c67 7261 645f 616e 645f 7661  varZ.grad_and_va
-00002690: 725a 0865 6e64 5f76 6172 735a 086e 6577  rZ.end_varsZ.new
-000026a0: 5f76 6172 73a9 0172 3500 0000 2903 7220  _vars..r5...).r 
-000026b0: 0000 0072 1d00 0000 7266 0000 0072 4500  ...r....rf...rE.
-000026c0: 0000 7268 0000 0018 0000 0073 1a02 0000  ..rh.......s....
-000026d0: 004f 1403 0c01 0201 06ff 0403 1202 0401  .O..............
-000026e0: 0601 0809 0801 0c01 1002 0601 0603 0e01  ................
-000026f0: 1001 0e01 0e01 1603 0c01 0802 0602 0601  ................
-00002700: 0601 1c02 0601 1a01 1202 0601 0802 0602  ................
-00002710: 0601 0802 0602 0e01 0401 02ff 0404 0e01  ................
-00002720: 0802 0601 1402 1202 0601 0601 0601 0601  ................
-00002730: 0601 0601 0601 0602 0601 0a01 0601 0601  ................
-00002740: 0601 0201 0c06 06fa 04ff 060a 0601 0601  ................
-00002750: 0601 0601 0601 0603 1a01 1a01 1a01 0401  ................
-00002760: 16ff 0806 0801 1a03 0803 0401 10ff 0805  ................
-00002770: 0401 10ff 0803 1203 1401 1401 1401 0401  ................
-00002780: 10ff 0803 0401 0cff 0803 0401 0aff 0806  ................
-00002790: 0e02 0401 1801 04fe 0204 0401 0401 18ff  ................
-000027a0: 0203 04fc 0206 0401 1e01 04fe 02f5 0410  ................
-000027b0: 0401 0e01 10fe 0404 0401 1eff 0404 0e01  ................
-000027c0: 10ff 0202 0efe 02ff 2407 0c01 0401 16ff  ........$.......
-000027d0: 0603 0801 0eff 0804 0401 14ff 0603 0401  ................
-000027e0: 14ff 2605 0c01 1201 3203 0c01 0e01 2e03  ..&.....2.......
-000027f0: 1401 0c01 1801 1801 1801 1801 1801 1803  ................
-00002800: 0e01 0e01 0e01 2e02 0801 0802 0c02 0802  ................
-00002810: 0e01 0e02 2001 0801 10ff 0a04 0c01 2c02  .... .........,.
-00002820: 0e01 0801 1202 08ff 0401 08ff 0404 0e01  ................
-00002830: 0e02 0c01 0e03 0e01 0e03 1601 1403 0401  ................
-00002840: 1aff 0603 0401 1aff 0405 0401 14ff 0403  ................
-00002850: 0401 10ff 0405 1201 3202 0c02 0801 0801  ........2.......
-00002860: 16ff 0803 0801 16ff 0a03 0801 0801 10ff  ................
-00002870: 0803 0801 10ff 0a04 0c01 2c02 0c02 0802  ..........,.....
-00002880: 0401 04ff 0202 04fe 0203 04fd 02ff 0607  ................
-00002890: 1404 0401 04ff 0202 04fe 0203 0efd 0204  ................
-000028a0: 04fc 02ff 2408 0c01 0601 0eff 0803 0e01  ....$...........
-000028b0: 1603 0401 0aff 0803 1201 0602 06fe 0405  ................
-000028c0: 02fb 0408 0c01 0401 06ff 0803 0801 3203  ..............2.
-000028d0: 0601 1601 1601 1601 1601 1601 1605 0401  ................
-000028e0: 1aff 0804 0c01 1401 1202 7a17 436f 756e  ..........z.Coun
-000028f0: 7465 7266 6163 7475 616c 2e5f 5f69 6e69  terfactual.__ini
-00002900: 745f 5f29 04da 0a74 7261 696e 5f64 6174  t__)...train_dat
-00002910: 61da 0570 7265 6473 da11 7472 7573 7473  a..preds..trusts
-00002920: 636f 7265 5f6b 7761 7267 7372 3100 0000  core_kwargsr1...
-00002930: 6304 0000 0000 0000 0000 0000 000b 0000  c...............
-00002940: 0006 0000 0043 0000 0073 c800 0000 7400  .....C...s....t.
-00002950: 8300 7d04 6401 6402 6702 7d05 7c05 4400  ..}.d.d.g.}.|.D.
-00002960: 5d0e 7d06 7c04 a001 7c06 a101 0100 7112  ].}.|...|.....q.
-00002970: 7c00 6a02 6403 1900 a003 7c04 a101 0100  |.j.d.....|.....
-00002980: 7c00 6a04 72a4 7c00 6a05 a006 7c01 a101  |.j.r.|.j...|...
-00002990: 7d07 6900 7c00 5f07 6900 7c00 5f08 7409  }.i.|._.i.|._.t.
-000029a0: 7c00 6a0a 8301 4400 5d46 7d08 740b a00c  |.j...D.]F}.t...
-000029b0: 7c02 7c08 6b02 a101 6404 1900 7d09 740b  |.|.k...d...}.t.
-000029c0: 6a0d 740b 6a0e 7c07 7c09 1900 6404 6405  j.t.j.|.|...d.d.
-000029d0: 8d02 6404 6405 8d02 7c00 6a07 7c08 3c00  ..d.d...|.j.|.<.
-000029e0: 7c07 7c09 1900 7c00 6a08 7c08 3c00 715a  |.|...|.j.|.<.qZ
-000029f0: 6e20 7c00 6a0f 72c4 7410 7c00 6a11 8301  n |.j.r.t.|.j...
-00002a00: 7d0a 7c0a 6a12 7c00 5f12 7c0a 6a13 7c00  }.|.j.|._.|.j.|.
-00002a10: 5f14 7c00 5300 2906 6188 0100 000a 2020  _.|.S.).a.....  
-00002a20: 2020 2020 2020 4765 7420 7072 6f74 6f74        Get protot
-00002a30: 7970 6573 2066 6f72 2065 6163 6820 636c  ypes for each cl
-00002a40: 6173 7320 7573 696e 6720 7468 6520 656e  ass using the en
-00002a50: 636f 6465 7220 6f72 206b 2d64 2074 7265  coder or k-d tre
-00002a60: 6573 2e0a 2020 2020 2020 2020 5468 6520  es..        The 
-00002a70: 7072 6f74 6f74 7970 6573 2061 7265 2075  prototypes are u
-00002a80: 7365 6420 666f 7220 7468 6520 656e 636f  sed for the enco
-00002a90: 6465 7220 6c6f 7373 2074 6572 6d20 6f72  der loss term or
-00002aa0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
-00002ab0: 6520 6f70 7469 6f6e 616c 2074 7275 7374  e optional trust
-00002ac0: 2073 636f 7265 732e 0a0a 2020 2020 2020   scores...      
-00002ad0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00002ae0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-00002af0: 2020 2020 2020 2020 7472 6169 6e5f 6461          train_da
-00002b00: 7461 0a20 2020 2020 2020 2020 2020 2052  ta.            R
-00002b10: 6570 7265 7365 6e74 6174 6976 6520 7361  epresentative sa
-00002b20: 6d70 6c65 2066 726f 6d20 7468 6520 7472  mple from the tr
-00002b30: 6169 6e69 6e67 2064 6174 612e 0a20 2020  aining data..   
-00002b40: 2020 2020 2074 7275 7374 7363 6f72 655f       trustscore_
-00002b50: 6b77 6172 6773 0a20 2020 2020 2020 2020  kwargs.         
-00002b60: 2020 204f 7074 696f 6e61 6c20 6172 6775     Optional argu
-00002b70: 6d65 6e74 7320 746f 2069 6e69 7469 616c  ments to initial
-00002b80: 697a 6520 7468 6520 7472 7573 7420 7363  ize the trust sc
-00002b90: 6f72 6573 206d 6574 686f 642e 0a20 2020  ores method..   
-00002ba0: 2020 2020 2072 3400 0000 72c0 0000 0072       r4...r....r
-00002bb0: 3600 0000 7201 0000 0072 5900 0000 2915  6...r....rY...).
-00002bc0: 726c 0000 0072 6d00 0000 7232 0000 0072  rl...rm...r2...r
-00002bd0: 6e00 0000 7223 0000 0072 7f00 0000 721b  n...r#...r....r.
-00002be0: 0000 00da 0b63 6c61 7373 5f70 726f 746f  .....class_proto
-00002bf0: da09 636c 6173 735f 656e 6372 8200 0000  ..class_encr....
-00002c00: 7278 0000 0072 3f00 0000 da05 7768 6572  rx...r?.....wher
-00002c10: 65da 0b65 7870 616e 645f 6469 6d73 da04  e..expand_dims..
-00002c20: 6d65 616e 7225 0000 00da 0b6c 6f61 645f  meanr%.....load_
-00002c30: 6f62 6a65 6374 722d 0000 00da 076b 6474  objectr-.....kdt
-00002c40: 7265 6573 5a08 585f 6b64 7472 6565 da0a  reesZ.X_kdtree..
-00002c50: 585f 6279 5f63 6c61 7373 290b 7234 0000  X_by_class).r4..
-00002c60: 0072 c000 0000 72c1 0000 0072 c200 0000  .r....r....r....
-00002c70: 7236 0000 0072 b700 0000 72b8 0000 005a  r6...r....r....Z
-00002c80: 0865 6e63 5f64 6174 61da 0169 da03 6964  .enc_data..i..id
-00002c90: 78da 0274 7372 4400 0000 7244 0000 0072  x..tsrD...rD...r
-00002ca0: 4500 0000 da03 6669 74d5 0100 0073 2800  E.....fit....s(.
-00002cb0: 0000 0012 0601 0801 0801 0c02 1002 0601  ................
-00002cc0: 0c01 0601 0601 0e01 1201 0401 12ff 0c03  ................
-00002cd0: 1201 0601 0a01 0801 0801 7a12 436f 756e  ..........z.Coun
-00002ce0: 7465 7266 6163 7475 616c 2e66 6974 2903  terfactual.fit).
-00002cf0: 72a4 0000 00da 0159 7231 0000 0063 0300  r......Yr1...c..
-00002d00: 0000 0000 0000 0000 0000 0700 0000 0500  ................
-00002d10: 0000 4300 0000 735e 0000 0074 00a0 017c  ..C...s^...t...|
-00002d20: 017c 0214 00a1 017d 0374 00a0 0264 017c  .|.....}.t...d.|
-00002d30: 0218 007c 0114 0064 027c 0214 0018 00a1  ...|...d.|......
-00002d40: 017d 0474 00a0 0364 037c 040b 007c 0317  .}.t...d.|...|..
-00002d50: 007c 006a 0417 00a1 027d 0574 00a0 017c  .|.j.....}.t...|
-00002d60: 006a 056a 067c 006a 0764 048d 017c 0514  .j.j.|.j.d...|..
-00002d70: 00a1 017d 067c 0653 0029 0561 1701 0000  ...}.|.S.).a....
-00002d80: 0a20 2020 2020 2020 2043 6f6d 7075 7465  .        Compute
-00002d90: 2074 6865 2061 7474 6163 6b20 6c6f 7373   the attack loss
-00002da0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00002db0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00002dc0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00002dd0: 2070 7265 645f 7072 6f62 610a 2020 2020   pred_proba.    
-00002de0: 2020 2020 2020 2020 5072 6564 6963 7469          Predicti
-00002df0: 6f6e 2070 726f 6261 6269 6c69 7469 6573  on probabilities
-00002e00: 206f 6620 616e 2069 6e73 7461 6e63 652e   of an instance.
-00002e10: 0a20 2020 2020 2020 2059 0a20 2020 2020  .        Y.     
-00002e20: 2020 2020 2020 204f 6e65 2d68 6f74 2072         One-hot r
-00002e30: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
-00002e40: 2069 6e73 7461 6e63 6520 6c61 6265 6c73   instance labels
-00002e50: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00002e60: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00002e70: 2d2d 0a20 2020 2020 2020 204c 6f73 7320  --.        Loss 
-00002e80: 6f66 2074 6865 2061 7474 6163 6b2e 0a20  of the attack.. 
-00002e90: 2020 2020 2020 2072 1a00 0000 725d 0000         r....r]..
-00002ea0: 0072 0f00 0000 a901 da07 7365 7373 696f  .r........sessio
-00002eb0: 6e29 0872 3f00 0000 da03 7375 6dda 036d  n).r?.....sum..m
-00002ec0: 6178 728f 0000 0072 1e00 0000 724e 0000  axr....r....rN..
-00002ed0: 00da 0465 7661 6c72 2f00 0000 2907 7234  ...evalr/...).r4
-00002ee0: 0000 0072 a400 0000 72cf 0000 0072 a600  ...r....r....r..
-00002ef0: 0000 72a7 0000 00da 046c 6f73 7372 5c00  ..r......lossr\.
-00002f00: 0000 7244 0000 0072 4400 0000 7245 0000  ..rD...rD...rE..
-00002f10: 00da 076c 6f73 735f 666e fe01 0000 730a  ...loss_fn....s.
-00002f20: 0000 0000 100e 021a 0218 021a 017a 1643  .............z.C
-00002f30: 6f75 6e74 6572 6661 6374 7561 6c2e 6c6f  ounterfactual.lo
-00002f40: 7373 5f66 6e29 04da 0158 72cf 0000 00da  ss_fn)...Xr.....
-00002f50: 0b67 7261 6473 5f73 6861 7065 7231 0000  .grads_shaper1..
-00002f60: 0063 0400 0000 0000 0000 0000 0000 1500  .c..............
-00002f70: 0000 0600 0000 0300 0000 73e8 0100 0074  ..........s....t
-00002f80: 00a0 017c 01a1 017d 047c 00a0 027c 04a1  ...|...}.|...|..
-00002f90: 01a0 03a1 00a0 04a1 007d 0574 057c 057c  .........}.t.|.|
-00002fa0: 006a 0664 0119 0064 0264 038d 035c 027d  .j.d...d.d...\.}
-00002fb0: 067d 0787 0066 0164 0464 0584 087d 0887  .}...f.d.d...}..
-00002fc0: 0066 0164 0664 0784 087d 0974 07a0 087c  .f.d.d...}.t...|
-00002fd0: 087c 0583 017c 097c 0583 0118 007c 006a  .|...|.|.....|.j
-00002fe0: 090b 006b 01a1 0164 0119 007d 0a74 0a7c  ...k...d...}.t.|
-00002ff0: 0a83 017c 016a 0b64 0119 006b 0272 9c74  ...|.j.d...k.r.t
-00003000: 07a0 0c64 0867 017c 016a 0b64 0864 0985  ...d.g.|.j.d.d..
-00003010: 0219 00a2 0152 00a1 0153 007c 087c 0683  .....R...S.|.|..
-00003020: 017c 087c 0783 0118 007d 0b7c 097c 0683  .|.|.....}.|.|..
-00003030: 017c 097c 0783 0118 007d 0c7c 0b7c 0c18  .|.|.....}.|.|..
-00003040: 007d 0d74 07a0 0d7c 0d7c 016a 0b64 0119  .}.t...|.|.j.d..
-00003050: 0064 0a66 02a1 0264 0b7c 006a 0664 0119  .d.f...d.|.j.d..
-00003060: 0014 001b 007d 0d74 057c 017c 006a 0664  .....}.t.|.|.j.d
-00003070: 0819 0064 0c64 038d 035c 027d 0e7d 0f74  ...d.d...\.}.}.t
-00003080: 076a 0e7c 0e7c 0f67 0264 0164 0d8d 027d  .j.|.|.g.d.d...}
-00003090: 107c 00a0 0274 00a0 017c 10a1 01a1 01a0  .|...t...|......
-000030a0: 03a1 00a0 04a1 007d 117c 0e6a 0b64 0119  .......}.|.j.d..
-000030b0: 007d 127c 1164 097c 1285 0219 007c 117c  .}.|.d.|.....|.|
-000030c0: 1264 0985 0219 0018 007d 1374 076a 0d74  .d.......}.t.j.t
-000030d0: 07a0 0d7c 137c 016a 0b64 0119 0064 0a66  ...|.|.j.d...d.f
-000030e0: 02a1 027c 016a 0b64 0119 007c 056a 0b64  ...|.j.d...|.j.d
-000030f0: 0819 0064 0a66 0364 0e64 0f8d 0364 0b7c  ...d.f.d.d...d.|
-00003100: 006a 0664 0819 0014 001b 007d 1374 07a0  .j.d.......}.t..
-00003110: 0f64 107c 0d7c 13a1 037d 1474 0a7c 0a83  .d.|.|...}.t.|..
-00003120: 0164 016b 0490 0172 c274 07a0 0c7c 146a  .d.k...r.t...|.j
-00003130: 0b64 0864 0985 0219 00a1 017c 147c 0a3c  .d.d.......|.|.<
-00003140: 0074 076a 107c 1464 0164 0d8d 027d 1474  .t.j.|.d.d...}.t
-00003150: 07a0 0d7c 147c 006a 1166 017c 0317 00a1  ...|.|.j.f.|....
-00003160: 027d 147c 1453 0029 1161 b801 0000 0a20  .}.|.S.).a..... 
-00003170: 2020 2020 2020 2043 6f6d 7075 7465 206e         Compute n
-00003180: 756d 6572 6963 616c 2067 7261 6469 656e  umerical gradien
-00003190: 7473 206f 6620 7468 6520 6174 7461 636b  ts of the attack
-000031a0: 206c 6f73 7320 7465 726d 3a0a 2020 2020   loss term:.    
-000031b0: 2020 2020 6064 4c2f 6478 203d 2028 644c      `dL/dx = (dL
-000031c0: 2f64 5029 2a28 6450 2f64 7829 6020 7769  /dP)*(dP/dx)` wi
-000031d0: 7468 2060 4c20 3d20 6c6f 7373 5f61 7474  th `L = loss_att
-000031e0: 6163 6b5f 733b 2050 203d 2070 7265 6469  ack_s; P = predi
-000031f0: 6374 3b20 7820 3d20 6164 765f 7360 2e0a  ct; x = adv_s`..
-00003200: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00003210: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00003220: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2058  ------.        X
-00003230: 0a20 2020 2020 2020 2020 2020 2049 6e73  .            Ins
-00003240: 7461 6e63 6520 6172 6f75 6e64 2077 6869  tance around whi
-00003250: 6368 2067 7261 6469 656e 7420 6973 2065  ch gradient is e
-00003260: 7661 6c75 6174 6564 2e0a 2020 2020 2020  valuated..      
-00003270: 2020 590a 2020 2020 2020 2020 2020 2020    Y.            
-00003280: 4f6e 652d 686f 7420 7265 7072 6573 656e  One-hot represen
-00003290: 7461 7469 6f6e 206f 6620 696e 7374 616e  tation of instan
-000032a0: 6365 206c 6162 656c 732e 0a20 2020 2020  ce labels..     
-000032b0: 2020 2067 7261 6473 5f73 6861 7065 0a20     grads_shape. 
-000032c0: 2020 2020 2020 2020 2020 2053 6861 7065             Shape
-000032d0: 206f 6620 6772 6164 6965 6e74 732e 0a0a   of gradients...
-000032e0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-000032f0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-00003300: 2020 2020 2020 2020 4172 7261 7920 7769          Array wi
-00003310: 7468 2067 7261 6469 656e 7473 2e0a 2020  th gradients..  
-00003320: 2020 2020 2020 7201 0000 0054 2901 da05        r....T)...
-00003330: 7072 6f62 6163 0100 0000 0000 0000 0000  probac..........
-00003340: 0000 0100 0000 0400 0000 1300 0000 7312  ..............s.
-00003350: 0000 0074 006a 0188 007c 0014 0064 0164  ...t.j...|...d.d
-00003360: 028d 0253 00a9 034e 721a 0000 0072 5900  ...S...Nr....rY.
-00003370: 0000 2902 723f 0000 0072 d200 0000 a901  ..).r?...r......
-00003380: 5a0a 7072 6564 735f 7065 7274 a901 72cf  Z.preds_pert..r.
-00003390: 0000 0072 4400 0000 7245 0000 00da 0166  ...rD...rE.....f
-000033a0: 3302 0000 7302 0000 0000 017a 2743 6f75  3...s......z'Cou
-000033b0: 6e74 6572 6661 6374 7561 6c2e 6765 745f  nterfactual.get_
-000033c0: 6772 6164 6965 6e74 732e 3c6c 6f63 616c  gradients.<local
-000033d0: 733e 2e66 6301 0000 0000 0000 0000 0000  s>.fc...........
-000033e0: 0001 0000 0004 0000 0013 0000 0073 1600  .............s..
-000033f0: 0000 7400 6a01 6401 8800 1800 7c00 1400  ..t.j.d.....|...
-00003400: 6401 6402 8d02 5300 72da 0000 0029 0272  d.d...S.r....).r
-00003410: 3f00 0000 72d3 0000 0072 db00 0000 72dc  ?...r....r....r.
-00003420: 0000 0072 4400 0000 7245 0000 00da 0167  ...rD...rE.....g
-00003430: 3602 0000 7302 0000 0000 017a 2743 6f75  6...s......z'Cou
-00003440: 6e74 6572 6661 6374 7561 6c2e 6765 745f  nterfactual.get_
-00003450: 6772 6164 6965 6e74 732e 3c6c 6f63 616c  gradients.<local
-00003460: 733e 2e67 721a 0000 004e 7233 0000 0072  s>.gr....Nr3...r
-00003470: 0700 0000 4672 5900 0000 da01 4629 01da  ....FrY.....F)..
-00003480: 056f 7264 6572 7a0a 696a 2c69 6a6b 2d3e  .orderz.ij,ijk->
-00003490: 696b 2912 7279 0000 00da 0674 656e 736f  ik).ry.....tenso
-000034a0: 7272 1b00 0000 da06 6465 7461 6368 da05  rr......detach..
-000034b0: 6e75 6d70 7972 0d00 0000 722a 0000 0072  numpyr....r*...r
-000034c0: 3f00 0000 72c5 0000 0072 1e00 0000 726b  ?...r....r....rk
-000034d0: 0000 0072 1d00 0000 7277 0000 00da 0772  ...r....rw.....r
-000034e0: 6573 6861 7065 da0b 636f 6e63 6174 656e  eshape..concaten
-000034f0: 6174 65da 0665 696e 7375 6d72 c700 0000  ate..einsumr....
-00003500: 7280 0000 0029 1572 3400 0000 72d7 0000  r....).r4...r...
-00003510: 0072 cf00 0000 72d8 0000 005a 0658 5f70  .r....r....Z.X_p
-00003520: 7265 6472 c100 0000 5a0e 7072 6564 735f  redr....Z.preds_
-00003530: 7065 7274 5f70 6f73 5a0e 7072 6564 735f  pert_posZ.preds_
-00003540: 7065 7274 5f6e 6567 72dd 0000 0072 de00  pert_negr....r..
-00003550: 0000 5a0a 6964 785f 6e6f 6772 6164 5a05  ..Z.idx_nogradZ.
-00003560: 646c 5f64 665a 0564 6c5f 6467 5a05 646c  dl_dfZ.dl_dgZ.dl
-00003570: 5f64 705a 0a58 5f70 6572 745f 706f 735a  _dpZ.X_pert_posZ
-00003580: 0a58 5f70 6572 745f 6e65 675a 0658 5f70  .X_pert_negZ.X_p
-00003590: 6572 745a 0c70 7265 6473 5f63 6f6e 6361  ertZ.preds_conca
-000035a0: 745a 066e 5f70 6572 745a 0564 705f 6478  tZ.n_pertZ.dp_dx
-000035b0: da05 6772 6164 7372 4400 0000 72dc 0000  ..gradsrD...r...
-000035c0: 0072 4500 0000 da0d 6765 745f 6772 6164  .rE.....get_grad
-000035d0: 6965 6e74 7317 0200 0073 4400 0000 0014  ients....sD.....
-000035e0: 0a03 1201 0201 0cff 0a04 0c03 0c04 2201  ..............".
-000035f0: 1201 1c01 1001 1001 0801 2403 0201 0cff  ..........$.....
-00003600: 0a03 1201 1801 0a01 1801 0401 1401 1401  ................
-00003610: 02fd 0405 0cfb 0409 0e02 0e01 1801 0e01  ................
-00003620: 1401 7a1c 436f 756e 7465 7266 6163 7475  ..z.Counterfactu
-00003630: 616c 2e67 6574 5f67 7261 6469 656e 7473  al.get_gradients
-00003640: e7bb bdd7 d9df 7cdb 3d29 0572 d700 0000  ......|.=).r....
-00003650: da09 6164 765f 636c 6173 73da 0a6f 7269  ..adv_class..ori
-00003660: 675f 636c 6173 7372 2a00 0000 7231 0000  g_classr*...r1..
-00003670: 0063 0500 0000 0000 0000 0000 0000 0a00  .c..............
-00003680: 0000 0400 0000 4300 0000 7396 0000 007c  ......C...s....|
-00003690: 006a 0072 487c 006a 01a0 027c 01a1 017d  .j.rH|.j...|...}
-000036a0: 057c 006a 037c 0219 007d 067c 006a 037c  .|.j.|...}.|.j.|
-000036b0: 0319 007d 0774 046a 05a0 067c 057c 0618  ...}.t.j...|.|..
-000036c0: 00a1 017d 0874 046a 05a0 067c 057c 0718  ...}.t.j...|.|..
-000036d0: 00a1 017d 096e 427c 006a 0772 807c 006a  ...}.nB|.j.r.|.j
-000036e0: 087c 0219 006a 0974 0a64 0164 028d 0264  .|...j.t.d.d...d
-000036f0: 0319 007d 087c 006a 087c 0319 006a 0974  ...}.|.j.|...j.t
-00003700: 0a64 0164 028d 0264 0319 007d 096e 0a74  .d.d...d...}.n.t
-00003710: 0ba0 0c64 04a1 0101 007c 097c 087c 0417  ...d.....|.|.|..
-00003720: 001b 0053 0029 0561 f501 0000 0a20 2020  ...S.).a.....   
-00003730: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00003740: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00003750: 2d2d 0a20 2020 2020 2020 2058 0a20 2020  --.        X.   
-00003760: 2020 2020 2020 2020 2050 6572 7475 7262           Perturb
-00003770: 6174 696f 6e2e 0a20 2020 2020 2020 2061  ation..        a
-00003780: 6476 5f63 6c61 7373 0a20 2020 2020 2020  dv_class.       
-00003790: 2020 2020 2050 7265 6469 6374 6564 2063       Predicted c
-000037a0: 6c61 7373 206f 6e20 7468 6520 7065 7274  lass on the pert
-000037b0: 7572 6265 6420 696e 7374 616e 6365 2e0a  urbed instance..
-000037c0: 2020 2020 2020 2020 6f72 6967 5f63 6c61          orig_cla
-000037d0: 7373 0a20 2020 2020 2020 2020 2020 2050  ss.            P
-000037e0: 7265 6469 6374 6564 2063 6c61 7373 206f  redicted class o
-000037f0: 6e20 7468 6520 6f72 6967 696e 616c 2069  n the original i
-00003800: 6e73 7461 6e63 652e 0a20 2020 2020 2020  nstance..       
-00003810: 2065 7073 0a20 2020 2020 2020 2020 2020   eps.           
-00003820: 2053 6d61 6c6c 206e 756d 6265 7220 746f   Small number to
-00003830: 2061 766f 6964 2064 6976 6964 696e 6720   avoid dividing 
-00003840: 6279 2030 2e0a 0a20 2020 2020 2020 2052  by 0...        R
-00003850: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00003860: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2052  ------.        R
-00003870: 6174 696f 2062 6574 7765 656e 2074 6865  atio between the
-00003880: 2064 6973 7461 6e63 6520 746f 2074 6865   distance to the
-00003890: 2070 726f 746f 7479 7065 206f 6620 7468   prototype of th
-000038a0: 6520 7072 6564 6963 7465 6420 636c 6173  e predicted clas
-000038b0: 7320 666f 7220 7468 6520 6f72 6967 696e  s for the origin
-000038c0: 616c 2069 6e73 7461 6e63 6520 616e 6420  al instance and 
-000038d0: 2020 2020 2020 2020 7468 6520 7072 6f74          the prot
-000038e0: 6f74 7970 6520 6f66 2074 6865 2070 7265  otype of the pre
-000038f0: 6469 6374 6564 2063 6c61 7373 2066 6f72  dicted class for
-00003900: 2074 6865 2070 6572 7475 7262 6564 2069   the perturbed i
-00003910: 6e73 7461 6e63 652e 0a20 2020 2020 2020  nstance..       
-00003920: 2072 1a00 0000 a901 da01 6b72 0100 0000   r........kr....
-00003930: 7a4b 4e65 6564 2065 6974 6865 7220 616e  zKNeed either an
-00003940: 2065 6e63 6f64 6572 206f 7220 7468 6520   encoder or the 
-00003950: 6b2d 6420 7472 6565 7320 656e 6162 6c65  k-d trees enable
-00003960: 6420 746f 2063 6f6d 7075 7465 2064 6973  d to compute dis
-00003970: 7461 6e63 6520 7363 6f72 6573 2e29 0d72  tance scores.).r
-00003980: 2300 0000 727f 0000 0072 1b00 0000 72c3  #...r....r....r.
-00003990: 0000 0072 3f00 0000 da06 6c69 6e61 6c67  ...r?.....linalg
-000039a0: 72a2 0000 0072 2500 0000 72c9 0000 00da  r....r%...r.....
-000039b0: 0571 7565 7279 5a06 5870 6174 6368 727b  .queryZ.Xpatchr{
-000039c0: 0000 0072 7c00 0000 290a 7234 0000 0072  ...r|...).r4...r
-000039d0: d700 0000 72ea 0000 0072 eb00 0000 722a  ....r....r....r*
-000039e0: 0000 00da 0558 5f65 6e63 5a09 6164 765f  .....X_encZ.adv_
-000039f0: 7072 6f74 6f5a 0a6f 7269 675f 7072 6f74  protoZ.orig_prot
-00003a00: 6f5a 0864 6973 745f 6164 765a 0964 6973  oZ.dist_advZ.dis
-00003a10: 745f 6f72 6967 7244 0000 0072 4400 0000  t_origrD...rD...
-00003a20: 7245 0000 00da 0573 636f 7265 5b02 0000  rE.....score[...
-00003a30: 731a 0000 0000 1406 010c 010a 010a 0110  s...............
-00003a40: 0112 0106 0318 011a 0204 0102 ff04 037a  ...............z
-00003a50: 1443 6f75 6e74 6572 6661 6374 7561 6c2e  .Counterfactual.
-00003a60: 7363 6f72 6572 c700 0000 e964 0000 0029  scorer.....d...)
-00003a70: 0a72 d700 0000 72cf 0000 00da 0c74 6172  .r....r......tar
-00003a80: 6765 745f 636c 6173 7372 ed00 0000 da06  get_classr......
-00003a90: 6b5f 7479 7065 da09 7468 7265 7368 6f6c  k_type..threshol
-00003aa0: 6472 3000 0000 da0b 7072 696e 745f 6576  dr0.....print_ev
-00003ab0: 6572 79da 096c 6f67 5f65 7665 7279 7231  ery..log_everyr1
-00003ac0: 0000 0063 0a00 0000 0000 0000 0000 0000  ...c............
-00003ad0: 4400 0000 0d00 0000 0300 0000 7328 0a00  D...........s(..
-00003ae0: 0088 006a 007c 016a 0164 0119 006b 0273  ...j.|.j.d...k.s
-00003af0: 144a 0082 0174 0274 0374 0474 056a 0666  .J...t.t.t.t.j.f
-00003b00: 0319 0074 0474 0764 029c 0387 0066 0164  ...t.t.d.....f.d
-00003b10: 0364 0484 0c7d 0a7c 0364 0575 0072 8a74  .d...}.|.d.u.r.t
-00003b20: 0874 0988 006a 0a83 0183 017d 037c 03a0  .t...j.....}.|..
-00003b30: 0b74 056a 0c7c 0264 0664 078d 02a1 0101  .t.j.|.d.d......
-00003b40: 007c 0772 8a74 0d64 08a0 0e74 056a 0c7c  .|.r.t.d...t.j.|
-00003b50: 0264 0664 078d 02a1 0183 0101 0074 0d64  .d.d.........t.d
-00003b60: 09a0 0e7c 03a1 0183 0101 007c 017d 0b69  ...|.......|.}.i
-00003b70: 007d 0c88 006a 0f90 0172 9688 006a 10a0  .}...j...r...j..
-00003b80: 1188 00a0 127c 01a1 01a1 017d 0d7c 0464  .....|.....}.|.d
-00003b90: 0575 0072 ba88 006a 136e 0488 006a 147d  .u.r...j.n...j.}
-00003ba0: 0e7c 0ea0 15a1 0044 005d ca5c 027d 0f7d  .|.....D.].\.}.}
-00003bb0: 107c 0f7c 0376 0172 da71 c87c 0464 0575  .|.|.v.r.q.|.d.u
-00003bc0: 0072 f874 056a 16a0 177c 0d7c 1018 00a1  .r.t.j...|.|....
-00003bd0: 017c 0c7c 0f3c 0071 c87c 0464 0575 0172  .|.|.<.q.|.d.u.r
-00003be0: c874 056a 166a 177c 0da0 187c 0d6a 0164  .t.j.j.|...|.j.d
-00003bf0: 0119 0064 0aa1 027c 10a0 187c 106a 0164  ...d...|...|.j.d
-00003c00: 0119 0064 0aa1 0218 0064 0664 078d 027d  ...d.....d.d...}
-00003c10: 1174 05a0 197c 11a1 0164 057c 0485 0219  .t...|...d.|....
-00003c20: 007d 127c 0564 0b6b 0290 0172 6074 05a0  .}.|.d.k...r`t..
-00003c30: 1a7c 117c 1219 00a1 017c 0c7c 0f3c 006e  .|.|.....|.|.<.n
-00003c40: 107c 117c 1264 0a19 0019 007c 0c7c 0f3c  .|.|.d.....|.|.<
-00003c50: 0074 056a 1b74 056a 1a7c 107c 1219 0064  .t.j.t.j.|.|...d
-00003c60: 0164 078d 0264 0164 078d 0288 006a 137c  .d...d.d.....j.|
-00003c70: 0f3c 0071 c86e 8888 006a 1c90 0272 1e7c  .<.q.n...j...r.|
-00003c80: 0464 0575 0090 0172 ac64 067d 0469 0088  .d.u...r.d.}.i..
-00003c90: 005f 1374 0988 006a 0a83 0144 005d 607d  ._.t...j...D.]`}
-00003ca0: 0f7c 0f7c 0376 0190 0172 ce90 0171 bc88  .|.|.v...r...q..
-00003cb0: 006a 1d7c 0f19 006a 1e7c 0b7c 0464 0c8d  .j.|...j.|.|.d..
-00003cc0: 025c 027d 137d 147c 1364 0119 0064 0a19  .\.}.}.|.d...d..
-00003cd0: 007c 0c7c 0f3c 0088 006a 1f7c 0f19 007c  .|.|.<...j.|...|
-00003ce0: 1464 0119 0064 0a19 0019 00a0 1864 0664  .d...d.......d.d
-00003cf0: 0aa1 0288 006a 137c 0f3c 0090 0171 bc88  .....j.|.<...q..
-00003d00: 006a 2090 0272 5a74 217c 0c7c 0c6a 2264  .j ..rZt!|.|.j"d
-00003d10: 0d8d 0288 005f 2388 006a 1388 006a 2319  ....._#..j...j#.
-00003d20: 007d 157c 0790 0272 6674 0d64 0ea0 0e88  .}.|...rft.d....
-00003d30: 006a 23a1 0183 0101 006e 0c74 05a0 2488  .j#......n.t..$.
-00003d40: 006a 25a1 017d 1588 006a 017d 1674 05a0  .j%..}...j.}.t..
-00003d50: 2488 006a 00a1 017d 1774 05a0 2688 006a  $..j...}.t..&..j
-00003d60: 00a1 0188 006a 2714 007d 1874 05a0 2688  .....j'..}.t..&.
-00003d70: 006a 00a1 0164 0f14 007d 1964 0f67 0188  .j...d...}.d.g..
-00003d80: 006a 0014 007d 1a74 05a0 2488 006a 0164  .j...}.t..$..j.d
-00003d90: 0664 0585 0219 00a1 0167 0188 006a 0014  .d.......g...j..
-00003da0: 007d 1b74 05a0 2488 006a 01a1 0174 05a0  .}.t..$..j...t..
-00003db0: 2488 006a 01a1 0166 027d 1c64 1064 1184  $..j...f.}.d.d..
-00003dc0: 0074 0988 006a 2883 0144 0083 0188 005f  .t...j(..D....._
-00003dd0: 2974 0988 006a 2883 0144 0090 065d f87d  )t...j(..D...].}
-00003de0: 1d88 006a 2aa0 2b88 006a 2ca1 0101 0064  ...j*.+..j,....d
-00003df0: 0f67 0188 006a 0014 007d 1e64 0a67 0188  .g...j...}.d.g..
-00003e00: 006a 0014 007d 1f88 006a 2d7c 0b88 006a  .j...}...j-|...j
-00003e10: 2e7c 0288 006a 2f7c 1888 006a 307c 0b88  .|...j/|...j0|..
-00003e20: 006a 317c 0b88 006a 327c 1569 067d 2088  .j1|...j2|.i.} .
-00003e30: 006a 2a6a 2b88 006a 337c 2064 128d 0201  .j*j+..j3| d....
-00003e40: 0067 0067 0002 007d 217d 2274 0988 006a  .g.g...}!}"t...j
-00003e50: 3483 0144 0090 055d b47d 2374 05a0 247c  4..D...].}#t..$|
-00003e60: 16a1 017d 2474 05a0 247c 16a1 017d 2588  ...}$t..$|...}%.
-00003e70: 006a 3590 0473 9688 006a 2764 136b 0390  .j5..s...j'd.k..
-00003e80: 0373 ae88 006a 2864 066b 0490 0472 9688  .s...j(d.k...r..
-00003e90: 006a 366a 3788 006a 2a64 148d 017d 2688  .j6j7..j*d...}&.
-00003ea0: 006a 386a 3788 006a 2a64 148d 017d 277c  .j8j7..j*d...}'|
-00003eb0: 21a0 397c 26a1 0101 007c 22a0 397c 27a1  !.9|&....|".9|'.
-00003ec0: 0101 007c 2388 006a 3a16 0064 016b 0290  ...|#..j:..d.k..
-00003ed0: 0472 967c 2364 016b 0490 0472 9688 006a  .r.|#d.k...r...j
-00003ee0: 3b6a 3788 006a 2a64 148d 017d 0f74 05a0  ;j7..j*d...}.t..
-00003ef0: 3c7c 21a1 017d 2174 05a0 3c7c 22a1 017d  <|!..}!t..<|"..}
-00003f00: 2288 006a 3d7c 217c 027c 1664 0664 0585  "..j=|!|.|.d.d..
-00003f10: 0219 0064 158d 037c 0f14 007d 2488 006a  ...d...|...}$..j
-00003f20: 3d7c 227c 027c 1664 0664 0585 0219 0064  =|"|.|.d.d.....d
-00003f30: 158d 037c 0f14 007d 2574 05a0 3e7c 2488  ...|...}%t..>|$.
-00003f40: 006a 3e64 0119 0088 006a 3e64 0619 00a1  .j>d.....j>d....
-00003f50: 037d 2474 05a0 3e7c 2588 006a 3e64 0119  .}$t..>|%..j>d..
-00003f60: 0088 006a 3e64 0619 00a1 037d 2567 0067  ...j>d.....}%g.g
-00003f70: 0002 007d 217d 2288 006a 2aa0 2b88 006a  ...}!}"..j*.+..j
-00003f80: 3fa1 017d 2864 1664 1784 007c 2844 0083  ?..}(d.d...|(D..
-00003f90: 0164 0119 007d 2974 05a0 3e7c 2988 006a  .d...})t..>|)..j
-00003fa0: 3e64 0119 0088 006a 3e64 0619 00a1 037d  >d.....j>d.....}
-00003fb0: 297c 297c 2517 007d 2a88 006a 2a6a 2b88  )|)|%..}*..j*j+.
-00003fc0: 006a 4088 006a 417c 2a69 0164 128d 0201  .j@..jA|*i.d....
-00003fd0: 0088 006a 2aa0 2b88 006a 4288 006a 4388  ...j*.+..jB..jC.
-00003fe0: 006a 4488 006a 4567 04a1 0101 0088 006a  .jD..jEg.......j
-00003ff0: 3590 0572 4088 006a 2aa0 2b88 006a 4688  5..r@..j*.+..jF.
-00004000: 006a 4788 006a 4888 006a 4988 006a 3667  .jG..jH..jI..j6g
-00004010: 05a1 015c 057d 2b7d 2c7d 2d7d 2e7d 2f6e  ...\.}+},}-}.}/n
-00004020: 6a88 006a 366a 3788 006a 2a64 148d 017d  j..j6j7..j*d...}
-00004030: 2674 4a6a 4b7c 2674 4a6a 4c64 188d 027d  &tJjK|&tJjLd...}
-00004040: 2688 00a0 117c 26a1 01a0 4da1 00a0 4ea1  &....|&...M...N.
-00004050: 007d 2e88 00a0 4f7c 2e7c 02a1 027d 2c88  .}....O|.|...},.
-00004060: 006a 477c 2c69 017d 2088 006a 2a6a 2b88  .jG|,i.} ..j*j+.
-00004070: 006a 4688 006a 4888 006a 3667 037c 2064  .jF..jH..j6g.| d
-00004080: 128d 025c 037d 2b7d 2d7d 2f7c 237c 0916  ...\.}+}-}/|#|..
-00004090: 0064 016b 0290 0573 c67c 237c 0816 0064  .d.k...s.|#|...d
-000040a0: 016b 0290 0672 1a88 006a 2aa0 2b88 006a  .k...r...j*.+..j
-000040b0: 5088 006a 5188 006a 5288 006a 5367 04a1  P..jQ..jR..jSg..
-000040c0: 015c 047d 307d 317d 327d 3374 05a0 547c  .\.}0}1}2}3t..T|
-000040d0: 2e7c 0214 00a1 017d 3474 05a0 5564 067c  .|.....}4t..Ud.|
-000040e0: 0218 007c 2e14 00a1 017d 357c 2d7c 2c17  ...|.....}5|-|,.
-000040f0: 007c 3217 007c 3317 007d 367c 237c 0916  .|2..|3..}6|#|..
-00004100: 0064 016b 0290 0772 2488 006a 5664 0575  .d.k...r$..jVd.u
-00004110: 0190 0772 2488 006a 2aa0 2b88 006a 5788  ...r$..j*.+..jW.
-00004120: 006a 5888 006a 5967 03a1 015c 037d 377d  .jX..jYg...\.}7}
-00004130: 387d 3974 5aa0 5ba1 007d 3a7c 3a6a 5c6a  8}9tZ.[..}:|:j\j
-00004140: 5d64 197c 3664 1a8d 0201 007c 3a6a 5c6a  ]d.|6d.....|:j\j
-00004150: 5d64 1b7c 2b64 1a8d 0201 007c 3a6a 5c6a  ]d.|+d.....|:j\j
-00004160: 5d64 1c7c 3164 1a8d 0201 007c 3a6a 5c6a  ]d.|1d.....|:j\j
-00004170: 5d64 1d7c 3064 1a8d 0201 007c 3a6a 5c6a  ]d.|0d.....|:j\j
-00004180: 5d64 1e7c 3264 1a8d 0201 007c 3a6a 5c6a  ]d.|2d.....|:j\j
-00004190: 5d64 1f7c 3364 1a8d 0201 007c 3a6a 5c6a  ]d.|3d.....|:j\j
-000041a0: 5d64 207c 1864 0119 0064 1a8d 0201 007c  ]d |.d...d.....|
-000041b0: 3a6a 5c6a 5d64 217c 2c64 1a8d 0201 007c  :j\j]d!|,d.....|
-000041c0: 3a6a 5c6a 5d64 227c 3764 1a8d 0201 007c  :j\j]d"|7d.....|
-000041d0: 3a6a 5c6a 5d64 237c 3864 1a8d 0201 007c  :j\j]d#|8d.....|
-000041e0: 3a6a 5c6a 5d64 247c 3964 1a8d 0201 0088  :j\j]d$|9d......
-000041f0: 006a 56a0 5e7c 3aa1 0101 0088 006a 56a0  .jV.^|:......jV.
-00004200: 5fa1 0001 007c 0790 0872 127c 237c 0816  _....|...r.|#|..
-00004210: 0064 016b 0290 0872 1274 0d64 25a0 0e7c  .d.k...r.t.d%..|
-00004220: 237c 1864 0119 00a1 0283 0101 0074 0d64  #|.d.........t.d
-00004230: 26a0 0e7c 2b7c 2ca1 0283 0101 0074 0d64  &..|+|,......t.d
-00004240: 27a0 0e7c 307c 317c 32a1 0383 0101 0074  '..|0|1|2......t
-00004250: 0d64 28a0 0e7c 33a1 0183 0101 0074 0d64  .d(..|3......t.d
-00004260: 29a0 0e7c 347c 35a1 0283 0101 0074 0d64  )..|4|5......t.d
-00004270: 2aa0 0e7c 29a0 21a1 007c 29a0 55a1 00a1  *..|).!..|).U...
-00004280: 0283 0101 0074 0d64 2ba0 0e74 05a0 1a7c  .....t.d+..t...|
-00004290: 29a1 0174 05a0 1a74 05a0 607c 29a1 01a1  )..t...t..`|)...
-000042a0: 01a1 0283 0101 0088 006a 3590 0873 0874  .........j5..s.t
-000042b0: 0d64 2ca0 0e7c 24a0 21a1 007c 24a0 55a1  .d,..|$.!..|$.U.
-000042c0: 00a1 0283 0101 0074 0d64 2da0 0e74 05a0  .......t.d-..t..
-000042d0: 1a7c 24a1 0174 05a0 1a74 05a0 607c 24a1  .|$..t...t..`|$.
-000042e0: 01a1 01a1 0283 0101 0074 616a 62a0 5fa1  .........tajb._.
-000042f0: 0001 0074 6374 647c 2d7c 2e7c 2f83 0383  ...tctd|-|.|/...
-00004300: 0144 0090 015d 025c 027d 3b5c 037d 3c7d  .D...].\.};\.}<}
-00004310: 3d7d 3e74 05a0 0c7c 027c 3b19 00a1 017d  =}>t...|.|;....}
-00004320: 3f74 05a0 0c7c 3da1 017d 4074 056a 1b7c  ?t...|=..}@t.j.|
-00004330: 3e64 0164 078d 027d 3e7c 0664 136b 0490  >d.d...}>|.d.k..
-00004340: 0872 8088 00a0 657c 3e74 05a0 0c7c 2ea1  .r....e|>t...|..
-00004350: 017c 3fa1 037d 417c 417c 066b 047d 426e  .|?..}A|A|.k.}Bn
-00004360: 0464 2e7d 427c 3c7c 1e7c 3b19 006b 0090  .d.}B|<|.|;..k..
-00004370: 0872 be7c 0a7c 3d7c 3f83 0290 0872 be7c  .r.|.|=|?....r.|
-00004380: 4290 0872 be7c 407c 0376 0090 0872 be7c  B..r.|@|.v...r.|
-00004390: 3c7c 1e7c 3b3c 007c 407c 1f7c 3b3c 007c  <|.|;<.|@|.|;<.|
-000043a0: 3c7c 1a7c 3b19 006b 0090 0872 227c 0a7c  <|.|;..k...r"|.|
-000043b0: 3d7c 3f83 0290 0872 227c 4290 0872 227c  =|?....r"|B..r"|
-000043c0: 407c 0376 0090 0872 227c 0790 0872 f674  @|.v...r"|...r.t
-000043d0: 0d64 2f83 0101 007c 3c7c 1a7c 3b3c 007c  .d/....|<|.|;<.|
-000043e0: 3e7c 1b7c 3b3c 007c 297c 2466 027d 1c64  >|.|;<.|)|$f.}.d
-000043f0: 2e88 005f 6688 006a 297c 1d19 00a0 397c  ..._f..j)|....9|
-00004400: 3ea1 0101 0090 0871 2290 0371 7474 0988  >......q"..qtt..
-00004410: 006a 0083 0144 005d ba7d 3b7c 0a7c 1f7c  .j...D.].};|.|.|
-00004420: 3b19 0074 05a0 0c7c 027c 3b19 00a1 0183  ;..t...|.|;.....
-00004430: 0290 0972 a07c 1f7c 3b19 0064 0a6b 0390  ...r.|.|;..d.k..
-00004440: 0972 a074 217c 197c 3b19 007c 187c 3b19  .r.t!|.|;..|.|;.
-00004450: 0083 027c 197c 3b3c 007c 197c 3b19 0064  ...|.|;<.|.|;..d
-00004460: 306b 0090 0972 ee7c 177c 3b19 007c 197c  0k...r.|.|;..|.|
-00004470: 3b19 0017 0064 311b 007c 187c 3b3c 006e  ;....d1..|.|;<.n
-00004480: 4e74 557c 177c 3b19 007c 187c 3b19 0083  NtU|.|;..|.|;...
-00004490: 027c 177c 3b3c 007c 197c 3b19 0064 306b  .|.|;<.|.|;..d0k
-000044a0: 0090 0972 de7c 177c 3b19 007c 197c 3b19  ...r.|.|;..|.|;.
-000044b0: 0017 0064 311b 007c 187c 3b3c 006e 107c  ...d1..|.|;<.n.|
-000044c0: 187c 3b05 0019 0064 3239 0003 003c 0090  .|;....d29...<..
-000044d0: 0971 3690 0271 fa74 056a 3c7c 1b64 0164  .q6..q.t.j<|.d.d
-000044e0: 078d 027d 437c 436a 0188 006a 016b 0390  ...}C|Cj...j.k..
-000044f0: 0a72 2074 056a 1b7c 4364 0164 078d 027d  .r t.j.|Cd.d...}
-00004500: 437c 437c 1c66 0253 0029 3361 9f06 0000  C|C|.f.S.)3a....
-00004510: 0a20 2020 2020 2020 2046 696e 6420 6120  .        Find a 
-00004520: 636f 756e 7465 7266 6163 7475 616c 2028  counterfactual (
-00004530: 4346 2920 666f 7220 696e 7374 616e 6365  CF) for instance
-00004540: 2060 5860 2075 7369 6e67 2061 2066 6173   `X` using a fas
-00004550: 7420 6974 6572 6174 6976 6520 7368 7269  t iterative shri
-00004560: 6e6b 6167 652d 7468 7265 7368 6f6c 6469  nkage-thresholdi
-00004570: 6e67 2061 6c67 6f72 6974 686d 2028 4649  ng algorithm (FI
-00004580: 5354 4129 2e0a 0a20 2020 2020 2020 2050  STA)...        P
-00004590: 6172 616d 6574 6572 7320 6d6b 0a20 2020  arameters mk.   
-000045a0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-000045b0: 2020 2020 2020 2020 580a 2020 2020 2020          X.      
-000045c0: 2020 2020 2020 496e 7374 616e 6365 2074        Instance t
-000045d0: 6f20 6174 7461 636b 2e0a 2020 2020 2020  o attack..      
-000045e0: 2020 590a 2020 2020 2020 2020 2020 2020    Y.            
-000045f0: 4c61 6265 6c73 2066 6f72 2060 5860 2061  Labels for `X` a
-00004600: 7320 6f6e 652d 686f 742d 656e 636f 6469  s one-hot-encodi
-00004610: 6e67 2e0a 2020 2020 2020 2020 7461 7267  ng..        targ
-00004620: 6574 5f63 6c61 7373 0a20 2020 2020 2020  et_class.       
-00004630: 2020 2020 204c 6973 7420 7769 7468 2074       List with t
-00004640: 6172 6765 7420 636c 6173 7365 7320 7573  arget classes us
-00004650: 6564 2074 6f20 6669 6e64 2063 6c6f 7365  ed to find close
-00004660: 7374 2070 726f 746f 7479 7065 2e20 4966  st prototype. If
-00004670: 2060 604e 6f6e 6560 602c 2074 6865 206e   ``None``, the n
-00004680: 6561 7265 7374 2070 726f 746f 7479 7065  earest prototype
-00004690: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-000046a0: 6570 7420 666f 7220 7468 6520 7072 6564  ept for the pred
-000046b0: 6963 7420 636c 6173 7320 6f6e 2074 6865  ict class on the
-000046c0: 2069 6e73 7461 6e63 6520 6973 2075 7365   instance is use
-000046d0: 642e 0a20 2020 2020 2020 206b 0a20 2020  d..        k.   
-000046e0: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
-000046f0: 6f66 206e 6561 7265 7374 2069 6e73 7461  of nearest insta
-00004700: 6e63 6573 2075 7365 6420 746f 2064 6566  nces used to def
-00004710: 696e 6520 7468 6520 7072 6f74 6f74 7970  ine the prototyp
-00004720: 6520 666f 7220 6120 636c 6173 732e 2044  e for a class. D
-00004730: 6566 6175 6c74 7320 746f 2075 7369 6e67  efaults to using
-00004740: 2061 6c6c 0a20 2020 2020 2020 2020 2020   all.           
-00004750: 2069 6e73 7461 6e63 6573 2062 656c 6f6e   instances belon
-00004760: 6769 6e67 2074 6f20 7468 6520 636c 6173  ging to the clas
-00004770: 7320 6966 2061 6e20 656e 636f 6465 7220  s if an encoder 
-00004780: 6973 2075 7365 6420 616e 6420 746f 2031  is used and to 1
-00004790: 2066 6f72 206b 2d64 2074 7265 6573 2e0a   for k-d trees..
-000047a0: 2020 2020 2020 2020 6b5f 7479 7065 0a20          k_type. 
-000047b0: 2020 2020 2020 2020 2020 2055 7365 2065             Use e
-000047c0: 6974 6865 7220 7468 6520 6176 6572 6167  ither the averag
-000047d0: 6520 656e 636f 6469 6e67 206f 6620 7468  e encoding of th
-000047e0: 6520 6b20 6e65 6172 6573 7420 696e 7374  e k nearest inst
-000047f0: 616e 6365 7320 696e 2061 2063 6c61 7373  ances in a class
-00004800: 2028 6060 6b5f 7479 7065 3d27 6d65 616e   (``k_type='mean
-00004810: 2760 6029 206f 720a 2020 2020 2020 2020  '``) or.        
-00004820: 2020 2020 7468 6520 6b2d 6e65 6172 6573      the k-neares
-00004830: 7420 656e 636f 6469 6e67 2069 6e20 7468  t encoding in th
-00004840: 6520 636c 6173 7320 2860 606b 5f74 7970  e class (``k_typ
-00004850: 653d 2770 6f69 6e74 2760 6029 2074 6f20  e='point'``) to 
-00004860: 6465 6669 6e65 2074 6865 2070 726f 746f  define the proto
-00004870: 7479 7065 206f 6620 7468 6174 2063 6c61  type of that cla
-00004880: 7373 2e0a 2020 2020 2020 2020 2020 2020  ss..            
-00004890: 4f6e 6c79 2072 656c 6576 616e 7420 6966  Only relevant if
-000048a0: 2061 6e20 656e 636f 6465 7220 6973 2075   an encoder is u
-000048b0: 7365 6420 746f 2064 6566 696e 6520 7468  sed to define th
-000048c0: 6520 7072 6f74 6f74 7970 6573 2e0a 2020  e prototypes..  
-000048d0: 2020 2020 2020 7468 7265 7368 6f6c 640a        threshold.
-000048e0: 2020 2020 2020 2020 2020 2020 5468 7265              Thre
-000048f0: 7368 6f6c 6420 6c65 7665 6c20 666f 7220  shold level for 
-00004900: 7468 6520 7261 7469 6f20 6265 7477 6565  the ratio betwee
-00004910: 6e20 7468 6520 6469 7374 616e 6365 206f  n the distance o
-00004920: 6620 7468 6520 636f 756e 7465 7266 6163  f the counterfac
-00004930: 7475 616c 2074 6f20 7468 6520 7072 6f74  tual to the prot
-00004940: 6f74 7970 6520 6f66 2074 6865 0a20 2020  otype of the.   
-00004950: 2020 2020 2020 2020 2070 7265 6469 6374           predict
-00004960: 6564 2063 6c61 7373 2066 6f72 2074 6865  ed class for the
-00004970: 206f 7269 6769 6e61 6c20 696e 7374 616e   original instan
-00004980: 6365 206f 7665 7220 7468 6520 6469 7374  ce over the dist
-00004990: 616e 6365 2074 6f20 7468 6520 7072 6f74  ance to the prot
-000049a0: 6f74 7970 6520 6f66 2074 6865 2070 7265  otype of the pre
-000049b0: 6469 6374 6564 2063 6c61 7373 0a20 2020  dicted class.   
-000049c0: 2020 2020 2020 2020 2066 6f72 2074 6865           for the
-000049d0: 2063 6f75 6e74 6572 6661 6374 7561 6c2e   counterfactual.
-000049e0: 2049 6620 7468 6520 7472 7573 7420 7363   If the trust sc
-000049f0: 6f72 6520 6973 2062 656c 6f77 2074 6865  ore is below the
-00004a00: 2074 6872 6573 686f 6c64 2c20 7468 6520   threshold, the 
-00004a10: 7072 6f70 6f73 6564 2063 6f75 6e74 6572  proposed counter
-00004a20: 6661 6374 7561 6c20 646f 6573 0a20 2020  factual does.   
-00004a30: 2020 2020 2020 2020 206e 6f74 206d 6565           not mee
-00004a40: 7420 7468 6520 7265 7175 6972 656d 656e  t the requiremen
-00004a50: 7473 2e0a 2020 2020 2020 2020 7665 7262  ts..        verb
-00004a60: 6f73 650a 2020 2020 2020 2020 2020 2020  ose.            
-00004a70: 5072 696e 7420 696e 7465 726d 6564 6961  Print intermedia
-00004a80: 7465 2072 6573 756c 7473 206f 6620 6f70  te results of op
-00004a90: 7469 6d69 7a61 7469 6f6e 2069 6620 6060  timization if ``
-00004aa0: 5472 7565 6060 2e0a 2020 2020 2020 2020  True``..        
-00004ab0: 7072 696e 745f 6576 6572 790a 2020 2020  print_every.    
-00004ac0: 2020 2020 2020 2020 5072 696e 7420 6672          Print fr
-00004ad0: 6571 7565 6e63 7920 6966 2076 6572 626f  equency if verbo
-00004ae0: 7365 2069 7320 6060 5472 7565 6060 2e0a  se is ``True``..
-00004af0: 2020 2020 2020 2020 6c6f 675f 6576 6572          log_ever
-00004b00: 790a 2020 2020 2020 2020 2020 2020 6074  y.            `t
-00004b10: 656e 736f 7262 6f61 7264 6020 6c6f 6720  ensorboard` log 
-00004b20: 6672 6571 7565 6e63 7920 6966 2077 7269  frequency if wri
-00004b30: 7465 2064 6972 6563 746f 7279 2069 7320  te directory is 
-00004b40: 7370 6563 6966 6965 642e 0a0a 2020 2020  specified...    
-00004b50: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00004b60: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00004b70: 2020 2020 4f76 6572 616c 6c20 6265 7374      Overall best
-00004b80: 2061 7474 6163 6b20 616e 6420 6772 6164   attack and grad
-00004b90: 6965 6e74 7320 666f 7220 7468 6174 2061  ients for that a
-00004ba0: 7474 6163 6b2e 0a20 2020 2020 2020 2072  ttack..        r
-00004bb0: 0100 0000 2903 7261 0000 00da 0179 7231  ....).ra.....yr1
-00004bc0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00004bd0: 0200 0000 0500 0000 1300 0000 7340 0000  ............s@..
-00004be0: 0074 007c 0074 0174 0274 036a 0466 0383  .t.|.t.t.t.j.f..
-00004bf0: 0273 3874 03a0 057c 00a1 017d 007c 007c  .s8t...|...}.|.|
-00004c00: 0105 0019 0088 006a 0637 0003 003c 0074  .......j.7...<.t
-00004c10: 03a0 077c 00a1 017d 007c 007c 016b 0353  ...|...}.|.|.k.S
-00004c20: 0029 0161 8501 0000 0a20 2020 2020 2020  .).a.....       
-00004c30: 2020 2020 2043 6f6d 7061 7265 2070 7265       Compare pre
-00004c40: 6469 6374 696f 6e73 2077 6974 6820 7461  dictions with ta
-00004c50: 7267 6574 206c 6162 656c 7320 616e 6420  rget labels and 
-00004c60: 7265 7475 726e 2077 6865 7468 6572 2063  return whether c
-00004c70: 6f75 6e74 6572 6661 6374 7561 6c20 636f  ounterfactual co
-00004c80: 6e64 6974 696f 6e73 2068 6f6c 642e 0a0a  nditions hold...
-00004c90: 2020 2020 2020 2020 2020 2020 5061 7261              Para
-00004ca0: 6d65 7465 7273 0a20 2020 2020 2020 2020  meters.         
-00004cb0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00004cc0: 2020 2020 2020 2020 2020 780a 2020 2020            x.    
-00004cd0: 2020 2020 2020 2020 2020 2020 5072 6564              Pred
-00004ce0: 6963 7465 6420 636c 6173 7320 7072 6f62  icted class prob
-00004cf0: 6162 696c 6974 6965 7320 6f72 206c 6162  abilities or lab
-00004d00: 656c 732e 0a20 2020 2020 2020 2020 2020  els..           
-00004d10: 2079 0a20 2020 2020 2020 2020 2020 2020   y.             
-00004d20: 2020 2054 6172 6765 7420 6f72 2070 7265     Target or pre
-00004d30: 6469 6374 6564 206c 6162 656c 732e 0a0a  dicted labels...
-00004d40: 2020 2020 2020 2020 2020 2020 5265 7475              Retu
-00004d50: 726e 730a 2020 2020 2020 2020 2020 2020  rns.            
-00004d60: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00004d70: 2020 2020 426f 6f6c 2077 6865 7468 6572      Bool whether
-00004d80: 2063 6f75 6e74 6572 6661 6374 7561 6c20   counterfactual 
-00004d90: 636f 6e64 6974 696f 6e73 2068 6f6c 642e  conditions hold.
-00004da0: 0a20 2020 2020 2020 2020 2020 2029 0872  .            ).r
-00004db0: 3d00 0000 723e 0000 00da 0369 6e74 723f  =...r>.....intr?
-00004dc0: 0000 00da 0569 6e74 3634 7269 0000 0072  .....int64ri...r
-00004dd0: 1e00 0000 da06 6172 676d 6178 2902 7261  ......argmax).ra
-00004de0: 0000 0072 f800 0000 a901 7234 0000 0072  ...r......r4...r
-00004df0: 4400 0000 7245 0000 00da 0763 6f6d 7061  D...rE.....compa
-00004e00: 7265 b302 0000 730a 0000 0000 0f12 010a  re....s.........
-00004e10: 0112 010a 017a 2643 6f75 6e74 6572 6661  .....z&Counterfa
-00004e20: 6374 7561 6c2e 6174 7461 636b 2e3c 6c6f  ctual.attack.<lo
-00004e30: 6361 6c73 3e2e 636f 6d70 6172 654e 721a  cals>.compareNr.
-00004e40: 0000 0072 5900 0000 7a13 5072 6564 6963  ...rY...z.Predic
-00004e50: 7465 6420 636c 6173 733a 207b 7d7a 1254  ted class: {}z.T
-00004e60: 6172 6765 7420 636c 6173 7365 733a 207b  arget classes: {
-00004e70: 7d72 3300 0000 72c7 0000 0072 ec00 0000  }r3...r....r....
-00004e80: 2901 72b8 0000 007a 1350 726f 746f 7479  ).r....z.Prototy
-00004e90: 7065 2063 6c61 7373 3a20 7b7d 7212 0000  pe class: {}r...
-00004ea0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00004eb0: 0000 0400 0000 5300 0000 7312 0000 0069  ......S...s....i
-00004ec0: 007c 005d 0a7d 017c 0167 0093 0271 0453  .|.].}.|.g...q.S
-00004ed0: 0072 4400 0000 7244 0000 0029 0272 4200  .rD...rD...).rB.
-00004ee0: 0000 72cb 0000 0072 4400 0000 7244 0000  ..r....rD...rD..
-00004ef0: 0072 4500 0000 da0a 3c64 6963 7463 6f6d  .rE.....<dictcom
-00004f00: 703e 1003 0000 7263 0000 007a 2943 6f75  p>....rc...z)Cou
-00004f10: 6e74 6572 6661 6374 7561 6c2e 6174 7461  nterfactual.atta
-00004f20: 636b 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  ck.<locals>.<dic
-00004f30: 7463 6f6d 703e 2901 da09 6665 6564 5f64  tcomp>)...feed_d
-00004f40: 6963 7472 0f00 0000 72d0 0000 0029 0172  ictr....r....).r
-00004f50: d800 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00004f60: 0003 0000 0004 0000 0053 0000 0073 1400  .........S...s..
-00004f70: 0000 6700 7c00 5d0c 5c02 7d01 7d02 7c01  ..g.|.].\.}.}.|.
-00004f80: 9102 7104 5300 7244 0000 0072 4400 0000  ..q.S.rD...rD...
-00004f90: 2903 7242 0000 0072 de00 0000 7243 0000  ).rB...r....rC..
-00004fa0: 0072 4400 0000 7244 0000 0072 4500 0000  .rD...rD...rE...
-00004fb0: 7246 0000 0050 0300 0072 6300 0000 7a29  rF...P...rc...z)
-00004fc0: 436f 756e 7465 7266 6163 7475 616c 2e61  Counterfactual.a
-00004fd0: 7474 6163 6b2e 3c6c 6f63 616c 733e 2e3c  ttack.<locals>.<
-00004fe0: 6c69 7374 636f 6d70 3e29 0172 4800 0000  listcomp>).rH...
-00004ff0: 7a0e 6c6f 7373 2f4f 7074 696d 697a 6564  z.loss/Optimized
-00005000: 2902 da03 7461 675a 0c73 696d 706c 655f  )...tagZ.simple_
-00005010: 7661 6c75 657a 0a6c 6f73 732f 546f 7461  valuez.loss/Tota
-00005020: 6c7a 076c 6f73 732f 4c31 7a07 6c6f 7373  lz.loss/L1z.loss
-00005030: 2f4c 327a 106c 6f73 732f 4175 746f 456e  /L2z.loss/AutoEn
-00005040: 636f 6465 727a 136c 6f73 732f 436c 6173  coderz.loss/Clas
-00005050: 7350 726f 746f 7479 7065 7a0e 6c6f 7373  sPrototypez.loss
-00005060: 2f50 7265 6453 6361 6c65 7a0d 6c6f 7373  /PredScalez.loss
-00005070: 2f50 7265 644c 6f73 737a 0b74 7261 696e  /PredLossz.train
-00005080: 696e 672f 6c72 7a0a 7472 6169 6e69 6e67  ing/lrz.training
-00005090: 2f7a 7a13 7472 6169 6e69 6e67 2f47 6c6f  /zz.training/Glo
-000050a0: 6261 6c53 7465 707a 190a 4974 6572 6174  balStepz..Iterat
-000050b0: 696f 6e3a 207b 7d3b 2043 6f6e 7374 3a20  ion: {}; Const: 
-000050c0: 7b7d 7a27 4c6f 7373 2074 6f74 616c 3a20  {}z'Loss total: 
-000050d0: 7b3a 2e33 667d 2c20 6c6f 7373 2061 7474  {:.3f}, loss att
-000050e0: 6163 6b3a 207b 3a2e 3366 7d7a 274c 323a  ack: {:.3f}z'L2:
-000050f0: 207b 3a2e 3366 7d2c 204c 313a 207b 3a2e   {:.3f}, L1: {:.
-00005100: 3366 7d2c 206c 6f73 7320 4145 3a20 7b3a  3f}, loss AE: {:
-00005110: 2e33 667d 7a12 4c6f 7373 2070 726f 746f  .3f}z.Loss proto
-00005120: 3a20 7b3a 2e33 667d 7a32 5461 7267 6574  : {:.3f}z2Target
-00005130: 2070 726f 6261 3a20 7b3a 2e32 667d 2c20   proba: {:.2f}, 
-00005140: 6d61 7820 6e6f 6e20 7461 7267 6574 2070  max non target p
-00005150: 726f 6261 3a20 7b3a 2e32 667d 7a25 4772  roba: {:.2f}z%Gr
-00005160: 6164 6965 6e74 2067 7261 7068 206d 696e  adient graph min
-00005170: 2f6d 6178 3a20 7b3a 2e33 667d 2f7b 3a2e  /max: {:.3f}/{:.
-00005180: 3366 7d7a 2b47 7261 6469 656e 7420 6772  3f}z+Gradient gr
-00005190: 6170 6820 6d65 616e 2f61 6273 206d 6561  aph mean/abs mea
-000051a0: 6e3a 207b 3a2e 3366 7d2f 7b3a 2e33 667d  n: {:.3f}/{:.3f}
-000051b0: 7a30 4772 6164 6965 6e74 206e 756d 6572  z0Gradient numer
-000051c0: 6963 616c 2061 7474 6163 6b20 6d69 6e2f  ical attack min/
-000051d0: 6d61 783a 207b 3a2e 3366 7d2f 7b3a 2e33  max: {:.3f}/{:.3
-000051e0: 667d 7a2f 4772 6164 6965 6e74 206e 756d  f}z/Gradient num
-000051f0: 6572 6963 616c 206d 6561 6e2f 6162 7320  erical mean/abs 
-00005200: 6d65 616e 3a20 7b3a 2e33 667d 2f7b 3a2e  mean: {:.3f}/{:.
-00005210: 3366 7d54 7a1f 0a4e 6577 2062 6573 7420  3f}Tz..New best 
-00005220: 636f 756e 7465 7266 6163 7475 616c 2066  counterfactual f
-00005230: 6f75 6e64 2167 0000 0000 65cd cd41 7207  ound!g....e..Ar.
-00005240: 0000 0072 1600 0000 2967 7280 0000 0072  ...r....)gr....r
-00005250: 1d00 0000 7206 0000 0072 3e00 0000 72f9  ....r....r>...r.
-00005260: 0000 0072 3f00 0000 da07 6e64 6172 7261  ...r?.....ndarra
-00005270: 79da 0462 6f6f 6c72 9900 0000 7282 0000  y..boolr....r...
-00005280: 0072 7800 0000 72b7 0000 0072 fb00 0000  .rx...r....r....
-00005290: 727a 0000 00da 0666 6f72 6d61 7472 2300  rz.....formatr#.
-000052a0: 0000 727f 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-000052b0: 0072 c300 0000 72c4 0000 00da 0569 7465  .r....r......ite
-000052c0: 6d73 72ee 0000 0072 a200 0000 72e4 0000  msr....r....r...
-000052d0: 00da 0761 7267 736f 7274 72c7 0000 0072  ...argsortr....r
-000052e0: c600 0000 7225 0000 0072 c900 0000 72ef  ....r%...r....r.
-000052f0: 0000 0072 ca00 0000 723b 0000 00da 036d  ...r....r;.....m
-00005300: 696e da03 6765 74da 0869 645f 7072 6f74  in..get..id_prot
-00005310: 6f72 7700 0000 7285 0000 0072 4000 0000  orw...r....r@...
-00005320: 7228 0000 0072 2900 0000 da09 6366 5f67  r(...r).....cf_g
-00005330: 6c6f 6261 6c72 2f00 0000 da03 7275 6e72  lobalr/.....runr
-00005340: b300 0000 7250 0000 0072 5400 0000 7255  ....rP...rT...rU
-00005350: 0000 0072 5200 0000 7253 0000 0072 5600  ...rR...rS...rV.
-00005360: 0000 72b1 0000 0072 2700 0000 7276 0000  ..r....r'...rv..
-00005370: 0072 4a00 0000 72d4 0000 0072 4b00 0000  .rJ...r....rK...
-00005380: 72b2 0000 0072 2c00 0000 724e 0000 0072  r....r,...rN...r
-00005390: e500 0000 72e8 0000 0072 2b00 0000 72ae  ....r....r+...r.
-000053a0: 0000 0072 b000 0000 72af 0000 0072 9500  ...r....r....r..
-000053b0: 0000 7296 0000 0072 9700 0000 7298 0000  ..r....r....r...
-000053c0: 0072 aa00 0000 725c 0000 0072 9f00 0000  .r....r\...r....
-000053d0: 72a4 0000 0072 7900 0000 72e1 0000 0072  r....ry...r....r
-000053e0: 8400 0000 72e2 0000 0072 e300 0000 72d6  ....r....r....r.
-000053f0: 0000 0072 a100 0000 72a0 0000 0072 5b00  ...r....r....r[.
-00005400: 0000 72a8 0000 0072 d200 0000 72d3 0000  ..r....r....r...
-00005410: 0072 b500 0000 72ac 0000 0072 9300 0000  .r....r....r....
-00005420: 724f 0000 0072 6f00 0000 da07 5375 6d6d  rO...ro.....Summ
-00005430: 6172 79da 0576 616c 7565 7290 0000 00da  ary..valuer.....
-00005440: 0b61 6464 5f73 756d 6d61 7279 da05 666c  .add_summary..fl
-00005450: 7573 6872 8b00 0000 da03 7379 73da 0673  ushr......sys..s
-00005460: 7464 6f75 74da 0965 6e75 6d65 7261 7465  tdout..enumerate
-00005470: da03 7a69 7072 f100 0000 da0b 6265 7374  ..zipr......best
-00005480: 5f61 7474 6163 6b29 4472 3400 0000 72d7  _attack)Dr4...r.
-00005490: 0000 0072 cf00 0000 72f3 0000 0072 ed00  ...r....r....r..
-000054a0: 0000 72f4 0000 0072 f500 0000 7230 0000  ..r....r....r0..
-000054b0: 0072 f600 0000 72f7 0000 0072 fd00 0000  .r....r....r....
-000054c0: 5a05 585f 6e75 6d5a 0a64 6973 745f 7072  Z.X_numZ.dist_pr
-000054d0: 6f74 6f72 f000 0000 da0a 636c 6173 735f  otor......class_
-000054e0: 6469 6374 da01 63da 0176 5a06 6469 7374  dict..c..vZ.dist
-000054f0: 5f6b 72cc 0000 005a 0664 6973 745f 635a  _kr....Z.dist_cZ
-00005500: 0569 6478 5f63 5a09 7072 6f74 6f5f 7661  .idx_cZ.proto_va
-00005510: 6c5a 0a70 6572 745f 7368 6170 655a 0863  lZ.pert_shapeZ.c
-00005520: 6f6e 7374 5f6c 6272 4e00 0000 5a08 636f  onst_lbrN...Z.co
-00005530: 6e73 745f 7562 5a11 6f76 6572 616c 6c5f  nst_ubZ.overall_
-00005540: 6265 7374 5f64 6973 745a 136f 7665 7261  best_distZ.overa
-00005550: 6c6c 5f62 6573 745f 6174 7461 636b 5a11  ll_best_attackZ.
-00005560: 6f76 6572 616c 6c5f 6265 7374 5f67 7261  overall_best_gra
-00005570: 6472 4300 0000 5a11 6375 7272 656e 745f  drC...Z.current_
-00005580: 6265 7374 5f64 6973 745a 1263 7572 7265  best_distZ.curre
-00005590: 6e74 5f62 6573 745f 7072 6f62 6172 ff00  nt_best_probar..
-000055a0: 0000 5a0b 585f 6465 725f 6261 7463 685a  ..Z.X_der_batchZ
-000055b0: 0d58 5f64 6572 5f62 6174 6368 5f73 72cb  .X_der_batch_sr.
-000055c0: 0000 00da 0967 7261 6473 5f6e 756d 5a0b  .....grads_numZ.
-000055d0: 6772 6164 735f 6e75 6d5f 735a 0558 5f64  grads_num_sZ.X_d
-000055e0: 6572 5a07 585f 6465 725f 735a 1067 7261  erZ.X_der_sZ.gra
-000055f0: 6473 5f76 6172 735f 6772 6170 68da 0b67  ds_vars_graph..g
-00005600: 7261 6473 5f67 7261 7068 72e7 0000 005a  rads_graphr....Z
-00005610: 086c 6f73 735f 746f 7472 5c00 0000 7258  .loss_totr\...rX
-00005620: 0000 0072 a400 0000 724a 0000 0072 a100  ...r....rJ...r..
-00005630: 0000 72a0 0000 0072 5b00 0000 72a8 0000  ..r....r[...r...
-00005640: 0072 a600 0000 72a7 0000 0072 a900 0000  .r....r....r....
-00005650: da02 6c72 7293 0000 00da 0267 7372 b400  ..lrr......gsr..
-00005660: 0000 da09 6261 7463 685f 6964 78da 0464  ....batch_idx..d
-00005670: 6973 7472 d900 0000 5a07 6164 765f 6964  istr....Z.adv_id
-00005680: 78da 0759 5f63 6c61 7373 72ea 0000 0072  x..Y_classr....r
-00005690: f100 0000 5a0f 6162 6f76 655f 7468 7265  ....Z.above_thre
-000056a0: 7368 6f6c 6472 1301 0000 7244 0000 0072  sholdr....rD...r
-000056b0: fc00 0000 7245 0000 00da 0661 7474 6163  ....rE.....attac
-000056c0: 6b80 0200 0073 f001 0000 0031 1402 2216  k....s.....1..".
-000056d0: 0801 0e01 1401 0401 1801 0e02 0403 0401  ................
-000056e0: 0802 1201 1402 1001 0801 0201 0801 1601  ................
-000056f0: 0801 0601 2201 02fe 0604 1201 0a01 1402  ...."...........
-00005700: 1001 0401 12ff 1003 0801 0a01 0401 0601  ................
-00005710: 0e01 0a01 0403 1801 1001 2802 0801 1002  ..........(.....
-00005720: 0c01 0601 1202 0c03 0604 0c01 1201 1003  ................
-00005730: 0c01 1c01 1803 1603 1003 0e03 0c01 0c04  ................
-00005740: 0601 0601 0601 0601 0601 06fa 0409 1202  ................
-00005750: 0a02 1003 0a01 0a03 2001 1001 1001 0a01  ........ .......
-00005760: 0a03 0cff 0401 06ff 0403 1001 0a01 0a02  ................
-00005770: 0401 0eff 0403 02fd 02ff 0207 0401 0eff  ................
-00005780: 0403 02fd 02ff 0207 1a01 1a01 0a03 0e01  ................
-00005790: 1201 1a03 0801 1803 0601 12ff 0407 0801  ................
-000057a0: 0602 0401 0401 0401 0401 04fb 02ff 100a  ................
-000057b0: 0601 04ff 0604 1001 1203 0c01 0a01 0601  ................
-000057c0: 10ff 0c04 1c01 0601 12ff 0c03 0e01 1201  ................
-000057d0: 1002 1a01 0601 0eff 0a05 0801 1001 1001  ................
-000057e0: 1001 1001 1001 0601 04ff 0603 1401 1001  ................
-000057f0: 1001 1001 1001 0c01 0a02 1401 1401 0201  ................
-00005800: 0401 04ff 02ff 0405 0201 0401 06ff 02ff  ................
-00005810: 0405 0e01 0201 0401 04ff 02ff 0405 0201  ................
-00005820: 0401 0cff 02ff 0405 0201 0401 16ff 02ff  ................
-00005830: 0405 0801 0201 0401 0cff 02ff 0405 0201  ................
-00005840: 0401 16ff 02ff 0405 0a05 0201 0aff 1403  ................
-00005850: 0e01 0a01 0e03 0a01 1401 0a02 0404 0aff  ................
-00005860: 0402 08fe 0403 02fd 0404 06fc 0406 0801  ................
-00005870: 0804 0aff 0402 08fe 0403 02fd 0404 06fc  ................
-00005880: 0406 0601 0801 0801 0801 0801 0601 1803  ................
-00005890: 0e02 16ff 0402 0afe 0406 1601 0e02 0e01  ................
-000058a0: 02fe 0a06 0201 0cff 0803 0e02 0e01 02fe  ................
-000058b0: 0a04 1803 0e01 0e01 0e02 7a15 436f 756e  ..........z.Coun
-000058c0: 7465 7266 6163 7475 616c 2e61 7474 6163  terfactual.attac
-000058d0: 6b29 0972 d700 0000 72cf 0000 0072 f300  k).r....r....r..
-000058e0: 0000 72ed 0000 0072 f400 0000 72f5 0000  ..r....r....r...
-000058f0: 0072 f600 0000 72f7 0000 0072 3100 0000  .r....r....r1...
-00005900: 6309 0000 0000 0000 0000 0000 0014 0000  c...............
-00005910: 000b 0000 0043 0000 0073 be01 0000 7400  .....C...s....t.
-00005920: 8300 7d09 6700 6401 a201 7d0a 7c0a 4400  ..}.g.d...}.|.D.
-00005930: 5d0e 7d0b 7c09 a001 7c0b a101 0100 7112  ].}.|...|.....q.
-00005940: 7c01 6a02 6402 1900 6403 6b03 7242 7403  |.j.d...d.k.rBt.
-00005950: a004 6404 7c01 6a02 6402 1900 a102 0100  ..d.|.j.d.......
-00005960: 7405 a006 7407 a101 7d0c 7c00 6a08 7260  t...t...}.|.j.r`
-00005970: 7c00 6a09 a009 7c01 a101 7d0d 6e0a 7c00  |.j...|...}.n.|.
-00005980: a009 7c01 a101 7d0d 740a a00b 7c0d 6a02  ..|...}.t...|.j.
-00005990: a101 7d0e 740a 6a0c 7c0d a00d a100 6403  ..}.t.j.|.....d.
-000059a0: 6405 8d02 7d0f 6403 7c0e 740a a00e 7c0d  d...}.d.|.t...|.
-000059b0: 6a02 6402 1900 a101 7c0f 6602 3c00 7c0e  j.d.....|.f.<.|.
-000059c0: a005 a100 7d02 7c0d 7c0c 6406 3c00 740a  ....}.|.|.d.<.t.
-000059d0: 6a0c 7c02 6403 6405 8d02 6402 1900 7c0c  j.|.d.d...d...|.
-000059e0: 6407 3c00 6408 7c00 5f0f 7c00 6a10 7c01  d.<.d.|._.|.j.|.
-000059f0: 7c02 7c03 7c04 7c05 7c00 6a11 7c06 7c07  |.|.|.|.|.j.|.|.
-00005a00: 7c08 6409 8d09 5c02 7d10 7d11 7c00 6a12  |.d...\.}.}.|.j.
-00005a10: 72fe 7c00 6a13 7c0c 640a 3c00 7c00 6a0f  r.|.j.|.d.<.|.j.
-00005a20: 9001 7328 7403 a004 640b a101 0100 7414  ..s(t...d.....t.
-00005a30: 7405 a006 7c00 6a15 a101 7c0c 640c 8d02  t...|.j...|.d...
-00005a40: 7d12 7c12 5300 7c00 6a16 7c0c 640d 3c00  }.|.S.|.j.|.d.<.
-00005a50: 6900 7c0c 640e 3c00 7c10 7c0c 640e 1900  i.|.d.<.|.|.d...
-00005a60: 640f 3c00 7c00 a009 7417 a018 7c10 a101  d.<.|...t...|...
-00005a70: a101 a00d a100 a019 a100 7d13 740a 6a0c  ..........}.t.j.
-00005a80: 7c13 6403 6405 8d02 6402 1900 7c0c 640e  |.d.d...d...|.d.
-00005a90: 1900 6410 3c00 7c13 7c0c 640e 1900 6411  ..d.<.|.|.d...d.
-00005aa0: 3c00 7c11 6402 1900 7c11 6403 1900 0200  <.|.d...|.d.....
-00005ab0: 7c0c 640e 1900 6412 3c00 7c0c 640e 1900  |.d...d.<.|.d...
-00005ac0: 6413 3c00 7414 7405 a006 7c00 6a15 a101  d.<.t.t...|.j...
-00005ad0: 7c0c 640c 8d02 7d12 7c12 5300 2914 61ab  |.d...}.|.S.).a.
-00005ae0: 0600 000a 2020 2020 2020 2020 4578 706c  ....        Expl
-00005af0: 6169 6e20 696e 7374 616e 6365 2061 6e64  ain instance and
-00005b00: 2072 6574 7572 6e20 636f 756e 7465 7266   return counterf
-00005b10: 6163 7475 616c 2077 6974 6820 6d65 7461  actual with meta
-00005b20: 6461 7461 2e0a 0a20 2020 2020 2020 2050  data...        P
-00005b30: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00005b40: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00005b50: 2020 2020 2058 0a20 2020 2020 2020 2020       X.         
-00005b60: 2020 2049 6e69 7469 616c 2070 6572 7475     Initial pertu
-00005b70: 7262 6174 696f 6e0a 2020 2020 2020 2020  rbation.        
-00005b80: 590a 2020 2020 2020 2020 2020 2020 4c61  Y.            La
-00005b90: 6265 6c73 2066 6f72 2060 5860 2061 7320  bels for `X` as 
-00005ba0: 6f6e 652d 686f 742d 656e 636f 6469 6e67  one-hot-encoding
-00005bb0: 2e0a 2020 2020 2020 2020 7461 7267 6574  ..        target
-00005bc0: 5f63 6c61 7373 0a20 2020 2020 2020 2020  _class.         
-00005bd0: 2020 204c 6973 7420 7769 7468 2074 6172     List with tar
-00005be0: 6765 7420 636c 6173 7365 7320 7573 6564  get classes used
-00005bf0: 2074 6f20 6669 6e64 2063 6c6f 7365 7374   to find closest
-00005c00: 2070 726f 746f 7479 7065 2e20 4966 2060   prototype. If `
-00005c10: 604e 6f6e 6560 602c 2074 6865 206e 6561  `None``, the nea
-00005c20: 7265 7374 2070 726f 746f 7479 7065 0a20  rest prototype. 
-00005c30: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00005c40: 7420 666f 7220 7468 6520 7072 6564 6963  t for the predic
-00005c50: 7420 636c 6173 7320 6f6e 2074 6865 2069  t class on the i
-00005c60: 6e73 7461 6e63 6520 6973 2075 7365 642e  nstance is used.
-00005c70: 0a20 2020 2020 2020 206b 0a20 2020 2020  .        k.     
-00005c80: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
-00005c90: 206e 6561 7265 7374 2069 6e73 7461 6e63   nearest instanc
-00005ca0: 6573 2075 7365 6420 746f 2064 6566 696e  es used to defin
-00005cb0: 6520 7468 6520 7072 6f74 6f74 7970 6520  e the prototype 
-00005cc0: 666f 7220 6120 636c 6173 732e 2044 6566  for a class. Def
-00005cd0: 6175 6c74 7320 746f 2075 7369 6e67 2061  aults to using a
-00005ce0: 6c6c 0a20 2020 2020 2020 2020 2020 2069  ll.            i
-00005cf0: 6e73 7461 6e63 6573 2062 656c 6f6e 6769  nstances belongi
-00005d00: 6e67 2074 6f20 7468 6520 636c 6173 7320  ng to the class 
-00005d10: 6966 2061 6e20 656e 636f 6465 7220 6973  if an encoder is
-00005d20: 2075 7365 6420 616e 6420 746f 2031 2066   used and to 1 f
-00005d30: 6f72 206b 2d64 2074 7265 6573 2e0a 2020  or k-d trees..  
-00005d40: 2020 2020 2020 6b5f 7479 7065 0a20 2020        k_type.   
-00005d50: 2020 2020 2020 2020 2055 7365 2065 6974           Use eit
-00005d60: 6865 7220 7468 6520 6176 6572 6167 6520  her the average 
-00005d70: 656e 636f 6469 6e67 206f 6620 7468 6520  encoding of the 
-00005d80: 606b 6020 6e65 6172 6573 7420 696e 7374  `k` nearest inst
-00005d90: 616e 6365 7320 696e 2061 2063 6c61 7373  ances in a class
-00005da0: 2028 6060 6b5f 7479 7065 3d27 6d65 616e   (``k_type='mean
-00005db0: 2760 6029 206f 720a 2020 2020 2020 2020  '``) or.        
-00005dc0: 2020 2020 7468 6520 6b2d 6e65 6172 6573      the k-neares
-00005dd0: 7420 656e 636f 6469 6e67 2069 6e20 7468  t encoding in th
-00005de0: 6520 636c 6173 7320 2860 606b 5f74 7970  e class (``k_typ
-00005df0: 653d 2770 6f69 6e74 2760 6029 2074 6f20  e='point'``) to 
-00005e00: 6465 6669 6e65 2074 6865 2070 726f 746f  define the proto
-00005e10: 7479 7065 206f 6620 7468 6174 2063 6c61  type of that cla
-00005e20: 7373 2e0a 2020 2020 2020 2020 2020 2020  ss..            
-00005e30: 4f6e 6c79 2072 656c 6576 616e 7420 6966  Only relevant if
-00005e40: 2061 6e20 656e 636f 6465 7220 6973 2075   an encoder is u
-00005e50: 7365 6420 746f 2064 6566 696e 6520 7468  sed to define th
-00005e60: 6520 7072 6f74 6f74 7970 6573 2e0a 2020  e prototypes..  
-00005e70: 2020 2020 2020 7468 7265 7368 6f6c 640a        threshold.
-00005e80: 2020 2020 2020 2020 2020 2020 5468 7265              Thre
-00005e90: 7368 6f6c 6420 6c65 7665 6c20 666f 7220  shold level for 
-00005ea0: 7468 6520 7261 7469 6f20 6265 7477 6565  the ratio betwee
-00005eb0: 6e20 7468 6520 6469 7374 616e 6365 206f  n the distance o
-00005ec0: 6620 7468 6520 636f 756e 7465 7266 6163  f the counterfac
-00005ed0: 7475 616c 2074 6f20 7468 6520 7072 6f74  tual to the prot
-00005ee0: 6f74 7970 6520 6f66 2074 6865 0a20 2020  otype of the.   
-00005ef0: 2020 2020 2020 2020 2070 7265 6469 6374           predict
-00005f00: 6564 2063 6c61 7373 2066 6f72 2074 6865  ed class for the
-00005f10: 206f 7269 6769 6e61 6c20 696e 7374 616e   original instan
-00005f20: 6365 206f 7665 7220 7468 6520 6469 7374  ce over the dist
-00005f30: 616e 6365 2074 6f20 7468 6520 7072 6f74  ance to the prot
-00005f40: 6f74 7970 6520 6f66 2074 6865 2070 7265  otype of the pre
-00005f50: 6469 6374 6564 2063 6c61 7373 0a20 2020  dicted class.   
-00005f60: 2020 2020 2020 2020 2066 6f72 2074 6865           for the
-00005f70: 2063 6f75 6e74 6572 6661 6374 7561 6c2e   counterfactual.
-00005f80: 2049 6620 7468 6520 7472 7573 7420 7363   If the trust sc
-00005f90: 6f72 6520 6973 2062 656c 6f77 2074 6865  ore is below the
-00005fa0: 2074 6872 6573 686f 6c64 2c20 7468 6520   threshold, the 
-00005fb0: 7072 6f70 6f73 6564 2063 6f75 6e74 6572  proposed counter
-00005fc0: 6661 6374 7561 6c20 646f 6573 0a20 2020  factual does.   
-00005fd0: 2020 2020 2020 2020 206e 6f74 206d 6565           not mee
-00005fe0: 7420 7468 6520 7265 7175 6972 656d 656e  t the requiremen
-00005ff0: 7473 2e0a 2020 2020 2020 2020 7665 7262  ts..        verb
-00006000: 6f73 650a 2020 2020 2020 2020 2020 2020  ose.            
-00006010: 5072 696e 7420 696e 7465 726d 6564 6961  Print intermedia
-00006020: 7465 2072 6573 756c 7473 206f 6620 6f70  te results of op
-00006030: 7469 6d69 7a61 7469 6f6e 2069 6620 6060  timization if ``
-00006040: 5472 7565 6060 2e0a 2020 2020 2020 2020  True``..        
-00006050: 7072 696e 745f 6576 6572 790a 2020 2020  print_every.    
-00006060: 2020 2020 2020 2020 5072 696e 7420 6672          Print fr
-00006070: 6571 7565 6e63 7920 6966 2076 6572 626f  equency if verbo
-00006080: 7365 2069 7320 6060 5472 7565 6060 2e0a  se is ``True``..
-00006090: 2020 2020 2020 2020 6c6f 675f 6576 6572          log_ever
-000060a0: 790a 2020 2020 2020 2020 2020 2020 6074  y.            `t
-000060b0: 656e 736f 7262 6f61 7264 6020 6c6f 6720  ensorboard` log 
-000060c0: 6672 6571 7565 6e63 7920 6966 2077 7269  frequency if wri
-000060d0: 7465 2064 6972 6563 746f 7279 2069 7320  te directory is 
-000060e0: 7370 6563 6966 6965 640a 0a20 2020 2020  specified..     
-000060f0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00006100: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00006110: 2020 2065 7870 6c61 6e61 7469 6f6e 0a20     explanation. 
-00006120: 2020 2020 2020 2020 2020 2060 4578 706c             `Expl
-00006130: 616e 6174 696f 6e60 206f 626a 6563 7420  anation` object 
-00006140: 636f 6e74 6169 6e69 6e67 2074 6865 2063  containing the c
-00006150: 6f75 6e74 6572 6661 6374 7561 6c20 7769  ounterfactual wi
-00006160: 7468 2061 6464 6974 696f 6e61 6c20 6d65  th additional me
-00006170: 7461 6461 7461 2061 7320 6174 7472 6962  tadata as attrib
-00006180: 7574 6573 2e0a 2020 2020 2020 2020 2903  utes..        ).
-00006190: 7234 0000 0072 d700 0000 72cf 0000 0072  r4...r....r....r
-000061a0: 0100 0000 721a 0000 007a 5943 7572 7265  ....r....zYCurre
-000061b0: 6e74 6c79 206f 6e6c 7920 7369 6e67 6c65  ntly only single
-000061c0: 2069 6e73 7461 6e63 6520 6578 706c 616e   instance explan
-000061d0: 6174 696f 6e73 2073 7570 706f 7274 6564  ations supported
-000061e0: 2028 6669 7273 7420 6469 6d20 3d20 3129   (first dim = 1)
-000061f0: 2c20 6275 7420 6669 7273 7420 6469 6d20  , but first dim 
-00006200: 3d20 2573 7259 0000 00da 0a6f 7269 675f  = %srY.....orig_
-00006210: 7072 6f62 6172 eb00 0000 4629 0872 cf00  probar....F).r..
-00006220: 0000 72f3 0000 0072 ed00 0000 72f4 0000  ..r....r....r...
-00006230: 0072 3000 0000 72f5 0000 0072 f600 0000  .r0...r....r....
-00006240: 72f7 0000 0072 0801 0000 7a18 4e6f 2063  r....r....z.No c
-00006250: 6f75 6e74 6572 6661 6374 7561 6c20 666f  ounterfactual fo
-00006260: 756e 6421 2902 7232 0000 00da 0464 6174  und!).r2.....dat
-00006270: 61da 0361 6c6c da02 6366 72d7 0000 00da  a..all..cfr.....
-00006280: 0563 6c61 7373 72d9 0000 0072 1801 0000  .classr....r....
-00006290: 7217 0100 0029 1a72 6c00 0000 726d 0000  r....).rl...rm..
-000062a0: 0072 1d00 0000 727b 0000 0072 7c00 0000  .r....r{...r|...
-000062b0: 7269 0000 0072 6a00 0000 7208 0000 0072  ri...rj...r....r
-000062c0: 7600 0000 721b 0000 0072 3f00 0000 7277  v...r....r?...rw
-000062d0: 0000 0072 fb00 0000 72e2 0000 0072 9a00  ...r....r....r..
-000062e0: 0000 7213 0100 0072 1e01 0000 7230 0000  ..r....r....r0..
-000062f0: 0072 3b00 0000 7208 0100 0072 0b00 0000  .r;...r....r....
-00006300: 7232 0000 0072 0901 0000 7279 0000 0072  r2...r....ry...r
-00006310: e100 0000 72e3 0000 0029 1472 3400 0000  ....r....).r4...
-00006320: 72d7 0000 0072 cf00 0000 72f3 0000 0072  r....r....r....r
-00006330: ed00 0000 72f4 0000 0072 f500 0000 72f6  ....r....r....r.
-00006340: 0000 0072 f700 0000 7236 0000 0072 b700  ...r....r6...r..
-00006350: 0000 72b8 0000 0072 2001 0000 5a07 595f  ..r....r ...Z.Y_
-00006360: 7072 6f62 615a 0559 5f6f 6865 721d 0100  probaZ.Y_oher...
-00006370: 0072 1301 0000 72e7 0000 00da 0b65 7870  .r....r......exp
-00006380: 6c61 6e61 7469 6f6e 5a06 595f 7065 7274  lanationZ.Y_pert
-00006390: 7244 0000 0072 4400 0000 7245 0000 00da  rD...rD...rE....
-000063a0: 0765 7870 6c61 696e 0b04 0000 735c 0000  .explain....s\..
-000063b0: 0000 3106 0108 0108 010c 020e 0104 0102  ..1.............
-000063c0: 0208 fd04 070a 0306 010e 020a 010c 0112  ................
-000063d0: 0118 0108 0108 0316 0306 0104 0102 0102  ................
-000063e0: 0102 0102 0102 0104 0102 0102 0102 f70a  ................
-000063f0: 0c06 010a 0308 010a 0314 0104 020a 0108  ................
-00006400: 010c 0118 011a 010c 0122 0314 027a 1643  ........."...z.C
-00006410: 6f75 6e74 6572 6661 6374 7561 6c2e 6578  ounterfactual.ex
-00006420: 706c 6169 6e29 1372 0f00 0000 7210 0000  plain).r....r...
-00006430: 0072 1100 0000 720f 0000 004e 4e72 0f00  .r....r....NNr..
-00006440: 0000 4672 1300 0000 7214 0000 0072 1500  ..Fr....r....r..
-00006450: 0000 7216 0000 0072 1700 0000 7219 0000  ..r....r....r...
-00006460: 0072 1a00 0000 4e4e 4e46 2901 72e9 0000  .r....NNNF).r...
-00006470: 0029 074e 4e72 c700 0000 720f 0000 0046  .).NNr....r....F
-00006480: 72f2 0000 0072 f200 0000 2907 4e4e 4e72  r....r....).NNNr
-00006490: c700 0000 720f 0000 0072 f200 0000 72f2  ....r....r....r.
-000064a0: 0000 0029 1eda 085f 5f6e 616d 655f 5fda  ...)...__name__.
-000064b0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000064c0: 7561 6c6e 616d 655f 5f72 0600 0000 7203  ualname__r....r.
-000064d0: 0000 0072 3f00 0000 7201 0100 0072 6f00  ...r?...r....ro.
-000064e0: 0000 7270 0000 0072 7100 0000 7281 0000  ..rp...rq...r...
-000064f0: 0072 3e00 0000 7205 0000 0072 0400 0000  .r>...r....r....
-00006500: 7202 0100 0072 f900 0000 da03 7374 7272  r....r......strr
-00006510: 7500 0000 7268 0000 0072 4100 0000 da04  u...rh...rA.....
-00006520: 6469 6374 72ce 0000 0072 d600 0000 72e8  dictr....r....r.
-00006530: 0000 0072 f100 0000 7299 0000 0072 1e01  ...r....r....r..
-00006540: 0000 720b 0000 0072 2501 0000 da0d 5f5f  ..r....r%.....__
-00006550: 636c 6173 7363 656c 6c5f 5f72 4400 0000  classcell__rD...
-00006560: 7244 0000 0072 bf00 0000 7245 0000 0072  rD...r....rE...r
-00006570: 0e00 0000 1600 0000 73d2 0000 0008 0700  ........s.......
-00006580: 0100 0100 0400 0100 0100 0100 0100 0100  ................
-00006590: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-000065a0: 0100 0100 e602 021c 011c 0102 0102 0102  ................
-000065b0: 011e 0402 010a 010a 0102 0102 0102 0102  ................
-000065c0: 0102 0102 0102 0102 0102 0106 0106 0108  ................
-000065d0: 0102 0102 e510 7f00 7f00 7f00 4208 0108  ............B...
-000065e0: 0102 fc02 0204 0104 0106 0102 fb0c 2918  ..............).
-000065f0: 1a0a 0104 fe0c 4500 ff02 010a 0102 fe0c  ......E.........
-00006600: 2900 0100 0100 0100 0100 0100 0100 f602  )...............
-00006610: 0204 0104 0106 0106 0102 0102 0102 0102  ................
-00006620: 0102 0118 f50c 7f00 7f00 7f00 1200 0100  ................
-00006630: 0100 0100 0100 0100 0100 f602 0304 0108  ................
-00006640: 0106 0106 0102 0102 0102 0102 0102 f572  ...............r
-00006650: 0e00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00006660: 0003 0000 0008 0000 0043 0000 0073 3c00  .........C...s<.
-00006670: 0000 7400 7c01 6401 8302 8f1e 7d02 7401  ..t.|.d.....}.t.
-00006680: a002 7c00 7c02 6402 a103 0100 5700 6400  ..|.|.d.....W.d.
-00006690: 0400 0400 8303 0100 6e10 3100 732e 3000  ........n.1.s.0.
-000066a0: 0100 0100 0100 5900 0100 6400 5300 2903  ......Y...d.S.).
-000066b0: 4eda 0277 6272 3300 0000 2903 da04 6f70  N..wbr3...)...op
-000066c0: 656e da06 7069 636b 6c65 da04 6475 6d70  en..pickle..dump
-000066d0: 2903 da03 6f62 6ada 0866 696c 656e 616d  )...obj..filenam
-000066e0: 65da 046f 7574 7072 4400 0000 7244 0000  e..outprD...rD..
-000066f0: 0072 4500 0000 da0b 7361 7665 5f6f 626a  .rE.....save_obj
-00006700: 6563 7480 0400 0073 0400 0000 0001 0c01  ect....s........
-00006710: 7233 0100 0063 0100 0000 0000 0000 0000  r3...c..........
-00006720: 0000 0200 0000 0800 0000 4300 0000 7338  ..........C...s8
-00006730: 0000 0074 007c 0064 0183 028f 1a7d 0174  ...t.|.d.....}.t
-00006740: 01a0 027c 01a1 0157 0002 0064 0004 0004  ...|...W...d....
-00006750: 0083 0301 0053 0031 0073 2a30 0001 0001  .....S.1.s*0....
-00006760: 0001 0059 0001 0064 0053 0029 024e da02  ...Y...d.S.).N..
-00006770: 7262 2903 722d 0100 0072 2e01 0000 da04  rb).r-...r......
-00006780: 6c6f 6164 2902 7231 0100 0072 3201 0000  load).r1...r2...
-00006790: 7244 0000 0072 4400 0000 7245 0000 0072  rD...rD...rE...r
-000067a0: c800 0000 8504 0000 7304 0000 0000 010c  ........s.......
-000067b0: 0172 c800 0000 2925 da02 6f73 7269 0000  .r....)%..osri..
-000067c0: 00da 076c 6f67 6769 6e67 720f 0100 00da  ...loggingr.....
-000067d0: 075f 7069 636b 6c65 722e 0100 00da 0674  ._pickler......t
-000067e0: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
-000067f0: 0400 0000 7205 0000 0072 0600 0000 72e3  ....r....r....r.
-00006800: 0000 0072 3f00 0000 5a14 7465 6e73 6f72  ...r?...Z.tensor
-00006810: 666c 6f77 2e63 6f6d 7061 742e 7631 7272  flow.compat.v1rr
-00006820: 0000 0072 7300 0000 726f 0000 005a 0c61  ...rs...ro...Z.a
-00006830: 7069 2e64 6566 6175 6c74 7372 0800 0000  pi.defaultsr....
-00006840: 7209 0000 005a 0e61 7069 2e69 6e74 6572  r....Z.api.inter
-00006850: 6661 6365 7372 0a00 0000 720b 0000 0072  facesr....r....r
-00006860: 0c00 0000 5a0f 7574 696c 732e 6772 6164  ....Z.utils.grad
-00006870: 6965 6e74 7372 0d00 0000 7279 0000 00da  ientsr....ry....
-00006880: 0967 6574 4c6f 6767 6572 7226 0100 0072  .getLoggerr&...r
-00006890: 7b00 0000 5a0d 7365 745f 7665 7262 6f73  {...Z.set_verbos
-000068a0: 6974 79da 0545 5252 4f52 5a17 6469 7361  ity..ERRORZ.disa
-000068b0: 626c 655f 6561 6765 725f 6578 6563 7574  ble_eager_execut
-000068c0: 696f 6e72 0e00 0000 7233 0100 0072 c800  ionr....r3...r..
-000068d0: 0000 7244 0000 0072 4400 0000 7244 0000  ..rD...rD...rD..
-000068e0: 0072 4500 0000 da08 3c6d 6f64 756c 653e  .rE.....<module>
-000068f0: 0100 0000 7332 0000 0008 0108 0108 0108  ....s2..........
-00006900: 0108 011c 0108 0112 0210 0114 010c 0108  ................
-00006910: 020a 0110 030c 0312 7f00 7f00 7f00 7f00  ................
-00006920: 7f00 7f00 7f00 7f00 7208 05              ........r..
+00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
+00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6400  m.Z.m.Z.m.Z...d.
+00000060: 6401 6c09 5a0a 6400 6401 6c0b 5a0b 6400  d.l.Z.d.d.l.Z.d.
+00000070: 6401 6c0c 5a0c 6400 6401 6c0d 6d0e 5a0e  d.l.Z.d.d.l.m.Z.
+00000080: 0100 6403 6404 6c0f 6d10 5a10 6d11 5a11  ..d.d.l.m.Z.m.Z.
+00000090: 0100 6403 6405 6c12 6d13 5a13 6d14 5a14  ..d.d.l.m.Z.m.Z.
+000000a0: 6d15 5a15 0100 6403 6406 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
+000000b0: 0100 4700 6407 6408 8400 6408 6513 6515  ..G.d.d...d.e.e.
+000000c0: 8304 5a18 6409 640a 8400 5a19 640b 640c  ..Z.d.d...Z.d.d.
+000000d0: 8400 5a1a 640f 640d 640e 8401 5a1b 6401  ..Z.d.d.d...Z.d.
+000000e0: 5300 2910 e900 0000 004e 2904 da08 4361  S.)......N)...Ca
+000000f0: 6c6c 6162 6c65 da08 4f70 7469 6f6e 616c  llable..Optional
+00000100: da05 5475 706c 65da 0555 6e69 6f6e e902  ..Tuple..Union..
+00000110: 0000 0029 02da 0c44 4546 4155 4c54 5f44  ...)...DEFAULT_D
+00000120: 4154 41da 0c44 4546 4155 4c54 5f4d 4554  ATA..DEFAULT_MET
+00000130: 4129 03da 0945 7870 6c61 696e 6572 da0b  A)...Explainer..
+00000140: 4578 706c 616e 6174 696f 6eda 0846 6974  Explanation..Fit
+00000150: 4d69 7869 6e29 01da 0770 6572 7475 7262  Mixin)...perturb
+00000160: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000170: 0019 0000 0000 0000 0073 e601 0000 6500  .........s....e.
+00000180: 5a01 6400 5a02 643a 6503 6504 6505 6a06  Z.d.Z.d:e.e.e.j.
+00000190: 6701 6505 6a06 6602 1900 6507 6a08 6a09  g.e.j.f...e.j.j.
+000001a0: 6602 1900 6503 6504 6505 6a06 6701 6505  f...e.e.e.j.g.e.
+000001b0: 6a06 6602 1900 6507 6a08 6a09 6602 1900  j.f...e.j.j.f...
+000001c0: 650a 650b 650b 650c 6503 650b 6505 6a06  e.e.e.e.e.e.e.j.
+000001d0: 6602 1900 6503 650b 6505 6a06 6602 1900  f...e.e.e.j.f...
+000001e0: 6602 1900 650b 650d 6507 6a08 6a09 1900  f...e.e.e.j.j...
+000001f0: 650d 6507 6a08 6a09 1900 650b 650e 650b  e.e.j.j...e.e.e.
+00000200: 650f 650b 650f 650a 650a 650f 650d 6510  e.e.e.e.e.e.e.e.
+00000210: 1900 650f 650e 6510 6404 640f 9c17 8700  ..e.e.e.d.d.....
+00000220: 6601 6410 6411 840d 5a11 6412 6413 8400  f.d.d...Z.d.d...
+00000230: 5a12 6414 6415 8400 5a13 6416 6417 8400  Z.d.d...Z.d.d...
+00000240: 5a14 6418 6419 8400 5a15 641a 641b 8400  Z.d.d...Z.d.d...
+00000250: 5a16 641c 641d 8400 5a17 641e 641f 8400  Z.d.d...Z.d.d...
+00000260: 5a18 6420 6421 8400 5a19 6422 6423 8400  Z.d d!..Z.d"d#..
+00000270: 5a1a 6507 6a1b 6507 6a1b 6507 6a1b 6424  Z.e.j.e.j.e.j.d$
+00000280: 9c03 6425 6426 8404 5a1c 6427 6428 8400  ..d%d&..Z.d'd(..
+00000290: 5a1d 6505 a01e 6700 a101 6505 a01e 6700  Z.e...g...e...g.
+000002a0: a101 6602 6505 6a06 6505 6a06 6400 6429  ..f.e.j.e.j.d.d)
+000002b0: 9c03 642a 642b 8405 5a1f 6505 6a06 6505  ..d*d+..Z.e.j.e.
+000002c0: 6a06 650a 6505 6a06 642c 9c04 642d 642e  j.e.e.j.d,..d-d.
+000002d0: 8404 5a20 643b 6505 6a06 650f 650f 650b  ..Z d;e.j.e.e.e.
+000002e0: 650b 6430 9c05 6431 6432 8405 5a21 643c  e.d0..d1d2..Z!d<
+000002f0: 6505 6a06 6505 6a06 650d 6522 1900 650d  e.j.e.j.e.e"..e.
+00000300: 650f 1900 6510 650b 650f 650c 6505 6a06  e...e.e.e.e.e.j.
+00000310: 650c 6505 6a06 6505 6a06 6602 1900 6602  e.e.j.e.j.f...f.
+00000320: 1900 6435 9c08 6436 6437 8405 5a23 643d  ..d5..d6d7..Z#d=
+00000330: 6505 6a06 650d 6505 6a06 1900 650d 6522  e.j.e.e.j...e.e"
+00000340: 1900 650d 650f 1900 6510 650b 650f 6524  ..e.e...e.e.e.e$
+00000350: 6435 9c08 6438 6439 8405 5a25 8700 0400  d5..d8d9..Z%....
+00000360: 5a26 5300 293e da0e 436f 756e 7465 7266  Z&S.)>..Counterf
+00000370: 6163 7475 616c e700 0000 0000 0000 00e7  actual..........
+00000380: 9a99 9999 9999 b93f a902 6700 0000 205f  .......?..g... _
+00000390: a002 c2e7 0000 0020 5fa0 0242 4e46 e77b  ....... _..BNF.{
+000003a0: 14ae 47e1 7a84 3fe9 e803 0000 e700 0000  ..G.z.?.........
+000003b0: 0000 0024 40e9 0a00 0000 a902 e7fc a9f1  ...$@...........
+000003c0: d24d 6250 3f72 1700 0000 a902 6700 0000  .MbP?r......g...
+000003d0: 0000 408f c067 0000 0000 0040 8f40 e901  ..@..g.....@.@..
+000003e0: 0000 0072 0100 0000 5429 17da 0770 7265  ...r....T)...pre
+000003f0: 6469 6374 da0f 696e 7075 745f 7472 616e  dict..input_tran
+00000400: 7366 6f72 6dda 0573 6861 7065 da05 6b61  sform..shape..ka
+00000410: 7070 61da 0462 6574 61da 0d66 6561 7475  ppa..beta..featu
+00000420: 7265 5f72 616e 6765 da05 6761 6d6d 61da  re_range..gamma.
+00000430: 0861 655f 6d6f 6465 6cda 0965 6e63 5f6d  .ae_model..enc_m
+00000440: 6f64 656c da05 7468 6574 61da 0a75 7365  odel..theta..use
+00000450: 5f6b 6474 7265 65da 126c 6561 726e 696e  _kdtree..learnin
+00000460: 675f 7261 7465 5f69 6e69 74da 0e6d 6178  g_rate_init..max
+00000470: 5f69 7465 7261 7469 6f6e 73da 0663 5f69  _iterations..c_i
+00000480: 6e69 74da 0763 5f73 7465 7073 da03 6570  nit..c_steps..ep
+00000490: 73da 0463 6c69 70da 0f75 7064 6174 655f  s..clip..update_
+000004a0: 6e75 6d5f 6772 6164 da0a 7472 7573 7473  num_grad..trusts
+000004b0: 636f 7265 da09 7665 7262 6f73 6974 79da  core..verbosity.
+000004c0: 0e6e 756d 6572 6963 616c 5f64 6966 66da  .numerical_diff.
+000004d0: 0664 6576 6963 65da 0672 6574 7572 6e63  .device..returnc
+000004e0: 1700 0000 0000 0000 0000 0000 1d00 0000  ................
+000004f0: 0500 0000 0300 0000 7312 0200 0074 0083  ........s....t..
+00000500: 006a 0174 02a0 0374 04a1 0164 018d 0101  .j.t...t...d....
+00000510: 0074 0583 007d 1767 0064 02a2 017d 187c  .t...}.g.d...}.|
+00000520: 1844 005d 0e7d 197c 17a0 067c 19a1 0101  .D.].}.|...|....
+00000530: 0071 267c 006a 0764 0319 00a0 087c 17a1  .q&|.j.d.....|..
+00000540: 0101 007c 017c 005f 097c 137c 005f 0a7c  ...|.|._.|.|._.|
+00000550: 157c 005f 0b7c 1664 0475 0172 647c 166e  .|._.|.d.u.rd|.n
+00000560: 1674 0ca0 0d74 0c6a 0ea0 0fa1 0072 7664  .t...t.j.....rvd
+00000570: 056e 0264 06a1 017c 005f 0d64 077d 1a7c  .n.d...|._.d.}.|
+00000580: 1a72 a27c 00a0 0974 0c6a 1088 0164 088d  .r.|...t.j...d..
+00000590: 01a1 016a 1164 0919 007c 005f 126e 2064  ...j.d...|._.n d
+000005a0: 077c 005f 0b7c 006a 09a0 0974 13a0 1088  .|._.|.j...t....
+000005b0: 01a1 01a1 016a 1164 0919 007c 005f 1274  .....j.d...|._.t
+000005c0: 147c 0874 0c6a 156a 1683 027d 1b74 147c  .|.t.j.j...}.t.|
+000005d0: 0974 0c6a 156a 1683 027d 1c7c 1c72 ea64  .t.j.j...}.|.r.d
+000005e0: 077c 005f 176e 0664 0a7c 005f 177c 1b72  .|._.n.d.|._.|.r
+000005f0: fc64 077c 005f 186e 0664 0a7c 005f 187c  .d.|._.n.d.|._.|
+00000600: 0b90 0172 1a7c 006a 1790 0172 1a74 19a0  ...r.|.j...r.t..
+00000610: 1a64 0ba1 0101 007c 0b90 0173 287c 006a  .d.....|...s(|.j
+00000620: 1790 0172 3064 077c 005f 1b6e 0664 0a7c  ...r0d.|._.n.d.|
+00000630: 005f 1b7c 006a 0764 0319 006a 087c 006a  ._.|.j.d...j.|.j
+00000640: 1b64 0c8d 0101 0088 017c 005f 117c 047c  .d.......|._.|.|
+00000650: 005f 1c7c 057c 005f 1d7c 077c 005f 1e7c  ._.|.|._.|.|._.|
+00000660: 0a7c 005f 1f7c 087c 005f 207c 097c 005f  .|._.|.|._ |.|._
+00000670: 217c 0b7c 005f 2288 0164 0d19 007c 005f  !|.|._"..d...|._
+00000680: 237c 0d7c 005f 2474 0ca0 257c 0ea1 017c  #|.|._$t..%|...|
+00000690: 005f 267c 0f7c 005f 2774 2887 0087 0166  ._&|.|._'t(....f
+000006a0: 0264 0e64 0f84 0874 2964 1083 0144 0083  .d.d...t)d...D..
+000006b0: 0183 017c 005f 2a7c 127c 005f 2b7c 107c  ...|._*|.|._+|.|
+000006c0: 005f 2c7c 117c 005f 2d7c 027c 005f 2e7c  ._,|.|._-|.|._.|
+000006d0: 0c7c 005f 2f7c 147c 005f 307c 006a 1790  .|._/|.|._0|.j..
+000006e0: 0272 007c 006a 21a0 0974 13a0 107c 006a  .r.|.j!..t...|.j
+000006f0: 11a1 01a1 016a 117c 005f 316e 087c 006a  .....j.|._1n.|.j
+00000700: 117c 005f 3174 3274 195f 3364 0453 0029  .|._1t2t._3d.S.)
+00000710: 1161 4709 0000 0a20 2020 2020 2020 2049  .aG....        I
+00000720: 6e69 7469 616c 697a 6520 7072 6f74 6f74  nitialize protot
+00000730: 7970 6963 616c 2063 6f75 6e74 6572 6661  ypical counterfa
+00000740: 6374 7561 6c20 6d65 7468 6f64 2e0a 0a20  ctual method... 
+00000750: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00000760: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00000770: 2d2d 2d2d 0a20 2020 2020 2020 2070 7265  ----.        pre
+00000780: 6469 6374 0a20 2020 2020 2020 2020 2020  dict.           
+00000790: 2060 7079 746f 7263 6860 206d 6f64 656c   `pytorch` model
+000007a0: 2773 2070 7265 6469 6374 696f 6e20 6675  's prediction fu
+000007b0: 6e63 7469 6f6e 2072 6574 7572 6e69 6e67  nction returning
+000007c0: 2063 6c61 7373 2070 726f 6261 6269 6c69   class probabili
+000007d0: 7469 6573 2e0a 2020 2020 2020 2020 7368  ties..        sh
+000007e0: 6170 650a 2020 2020 2020 2020 2020 2020  ape.            
+000007f0: 5368 6170 6520 6f66 2069 6e70 7574 2064  Shape of input d
+00000800: 6174 6120 7374 6172 7469 6e67 2077 6974  ata starting wit
+00000810: 6820 6261 7463 6820 7369 7a65 2e0a 2020  h batch size..  
+00000820: 2020 2020 2020 6b61 7070 610a 2020 2020        kappa.    
+00000830: 2020 2020 2020 2020 436f 6e66 6964 656e          Confiden
+00000840: 6365 2070 6172 616d 6574 6572 2066 6f72  ce parameter for
+00000850: 2074 6865 2061 7474 6163 6b20 6c6f 7373   the attack loss
+00000860: 2074 6572 6d2e 0a20 2020 2020 2020 2062   term..        b
+00000870: 6574 610a 2020 2020 2020 2020 2020 2020  eta.            
+00000880: 5265 6775 6c61 7269 7a61 7469 6f6e 2063  Regularization c
+00000890: 6f6e 7374 616e 7420 666f 7220 4c31 206c  onstant for L1 l
+000008a0: 6f73 7320 7465 726d 2e0a 2020 2020 2020  oss term..      
+000008b0: 2020 6665 6174 7572 655f 7261 6e67 650a    feature_range.
+000008c0: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
+000008d0: 6520 7769 7468 2060 6d69 6e60 2061 6e64  e with `min` and
+000008e0: 2060 6d61 7860 2072 616e 6765 7320 746f   `max` ranges to
+000008f0: 2061 6c6c 6f77 2066 6f72 2070 6572 7475   allow for pertu
+00000900: 7262 6564 2069 6e73 7461 6e63 6573 2e20  rbed instances. 
+00000910: 604d 696e 6020 616e 6420 606d 6178 6020  `Min` and `max` 
+00000920: 7261 6e67 6573 2063 616e 2062 6520 6066  ranges can be `f
+00000930: 6c6f 6174 600a 2020 2020 2020 2020 2020  loat`.          
+00000940: 2020 6f72 2060 6e75 6d70 7960 2061 7272    or `numpy` arr
+00000950: 6179 7320 7769 7468 2064 696d 656e 7369  ays with dimensi
+00000960: 6f6e 2028 3178 206e 6220 6f66 2066 6561  on (1x nb of fea
+00000970: 7475 7265 7329 2066 6f72 2066 6561 7475  tures) for featu
+00000980: 7265 2d77 6973 6520 7261 6e67 6573 2e0a  re-wise ranges..
+00000990: 2020 2020 2020 2020 6761 6d6d 610a 2020          gamma.  
+000009a0: 2020 2020 2020 2020 2020 5265 6775 6c61            Regula
+000009b0: 7269 7a61 7469 6f6e 2063 6f6e 7374 616e  rization constan
+000009c0: 7420 666f 7220 6f70 7469 6f6e 616c 2061  t for optional a
+000009d0: 7574 6f2d 656e 636f 6465 7220 6c6f 7373  uto-encoder loss
+000009e0: 2074 6572 6d2e 0a20 2020 2020 2020 2061   term..        a
+000009f0: 655f 6d6f 6465 6c0a 2020 2020 2020 2020  e_model.        
+00000a00: 2020 2020 4f70 7469 6f6e 616c 2061 7574      Optional aut
+00000a10: 6f2d 656e 636f 6465 7220 6d6f 6465 6c20  o-encoder model 
+00000a20: 7573 6564 2066 6f72 206c 6f73 7320 7265  used for loss re
+00000a30: 6775 6c61 7269 7a61 7469 6f6e 2e0a 2020  gularization..  
+00000a40: 2020 2020 2020 656e 635f 6d6f 6465 6c0a        enc_model.
+00000a50: 2020 2020 2020 2020 2020 2020 4f70 7469              Opti
+00000a60: 6f6e 616c 2065 6e63 6f64 6572 206d 6f64  onal encoder mod
+00000a70: 656c 2075 7365 6420 746f 2067 7569 6465  el used to guide
+00000a80: 2069 6e73 7461 6e63 6520 7065 7274 7572   instance pertur
+00000a90: 6261 7469 6f6e 7320 746f 7761 7264 7320  bations towards 
+00000aa0: 6120 636c 6173 7320 7072 6f74 6f74 7970  a class prototyp
+00000ab0: 652e 0a20 2020 2020 2020 2074 6865 7461  e..        theta
+00000ac0: 0a20 2020 2020 2020 2020 2020 2043 6f6e  .            Con
+00000ad0: 7374 616e 7420 666f 7220 7468 6520 7072  stant for the pr
+00000ae0: 6f74 6f74 7970 6520 7365 6172 6368 206c  ototype search l
+00000af0: 6f73 7320 7465 726d 2e0a 2020 2020 2020  oss term..      
+00000b00: 2020 7573 655f 6b64 7472 6565 0a20 2020    use_kdtree.   
+00000b10: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
+00000b20: 2074 6f20 7573 6520 6b2d 6420 7472 6565   to use k-d tree
+00000b30: 7320 666f 7220 7468 6520 7072 6f74 6f74  s for the protot
+00000b40: 7970 6520 6c6f 7373 2074 6572 6d20 6966  ype loss term if
+00000b50: 206e 6f20 656e 636f 6465 7220 6973 2061   no encoder is a
+00000b60: 7661 696c 6162 6c65 2e0a 2020 2020 2020  vailable..      
+00000b70: 2020 6c65 6172 6e69 6e67 5f72 6174 655f    learning_rate_
+00000b80: 696e 6974 0a20 2020 2020 2020 2020 2020  init.           
+00000b90: 2049 6e69 7469 616c 206c 6561 726e 696e   Initial learnin
+00000ba0: 6720 7261 7465 206f 6620 6f70 7469 6d69  g rate of optimi
+00000bb0: 7a65 722e 0a20 2020 2020 2020 206d 6178  zer..        max
+00000bc0: 5f69 7465 7261 7469 6f6e 730a 2020 2020  _iterations.    
+00000bd0: 2020 2020 2020 2020 4d61 7869 6d75 6d20          Maximum 
+00000be0: 6e75 6d62 6572 206f 6620 6974 6572 6174  number of iterat
+00000bf0: 696f 6e73 2066 6f72 2066 696e 6469 6e67  ions for finding
+00000c00: 2061 2063 6f75 6e74 6572 6661 6374 7561   a counterfactua
+00000c10: 6c2e 0a20 2020 2020 2020 2063 5f69 6e69  l..        c_ini
+00000c20: 740a 2020 2020 2020 2020 2020 2020 496e  t.            In
+00000c30: 6974 6961 6c20 7661 6c75 6520 746f 2073  itial value to s
+00000c40: 6361 6c65 2074 6865 2061 7474 6163 6b20  cale the attack 
+00000c50: 6c6f 7373 2074 6572 6d2e 0a20 2020 2020  loss term..     
+00000c60: 2020 2063 5f73 7465 7073 0a20 2020 2020     c_steps.     
+00000c70: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
+00000c80: 2069 7465 7261 7469 6f6e 7320 746f 2061   iterations to a
+00000c90: 646a 7573 7420 7468 6520 636f 6e73 7461  djust the consta
+00000ca0: 6e74 2073 6361 6c69 6e67 2074 6865 2061  nt scaling the a
+00000cb0: 7474 6163 6b20 6c6f 7373 2074 6572 6d2e  ttack loss term.
+00000cc0: 0a20 2020 2020 2020 2065 7073 0a20 2020  .        eps.   
+00000cd0: 2020 2020 2020 2020 2049 6620 6e75 6d65           If nume
+00000ce0: 7269 6361 6c20 6772 6164 6965 6e74 7320  rical gradients 
+00000cf0: 6172 6520 7573 6564 2074 6f20 636f 6d70  are used to comp
+00000d00: 7574 6520 6064 4c2f 6478 203d 2028 644c  ute `dL/dx = (dL
+00000d10: 2f64 7029 202a 2028 6470 2f64 7829 602c  /dp) * (dp/dx)`,
+00000d20: 2074 6865 6e20 6065 7073 5b30 5d60 2069   then `eps[0]` i
+00000d30: 7320 7573 6564 2074 6f0a 2020 2020 2020  s used to.      
+00000d40: 2020 2020 2020 6361 6c63 756c 6174 6520        calculate 
+00000d50: 6064 4c2f 6470 6020 616e 6420 6065 7073  `dL/dp` and `eps
+00000d60: 5b31 5d60 2069 7320 7573 6564 2066 6f72  [1]` is used for
+00000d70: 2060 6470 2f64 7860 2e20 6065 7073 5b30   `dp/dx`. `eps[0
+00000d80: 5d60 2061 6e64 2060 6570 735b 315d 6020  ]` and `eps[1]` 
+00000d90: 6361 6e20 6265 2061 2063 6f6d 6269 6e61  can be a combina
+00000da0: 7469 6f6e 206f 6620 6066 6c6f 6174 600a  tion of `float`.
+00000db0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00000dc0: 6573 2061 6e64 2060 6e75 6d70 7960 2061  es and `numpy` a
+00000dd0: 7272 6179 732e 2046 6f72 2060 6570 735b  rrays. For `eps[
+00000de0: 305d 602c 2074 6865 2061 7272 6179 2064  0]`, the array d
+00000df0: 696d 656e 7369 6f6e 2073 686f 756c 6420  imension should 
+00000e00: 6265 2028 3178 206e 6220 6f66 2070 7265  be (1x nb of pre
+00000e10: 6469 6374 696f 6e20 6361 7465 676f 7269  diction categori
+00000e20: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
+00000e30: 616e 6420 666f 7220 6065 7073 5b31 5d60  and for `eps[1]`
+00000e40: 2069 7420 7368 6f75 6c64 2062 6520 2831   it should be (1
+00000e50: 7820 6e62 206f 6620 6665 6174 7572 6573  x nb of features
+00000e60: 292e 0a20 2020 2020 2020 2063 6c69 700a  )..        clip.
+00000e70: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
+00000e80: 6520 7769 7468 206d 696e 2061 6e64 206d  e with min and m
+00000e90: 6178 2063 6c69 7020 7261 6e67 6573 2066  ax clip ranges f
+00000ea0: 6f72 2062 6f74 6820 7468 6520 6e75 6d65  or both the nume
+00000eb0: 7269 6361 6c20 6772 6164 6965 6e74 7320  rical gradients 
+00000ec0: 616e 6420 7468 6520 6772 6164 6965 6e74  and the gradient
+00000ed0: 730a 2020 2020 2020 2020 2020 2020 6f62  s.            ob
+00000ee0: 7461 696e 6564 2066 726f 6d20 7468 6520  tained from the 
+00000ef0: 6074 656e 736f 7266 6c6f 7760 2067 7261  `tensorflow` gra
+00000f00: 7068 2e0a 2020 2020 2020 2020 7570 6461  ph..        upda
+00000f10: 7465 5f6e 756d 5f67 7261 640a 2020 2020  te_num_grad.    
+00000f20: 2020 2020 2020 2020 4966 206e 756d 6572          If numer
+00000f30: 6963 616c 2067 7261 6469 656e 7473 2061  ical gradients a
+00000f40: 7265 2075 7365 642c 2074 6865 7920 7769  re used, they wi
+00000f50: 6c6c 2062 6520 7570 6461 7465 6420 6576  ll be updated ev
+00000f60: 6572 7920 6075 7064 6174 655f 6e75 6d5f  ery `update_num_
+00000f70: 6772 6164 6020 6974 6572 6174 696f 6e73  grad` iterations
+00000f80: 2e0a 2020 2020 2020 2020 7472 7573 7473  ..        trusts
+00000f90: 636f 7265 0a20 2020 2020 2020 2020 2020  core.           
+00000fa0: 2044 6972 6563 746f 7279 2077 6865 7265   Directory where
+00000fb0: 2074 7275 7374 7363 6f72 6520 6f62 6a65   trustscore obje
+00000fc0: 6374 2069 7320 746f 2062 6520 7573 6564  ct is to be used
+00000fd0: 0a20 2020 2020 2020 2073 6573 730a 2020  .        sess.  
+00000fe0: 2020 2020 2020 2020 2020 4f70 7469 6f6e            Option
+00000ff0: 616c 2060 7465 6e73 6f72 666c 6f77 6020  al `tensorflow` 
+00001000: 7365 7373 696f 6e20 7468 6174 2077 696c  session that wil
+00001010: 6c20 6265 2075 7365 6420 6966 2070 6173  l be used if pas
+00001020: 7365 6420 696e 7374 6561 6420 6f66 2063  sed instead of c
+00001030: 7265 6174 696e 6720 6f72 2069 6e66 6572  reating or infer
+00001040: 7269 6e67 206f 6e65 2069 6e74 6572 6e61  ring one interna
+00001050: 6c6c 792e 0a20 2020 2020 2020 2029 01da  lly..        )..
+00001060: 046d 6574 6129 06da 0473 656c 6672 1a00  .meta)...selfr..
+00001070: 0000 721b 0000 0072 2100 0000 7222 0000  ..r....r!...r"..
+00001080: 00da 095f 5f63 6c61 7373 5f5f da06 7061  ...__class__..pa
+00001090: 7261 6d73 4eda 0463 7564 61da 0363 7075  ramsN..cuda..cpu
+000010a0: 5429 01da 0473 697a 6572 1900 0000 467a  T)...sizer....Fz
+000010b0: 5542 6f74 6820 616e 2065 6e63 6f64 6572  UBoth an encoder
+000010c0: 2061 6e64 206b 2d64 2074 7265 6573 2065   and k-d trees e
+000010d0: 6e61 626c 6564 2e20 5573 696e 6720 7468  nabled. Using th
+000010e0: 6520 656e 636f 6465 7220 666f 7220 7468  e encoder for th
+000010f0: 6520 7072 6f74 6f74 7970 6520 6c6f 7373  e prototype loss
+00001100: 2074 6572 6d2e 2901 da0d 656e 635f 6f72   term.)...enc_or
+00001110: 5f6b 6474 7265 6572 0100 0000 6301 0000  _kdtreer....c...
+00001120: 0000 0000 0000 0000 0002 0000 0007 0000  ................
+00001130: 0013 0000 0073 4800 0000 6700 7c00 5d40  .....sH...g.|.]@
+00001140: 7d01 7400 8800 7c01 1900 7401 8302 723c  }.t...|...t...r<
+00001150: 7402 a003 8801 6400 6401 8502 1900 a101  t.....d.d.......
+00001160: 8800 7c01 1900 1400 6401 6401 6401 8502  ..|.....d.d.d...
+00001170: 6602 1900 6e06 8800 7c01 1900 9102 7104  f...n...|.....q.
+00001180: 5300 2902 7219 0000 004e 2904 da0a 6973  S.).r....N)...is
+00001190: 696e 7374 616e 6365 da05 666c 6f61 74da  instance..float.
+000011a0: 0574 6f72 6368 da04 6f6e 6573 2902 da02  .torch..ones)...
+000011b0: 2e30 da01 5fa9 0272 1f00 0000 721c 0000  .0.._..r....r...
+000011c0: 00a9 00fa 502f 6365 6e74 7261 6c2f 686f  ....P/central/ho
+000011d0: 6d65 2f7a 7761 6e67 322f 6d6f 7270 6865  me/zwang2/morphe
+000011e0: 7573 2d73 7061 7469 616c 2f6d 6f72 7068  us-spatial/morph
+000011f0: 6575 732f 7372 632f 6d6f 7270 6865 7573  eus/src/morpheus
+00001200: 2f63 6f75 6e74 6572 6661 6374 7561 6c2f  /counterfactual/
+00001210: 6366 2e70 79da 0a3c 6c69 7374 636f 6d70  cf.py..<listcomp
+00001220: 3ea2 0000 0073 0800 0000 0606 02fd 0cff  >....s..........
+00001230: 2802 7a2b 436f 756e 7465 7266 6163 7475  (.z+Counterfactu
+00001240: 616c 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  al.__init__.<loc
+00001250: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
+00001260: 0600 0000 2934 da05 7375 7065 72da 085f  ....)4..super.._
+00001270: 5f69 6e69 745f 5fda 0463 6f70 79da 0864  _init__..copy..d
+00001280: 6565 7063 6f70 7972 0800 0000 da06 6c6f  eepcopyr......lo
+00001290: 6361 6c73 da03 706f 7072 3100 0000 da06  cals..popr1.....
+000012a0: 7570 6461 7465 721a 0000 0072 2c00 0000  updater....r,...
+000012b0: 722e 0000 0072 3b00 0000 722f 0000 0072  r....r;...r/...r
+000012c0: 3500 0000 da0c 6973 5f61 7661 696c 6162  5.....is_availab
+000012d0: 6c65 da05 7a65 726f 7372 1c00 0000 da07  le..zerosr......
+000012e0: 636c 6173 7365 73da 026e 7072 3900 0000  classes..npr9...
+000012f0: da02 6e6e da06 4d6f 6475 6c65 7222 0000  ..nn..Moduler"..
+00001300: 0072 2100 0000 da08 7761 726e 696e 6773  .r!.....warnings
+00001310: da04 7761 726e 7238 0000 0072 1d00 0000  ..warnr8...r....
+00001320: 721e 0000 0072 2000 0000 7223 0000 00da  r....r ...r#....
+00001330: 0261 65da 0365 6e63 7224 0000 00da 0a62  .ae..encr$.....b
+00001340: 6174 6368 5f73 697a 6572 2600 0000 da06  atch_sizer&.....
+00001350: 7465 6e73 6f72 7227 0000 0072 2800 0000  tensorr'...r(...
+00001360: da05 7475 706c 65da 0572 616e 6765 721f  ..tuple..ranger.
+00001370: 0000 0072 2b00 0000 7229 0000 0072 2a00  ...r+...r)...r*.
+00001380: 0000 721b 0000 0072 2500 0000 722d 0000  ..r....r%...r-..
+00001390: 00da 0973 6861 7065 5f65 6e63 da0e 7369  ...shape_enc..si
+000013a0: 6d70 6c65 5f77 6172 6e69 6e67 da0b 7368  mple_warning..sh
+000013b0: 6f77 7761 726e 696e 6729 1d72 3200 0000  owwarning).r2...
+000013c0: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+000013d0: 1d00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
+000013e0: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
+000013f0: 0000 7224 0000 0072 2500 0000 7226 0000  ..r$...r%...r&..
+00001400: 0072 2700 0000 7228 0000 0072 2900 0000  .r'...r(...r)...
+00001410: 722a 0000 0072 2b00 0000 722c 0000 0072  r*...r+...r,...r
+00001420: 2d00 0000 722e 0000 0072 2f00 0000 7234  -...r....r/...r4
+00001430: 0000 00da 0672 656d 6f76 65da 036b 6579  .....remove..key
+00001440: 5a08 6973 5f6d 6f64 656c 5a05 6973 5f61  Z.is_modelZ.is_a
+00001450: 655a 0669 735f 656e 63a9 0172 3300 0000  eZ.is_enc..r3...
+00001460: 723f 0000 0072 4100 0000 7244 0000 0011  r?...rA...rD....
+00001470: 0000 0073 7a00 0000 004d 1402 0601 0808  ...sz....M......
+00001480: 0801 0c01 1001 0601 0601 0603 06ff 0602  ................
+00001490: 16fd 0407 0401 0401 1c02 0601 1a02 0e01  ................
+000014a0: 0e02 0401 0802 0602 0401 0802 0602 0e01  ................
+000014b0: 0401 02ff 0404 0e01 0802 0601 1402 0601  ................
+000014c0: 0601 0601 0601 0601 0601 0601 0601 0a01  ................
+000014d0: 0601 0c01 0601 0201 0c06 06fa 04ff 060a  ................
+000014e0: 0601 0601 0601 0601 0601 0603 0801 1a03  ................
+000014f0: 0803 7a17 436f 756e 7465 7266 6163 7475  ..z.Counterfactu
+00001500: 616c 2e5f 5f69 6e69 745f 5f63 0200 0000  al.__init__c....
+00001510: 0000 0000 0000 0000 0700 0000 0500 0000  ................
+00001520: 4300 0000 739a 0000 007c 006a 007c 006a  C...s....|.j.|.j
+00001530: 0118 007c 006a 026b 047d 0274 03a0 047c  ...|.j.k.}.t...|
+00001540: 006a 007c 006a 0118 00a1 017c 006a 026b  .j.|.j.....|.j.k
+00001550: 017d 037c 006a 007c 006a 0118 007c 006a  .}.|.j.|.j...|.j
+00001560: 020b 006b 007d 0474 03a0 057c 006a 007c  ...k.}.t...|.j.|
+00001570: 006a 0218 007c 0164 0119 00a1 027d 0574  .j...|.d.....}.t
+00001580: 03a0 067c 006a 007c 006a 0217 007c 0164  ...|.j.|.j...|.d
+00001590: 0219 00a1 027d 067c 02a0 07a1 007c 0514  .....}.|.....|..
+000015a0: 007c 03a0 07a1 007c 006a 0114 0017 007c  .|.....|.j.....|
+000015b0: 04a0 07a1 007c 0614 0017 007c 005f 0864  .....|.....|._.d
+000015c0: 0053 0029 034e 7219 0000 0072 0100 0000  .S.).Nr....r....
+000015d0: 2909 da05 6164 765f 73da 046f 7269 6772  )...adv_s..origr
+000015e0: 1e00 0000 723b 0000 00da 0361 6273 da03  ....r;.....abs..
+000015f0: 6d69 6eda 036d 6178 723a 0000 00da 0a61  min..maxr:.....a
+00001600: 7373 6967 6e5f 6164 7629 0772 3200 0000  ssign_adv).r2...
+00001610: 721f 0000 005a 0663 6f6e 645f 305a 0663  r....Z.cond_0Z.c
+00001620: 6f6e 645f 315a 0663 6f6e 645f 32da 0575  ond_1Z.cond_2..u
+00001630: 7070 6572 da05 6c6f 7765 7272 4000 0000  pper..lowerr@...
+00001640: 7240 0000 0072 4100 0000 da1e 636f 6d70  r@...rA.....comp
+00001650: 7574 655f 7368 7269 6e6b 6167 655f 7468  ute_shrinkage_th
+00001660: 7265 7368 6f6c 6469 6e67 bc00 0000 730e  resholding....s.
+00001670: 0000 0000 0212 0118 0114 0318 0118 0424  ...............$
+00001680: ff7a 2d43 6f75 6e74 6572 6661 6374 7561  .z-Counterfactua
+00001690: 6c2e 636f 6d70 7574 655f 7368 7269 6e6b  l.compute_shrink
+000016a0: 6167 655f 7468 7265 7368 6f6c 6469 6e67  age_thresholding
+000016b0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000016c0: 0006 0000 0043 0000 0073 4e00 0000 7c00  .....C...sN...|.
+000016d0: 6a00 7c00 6a00 6401 1700 1b00 7c00 5f01  j.|.j.d.....|._.
+000016e0: 7c00 6a02 7c00 6a01 7c00 6a02 7c00 6a03  |.j.|.j.|.j.|.j.
+000016f0: 1800 1400 1700 7c00 5f04 7405 a006 7c00  ......|._.t...|.
+00001700: 6a04 7c00 6a07 6402 1900 7c00 6a07 6403  j.|.j.d...|.j.d.
+00001710: 1900 a103 7c00 5f04 6400 5300 2904 4e67  ....|._.d.S.).Ng
+00001720: 0000 0000 0000 0840 7201 0000 0072 1900  .......@r....r..
+00001730: 0000 2908 da0b 676c 6f62 616c 5f73 7465  ..)...global_ste
+00001740: 70da 027a 7472 6300 0000 da03 6164 76da  p..ztrc.....adv.
+00001750: 0c61 7373 6967 6e5f 6164 765f 7372 3b00  .assign_adv_sr;.
+00001760: 0000 da05 636c 616d 7072 1f00 0000 a901  ....clampr......
+00001770: 7232 0000 0072 4000 0000 7240 0000 0072  r2...r@...r@...r
+00001780: 4100 0000 da1f 636f 6d70 7574 655f 7065  A.....compute_pe
+00001790: 7274 7572 6261 7469 6f6e 5f70 726f 6a65  rturbation_proje
+000017a0: 6374 696f 6ecb 0000 0073 0a00 0000 0002  ction....s......
+000017b0: 1201 1a03 0401 14ff 7a2e 436f 756e 7465  ........z.Counte
+000017c0: 7266 6163 7475 616c 2e63 6f6d 7075 7465  rfactual.compute
+000017d0: 5f70 6572 7475 7262 6174 696f 6e5f 7072  _perturbation_pr
+000017e0: 6f6a 6563 7469 6f6e 6301 0000 0000 0000  ojectionc.......
+000017f0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00001800: 0073 2000 0000 7c00 6a00 a001 a100 7c00  .s ...|.j.....|.
+00001810: 5f02 7c00 6a03 6a04 a001 a100 7c00 6a05  _.|.j.j.....|.j.
+00001820: 5f04 6400 5300 a901 4e29 0672 6300 0000  _.d.S...N).rc...
+00001830: da05 636c 6f6e 6572 6900 0000 726a 0000  ..cloneri...rj..
+00001840: 00da 0464 6174 6172 5e00 0000 726c 0000  ...datar^...rl..
+00001850: 0072 4000 0000 7240 0000 0072 4100 0000  .r@...r@...rA...
+00001860: da16 7570 6461 7465 5f63 6f75 6e74 6572  ..update_counter
+00001870: 6661 6374 7561 6c73 d500 0000 7304 0000  factuals....s...
+00001880: 0000 020c 017a 2543 6f75 6e74 6572 6661  .....z%Counterfa
+00001890: 6374 7561 6c2e 7570 6461 7465 5f63 6f75  ctual.update_cou
+000018a0: 6e74 6572 6661 6374 7561 6c73 6301 0000  nterfactualsc...
+000018b0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+000018c0: 0043 0000 0073 2000 0000 7c00 6a00 7c00  .C...s ...|.j.|.
+000018d0: 6a01 1800 7c00 5f02 7c00 6a00 7c00 6a03  j...|._.|.j.|.j.
+000018e0: 1800 7c00 5f04 6400 5300 726e 0000 0029  ..|._.d.S.rn...)
+000018f0: 0572 5f00 0000 7269 0000 00da 0564 656c  .r_...ri.....del
+00001900: 7461 725e 0000 00da 0764 656c 7461 5f73  tar^.....delta_s
+00001910: 726c 0000 0072 4000 0000 7240 0000 0072  rl...r@...r@...r
+00001920: 4100 0000 da12 636f 6d70 7574 655f 6465  A.....compute_de
+00001930: 7669 6174 696f 6e73 da00 0000 7304 0000  viations....s...
+00001940: 0000 020e 017a 2143 6f75 6e74 6572 6661  .....z!Counterfa
+00001950: 6374 7561 6c2e 636f 6d70 7574 655f 6465  ctual.compute_de
+00001960: 7669 6174 696f 6e73 6302 0000 0000 0000  viationsc.......
+00001970: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
+00001980: 0073 da00 0000 7c00 a000 a100 0100 7401  .s....|.......t.
+00001990: 7402 6401 7403 7c01 8301 8302 8301 7d02  t.d.t.|.......}.
+000019a0: 7404 6a05 7c00 6a06 6402 1300 7c02 6403  t.j.|.j.d...|.d.
+000019b0: 8d02 7c00 5f07 7404 6a05 7c00 6a08 6402  ..|._.t.j.|.j.d.
+000019c0: 1300 7c02 6403 8d02 7c00 5f09 7404 6a05  ..|.d...|._.t.j.
+000019d0: 7404 a00a 7c00 6a06 a101 7c02 6403 8d02  t...|.j...|.d...
+000019e0: 7c00 5f0b 7404 6a05 7404 a00a 7c00 6a08  |._.t.j.t...|.j.
+000019f0: a101 7c02 6403 8d02 7c00 5f0c 7c00 6a07  ..|.d...|._.|.j.
+00001a00: 7c00 6a0b 7c00 6a0d 1400 1700 7c00 5f0e  |.j.|.j.....|._.
+00001a10: 7c00 6a09 7c00 6a0c 7c00 6a0d 1400 1700  |.j.|.j.|.j.....
+00001a20: 7c00 5f0f 7404 a005 7c00 6a0b a101 7c00  |._.t...|.j...|.
+00001a30: 5f10 7404 a005 7c00 6a0c a101 7c00 5f11  _.t...|.j...|._.
+00001a40: 7404 a005 7c00 6a07 a101 7c00 5f12 7404  t...|.j...|._.t.
+00001a50: a005 7c00 6a09 a101 7c00 5f13 6400 5300  ..|.j...|._.d.S.
+00001a60: 2904 4e72 1900 0000 7206 0000 00a9 01da  ).Nr....r.......
+00001a70: 0364 696d 2914 7274 0000 0072 5600 0000  .dim).rt...rV...
+00001a80: 7257 0000 00da 036c 656e 723b 0000 00da  rW.....lenr;....
+00001a90: 0373 756d 7272 0000 00da 026c 3272 7300  .sumrr.....l2rs.
+00001aa0: 0000 5a04 6c32 5f73 7260 0000 00da 026c  ..Z.l2_sr`.....l
+00001ab0: 315a 046c 315f 7372 1e00 0000 da05 6c31  1Z.l1_sr......l1
+00001ac0: 5f6c 325a 076c 315f 6c32 5f73 da07 6c6f  _l2Z.l1_l2_s..lo
+00001ad0: 7373 5f6c 315a 096c 6f73 735f 6c31 5f73  ss_l1Z.loss_l1_s
+00001ae0: da07 6c6f 7373 5f6c 32da 096c 6f73 735f  ..loss_l2..loss_
+00001af0: 6c32 5f73 2903 7232 0000 0072 1c00 0000  l2_s).r2...r....
+00001b00: 5a06 6178 5f73 756d 7240 0000 0072 4000  Z.ax_sumr@...r@.
+00001b10: 0000 7241 0000 00da 1463 6f6d 7075 7465  ..rA.....compute
+00001b20: 5f6c 315f 6c32 5f6c 6f73 7365 73df 0000  _l1_l2_losses...
+00001b30: 0073 1800 0000 0002 0802 1202 1601 1602  .s..............
+00001b40: 1801 1802 1401 1403 0e01 0e01 0e01 7a23  ..............z#
+00001b50: 436f 756e 7465 7266 6163 7475 616c 2e63  Counterfactual.c
+00001b60: 6f6d 7075 7465 5f6c 315f 6c32 5f6c 6f73  ompute_l1_l2_los
+00001b70: 7365 7363 0100 0000 0000 0000 0000 0000  sesc............
+00001b80: 0100 0000 0500 0000 4300 0000 737c 0000  ........C...s|..
+00001b90: 007c 006a 0072 607c 00a0 017c 006a 02a1  .|.j.r`|...|.j..
+00001ba0: 017c 005f 037c 00a0 017c 006a 04a1 017c  .|._.|...|.j...|
+00001bb0: 005f 057c 006a 0674 07a0 087c 006a 037c  ._.|.j.t...|.j.|
+00001bc0: 006a 0218 00a1 0164 0113 0014 007c 005f  .j.....d.....|._
+00001bd0: 097c 006a 0674 07a0 087c 006a 057c 006a  .|.j.t...|.j.|.j
+00001be0: 0418 00a1 0164 0113 0014 007c 005f 0a6e  .....d.....|._.n
+00001bf0: 1874 07a0 0b64 02a1 017c 005f 0974 07a0  .t...d...|._.t..
+00001c00: 0b64 02a1 017c 005f 0a64 0053 0029 034e  .d...|._.d.S.).N
+00001c10: 7206 0000 0072 0e00 0000 290c 7221 0000  r....r....).r!..
+00001c20: 0072 5200 0000 7269 0000 005a 0661 6476  .rR...ri...Z.adv
+00001c30: 5f61 6572 5e00 0000 5a08 6164 765f 6165  _aer^...Z.adv_ae
+00001c40: 5f73 7220 0000 0072 3b00 0000 da04 6e6f  _sr ...r;.....no
+00001c50: 726d da07 6c6f 7373 5f61 65da 096c 6f73  rm..loss_ae..los
+00001c60: 735f 6165 5f73 7255 0000 0072 6c00 0000  s_ae_srU...rl...
+00001c70: 7240 0000 0072 4000 0000 7241 0000 00da  r@...r@...rA....
+00001c80: 1863 6f6d 7075 7465 5f61 7574 6f65 6e63  .compute_autoenc
+00001c90: 6f64 6572 5f6c 6f73 73f4 0000 0073 0e00  oder_loss....s..
+00001ca0: 0000 0002 0602 0e01 0e02 1e01 2002 0c01  ............ ...
+00001cb0: 7a27 436f 756e 7465 7266 6163 7475 616c  z'Counterfactual
+00001cc0: 2e63 6f6d 7075 7465 5f61 7574 6f65 6e63  .compute_autoenc
+00001cd0: 6f64 6572 5f6c 6f73 7363 0100 0000 0000  oder_lossc......
+00001ce0: 0000 0000 0000 0500 0000 0800 0000 4300  ..............C.
+00001cf0: 0000 7376 0100 007c 00a0 007c 006a 01a1  ..sv...|...|.j..
+00001d00: 017c 005f 027c 00a0 007c 006a 03a1 017c  .|._.|...|.j...|
+00001d10: 005f 047c 006a 0572 6074 06a0 07a1 008f  ._.|.j.r`t......
+00001d20: 2201 007c 00a0 087c 006a 027c 006a 09a1  "..|...|.j.|.j..
+00001d30: 027c 005f 0a57 0064 0004 0004 0083 0301  .|._.W.d........
+00001d40: 006e 1031 0073 5230 0001 0001 0001 0059  .n.1.sR0.......Y
+00001d50: 0001 0090 016e 127c 006a 0b64 016b 0272  .....n.|.j.d.k.r
+00001d60: 8e7c 006a 0c64 026b 0272 8e74 06a0 0d64  .|.j.d.k.r.t...d
+00001d70: 01a1 017c 005f 0a74 06a0 0d64 01a1 017c  ...|._.t...d...|
+00001d80: 005f 0e6e e474 066a 0f7c 006a 097c 006a  ._.n.t.j.|.j.|.j
+00001d90: 0214 0064 0264 038d 027c 005f 1074 066a  ...d.d...|._.t.j
+00001da0: 0f7c 006a 097c 006a 0414 0064 0264 038d  .|.j.|.j...d.d..
+00001db0: 027d 0174 066a 1164 027c 006a 0918 007c  .}.t.j.d.|.j...|
+00001dc0: 006a 0214 007c 006a 0964 0414 0018 0064  .j...|.j.d.....d
+00001dd0: 0264 038d 0264 0519 007c 005f 1274 066a  .d...d...|._.t.j
+00001de0: 1164 027c 006a 0918 007c 006a 0414 007c  .d.|.j...|.j...|
+00001df0: 006a 0964 0414 0018 0064 0264 038d 0264  .j.d.....d.d...d
+00001e00: 0519 007d 0274 06a0 1374 06a0 0d64 01a1  ...}.t...t...d..
+00001e10: 017c 006a 120b 007c 006a 1017 007c 006a  .|.j...|.j...|.j
+00001e20: 1417 00a1 027d 0374 06a0 1374 06a0 0d64  .....}.t...t...d
+00001e30: 01a1 017c 020b 007c 0117 007c 006a 1417  ...|...|...|.j..
+00001e40: 00a1 027d 0474 06a0 0f7c 006a 157c 0314  ...}.t...|.j.|..
+00001e50: 00a1 017c 005f 0a74 06a0 0f7c 006a 157c  ...|._.t...|.j.|
+00001e60: 0414 00a1 017c 005f 0e64 0053 0029 064e  .....|._.d.S.).N
+00001e70: 720e 0000 0072 1900 0000 7275 0000 00e9  r....r....ru....
+00001e80: 1027 0000 7201 0000 0029 1672 1a00 0000  .'..r....).r....
+00001e90: 7269 0000 00da 0a70 7265 645f 7072 6f62  ri.....pred_prob
+00001ea0: 6172 5e00 0000 5a0c 7072 6564 5f70 726f  ar^...Z.pred_pro
+00001eb0: 6261 5f73 722e 0000 0072 3b00 0000 da07  ba_sr....r;.....
+00001ec0: 6e6f 5f67 7261 64da 076c 6f73 735f 666e  no_grad..loss_fn
+00001ed0: da06 7461 7267 6574 da0b 6c6f 7373 5f61  ..target..loss_a
+00001ee0: 7474 6163 6b72 2700 0000 7228 0000 0072  ttackr'...r(...r
+00001ef0: 5500 0000 da0d 6c6f 7373 5f61 7474 6163  U.....loss_attac
+00001f00: 6b5f 7372 7800 0000 da0c 7461 7267 6574  k_srx.....target
+00001f10: 5f70 726f 6261 7262 0000 00da 136e 6f6e  _probarb.....non
+00001f20: 7461 7267 6574 5f70 726f 6261 5f6d 6178  target_proba_max
+00001f30: da07 6d61 7869 6d75 6d72 1d00 0000 da05  ..maximumr......
+00001f40: 636f 6e73 7429 0572 3200 0000 5a0e 7461  const).r2...Z.ta
+00001f50: 7267 6574 5f70 726f 6261 5f73 5a15 6e6f  rget_proba_sZ.no
+00001f60: 6e74 6172 6765 745f 7072 6f62 615f 6d61  ntarget_proba_ma
+00001f70: 785f 7372 8900 0000 728a 0000 0072 4000  x_sr....r....r@.
+00001f80: 0000 7240 0000 0072 4100 0000 da13 636f  ..r@...rA.....co
+00001f90: 6d70 7574 655f 6174 7461 636b 5f6c 6f73  mpute_attack_los
+00001fa0: 7301 0100 0073 3a00 0000 0001 0e01 0e02  s....s:.........
+00001fb0: 0601 0a01 3401 1401 0c01 0e03 1801 1603  ....4...........
+00001fc0: 0401 1aff 0402 02fe 0603 0401 1aff 0402  ................
+00001fd0: 02fe 0405 0401 0801 12fe 0404 0401 16ff  ................
+00001fe0: 0405 1201 7a22 436f 756e 7465 7266 6163  ....z"Counterfac
+00001ff0: 7475 616c 2e63 6f6d 7075 7465 5f61 7474  tual.compute_att
+00002000: 6163 6b5f 6c6f 7373 6301 0000 0000 0000  ack_lossc.......
+00002010: 0000 0000 0001 0000 0006 0000 0043 0000  .............C..
+00002020: 0073 b000 0000 7c00 6a00 7250 7c00 6a01  .s....|.j.rP|.j.
+00002030: 7402 a003 7c00 a004 7c00 6a05 a101 7c00  t...|...|.j...|.
+00002040: 6a06 1800 a101 6401 1300 1400 7c00 5f07  j.....d.....|._.
+00002050: 7c00 6a01 7402 a003 7c00 a004 7c00 6a08  |.j.t...|...|.j.
+00002060: a101 7c00 6a06 1800 a101 6401 1300 1400  ..|.j.....d.....
+00002070: 7c00 5f09 6e5c 7c00 6a0a 7294 7c00 6a01  |._.n\|.j.r.|.j.
+00002080: 7402 a003 7c00 6a05 7c00 6a06 1800 a101  t...|.j.|.j.....
+00002090: 6401 1300 1400 7c00 5f07 7c00 6a01 7402  d.....|._.|.j.t.
+000020a0: a003 7c00 6a08 7c00 6a06 1800 a101 6401  ..|.j.|.j.....d.
+000020b0: 1300 1400 7c00 5f09 6e18 7402 a00b 6402  ....|._.n.t...d.
+000020c0: a101 7c00 5f07 7402 a00b 6402 a101 7c00  ..|._.t...d...|.
+000020d0: 5f09 6403 5300 2904 7a1b 436f 6d70 7574  _.d.S.).z.Comput
+000020e0: 6520 7468 6520 7072 6f74 6f74 7970 6520  e the prototype 
+000020f0: 6c6f 7373 2e72 0600 0000 720e 0000 004e  loss.r....r....N
+00002100: 290c 7222 0000 0072 2300 0000 723b 0000  ).r"...r#...r;..
+00002110: 0072 8000 0000 7253 0000 0072 6900 0000  .r....rS...ri...
+00002120: da0c 7461 7267 6574 5f70 726f 746f da0a  ..target_proto..
+00002130: 6c6f 7373 5f70 726f 746f 725e 0000 00da  loss_protor^....
+00002140: 0c6c 6f73 735f 7072 6f74 6f5f 7372 2400  .loss_proto_sr$.
+00002150: 0000 7255 0000 0072 6c00 0000 7240 0000  ..rU...rl...r@..
+00002160: 0072 4000 0000 7241 0000 00da 1663 6f6d  .r@...rA.....com
+00002170: 7075 7465 5f70 726f 746f 7479 7065 5f6c  pute_prototype_l
+00002180: 6f73 7325 0100 0073 1600 0000 0002 0602  oss%...s........
+00002190: 20ff 0404 20ff 0603 0601 1e02 1aff 0604   ... ...........
+000021a0: 0c01 7a25 436f 756e 7465 7266 6163 7475  ..z%Counterfactu
+000021b0: 616c 2e63 6f6d 7075 7465 5f70 726f 746f  al.compute_proto
+000021c0: 7479 7065 5f6c 6f73 7363 0100 0000 0000  type_lossc......
+000021d0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+000021e0: 0000 735a 0000 007c 00a0 007c 006a 01a1  ..sZ...|...|.j..
+000021f0: 0101 007c 00a0 02a1 0001 007c 00a0 03a1  ...|.......|....
+00002200: 0001 007c 006a 047c 006a 0517 007c 006a  ...|.j.|.j...|.j
+00002210: 0617 007c 005f 077c 006a 087c 006a 0917  ...|._.|.j.|.j..
+00002220: 007c 006a 0a17 007c 006a 0b7c 006a 0c14  .|.j...|.j.|.j..
+00002230: 0017 007c 006a 0d17 007c 005f 0e64 0053  ...|.j...|._.d.S
+00002240: 0072 6e00 0000 290f 727f 0000 0072 1c00  .rn...).r....r..
+00002250: 0000 7283 0000 0072 9300 0000 727e 0000  ..r....r....r~..
+00002260: 0072 8200 0000 7292 0000 00da 086c 6f73  .r....r......los
+00002270: 735f 7265 6772 8900 0000 727d 0000 0072  s_regr....r}...r
+00002280: 8100 0000 721e 0000 0072 7c00 0000 7291  ....r....r|...r.
+00002290: 0000 00da 0a6c 6f73 735f 746f 7461 6c72  .....loss_totalr
+000022a0: 6c00 0000 7240 0000 0072 4000 0000 7241  l...r@...r@...rA
+000022b0: 0000 00da 1863 6f6d 7075 7465 5f72 6567  .....compute_reg
+000022c0: 756c 6172 697a 6572 5f6c 6f73 7337 0100  ularizer_loss7..
+000022d0: 0073 1c00 0000 0003 0c01 0801 0803 1404  .s..............
+000022e0: 0401 04ff 0202 04fe 0203 0afd 0204 04fc  ................
+000022f0: 02ff 7a27 436f 756e 7465 7266 6163 7475  ..z'Counterfactu
+00002300: 616c 2e63 6f6d 7075 7465 5f72 6567 756c  al.compute_regul
+00002310: 6172 697a 6572 5f6c 6f73 7329 0372 8500  arizer_loss).r..
+00002320: 0000 da01 5972 3000 0000 6303 0000 0000  ....Yr0...c.....
+00002330: 0000 0000 0000 0007 0000 0005 0000 0043  ...............C
+00002340: 0000 0073 5c00 0000 7400 a001 7c01 7c02  ...s\...t...|.|.
+00002350: 1400 a101 7d03 7400 a002 6401 7c02 1800  ....}.t...d.|...
+00002360: 7c01 1400 6402 7c02 1400 1800 a101 7d04  |...d.|.......}.
+00002370: 7400 a003 7400 a004 6403 6701 a101 7c04  t...t...d.g...|.
+00002380: 0b00 7c03 1700 7c00 6a05 1700 a102 7d05  ..|...|.j.....}.
+00002390: 7400 a001 7c00 6a06 7c05 1400 a101 7d06  t...|.j.|.....}.
+000023a0: 7c06 5300 2904 6117 0100 000a 2020 2020  |.S.).a.....    
+000023b0: 2020 2020 436f 6d70 7574 6520 7468 6520      Compute the 
+000023c0: 6174 7461 636b 206c 6f73 732e 0a0a 2020  attack loss...  
+000023d0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+000023e0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000023f0: 2d2d 2d0a 2020 2020 2020 2020 7072 6564  ---.        pred
+00002400: 5f70 726f 6261 0a20 2020 2020 2020 2020  _proba.         
+00002410: 2020 2050 7265 6469 6374 696f 6e20 7072     Prediction pr
+00002420: 6f62 6162 696c 6974 6965 7320 6f66 2061  obabilities of a
+00002430: 6e20 696e 7374 616e 6365 2e0a 2020 2020  n instance..    
+00002440: 2020 2020 590a 2020 2020 2020 2020 2020      Y.          
+00002450: 2020 4f6e 652d 686f 7420 7265 7072 6573    One-hot repres
+00002460: 656e 7461 7469 6f6e 206f 6620 696e 7374  entation of inst
+00002470: 616e 6365 206c 6162 656c 732e 0a0a 2020  ance labels...  
+00002480: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+00002490: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+000024a0: 2020 2020 2020 4c6f 7373 206f 6620 7468        Loss of th
+000024b0: 6520 6174 7461 636b 2e0a 2020 2020 2020  e attack..      
+000024c0: 2020 7219 0000 0072 8400 0000 720e 0000    r....r....r...
+000024d0: 0029 0772 3b00 0000 7278 0000 0072 6200  .).r;...rx...rb.
+000024e0: 0000 728d 0000 0072 5500 0000 721d 0000  ..r....rU...r...
+000024f0: 0072 8e00 0000 2907 7232 0000 0072 8500  .r....).r2...r..
+00002500: 0000 7297 0000 0072 8b00 0000 728c 0000  ..r....r....r...
+00002510: 00da 046c 6f73 7372 8900 0000 7240 0000  ...lossr....r@..
+00002520: 0072 4000 0000 7241 0000 0072 8700 0000  .r@...rA...r....
+00002530: 4a01 0000 730e 0000 0000 100e 021a 0204  J...s...........
+00002540: 0118 ff04 0410 017a 1643 6f75 6e74 6572  .......z.Counter
+00002550: 6661 6374 7561 6c2e 6c6f 7373 5f66 6e63  factual.loss_fnc
+00002560: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00002570: 0400 0000 0300 0000 7338 0000 0074 006a  ........s8...t.j
+00002580: 0188 006a 0267 017c 0164 018d 0288 005f  ...j.g.|.d....._
+00002590: 0387 0066 0164 0264 0384 087d 0274 006a  ...f.d.d...}.t.j
+000025a0: 046a 0588 006a 037c 0264 048d 0288 005f  .j...j.|.d....._
+000025b0: 0664 0553 0029 067a 1f53 6574 2075 7020  .d.S.).z.Set up 
+000025c0: 7468 6520 7472 6169 6e69 6e67 2070 6172  the training par
+000025d0: 616d 6574 6572 732e 2901 da02 6c72 6301  ameters.)...lrc.
+000025e0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+000025f0: 0000 0013 0000 0073 1200 0000 6401 7c00  .......s....d.|.
+00002600: 8800 6a00 1b00 1800 6402 1300 5300 2903  ..j.....d...S.).
+00002610: 4e72 1900 0000 6700 0000 0000 00e0 3f29  Nr....g.......?)
+00002620: 0172 2600 0000 2901 da05 6570 6f63 6872  .r&...)...epochr
+00002630: 6c00 0000 7240 0000 0072 4100 0000 da08  l...r@...rA.....
+00002640: 3c6c 616d 6264 613e 6801 0000 f300 0000  <lambda>h.......
+00002650: 007a 2f43 6f75 6e74 6572 6661 6374 7561  .z/Counterfactua
+00002660: 6c2e 7365 7475 705f 7472 6169 6e69 6e67  l.setup_training
+00002670: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00002680: 613e 2902 da09 6f70 7469 6d69 7a65 72da  a>)...optimizer.
+00002690: 096c 725f 6c61 6d62 6461 4e29 07da 056f  .lr_lambdaN)...o
+000026a0: 7074 696d da03 5347 4472 5e00 0000 729d  ptim..SGDr^...r.
+000026b0: 0000 00da 0c6c 725f 7363 6865 6475 6c65  .....lr_schedule
+000026c0: 72da 084c 616d 6264 614c 52da 0d6c 6561  r..LambdaLR..lea
+000026d0: 726e 696e 675f 7261 7465 2903 7232 0000  rning_rate).r2..
+000026e0: 0072 2500 0000 5a11 6c61 6d62 6461 5f70  .r%...Z.lambda_p
+000026f0: 6f6c 795f 6465 6361 7972 4000 0000 726c  oly_decayr@...rl
+00002700: 0000 0072 4100 0000 da0e 7365 7475 705f  ...rA.....setup_
+00002710: 7472 6169 6e69 6e67 6501 0000 730a 0000  traininge...s...
+00002720: 0000 0214 010c 0106 0106 ff7a 1d43 6f75  ...........z.Cou
+00002730: 6e74 6572 6661 6374 7561 6c2e 7365 7475  nterfactual.setu
+00002740: 705f 7472 6169 6e69 6e67 2903 da0a 7472  p_training)...tr
+00002750: 6169 6e5f 6461 7461 da05 7072 6564 7372  ain_data..predsr
+00002760: 3000 0000 6303 0000 0000 0000 0000 0000  0...c...........
+00002770: 000a 0000 0006 0000 0043 0000 0073 c800  .........C...s..
+00002780: 0000 7400 8300 7d03 6401 6402 6702 7d04  ..t...}.d.d.g.}.
+00002790: 7c04 4400 5d0e 7d05 7c03 a001 7c05 a101  |.D.].}.|...|...
+000027a0: 0100 7112 7c00 6a02 6403 1900 a003 7c03  ..q.|.j.d.....|.
+000027b0: a101 0100 7c00 6a04 72a4 7c00 6a05 a006  ....|.j.r.|.j...
+000027c0: 7c01 a101 7d06 6900 7c00 5f07 6900 7c00  |...}.i.|._.i.|.
+000027d0: 5f08 7409 7c00 6a0a 8301 4400 5d46 7d07  _.t.|.j...D.]F}.
+000027e0: 740b a00c 7c02 7c07 6b02 a101 6404 1900  t...|.|.k...d...
+000027f0: 7d08 740b 6a0d 740b 6a0e 7c06 7c08 1900  }.t.j.t.j.|.|...
+00002800: 6404 6405 8d02 6404 6405 8d02 7c00 6a07  d.d...d.d...|.j.
+00002810: 7c07 3c00 7c06 7c08 1900 7c00 6a08 7c07  |.<.|.|...|.j.|.
+00002820: 3c00 715a 6e20 7c00 6a0f 72c4 7410 7c00  <.qZn |.j.r.t.|.
+00002830: 6a11 8301 7d09 7c09 6a12 7c00 5f12 7c09  j...}.|.j.|._.|.
+00002840: 6a13 7c00 5f14 7c00 5300 2906 6128 0100  j.|._.|.S.).a(..
+00002850: 000a 2020 2020 2020 2020 4765 7420 7072  ..        Get pr
+00002860: 6f74 6f74 7970 6573 2066 6f72 2065 6163  ototypes for eac
+00002870: 6820 636c 6173 7320 7573 696e 6720 7468  h class using th
+00002880: 6520 656e 636f 6465 7220 6f72 206b 2d64  e encoder or k-d
+00002890: 2074 7265 6573 2e0a 2020 2020 2020 2020   trees..        
+000028a0: 5468 6520 7072 6f74 6f74 7970 6573 2061  The prototypes a
+000028b0: 7265 2075 7365 6420 666f 7220 7468 6520  re used for the 
+000028c0: 656e 636f 6465 7220 6c6f 7373 2074 6572  encoder loss ter
+000028d0: 6d20 6f72 2074 6f20 6361 6c63 756c 6174  m or to calculat
+000028e0: 6520 7468 6520 6f70 7469 6f6e 616c 2074  e the optional t
+000028f0: 7275 7374 2073 636f 7265 732e 0a0a 2020  rust scores...  
+00002900: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00002910: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00002920: 2d2d 2d0a 2020 2020 2020 2020 7472 6169  ---.        trai
+00002930: 6e5f 6461 7461 0a20 2020 2020 2020 2020  n_data.         
+00002940: 2020 2052 6570 7265 7365 6e74 6174 6976     Representativ
+00002950: 6520 7361 6d70 6c65 2066 726f 6d20 7468  e sample from th
+00002960: 6520 7472 6169 6e69 6e67 2064 6174 612e  e training data.
+00002970: 0a20 2020 2020 2020 2072 3200 0000 72a5  .        r2...r.
+00002980: 0000 0072 3400 0000 7201 0000 00a9 01da  ...r4...r.......
+00002990: 0461 7869 7329 1572 4700 0000 7248 0000  .axis).rG...rH..
+000029a0: 0072 3100 0000 7249 0000 0072 2200 0000  .r1...rI...r"...
+000029b0: 7253 0000 0072 1a00 0000 da0b 636c 6173  rS...r......clas
+000029c0: 735f 7072 6f74 6fda 0963 6c61 7373 5f65  s_proto..class_e
+000029d0: 6e63 7257 0000 0072 4c00 0000 724d 0000  ncrW...rL...rM..
+000029e0: 00da 0577 6865 7265 da0b 6578 7061 6e64  ...where..expand
+000029f0: 5f64 696d 73da 046d 6561 6e72 2400 0000  _dims..meanr$...
+00002a00: da0b 6c6f 6164 5f6f 626a 6563 7472 2c00  ..load_objectr,.
+00002a10: 0000 da07 6b64 7472 6565 735a 0858 5f6b  ....kdtreesZ.X_k
+00002a20: 6474 7265 65da 0a58 5f62 795f 636c 6173  dtree..X_by_clas
+00002a30: 7329 0a72 3200 0000 72a5 0000 0072 a600  s).r2...r....r..
+00002a40: 0000 7234 0000 0072 5b00 0000 725c 0000  ..r4...r[...r\..
+00002a50: 005a 0865 6e63 5f64 6174 61da 0169 da03  .Z.enc_data..i..
+00002a60: 6964 78da 0274 7372 4000 0000 7240 0000  idx..tsr@...r@..
+00002a70: 0072 4100 0000 da03 6669 746d 0100 0073  .rA.....fitm...s
+00002a80: 2800 0000 000f 0601 0801 0801 0c02 1002  (...............
+00002a90: 0601 0c01 0601 0601 0e01 1201 0401 12ff  ................
+00002aa0: 0c03 1201 0604 0a01 0801 0801 7a12 436f  ............z.Co
+00002ab0: 756e 7465 7266 6163 7475 616c 2e66 6974  unterfactual.fit
+00002ac0: 2904 da01 5872 9700 0000 da0b 6772 6164  )...Xr......grad
+00002ad0: 735f 7368 6170 6572 3000 0000 6304 0000  s_shaper0...c...
+00002ae0: 0000 0000 0000 0000 0015 0000 0006 0000  ................
+00002af0: 0003 0000 0073 ea01 0000 7c01 a000 a100  .....s....|.....
+00002b00: a001 a100 7d04 7c00 a002 7c04 a101 a001  ....}.|...|.....
+00002b10: a100 a003 a100 7d05 7404 7c05 7c00 6a05  ......}.t.|.|.j.
+00002b20: 6401 1900 6402 6403 8d03 5c02 7d06 7d07  d...d.d...\.}.}.
+00002b30: 8700 6601 6404 6405 8408 7d08 8700 6601  ..f.d.d...}...f.
+00002b40: 6406 6407 8408 7d09 7406 a007 7c08 7c05  d.d...}.t...|.|.
+00002b50: 8301 7c09 7c05 8301 1800 7c00 6a08 0b00  ..|.|.....|.j...
+00002b60: 6b01 a101 6401 1900 7d0a 7409 7c0a 8301  k...d...}.t.|...
+00002b70: 7c01 6a0a 6401 1900 6b02 729e 7406 a00b  |.j.d...k.r.t...
+00002b80: 6408 6701 7c01 6a0a 6408 6409 8502 1900  d.g.|.j.d.d.....
+00002b90: a201 5200 a101 5300 7c08 7c06 8301 7c08  ..R...S.|.|...|.
+00002ba0: 7c07 8301 1800 7d0b 7c09 7c06 8301 7c09  |.....}.|.|...|.
+00002bb0: 7c07 8301 1800 7d0c 7c0b 7c0c 1800 7d0d  |.....}.|.|...}.
+00002bc0: 7406 a00c 7c0d 7c01 6a0a 6401 1900 640a  t...|.|.j.d...d.
+00002bd0: 6602 a102 640b 7c00 6a05 6401 1900 1400  f...d.|.j.d.....
+00002be0: 1b00 7d0d 7404 7c01 7c00 6a05 6408 1900  ..}.t.|.|.j.d...
+00002bf0: 640c 6403 8d03 5c02 7d0e 7d0f 7406 6a0d  d.d...\.}.}.t.j.
+00002c00: 7c0e 7c0f 6702 6401 640d 8d02 7d10 7c00  |.|.g.d.d...}.|.
+00002c10: a002 740e a00f 7c10 a101 a101 a001 a100  ..t...|.........
+00002c20: a003 a100 7d11 7c0e 6a0a 6401 1900 7d12  ....}.|.j.d...}.
+00002c30: 7c11 6409 7c12 8502 1900 7c11 7c12 6409  |.d.|.....|.|.d.
+00002c40: 8502 1900 1800 7d13 7406 6a0c 7406 a00c  ......}.t.j.t...
+00002c50: 7c13 7c01 6a0a 6401 1900 640a 6602 a102  |.|.j.d...d.f...
+00002c60: 7c01 6a0a 6401 1900 7c05 6a0a 6408 1900  |.j.d...|.j.d...
+00002c70: 640a 6603 640e 640f 8d03 640b 7c00 6a05  d.f.d.d...d.|.j.
+00002c80: 6408 1900 1400 1b00 7d13 7406 a010 6410  d.......}.t...d.
+00002c90: 7c0d 7c13 a103 7d14 7409 7c0a 8301 6401  |.|...}.t.|...d.
+00002ca0: 6b04 9001 72c4 7406 a00b 7c14 6a0a 6408  k...r.t...|.j.d.
+00002cb0: 6409 8502 1900 a101 7c14 7c0a 3c00 7406  d.......|.|.<.t.
+00002cc0: 6a11 7c14 6401 640d 8d02 7d14 7406 a00c  j.|.d.d...}.t...
+00002cd0: 7c14 7c00 6a12 6601 7c03 1700 a102 7d14  |.|.j.f.|.....}.
+00002ce0: 7c14 5300 2911 61b8 0100 000a 2020 2020  |.S.).a.....    
+00002cf0: 2020 2020 436f 6d70 7574 6520 6e75 6d65      Compute nume
+00002d00: 7269 6361 6c20 6772 6164 6965 6e74 7320  rical gradients 
+00002d10: 6f66 2074 6865 2061 7474 6163 6b20 6c6f  of the attack lo
+00002d20: 7373 2074 6572 6d3a 0a20 2020 2020 2020  ss term:.       
+00002d30: 2060 644c 2f64 7820 3d20 2864 4c2f 6450   `dL/dx = (dL/dP
+00002d40: 292a 2864 502f 6478 2960 2077 6974 6820  )*(dP/dx)` with 
+00002d50: 604c 203d 206c 6f73 735f 6174 7461 636b  `L = loss_attack
+00002d60: 5f73 3b20 5020 3d20 7072 6564 6963 743b  _s; P = predict;
+00002d70: 2078 203d 2061 6476 5f73 602e 0a0a 2020   x = adv_s`...  
+00002d80: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00002d90: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00002da0: 2d2d 2d0a 2020 2020 2020 2020 580a 2020  ---.        X.  
+00002db0: 2020 2020 2020 2020 2020 496e 7374 616e            Instan
+00002dc0: 6365 2061 726f 756e 6420 7768 6963 6820  ce around which 
+00002dd0: 6772 6164 6965 6e74 2069 7320 6576 616c  gradient is eval
+00002de0: 7561 7465 642e 0a20 2020 2020 2020 2059  uated..        Y
+00002df0: 0a20 2020 2020 2020 2020 2020 204f 6e65  .            One
+00002e00: 2d68 6f74 2072 6570 7265 7365 6e74 6174  -hot representat
+00002e10: 696f 6e20 6f66 2069 6e73 7461 6e63 6520  ion of instance 
+00002e20: 6c61 6265 6c73 2e0a 2020 2020 2020 2020  labels..        
+00002e30: 6772 6164 735f 7368 6170 650a 2020 2020  grads_shape.    
+00002e40: 2020 2020 2020 2020 5368 6170 6520 6f66          Shape of
+00002e50: 2067 7261 6469 656e 7473 2e0a 0a20 2020   gradients...   
+00002e60: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00002e70: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00002e80: 2020 2020 2041 7272 6179 2077 6974 6820       Array with 
+00002e90: 6772 6164 6965 6e74 732e 0a20 2020 2020  gradients..     
+00002ea0: 2020 2072 0100 0000 5429 01da 0570 726f     r....T)...pro
+00002eb0: 6261 6301 0000 0000 0000 0000 0000 0001  bac.............
+00002ec0: 0000 0004 0000 0013 0000 0073 1200 0000  ...........s....
+00002ed0: 7400 6a01 8800 7c00 1400 6401 6402 8d02  t.j...|...d.d...
+00002ee0: 5300 a903 4e72 1900 0000 72a7 0000 0029  S...Nr....r....)
+00002ef0: 0272 4d00 0000 7278 0000 00a9 015a 0a70  .rM...rx.....Z.p
+00002f00: 7265 6473 5f70 6572 74a9 0172 9700 0000  reds_pert..r....
+00002f10: 7240 0000 0072 4100 0000 da01 66b2 0100  r@...rA.....f...
+00002f20: 0073 0200 0000 0001 7a27 436f 756e 7465  .s......z'Counte
+00002f30: 7266 6163 7475 616c 2e67 6574 5f67 7261  rfactual.get_gra
+00002f40: 6469 656e 7473 2e3c 6c6f 6361 6c73 3e2e  dients.<locals>.
+00002f50: 6663 0100 0000 0000 0000 0000 0000 0100  fc..............
+00002f60: 0000 0400 0000 1300 0000 7316 0000 0074  ..........s....t
+00002f70: 006a 0164 0188 0018 007c 0014 0064 0164  .j.d.....|...d.d
+00002f80: 028d 0253 0072 b800 0000 2902 724d 0000  ...S.r....).rM..
+00002f90: 0072 6200 0000 72b9 0000 0072 ba00 0000  .rb...r....r....
+00002fa0: 7240 0000 0072 4100 0000 da01 67b5 0100  r@...rA.....g...
+00002fb0: 0073 0200 0000 0001 7a27 436f 756e 7465  .s......z'Counte
+00002fc0: 7266 6163 7475 616c 2e67 6574 5f67 7261  rfactual.get_gra
+00002fd0: 6469 656e 7473 2e3c 6c6f 6361 6c73 3e2e  dients.<locals>.
+00002fe0: 6772 1900 0000 4ee9 ffff ffff 7206 0000  gr....N.....r...
+00002ff0: 0046 72a7 0000 00da 0146 2901 da05 6f72  .Fr......F)...or
+00003000: 6465 727a 0a69 6a2c 696a 6b2d 3e69 6b29  derz.ij,ijk->ik)
+00003010: 1372 6f00 0000 da06 6465 7461 6368 721a  .ro.....detachr.
+00003020: 0000 00da 056e 756d 7079 720c 0000 0072  .....numpyr....r
+00003030: 2900 0000 724d 0000 0072 ab00 0000 721d  )...rM...r....r.
+00003040: 0000 0072 7700 0000 721c 0000 0072 4b00  ...rw...r....rK.
+00003050: 0000 da07 7265 7368 6170 65da 0b63 6f6e  ....reshape..con
+00003060: 6361 7465 6e61 7465 723b 0000 0072 5500  catenater;...rU.
+00003070: 0000 da06 6569 6e73 756d 72ad 0000 0072  ....einsumr....r
+00003080: 5400 0000 2915 7232 0000 0072 b500 0000  T...).r2...r....
+00003090: 7297 0000 0072 b600 0000 5a06 585f 7072  r....r....Z.X_pr
+000030a0: 6564 72a6 0000 005a 0e70 7265 6473 5f70  edr....Z.preds_p
+000030b0: 6572 745f 706f 735a 0e70 7265 6473 5f70  ert_posZ.preds_p
+000030c0: 6572 745f 6e65 6772 bb00 0000 72bc 0000  ert_negr....r...
+000030d0: 005a 0a69 6478 5f6e 6f67 7261 645a 0564  .Z.idx_nogradZ.d
+000030e0: 6c5f 6466 5a05 646c 5f64 675a 0564 6c5f  l_dfZ.dl_dgZ.dl_
+000030f0: 6470 5a0a 585f 7065 7274 5f70 6f73 5a0a  dpZ.X_pert_posZ.
+00003100: 585f 7065 7274 5f6e 6567 5a06 585f 7065  X_pert_negZ.X_pe
+00003110: 7274 5a0c 7072 6564 735f 636f 6e63 6174  rtZ.preds_concat
+00003120: 5a06 6e5f 7065 7274 5a05 6470 5f64 78da  Z.n_pertZ.dp_dx.
+00003130: 0567 7261 6473 7240 0000 0072 ba00 0000  .gradsr@...r....
+00003140: 7241 0000 00da 0d67 6574 5f67 7261 6469  rA.....get_gradi
+00003150: 656e 7473 9601 0000 7344 0000 0000 140c  ents....sD......
+00003160: 0312 0102 010c ff0a 040c 030c 0422 0112  ............."..
+00003170: 011c 0110 0110 0108 0124 0302 010c ff0a  .........$......
+00003180: 0312 0118 010a 0118 0104 0114 0114 0102  ................
+00003190: fd04 050c fb04 090e 020e 0118 010e 0114  ................
+000031a0: 017a 1c43 6f75 6e74 6572 6661 6374 7561  .z.Counterfactua
+000031b0: 6c2e 6765 745f 6772 6164 6965 6e74 73e7  l.get_gradients.
+000031c0: bbbd d7d9 df7c db3d 2905 72b5 0000 00da  .....|.=).r.....
+000031d0: 0961 6476 5f63 6c61 7373 da0a 6f72 6967  .adv_class..orig
+000031e0: 5f63 6c61 7373 7229 0000 0072 3000 0000  _classr)...r0...
+000031f0: 6305 0000 0000 0000 0000 0000 000a 0000  c...............
+00003200: 0004 0000 0043 0000 0073 9600 0000 7c00  .....C...s....|.
+00003210: 6a00 7248 7c00 6a01 a002 7c01 a101 7d05  j.rH|.j...|...}.
+00003220: 7c00 6a03 7c02 1900 7d06 7c00 6a03 7c03  |.j.|...}.|.j.|.
+00003230: 1900 7d07 7404 6a05 a006 7c05 7c06 1800  ..}.t.j...|.|...
+00003240: a101 7d08 7404 6a05 a006 7c05 7c07 1800  ..}.t.j...|.|...
+00003250: a101 7d09 6e42 7c00 6a07 7280 7c00 6a08  ..}.nB|.j.r.|.j.
+00003260: 7c02 1900 6a09 740a 6401 6402 8d02 6403  |...j.t.d.d...d.
+00003270: 1900 7d08 7c00 6a08 7c03 1900 6a09 740a  ..}.|.j.|...j.t.
+00003280: 6401 6402 8d02 6403 1900 7d09 6e0a 740b  d.d...d...}.n.t.
+00003290: a00c 6404 a101 0100 7c09 7c08 7c04 1700  ..d.....|.|.|...
+000032a0: 1b00 5300 2905 61f5 0100 000a 2020 2020  ..S.).a.....    
+000032b0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+000032c0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000032d0: 2d0a 2020 2020 2020 2020 580a 2020 2020  -.        X.    
+000032e0: 2020 2020 2020 2020 5065 7274 7572 6261          Perturba
+000032f0: 7469 6f6e 2e0a 2020 2020 2020 2020 6164  tion..        ad
+00003300: 765f 636c 6173 730a 2020 2020 2020 2020  v_class.        
+00003310: 2020 2020 5072 6564 6963 7465 6420 636c      Predicted cl
+00003320: 6173 7320 6f6e 2074 6865 2070 6572 7475  ass on the pertu
+00003330: 7262 6564 2069 6e73 7461 6e63 652e 0a20  rbed instance.. 
+00003340: 2020 2020 2020 206f 7269 675f 636c 6173         orig_clas
+00003350: 730a 2020 2020 2020 2020 2020 2020 5072  s.            Pr
+00003360: 6564 6963 7465 6420 636c 6173 7320 6f6e  edicted class on
+00003370: 2074 6865 206f 7269 6769 6e61 6c20 696e   the original in
+00003380: 7374 616e 6365 2e0a 2020 2020 2020 2020  stance..        
+00003390: 6570 730a 2020 2020 2020 2020 2020 2020  eps.            
+000033a0: 536d 616c 6c20 6e75 6d62 6572 2074 6f20  Small number to 
+000033b0: 6176 6f69 6420 6469 7669 6469 6e67 2062  avoid dividing b
+000033c0: 7920 302e 0a0a 2020 2020 2020 2020 5265  y 0...        Re
+000033d0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+000033e0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 5261  -----.        Ra
+000033f0: 7469 6f20 6265 7477 6565 6e20 7468 6520  tio between the 
+00003400: 6469 7374 616e 6365 2074 6f20 7468 6520  distance to the 
+00003410: 7072 6f74 6f74 7970 6520 6f66 2074 6865  prototype of the
+00003420: 2070 7265 6469 6374 6564 2063 6c61 7373   predicted class
+00003430: 2066 6f72 2074 6865 206f 7269 6769 6e61   for the origina
+00003440: 6c20 696e 7374 616e 6365 2061 6e64 2020  l instance and  
+00003450: 2020 2020 2020 2074 6865 2070 726f 746f         the proto
+00003460: 7479 7065 206f 6620 7468 6520 7072 6564  type of the pred
+00003470: 6963 7465 6420 636c 6173 7320 666f 7220  icted class for 
+00003480: 7468 6520 7065 7274 7572 6265 6420 696e  the perturbed in
+00003490: 7374 616e 6365 2e0a 2020 2020 2020 2020  stance..        
+000034a0: 7219 0000 00a9 01da 016b 7201 0000 007a  r........kr....z
+000034b0: 4b4e 6565 6420 6569 7468 6572 2061 6e20  KNeed either an 
+000034c0: 656e 636f 6465 7220 6f72 2074 6865 206b  encoder or the k
+000034d0: 2d64 2074 7265 6573 2065 6e61 626c 6564  -d trees enabled
+000034e0: 2074 6f20 636f 6d70 7574 6520 6469 7374   to compute dist
+000034f0: 616e 6365 2073 636f 7265 732e 290d 7222  ance scores.).r"
+00003500: 0000 0072 5300 0000 721a 0000 0072 a900  ...rS...r....r..
+00003510: 0000 724d 0000 00da 066c 696e 616c 6772  ..rM.....linalgr
+00003520: 8000 0000 7224 0000 0072 af00 0000 da05  ....r$...r......
+00003530: 7175 6572 795a 0658 7061 7463 6872 5000  queryZ.XpatchrP.
+00003540: 0000 7251 0000 0029 0a72 3200 0000 72b5  ..rQ...).r2...r.
+00003550: 0000 0072 c800 0000 72c9 0000 0072 2900  ...r....r....r).
+00003560: 0000 da05 585f 656e 635a 0961 6476 5f70  ....X_encZ.adv_p
+00003570: 726f 746f 5a0a 6f72 6967 5f70 726f 746f  rotoZ.orig_proto
+00003580: 5a08 6469 7374 5f61 6476 5a09 6469 7374  Z.dist_advZ.dist
+00003590: 5f6f 7269 6772 4000 0000 7240 0000 0072  _origr@...r@...r
+000035a0: 4100 0000 da05 7363 6f72 65da 0100 0073  A.....score....s
+000035b0: 1a00 0000 0014 0601 0c01 0a01 0a01 1001  ................
+000035c0: 1201 0603 1801 1a02 0401 02ff 0403 7a14  ..............z.
+000035d0: 436f 756e 7465 7266 6163 7475 616c 2e73  Counterfactual.s
+000035e0: 636f 7265 72ad 0000 00e9 6400 0000 2908  corer.....d...).
+000035f0: 72b5 0000 0072 9700 0000 da0c 7461 7267  r....r......targ
+00003600: 6574 5f63 6c61 7373 72cb 0000 00da 066b  et_classr......k
+00003610: 5f74 7970 65da 0974 6872 6573 686f 6c64  _type..threshold
+00003620: da0b 7072 696e 745f 6576 6572 7972 3000  ..print_everyr0.
+00003630: 0000 6308 0000 0000 0000 0000 0000 0033  ..c............3
+00003640: 0000 000c 0000 0003 0000 0073 040a 0000  ...........s....
+00003650: 8800 6a00 7c01 6a01 6401 1900 6b02 7314  ..j.|.j.d...k.s.
+00003660: 4a00 8201 7402 7403 7404 7405 6a06 6603  J...t.t.t.t.j.f.
+00003670: 1900 7404 7407 6402 9c03 8700 6601 6403  ..t.t.d.....f.d.
+00003680: 6404 840c 7d08 7c03 6405 7500 7290 7408  d...}.|.d.u.r.t.
+00003690: 7409 8800 6a0a 8301 8301 7d03 7c03 a00b  t...j.....}.|...
+000036a0: 7405 6a0c 7c02 6406 6407 8d02 a101 0100  t.j.|.d.d.......
+000036b0: 8800 6a0d 6406 6b04 7290 740e 6408 a00f  ..j.d.k.r.t.d...
+000036c0: 7405 6a0c 7c02 6406 6407 8d02 a101 8301  t.j.|.d.d.......
+000036d0: 0100 740e 6409 a00f 7c03 a101 8301 0100  ..t.d...|.......
+000036e0: 7c01 7d09 6900 7d0a 8800 6a10 9001 729c  |.}.i.}...j...r.
+000036f0: 8800 6a11 a012 8800 a013 7c01 a101 a101  ..j.......|.....
+00003700: 7d0b 7c04 6405 7500 72c0 8800 6a14 6e04  }.|.d.u.r...j.n.
+00003710: 8800 6a15 7d0c 7c0c a016 a100 4400 5dca  ..j.}.|.....D.].
+00003720: 5c02 7d0d 7d0e 7c0d 7c03 7601 72e0 71ce  \.}.}.|.|.v.r.q.
+00003730: 7c04 6405 7500 72fe 7405 6a17 a018 7c0b  |.d.u.r.t.j...|.
+00003740: 7c0e 1800 a101 7c0a 7c0d 3c00 71ce 7c04  |.....|.|.<.q.|.
+00003750: 6405 7501 72ce 7405 6a17 6a18 7c0b a019  d.u.r.t.j.j.|...
+00003760: 7c0b 6a01 6401 1900 640a a102 7c0e a019  |.j.d...d...|...
+00003770: 7c0e 6a01 6401 1900 640a a102 1800 6406  |.j.d...d.....d.
+00003780: 6407 8d02 7d0f 7405 a01a 7c0f a101 6405  d...}.t...|...d.
+00003790: 7c04 8502 1900 7d10 7c05 640b 6b02 9001  |.....}.|.d.k...
+000037a0: 7266 7405 a01b 7c0f 7c10 1900 a101 7c0a  rft...|.|.....|.
+000037b0: 7c0d 3c00 6e10 7c0f 7c10 640a 1900 1900  |.<.n.|.|.d.....
+000037c0: 7c0a 7c0d 3c00 7405 6a1c 7405 6a1b 7c0e  |.|.<.t.j.t.j.|.
+000037d0: 7c10 1900 6401 6407 8d02 6401 6407 8d02  |...d.d...d.d...
+000037e0: 8800 6a14 7c0d 3c00 71ce 6e8c 8800 6a1d  ..j.|.<.q.n...j.
+000037f0: 9002 7228 7c04 6405 7500 9001 72b2 6406  ..r(|.d.u...r.d.
+00003800: 7d04 6900 8800 5f14 7409 8800 6a0a 8301  }.i..._.t...j...
+00003810: 4400 5d64 7d0d 7c0d 7c03 7601 9001 72d4  D.]d}.|.|.v...r.
+00003820: 9001 71c2 8800 6a1e 7c0d 1900 6a1f 7c09  ..q...j.|...j.|.
+00003830: a020 a100 7c04 640c 8d02 5c02 7d11 7d12  . ..|.d...\.}.}.
+00003840: 7c11 6401 1900 640a 1900 7c0a 7c0d 3c00  |.d...d...|.|.<.
+00003850: 8800 6a21 7c0d 1900 7c12 6401 1900 640a  ..j!|...|.d...d.
+00003860: 1900 1900 a019 6406 640a a102 8800 6a14  ......d.d.....j.
+00003870: 7c0d 3c00 9001 71c2 8800 6a22 9002 7272  |.<...q...j"..rr
+00003880: 7423 7c0a 7c0a 6a24 640d 8d02 8800 5f25  t#|.|.j$d....._%
+00003890: 8800 6a14 8800 6a25 1900 a026 8800 6a27  ..j...j%...&..j'
+000038a0: a101 7d13 8800 6a0d 6406 6b04 9002 727e  ..}...j.d.k...r~
+000038b0: 740e 640e a00f 8800 6a25 a101 8301 0100  t.d.....j%......
+000038c0: 6e0c 7428 a029 8800 6a2a a101 0100 8800  n.t(.)..j*......
+000038d0: 6a01 7d14 7428 a029 8800 6a00 a101 7d15  j.}.t(.)..j...}.
+000038e0: 7428 a02b 8800 6a00 a101 8800 6a2c 1400  t(.+..j.....j,..
+000038f0: 7d16 7428 a02b 8800 6a00 a101 640f 1400  }.t(.+..j...d...
+00003900: 7d17 640f 6701 8800 6a00 1400 7d18 7428  }.d.g...j...}.t(
+00003910: a029 8800 6a01 6406 6405 8502 1900 a101  .)..j.d.d.......
+00003920: 6701 8800 6a00 1400 7d19 7428 a029 8800  g...j...}.t(.)..
+00003930: 6a01 a101 7428 a029 8800 6a01 a101 6602  j...t(.)..j...f.
+00003940: 7d1a 6410 6411 8400 7409 8800 6a2d 8301  }.d.d...t...j-..
+00003950: 4400 8301 8800 5f2e 7409 8800 6a2d 8301  D....._.t...j-..
+00003960: 4400 9006 5db2 7d1b 7c09 a02f a100 a030  D...].}.|../...0
+00003970: a100 8800 5f31 7c02 a02f a100 a030 a100  ...._1|../...0..
+00003980: 8800 5f32 7c16 a02f a100 a030 a100 8800  .._2|../...0....
+00003990: 5f33 7c09 a02f a100 a030 a100 8800 5f34  _3|../...0...._4
+000039a0: 7c09 a02f a100 a035 a100 8800 5f36 7c13  |../...5...._6|.
+000039b0: a02f a100 a030 a100 8800 5f37 8800 a038  ./...0...._7...8
+000039c0: 8800 6a39 a101 0100 640f 6701 8800 6a00  ..j9....d.g...j.
+000039d0: 1400 7d1c 640a 6701 8800 6a00 1400 7d1d  ..}.d.g...j...}.
+000039e0: 6401 8800 5f3a 6700 6700 0200 7d1e 7d1f  d..._:g.g...}.}.
+000039f0: 8800 6a3b a03c a100 0100 8800 a03d a100  ..j;.<.......=..
+00003a00: 0100 8800 a03e a100 0100 7409 8800 6a3f  .....>....t...j?
+00003a10: 8301 4400 9005 5d32 7d20 7405 a029 7c14  ..D...]2} t..)|.
+00003a20: a101 7d21 7405 a029 7c14 a101 7d22 8800  ..}!t..)|...}"..
+00003a30: 6a40 9004 72ee 8800 6a2c 6412 6b03 9003  j@..r...j,d.k...
+00003a40: 73fe 8800 6a2d 6406 6b04 9004 72ee 8800  s...j-d.k...r...
+00003a50: 6a34 a02f a100 a030 a100 7d23 8800 6a36  j4./...0..}#..j6
+00003a60: a02f a100 a030 a100 7d24 7c02 a02f a100  ./...0..}$|../..
+00003a70: a030 a100 a041 a100 7d25 7c1e a042 7c23  .0...A..}%|..B|#
+00003a80: a101 0100 7c1f a042 7c24 a101 0100 7c20  ....|..B|$....| 
+00003a90: 8800 6a43 1600 6401 6b02 9005 7246 7c20  ..jC..d.k...rF| 
+00003aa0: 6401 6b04 9005 7246 8800 6a33 a041 a100  d.k...rF..j3.A..
+00003ab0: 7d0d 7428 a044 7c1e a101 7d1e 7428 a044  }.t(.D|...}.t(.D
+00003ac0: 7c1f a101 7d1f 8800 6a45 7c1e 7c25 7c14  |...}...jE|.|%|.
+00003ad0: 6406 6405 8502 1900 6413 8d03 7c0d 1400  d.d.....d...|...
+00003ae0: 7d21 8800 6a45 7c1f 7c25 7c14 6406 6405  }!..jE|.|%|.d.d.
+00003af0: 8502 1900 6413 8d03 7c0d 1400 7d22 7405  ....d...|...}"t.
+00003b00: a046 7c21 8800 6a46 6401 1900 8800 6a46  .F|!..jFd.....jF
+00003b10: 6406 1900 a103 7d21 7405 a046 7c22 8800  d.....}!t..F|"..
+00003b20: 6a46 6401 1900 8800 6a46 6406 1900 a103  jFd.....jFd.....
+00003b30: 7d22 6700 6700 0200 7d1e 7d1f 6e58 8800  }"g.g...}.}.nX..
+00003b40: 6a40 9005 7346 8800 6a47 a048 a100 0100  j@..sF..jG.H....
+00003b50: 7428 a049 a100 8f2c 0100 8800 6a36 6a4a  t(.I...,....j6jJ
+00003b60: a04b 8800 6a46 6401 1900 8800 6a46 6406  .K..jFd.....jFd.
+00003b70: 1900 a102 0100 5700 6405 0400 0400 8303  ......W.d.......
+00003b80: 0100 6e12 3100 9005 733c 3000 0100 0100  ..n.1...s<0.....
+00003b90: 0100 5900 0100 8800 6a4c 6a48 6414 6415  ..Y.....jLjHd.d.
+00003ba0: 8d01 0100 7428 a049 a100 8f76 0100 8800  ....t(.I...v....
+00003bb0: 6a40 9005 7284 8800 6a36 6a4a a04b 8800  j@..r...j6jJ.K..
+00003bc0: 6a46 6401 1900 8800 6a46 6406 1900 a102  jFd.....jFd.....
+00003bd0: 0100 6e24 8800 6a36 6a4a a04b 8800 6a46  ..n$..j6jJ.K..jF
+00003be0: 6401 1900 6416 1400 8800 6a46 6406 1900  d...d.....jFd...
+00003bf0: 6416 1400 a102 0100 8800 6a36 6a4a a04d  d.........j6jJ.M
+00003c00: 7428 a04e 7c22 a101 a101 0100 8800 6a36  t(.N|"........j6
+00003c10: 6a4a 7d26 5700 6405 0400 0400 8303 0100  jJ}&W.d.........
+00003c20: 6e12 3100 9005 73da 3000 0100 0100 0100  n.1...s.0.......
+00003c30: 5900 0100 8800 6a3b a04f a100 0100 8800  Y.....j;.O......
+00003c40: 6a50 a04f a100 0100 8800 0400 6a3a 6406  jP.O........j:d.
+00003c50: 3700 0200 5f3a 7428 a049 a100 8f2c 0100  7..._:t(.I...,..
+00003c60: 8800 a051 8800 6a52 a101 0100 8800 a053  ...Q..jR.......S
+00003c70: a100 0100 8800 a054 a100 0100 5700 6405  .......T....W.d.
+00003c80: 0400 0400 8303 0100 6e12 3100 9006 7342  ........n.1...sB
+00003c90: 3000 0100 0100 0100 5900 0100 8800 6a3b  0.......Y.....j;
+00003ca0: a03c a100 0100 8800 a03d a100 0100 8800  .<.......=......
+00003cb0: a03e a100 0100 7428 a049 a100 9002 8f74  .>....t(.I.....t
+00003cc0: 0100 8800 6a0d 6406 6b04 9007 72bc 7c20  ....j.d.k...r.| 
+00003cd0: 7c07 1600 6401 6b02 9007 72bc 7428 a055  |...d.k...r.t(.U
+00003ce0: 8800 6a56 7c02 1400 a101 7d27 7428 a057  ..jV|.....}'t(.W
+00003cf0: 6406 7c02 1800 8800 6a56 1400 a101 7d28  d.|.....jV....}(
+00003d00: 740e 6417 a00f 7c20 7c16 6401 1900 a102  t.d...| |.d.....
+00003d10: 8301 0100 740e 6418 a00f 8800 6a58 8800  ....t.d.....jX..
+00003d20: 6a59 a102 8301 0100 740e 6419 a00f 8800  jY......t.d.....
+00003d30: 6a5a 8800 6a5b a102 8301 0100 740e 641a  jZ..j[......t.d.
+00003d40: a00f 8800 6a5c a101 8301 0100 740e 641b  ....j\......t.d.
+00003d50: a00f 7c27 7c28 a102 8301 0100 7c26 6405  ..|'|(......|&d.
+00003d60: 7501 9007 7260 7c26 a030 a100 a020 a100  u...r`|&.0... ..
+00003d70: a041 a100 7d29 740e 641c a00f 7c29 a023  .A..})t.d...|).#
+00003d80: a100 7c29 a057 a100 a102 8301 0100 740e  ..|).W........t.
+00003d90: 641d a00f 7c29 a01b a100 7405 a01b 7405  d...|)....t...t.
+00003da0: a05d 7c29 a101 a101 a102 8301 0100 6e10  .]|)..........n.
+00003db0: 740e 641e 8301 0100 740e 641f 8301 0100  t.d.....t.d.....
+00003dc0: 8800 6a40 9007 72b2 740e 6420 a00f 7c21  ..j@..r.t.d ..|!
+00003dd0: a023 a100 7c21 a057 a100 a102 8301 0100  .#..|!.W........
+00003de0: 740e 6421 a00f 7405 a01b 7c21 a101 7405  t.d!..t...|!..t.
+00003df0: a01b 7405 a05d 7c21 a101 a101 a102 8301  ..t..]|!........
+00003e00: 0100 745e 6a5f a060 a100 0100 7461 7462  ..t^j_.`....tatb
+00003e10: 8800 6a63 8800 6a56 8800 6a34 8303 8301  ..jc..jV..j4....
+00003e20: 4400 9001 5d00 5c02 7d2a 5c03 7d2b 7d2c  D...].\.}*\.}+},
+00003e30: 7d2d 7428 a00c 7c02 7c2a 1900 a101 7d2e  }-t(..|.|*....}.
+00003e40: 7428 a00c 7c2c a101 7d2f 7c2d a064 6401  t(..|,..}/|-.dd.
+00003e50: a101 7d2d 7c06 6412 6b04 9008 722c 8800  ..}-|.d.k...r,..
+00003e60: a065 7c2d 7405 a00c 7456 a101 7c2e a103  .e|-t...tV..|...
+00003e70: 7d30 7c30 7c06 6b04 7d31 6e04 6414 7d31  }0|0|.k.}1n.d.}1
+00003e80: 7c2b 7c1c 7c2a 1900 6b00 9008 726a 7c08  |+|.|*..k...rj|.
+00003e90: 7c2c 7c2e 8302 9008 726a 7c31 9008 726a  |,|.....rj|1..rj
+00003ea0: 7c2f 7c03 7600 9008 726a 7c2b 7c1c 7c2a  |/|.v...rj|+|.|*
+00003eb0: 3c00 7c2f 7c1d 7c2a 3c00 7c2b 7c18 7c2a  <.|/|.|*<.|+|.|*
+00003ec0: 1900 6b00 9007 72d2 7c08 7c2c 7c2e 8302  ..k...r.|.|,|...
+00003ed0: 9007 72d2 7c31 9007 72d2 7c2f 7c03 7600  ..r.|1..r.|/|.v.
+00003ee0: 9007 72d2 8800 6a0d 6406 6b04 9008 72a8  ..r...j.d.k...r.
+00003ef0: 740e 6422 8301 0100 7c2b 7c18 7c2a 3c00  t.d"....|+|.|*<.
+00003f00: 7c2d 7c19 7c2a 3c00 7c26 7d1a 6414 8800  |-|.|*<.|&}.d...
+00003f10: 5f66 8800 6a2e 7c1b 1900 a042 7c2d a101  _f..j.|....B|-..
+00003f20: 0100 9007 71d2 5700 6405 0400 0400 8303  ....q.W.d.......
+00003f30: 0100 6e12 3100 9008 73ec 3000 0100 0100  ..n.1...s.0.....
+00003f40: 0100 5900 0100 9003 71c4 7409 8800 6a00  ..Y.....q.t...j.
+00003f50: 8301 4400 5dbe 7d2a 7c08 7c1d 7c2a 1900  ..D.].}*|.|.|*..
+00003f60: 7405 a00c 7c02 7c2a 1900 a020 a100 a101  t...|.|*... ....
+00003f70: 8302 9009 7272 7c1d 7c2a 1900 640a 6b03  ....rr|.|*..d.k.
+00003f80: 9009 7272 7423 7c17 7c2a 1900 7c16 7c2a  ..rrt#|.|*..|.|*
+00003f90: 1900 8302 7c17 7c2a 3c00 7c17 7c2a 1900  ....|.|*<.|.|*..
+00003fa0: 6423 6b00 9009 72c0 7c15 7c2a 1900 7c17  d#k...r.|.|*..|.
+00003fb0: 7c2a 1900 1700 6416 1b00 7c16 7c2a 3c00  |*....d...|.|*<.
+00003fc0: 6e4e 7457 7c15 7c2a 1900 7c16 7c2a 1900  nNtW|.|*..|.|*..
+00003fd0: 8302 7c15 7c2a 3c00 7c17 7c2a 1900 6423  ..|.|*<.|.|*..d#
+00003fe0: 6b00 9009 72b0 7c15 7c2a 1900 7c17 7c2a  k...r.|.|*..|.|*
+00003ff0: 1900 1700 6416 1b00 7c16 7c2a 3c00 6e10  ....d...|.|*<.n.
+00004000: 7c16 7c2a 0500 1900 6424 3900 0300 3c00  |.|*....d$9...<.
+00004010: 9009 7104 9003 7112 7405 6a67 6425 6426  ..q...q.t.jgd%d&
+00004020: 8400 7c19 4400 8301 6401 6407 8d02 7d32  ..|.D...d.d...}2
+00004030: 7c32 6a01 8800 6a01 6b03 9009 72fc 7405  |2j...j.k...r.t.
+00004040: 6a1c 7c32 6401 6407 8d02 7d32 7c32 7c1a  j.|2d.d...}2|2|.
+00004050: 6602 5300 2927 61ad 0600 000a 2020 2020  f.S.)'a.....    
+00004060: 2020 2020 4669 6e64 2061 2063 6f75 6e74      Find a count
+00004070: 6572 6661 6374 7561 6c20 2843 4629 2066  erfactual (CF) f
+00004080: 6f72 2069 6e73 7461 6e63 6520 6058 6020  or instance `X` 
+00004090: 7573 696e 6720 6120 6661 7374 2069 7465  using a fast ite
+000040a0: 7261 7469 7665 2073 6872 696e 6b61 6765  rative shrinkage
+000040b0: 2d74 6872 6573 686f 6c64 696e 6720 616c  -thresholding al
+000040c0: 676f 7269 7468 6d20 2846 4953 5441 292e  gorithm (FISTA).
+000040d0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+000040e0: 7465 7273 206d 6b0a 2020 2020 2020 2020  ters mk.        
+000040f0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00004100: 2020 2058 0a20 2020 2020 2020 2020 2020     X.           
+00004110: 2049 6e73 7461 6e63 6520 746f 2061 7474   Instance to att
+00004120: 6163 6b2e 0a20 2020 2020 2020 2059 0a20  ack..        Y. 
+00004130: 2020 2020 2020 2020 2020 204c 6162 656c             Label
+00004140: 7320 666f 7220 6058 6020 6173 206f 6e65  s for `X` as one
+00004150: 2d68 6f74 2d65 6e63 6f64 696e 672e 0a20  -hot-encoding.. 
+00004160: 2020 2020 2020 2074 6172 6765 745f 636c         target_cl
+00004170: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
+00004180: 4c69 7374 2077 6974 6820 7461 7267 6574  List with target
+00004190: 2063 6c61 7373 6573 2075 7365 6420 746f   classes used to
+000041a0: 2066 696e 6420 636c 6f73 6573 7420 7072   find closest pr
+000041b0: 6f74 6f74 7970 652e 2049 6620 6060 4e6f  ototype. If ``No
+000041c0: 6e65 6060 2c20 7468 6520 6e65 6172 6573  ne``, the neares
+000041d0: 7420 7072 6f74 6f74 7970 650a 2020 2020  t prototype.    
+000041e0: 2020 2020 2020 2020 6578 6365 7074 2066          except f
+000041f0: 6f72 2074 6865 2070 7265 6469 6374 2063  or the predict c
+00004200: 6c61 7373 206f 6e20 7468 6520 696e 7374  lass on the inst
+00004210: 616e 6365 2069 7320 7573 6564 2e0a 2020  ance is used..  
+00004220: 2020 2020 2020 6b0a 2020 2020 2020 2020        k.        
+00004230: 2020 2020 4e75 6d62 6572 206f 6620 6e65      Number of ne
+00004240: 6172 6573 7420 696e 7374 616e 6365 7320  arest instances 
+00004250: 7573 6564 2074 6f20 6465 6669 6e65 2074  used to define t
+00004260: 6865 2070 726f 746f 7479 7065 2066 6f72  he prototype for
+00004270: 2061 2063 6c61 7373 2e20 4465 6661 756c   a class. Defaul
+00004280: 7473 2074 6f20 7573 696e 6720 616c 6c0a  ts to using all.
+00004290: 2020 2020 2020 2020 2020 2020 696e 7374              inst
+000042a0: 616e 6365 7320 6265 6c6f 6e67 696e 6720  ances belonging 
+000042b0: 746f 2074 6865 2063 6c61 7373 2069 6620  to the class if 
+000042c0: 616e 2065 6e63 6f64 6572 2069 7320 7573  an encoder is us
+000042d0: 6564 2061 6e64 2074 6f20 3120 666f 7220  ed and to 1 for 
+000042e0: 6b2d 6420 7472 6565 732e 0a20 2020 2020  k-d trees..     
+000042f0: 2020 206b 5f74 7970 650a 2020 2020 2020     k_type.      
+00004300: 2020 2020 2020 5573 6520 6569 7468 6572        Use either
+00004310: 2074 6865 2061 7665 7261 6765 2065 6e63   the average enc
+00004320: 6f64 696e 6720 6f66 2074 6865 206b 206e  oding of the k n
+00004330: 6561 7265 7374 2069 6e73 7461 6e63 6573  earest instances
+00004340: 2069 6e20 6120 636c 6173 7320 2860 606b   in a class (``k
+00004350: 5f74 7970 653d 276d 6561 6e27 6060 2920  _type='mean'``) 
+00004360: 6f72 0a20 2020 2020 2020 2020 2020 2074  or.            t
+00004370: 6865 206b 2d6e 6561 7265 7374 2065 6e63  he k-nearest enc
+00004380: 6f64 696e 6720 696e 2074 6865 2063 6c61  oding in the cla
+00004390: 7373 2028 6060 6b5f 7479 7065 3d27 706f  ss (``k_type='po
+000043a0: 696e 7427 6060 2920 746f 2064 6566 696e  int'``) to defin
+000043b0: 6520 7468 6520 7072 6f74 6f74 7970 6520  e the prototype 
+000043c0: 6f66 2074 6861 7420 636c 6173 732e 0a20  of that class.. 
+000043d0: 2020 2020 2020 2020 2020 204f 6e6c 7920             Only 
+000043e0: 7265 6c65 7661 6e74 2069 6620 616e 2065  relevant if an e
+000043f0: 6e63 6f64 6572 2069 7320 7573 6564 2074  ncoder is used t
+00004400: 6f20 6465 6669 6e65 2074 6865 2070 726f  o define the pro
+00004410: 746f 7479 7065 732e 0a20 2020 2020 2020  totypes..       
+00004420: 2074 6872 6573 686f 6c64 0a20 2020 2020   threshold.     
+00004430: 2020 2020 2020 2054 6872 6573 686f 6c64         Threshold
+00004440: 206c 6576 656c 2066 6f72 2074 6865 2072   level for the r
+00004450: 6174 696f 2062 6574 7765 656e 2074 6865  atio between the
+00004460: 2064 6973 7461 6e63 6520 6f66 2074 6865   distance of the
+00004470: 2063 6f75 6e74 6572 6661 6374 7561 6c20   counterfactual 
+00004480: 746f 2074 6865 2070 726f 746f 7479 7065  to the prototype
+00004490: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
+000044a0: 2020 2020 7072 6564 6963 7465 6420 636c      predicted cl
+000044b0: 6173 7320 666f 7220 7468 6520 6f72 6967  ass for the orig
+000044c0: 696e 616c 2069 6e73 7461 6e63 6520 6f76  inal instance ov
+000044d0: 6572 2074 6865 2064 6973 7461 6e63 6520  er the distance 
+000044e0: 746f 2074 6865 2070 726f 746f 7479 7065  to the prototype
+000044f0: 206f 6620 7468 6520 7072 6564 6963 7465   of the predicte
+00004500: 6420 636c 6173 730a 2020 2020 2020 2020  d class.        
+00004510: 2020 2020 666f 7220 7468 6520 636f 756e      for the coun
+00004520: 7465 7266 6163 7475 616c 2e20 4966 2074  terfactual. If t
+00004530: 6865 2074 7275 7374 2073 636f 7265 2069  he trust score i
+00004540: 7320 6265 6c6f 7720 7468 6520 7468 7265  s below the thre
+00004550: 7368 6f6c 642c 2074 6865 2070 726f 706f  shold, the propo
+00004560: 7365 6420 636f 756e 7465 7266 6163 7475  sed counterfactu
+00004570: 616c 2064 6f65 730a 2020 2020 2020 2020  al does.        
+00004580: 2020 2020 6e6f 7420 6d65 6574 2074 6865      not meet the
+00004590: 2072 6571 7569 7265 6d65 6e74 732e 0a20   requirements.. 
+000045a0: 2020 2020 2020 2076 6572 626f 7369 7479         verbosity
+000045b0: 0a20 2020 2020 2020 2020 2020 2050 7269  .            Pri
+000045c0: 6e74 2069 6e74 6572 6d65 6469 6174 6520  nt intermediate 
+000045d0: 7265 7375 6c74 7320 6f66 206f 7074 696d  results of optim
+000045e0: 697a 6174 696f 6e20 6966 2067 7265 6174  ization if great
+000045f0: 6572 2074 6861 6e20 312e 0a20 2020 2020  er than 1..     
+00004600: 2020 2070 7269 6e74 5f65 7665 7279 0a20     print_every. 
+00004610: 2020 2020 2020 2020 2020 2050 7269 6e74             Print
+00004620: 2066 7265 7175 656e 6379 2069 6620 7665   frequency if ve
+00004630: 7262 6f73 6520 6973 2067 7265 6174 6572  rbose is greater
+00004640: 2074 6861 6e20 312e 0a20 2020 2020 2020   than 1..       
+00004650: 206c 6f67 5f65 7665 7279 0a20 2020 2020   log_every.     
+00004660: 2020 2020 2020 2060 7465 6e73 6f72 626f         `tensorbo
+00004670: 6172 6460 206c 6f67 2066 7265 7175 656e  ard` log frequen
+00004680: 6379 2069 6620 7772 6974 6520 6469 7265  cy if write dire
+00004690: 6374 6f72 7920 6973 2073 7065 6369 6669  ctory is specifi
+000046a0: 6564 2e0a 0a20 2020 2020 2020 2052 6574  ed...        Ret
+000046b0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+000046c0: 2d2d 2d2d 0a20 2020 2020 2020 204f 7665  ----.        Ove
+000046d0: 7261 6c6c 2062 6573 7420 6174 7461 636b  rall best attack
+000046e0: 2061 6e64 2067 7261 6469 656e 7473 2066   and gradients f
+000046f0: 6f72 2074 6861 7420 6174 7461 636b 2e0a  or that attack..
+00004700: 2020 2020 2020 2020 7201 0000 0029 03da          r....)..
+00004710: 0178 da01 7972 3000 0000 6302 0000 0000  .x..yr0...c.....
+00004720: 0000 0000 0000 0002 0000 0005 0000 0013  ................
+00004730: 0000 0073 4600 0000 7400 7c00 7401 7402  ...sF...t.|.t.t.
+00004740: 7403 6a04 6603 8302 733e 7405 7c00 8301  t.j.f...s>t.|...
+00004750: 733e 7c00 a006 a100 7d00 7c00 7c01 0500  s>|.....}.|.|...
+00004760: 1900 8800 6a07 3700 0300 3c00 7408 a009  ....j.7...<.t...
+00004770: 7c00 a101 7d00 7c00 7c01 6b03 5300 2901  |...}.|.|.k.S.).
+00004780: 6185 0100 000a 2020 2020 2020 2020 2020  a.....          
+00004790: 2020 436f 6d70 6172 6520 7072 6564 6963    Compare predic
+000047a0: 7469 6f6e 7320 7769 7468 2074 6172 6765  tions with targe
+000047b0: 7420 6c61 6265 6c73 2061 6e64 2072 6574  t labels and ret
+000047c0: 7572 6e20 7768 6574 6865 7220 636f 756e  urn whether coun
+000047d0: 7465 7266 6163 7475 616c 2063 6f6e 6469  terfactual condi
+000047e0: 7469 6f6e 7320 686f 6c64 2e0a 0a20 2020  tions hold...   
+000047f0: 2020 2020 2020 2020 2050 6172 616d 6574           Paramet
+00004800: 6572 730a 2020 2020 2020 2020 2020 2020  ers.            
+00004810: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00004820: 2020 2020 2020 2078 0a20 2020 2020 2020         x.       
+00004830: 2020 2020 2020 2020 2050 7265 6469 6374           Predict
+00004840: 6564 2063 6c61 7373 2070 726f 6261 6269  ed class probabi
+00004850: 6c69 7469 6573 206f 7220 6c61 6265 6c73  lities or labels
+00004860: 2e0a 2020 2020 2020 2020 2020 2020 790a  ..            y.
+00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004880: 5461 7267 6574 206f 7220 7072 6564 6963  Target or predic
+00004890: 7465 6420 6c61 6265 6c73 2e0a 0a20 2020  ted labels...   
+000048a0: 2020 2020 2020 2020 2052 6574 7572 6e73           Returns
+000048b0: 0a20 2020 2020 2020 2020 2020 202d 2d2d  .            ---
+000048c0: 2d2d 2d2d 0a20 2020 2020 2020 2020 2020  ----.           
+000048d0: 2042 6f6f 6c20 7768 6574 6865 7220 636f   Bool whether co
+000048e0: 756e 7465 7266 6163 7475 616c 2063 6f6e  unterfactual con
+000048f0: 6469 7469 6f6e 7320 686f 6c64 2e0a 2020  ditions hold..  
+00004900: 2020 2020 2020 2020 2020 290a 7239 0000            ).r9..
+00004910: 0072 3a00 0000 da03 696e 7472 4d00 0000  .r:.....intrM...
+00004920: da05 696e 7436 34da 1d69 735f 7369 6e67  ..int64..is_sing
+00004930: 6c65 5f66 6c6f 6174 5f6f 725f 696e 745f  le_float_or_int_
+00004940: 7465 6e73 6f72 726f 0000 0072 1d00 0000  tensorro...r....
+00004950: 723b 0000 00da 0661 7267 6d61 7829 0272  r;.....argmax).r
+00004960: d500 0000 72d6 0000 0072 6c00 0000 7240  ....r....rl...r@
+00004970: 0000 0072 4100 0000 da07 636f 6d70 6172  ...rA.....compar
+00004980: 652f 0200 0073 0e00 0000 000f 1201 06ff  e/...s..........
+00004990: 0203 0801 1201 0a01 7a26 436f 756e 7465  ........z&Counte
+000049a0: 7266 6163 7475 616c 2e61 7474 6163 6b2e  rfactual.attack.
+000049b0: 3c6c 6f63 616c 733e 2e63 6f6d 7061 7265  <locals>.compare
+000049c0: 4e72 1900 0000 72a7 0000 007a 1350 7265  Nr....r....z.Pre
+000049d0: 6469 6374 6564 2063 6c61 7373 3a20 7b7d  dicted class: {}
+000049e0: 7a12 5461 7267 6574 2063 6c61 7373 6573  z.Target classes
+000049f0: 3a20 7b7d 72bd 0000 0072 ad00 0000 72ca  : {}r....r....r.
+00004a00: 0000 0029 0172 5c00 0000 7a13 5072 6f74  ...).r\...z.Prot
+00004a10: 6f74 7970 6520 636c 6173 733a 207b 7d72  otype class: {}r
+00004a20: 1100 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00004a30: 0002 0000 0004 0000 0053 0000 0073 1200  .........S...s..
+00004a40: 0000 6900 7c00 5d0a 7d01 7c01 6700 9302  ..i.|.].}.|.g...
+00004a50: 7104 5300 7240 0000 0072 4000 0000 2902  q.S.r@...r@...).
+00004a60: 723d 0000 0072 b100 0000 7240 0000 0072  r=...r....r@...r
+00004a70: 4000 0000 7241 0000 00da 0a3c 6469 6374  @...rA.....<dict
+00004a80: 636f 6d70 3e8a 0200 0072 9c00 0000 7a29  comp>....r....z)
+00004a90: 436f 756e 7465 7266 6163 7475 616c 2e61  Counterfactual.a
+00004aa0: 7474 6163 6b2e 3c6c 6f63 616c 733e 2e3c  ttack.<locals>.<
+00004ab0: 6469 6374 636f 6d70 3e72 0e00 0000 2901  dictcomp>r....).
+00004ac0: 72b6 0000 0054 2901 da0c 7265 7461 696e  r....T)...retain
+00004ad0: 5f67 7261 7068 7206 0000 007a 190a 4974  _graphr....z..It
+00004ae0: 6572 6174 696f 6e3a 207b 7d3b 2043 6f6e  eration: {}; Con
+00004af0: 7374 3a20 7b7d 7a27 4c6f 7373 2074 6f74  st: {}z'Loss tot
+00004b00: 616c 3a20 7b3a 2e33 667d 2c20 6c6f 7373  al: {:.3f}, loss
+00004b10: 2061 7474 6163 6b3a 207b 3a2e 3366 7d7a   attack: {:.3f}z
+00004b20: 164c 323a 207b 3a2e 3366 7d2c 204c 313a  .L2: {:.3f}, L1:
+00004b30: 207b 3a2e 3366 7d7a 124c 6f73 7320 7072   {:.3f}z.Loss pr
+00004b40: 6f74 6f3a 207b 3a2e 3366 7d7a 3254 6172  oto: {:.3f}z2Tar
+00004b50: 6765 7420 7072 6f62 613a 207b 3a2e 3266  get proba: {:.2f
+00004b60: 7d2c 206d 6178 206e 6f6e 2074 6172 6765  }, max non targe
+00004b70: 7420 7072 6f62 613a 207b 3a2e 3266 7d7a  t proba: {:.2f}z
+00004b80: 1f47 7261 6469 656e 7420 6d69 6e2f 6d61  .Gradient min/ma
+00004b90: 783a 207b 3a2e 3366 7d2f 7b3a 2e33 667d  x: {:.3f}/{:.3f}
+00004ba0: 7a25 4772 6164 6965 6e74 206d 6561 6e2f  z%Gradient mean/
+00004bb0: 6162 7320 6d65 616e 3a20 7b3a 2e33 667d  abs mean: {:.3f}
+00004bc0: 2f7b 3a2e 3366 7d7a 1647 7261 6469 656e  /{:.3f}z.Gradien
+00004bd0: 7420 6d69 6e2f 6d61 783a 204e 6f6e 657a  t min/max: Nonez
+00004be0: 1c47 7261 6469 656e 7420 6d65 616e 2f61  .Gradient mean/a
+00004bf0: 6273 206d 6561 6e3a 204e 6f6e 657a 3047  bs mean: Nonez0G
+00004c00: 7261 6469 656e 7420 6e75 6d65 7269 6361  radient numerica
+00004c10: 6c20 6174 7461 636b 206d 696e 2f6d 6178  l attack min/max
+00004c20: 3a20 7b3a 2e33 667d 2f7b 3a2e 3366 7d7a  : {:.3f}/{:.3f}z
+00004c30: 2f47 7261 6469 656e 7420 6e75 6d65 7269  /Gradient numeri
+00004c40: 6361 6c20 6d65 616e 2f61 6273 206d 6561  cal mean/abs mea
+00004c50: 6e3a 207b 3a2e 3366 7d2f 7b3a 2e33 667d  n: {:.3f}/{:.3f}
+00004c60: 7a1f 0a4e 6577 2062 6573 7420 636f 756e  z..New best coun
+00004c70: 7465 7266 6163 7475 616c 2066 6f75 6e64  terfactual found
+00004c80: 2167 0000 0000 65cd cd41 7215 0000 0063  !g....e..Ar....c
+00004c90: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00004ca0: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
+00004cb0: 005d 0c7d 017c 01a0 00a1 0091 0271 0453  .].}.|.......q.S
+00004cc0: 0072 4000 0000 2901 7236 0000 0029 0272  .r@...).r6...).r
+00004cd0: 3d00 0000 da04 6974 656d 7240 0000 0072  =.....itemr@...r
+00004ce0: 4000 0000 7241 0000 0072 4200 0000 6803  @...rA...rB...h.
+00004cf0: 0000 729c 0000 007a 2943 6f75 6e74 6572  ..r....z)Counter
+00004d00: 6661 6374 7561 6c2e 6174 7461 636b 2e3c  factual.attack.<
+00004d10: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00004d20: 703e 2968 7254 0000 0072 1c00 0000 7205  p>)hrT...r....r.
+00004d30: 0000 0072 3a00 0000 72d7 0000 0072 4d00  ...r:...r....rM.
+00004d40: 0000 da07 6e64 6172 7261 79da 0462 6f6f  ....ndarray..boo
+00004d50: 6cda 046c 6973 7472 5700 0000 724c 0000  l..listrW...rL..
+00004d60: 0072 5b00 0000 72da 0000 0072 2d00 0000  .r[...r....r-...
+00004d70: da05 7072 696e 74da 0666 6f72 6d61 7472  ..print..formatr
+00004d80: 2200 0000 7253 0000 0072 1a00 0000 721b  "...rS...r....r.
+00004d90: 0000 0072 a900 0000 72aa 0000 00da 0569  ...r....r......i
+00004da0: 7465 6d73 72cc 0000 0072 8000 0000 72c2  temsr....r....r.
+00004db0: 0000 00da 0761 7267 736f 7274 72ad 0000  .....argsortr...
+00004dc0: 0072 ac00 0000 7224 0000 0072 af00 0000  .r....r$...r....
+00004dd0: 72cd 0000 0072 3600 0000 72b0 0000 0072  r....r6...r....r
+00004de0: 3800 0000 7261 0000 00da 0367 6574 da08  8...ra.....get..
+00004df0: 6964 5f70 726f 746f da02 746f 722f 0000  id_proto..tor/..
+00004e00: 0072 3b00 0000 724b 0000 0072 5800 0000  .r;...rK...rX...
+00004e10: 723c 0000 0072 2700 0000 7228 0000 00da  r<...r'...r(....
+00004e20: 0963 665f 676c 6f62 616c 726f 0000 0072  .cf_globalro...r
+00004e30: c000 0000 725f 0000 0072 8800 0000 728e  ....r_...r....r.
+00004e40: 0000 0072 6900 0000 da0e 7265 7175 6972  ...ri.....requir
+00004e50: 6573 5f67 7261 645f 725e 0000 0072 9000  es_grad_r^...r..
+00004e60: 0000 72a4 0000 0072 2500 0000 7267 0000  ..r....r%...rg..
+00004e70: 0072 9d00 0000 da09 7a65 726f 5f67 7261  .r......zero_gra
+00004e80: 6472 8f00 0000 7296 0000 0072 2600 0000  dr....r....r&...
+00004e90: 722e 0000 0072 c100 0000 da06 6170 7065  r....r......appe
+00004ea0: 6e64 722b 0000 00da 0363 6174 72c6 0000  ndr+.....catr...
+00004eb0: 0072 2a00 0000 728a 0000 00da 0862 6163  .r*...r......bac
+00004ec0: 6b77 6172 6472 8600 0000 da04 6772 6164  kwardr......grad
+00004ed0: da06 636c 616d 705f 7294 0000 00da 0461  ..clamp_r......a
+00004ee0: 6464 5fda 0a66 726f 6d5f 6e75 6d70 79da  dd_..from_numpy.
+00004ef0: 0473 7465 7072 a300 0000 7266 0000 0072  .stepr....rf...r
+00004f00: 1f00 0000 726d 0000 0072 7100 0000 7278  ....rm...rq...rx
+00004f10: 0000 0072 8500 0000 7262 0000 0072 9500  ...r....rb...r..
+00004f20: 0000 7289 0000 0072 7d00 0000 727c 0000  ..r....r}...r|..
+00004f30: 0072 9100 0000 7260 0000 00da 0373 7973  .r....r`.....sys
+00004f40: da06 7374 646f 7574 da05 666c 7573 68da  ..stdout..flush.
+00004f50: 0965 6e75 6d65 7261 7465 da03 7a69 7072  .enumerate..zipr
+00004f60: 7b00 0000 da09 756e 7371 7565 657a 6572  {.....unsqueezer
+00004f70: cf00 0000 da0b 6265 7374 5f61 7474 6163  ......best_attac
+00004f80: 6b72 c300 0000 2933 7232 0000 0072 b500  kr....)3r2...r..
+00004f90: 0000 7297 0000 0072 d100 0000 72cb 0000  ..r....r....r...
+00004fa0: 0072 d200 0000 72d3 0000 0072 d400 0000  .r....r....r....
+00004fb0: 72db 0000 005a 0558 5f6e 756d 5a0a 6469  r....Z.X_numZ.di
+00004fc0: 7374 5f70 726f 746f 72ce 0000 00da 0a63  st_protor......c
+00004fd0: 6c61 7373 5f64 6963 74da 0163 da01 765a  lass_dict..c..vZ
+00004fe0: 0664 6973 745f 6b72 b200 0000 5a06 6469  .dist_kr....Z.di
+00004ff0: 7374 5f63 5a05 6964 785f 635a 0970 726f  st_cZ.idx_cZ.pro
+00005000: 746f 5f76 616c 5a0a 7065 7274 5f73 6861  to_valZ.pert_sha
+00005010: 7065 5a08 636f 6e73 745f 6c62 728e 0000  peZ.const_lbr...
+00005020: 005a 0863 6f6e 7374 5f75 625a 116f 7665  .Z.const_ubZ.ove
+00005030: 7261 6c6c 5f62 6573 745f 6469 7374 5a13  rall_best_distZ.
+00005040: 6f76 6572 616c 6c5f 6265 7374 5f61 7474  overall_best_att
+00005050: 6163 6b5a 116f 7665 7261 6c6c 5f62 6573  ackZ.overall_bes
+00005060: 745f 6772 6164 723e 0000 005a 1163 7572  t_gradr>...Z.cur
+00005070: 7265 6e74 5f62 6573 745f 6469 7374 5a12  rent_best_distZ.
+00005080: 6375 7272 656e 745f 6265 7374 5f70 726f  current_best_pro
+00005090: 6261 5a0b 585f 6465 725f 6261 7463 685a  baZ.X_der_batchZ
+000050a0: 0d58 5f64 6572 5f62 6174 6368 5f73 72b1  .X_der_batch_sr.
+000050b0: 0000 005a 0967 7261 6473 5f6e 756d 5a0b  ...Z.grads_numZ.
+000050c0: 6772 6164 735f 6e75 6d5f 735a 0558 5f64  grads_num_sZ.X_d
+000050d0: 6572 5a07 585f 6465 725f 735a 0759 5f6e  erZ.X_der_sZ.Y_n
+000050e0: 756d 7079 da09 6772 6164 6965 6e74 7372  umpy..gradientsr
+000050f0: 8b00 0000 728c 0000 005a 0c67 7261 6469  ....r....Z.gradi
+00005100: 656e 7473 5f6e 70da 0962 6174 6368 5f69  ents_np..batch_i
+00005110: 6478 da04 6469 7374 72b7 0000 005a 0761  dx..distr....Z.a
+00005120: 6476 5f69 6478 da07 595f 636c 6173 7372  dv_idx..Y_classr
+00005130: c800 0000 72cf 0000 005a 0f61 626f 7665  ....r....Z.above
+00005140: 5f74 6872 6573 686f 6c64 72fa 0000 0072  _thresholdr....r
+00005150: 4000 0000 726c 0000 0072 4100 0000 da06  @...rl...rA.....
+00005160: 6174 7461 636b ff01 0000 73be 0100 0000  attack....s.....
+00005170: 2e14 0222 1808 010e 0114 010a 0118 010e  ..."............
+00005180: 0104 0304 0108 0212 0114 0210 0108 0102  ................
+00005190: 0108 0116 0108 0106 0122 0102 fe06 0412  ........."......
+000051a0: 010a 0114 0210 0104 0112 ff10 0308 010a  ................
+000051b0: 0104 0106 010e 010a 0104 011c 0110 0128  ...............(
+000051c0: 0208 0110 0114 010c 0112 020c 0306 040c  ................
+000051d0: 0112 0110 030c 011c 0118 0316 0310 030e  ................
+000051e0: 010e 010e 010e 010e 010e 030c 030c 010c  ................
+000051f0: 0106 020a 030a 0308 0108 0210 030a 010a  ................
+00005200: 0320 010e 010e 0110 020a 010a 020c ff04  . ..............
+00005210: 0106 ff04 030a 010a 010a 0204 010e ff04  ................
+00005220: 0302 fd02 ff02 0704 010e ff04 0302 fd02  ................
+00005230: ff02 071a 011a 010c 0108 010a 010a 013c  ...............<
+00005240: 020e 010a 0108 011e 0224 0114 0128 030a  .........$...(..
+00005250: 030a 030e 030a 010c 0108 0128 050a 0208  ...........(....
+00005260: 0108 020c 011a 0210 0114 0214 0102 0104  ................
+00005270: 0108 ff02 ff04 0502 010e ff04 0310 0102  ................
+00005280: 0104 0104 ff02 ff04 060a 0210 0102 0104  ................
+00005290: 010c ff02 ff04 0522 0208 0108 0108 0102  ......."........
+000052a0: 0104 010c ff02 ff04 0502 0104 0116 ff02  ................
+000052b0: ff04 050a 0502 0110 ff14 030e 010a 010a  ................
+000052c0: 030a 0114 010a 0204 040a ff04 0208 fe04  ................
+000052d0: 0302 fd04 0406 fc04 0608 0108 040a ff04  ................
+000052e0: 0208 fe04 0302 fd04 0406 fc04 060c 0108  ................
+000052f0: 0108 0108 0104 0106 0138 030e 0202 0116  .........8......
+00005300: ff02 ff04 040a fc04 0816 010e 020e 0102  ................
+00005310: fe0a 0602 010c ff08 030e 020e 0102 fe0a  ................
+00005320: 0418 0304 010e ff06 030e 010e 027a 1543  .............z.C
+00005330: 6f75 6e74 6572 6661 6374 7561 6c2e 6174  ounterfactual.at
+00005340: 7461 636b 6308 0000 0000 0000 0000 0000  tackc...........
+00005350: 0010 0000 0009 0000 0043 0000 0073 a401  .........C...s..
+00005360: 0000 7c01 6a00 6401 1900 6402 6b03 7220  ..|.j.d...d.k.r 
+00005370: 7401 a002 6403 7c01 6a00 6401 1900 a102  t...d.|.j.d.....
+00005380: 0100 7403 a004 7405 a101 7d08 7c00 a006  ..t...t...}.|...
+00005390: 7c01 a101 a007 a100 a008 a100 a009 a100  |...............
+000053a0: 7d09 740a a00b 7c09 6a00 a101 7d0a 740a  }.t...|.j...}.t.
+000053b0: 6a0c 7c09 6402 6404 8d02 7d0b 6402 7c0a  j.|.d.d...}.d.|.
+000053c0: 740a a00d 7c09 6a00 6401 1900 a101 7c0b  t...|.j.d.....|.
+000053d0: 6602 3c00 740e a00f 7c0a a101 a010 a100  f.<.t...|.......
+000053e0: a011 7c00 6a12 a101 7d02 7c09 7c08 6405  ..|.j...}.|.|.d.
+000053f0: 3c00 740a 6a0c 7c09 6402 6404 8d02 6401  <.t.j.|.d.d...d.
+00005400: 1900 7c08 6406 3c00 6407 7c00 5f13 7c00  ..|.d.<.d.|._.|.
+00005410: 6a14 7c01 7c02 7c03 7c04 7c05 7c06 7c07  j.|.|.|.|.|.|.|.
+00005420: 6408 8d07 5c02 7d0c 7d0d 7c00 6a15 72d8  d...\.}.}.|.j.r.
+00005430: 7c00 6a16 7c08 6409 3c00 7c00 6a13 9001  |.j.|.d.<.|.j...
+00005440: 730c 7c00 6a17 6401 6b04 72f4 7401 a002  s.|.j.d.k.r.t...
+00005450: 640a a101 0100 7418 7403 a004 7c00 6a19  d.....t.t...|.j.
+00005460: a101 7c08 640b 8d02 7d0e 7c0e 5300 7c00  ..|.d...}.|.S.|.
+00005470: 6a1a 7c08 640c 3c00 6900 7c08 640d 3c00  j.|.d.<.i.|.d.<.
+00005480: 7c0c 7c08 640d 1900 640e 3c00 7c00 a006  |.|.d...d.<.|...
+00005490: 740e a00f 7c0c a101 a011 7c00 6a12 a101  t...|.....|.j...
+000054a0: a101 a007 a100 a008 a100 a009 a100 7d0f  ..............}.
+000054b0: 7c0f 7c08 640d 1900 640f 3c00 740a 6a0c  |.|.d...d.<.t.j.
+000054c0: 7c0f 6402 6404 8d02 6401 1900 7c08 640d  |.d.d...d...|.d.
+000054d0: 1900 6410 3c00 7c0d a007 a100 a008 a100  ..d.<.|.........
+000054e0: a009 a100 7c08 640d 1900 6411 3c00 7418  ....|.d...d.<.t.
+000054f0: 7403 a004 7c00 6a19 a101 7c08 640b 8d02  t...|.j...|.d...
+00005500: 7d0e 7c0e 5300 2912 61bb 0600 000a 2020  }.|.S.).a.....  
+00005510: 2020 2020 2020 4578 706c 6169 6e20 696e        Explain in
+00005520: 7374 616e 6365 2061 6e64 2072 6574 7572  stance and retur
+00005530: 6e20 636f 756e 7465 7266 6163 7475 616c  n counterfactual
+00005540: 2077 6974 6820 6d65 7461 6461 7461 2e0a   with metadata..
+00005550: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00005560: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00005570: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2058  ------.        X
+00005580: 0a20 2020 2020 2020 2020 2020 2049 6e69  .            Ini
+00005590: 7469 616c 2070 6572 7475 7262 6174 696f  tial perturbatio
+000055a0: 6e0a 2020 2020 2020 2020 590a 2020 2020  n.        Y.    
+000055b0: 2020 2020 2020 2020 4c61 6265 6c73 2066          Labels f
+000055c0: 6f72 2060 5860 2061 7320 6f6e 652d 686f  or `X` as one-ho
+000055d0: 742d 656e 636f 6469 6e67 2e0a 2020 2020  t-encoding..    
+000055e0: 2020 2020 7461 7267 6574 5f63 6c61 7373      target_class
+000055f0: 0a20 2020 2020 2020 2020 2020 204c 6973  .            Lis
+00005600: 7420 7769 7468 2074 6172 6765 7420 636c  t with target cl
+00005610: 6173 7365 7320 7573 6564 2074 6f20 6669  asses used to fi
+00005620: 6e64 2063 6c6f 7365 7374 2070 726f 746f  nd closest proto
+00005630: 7479 7065 2e20 4966 2060 604e 6f6e 6560  type. If ``None`
+00005640: 602c 2074 6865 206e 6561 7265 7374 2070  `, the nearest p
+00005650: 726f 746f 7479 7065 0a20 2020 2020 2020  rototype.       
+00005660: 2020 2020 2065 7863 6570 7420 666f 7220       except for 
+00005670: 7468 6520 7072 6564 6963 7420 636c 6173  the predict clas
+00005680: 7320 6f6e 2074 6865 2069 6e73 7461 6e63  s on the instanc
+00005690: 6520 6973 2075 7365 642e 0a20 2020 2020  e is used..     
+000056a0: 2020 206b 0a20 2020 2020 2020 2020 2020     k.           
+000056b0: 204e 756d 6265 7220 6f66 206e 6561 7265   Number of neare
+000056c0: 7374 2069 6e73 7461 6e63 6573 2075 7365  st instances use
+000056d0: 6420 746f 2064 6566 696e 6520 7468 6520  d to define the 
+000056e0: 7072 6f74 6f74 7970 6520 666f 7220 6120  prototype for a 
+000056f0: 636c 6173 732e 2044 6566 6175 6c74 7320  class. Defaults 
+00005700: 746f 2075 7369 6e67 2061 6c6c 0a20 2020  to using all.   
+00005710: 2020 2020 2020 2020 2069 6e73 7461 6e63           instanc
+00005720: 6573 2062 656c 6f6e 6769 6e67 2074 6f20  es belonging to 
+00005730: 7468 6520 636c 6173 7320 6966 2061 6e20  the class if an 
+00005740: 656e 636f 6465 7220 6973 2075 7365 6420  encoder is used 
+00005750: 616e 6420 746f 2031 2066 6f72 206b 2d64  and to 1 for k-d
+00005760: 2074 7265 6573 2e0a 2020 2020 2020 2020   trees..        
+00005770: 6b5f 7479 7065 0a20 2020 2020 2020 2020  k_type.         
+00005780: 2020 2055 7365 2065 6974 6865 7220 7468     Use either th
+00005790: 6520 6176 6572 6167 6520 656e 636f 6469  e average encodi
+000057a0: 6e67 206f 6620 7468 6520 606b 6020 6e65  ng of the `k` ne
+000057b0: 6172 6573 7420 696e 7374 616e 6365 7320  arest instances 
+000057c0: 696e 2061 2063 6c61 7373 2028 6060 6b5f  in a class (``k_
+000057d0: 7479 7065 3d27 6d65 616e 2760 6029 206f  type='mean'``) o
+000057e0: 720a 2020 2020 2020 2020 2020 2020 7468  r.            th
+000057f0: 6520 6b2d 6e65 6172 6573 7420 656e 636f  e k-nearest enco
+00005800: 6469 6e67 2069 6e20 7468 6520 636c 6173  ding in the clas
+00005810: 7320 2860 606b 5f74 7970 653d 2770 6f69  s (``k_type='poi
+00005820: 6e74 2760 6029 2074 6f20 6465 6669 6e65  nt'``) to define
+00005830: 2074 6865 2070 726f 746f 7479 7065 206f   the prototype o
+00005840: 6620 7468 6174 2063 6c61 7373 2e0a 2020  f that class..  
+00005850: 2020 2020 2020 2020 2020 4f6e 6c79 2072            Only r
+00005860: 656c 6576 616e 7420 6966 2061 6e20 656e  elevant if an en
+00005870: 636f 6465 7220 6973 2075 7365 6420 746f  coder is used to
+00005880: 2064 6566 696e 6520 7468 6520 7072 6f74   define the prot
+00005890: 6f74 7970 6573 2e0a 2020 2020 2020 2020  otypes..        
+000058a0: 7468 7265 7368 6f6c 640a 2020 2020 2020  threshold.      
+000058b0: 2020 2020 2020 5468 7265 7368 6f6c 6420        Threshold 
+000058c0: 6c65 7665 6c20 666f 7220 7468 6520 7261  level for the ra
+000058d0: 7469 6f20 6265 7477 6565 6e20 7468 6520  tio between the 
+000058e0: 6469 7374 616e 6365 206f 6620 7468 6520  distance of the 
+000058f0: 636f 756e 7465 7266 6163 7475 616c 2074  counterfactual t
+00005900: 6f20 7468 6520 7072 6f74 6f74 7970 6520  o the prototype 
+00005910: 6f66 2074 6865 0a20 2020 2020 2020 2020  of the.         
+00005920: 2020 2070 7265 6469 6374 6564 2063 6c61     predicted cla
+00005930: 7373 2066 6f72 2074 6865 206f 7269 6769  ss for the origi
+00005940: 6e61 6c20 696e 7374 616e 6365 206f 7665  nal instance ove
+00005950: 7220 7468 6520 6469 7374 616e 6365 2074  r the distance t
+00005960: 6f20 7468 6520 7072 6f74 6f74 7970 6520  o the prototype 
+00005970: 6f66 2074 6865 2070 7265 6469 6374 6564  of the predicted
+00005980: 2063 6c61 7373 0a20 2020 2020 2020 2020   class.         
+00005990: 2020 2066 6f72 2074 6865 2063 6f75 6e74     for the count
+000059a0: 6572 6661 6374 7561 6c2e 2049 6620 7468  erfactual. If th
+000059b0: 6520 7472 7573 7420 7363 6f72 6520 6973  e trust score is
+000059c0: 2062 656c 6f77 2074 6865 2074 6872 6573   below the thres
+000059d0: 686f 6c64 2c20 7468 6520 7072 6f70 6f73  hold, the propos
+000059e0: 6564 2063 6f75 6e74 6572 6661 6374 7561  ed counterfactua
+000059f0: 6c20 646f 6573 0a20 2020 2020 2020 2020  l does.         
+00005a00: 2020 206e 6f74 206d 6565 7420 7468 6520     not meet the 
+00005a10: 7265 7175 6972 656d 656e 7473 2e0a 2020  requirements..  
+00005a20: 2020 2020 2020 7665 7262 6f73 6974 790a        verbosity.
+00005a30: 2020 2020 2020 2020 2020 2020 5072 696e              Prin
+00005a40: 7420 696e 7465 726d 6564 6961 7465 2072  t intermediate r
+00005a50: 6573 756c 7473 206f 6620 6f70 7469 6d69  esults of optimi
+00005a60: 7a61 7469 6f6e 2069 6620 6772 6561 7465  zation if greate
+00005a70: 7220 7468 616e 2031 2e0a 2020 2020 2020  r than 1..      
+00005a80: 2020 7072 696e 745f 6576 6572 790a 2020    print_every.  
+00005a90: 2020 2020 2020 2020 2020 5072 696e 7420            Print 
+00005aa0: 6672 6571 7565 6e63 7920 6966 2076 6572  frequency if ver
+00005ab0: 626f 7369 7479 2069 7320 6772 6561 7465  bosity is greate
+00005ac0: 7220 7468 616e 2031 2e0a 2020 2020 2020  r than 1..      
+00005ad0: 2020 6c6f 675f 6576 6572 790a 2020 2020    log_every.    
+00005ae0: 2020 2020 2020 2020 6074 656e 736f 7262          `tensorb
+00005af0: 6f61 7264 6020 6c6f 6720 6672 6571 7565  oard` log freque
+00005b00: 6e63 7920 6966 2077 7269 7465 2064 6972  ncy if write dir
+00005b10: 6563 746f 7279 2069 7320 7370 6563 6966  ectory is specif
+00005b20: 6965 640a 0a20 2020 2020 2020 2052 6574  ied..        Ret
+00005b30: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00005b40: 2d2d 2d2d 0a20 2020 2020 2020 2065 7870  ----.        exp
+00005b50: 6c61 6e61 7469 6f6e 0a20 2020 2020 2020  lanation.       
+00005b60: 2020 2020 2060 4578 706c 616e 6174 696f       `Explanatio
+00005b70: 6e60 206f 626a 6563 7420 636f 6e74 6169  n` object contai
+00005b80: 6e69 6e67 2074 6865 2063 6f75 6e74 6572  ning the counter
+00005b90: 6661 6374 7561 6c20 7769 7468 2061 6464  factual with add
+00005ba0: 6974 696f 6e61 6c20 6d65 7461 6461 7461  itional metadata
+00005bb0: 2061 7320 6174 7472 6962 7574 6573 2e0a   as attributes..
+00005bc0: 2020 2020 2020 2020 7201 0000 0072 1900          r....r..
+00005bd0: 0000 7a59 4375 7272 656e 746c 7920 6f6e  ..zYCurrently on
+00005be0: 6c79 2073 696e 676c 6520 696e 7374 616e  ly single instan
+00005bf0: 6365 2065 7870 6c61 6e61 7469 6f6e 7320  ce explanations 
+00005c00: 7375 7070 6f72 7465 6420 2866 6972 7374  supported (first
+00005c10: 2064 696d 203d 2031 292c 2062 7574 2066   dim = 1), but f
+00005c20: 6972 7374 2064 696d 203d 2025 7372 a700  irst dim = %sr..
+00005c30: 0000 5a0a 6f72 6967 5f70 726f 6261 72c9  ..Z.orig_probar.
+00005c40: 0000 0046 2906 7297 0000 0072 d100 0000  ...F).r....r....
+00005c50: 72cb 0000 0072 d200 0000 72d3 0000 0072  r....r....r....r
+00005c60: d400 0000 72e7 0000 007a 184e 6f20 636f  ....r....z.No co
+00005c70: 756e 7465 7266 6163 7475 616c 2066 6f75  unterfactual fou
+00005c80: 6e64 2129 0272 3100 0000 7270 0000 00da  nd!).r1...rp....
+00005c90: 0361 6c6c da02 6366 72b5 0000 0072 b700  .all..cfr....r..
+00005ca0: 0000 da05 636c 6173 7372 c500 0000 291b  ....classr....).
+00005cb0: 721c 0000 0072 5000 0000 7251 0000 0072  r....rP...rQ...r
+00005cc0: 4500 0000 7246 0000 0072 0700 0000 721a  E...rF...r....r.
+00005cd0: 0000 0072 c000 0000 7236 0000 0072 c100  ...r....r6...r..
+00005ce0: 0000 724d 0000 0072 4b00 0000 72da 0000  ..rM...rK...r...
+00005cf0: 00da 0661 7261 6e67 6572 3b00 0000 72f2  ...aranger;...r.
+00005d00: 0000 0072 6f00 0000 72e8 0000 0072 2f00  ...ro...r....r/.
+00005d10: 0000 72fa 0000 0072 0201 0000 7238 0000  ..r....r....r8..
+00005d20: 0072 e700 0000 722d 0000 0072 0a00 0000  .r....r-...r....
+00005d30: 7231 0000 0072 e900 0000 2910 7232 0000  r1...r....).r2..
+00005d40: 0072 b500 0000 7297 0000 0072 d100 0000  .r....r....r....
+00005d50: 72cb 0000 0072 d200 0000 72d3 0000 0072  r....r....r....r
+00005d60: d400 0000 7270 0000 005a 0759 5f70 726f  ....rp...Z.Y_pro
+00005d70: 6261 5a05 595f 6f68 6572 0101 0000 72fa  baZ.Y_oher....r.
+00005d80: 0000 0072 c500 0000 da0b 6578 706c 616e  ...r......explan
+00005d90: 6174 696f 6e5a 0659 5f70 6572 7472 4000  ationZ.Y_pertr@.
+00005da0: 0000 7240 0000 0072 4100 0000 da07 6578  ..r@...rA.....ex
+00005db0: 706c 6169 6e6f 0300 0073 5000 0000 002f  plaino...sP..../
+00005dc0: 0e01 0401 0202 08fd 0407 0a03 1601 0c01  ................
+00005dd0: 0e01 1801 1602 0801 1603 0601 0401 0201  ................
+00005de0: 0201 0201 0201 0201 0201 02f9 0a0b 0601  ................
+00005df0: 0a03 0801 0a01 0a03 1401 0402 0a01 0801  ................
+00005e00: 0c02 22ff 0206 0c01 1a01 1803 1402 7a16  .."...........z.
+00005e10: 436f 756e 7465 7266 6163 7475 616c 2e65  Counterfactual.e
+00005e20: 7870 6c61 696e 2913 720e 0000 0072 0f00  xplain).r....r..
+00005e30: 0000 7210 0000 0072 0e00 0000 4e4e 720e  ..r....r....NNr.
+00005e40: 0000 0046 7212 0000 0072 1300 0000 7214  ...Fr....r....r.
+00005e50: 0000 0072 1500 0000 7216 0000 0072 1800  ...r....r....r..
+00005e60: 0000 7219 0000 004e 7201 0000 0054 4e29  ..r....Nr....TN)
+00005e70: 0172 c700 0000 2905 4e4e 72ad 0000 0072  .r....).NNr....r
+00005e80: 0e00 0000 72d0 0000 0029 064e 4e4e 72ad  ....r....).NNNr.
+00005e90: 0000 0072 0e00 0000 72d0 0000 0029 27da  ...r....r....)'.
+00005ea0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00005eb0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00005ec0: 655f 5f72 0500 0000 7202 0000 0072 4d00  e__r....r....rM.
+00005ed0: 0000 72df 0000 0072 3b00 0000 724e 0000  ..r....r;...rN..
+00005ee0: 0072 4f00 0000 7256 0000 0072 3a00 0000  .rO...rV...r:...
+00005ef0: 7204 0000 0072 0300 0000 72e0 0000 0072  r....r....r....r
+00005f00: d700 0000 da03 7374 7272 4400 0000 7266  ......strrD...rf
+00005f10: 0000 0072 6d00 0000 7271 0000 0072 7400  ...rm...rq...rt.
+00005f20: 0000 727f 0000 0072 8300 0000 728f 0000  ..r....r....r...
+00005f30: 0072 9300 0000 7296 0000 00da 0654 656e  .r....r......Ten
+00005f40: 736f 7272 8700 0000 72a4 0000 00da 0561  sorr....r......a
+00005f50: 7272 6179 72b4 0000 0072 c600 0000 72cf  rrayr....r....r.
+00005f60: 0000 0072 e100 0000 7202 0100 0072 0a00  ...r....r....r..
+00005f70: 0000 7208 0100 00da 0d5f 5f63 6c61 7373  ..r......__class
+00005f80: 6365 6c6c 5f5f 7240 0000 0072 4000 0000  cell__r@...r@...
+00005f90: 725d 0000 0072 4100 0000 720d 0000 0010  r]...rA...r.....
+00005fa0: 0000 0073 d000 0000 0806 0001 0001 0004  ...s............
+00005fb0: 0001 0001 0001 0001 0001 0001 0001 0001  ................
+00005fc0: 0001 0001 0001 0001 0001 0001 0001 00e6  ................
+00005fd0: 0202 1c01 1c01 0201 0201 0201 1e04 0201  ................
+00005fe0: 0a01 0a01 0201 0201 0201 0201 0201 0201  ................
+00005ff0: 0201 0201 0201 0601 0201 0201 0201 02e5  ................
+00006000: 107f 002c 080f 080a 0805 0805 0815 080d  ...,............
+00006010: 0824 0812 0813 181b 080a 0801 08fd 0202  .$..............
+00006020: 0401 0401 02fc 0c2a 0a01 04fe 0c45 00ff  .......*.....E..
+00006030: 0201 0a01 02fe 0c29 0001 0001 0001 0001  .......)........
+00006040: 00f8 0202 0401 0401 0601 0601 0201 0201  ................
+00006050: 0201 18f7 0c7f 007f 0076 0001 0001 0001  .........v......
+00006060: 0001 0001 00f7 0203 0401 0801 0601 0601  ................
+00006070: 0201 0201 0201 02f6 720d 0000 0063 0100  ........r....c..
+00006080: 0000 0000 0000 0000 0000 0200 0000 0800  ................
+00006090: 0000 4300 0000 7338 0000 0074 007c 0064  ..C...s8...t.|.d
+000060a0: 0183 028f 1a7d 0174 01a0 027c 01a1 0157  .....}.t...|...W
+000060b0: 0002 0064 0004 0004 0083 0301 0053 0031  ...d.........S.1
+000060c0: 0073 2a30 0001 0001 0001 0059 0001 0064  .s*0.......Y...d
+000060d0: 0053 0029 024e da02 7262 2903 da04 6f70  .S.).N..rb)...op
+000060e0: 656e da06 7069 636b 6c65 da04 6c6f 6164  en..pickle..load
+000060f0: 2902 da08 6669 6c65 6e61 6d65 da04 6f75  )...filename..ou
+00006100: 7470 7240 0000 0072 4000 0000 7241 0000  tpr@...r@...rA..
+00006110: 0072 ae00 0000 de03 0000 7304 0000 0000  .r........s.....
+00006120: 010c 0172 ae00 0000 6301 0000 0000 0000  ...r....c.......
+00006130: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
+00006140: 0073 5400 0000 7400 7c00 7401 6a02 8302  .sT...t.|.t.j...
+00006150: 7250 7c00 a003 a100 6401 6b02 7250 7c00  rP|.....d.k.rP|.
+00006160: 6a04 7401 6a05 7401 6a06 7401 6a07 7401  j.t.j.t.j.t.j.t.
+00006170: 6a08 6604 7600 7236 6402 5300 7c00 6a04  j.f.v.r6d.S.|.j.
+00006180: 7401 6a09 7401 6a0a 7401 6a0b 6603 7600  t.j.t.j.t.j.f.v.
+00006190: 7250 6402 5300 6403 5300 2904 4e72 1900  rPd.S.d.S.).Nr..
+000061a0: 0000 5446 290c 7239 0000 0072 3b00 0000  ..TF).r9...r;...
+000061b0: 720d 0100 00da 056e 756d 656c da05 6474  r......numel..dt
+000061c0: 7970 65da 0569 6e74 3332 72d8 0000 00da  ype..int32r.....
+000061d0: 0569 6e74 3136 da04 696e 7438 da07 666c  .int16..int8..fl
+000061e0: 6f61 7433 32da 0766 6c6f 6174 3634 da07  oat32..float64..
+000061f0: 666c 6f61 7431 3629 0172 d500 0000 7240  float16).r....r@
+00006200: 0000 0072 4000 0000 7241 0000 0072 d900  ...r@...rA...r..
+00006210: 0000 e303 0000 730c 0000 0000 0218 021a  ......s.........
+00006220: 0104 0216 0104 0272 d900 0000 6306 0000  .......r....c...
+00006230: 0000 0000 0000 0000 0006 0000 0004 0000  ................
+00006240: 0043 0000 0073 1800 0000 7400 7c01 6a01  .C...s....t.|.j.
+00006250: 9b00 6401 7c00 9b00 9d03 8301 0100 6400  ..d.|.........d.
+00006260: 5300 2902 4e7a 023a 2029 0272 e200 0000  S.).Nz.: ).r....
+00006270: 7209 0100 0029 06da 076d 6573 7361 6765  r....)...message
+00006280: da08 6361 7465 676f 7279 7214 0100 00da  ..categoryr.....
+00006290: 066c 696e 656e 6fda 0466 696c 65da 046c  .lineno..file..l
+000062a0: 696e 6572 4000 0000 7240 0000 0072 4100  iner@...r@...rA.
+000062b0: 0000 7259 0000 00f1 0300 0073 0200 0000  ..rY.......s....
+000062c0: 0001 7259 0000 0029 024e 4e29 1c72 4500  ..rY...).NN).rE.
+000062d0: 0000 72f4 0000 00da 075f 7069 636b 6c65  ..r......_pickle
+000062e0: 7212 0100 00da 0674 7970 696e 6772 0200  r......typingr..
+000062f0: 0000 7203 0000 0072 0400 0000 7205 0000  ..r....r....r...
+00006300: 0072 c100 0000 724d 0000 0072 5000 0000  .r....rM...rP...
+00006310: 723b 0000 005a 0b74 6f72 6368 2e6f 7074  r;...Z.torch.opt
+00006320: 696d 729f 0000 005a 0c61 7069 2e64 6566  imr....Z.api.def
+00006330: 6175 6c74 7372 0700 0000 7208 0000 005a  aultsr....r....Z
+00006340: 0e61 7069 2e69 6e74 6572 6661 6365 7372  .api.interfacesr
+00006350: 0900 0000 720a 0000 0072 0b00 0000 5a0f  ....r....r....Z.
+00006360: 7574 696c 732e 6772 6164 6965 6e74 7372  utils.gradientsr
+00006370: 0c00 0000 720d 0000 0072 ae00 0000 72d9  ....r....r....r.
+00006380: 0000 0072 5900 0000 7240 0000 0072 4000  ...rY...r@...r@.
+00006390: 0000 7240 0000 0072 4100 0000 da08 3c6d  ..r@...rA.....<m
+000063a0: 6f64 756c 653e 0100 0000 732a 0000 0008  odule>....s*....
+000063b0: 0108 0108 0118 0108 0108 0208 010c 0210  ................
+000063c0: 0114 010c 0312 7f00 7f00 7f00 7f00 7f00  ................
+000063d0: 7f00 7f00 5508 0508 0e                   ....U....
```

### Comparing `morpheus_spatial-0.4.0/src/morpheus/counterfactual/__pycache__/generate.cpython-39.pyc` & `morpheus_spatial-0.5.0/src/morpheus/counterfactual/__pycache__/generate.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr  5 23:40:35 2024 UTC, .py size: 12218 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,652 +1,685 @@
-00000000: 610d 0d0a 0000 0000 f38b 1066 ba2f 0000  a..........f./..
+00000000: 610d 0d0a 0000 0000 4dc3 2166 9538 0000  a.......M.!f.8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0011 0000 0040 0000 0073 5a01 0000 6400  .....@...sZ...d.
+00000020: 0012 0000 0040 0000 0073 8001 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c06 5a07 6400 6402 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
-00000060: 0100 6400 6401 6c0a 5a0a 6400 6403 6c0b  ..d.d.l.Z.d.d.l.
-00000070: 6d0b 5a0b 0100 6404 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
-00000080: 0100 6406 6407 6c0e 6d0f 5a0f 0100 6404  ..d.d.l.m.Z...d.
-00000090: 6408 6c10 6d11 5a11 0100 6404 6409 6c12  d.l.m.Z...d.d.l.
-000000a0: 6d13 5a13 6d14 5a14 6d15 5a15 6d16 5a16  m.Z.m.Z.m.Z.m.Z.
-000000b0: 0100 650a 6a17 640a 650a 6a18 640b 8d02  ..e.j.d.e.j.d...
-000000c0: 5a19 6422 650d 651a 650a 6a1b 6a1c 651d  Z.d"e.e.e.j.j.e.
-000000d0: 651e 6507 6a1f 6520 6521 6521 651a 6521  e.e.j.e e!e!e.e!
-000000e0: 6522 6509 651e 1900 640e 9c0d 640f 6410  e"e.e...d...d.d.
-000000f0: 8405 5a23 6423 6505 6a24 6505 6a24 651a  ..Z#d#e.j$e.j$e.
-00000100: 650a 6a1b 6a1c 651d 651d 6505 6a24 6505  e.j.j.e.e.e.j$e.
-00000110: 6a24 6521 6522 651e 6521 651a 6520 6401  j$e!e"e.e!e.e d.
-00000120: 6411 9c0f 6412 6413 8405 5a25 6424 6521  d...d.d...Z%d$e!
-00000130: 650a 6a1b 6a1c 651d 651d 6509 651e 1900  e.j.j.e.e.e.e...
-00000140: 6414 9c05 6415 6416 8405 5a26 6417 6418  d...d.d...Z&d.d.
-00000150: 8400 5a27 6419 641a 8400 5a28 641b 641c  ..Z'd.d...Z(d.d.
-00000160: 8400 5a29 6425 650a 6a2a 652b 650a 6a2a  ..Z)d%e.j*e+e.j*
-00000170: 641d 9c03 641e 641f 8405 5a2c 6420 6421  d...d.d...Z,d d!
-00000180: 8400 5a2d 6401 5300 2926 e900 0000 004e  ..Z-d.S.)&.....N
-00000190: 2901 da08 4f70 7469 6f6e 616c 2901 da04  )...Optional)...
-000001a0: 7471 646d e902 0000 0029 01da 0e53 7061  tqdm.....)...Spa
-000001b0: 7469 616c 4461 7461 7365 74e9 0100 0000  tialDataset.....
-000001c0: 2901 da0e 436f 756e 7465 7266 6163 7475  )...Counterfactu
-000001d0: 616c 2901 da0a 5472 7573 7453 636f 7265  al)...TrustScore
-000001e0: 2904 da06 5370 6c69 7473 da07 436f 6c4e  )...Splits..ColN
-000001f0: 616d 65da 1144 6566 6175 6c74 466f 6c64  ame..DefaultFold
-00000200: 6572 4e61 6d65 da0f 4465 6661 756c 7446  erName..DefaultF
-00000210: 696c 654e 616d 6567 2342 920c a19c c73b  ileNameg#B.....;
-00000220: a901 da05 6474 7970 65e7 0000 0000 0000  ....dtype.......
-00000230: e03f 4629 0dda 0764 6174 6173 6574 da0c  .?F)...dataset..
-00000240: 7461 7267 6574 5f63 6c61 7373 da05 6d6f  target_class..mo
-00000250: 6465 6cda 1263 6861 6e6e 656c 5f74 6f5f  del..channel_to_
-00000260: 7065 7274 7572 62da 136f 7074 696d 697a  perturb..optimiz
-00000270: 6174 696f 6e5f 7061 7261 6d73 da06 696d  ation_params..im
-00000280: 6167 6573 da09 7468 7265 7368 6f6c 64da  ages..threshold.
-00000290: 0b6b 6474 7265 655f 7061 7468 da08 7361  .kdtree_path..sa
-000002a0: 7665 5f64 6972 da0b 6e75 6d5f 776f 726b  ve_dir..num_work
-000002b0: 6572 73da 0a74 7261 696e 5f64 6174 61da  ers..train_data.
-000002c0: 0776 6572 626f 7365 da11 7472 7573 7473  .verbose..trusts
-000002d0: 636f 7265 5f6b 7761 7267 7363 0d00 0000  core_kwargsc....
-000002e0: 0000 0000 0000 0000 1e00 0000 1100 0000  ................
-000002f0: 0300 0000 7302 0200 0074 007c 0583 017d  ....s....t.|...}
-00000300: 0d74 0174 026a 03a0 047c 006a 0564 01a1  .t.t.j...|.j.d..
-00000310: 0283 018f 2a7d 0e74 06a0 077c 0ea1 017d  ....*}.t...|...}
-00000320: 0f7c 0f64 0219 007d 107c 0f64 0319 007d  .|.d...}.|.d...}
-00000330: 1157 0064 0404 0004 0083 0301 006e 1031  .W.d.........n.1
-00000340: 0073 4c30 0001 0001 0001 0059 0001 007c  .sL0.......Y...|
-00000350: 0a64 0475 0072 7274 026a 03a0 047c 006a  .d.u.rrt.j...|.j
-00000360: 0574 086a 096a 0aa1 027d 0a7c 0764 0475  .t.j.j...}.|.d.u
-00000370: 0072 8e74 026a 03a0 047c 006a 0b74 0c6a  .r.t.j...|.j.t.j
-00000380: 0d6a 0aa1 027d 077c 0564 0475 0072 9c7c  .j...}.|.d.u.r.|
-00000390: 006a 0e7d 057c 0864 0475 0072 b874 026a  .j.}.|.d.u.r.t.j
-000003a0: 03a0 047c 006a 0b74 0f6a 106a 0aa1 027d  ...|.j.t.j.j...}
-000003b0: 0874 026a 117c 0864 0564 068d 0201 007c  .t.j.|.d.d.....|
-000003c0: 087c 005f 1274 026a 03a0 137c 07a1 0173  .|._.t.j...|...s
-000003d0: f274 147c 077c 0a7c 027c 107c 117c 0c83  .t.|.|.|.|.|.|..
-000003e0: 0601 0074 1564 0783 0101 0067 007d 1274  ...t.d.....g.}.t
-000003f0: 167c 0d83 0144 005d 847d 137c 006a 177c  .|...D.].}.|.j.|
-00000400: 056a 187c 1319 0074 196a 1a6a 0a19 007c  .j.|...t.j.j...|
-00000410: 056a 187c 1319 007c 006a 1b19 007c 056a  .j.|...|.j...|.j
-00000420: 187c 1319 0074 196a 1c6a 0a19 0064 088d  .|...t.j.j...d..
-00000430: 037d 1474 1da0 1e7c 14a1 015c 027d 157d  .}.t...|...\.}.}
-00000440: 167c 006a 0e6a 187c 1619 007c 006a 1b19  .|.j.j.|...|.j..
-00000450: 007d 177c 12a0 1f7c 157c 177c 017c 027c  .}.|...|.|.|.|.|
-00000460: 006a 207c 037c 107c 117c 077c 0b7c 047c  .j |.|.|.|.|.|.|
-00000470: 087c 167c 0666 0ea1 0101 0071 fe7c 0964  .|.|.f.....q.|.d
-00000480: 096b 0490 0172 9264 056e 0264 0a7d 187c  .k...r.d.n.d.}.|
-00000490: 1890 0172 e264 0b64 0c6c 216d 227d 1901  ...r.d.d.l!m"}..
-000004a0: 0064 0b64 046c 237d 1a7c 1964 0d64 0e84  .d.d.l#}.|.d.d..
-000004b0: 0083 0189 0087 0066 0164 0f64 1084 087c  .......f.d.d...|
-000004c0: 1244 0083 017d 1b7c 1a6a 247c 1b64 117c  .D...}.|.j$|.d.|
-000004d0: 0964 129c 028e 017d 1c6e 1c74 257c 127c  .d.....}.n.t%|.|
-000004e0: 0d64 138d 0244 005d 0e7d 1d74 267c 1d8e  .d...D.].}.t&|..
-000004f0: 0001 0090 0171 ee64 0453 0029 1461 da03  .....q.d.S.).a..
-00000500: 0000 0a20 2020 2047 656e 6572 6174 6520  ...    Generate 
-00000510: 636f 756e 7465 7266 6163 7475 616c 7320  counterfactuals 
-00000520: 666f 7220 7468 6520 6461 7461 7365 742e  for the dataset.
-00000530: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00000540: 2020 2020 6461 7461 7365 7420 2853 7061      dataset (Spa
-00000550: 7469 616c 4461 7461 7365 7429 3a20 4461  tialDataset): Da
-00000560: 7461 7365 7420 746f 2067 656e 6572 6174  taset to generat
-00000570: 6520 636f 756e 7465 7266 6163 7475 616c  e counterfactual
-00000580: 7320 666f 722e 0a20 2020 2020 2020 2074  s for..        t
-00000590: 6172 6765 745f 636c 6173 7320 2869 6e74  arget_class (int
-000005a0: 293a 2054 6172 6765 7420 636c 6173 7320  ): Target class 
-000005b0: 666f 7220 7468 6520 636f 756e 7465 7266  for the counterf
-000005c0: 6163 7475 616c 732e 0a20 2020 2020 2020  actuals..       
-000005d0: 206d 6f64 656c 2028 746f 7263 682e 6e6e   model (torch.nn
-000005e0: 2e4d 6f64 756c 6529 3a20 4d6f 6465 6c20  .Module): Model 
-000005f0: 746f 2067 656e 6572 6174 6520 636f 756e  to generate coun
-00000600: 7465 7266 6163 7475 616c 7320 666f 722e  terfactuals for.
-00000610: 0a20 2020 2020 2020 2063 6861 6e6e 656c  .        channel
-00000620: 5f74 6f5f 7065 7274 7572 6220 286c 6973  _to_perturb (lis
-00000630: 7429 3a20 4c69 7374 206f 6620 6368 616e  t): List of chan
-00000640: 6e65 6c73 2074 6f20 7065 7274 7572 622e  nels to perturb.
-00000650: 0a20 2020 2020 2020 206f 7074 696d 697a  .        optimiz
-00000660: 6174 696f 6e5f 7061 7261 6d73 2028 6469  ation_params (di
-00000670: 6374 293a 2044 6963 7469 6f6e 6172 7920  ct): Dictionary 
-00000680: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
-00000690: 6172 616d 6574 6572 7320 666f 7220 7468  arameters for th
-000006a0: 6520 6f70 7469 6d69 7a61 7469 6f6e 2e0a  e optimization..
-000006b0: 2020 2020 2020 2020 696d 6167 6573 2028          images (
-000006c0: 7064 2e44 6174 6146 7261 6d65 2c20 6f70  pd.DataFrame, op
-000006d0: 7469 6f6e 616c 293a 2049 6d61 6765 7320  tional): Images 
-000006e0: 746f 2067 656e 6572 6174 6520 636f 756e  to generate coun
-000006f0: 7465 7266 6163 7475 616c 7320 666f 722e  terfactuals for.
-00000700: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-00000710: 652e 0a20 2020 2020 2020 2074 6872 6573  e..        thres
-00000720: 686f 6c64 2028 666c 6f61 742c 206f 7074  hold (float, opt
-00000730: 696f 6e61 6c29 3a20 5468 7265 7368 6f6c  ional): Threshol
-00000740: 6420 666f 7220 7468 6520 7072 6564 6963  d for the predic
-00000750: 7469 6f6e 2070 726f 6261 6269 6c69 7479  tion probability
-00000760: 2e20 4465 6661 756c 7473 2074 6f20 302e  . Defaults to 0.
-00000770: 352e 0a20 2020 2020 2020 206b 6474 7265  5..        kdtre
-00000780: 655f 7061 7468 2028 7374 722c 206f 7074  e_path (str, opt
-00000790: 696f 6e61 6c29 3a20 5061 7468 2074 6f20  ional): Path to 
-000007a0: 7468 6520 6b64 7472 6565 2066 696c 652e  the kdtree file.
-000007b0: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-000007c0: 652e 0a20 2020 2020 2020 2073 6176 655f  e..        save_
-000007d0: 6469 7220 2873 7472 2c20 6f70 7469 6f6e  dir (str, option
-000007e0: 616c 293a 2044 6972 6563 746f 7279 2077  al): Directory w
-000007f0: 6865 7265 206f 7574 7075 7420 7769 6c6c  here output will
-00000800: 2062 6520 7361 7665 642e 2044 6566 6175   be saved. Defau
-00000810: 6c74 7320 746f 204e 6f6e 652e 0a20 2020  lts to None..   
-00000820: 2020 2020 206e 756d 5f77 6f72 6b65 7273       num_workers
-00000830: 2028 626f 6f6c 2c20 6f70 7469 6f6e 616c   (bool, optional
-00000840: 293a 204e 756d 6265 7220 6f66 2077 6f72  ): Number of wor
-00000850: 6b65 7273 2074 6f20 7573 6520 666f 7220  kers to use for 
-00000860: 7061 7261 6c6c 656c 2070 726f 6365 7373  parallel process
-00000870: 696e 672e 2044 6566 6175 6c74 7320 746f  ing. Defaults to
-00000880: 204e 6f6e 652e 0a20 2020 2020 2020 2074   None..        t
-00000890: 7261 696e 5f64 6174 6120 2873 7472 2c20  rain_data (str, 
-000008a0: 6f70 7469 6f6e 616c 293a 2050 6174 6820  optional): Path 
-000008b0: 746f 2074 6865 2074 7261 696e 696e 6720  to the training 
-000008c0: 6461 7461 2e20 4465 6661 756c 7473 2074  data. Defaults t
-000008d0: 6f20 4e6f 6e65 2e0a 2020 2020 7a19 6e6f  o None..    z.no
-000008e0: 726d 616c 697a 6174 696f 6e5f 7061 7261  rmalization_para
-000008f0: 6d73 2e6a 736f 6eda 046d 6561 6eda 0573  ms.json..mean..s
-00000900: 7464 6576 4e54 a901 da08 6578 6973 745f  tdevNT....exist_
-00000910: 6f6b 7a0c 6b64 7472 6565 2073 6176 6564  okz.kdtree saved
-00000920: 2903 da08 7061 7463 685f 6964 da05 6c61  )...patch_id..la
-00000930: 6265 6cda 0573 706c 6974 7206 0000 0046  bel..splitr....F
-00000940: 7201 0000 0029 01da 0764 656c 6179 6564  r....)...delayed
-00000950: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000960: 0002 0000 0053 0000 0073 0800 0000 7400  .....S...s....t.
-00000970: 7c00 8e00 5300 a901 4e29 01da 0f67 656e  |...S...N)...gen
-00000980: 6572 6174 655f 6f6e 655f 6366 2901 da04  erate_one_cf)...
-00000990: 6172 6773 a900 7228 0000 00fa 562f 6365  args..r(....V/ce
-000009a0: 6e74 7261 6c2f 686f 6d65 2f7a 7761 6e67  ntral/home/zwang
-000009b0: 322f 6d6f 7270 6865 7573 2d73 7061 7469  2/morpheus-spati
-000009c0: 616c 2f6d 6f72 7068 6575 732f 7372 632f  al/morpheus/src/
-000009d0: 6d6f 7270 6865 7573 2f63 6f75 6e74 6572  morpheus/counter
-000009e0: 6661 6374 7561 6c2f 6765 6e65 7261 7465  factual/generate
-000009f0: 2e70 79da 1767 656e 6572 6174 655f 6f6e  .py..generate_on
-00000a00: 655f 6366 5f64 656c 6179 6564 7c00 0000  e_cf_delayed|...
-00000a10: 7302 0000 0000 027a 3367 6574 5f63 6f75  s......z3get_cou
-00000a20: 6e74 6572 6661 6374 7561 6c2e 3c6c 6f63  nterfactual.<loc
-00000a30: 616c 733e 2e67 656e 6572 6174 655f 6f6e  als>.generate_on
-00000a40: 655f 6366 5f64 656c 6179 6564 6301 0000  e_cf_delayedc...
-00000a50: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000a60: 0013 0000 0073 1400 0000 6700 7c00 5d0c  .....s....g.|.].
-00000a70: 7d01 8800 7c01 8301 9102 7104 5300 7228  }...|.....q.S.r(
-00000a80: 0000 0072 2800 0000 2902 da02 2e30 7227  ...r(...)....0r'
-00000a90: 0000 00a9 0172 2a00 0000 7228 0000 0072  .....r*...r(...r
-00000aa0: 2900 0000 da0a 3c6c 6973 7463 6f6d 703e  ).....<listcomp>
-00000ab0: 8000 0000 f300 0000 007a 2667 6574 5f63  .........z&get_c
-00000ac0: 6f75 6e74 6572 6661 6374 7561 6c2e 3c6c  ounterfactual.<l
-00000ad0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00000ae0: 3eda 0970 726f 6365 7373 6573 2902 da09  >..processes)...
-00000af0: 7363 6865 6475 6c65 7272 1900 0000 2901  schedulerr....).
-00000b00: da05 746f 7461 6c29 27da 036c 656e da04  ..total)'..len..
-00000b10: 6f70 656e da02 6f73 da04 7061 7468 da04  open..os..path..
-00000b20: 6a6f 696e da09 7370 6c69 745f 6469 72da  join..split_dir.
-00000b30: 046a 736f 6eda 046c 6f61 6472 0900 0000  .json..loadr....
-00000b40: da05 7472 6169 6eda 0576 616c 7565 da08  ..train..value..
-00000b50: 726f 6f74 5f64 6972 720c 0000 00da 066b  root_dirr......k
-00000b60: 6474 7265 65da 086d 6574 6164 6174 6172  dtree..metadatar
-00000b70: 0b00 0000 da0e 636f 756e 7465 7266 6163  ......counterfac
-00000b80: 7475 616c da08 6d61 6b65 6469 7273 da06  tual..makedirs..
-00000b90: 6366 5f64 6972 da06 6578 6973 7473 da0c  cf_dir..exists..
-00000ba0: 6275 696c 645f 6b64 7472 6565 da05 7072  build_kdtree..pr
-00000bb0: 696e 74da 0572 616e 6765 da13 6765 6e65  int..range..gene
-00000bc0: 7261 7465 5f70 6174 6368 5f70 6174 68da  rate_patch_path.
-00000bd0: 0469 6c6f 6372 0a00 0000 7221 0000 00da  .ilocr....r!....
-00000be0: 0a6c 6162 656c 5f6e 616d 65da 0673 706c  .label_name..spl
-00000bf0: 6974 7372 0500 0000 da11 6c6f 6164 5f73  itsr......load_s
-00000c00: 696e 676c 655f 696d 6167 65da 0661 7070  ingle_image..app
-00000c10: 656e 64da 0d63 6861 6e6e 656c 5f6e 616d  end..channel_nam
-00000c20: 6573 da04 6461 736b 7224 0000 005a 1464  es..daskr$...Z.d
-00000c30: 6173 6b2e 6d75 6c74 6970 726f 6365 7373  ask.multiprocess
-00000c40: 696e 67da 0763 6f6d 7075 7465 7203 0000  ing..computer...
-00000c50: 0072 2600 0000 291e 7210 0000 0072 1100  .r&...).r....r..
-00000c60: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00000c70: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000c80: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00000c90: 1b00 0000 721c 0000 00da 0a6e 756d 5f69  ....r......num_i
-00000ca0: 6d61 6765 735a 096a 736f 6e5f 6669 6c65  magesZ.json_file
-00000cb0: da14 6e6f 726d 616c 697a 6174 696f 6e5f  ..normalization_
-00000cc0: 7061 7261 6d73 da02 6d75 721e 0000 005a  params..mur....Z
-00000cd0: 1467 656e 6572 6174 655f 6f6e 655f 6366  .generate_one_cf
-00000ce0: 5f61 7267 73da 0169 da08 696d 675f 7061  _args..i..img_pa
-00000cf0: 7468 da03 696d 6772 2100 0000 7222 0000  th..imgr!...r"..
-00000d00: 00da 0870 6172 616c 6c65 6c72 2400 0000  ...parallelr$...
-00000d10: 724d 0000 005a 0a64 6173 6b5f 7461 736b  rM...Z.dask_task
-00000d20: 73da 015f 7227 0000 0072 2800 0000 722c  s.._r'...r(...r,
-00000d30: 0000 0072 2900 0000 da12 6765 745f 636f  ...r).....get_co
-00000d40: 756e 7465 7266 6163 7475 616c 1b00 0000  unterfactual....
-00000d50: 7376 0000 0000 1f08 0302 010e ff04 0202  sv..............
-00000d60: 010a 0108 0126 0308 0114 0108 0114 0108  .....&..........
-00000d70: 0106 0308 0106 010a ff04 030e 0106 030c  ................
-00000d80: 0112 0108 0304 010c 0104 0110 010e 0110  ................
-00000d90: fd06 050e 0112 0104 0202 0102 0102 0102  ................
-00000da0: 0104 0102 0102 0102 0102 0102 0102 0102  ................
-00000db0: 0102 0102 f202 ff06 1412 0106 010c 0108  ................
-00000dc0: 0202 010a 0312 0114 0210 0172 5700 0000  ...........rW...
-00000dd0: 290f da0e 6f72 6967 696e 616c 5f70 6174  )...original_pat
-00000de0: 6368 da0e 6f72 6967 696e 616c 5f63 6c61  ch..original_cla
-00000df0: 7373 7211 0000 0072 1200 0000 da07 6368  ssr....r......ch
-00000e00: 616e 6e65 6c72 1300 0000 7251 0000 0072  annelr....rQ...r
-00000e10: 1e00 0000 7217 0000 0072 1b00 0000 7214  ....r....r....r.
-00000e20: 0000 0072 1800 0000 7221 0000 0072 1600  ...r....r!...r..
-00000e30: 0000 da06 7265 7475 726e 630e 0000 0000  ....returnc.....
-00000e40: 0000 0000 0000 0022 0000 0007 0000 0003  ......."........
-00000e50: 0000 0073 3403 0000 7400 a001 8804 a101  ...s4...t.......
-00000e60: a002 a100 7400 a001 8803 a101 a002 a100  ....t...........
-00000e70: 0200 8904 8903 7c00 6a03 5c03 7d0e 7d0f  ......|.j.\.}.}.
-00000e80: 7d10 7400 a004 7c00 a101 a002 a100 8803  }.t...|.........
-00000e90: 1800 8804 1b00 7d00 7400 6a01 7c01 6701  ......}.t.j.|.g.
-00000ea0: 7400 6a05 6401 8d02 7d01 7400 6a06 7c00  t.j.d...}.t.j.|.
-00000eb0: 6402 6403 8d02 7d11 8802 6a07 6404 6b02  d.d...}...j.d.k.
-00000ec0: 726e 7c11 7d00 7c11 8804 1400 8803 1700  rn|.}.|.........
-00000ed0: 8905 8802 6a07 6404 6b02 729a 8702 6601  ....j.d.k.r...f.
-00000ee0: 6405 6406 8408 8900 6407 6406 8400 7d12  d.d.....d.d...}.
-00000ef0: 6e38 7c00 6408 6408 6408 8502 6602 1900  n8|.d.d.d...f...
-00000f00: 8804 1400 8803 1700 8906 8703 8704 8705  ................
-00000f10: 8706 6604 6409 6406 8408 7d13 7408 7c13  ..f.d.d...}.t.|.
-00000f20: 8802 8302 5c02 8900 7d12 7409 a00a 8701  ....\...}.t.....
-00000f30: 6601 640a 640b 8408 7c04 4400 8301 a101  f.d.d...|.D.....
-00000f40: 7d14 7400 a00b 8803 0b00 8804 1b00 7400  }.t...........t.
-00000f50: a00c 7c10 a101 640c 1400 a102 7400 a00c  ..|...d.....t...
-00000f60: 7c10 a101 640d 1400 6602 7d15 7c11 7c14  |...d...f.}.|.|.
-00000f70: 0f00 1900 740d 1800 7c15 640e 1900 7c14  ....t...|.d...|.
-00000f80: 0f00 3c00 7c11 7c14 0f00 1900 740d 1700  ..<.|.|.....t...
-00000f90: 7c15 640f 1900 7c14 0f00 3c00 8700 6601  |.d...|...<...f.
-00000fa0: 6410 6406 8408 7d16 7c16 7c11 6408 6408  d.d...}.|.|.d.d.
-00000fb0: 6408 8502 6602 1900 8301 a00e a100 a00f  d...f...........
-00000fc0: a100 a010 a100 7d17 7c09 9001 7284 7411  ......}.|...r.t.
-00000fd0: 6411 7c17 9b00 9d02 8301 0100 7c17 6402  d.|.........|.d.
-00000fe0: 1900 7c0d 6b04 7d18 7c18 7c02 6b02 9001  ..|.k.}.|.|.k...
-00000ff0: 72a6 7411 6412 8301 0100 6408 5300 6413  r.t.d.....d.S.d.
-00001000: 7c00 6a03 1700 7d19 7412 7c16 7c12 7c19  |.j...}.t.|.|.|.
-00001010: 6603 7c15 7c08 7c09 6414 9c03 7c0a a401  f.|.|.|.d...|...
-00001020: 8e01 7d1a 7c1a a013 a100 0100 7c1a 6a14  ..}.|.......|.j.
-00001030: 7c11 6408 6408 6408 8502 6602 1900 7c01  |.d.d.d...f...|.
-00001040: 6408 6408 6408 8502 6602 1900 7c02 6701  d.d.d...f...|.g.
-00001050: 6415 8d03 7d1b 7c1b 6a15 6408 7501 9003  d...}.|.j.d.u...
-00001060: 7230 7c1b 6a15 6416 1900 640e 1900 7d1c  r0|.j.d...d...}.
-00001070: 7c1b 6a15 6417 1900 640e 1900 7d1a 7c12  |.j.d...d...}.|.
-00001080: 7400 a004 7c1a 6408 6408 6408 8502 6602  t...|.d.d.d...f.
-00001090: 1900 a101 8301 7d1a 8802 6a07 6404 6b02  ......}...j.d.k.
-000010a0: 9002 7254 8800 7c1a 8301 6e06 8802 7c1a  ..rT..|...n...|.
-000010b0: 8301 7d1d 8802 6a07 6404 6b03 9002 7274  ..}...j.d.k...rt
-000010c0: 7400 a016 7c1a 6418 a102 7d1a 7411 6419  t...|.d...}.t.d.
-000010d0: 7c1d 9b00 9d02 8301 0100 7417 7c1a 8804  |.........t.|...
-000010e0: 1400 8803 1700 7c1a 6a18 640f 1800 641a  ......|.j.d...d.
-000010f0: 8d02 7d1e 7c11 8804 1400 8803 1700 7d00  ..}.|.........}.
-00001100: 7c1e 7c00 1800 7c00 1b00 641b 1400 7d1f  |.|...|...d...}.
-00001110: 7419 741a 7409 a00a 7c04 a101 7c14 1900  t.t.t...|...|...
-00001120: 7c1f 7c14 1900 a010 a100 8302 8301 7d20  |.|...........} 
-00001130: 7411 641c 7c20 9b00 9d02 8301 0100 7c0b  t.d.| ........|.
-00001140: 6408 7501 9003 7230 741b 6a1c 7c0b 641d  d.u...r0t.j.|.d.
-00001150: 641e 8d02 0100 741b 6a1d a01e 7c0b 641f  d.....t.j...|.d.
-00001160: 7c0c 9b00 6420 9d03 a102 7d21 7409 6a1f  |...d ....}!t.j.
-00001170: 7c21 7c1b 7c20 7409 a00a 7c04 a101 7c14  |!|.| t...|...|.
-00001180: 1900 6421 8d04 0100 7c1b 5300 2922 619a  ..d!....|.S.)"a.
-00001190: 0300 000a 2020 2020 4765 6e65 7261 7465  ....    Generate
-000011a0: 2063 6f75 6e74 6572 6661 6374 7561 6c73   counterfactuals
-000011b0: 2066 6f72 2061 2067 6976 656e 2069 6d61   for a given ima
-000011c0: 6765 2070 6174 6368 2e0a 0a20 2020 2041  ge patch...    A
-000011d0: 7267 733a 0a20 2020 2020 2020 2020 6f72  rgs:.         or
-000011e0: 6967 696e 616c 5f70 6174 6368 2028 6e70  iginal_patch (np
-000011f0: 2e6e 6461 7272 6179 293a 204f 7269 6769  .ndarray): Origi
-00001200: 6e61 6c20 7061 7463 6820 746f 2062 6520  nal patch to be 
-00001210: 6578 706c 6169 6e65 642e 0a20 2020 2020  explained..     
-00001220: 2020 2020 6f72 6967 696e 616c 5f63 6c61      original_cla
-00001230: 7373 2028 6e70 2e6e 6461 7272 6179 293a  ss (np.ndarray):
-00001240: 204f 7269 6769 6e61 6c20 6c61 6265 6c20   Original label 
-00001250: 6f66 2074 6865 2070 6174 6368 2e0a 2020  of the patch..  
-00001260: 2020 2020 2020 206d 6f64 656c 2028 746f         model (to
-00001270: 7263 682e 6e6e 2e4d 6f64 756c 6529 3a20  rch.nn.Module): 
-00001280: 4d6f 6465 6c20 746f 2062 6520 6578 706c  Model to be expl
-00001290: 6169 6e65 642e 0a20 2020 2020 2020 2020  ained..         
-000012a0: 6368 616e 6e65 6c5f 746f 5f70 6572 7475  channel_to_pertu
-000012b0: 7262 2028 6c69 7374 293a 204c 6973 7420  rb (list): List 
-000012c0: 6f66 2063 6861 6e6e 656c 7320 746f 2070  of channels to p
-000012d0: 6572 7475 7262 2e0a 2020 2020 2020 2020  erturb..        
-000012e0: 206e 6f72 6d61 6c69 7a61 7469 6f6e 5f70   normalization_p
-000012f0: 6172 616d 7320 2864 6963 7429 3a20 4469  arams (dict): Di
-00001300: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
-00001310: 696e 6720 7468 6520 6d65 616e 2061 6e64  ing the mean and
-00001320: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
-00001330: 696f 6e20 6f66 2065 6163 6820 6368 616e  ion of each chan
-00001340: 6e65 6c2e 0a20 2020 2020 2020 2020 7472  nel..         tr
-00001350: 6169 6e5f 6461 7461 2028 7374 722c 206f  ain_data (str, o
-00001360: 7074 696f 6e61 6c29 3a20 5061 7468 2074  ptional): Path t
-00001370: 6f20 7468 6520 7472 6169 6e69 6e67 2064  o the training d
-00001380: 6174 612e 2044 6566 6175 6c74 7320 746f  ata. Defaults to
-00001390: 204e 6f6e 652e 0a20 2020 2020 2020 2020   None..         
-000013a0: 6f70 7469 6d69 7a61 7469 6f6e 5f70 6172  optimization_par
-000013b0: 616d 7320 2864 6963 742c 206f 7074 696f  ams (dict, optio
-000013c0: 6e61 6c29 3a20 4469 6374 696f 6e61 7279  nal): Dictionary
-000013d0: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
-000013e0: 7061 7261 6d65 7465 7273 2066 6f72 2074  parameters for t
-000013f0: 6865 206f 7074 696d 697a 6174 696f 6e2e  he optimization.
-00001400: 2044 6566 6175 6c74 7320 746f 207b 7d2e   Defaults to {}.
-00001410: 0a20 2020 2020 2020 2020 7361 7665 5f64  .         save_d
-00001420: 6972 2028 7374 722c 206f 7074 696f 6e61  ir (str, optiona
-00001430: 6c29 3a20 4469 7265 6374 6f72 7920 7768  l): Directory wh
-00001440: 6572 6520 6f75 7470 7574 2077 696c 6c20  ere output will 
-00001450: 6265 2073 6176 6564 2e20 4465 6661 756c  be saved. Defaul
-00001460: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
-00001470: 2020 2020 2070 6174 6368 5f69 6420 2869       patch_id (i
-00001480: 6e74 2c20 6f70 7469 6f6e 616c 293a 2050  nt, optional): P
-00001490: 6174 6368 2049 442e 2044 6566 6175 6c74  atch ID. Default
-000014a0: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
-000014b0: 2020 2020 7468 7265 7368 6f6c 6420 2866      threshold (f
-000014c0: 6c6f 6174 2c20 6f70 7469 6f6e 616c 293a  loat, optional):
-000014d0: 2054 6872 6573 686f 6c64 2066 6f72 2074   Threshold for t
-000014e0: 6865 2070 7265 6469 6374 696f 6e20 7072  he prediction pr
-000014f0: 6f62 6162 696c 6974 792e 2044 6566 6175  obability. Defau
-00001500: 6c74 7320 746f 2030 2e35 2e0a 0a20 2020  lts to 0.5...   
-00001510: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00001520: 2020 2020 4e6f 6e65 0a20 2020 2072 0d00      None.    r..
-00001530: 0000 2902 7201 0000 0072 0600 0000 a901  ..).r....r......
-00001540: da03 6469 6dda 036d 6c70 6301 0000 0000  ..dim..mlpc.....
-00001550: 0000 0000 0000 0001 0000 0004 0000 0013  ................
-00001560: 0000 0073 1600 0000 7400 6a01 6a02 6a03  ...s....t.j.j.j.
-00001570: 8800 7c00 8301 6401 6402 8d02 5300 2903  ..|...d.d...S.).
-00001580: 4e72 0600 0000 725c 0000 0029 04da 0574  Nr....r\...)...t
-00001590: 6f72 6368 da02 6e6e da0a 6675 6e63 7469  orch..nn..functi
-000015a0: 6f6e 616c da07 736f 6674 6d61 78a9 01da  onal..softmax...
-000015b0: 0178 2901 7212 0000 0072 2800 0000 7229  .x).r....r(...r)
-000015c0: 0000 00da 083c 6c61 6d62 6461 3eb9 0000  .....<lambda>...
-000015d0: 0072 2e00 0000 7a21 6765 6e65 7261 7465  .r....z!generate
-000015e0: 5f6f 6e65 5f63 662e 3c6c 6f63 616c 733e  _one_cf.<locals>
-000015f0: 2e3c 6c61 6d62 6461 3e63 0100 0000 0000  .<lambda>c......
-00001600: 0000 0000 0000 0100 0000 0100 0000 5300  ..............S.
-00001610: 0000 7304 0000 007c 0053 0072 2500 0000  ..s....|.S.r%...
-00001620: 7228 0000 0072 6300 0000 7228 0000 0072  r(...rc...r(...r
-00001630: 2800 0000 7229 0000 0072 6500 0000 ba00  (...r)...re.....
-00001640: 0000 722e 0000 004e 6301 0000 0000 0000  ..r....Nc.......
-00001650: 0000 0000 0001 0000 0006 0000 0013 0000  ................
-00001660: 0073 1000 0000 7400 7c00 8803 8800 8801  .s....t.|.......
-00001670: 8802 8305 5300 7225 0000 0029 01da 0b61  ....S.r%...)...a
-00001680: 6c74 6572 5f69 6d61 6765 2901 da01 7929  lter_image)...y)
-00001690: 0472 5100 0000 721e 0000 00da 0d75 6e6e  .rQ...r......unn
-000016a0: 6f72 6d65 645f 6d65 616e da0e 756e 6e6f  ormed_mean..unno
-000016b0: 726d 6564 5f70 6174 6368 7228 0000 0072  rmed_patchr(...r
-000016c0: 2900 0000 7265 0000 00bd 0000 0072 2e00  )...re.......r..
-000016d0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-000016e0: 0000 0004 0000 0013 0000 0073 1c00 0000  ...........s....
-000016f0: 6700 7c00 5d14 7d01 7c01 8800 7600 7214  g.|.].}.|...v.r.
-00001700: 6400 6e02 6401 9102 7104 5300 2902 5446  d.n.d...q.S.).TF
-00001710: 7228 0000 0029 0272 2b00 0000 da04 6e61  r(...).r+.....na
-00001720: 6d65 2901 7213 0000 0072 2800 0000 7229  me).r....r(...r)
-00001730: 0000 0072 2d00 0000 c200 0000 722e 0000  ...r-.......r...
-00001740: 007a 2367 656e 6572 6174 655f 6f6e 655f  .z#generate_one_
-00001750: 6366 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  cf.<locals>.<lis
-00001760: 7463 6f6d 703e e9fc ffff ffe9 0400 0000  tcomp>..........
-00001770: 7201 0000 0072 0600 0000 6301 0000 0000  r....r....c.....
-00001780: 0000 0000 0000 0001 0000 0002 0000 0013  ................
-00001790: 0000 0073 0800 0000 8800 7c00 8301 5300  ...s......|...S.
-000017a0: 7225 0000 0072 2800 0000 7263 0000 0029  r%...r(...rc...)
-000017b0: 01da 0d61 6c74 6572 6564 5f6d 6f64 656c  ...altered_model
-000017c0: 7228 0000 0072 2900 0000 7265 0000 00c9  r(...r)...re....
-000017d0: 0000 0072 2e00 0000 7a15 496e 6974 6961  ...r....z.Initia
-000017e0: 6c20 7072 6f62 6162 696c 6974 793a 207a  l probability: z
-000017f0: 4549 6e73 7461 6e63 6520 616c 7265 6164  EInstance alread
-00001800: 7920 636c 6173 7369 6669 6564 2061 7320  y classified as 
-00001810: 7461 7267 6574 2063 6c61 7373 2c20 6e6f  target class, no
-00001820: 2063 6f75 6e74 6572 6661 6374 7561 6c20   counterfactual 
-00001830: 6e65 6564 6564 2901 7206 0000 0029 03da  needed).r....)..
-00001840: 0d66 6561 7475 7265 5f72 616e 6765 5a0a  .feature_rangeZ.
-00001850: 7472 7573 7473 636f 7265 721b 0000 0029  trustscorer....)
-00001860: 03da 0158 da01 5972 1100 0000 5a05 7072  ...X..Yr....Z.pr
-00001870: 6f62 6172 6f00 0000 2904 7201 0000 0072  obaro...).r....r
-00001880: 0400 0000 e903 0000 0072 0600 0000 7a1c  .........r....z.
-00001890: 436f 756e 7465 7266 6163 7475 616c 2070  Counterfactual p
-000018a0: 726f 6261 6269 6c69 7479 3a20 a901 da0c  robability: ....
-000018b0: 7072 6573 6572 7665 4178 6973 e964 0000  preserveAxis.d..
-000018c0: 007a 0e63 6620 7065 7274 7572 6265 643a  .z.cf perturbed:
-000018d0: 2054 721f 0000 005a 0670 6174 6368 5f7a   Tr....Z.patch_z
-000018e0: 042e 6e70 7a29 03da 0b65 7870 6c61 6e61  ..npz)...explana
-000018f0: 7469 6f6e da0c 6366 5f70 6572 7475 7262  tion..cf_perturb
-00001900: 6564 7213 0000 0029 2072 5f00 0000 da06  edr....) r_.....
-00001910: 7465 6e73 6f72 da05 666c 6f61 74da 0573  tensor..float..s
-00001920: 6861 7065 da0a 6672 6f6d 5f6e 756d 7079  hape..from_numpy
-00001930: da05 696e 7436 3472 1d00 0000 da04 6172  ..int64r......ar
-00001940: 6368 da0e 6164 645f 696e 6974 5f6c 6179  ch..add_init_lay
-00001950: 6572 da02 6e70 da05 6172 7261 79da 076d  er..np..array..m
-00001960: 6178 696d 756d da04 6f6e 6573 da07 4550  aximum..ones..EP
-00001970: 5349 4c4f 4eda 0664 6574 6163 68da 0363  SILON..detach..c
-00001980: 7075 da05 6e75 6d70 7972 4400 0000 7207  pu..numpyrD...r.
-00001990: 0000 00da 0366 6974 da07 6578 706c 6169  .....fit..explai
-000019a0: 6eda 0263 66da 0770 6572 6d75 7465 da18  n..cf..permute..
-000019b0: 6d65 616e 5f70 7265 7365 7276 655f 6469  mean_preserve_di
-000019c0: 6d65 6e73 696f 6e73 da04 6e64 696d da04  mensions..ndim..
-000019d0: 6469 6374 da03 7a69 7072 3400 0000 7240  dict..zipr4...r@
-000019e0: 0000 0072 3500 0000 7236 0000 00da 0573  ...r5...r6.....s
-000019f0: 6176 657a 2922 7258 0000 0072 5900 0000  avez)"rX...rY...
-00001a00: 7211 0000 0072 1200 0000 725a 0000 0072  r....r....rZ...r
-00001a10: 1300 0000 7251 0000 0072 1e00 0000 7217  ....rQ...r....r.
-00001a20: 0000 0072 1b00 0000 7214 0000 0072 1800  ...r....r....r..
-00001a30: 0000 7221 0000 0072 1600 0000 da01 4872  ..r!...r......Hr
-00001a40: 5600 0000 da01 435a 0658 5f6d 6561 6eda  V.....CZ.X_mean.
-00001a50: 0f69 6e70 7574 5f74 7261 6e73 666f 726d  .input_transform
-00001a60: da08 696e 6974 5f66 756e 5a0c 6973 5f70  ..init_funZ.is_p
-00001a70: 6572 7475 7262 6564 726e 0000 005a 0a70  erturbedrn...Z.p
-00001a80: 7265 6469 6374 5f66 6e5a 0a6f 7269 675f  redict_fnZ.orig_
-00001a90: 7072 6f62 61da 0470 7265 6472 7900 0000  proba..predry...
-00001aa0: 7288 0000 0072 7500 0000 5a07 6366 5f70  r....ru...Z.cf_p
-00001ab0: 726f 625a 1c63 6f75 6e74 6572 6661 6374  robZ.counterfact
-00001ac0: 7561 6c5f 7072 6f62 6162 696c 6974 6965  ual_probabilitie
-00001ad0: 735a 0b58 5f70 6572 7475 7262 6564 5a08  sZ.X_perturbedZ.
-00001ae0: 6366 5f64 656c 7461 7276 0000 005a 0a73  cf_deltarv...Z.s
-00001af0: 6176 6564 5f66 696c 6572 2800 0000 2907  aved_filer(...).
-00001b00: 726d 0000 0072 1300 0000 7212 0000 0072  rm...r....r....r
-00001b10: 5100 0000 721e 0000 0072 6800 0000 7269  Q...r....rh...ri
-00001b20: 0000 0072 2900 0000 7226 0000 0087 0000  ...r)...r&......
-00001b30: 0073 9a00 0000 0024 0c01 0cfe 0604 0c01  .s.....$........
-00001b40: 1601 1201 0e02 0a01 0403 0c01 0a01 0c01  ................
-00001b50: 0a02 1801 1201 0e03 0401 10ff 0403 2a01  ..............*.
-00001b60: 1801 1803 0c03 2001 0601 0e01 0c01 0a01  ...... .........
-00001b70: 0801 0403 0a01 0201 0201 0201 02fd 0204  ................
-00001b80: 0201 0201 02fa 0407 02f9 0609 0803 0401  ................
-00001b90: 20ff 0604 0c01 0e01 0e03 1a02 1aff 0203   ...............
-00001ba0: 0c01 0c02 0e01 0201 12ff 0603 0c01 1001  ................
-00001bb0: 0201 0201 0c01 0afe 02ff 0406 0e02 0a01  ................
-00001bc0: 0e01 1601 0401 0201 0201 0201 0cfc 0606  ................
-00001bd0: 7226 0000 0029 0572 1a00 0000 7212 0000  r&...).r....r...
-00001be0: 0072 5100 0000 721e 0000 0072 1c00 0000  .rQ...r....r....
-00001bf0: 6306 0000 0000 0000 0000 0000 000b 0000  c...............
-00001c00: 0006 0000 0043 0000 0073 b400 0000 7400  .....C...s....t.
-00001c10: 7c01 8301 7d06 7401 a002 7c06 7403 a004  |...}.t...|.t...
-00001c20: 7c03 a101 1800 7403 a004 7c04 a101 1b00  |.....t...|.....
-00001c30: a101 a005 a100 7d06 7c02 6a06 6401 6b02  ......}.|.j.d.k.
-00001c40: 7242 7401 a007 7c06 6402 a102 7d07 6e0c  rBt...|.d...}.n.
-00001c50: 7401 a008 7c06 6403 a102 7d07 7c02 7c07  t...|.d...}.|.|.
-00001c60: 8301 a009 a100 a00a a100 7d08 7403 6a0b  ..........}.t.j.
-00001c70: 7c08 6404 6405 8d02 7d09 7c05 6400 7501  |.d.d...}.|.d.u.
-00001c80: 7284 740c 6600 6900 7c05 a401 8e01 7d0a  r.t.f.i.|.....}.
-00001c90: 6e06 740c 8300 7d0a 7401 a007 7c06 6402  n.t...}.t...|.d.
-00001ca0: a102 7d06 7c0a 6a0d 7c06 7c09 6406 6407  ..}.|.j.|.|.d.d.
-00001cb0: 8d03 0100 740e 7c0a 7c00 8302 0100 6400  ....t.|.|.....d.
-00001cc0: 5300 2908 4e72 5e00 0000 2902 7206 0000  S.).Nr^...).r...
-00001cd0: 0072 0400 0000 a904 7201 0000 0072 7100  .r......r....rq.
-00001ce0: 0000 7206 0000 0072 0400 0000 7206 0000  ..r....r....r...
-00001cf0: 00a9 01da 0461 7869 7372 0400 0000 2901  .....axisr....).
-00001d00: da07 636c 6173 7365 7329 0fda 176c 6f61  ..classes)...loa
-00001d10: 645f 6e70 795f 6669 6c65 735f 746f 5f61  d_npy_files_to_a
-00001d20: 7272 6179 725f 0000 0072 7a00 0000 727e  rrayr_...rz...r~
-00001d30: 0000 0072 7f00 0000 7278 0000 0072 7c00  ...r....rx...r|.
-00001d40: 0000 721d 0000 0072 8900 0000 7283 0000  ..r....r....r...
-00001d50: 0072 8500 0000 da06 6172 676d 6178 7208  .r......argmaxr.
-00001d60: 0000 0072 8600 0000 da0b 7361 7665 5f6f  ...r......save_o
-00001d70: 626a 6563 7429 0b72 1700 0000 721a 0000  bject).r....r...
-00001d80: 0072 1200 0000 7251 0000 0072 1e00 0000  .r....rQ...r....
-00001d90: 721c 0000 005a 0b74 7261 696e 5f70 6174  r....Z.train_pat
-00001da0: 6368 5a03 585f 745a 096d 6f64 656c 5f6f  chZ.X_tZ.model_o
-00001db0: 7574 da05 7072 6564 73da 0274 7372 2800  ut..preds..tsr(.
-00001dc0: 0000 7228 0000 0072 2900 0000 7243 0000  ..r(...r)...rC..
-00001dd0: 000c 0100 0073 1e00 0000 0008 0801 0401  .....s..........
-00001de0: 16ff 0803 0a01 0e02 0c02 1001 0e02 0801  ................
-00001df0: 1002 0601 0c01 1001 7243 0000 0063 0100  ........rC...c..
-00001e00: 0000 0000 0000 0000 0000 0900 0000 0600  ................
-00001e10: 0000 4300 0000 7372 0000 0067 007d 0164  ..C...sr...g.}.d
-00001e20: 0164 0267 027d 027c 0244 005d 4e7d 0374  .d.g.}.|.D.]N}.t
-00001e30: 006a 01a0 027c 007c 03a1 027d 0474 00a0  .j...|.|...}.t..
-00001e40: 037c 04a1 0144 005d 307d 057c 05a0 0464  .|...D.]0}.|...d
-00001e50: 03a1 0172 2c74 006a 01a0 027c 047c 05a1  ...r,t.j...|.|..
-00001e60: 027d 0674 05a0 067c 06a1 017d 077c 01a0  .}.t...|...}.|..
-00001e70: 077c 07a1 0101 0071 2c71 1074 056a 087c  .|.....q,q.t.j.|
-00001e80: 0164 0464 058d 027d 087c 0853 0029 064e  .d.d...}.|.S.).N
-00001e90: da01 30da 0131 7a04 2e6e 7079 7201 0000  ..0..1z..npyr...
-00001ea0: 0072 9500 0000 2909 7234 0000 0072 3500  .r....).r4...r5.
-00001eb0: 0000 7236 0000 00da 076c 6973 7464 6972  ..r6.....listdir
-00001ec0: da08 656e 6473 7769 7468 727e 0000 0072  ..endswithr~...r
-00001ed0: 3900 0000 724b 0000 00da 0573 7461 636b  9...rK.....stack
-00001ee0: 2909 da08 6261 7365 5f64 6972 da06 6172  )...base_dir..ar
-00001ef0: 7261 7973 5a08 7375 625f 6469 7273 da07  raysZ.sub_dirs..
-00001f00: 7375 625f 6469 725a 0c73 7562 5f64 6972  sub_dirZ.sub_dir
-00001f10: 5f70 6174 68da 0466 696c 65da 0966 696c  _path..file..fil
-00001f20: 655f 7061 7468 727f 0000 005a 0b66 696e  e_pathr....Z.fin
-00001f30: 616c 5f61 7272 6179 7228 0000 0072 2800  al_arrayr(...r(.
-00001f40: 0000 7229 0000 0072 9800 0000 2901 0000  ..r)...r....)...
-00001f50: 7316 0000 0000 0104 0108 0208 010e 010e  s...............
-00001f60: 010a 010e 010a 010e 030e 0172 9800 0000  ...........r....
-00001f70: 6305 0000 0000 0000 0000 0000 0007 0000  c...............
-00001f80: 0007 0000 0043 0000 0073 3800 0000 7c00  .....C...s8...|.
-00001f90: 7c03 1400 7c02 1700 7d05 7c01 7c05 7c04  |...|...}.|.|.|.
-00001fa0: 1b00 6400 6400 8502 6400 6400 6400 6400  ..d.d...d.d.d.d.
-00001fb0: 8502 6604 1900 1400 7d06 7c06 7c02 1800  ..f.....}.|.|...
-00001fc0: 7c03 1b00 5300 7225 0000 0072 2800 0000  |...S.r%...r(...
-00001fd0: 2907 7267 0000 0072 6900 0000 7251 0000  ).rg...ri...rQ..
-00001fe0: 0072 1e00 0000 7268 0000 005a 0a75 6e6e  .r....rh...Z.unn
-00001ff0: 6f72 6d65 645f 795a 096e 6577 5f70 6174  ormed_yZ.new_pat
-00002000: 6368 7228 0000 0072 2800 0000 7229 0000  chr(...r(...r)..
-00002010: 0072 6600 0000 3a01 0000 7306 0000 0000  .rf...:...s.....
-00002020: 010c 0120 0172 6600 0000 6302 0000 0000  ... .rf...c.....
-00002030: 0000 0000 0000 0005 0000 0004 0000 0003  ................
-00002040: 0000 0073 3400 0000 4700 8700 6601 6401  ...s4...G...f.d.
-00002050: 6402 8408 6402 7400 6a01 6a02 8303 7d02  d...d.t.j.j...}.
-00002060: 7c02 8300 7d03 7400 6a01 a003 7c03 7c01  |...}.t.j...|.|.
-00002070: a102 7d04 7c04 7c03 6602 5300 2903 6116  ..}.|.|.f.S.).a.
-00002080: 0100 000a 2020 2020 4164 6420 616e 2069  ....    Add an i
-00002090: 6e69 7469 616c 697a 6174 696f 6e20 6c61  nitialization la
-000020a0: 7965 7220 746f 2074 6865 206d 6f64 656c  yer to the model
-000020b0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-000020c0: 2020 2020 2069 6e69 745f 6675 6e20 2863       init_fun (c
-000020d0: 616c 6c61 626c 6529 3a20 496e 6974 6961  allable): Initia
-000020e0: 6c69 7a61 7469 6f6e 2066 756e 6374 696f  lization functio
-000020f0: 6e2e 0a20 2020 2020 2020 206d 6f64 656c  n..        model
-00002100: 2028 746f 7263 682e 6e6e 2e4d 6f64 756c   (torch.nn.Modul
-00002110: 6529 3a20 4f72 6967 696e 616c 206d 6f64  e): Original mod
-00002120: 656c 2e0a 0a20 2020 2052 6574 7572 6e73  el...    Returns
-00002130: 3a0a 2020 2020 2020 2020 7475 706c 653a  :.        tuple:
-00002140: 2028 746f 7263 682e 6e6e 2e4d 6f64 756c   (torch.nn.Modul
-00002150: 652c 2074 6f72 6368 2e6e 6e2e 4d6f 6475  e, torch.nn.Modu
-00002160: 6c65 2920 2d20 4d6f 6469 6669 6564 206d  le) - Modified m
-00002170: 6f64 656c 2061 6e64 2069 6e70 7574 2074  odel and input t
-00002180: 7261 6e73 666f 726d 6174 696f 6e20 6c61  ransformation la
-00002190: 7965 722e 0a20 2020 2063 0000 0000 0000  yer..    c......
-000021a0: 0000 0000 0000 0000 0000 0300 0000 0000  ................
-000021b0: 0000 7318 0000 0065 005a 0164 005a 0287  ..s....e.Z.d.Z..
-000021c0: 0066 0164 0164 0284 085a 0364 0353 0029  .f.d.d...Z.d.S.)
-000021d0: 047a 2061 6464 5f69 6e69 745f 6c61 7965  .z add_init_laye
-000021e0: 722e 3c6c 6f63 616c 733e 2e49 6e70 7574  r.<locals>.Input
-000021f0: 4675 6e63 0200 0000 0000 0000 0000 0000  Func............
-00002200: 0200 0000 0400 0000 1300 0000 7314 0000  ............s...
-00002210: 0074 00a0 0188 007c 0183 0164 01a1 02a0  .t.....|...d....
-00002220: 02a1 0053 0029 024e 7294 0000 0029 0372  ...S.).Nr....).r
-00002230: 5f00 0000 7289 0000 0072 7800 0000 2902  _...r....rx...).
-00002240: da04 7365 6c66 da05 696e 7075 74a9 0172  ..self..input..r
-00002250: 9200 0000 7228 0000 0072 2900 0000 da07  ....r(...r).....
-00002260: 666f 7277 6172 644d 0100 0073 0200 0000  forwardM...s....
-00002270: 0001 7a28 6164 645f 696e 6974 5f6c 6179  ..z(add_init_lay
-00002280: 6572 2e3c 6c6f 6361 6c73 3e2e 496e 7075  er.<locals>.Inpu
-00002290: 7446 756e 2e66 6f72 7761 7264 4e29 04da  tFun.forwardN)..
-000022a0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000022b0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000022c0: 655f 5f72 aa00 0000 7228 0000 0072 a900  e__r....r(...r..
-000022d0: 0000 7228 0000 0072 2900 0000 da08 496e  ..r(...r).....In
-000022e0: 7075 7446 756e 4c01 0000 7302 0000 0008  putFunL...s.....
-000022f0: 0172 ae00 0000 2904 725f 0000 0072 6000  .r....).r_...r`.
-00002300: 0000 da06 4d6f 6475 6c65 da0a 5365 7175  ....Module..Sequ
-00002310: 656e 7469 616c 2905 7292 0000 0072 1200  ential).r....r..
-00002320: 0000 72ae 0000 0072 9100 0000 5a0e 636f  ..r....r....Z.co
-00002330: 6d70 6c65 7465 5f6d 6f64 656c 7228 0000  mplete_modelr(..
-00002340: 0072 a900 0000 7229 0000 0072 7d00 0000  .r....r)...r}...
-00002350: 4001 0000 7308 0000 0000 0c18 0406 010e  @...s...........
-00002360: 0172 7d00 0000 2903 7277 0000 0072 7300  .r}...).rw...rs.
-00002370: 0000 725b 0000 0063 0200 0000 0000 0000  ..r[...c........
-00002380: 0000 0000 0400 0000 0300 0000 0300 0000  ................
-00002390: 7338 0000 0074 0088 0074 0183 0272 1088  s8...t...t...r..
-000023a0: 0066 0189 0087 0066 0164 0164 0284 0874  .f.....f.d.d...t
-000023b0: 027c 006a 0383 0144 0083 017d 027c 006a  .|.j...D...}.|.j
-000023c0: 047c 0264 038d 017d 037c 0353 0029 0461  .|.d...}.|.S.).a
-000023d0: 2701 0000 0a20 2020 2043 6f6d 7075 7465  '....    Compute
-000023e0: 2074 6865 206d 6561 6e20 616c 6f6e 6720   the mean along 
-000023f0: 616c 6c20 6469 6d65 6e73 696f 6e73 2065  all dimensions e
-00002400: 7863 6570 7420 7468 6f73 6520 7370 6563  xcept those spec
-00002410: 6966 6965 6420 696e 2070 7265 7365 7276  ified in preserv
-00002420: 6541 7869 732e 0a0a 2020 2020 4172 6773  eAxis...    Args
-00002430: 3a0a 2020 2020 2020 2020 7465 6e73 6f72  :.        tensor
-00002440: 2028 746f 7263 682e 5465 6e73 6f72 293a   (torch.Tensor):
-00002450: 2049 6e70 7574 2074 656e 736f 722e 0a20   Input tensor.. 
-00002460: 2020 2020 2020 2070 7265 7365 7276 6541         preserveA
-00002470: 7869 7320 2874 7570 6c65 2c20 6f70 7469  xis (tuple, opti
-00002480: 6f6e 616c 293a 2044 696d 656e 7369 6f6e  onal): Dimension
-00002490: 7320 746f 2070 7265 7365 7276 652e 2044  s to preserve. D
-000024a0: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
-000024b0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-000024c0: 2020 2020 2020 2074 6f72 6368 2e54 656e         torch.Ten
-000024d0: 736f 723a 2054 656e 736f 7220 7769 7468  sor: Tensor with
-000024e0: 2070 7265 7365 7276 6564 2064 696d 656e   preserved dimen
-000024f0: 7369 6f6e 732e 0a20 2020 2063 0100 0000  sions..    c....
-00002500: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00002510: 1300 0000 7318 0000 0067 007c 005d 107d  ....s....g.|.].}
-00002520: 017c 0188 0076 0172 047c 0191 0271 0453  .|...v.r.|...q.S
-00002530: 0072 2800 0000 7228 0000 0029 0272 2b00  .r(...r(...).r+.
-00002540: 0000 7252 0000 0072 7200 0000 7228 0000  ..rR...rr...r(..
-00002550: 0072 2900 0000 722d 0000 0065 0100 0072  .r)...r-...e...r
-00002560: 2e00 0000 7a2c 6d65 616e 5f70 7265 7365  ....z,mean_prese
-00002570: 7276 655f 6469 6d65 6e73 696f 6e73 2e3c  rve_dimensions.<
-00002580: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00002590: 703e 725c 0000 0029 05da 0a69 7369 6e73  p>r\...)...isins
-000025a0: 7461 6e63 65da 0369 6e74 7245 0000 0072  tance..intrE...r
-000025b0: 8b00 0000 721d 0000 0029 0472 7700 0000  ....r....).rw...
-000025c0: 7273 0000 005a 0e64 696d 735f 746f 5f72  rs...Z.dims_to_r
-000025d0: 6564 7563 65da 0672 6573 756c 7472 2800  educe..resultr(.
-000025e0: 0000 7272 0000 0072 2900 0000 728a 0000  ..rr...r)...r...
-000025f0: 0055 0100 0073 0a00 0000 000d 0a01 0602  .U...s..........
-00002600: 1801 0c01 728a 0000 0063 0200 0000 0000  ....r....c......
-00002610: 0000 0000 0000 0300 0000 0800 0000 4300  ..............C.
-00002620: 0000 733c 0000 0074 007c 0164 0183 028f  ..s<...t.|.d....
-00002630: 1e7d 0274 01a0 027c 007c 0264 02a1 0301  .}.t...|.|.d....
-00002640: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
-00002650: 0073 2e30 0001 0001 0001 0059 0001 0064  .s.0.......Y...d
-00002660: 0053 0029 034e da02 7762 e9ff ffff ff29  .S.).N..wb.....)
-00002670: 0372 3300 0000 da06 7069 636b 6c65 da04  .r3.....pickle..
-00002680: 6475 6d70 2903 da03 6f62 6ada 0866 696c  dump)...obj..fil
-00002690: 656e 616d 655a 046f 7574 7072 2800 0000  enameZ.outpr(...
-000026a0: 7228 0000 0072 2900 0000 729a 0000 006a  r(...r)...r....j
-000026b0: 0100 0073 0400 0000 0001 0c01 729a 0000  ...s........r...
-000026c0: 0029 084e 720f 0000 004e 4e72 0600 0000  .).Nr....NNr....
-000026d0: 4e46 4e29 0546 4e4e 4e72 0f00 0000 2901  NFN).FNNNr....).
-000026e0: 4e29 014e 292e 7234 0000 0072 3800 0000  N).N).r4...r8...
-000026f0: da07 5f70 6963 6b6c 6572 b600 0000 7285  .._pickler....r.
-00002700: 0000 0072 7e00 0000 da06 7061 6e64 6173  ...r~.....pandas
-00002710: da02 7064 da06 7479 7069 6e67 7202 0000  ..pd..typingr...
-00002720: 0072 5f00 0000 7203 0000 00da 0864 6174  .r_...r......dat
-00002730: 6173 6574 7372 0500 0000 7288 0000 0072  asetsr....r....r
-00002740: 0700 0000 da0a 636f 6e66 6964 656e 6365  ......confidence
-00002750: 7208 0000 00da 0d63 6f6e 6669 6775 7261  r......configura
-00002760: 7469 6f6e 7209 0000 0072 0a00 0000 720b  tionr....r....r.
-00002770: 0000 0072 0c00 0000 7277 0000 00da 0766  ...r....rw.....f
-00002780: 6c6f 6174 3332 7282 0000 0072 b200 0000  loat32r....r....
-00002790: 7260 0000 0072 af00 0000 da04 6c69 7374  r`...r......list
-000027a0: 728c 0000 00da 0944 6174 6146 7261 6d65  r......DataFrame
-000027b0: 7278 0000 00da 0373 7472 da04 626f 6f6c  rx.....str..bool
-000027c0: 7257 0000 00da 076e 6461 7272 6179 7226  rW.....ndarrayr&
-000027d0: 0000 0072 4300 0000 7298 0000 0072 6600  ...rC...r....rf.
-000027e0: 0000 727d 0000 00da 0654 656e 736f 72da  ..r}.....Tensor.
-000027f0: 0574 7570 6c65 728a 0000 0072 9a00 0000  .tupler....r....
-00002800: 7228 0000 0072 2800 0000 7228 0000 0072  r(...r(...r(...r
-00002810: 2900 0000 da08 3c6d 6f64 756c 653e 0100  ).....<module>..
-00002820: 0000 7396 0000 0008 0108 0108 0108 0108  ..s.............
-00002830: 010c 0108 020c 050c 010c 010c 0118 0710  ................
-00002840: 0900 0100 0100 0100 0100 0100 0100 0100  ................
-00002850: f302 0102 0102 0106 0102 0102 0104 0102  ................
-00002860: 0102 0102 0102 0102 0102 0106 f30c 7600  ..............v.
-00002870: 0100 0100 0100 0100 f202 0104 0104 0102  ................
-00002880: 0106 0102 0102 0104 0104 0102 0102 0102  ................
-00002890: 0102 0102 0102 0102 f10c 7f00 0c00 fa02  ................
-000028a0: 0202 0106 0102 0102 0106 fa0c 1d08 1108  ................
-000028b0: 0608 1600 ff02 0106 0104 fe0c 15         .............
+00000060: 0100 6400 6401 6c0a 5a0a 6400 6401 6c0b  ..d.d.l.Z.d.d.l.
+00000070: 5a0b 6400 6401 6c0c 5a0c 6400 6403 6c0d  Z.d.d.l.Z.d.d.l.
+00000080: 6d0d 5a0d 0100 6404 6405 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
+00000090: 0100 6406 6407 6c10 6d11 5a11 0100 6404  ..d.d.l.m.Z...d.
+000000a0: 6408 6c12 6d13 5a13 0100 6404 6409 6c14  d.l.m.Z...d.d.l.
+000000b0: 6d15 5a15 0100 6404 640a 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
+000000c0: 6d18 5a18 6d19 5a19 6d1a 5a1a 0100 650a  m.Z.m.Z.m.Z...e.
+000000d0: 6a1b 640b 650a 6a1c 640c 8d02 5a1d 6424  j.d.e.j.d...Z.d$
+000000e0: 650f 651e 651f 6520 6521 6507 6a22 6523  e.e.e.e e!e.j"e#
+000000f0: 651f 651f 651e 651f 651e 6509 6521 1900  e.e.e.e.e.e.e!..
+00000100: 651f 640e 9c0e 640f 6410 8405 5a24 650c  e.d...d.d...Z$e.
+00000110: 6a25 6411 6412 8400 8301 5a26 6425 6505  j%d.d.....Z&d%e.
+00000120: 6a27 6505 6a27 651e 651e 651f 6520 6520  j'e.j'e.e.e.e e 
+00000130: 6505 6a27 6505 6a27 651f 651e 6521 651f  e.j'e.j'e.e.e!e.
+00000140: 6523 651f 6401 6413 9c10 6414 6415 8405  e#e.d.d...d.d...
+00000150: 5a28 6426 651f 650a 6a29 6a2a 6520 6520  Z(d&e.e.j)j*e e 
+00000160: 6509 6521 1900 6416 9c05 6417 6418 8405  e.e!..d...d.d...
+00000170: 5a2b 6419 641a 8400 5a2c 641b 641c 8400  Z+d.d...Z,d.d...
+00000180: 5a2d 641d 641e 8400 5a2e 6427 650a 6a2f  Z-d.d...Z.d'e.j/
+00000190: 6530 650a 6a2f 641f 9c03 6420 6421 8405  e0e.j/d...d d!..
+000001a0: 5a31 6422 6423 8400 5a32 6401 5300 2928  Z1d"d#..Z2d.S.)(
+000001b0: e900 0000 004e 2901 da08 4f70 7469 6f6e  .....N)...Option
+000001c0: 616c 2901 da04 7471 646d e902 0000 0029  al)...tqdm.....)
+000001d0: 01da 0e53 7061 7469 616c 4461 7461 7365  ...SpatialDatase
+000001e0: 74e9 0100 0000 2901 da0e 436f 756e 7465  t.....)...Counte
+000001f0: 7266 6163 7475 616c 2901 da0a 6c6f 6164  rfactual)...load
+00000200: 5f6d 6f64 656c 2901 da0a 5472 7573 7453  _model)...TrustS
+00000210: 636f 7265 2904 da06 5370 6c69 7473 da07  core)...Splits..
+00000220: 436f 6c4e 616d 65da 1144 6566 6175 6c74  ColName..Default
+00000230: 466f 6c64 6572 4e61 6d65 da0f 4465 6661  FolderName..Defa
+00000240: 756c 7446 696c 654e 616d 6567 2342 920c  ultFileNameg#B..
+00000250: a19c c73b a901 da05 6474 7970 65e7 0000  ...;....dtype...
+00000260: 0000 0000 e03f 290e da07 6461 7461 7365  .....?)...datase
+00000270: 74da 0c74 6172 6765 745f 636c 6173 73da  t..target_class.
+00000280: 0a6d 6f64 656c 5f70 6174 68da 1263 6861  .model_path..cha
+00000290: 6e6e 656c 5f74 6f5f 7065 7274 7572 62da  nnel_to_perturb.
+000002a0: 136f 7074 696d 697a 6174 696f 6e5f 7061  .optimization_pa
+000002b0: 7261 6d73 da06 696d 6167 6573 da09 7468  rams..images..th
+000002c0: 7265 7368 6f6c 64da 0b6b 6474 7265 655f  reshold..kdtree_
+000002d0: 7061 7468 da08 7361 7665 5f64 6972 da0b  path..save_dir..
+000002e0: 6e75 6d5f 776f 726b 6572 73da 0a74 7261  num_workers..tra
+000002f0: 696e 5f64 6174 61da 0976 6572 626f 7369  in_data..verbosi
+00000300: 7479 da11 7472 7573 7473 636f 7265 5f6b  ty..trustscore_k
+00000310: 7761 7267 73da 0664 6576 6963 6563 0e00  wargs..devicec..
+00000320: 0000 0000 0000 0000 0000 1e00 0000 0d00  ................
+00000330: 0000 0300 0000 73de 0200 0074 00a0 0174  ......s....t...t
+00000340: 006a 02a0 03a1 0072 1674 006a 026a 046e  .j.....r.t.j.j.n
+00000350: 0474 006a 04a1 0101 0074 0574 066a 07a0  .t.j.....t.t.j..
+00000360: 087c 006a 0964 01a1 0283 018f 2a7d 0e74  .|.j.d......*}.t
+00000370: 0aa0 0b7c 0ea1 017d 0f7c 0f64 0219 007d  ...|...}.|.d...}
+00000380: 107c 0f64 0319 007d 1157 0064 0404 0004  .|.d...}.W.d....
+00000390: 0083 0301 006e 1031 0073 6230 0001 0001  .....n.1.sb0....
+000003a0: 0001 0059 0001 007c 0a64 0475 0072 8874  ...Y...|.d.u.r.t
+000003b0: 066a 07a0 087c 006a 0974 0c6a 0d6a 0ea1  .j...|.j.t.j.j..
+000003c0: 027d 0a7c 0764 0475 0072 a474 066a 07a0  .}.|.d.u.r.t.j..
+000003d0: 087c 006a 0f74 106a 116a 0ea1 027d 077c  .|.j.t.j.j...}.|
+000003e0: 0564 0475 0072 b27c 006a 127d 057c 0864  .d.u.r.|.j.}.|.d
+000003f0: 0475 0072 ce74 066a 07a0 087c 006a 0f74  .u.r.t.j...|.j.t
+00000400: 136a 146a 0ea1 027d 0874 066a 157c 0864  .j.j...}.t.j.|.d
+00000410: 0564 068d 0201 0074 066a 07a0 167c 07a1  .d.....t.j...|..
+00000420: 0190 0173 0474 177c 077c 0a74 187c 107c  ...s.t.|.|.t.|.|
+00000430: 117c 0c83 0601 0074 1964 0783 0101 007c  .|.....t.d.....|
+00000440: 017c 027c 006a 1a7c 037c 107c 117c 077c  .|.|.j.|.|.|.|.|
+00000450: 0b7c 047c 087c 067c 0d64 089c 0c89 0067  .|.|.|.|.d.....g
+00000460: 007d 1274 1b74 1c7c 0583 0183 0144 005d  .}.t.t.|.....D.]
+00000470: 707d 137c 006a 1d7c 056a 1e7c 1319 0074  p}.|.j.|.j.|...t
+00000480: 1f6a 206a 0e19 007c 056a 1e7c 1319 007c  .j j...|.j.|...|
+00000490: 006a 2119 007c 056a 1e7c 1319 0074 1f6a  .j!..|.j.|...t.j
+000004a0: 226a 0e19 0064 098d 037d 1474 23a0 247c  "j...d...}.t#.$|
+000004b0: 14a1 015c 027d 157d 167c 006a 126a 1e7c  ...\.}.}.|.j.j.|
+000004c0: 1619 007c 006a 2119 007d 177c 12a0 257c  ...|.j!..}.|..%|
+000004d0: 157c 177c 1664 0a9c 03a1 0101 0090 0171  .|.|.d.........q
+000004e0: 3474 0574 066a 07a0 087c 0864 0ba1 0264  4t.t.j...|.d...d
+000004f0: 0c83 028f 267d 0e74 0aa0 267c 017c 037c  ....&}.t..&|.|.|
+00000500: 047c 0664 0d9c 047c 0ea1 0201 0057 0064  .|.d...|.....W.d
+00000510: 0404 0004 0083 0301 006e 1231 0090 0173  .........n.1...s
+00000520: e830 0001 0001 0001 0059 0001 007c 0964  .0.......Y...|.d
+00000530: 0e6b 0490 0272 ac74 27a0 28a1 0001 0074  .k...r.t'.(....t
+00000540: 27a0 29a1 0001 0074 27a0 2aa1 0064 0f19  '.)....t'.*..d..
+00000550: 007d 1874 1964 107c 189b 009d 0283 0101  .}.t.d.|........
+00000560: 0087 0066 0164 1164 1284 087c 1244 0083  ...f.d.d...|.D..
+00000570: 017d 1974 2b74 1c7c 1283 0164 138d 018f  .}.t+t.|...d....
+00000580: 4a7d 1a67 007d 1b7c 1990 0272 8274 27a0  J}.g.}.|...r.t'.
+00000590: 2c7c 19a1 015c 027d 1c7d 197c 1ba0 2d74  ,|...\.}.}.|..-t
+000005a0: 27a0 2e7c 1ca1 01a1 0101 007c 1aa0 2f74  '..|.......|../t
+000005b0: 1c7c 1c83 01a1 0101 0090 0271 4c57 0064  .|.........qLW.d
+000005c0: 0404 0004 0083 0301 006e 1231 0090 0273  .........n.1...s
+000005d0: 9830 0001 0001 0001 0059 0001 0074 27a0  .0.......Y...t'.
+000005e0: 28a1 0001 006e 2e74 2b7c 1274 1c7c 1283  (....n.t+|.t.|..
+000005f0: 0164 138d 0244 005d 1c7d 1d74 3066 0069  .d...D.].}.t0f.i
+00000600: 0069 007c 1da5 0188 00a5 01a4 018e 0101  .i.|............
+00000610: 0090 0271 bc64 0453 0029 1461 da03 0000  ...q.d.S.).a....
+00000620: 0a20 2020 2047 656e 6572 6174 6520 636f  .    Generate co
+00000630: 756e 7465 7266 6163 7475 616c 7320 666f  unterfactuals fo
+00000640: 7220 7468 6520 6461 7461 7365 742e 0a0a  r the dataset...
+00000650: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00000660: 2020 6461 7461 7365 7420 2853 7061 7469    dataset (Spati
+00000670: 616c 4461 7461 7365 7429 3a20 4461 7461  alDataset): Data
+00000680: 7365 7420 746f 2067 656e 6572 6174 6520  set to generate 
+00000690: 636f 756e 7465 7266 6163 7475 616c 7320  counterfactuals 
+000006a0: 666f 722e 0a20 2020 2020 2020 2074 6172  for..        tar
+000006b0: 6765 745f 636c 6173 7320 2869 6e74 293a  get_class (int):
+000006c0: 2054 6172 6765 7420 636c 6173 7320 666f   Target class fo
+000006d0: 7220 7468 6520 636f 756e 7465 7266 6163  r the counterfac
+000006e0: 7475 616c 732e 0a20 2020 2020 2020 206d  tuals..        m
+000006f0: 6f64 656c 2028 746f 7263 682e 6e6e 2e4d  odel (torch.nn.M
+00000700: 6f64 756c 6529 3a20 4d6f 6465 6c20 746f  odule): Model to
+00000710: 2067 656e 6572 6174 6520 636f 756e 7465   generate counte
+00000720: 7266 6163 7475 616c 7320 666f 722e 0a20  rfactuals for.. 
+00000730: 2020 2020 2020 2063 6861 6e6e 656c 5f74         channel_t
+00000740: 6f5f 7065 7274 7572 6220 286c 6973 7429  o_perturb (list)
+00000750: 3a20 4c69 7374 206f 6620 6368 616e 6e65  : List of channe
+00000760: 6c73 2074 6f20 7065 7274 7572 622e 0a20  ls to perturb.. 
+00000770: 2020 2020 2020 206f 7074 696d 697a 6174         optimizat
+00000780: 696f 6e5f 7061 7261 6d73 2028 6469 6374  ion_params (dict
+00000790: 293a 2044 6963 7469 6f6e 6172 7920 636f  ): Dictionary co
+000007a0: 6e74 6169 6e69 6e67 2074 6865 2070 6172  ntaining the par
+000007b0: 616d 6574 6572 7320 666f 7220 7468 6520  ameters for the 
+000007c0: 6f70 7469 6d69 7a61 7469 6f6e 2e0a 2020  optimization..  
+000007d0: 2020 2020 2020 696d 6167 6573 2028 7064        images (pd
+000007e0: 2e44 6174 6146 7261 6d65 2c20 6f70 7469  .DataFrame, opti
+000007f0: 6f6e 616c 293a 2049 6d61 6765 7320 746f  onal): Images to
+00000800: 2067 656e 6572 6174 6520 636f 756e 7465   generate counte
+00000810: 7266 6163 7475 616c 7320 666f 722e 2044  rfactuals for. D
+00000820: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
+00000830: 0a20 2020 2020 2020 2074 6872 6573 686f  .        thresho
+00000840: 6c64 2028 666c 6f61 742c 206f 7074 696f  ld (float, optio
+00000850: 6e61 6c29 3a20 5468 7265 7368 6f6c 6420  nal): Threshold 
+00000860: 666f 7220 7468 6520 7072 6564 6963 7469  for the predicti
+00000870: 6f6e 2070 726f 6261 6269 6c69 7479 2e20  on probability. 
+00000880: 4465 6661 756c 7473 2074 6f20 302e 352e  Defaults to 0.5.
+00000890: 0a20 2020 2020 2020 206b 6474 7265 655f  .        kdtree_
+000008a0: 7061 7468 2028 7374 722c 206f 7074 696f  path (str, optio
+000008b0: 6e61 6c29 3a20 5061 7468 2074 6f20 7468  nal): Path to th
+000008c0: 6520 6b64 7472 6565 2066 696c 652e 2044  e kdtree file. D
+000008d0: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
+000008e0: 0a20 2020 2020 2020 2073 6176 655f 6469  .        save_di
+000008f0: 7220 2873 7472 2c20 6f70 7469 6f6e 616c  r (str, optional
+00000900: 293a 2044 6972 6563 746f 7279 2077 6865  ): Directory whe
+00000910: 7265 206f 7574 7075 7420 7769 6c6c 2062  re output will b
+00000920: 6520 7361 7665 642e 2044 6566 6175 6c74  e saved. Default
+00000930: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
+00000940: 2020 206e 756d 5f77 6f72 6b65 7273 2028     num_workers (
+00000950: 626f 6f6c 2c20 6f70 7469 6f6e 616c 293a  bool, optional):
+00000960: 204e 756d 6265 7220 6f66 2077 6f72 6b65   Number of worke
+00000970: 7273 2074 6f20 7573 6520 666f 7220 7061  rs to use for pa
+00000980: 7261 6c6c 656c 2070 726f 6365 7373 696e  rallel processin
+00000990: 672e 2044 6566 6175 6c74 7320 746f 204e  g. Defaults to N
+000009a0: 6f6e 652e 0a20 2020 2020 2020 2074 7261  one..        tra
+000009b0: 696e 5f64 6174 6120 2873 7472 2c20 6f70  in_data (str, op
+000009c0: 7469 6f6e 616c 293a 2050 6174 6820 746f  tional): Path to
+000009d0: 2074 6865 2074 7261 696e 696e 6720 6461   the training da
+000009e0: 7461 2e20 4465 6661 756c 7473 2074 6f20  ta. Defaults to 
+000009f0: 4e6f 6e65 2e0a 2020 2020 7a19 6e6f 726d  None..    z.norm
+00000a00: 616c 697a 6174 696f 6e5f 7061 7261 6d73  alization_params
+00000a10: 2e6a 736f 6eda 046d 6561 6eda 0573 7464  .json..mean..std
+00000a20: 6576 4e54 a901 da08 6578 6973 745f 6f6b  evNT....exist_ok
+00000a30: 7a0c 6b64 7472 6565 2073 6176 6564 290c  z.kdtree saved).
+00000a40: 7212 0000 0072 1300 0000 da07 6368 616e  r....r......chan
+00000a50: 6e65 6c72 1400 0000 da02 6d75 7220 0000  nelr......mur ..
+00000a60: 0072 1800 0000 721c 0000 0072 1500 0000  .r....r....r....
+00000a70: 7219 0000 0072 1700 0000 721e 0000 0029  r....r....r....)
+00000a80: 03da 0870 6174 6368 5f69 64da 056c 6162  ...patch_id..lab
+00000a90: 656c da05 7370 6c69 7429 03da 0e6f 7269  el..split)...ori
+00000aa0: 6769 6e61 6c5f 7061 7463 68da 0e6f 7269  ginal_patch..ori
+00000ab0: 6769 6e61 6c5f 636c 6173 7372 2500 0000  ginal_classr%...
+00000ac0: 7a14 6879 7065 7270 6172 616d 6574 6572  z.hyperparameter
+00000ad0: 732e 6a73 6f6e da01 7729 0472 1200 0000  s.json..w).r....
+00000ae0: 7214 0000 0072 1500 0000 7217 0000 0072  r....r....r....r
+00000af0: 0600 0000 da03 4350 557a 1a4e 756d 6265  ......CPUz.Numbe
+00000b00: 7220 6f66 2061 7661 696c 6162 6c65 2043  r of available C
+00000b10: 5055 733a 2063 0100 0000 0000 0000 0000  PUs: c..........
+00000b20: 0000 0200 0000 0600 0000 1300 0000 731e  ..............s.
+00000b30: 0000 0067 007c 005d 167d 0174 00a0 0169  ...g.|.].}.t...i
+00000b40: 007c 01a5 0188 00a5 01a1 0191 0271 0453  .|...........q.S
+00000b50: 00a9 0029 02da 1767 656e 6572 6174 655f  ...)...generate_
+00000b60: 6f6e 655f 6366 5f77 7261 7070 6572 da06  one_cf_wrapper..
+00000b70: 7265 6d6f 7465 2902 da02 2e30 da04 6172  remote)....0..ar
+00000b80: 6773 a901 5a0c 6765 6e65 7261 6c5f 6172  gs..Z.general_ar
+00000b90: 6773 722c 0000 00fa 562f 6365 6e74 7261  gsr,....V/centra
+00000ba0: 6c2f 686f 6d65 2f7a 7761 6e67 322f 6d6f  l/home/zwang2/mo
+00000bb0: 7270 6865 7573 2d73 7061 7469 616c 2f6d  rpheus-spatial/m
+00000bc0: 6f72 7068 6575 732f 7372 632f 6d6f 7270  orpheus/src/morp
+00000bd0: 6865 7573 2f63 6f75 6e74 6572 6661 6374  heus/counterfact
+00000be0: 7561 6c2f 6765 6e65 7261 7465 2e70 79da  ual/generate.py.
+00000bf0: 0a3c 6c69 7374 636f 6d70 3ea9 0000 0073  .<listcomp>....s
+00000c00: 0400 0000 0602 02ff 7a26 6765 745f 636f  ........z&get_co
+00000c10: 756e 7465 7266 6163 7475 616c 2e3c 6c6f  unterfactual.<lo
+00000c20: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00000c30: 2901 da05 746f 7461 6c29 31da 0574 6f72  )...total)1..tor
+00000c40: 6368 da17 7365 745f 6465 6661 756c 745f  ch..set_default_
+00000c50: 7465 6e73 6f72 5f74 7970 65da 0463 7564  tensor_type..cud
+00000c60: 61da 0c69 735f 6176 6169 6c61 626c 65da  a..is_available.
+00000c70: 0b46 6c6f 6174 5465 6e73 6f72 da04 6f70  .FloatTensor..op
+00000c80: 656e da02 6f73 da04 7061 7468 da04 6a6f  en..os..path..jo
+00000c90: 696e da09 7370 6c69 745f 6469 72da 046a  in..split_dir..j
+00000ca0: 736f 6eda 046c 6f61 6472 0a00 0000 da05  son..loadr......
+00000cb0: 7472 6169 6eda 0576 616c 7565 da08 726f  train..value..ro
+00000cc0: 6f74 5f64 6972 720d 0000 00da 066b 6474  ot_dirr......kdt
+00000cd0: 7265 65da 086d 6574 6164 6174 6172 0c00  ree..metadatar..
+00000ce0: 0000 da0e 636f 756e 7465 7266 6163 7475  ....counterfactu
+00000cf0: 616c da08 6d61 6b65 6469 7273 da06 6578  al..makedirs..ex
+00000d00: 6973 7473 da0c 6275 696c 645f 6b64 7472  ists..build_kdtr
+00000d10: 6565 da05 6d6f 6465 6cda 0570 7269 6e74  ee..model..print
+00000d20: da0d 6368 616e 6e65 6c5f 6e61 6d65 73da  ..channel_names.
+00000d30: 0572 616e 6765 da03 6c65 6eda 1367 656e  .range..len..gen
+00000d40: 6572 6174 655f 7061 7463 685f 7061 7468  erate_patch_path
+00000d50: da04 696c 6f63 720b 0000 0072 2500 0000  ..ilocr....r%...
+00000d60: da0a 6c61 6265 6c5f 6e61 6d65 da06 7370  ..label_name..sp
+00000d70: 6c69 7473 7205 0000 00da 116c 6f61 645f  litsr......load_
+00000d80: 7369 6e67 6c65 5f69 6d61 6765 da06 6170  single_image..ap
+00000d90: 7065 6e64 da04 6475 6d70 da03 7261 79da  pend..dump..ray.
+00000da0: 0873 6875 7464 6f77 6eda 0469 6e69 745a  .shutdown..initZ
+00000db0: 1361 7661 696c 6162 6c65 5f72 6573 6f75  .available_resou
+00000dc0: 7263 6573 7203 0000 00da 0477 6169 74da  rcesr......wait.
+00000dd0: 0665 7874 656e 64da 0367 6574 da06 7570  .extend..get..up
+00000de0: 6461 7465 da0f 6765 6e65 7261 7465 5f6f  date..generate_o
+00000df0: 6e65 5f63 6629 1e72 1100 0000 7212 0000  ne_cf).r....r...
+00000e00: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000e10: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00000e20: 1900 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
+00000e30: 0000 0072 1d00 0000 721e 0000 005a 096a  ...r....r....Z.j
+00000e40: 736f 6e5f 6669 6c65 da14 6e6f 726d 616c  son_file..normal
+00000e50: 697a 6174 696f 6e5f 7061 7261 6d73 7224  ization_paramsr$
+00000e60: 0000 0072 2000 0000 5a0a 696d 6167 655f  ...r ...Z.image_
+00000e70: 6172 6773 da01 69da 0869 6d67 5f70 6174  args..i..img_pat
+00000e80: 68da 0369 6d67 7225 0000 0072 2600 0000  h..imgr%...r&...
+00000e90: 5a08 6e75 6d5f 6370 7573 5a07 6366 5f72  Z.num_cpusZ.cf_r
+00000ea0: 6566 73da 0470 6261 72da 0772 6573 756c  efs..pbar..resul
+00000eb0: 7473 5a09 646f 6e65 5f72 6566 7372 3000  tsZ.done_refsr0.
+00000ec0: 0000 722c 0000 0072 3100 0000 7232 0000  ..r,...r1...r2..
+00000ed0: 00da 1267 6574 5f63 6f75 6e74 6572 6661  ...get_counterfa
+00000ee0: 6374 7561 6c1b 0000 0073 9c00 0000 0022  ctual....s....."
+00000ef0: 0401 16ff 0405 0201 0eff 0402 0201 0a01  ................
+00000f00: 0801 2603 0801 1401 0801 1401 0801 0603  ..&.............
+00000f10: 0801 0601 0aff 0403 0e03 0e01 1201 0806  ................
+00000f20: 0201 0201 0401 0201 0201 0201 0201 0201  ................
+00000f30: 0201 0201 0201 02f4 0610 0401 1001 0401  ................
+00000f40: 1001 0e01 10fd 0605 0e01 1201 0402 0201  ................
+00000f50: 0201 02fd 04ff 081a 1601 0402 0201 0201  ................
+00000f60: 0201 02fc 0406 02f9 240b 0a02 0801 0803  ........$.......
+00000f70: 0c01 0e03 0a02 02fe 0606 1002 0401 0601  ................
+00000f80: 0e01 1001 3203 0a14 1401 7264 0000 0063  ....2.....rd...c
+00000f90: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000fa0: 0400 0000 4300 0000 7318 0000 0074 00a0  ....C...s....t..
+00000fb0: 0164 01a1 0101 0074 0266 0069 007c 00a4  .d.....t.f.i.|..
+00000fc0: 018e 0153 0029 024e 7206 0000 0029 0372  ...S.).Nr....).r
+00000fd0: 3500 0000 da0f 7365 745f 6e75 6d5f 7468  5.....set_num_th
+00000fe0: 7265 6164 7372 5d00 0000 2901 5a0d 636f  readsr]...).Z.co
+00000ff0: 6d62 696e 6564 5f61 7267 7372 2c00 0000  mbined_argsr,...
+00001000: 722c 0000 0072 3200 0000 722d 0000 00d0  r,...r2...r-....
+00001010: 0000 0073 0400 0000 0002 0a01 722d 0000  ...s........r-..
+00001020: 0029 1072 2800 0000 7229 0000 0072 2500  .).r(...r)...r%.
+00001030: 0000 7212 0000 0072 1300 0000 7223 0000  ..r....r....r#..
+00001040: 0072 1400 0000 7224 0000 0072 2000 0000  .r....r$...r ...
+00001050: 7218 0000 0072 1c00 0000 7215 0000 0072  r....r....r....r
+00001060: 1900 0000 7217 0000 0072 1e00 0000 da06  ....r....r......
+00001070: 7265 7475 726e 630f 0000 0000 0000 0000  returnc.........
+00001080: 0000 0020 0000 0007 0000 0003 0000 0073  ... ...........s
+00001090: 1803 0000 7400 7c04 8301 8902 7401 a002  ....t.|.....t...
+000010a0: 8804 a101 a003 a100 7401 a002 8803 a101  ........t.......
+000010b0: a003 a100 0200 8904 8903 7c00 6a04 5c03  ..........|.j.\.
+000010c0: 7d0f 7d10 7d11 7401 a005 7c00 a006 a100  }.}.}.t...|.....
+000010d0: a101 a003 a100 a007 7c0e a101 7d00 7c00  ........|...}.|.
+000010e0: 8803 1800 8804 1b00 7d00 7401 6a02 7c01  ........}.t.j.|.
+000010f0: 6701 7401 6a08 6401 8d02 7d01 7401 6a09  g.t.j.d...}.t.j.
+00001100: 7c00 6402 6403 8d02 7d12 7401 6a0a a00b  |.d.d...}.t.j...
+00001110: a100 72a8 7c00 a00a a100 7d00 7c01 a00a  ..r.|.....}.|...
+00001120: a100 7d01 7c12 a00a a100 7d12 8804 a00a  ..}.|.....}.....
+00001130: a100 8904 8803 a00a a100 8903 8802 6a0c  ..............j.
+00001140: 6404 6b02 72b6 7c12 7d00 7c12 8804 1400  d.k.r.|.}.|.....
+00001150: 8803 1700 8905 8802 6a0c 6404 6b02 72e2  ........j.d.k.r.
+00001160: 8702 6601 6405 6406 8408 8900 6407 6406  ..f.d.d.....d.d.
+00001170: 8400 7d13 6e38 7c00 6408 6408 6408 8502  ..}.n8|.d.d.d...
+00001180: 6602 1900 8804 1400 8803 1700 8906 8703  f...............
+00001190: 8704 8705 8706 6604 6409 6406 8408 7d14  ......f.d.d...}.
+000011a0: 740d 7c14 8802 8302 5c02 8900 7d13 740e  t.|.....\...}.t.
+000011b0: a00f 8701 6601 640a 640b 8408 7c05 4400  ....f.d.d...|.D.
+000011c0: 8301 a101 7d15 7401 a010 8803 0b00 8804  ....}.t.........
+000011d0: 1b00 7401 a011 7c11 a101 640c 1400 a102  ..t...|...d.....
+000011e0: 7401 a011 7c11 a101 640d 1400 6602 7d16  t...|...d...f.}.
+000011f0: 7c12 7c15 0f00 1900 7412 1800 7c16 640e  |.|.....t...|.d.
+00001200: 1900 7c15 0f00 3c00 7c12 7c15 0f00 1900  ..|...<.|.|.....
+00001210: 7412 1700 7c16 640f 1900 7c15 0f00 3c00  t...|.d...|...<.
+00001220: 8700 6601 6410 6406 8408 7d17 6411 7c12  ..f.d.d...}.d.|.
+00001230: 6a04 1700 7d18 7413 7c17 7c13 7c18 6603  j...}.t.|.|.|.f.
+00001240: 7c16 7c09 7c0a 7c0e 6412 9c04 7c0b a401  |.|.|.|.d...|...
+00001250: 8e01 7d19 7c19 a014 a100 0100 7c19 6a15  ..}.|.......|.j.
+00001260: 7c12 6408 6408 6408 8502 6602 1900 7c01  |.d.d.d...f...|.
+00001270: 6408 6408 6408 8502 6602 1900 7c03 6701  d.d.d...f...|.g.
+00001280: 6413 8d03 7d1a 7c1a 6a16 6408 7501 9003  d...}.|.j.d.u...
+00001290: 7214 7c1a 6a16 6414 1900 640e 1900 7d1b  r.|.j.d...d...}.
+000012a0: 7c0a 640e 6b04 9002 7224 7417 6415 7c1b  |.d.k...r$t.d.|.
+000012b0: 9b00 9d02 8301 0100 7c1a 6a16 6416 1900  ........|.j.d...
+000012c0: 640e 1900 7d19 7c13 7401 a005 7c19 6408  d...}.|.t...|.d.
+000012d0: 6408 6408 8502 6602 1900 a101 a007 7c0e  d.d...f.......|.
+000012e0: a101 8301 7d19 7401 a018 7c19 6417 a102  ....}.t...|.d...
+000012f0: 7d19 7419 7c19 8804 1400 8803 1700 7c19  }.t.|.........|.
+00001300: 6a1a 640f 1800 6418 8d02 7d1c 7c12 8804  j.d...d...}.|...
+00001310: 1400 8803 1700 7d00 7c1c 7c00 1800 7c00  ......}.|.|...|.
+00001320: 1b00 6419 1400 7d1d 741b 741c 740e a00f  ..d...}.t.t.t...
+00001330: 7c05 a101 7c15 1900 7c1d 7c15 1900 a01d  |...|...|.|.....
+00001340: a100 a01e a100 8302 8301 7d1e 7c0a 640e  ..........}.|.d.
+00001350: 6b04 9002 72d0 7417 641a 7c1e 9b00 9d02  k...r.t.d.|.....
+00001360: 8301 0100 7c0c 6408 7501 9003 7210 741f  ....|.d.u...r.t.
+00001370: 6a20 7c0c 641b 641c 8d02 0100 741f 6a21  j |.d.d.....t.j!
+00001380: a022 7c0c 641d 7c02 9b00 641e 9d03 a102  ."|.d.|...d.....
+00001390: 7d1f 740e 6a23 7c1f 7c1c 7c1b 7c1e 641f  }.t.j#|.|.|.|.d.
+000013a0: 8d04 0100 7c1e 5300 6408 5300 2920 619a  ....|.S.d.S.) a.
+000013b0: 0300 000a 2020 2020 4765 6e65 7261 7465  ....    Generate
+000013c0: 2063 6f75 6e74 6572 6661 6374 7561 6c73   counterfactuals
+000013d0: 2066 6f72 2061 2067 6976 656e 2069 6d61   for a given ima
+000013e0: 6765 2070 6174 6368 2e0a 0a20 2020 2041  ge patch...    A
+000013f0: 7267 733a 0a20 2020 2020 2020 2020 6f72  rgs:.         or
+00001400: 6967 696e 616c 5f70 6174 6368 2028 6e70  iginal_patch (np
+00001410: 2e6e 6461 7272 6179 293a 204f 7269 6769  .ndarray): Origi
+00001420: 6e61 6c20 7061 7463 6820 746f 2062 6520  nal patch to be 
+00001430: 6578 706c 6169 6e65 642e 0a20 2020 2020  explained..     
+00001440: 2020 2020 6f72 6967 696e 616c 5f63 6c61      original_cla
+00001450: 7373 2028 6e70 2e6e 6461 7272 6179 293a  ss (np.ndarray):
+00001460: 204f 7269 6769 6e61 6c20 6c61 6265 6c20   Original label 
+00001470: 6f66 2074 6865 2070 6174 6368 2e0a 2020  of the patch..  
+00001480: 2020 2020 2020 206d 6f64 656c 2028 746f         model (to
+00001490: 7263 682e 6e6e 2e4d 6f64 756c 6529 3a20  rch.nn.Module): 
+000014a0: 4d6f 6465 6c20 746f 2062 6520 6578 706c  Model to be expl
+000014b0: 6169 6e65 642e 0a20 2020 2020 2020 2020  ained..         
+000014c0: 6368 616e 6e65 6c5f 746f 5f70 6572 7475  channel_to_pertu
+000014d0: 7262 2028 6c69 7374 293a 204c 6973 7420  rb (list): List 
+000014e0: 6f66 2063 6861 6e6e 656c 7320 746f 2070  of channels to p
+000014f0: 6572 7475 7262 2e0a 2020 2020 2020 2020  erturb..        
+00001500: 206e 6f72 6d61 6c69 7a61 7469 6f6e 5f70   normalization_p
+00001510: 6172 616d 7320 2864 6963 7429 3a20 4469  arams (dict): Di
+00001520: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
+00001530: 696e 6720 7468 6520 6d65 616e 2061 6e64  ing the mean and
+00001540: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
+00001550: 696f 6e20 6f66 2065 6163 6820 6368 616e  ion of each chan
+00001560: 6e65 6c2e 0a20 2020 2020 2020 2020 7472  nel..         tr
+00001570: 6169 6e5f 6461 7461 2028 7374 722c 206f  ain_data (str, o
+00001580: 7074 696f 6e61 6c29 3a20 5061 7468 2074  ptional): Path t
+00001590: 6f20 7468 6520 7472 6169 6e69 6e67 2064  o the training d
+000015a0: 6174 612e 2044 6566 6175 6c74 7320 746f  ata. Defaults to
+000015b0: 204e 6f6e 652e 0a20 2020 2020 2020 2020   None..         
+000015c0: 6f70 7469 6d69 7a61 7469 6f6e 5f70 6172  optimization_par
+000015d0: 616d 7320 2864 6963 742c 206f 7074 696f  ams (dict, optio
+000015e0: 6e61 6c29 3a20 4469 6374 696f 6e61 7279  nal): Dictionary
+000015f0: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00001600: 7061 7261 6d65 7465 7273 2066 6f72 2074  parameters for t
+00001610: 6865 206f 7074 696d 697a 6174 696f 6e2e  he optimization.
+00001620: 2044 6566 6175 6c74 7320 746f 207b 7d2e   Defaults to {}.
+00001630: 0a20 2020 2020 2020 2020 7361 7665 5f64  .         save_d
+00001640: 6972 2028 7374 722c 206f 7074 696f 6e61  ir (str, optiona
+00001650: 6c29 3a20 4469 7265 6374 6f72 7920 7768  l): Directory wh
+00001660: 6572 6520 6f75 7470 7574 2077 696c 6c20  ere output will 
+00001670: 6265 2073 6176 6564 2e20 4465 6661 756c  be saved. Defaul
+00001680: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
+00001690: 2020 2020 2070 6174 6368 5f69 6420 2869       patch_id (i
+000016a0: 6e74 2c20 6f70 7469 6f6e 616c 293a 2050  nt, optional): P
+000016b0: 6174 6368 2049 442e 2044 6566 6175 6c74  atch ID. Default
+000016c0: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
+000016d0: 2020 2020 7468 7265 7368 6f6c 6420 2866      threshold (f
+000016e0: 6c6f 6174 2c20 6f70 7469 6f6e 616c 293a  loat, optional):
+000016f0: 2054 6872 6573 686f 6c64 2066 6f72 2074   Threshold for t
+00001700: 6865 2070 7265 6469 6374 696f 6e20 7072  he prediction pr
+00001710: 6f62 6162 696c 6974 792e 2044 6566 6175  obability. Defau
+00001720: 6c74 7320 746f 2030 2e35 2e0a 0a20 2020  lts to 0.5...   
+00001730: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00001740: 2020 2020 4e6f 6e65 0a20 2020 2072 0e00      None.    r..
+00001750: 0000 2902 7201 0000 0072 0600 0000 a901  ..).r....r......
+00001760: da03 6469 6dda 036d 6c70 6301 0000 0000  ..dim..mlpc.....
+00001770: 0000 0000 0000 0001 0000 0004 0000 0013  ................
+00001780: 0000 0073 1600 0000 7400 6a01 6a02 6a03  ...s....t.j.j.j.
+00001790: 8800 7c00 8301 6401 6402 8d02 5300 2903  ..|...d.d...S.).
+000017a0: 4e72 0600 0000 7267 0000 0029 0472 3500  Nr....rg...).r5.
+000017b0: 0000 da02 6e6e da0a 6675 6e63 7469 6f6e  ....nn..function
+000017c0: 616c da07 736f 6674 6d61 78a9 01da 0178  al..softmax....x
+000017d0: 2901 724a 0000 0072 2c00 0000 7232 0000  ).rJ...r,...r2..
+000017e0: 00da 083c 6c61 6d62 6461 3e15 0100 00f3  ...<lambda>.....
+000017f0: 0000 0000 7a21 6765 6e65 7261 7465 5f6f  ....z!generate_o
+00001800: 6e65 5f63 662e 3c6c 6f63 616c 733e 2e3c  ne_cf.<locals>.<
+00001810: 6c61 6d62 6461 3e63 0100 0000 0000 0000  lambda>c........
+00001820: 0000 0000 0100 0000 0100 0000 5300 0000  ............S...
+00001830: 7304 0000 007c 0053 00a9 014e 722c 0000  s....|.S...Nr,..
+00001840: 0072 6d00 0000 722c 0000 0072 2c00 0000  .rm...r,...r,...
+00001850: 7232 0000 0072 6f00 0000 1601 0000 7270  r2...ro.......rp
+00001860: 0000 004e 6301 0000 0000 0000 0000 0000  ...Nc...........
+00001870: 0001 0000 0006 0000 0013 0000 0073 1000  .............s..
+00001880: 0000 7400 7c00 8803 8800 8801 8802 8305  ..t.|...........
+00001890: 5300 7271 0000 0029 01da 0b61 6c74 6572  S.rq...)...alter
+000018a0: 5f69 6d61 6765 2901 da01 7929 0472 2400  _image)...y).r$.
+000018b0: 0000 7220 0000 00da 0d75 6e6e 6f72 6d65  ..r .....unnorme
+000018c0: 645f 6d65 616e da0e 756e 6e6f 726d 6564  d_mean..unnormed
+000018d0: 5f70 6174 6368 722c 0000 0072 3200 0000  _patchr,...r2...
+000018e0: 726f 0000 0019 0100 0072 7000 0000 6301  ro.......rp...c.
+000018f0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001900: 0000 0013 0000 0073 1c00 0000 6700 7c00  .......s....g.|.
+00001910: 5d14 7d01 7c01 8800 7600 7214 6400 6e02  ].}.|...v.r.d.n.
+00001920: 6401 9102 7104 5300 2902 5446 722c 0000  d...q.S.).TFr,..
+00001930: 0029 0272 2f00 0000 da04 6e61 6d65 2901  .).r/.....name).
+00001940: 7214 0000 0072 2c00 0000 7232 0000 0072  r....r,...r2...r
+00001950: 3300 0000 1e01 0000 7270 0000 007a 2367  3.......rp...z#g
+00001960: 656e 6572 6174 655f 6f6e 655f 6366 2e3c  enerate_one_cf.<
+00001970: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00001980: 703e e9fc ffff ffe9 0400 0000 7201 0000  p>..........r...
+00001990: 0072 0600 0000 6301 0000 0000 0000 0000  .r....c.........
+000019a0: 0000 0001 0000 0002 0000 0013 0000 0073  ...............s
+000019b0: 0800 0000 8800 7c00 8301 5300 7271 0000  ......|...S.rq..
+000019c0: 0072 2c00 0000 726d 0000 0029 01da 0d61  .r,...rm...)...a
+000019d0: 6c74 6572 6564 5f6d 6f64 656c 722c 0000  ltered_modelr,..
+000019e0: 0072 3200 0000 726f 0000 0028 0100 0072  .r2...ro...(...r
+000019f0: 7000 0000 2901 7206 0000 0029 04da 0d66  p...).r....)...f
+00001a00: 6561 7475 7265 5f72 616e 6765 5a0a 7472  eature_rangeZ.tr
+00001a10: 7573 7473 636f 7265 721c 0000 0072 1e00  ustscorer....r..
+00001a20: 0000 2903 da01 58da 0159 7212 0000 00da  ..)...X..Yr.....
+00001a30: 0570 726f 6261 7a1c 436f 756e 7465 7266  .probaz.Counterf
+00001a40: 6163 7475 616c 2070 726f 6261 6269 6c69  actual probabili
+00001a50: 7479 3a20 727b 0000 0029 0472 0100 0000  ty: r{...).r....
+00001a60: 7204 0000 00e9 0300 0000 7206 0000 00a9  r.........r.....
+00001a70: 01da 0c70 7265 7365 7276 6541 7869 73e9  ...preserveAxis.
+00001a80: 6400 0000 7a12 6366 2070 6572 7475 7262  d...z.cf perturb
+00001a90: 6564 2028 2529 3a20 5472 2100 0000 5a06  ed (%): Tr!...Z.
+00001aa0: 7061 7463 685f 7a04 2e6e 707a 2903 da02  patch_z..npz)...
+00001ab0: 6366 727d 0000 005a 1364 656c 7461 5f69  cfr}...Z.delta_i
+00001ac0: 6e5f 7065 7263 656e 7461 6765 2924 7208  n_percentage)$r.
+00001ad0: 0000 0072 3500 0000 da06 7465 6e73 6f72  ...r5.....tensor
+00001ae0: da05 666c 6f61 74da 0573 6861 7065 da0a  ..float..shape..
+00001af0: 6672 6f6d 5f6e 756d 7079 da04 636f 7079  from_numpy..copy
+00001b00: da02 746f da05 696e 7436 3472 1f00 0000  ..to..int64r....
+00001b10: 7237 0000 0072 3800 0000 da04 6172 6368  r7...r8.....arch
+00001b20: da0e 6164 645f 696e 6974 5f6c 6179 6572  ..add_init_layer
+00001b30: da02 6e70 da05 6172 7261 79da 076d 6178  ..np..array..max
+00001b40: 696d 756d da04 6f6e 6573 da07 4550 5349  imum..ones..EPSI
+00001b50: 4c4f 4e72 0700 0000 da03 6669 74da 0765  LONr......fit..e
+00001b60: 7870 6c61 696e 7282 0000 0072 4b00 0000  xplainr....rK...
+00001b70: da07 7065 726d 7574 65da 186d 6561 6e5f  ..permute..mean_
+00001b80: 7072 6573 6572 7665 5f64 696d 656e 7369  preserve_dimensi
+00001b90: 6f6e 73da 046e 6469 6dda 0464 6963 74da  ons..ndim..dict.
+00001ba0: 037a 6970 da03 6370 75da 056e 756d 7079  .zip..cpu..numpy
+00001bb0: 723b 0000 0072 4700 0000 723c 0000 0072  r;...rG...r<...r
+00001bc0: 3d00 0000 da05 7361 7665 7a29 2072 2800  =.....savez) r(.
+00001bd0: 0000 7229 0000 0072 2500 0000 7212 0000  ..r)...r%...r...
+00001be0: 0072 1300 0000 7223 0000 0072 1400 0000  .r....r#...r....
+00001bf0: 7224 0000 0072 2000 0000 7218 0000 0072  r$...r ...r....r
+00001c00: 1c00 0000 7215 0000 0072 1900 0000 7217  ....r....r....r.
+00001c10: 0000 0072 1e00 0000 da01 48da 015f da01  ...r......H.._..
+00001c20: 435a 0658 5f6d 6561 6eda 0f69 6e70 7574  CZ.X_mean..input
+00001c30: 5f74 7261 6e73 666f 726d da08 696e 6974  _transform..init
+00001c40: 5f66 756e 5a0c 6973 5f70 6572 7475 7262  _funZ.is_perturb
+00001c50: 6564 727a 0000 005a 0a70 7265 6469 6374  edrz...Z.predict
+00001c60: 5f66 6e72 8500 0000 7282 0000 00da 0b65  _fnr....r......e
+00001c70: 7870 6c61 6e61 7469 6f6e 5a07 6366 5f70  xplanationZ.cf_p
+00001c80: 726f 625a 0b58 5f70 6572 7475 7262 6564  robZ.X_perturbed
+00001c90: 5a08 6366 5f64 656c 7461 5a0d 7065 7263  Z.cf_deltaZ.perc
+00001ca0: 656e 745f 6465 6c74 615a 0a73 6176 6564  ent_deltaZ.saved
+00001cb0: 5f66 696c 6572 2c00 0000 2907 7279 0000  _filer,...).ry..
+00001cc0: 0072 1400 0000 724a 0000 0072 2400 0000  .r....rJ...r$...
+00001cd0: 7220 0000 0072 7400 0000 7275 0000 0072  r ...rt...ru...r
+00001ce0: 3200 0000 725d 0000 00d6 0000 0073 a000  2...r].......s..
+00001cf0: 0000 0024 0804 0c01 0cfe 0604 0c01 1801  ...$............
+00001d00: 0c01 1201 0e03 0a01 0801 0801 0801 0801  ................
+00001d10: 0802 0a01 0403 0c01 0a01 0c01 0a02 1801  ................
+00001d20: 1201 0e03 0401 10ff 0404 1a01 0cfe 0404  ................
+00001d30: 1801 1803 0c03 0a01 0201 0201 0201 02fd  ................
+00001d40: 0204 0201 0201 0201 02f9 0408 02f8 060a  ................
+00001d50: 0803 0401 20ff 0604 0c01 0e01 0a01 0e02  .... ...........
+00001d60: 0e01 2001 0c02 0201 12ff 0603 0c01 1001  .. .............
+00001d70: 0201 0201 0c01 0efe 02ff 0406 0a01 0e02  ................
+00001d80: 0a01 0e01 1601 0401 0201 0201 0201 02fc  ................
+00001d90: 0606 725d 0000 0029 0572 1b00 0000 724a  ..r]...).r....rJ
+00001da0: 0000 0072 2400 0000 7220 0000 0072 1d00  ...r$...r ...r..
+00001db0: 0000 6306 0000 0000 0000 0000 0000 000b  ..c.............
+00001dc0: 0000 0006 0000 0043 0000 0073 b400 0000  .......C...s....
+00001dd0: 7400 7c01 8301 7d06 7401 a002 7c06 7403  t.|...}.t...|.t.
+00001de0: a004 7c03 a101 1800 7403 a004 7c04 a101  ..|.....t...|...
+00001df0: 1b00 a101 a005 a100 7d06 7c02 6a06 6401  ........}.|.j.d.
+00001e00: 6b02 7242 7401 a007 7c06 6402 a102 7d07  k.rBt...|.d...}.
+00001e10: 6e0c 7401 a008 7c06 6403 a102 7d07 7c02  n.t...|.d...}.|.
+00001e20: 7c07 8301 a009 a100 a00a a100 7d08 7403  |...........}.t.
+00001e30: 6a0b 7c08 6404 6405 8d02 7d09 7c05 6400  j.|.d.d...}.|.d.
+00001e40: 7501 7284 740c 6600 6900 7c05 a401 8e01  u.r.t.f.i.|.....
+00001e50: 7d0a 6e06 740c 8300 7d0a 7401 a007 7c06  }.n.t...}.t...|.
+00001e60: 6402 a102 7d06 7c0a 6a0d 7c06 7c09 6406  d...}.|.j.|.|.d.
+00001e70: 6407 8d03 0100 740e 7c0a 7c00 8302 0100  d.....t.|.|.....
+00001e80: 6400 5300 2908 4e72 6900 0000 2902 7206  d.S.).Nri...).r.
+00001e90: 0000 0072 0400 0000 a904 7201 0000 0072  ...r......r....r
+00001ea0: 7e00 0000 7206 0000 0072 0400 0000 7206  ~...r....r....r.
+00001eb0: 0000 00a9 01da 0461 7869 7372 0400 0000  .......axisr....
+00001ec0: 2901 da07 636c 6173 7365 7329 0fda 176c  )...classes)...l
+00001ed0: 6f61 645f 6e70 795f 6669 6c65 735f 746f  oad_npy_files_to
+00001ee0: 5f61 7272 6179 7235 0000 0072 8600 0000  _arrayr5...r....
+00001ef0: 728c 0000 0072 8d00 0000 7284 0000 0072  r....r....r....r
+00001f00: 8a00 0000 721f 0000 0072 9300 0000 da06  ....r....r......
+00001f10: 6465 7461 6368 7299 0000 00da 0661 7267  detachr......arg
+00001f20: 6d61 7872 0900 0000 7291 0000 00da 0b73  maxr....r......s
+00001f30: 6176 655f 6f62 6a65 6374 290b 7218 0000  ave_object).r...
+00001f40: 0072 1b00 0000 724a 0000 0072 2400 0000  .r....rJ...r$...
+00001f50: 7220 0000 0072 1d00 0000 5a0b 7472 6169  r ...r....Z.trai
+00001f60: 6e5f 7061 7463 685a 0358 5f74 5a09 6d6f  n_patchZ.X_tZ.mo
+00001f70: 6465 6c5f 6f75 74da 0570 7265 6473 da02  del_out..preds..
+00001f80: 7473 722c 0000 0072 2c00 0000 7232 0000  tsr,...r,...r2..
+00001f90: 0072 4900 0000 6001 0000 731e 0000 0000  .rI...`...s.....
+00001fa0: 0808 0104 0116 ff08 030a 010e 020c 0210  ................
+00001fb0: 010e 0208 0110 0206 010c 0110 0172 4900  .............rI.
+00001fc0: 0000 6301 0000 0000 0000 0000 0000 0009  ..c.............
+00001fd0: 0000 0006 0000 0043 0000 0073 7200 0000  .......C...sr...
+00001fe0: 6700 7d01 6401 6402 6702 7d02 7c02 4400  g.}.d.d.g.}.|.D.
+00001ff0: 5d4e 7d03 7400 6a01 a002 7c00 7c03 a102  ]N}.t.j...|.|...
+00002000: 7d04 7400 a003 7c04 a101 4400 5d30 7d05  }.t...|...D.]0}.
+00002010: 7c05 a004 6403 a101 722c 7400 6a01 a002  |...d...r,t.j...
+00002020: 7c04 7c05 a102 7d06 7405 a006 7c06 a101  |.|...}.t...|...
+00002030: 7d07 7c01 a007 7c07 a101 0100 712c 7110  }.|...|.....q,q.
+00002040: 7405 6a08 7c01 6404 6405 8d02 7d08 7c08  t.j.|.d.d...}.|.
+00002050: 5300 2906 4eda 0130 da01 317a 042e 6e70  S.).N..0..1z..np
+00002060: 7972 0100 0000 72a2 0000 0029 0972 3b00  yr....r....).r;.
+00002070: 0000 723c 0000 0072 3d00 0000 da07 6c69  ..r<...r=.....li
+00002080: 7374 6469 72da 0865 6e64 7377 6974 6872  stdir..endswithr
+00002090: 8c00 0000 7240 0000 0072 5400 0000 da05  ....r@...rT.....
+000020a0: 7374 6163 6b29 09da 0862 6173 655f 6469  stack)...base_di
+000020b0: 72da 0661 7272 6179 735a 0873 7562 5f64  r..arraysZ.sub_d
+000020c0: 6972 73da 0773 7562 5f64 6972 5a0c 7375  irs..sub_dirZ.su
+000020d0: 625f 6469 725f 7061 7468 da04 6669 6c65  b_dir_path..file
+000020e0: da09 6669 6c65 5f70 6174 6872 8d00 0000  ..file_pathr....
+000020f0: 5a0b 6669 6e61 6c5f 6172 7261 7972 2c00  Z.final_arrayr,.
+00002100: 0000 722c 0000 0072 3200 0000 72a5 0000  ..r,...r2...r...
+00002110: 007d 0100 0073 1600 0000 0001 0401 0802  .}...s..........
+00002120: 0801 0e01 0e01 0a01 0e01 0a01 0e03 0e01  ................
+00002130: 72a5 0000 0063 0500 0000 0000 0000 0000  r....c..........
+00002140: 0000 0700 0000 0700 0000 4300 0000 7338  ..........C...s8
+00002150: 0000 007c 007c 0314 007c 0217 007d 057c  ...|.|...|...}.|
+00002160: 017c 057c 041b 0064 0064 0085 0264 0064  .|.|...d.d...d.d
+00002170: 0064 0064 0085 0266 0419 0014 007d 067c  .d.d...f.....}.|
+00002180: 067c 0218 007c 031b 0053 0072 7100 0000  .|...|...S.rq...
+00002190: 722c 0000 0029 0772 7300 0000 7275 0000  r,...).rs...ru..
+000021a0: 0072 2400 0000 7220 0000 0072 7400 0000  .r$...r ...rt...
+000021b0: 5a0a 756e 6e6f 726d 6564 5f79 5a09 6e65  Z.unnormed_yZ.ne
+000021c0: 775f 7061 7463 6872 2c00 0000 722c 0000  w_patchr,...r,..
+000021d0: 0072 3200 0000 7272 0000 008e 0100 0073  .r2...rr.......s
+000021e0: 0600 0000 0001 0c01 2001 7272 0000 0063  ........ .rr...c
+000021f0: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+00002200: 0400 0000 0300 0000 7334 0000 0047 0087  ........s4...G..
+00002210: 0066 0164 0164 0284 0864 0274 006a 016a  .f.d.d...d.t.j.j
+00002220: 0283 037d 027c 0283 007d 0374 006a 01a0  ...}.|...}.t.j..
+00002230: 037c 037c 01a1 027d 047c 047c 0366 0253  .|.|...}.|.|.f.S
+00002240: 0029 0361 1601 0000 0a20 2020 2041 6464  .).a.....    Add
+00002250: 2061 6e20 696e 6974 6961 6c69 7a61 7469   an initializati
+00002260: 6f6e 206c 6179 6572 2074 6f20 7468 6520  on layer to the 
+00002270: 6d6f 6465 6c2e 0a0a 2020 2020 4172 6773  model...    Args
+00002280: 3a0a 2020 2020 2020 2020 696e 6974 5f66  :.        init_f
+00002290: 756e 2028 6361 6c6c 6162 6c65 293a 2049  un (callable): I
+000022a0: 6e69 7469 616c 697a 6174 696f 6e20 6675  nitialization fu
+000022b0: 6e63 7469 6f6e 2e0a 2020 2020 2020 2020  nction..        
+000022c0: 6d6f 6465 6c20 2874 6f72 6368 2e6e 6e2e  model (torch.nn.
+000022d0: 4d6f 6475 6c65 293a 204f 7269 6769 6e61  Module): Origina
+000022e0: 6c20 6d6f 6465 6c2e 0a0a 2020 2020 5265  l model...    Re
+000022f0: 7475 726e 733a 0a20 2020 2020 2020 2074  turns:.        t
+00002300: 7570 6c65 3a20 2874 6f72 6368 2e6e 6e2e  uple: (torch.nn.
+00002310: 4d6f 6475 6c65 2c20 746f 7263 682e 6e6e  Module, torch.nn
+00002320: 2e4d 6f64 756c 6529 202d 204d 6f64 6966  .Module) - Modif
+00002330: 6965 6420 6d6f 6465 6c20 616e 6420 696e  ied model and in
+00002340: 7075 7420 7472 616e 7366 6f72 6d61 7469  put transformati
+00002350: 6f6e 206c 6179 6572 2e0a 2020 2020 6300  on layer..    c.
+00002360: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00002370: 0000 0000 0000 0073 1800 0000 6500 5a01  .......s....e.Z.
+00002380: 6400 5a02 8700 6601 6401 6402 8408 5a03  d.Z...f.d.d...Z.
+00002390: 6403 5300 2904 7a20 6164 645f 696e 6974  d.S.).z add_init
+000023a0: 5f6c 6179 6572 2e3c 6c6f 6361 6c73 3e2e  _layer.<locals>.
+000023b0: 496e 7075 7446 756e 6302 0000 0000 0000  InputFunc.......
+000023c0: 0000 0000 0002 0000 0004 0000 0013 0000  ................
+000023d0: 0073 1400 0000 7400 a001 8800 7c01 8301  .s....t.....|...
+000023e0: 6401 a102 a002 a100 5300 2902 4e72 a100  d.......S.).Nr..
+000023f0: 0000 2903 7235 0000 0072 9300 0000 7284  ..).r5...r....r.
+00002400: 0000 0029 02da 0473 656c 66da 0569 6e70  ...)...self..inp
+00002410: 7574 a901 729f 0000 0072 2c00 0000 7232  ut..r....r,...r2
+00002420: 0000 00da 0766 6f72 7761 7264 a101 0000  .....forward....
+00002430: 7302 0000 0000 017a 2861 6464 5f69 6e69  s......z(add_ini
+00002440: 745f 6c61 7965 722e 3c6c 6f63 616c 733e  t_layer.<locals>
+00002450: 2e49 6e70 7574 4675 6e2e 666f 7277 6172  .InputFun.forwar
+00002460: 644e 2904 da08 5f5f 6e61 6d65 5f5f da0a  dN)...__name__..
+00002470: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00002480: 616c 6e61 6d65 5f5f 72b8 0000 0072 2c00  alname__r....r,.
+00002490: 0000 72b7 0000 0072 2c00 0000 7232 0000  ..r....r,...r2..
+000024a0: 00da 0849 6e70 7574 4675 6ea0 0100 0073  ...InputFun....s
+000024b0: 0200 0000 0801 72bc 0000 0029 0472 3500  ......r....).r5.
+000024c0: 0000 726a 0000 00da 064d 6f64 756c 65da  ..rj.....Module.
+000024d0: 0a53 6571 7565 6e74 6961 6c29 0572 9f00  .Sequential).r..
+000024e0: 0000 724a 0000 0072 bc00 0000 729e 0000  ..rJ...r....r...
+000024f0: 005a 0e63 6f6d 706c 6574 655f 6d6f 6465  .Z.complete_mode
+00002500: 6c72 2c00 0000 72b7 0000 0072 3200 0000  lr,...r....r2...
+00002510: 728b 0000 0094 0100 0073 0800 0000 000c  r........s......
+00002520: 1804 0601 0e01 728b 0000 0029 0372 8300  ......r....).r..
+00002530: 0000 7280 0000 0072 6600 0000 6302 0000  ..r....rf...c...
+00002540: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+00002550: 0003 0000 0073 3800 0000 7400 8800 7401  .....s8...t...t.
+00002560: 8302 7210 8800 6601 8900 8700 6601 6401  ..r...f.....f.d.
+00002570: 6402 8408 7402 7c00 6a03 8301 4400 8301  d...t.|.j...D...
+00002580: 7d02 7c00 6a04 7c02 6403 8d01 7d03 7c03  }.|.j.|.d...}.|.
+00002590: 5300 2904 6127 0100 000a 2020 2020 436f  S.).a'....    Co
+000025a0: 6d70 7574 6520 7468 6520 6d65 616e 2061  mpute the mean a
+000025b0: 6c6f 6e67 2061 6c6c 2064 696d 656e 7369  long all dimensi
+000025c0: 6f6e 7320 6578 6365 7074 2074 686f 7365  ons except those
+000025d0: 2073 7065 6369 6669 6564 2069 6e20 7072   specified in pr
+000025e0: 6573 6572 7665 4178 6973 2e0a 0a20 2020  eserveAxis...   
+000025f0: 2041 7267 733a 0a20 2020 2020 2020 2074   Args:.        t
+00002600: 656e 736f 7220 2874 6f72 6368 2e54 656e  ensor (torch.Ten
+00002610: 736f 7229 3a20 496e 7075 7420 7465 6e73  sor): Input tens
+00002620: 6f72 2e0a 2020 2020 2020 2020 7072 6573  or..        pres
+00002630: 6572 7665 4178 6973 2028 7475 706c 652c  erveAxis (tuple,
+00002640: 206f 7074 696f 6e61 6c29 3a20 4469 6d65   optional): Dime
+00002650: 6e73 696f 6e73 2074 6f20 7072 6573 6572  nsions to preser
+00002660: 7665 2e20 4465 6661 756c 7473 2074 6f20  ve. Defaults to 
+00002670: 4e6f 6e65 2e0a 0a20 2020 2052 6574 7572  None...    Retur
+00002680: 6e73 3a0a 2020 2020 2020 2020 746f 7263  ns:.        torc
+00002690: 682e 5465 6e73 6f72 3a20 5465 6e73 6f72  h.Tensor: Tensor
+000026a0: 2077 6974 6820 7072 6573 6572 7665 6420   with preserved 
+000026b0: 6469 6d65 6e73 696f 6e73 2e0a 2020 2020  dimensions..    
+000026c0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000026d0: 0004 0000 0013 0000 0073 1800 0000 6700  .........s....g.
+000026e0: 7c00 5d10 7d01 7c01 8800 7601 7204 7c01  |.].}.|...v.r.|.
+000026f0: 9102 7104 5300 722c 0000 0072 2c00 0000  ..q.S.r,...r,...
+00002700: 2902 722f 0000 0072 5f00 0000 727f 0000  ).r/...r_...r...
+00002710: 0072 2c00 0000 7232 0000 0072 3300 0000  .r,...r2...r3...
+00002720: b901 0000 7270 0000 007a 2c6d 6561 6e5f  ....rp...z,mean_
+00002730: 7072 6573 6572 7665 5f64 696d 656e 7369  preserve_dimensi
+00002740: 6f6e 732e 3c6c 6f63 616c 733e 2e3c 6c69  ons.<locals>.<li
+00002750: 7374 636f 6d70 3e72 6700 0000 2905 da0a  stcomp>rg...)...
+00002760: 6973 696e 7374 616e 6365 da03 696e 7472  isinstance..intr
+00002770: 4d00 0000 7295 0000 0072 1f00 0000 2904  M...r....r....).
+00002780: 7283 0000 0072 8000 0000 5a0e 6469 6d73  r....r....Z.dims
+00002790: 5f74 6f5f 7265 6475 6365 da06 7265 7375  _to_reduce..resu
+000027a0: 6c74 722c 0000 0072 7f00 0000 7232 0000  ltr,...r....r2..
+000027b0: 0072 9400 0000 a901 0000 730a 0000 0000  .r........s.....
+000027c0: 0d0a 0106 0218 010c 0172 9400 0000 6302  .........r....c.
+000027d0: 0000 0000 0000 0000 0000 0003 0000 0008  ................
+000027e0: 0000 0043 0000 0073 3c00 0000 7400 7c01  ...C...s<...t.|.
+000027f0: 6401 8302 8f1e 7d02 7401 a002 7c00 7c02  d.....}.t...|.|.
+00002800: 6402 a103 0100 5700 6400 0400 0400 8303  d.....W.d.......
+00002810: 0100 6e10 3100 732e 3000 0100 0100 0100  ..n.1.s.0.......
+00002820: 5900 0100 6400 5300 2903 4eda 0277 62e9  Y...d.S.).N..wb.
+00002830: ffff ffff 2903 723a 0000 00da 0670 6963  ....).r:.....pic
+00002840: 6b6c 6572 5500 0000 2903 da03 6f62 6ada  klerU...)...obj.
+00002850: 0866 696c 656e 616d 655a 046f 7574 7072  .filenameZ.outpr
+00002860: 2c00 0000 722c 0000 0072 3200 0000 72a8  ,...r,...r2...r.
+00002870: 0000 00be 0100 0073 0400 0000 0001 0c01  .......s........
+00002880: 72a8 0000 0029 094e 7210 0000 004e 4e72  r....).Nr....NNr
+00002890: 0600 0000 4e72 0100 0000 4e4e 2905 7201  ....Nr....NN).r.
+000028a0: 0000 004e 4e72 1000 0000 4e29 014e 2901  ...NNr....N).N).
+000028b0: 4e29 3372 3b00 0000 723f 0000 00da 075f  N)3r;...r?....._
+000028c0: 7069 636b 6c65 72c4 0000 0072 9900 0000  pickler....r....
+000028d0: 728c 0000 00da 0670 616e 6461 73da 0270  r......pandas..p
+000028e0: 64da 0674 7970 696e 6772 0200 0000 7235  d..typingr....r5
+000028f0: 0000 00da 0f6d 756c 7469 7072 6f63 6573  .....multiproces
+00002900: 7369 6e67 7256 0000 0072 0300 0000 da08  singrV...r......
+00002910: 6461 7461 7365 7473 7205 0000 0072 8200  datasetsr....r..
+00002920: 0000 7207 0000 00da 0e63 6c61 7373 6966  ..r......classif
+00002930: 6963 6174 696f 6e72 0800 0000 da0a 636f  icationr......co
+00002940: 6e66 6964 656e 6365 7209 0000 00da 0d63  nfidencer......c
+00002950: 6f6e 6669 6775 7261 7469 6f6e 720a 0000  onfigurationr...
+00002960: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00002970: 7283 0000 00da 0766 6c6f 6174 3332 7290  r......float32r.
+00002980: 0000 0072 c000 0000 da03 7374 72da 046c  ...r......str..l
+00002990: 6973 7472 9600 0000 da09 4461 7461 4672  istr......DataFr
+000029a0: 616d 6572 8400 0000 7264 0000 0072 2e00  amer....rd...r..
+000029b0: 0000 722d 0000 00da 076e 6461 7272 6179  ..r-.....ndarray
+000029c0: 725d 0000 0072 6a00 0000 72bd 0000 0072  r]...rj...r....r
+000029d0: 4900 0000 72a5 0000 0072 7200 0000 728b  I...r....rr...r.
+000029e0: 0000 00da 0654 656e 736f 72da 0574 7570  .....Tensor..tup
+000029f0: 6c65 7294 0000 0072 a800 0000 722c 0000  ler....r....r,..
+00002a00: 0072 2c00 0000 722c 0000 0072 3200 0000  .r,...r,...r2...
+00002a10: da08 3c6d 6f64 756c 653e 0100 0000 73a8  ..<module>....s.
+00002a20: 0000 0008 0108 0108 0108 0108 010c 0108  ................
+00002a30: 0108 0208 010c 020c 010c 010c 010c 0118  ................
+00002a40: 0710 0900 0100 0100 0100 0100 0100 0100  ................
+00002a50: 0100 0100 f202 0102 0102 0102 0102 0102  ................
+00002a60: 0104 0102 0102 0102 0102 0102 0102 0106  ................
+00002a70: 0102 f20c 7f00 3604 010a 1000 0100 0100  ......6.........
+00002a80: 0100 0100 f102 0104 0104 0102 0102 0102  ................
+00002a90: 0102 0102 0104 0104 0102 0102 0102 0102  ................
+00002aa0: 0102 0102 0102 f00c 7f00 1100 fa02 0202  ................
+00002ab0: 0106 0102 0102 0106 fa0c 1d08 1108 0608  ................
+00002ac0: 1600 ff02 0106 0104 fe0c 15              ...........
```

### Comparing `morpheus_spatial-0.4.0/src/morpheus/counterfactual/cf.py` & `morpheus_spatial-0.5.0/src/morpheus/counterfactual/cf_tf.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import torch
 
 logger = logging.getLogger(__name__)
 tf.logging.set_verbosity(tf.logging.ERROR)
 
 # disable eager execution
 tf.compat.v1.disable_eager_execution()
+tf.random.set_random_seed(42)
 
 
 class Counterfactual(Explainer, FitMixin):
 
     def __init__(
         self,
         predict: Union[Callable[[np.ndarray], np.ndarray], tf.keras.Model],
@@ -44,14 +45,17 @@
         eps: tuple = (1e-3, 1e-3),
         clip: tuple = (-1000.0, 1000.0),
         update_num_grad: int = 1,
         trustscore: Optional[str] = None,
         write_dir: Optional[str] = None,
         sess: Optional[tf.Session] = None,
         verbose: bool = False,
+        device: str = "cpu",
+        verbosity: int = 0,
+        numerical_diff: bool = False,
     ) -> None:
         """
         Initialize prototypical counterfactual method.
 
         Parameters
         ----------
         predict
@@ -142,15 +146,14 @@
 
         if is_model:  # Keras or TF model
             self.model = True
             self.classes = self.predict.predict(np.zeros(shape)).shape[1]  # type: ignore
         else:  # black-box model
             self.model = False
             self.classes = self.predict(torch.zeros(size=shape)).shape[1]
-            print(f"Black box model with {self.classes} classes")
 
         if is_enc:
             self.enc_model = True
         else:
             self.enc_model = False
 
         if is_ae:
@@ -525,15 +528,16 @@
         # probability of target label prediction
         target_proba = np.sum(pred_proba * Y)
         # max probability of non target label prediction
         nontarget_proba_max = np.max((1 - Y) * pred_proba - 10000 * Y)
         # loss term f(x,d)
         loss = np.maximum(0.0, -nontarget_proba_max + target_proba + self.kappa)
         # c * f(x,d)
-        loss_attack = np.sum(self.const.eval(session=self.sess) * loss)
+        c = self.const.eval(session=self.sess)
+        loss_attack = np.sum(c * loss)
         return loss_attack
 
     def get_gradients(
         self, X: np.ndarray, Y: np.ndarray, grads_shape: tuple
     ) -> np.ndarray:
         """
         Compute numerical gradients of the attack loss term:
```

### Comparing `morpheus_spatial-0.4.0/src/morpheus/counterfactual/cf_in_progress.py` & `morpheus_spatial-0.5.0/src/morpheus/counterfactual/cf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import os
 import copy
 import sys
 import _pickle as pickle
 from typing import Callable, Optional, Tuple, Union
 import numpy as np
 import warnings
 
 import torch
 import torch.optim as optim
 
 from ..api.defaults import DEFAULT_DATA, DEFAULT_META
 from ..api.interfaces import Explainer, Explanation, FitMixin
+from ..utils.gradients import perturb
 
 
 class Counterfactual(Explainer, FitMixin):
     def __init__(
         self,
         predict: Union[Callable[[np.ndarray], np.ndarray], torch.nn.Module],
         input_transform: Union[Callable[[np.ndarray], np.ndarray], torch.nn.Module],
@@ -34,15 +34,17 @@
         max_iterations: int = 1000,
         c_init: float = 10.0,
         c_steps: int = 10,
         eps: tuple = (1e-3, 1e-3),
         clip: tuple = (-1000.0, 1000.0),
         update_num_grad: int = 1,
         trustscore: Optional[str] = None,
-        verbose: bool = False,
+        verbosity: int = 0,
+        numerical_diff: bool = True,
+        device: str = None,
     ) -> None:
         """
         Initialize prototypical counterfactual method.
 
         Parameters
         ----------
         predict
@@ -87,37 +89,42 @@
         trustscore
             Directory where trustscore object is to be used
         sess
             Optional `tensorflow` session that will be used if passed instead of creating or inferring one internally.
         """
         super().__init__(meta=copy.deepcopy(DEFAULT_META))
 
-        # if image as input
-        if len(shape) > 2:
-            patch_shape = shape[
-                1:
-            ]  # should be [x length, y length, and number of color channels]
-            shape = (shape[0], shape[-1])
-        else:
-            patch_shape = shape
         params = locals()
         remove = [
             "self",
             "predict",
             "input_transform",
             "ae_model",
             "enc_model",
             "__class__",
         ]
         for key in remove:
             params.pop(key)
         self.meta["params"].update(params)
         self.predict = predict
         self.trustscore = trustscore
-        self.classes = self.predict(torch.zeros(size=shape)).shape[1]
+        self.numerical_diff = numerical_diff
+        self.device = (
+            device
+            if device is not None
+            else torch.device("cuda" if torch.cuda.is_available() else "cpu")
+        )
+
+        # check if predict is a pytorch model
+        is_model = True
+        if is_model:
+            self.classes = self.predict(torch.zeros(size=shape)).shape[1]
+        else:
+            self.numerical_diff = True
+            self.classes = self.predict.predict(np.zeros(shape)).shape[1]
 
         is_ae = isinstance(ae_model, torch.nn.Module)
         is_enc = isinstance(enc_model, torch.nn.Module)
 
         if is_enc:
             self.enc_model = True
         else:
@@ -136,25 +143,24 @@
         if use_kdtree or self.enc_model:
             self.enc_or_kdtree = True
         else:
             self.enc_or_kdtree = False
         self.meta["params"].update(enc_or_kdtree=self.enc_or_kdtree)
 
         self.shape = shape
-        self.patch_shape = patch_shape
         self.kappa = kappa
         self.beta = beta
         self.gamma = gamma
         self.theta = theta
         self.ae = ae_model
         self.enc = enc_model
         self.use_kdtree = use_kdtree
         self.batch_size = shape[0]
         self.max_iterations = max_iterations
-        self.c_init = torch.tensor(c_init, dtype=torch.float32)
+        self.c_init = torch.tensor(c_init)
         self.c_steps = c_steps
         self.feature_range = tuple(
             [
                 (
                     (torch.ones(shape[1:]) * feature_range[_])[None, :]
                     if isinstance(feature_range[_], float)
                     else feature_range[_]
@@ -163,15 +169,15 @@
             ]
         )
         self.update_num_grad = update_num_grad
         self.eps = eps
         self.clip = clip
         self.input_transform = input_transform
         self.learning_rate_init = learning_rate_init
-        self.verbose = verbose
+        self.verbosity = verbosity
 
         # variable for target class proto
         if self.enc_model:
             self.shape_enc = self.enc.predict(np.zeros(self.shape)).shape  # type: ignore[union-attr]
         else:
             # shape_env may not be equal to shape
             self.shape_enc = self.shape
@@ -245,24 +251,24 @@
             self.loss_ae = self.gamma * torch.norm(self.adv_ae - self.adv) ** 2
             self.loss_ae_s = self.gamma * torch.norm(self.adv_ae_s - self.adv_s) ** 2
         else:  # No auto-encoder available
             self.loss_ae = torch.tensor(0.0)
             self.loss_ae_s = torch.tensor(0.0)
 
     def compute_attack_loss(self):
-        if self.c_init == 0.0 and self.c_steps == 1:  # Prediction loss term not used
-            self.pred_proba = self.predict(self.adv)
-            self.pred_proba_s = self.predict(self.adv_s)
+        self.pred_proba = self.predict(self.adv)
+        self.pred_proba_s = self.predict(self.adv_s)
 
+        if self.numerical_diff:
+            with torch.no_grad():
+                self.loss_attack = self.loss_fn(self.pred_proba, self.target)
+        elif self.c_init == 0.0 and self.c_steps == 1:  # Prediction loss term not used
             self.loss_attack = torch.tensor(0.0)
             self.loss_attack_s = torch.tensor(0.0)
         else:
-            self.pred_proba = self.predict(self.adv)
-            self.pred_proba_s = self.predict(self.adv_s)
-
             # Probability of target label prediction
             self.target_proba = torch.sum(self.target * self.pred_proba, dim=1)
             target_proba_s = torch.sum(self.target * self.pred_proba_s, dim=1)
 
             # Max probability of non-target label prediction
             self.nontarget_proba_max = torch.max(
                 (1 - self.target) * self.pred_proba - (self.target * 10000), dim=1
@@ -298,41 +304,64 @@
             self.loss_proto_s = (
                 self.theta * torch.norm(self.adv_s - self.target_proto) ** 2
             )
         else:  # No encoder available and no k-d trees used
             self.loss_proto = torch.tensor(0.0)
             self.loss_proto_s = torch.tensor(0.0)
 
-    def compute_combined_loss(self):
+    def compute_regularizer_loss(self):
 
         # Computer each loss term
-        self.compute_attack_loss()
         self.compute_l1_l2_losses(self.shape)
         self.compute_autoencoder_loss()
         self.compute_prototype_loss()
 
-        """Compute the combined loss."""
-        self.loss_opt = (
-            self.loss_attack_s + self.loss_l2_s + self.loss_ae_s + self.loss_proto_s
-        )
+        """Compute the regularization loss."""
+        self.loss_reg = self.loss_l2_s + self.loss_ae_s + self.loss_proto_s
+
         # add L1 term to overall loss; this is not the loss that will be directly optimized
         self.loss_total = (
             self.loss_attack
             + self.loss_l2
             + self.loss_ae
             + self.beta * self.loss_l1
             + self.loss_proto
         )
 
+    def loss_fn(self, pred_proba: torch.Tensor, Y: torch.Tensor) -> torch.Tensor:
+        """
+        Compute the attack loss.
+
+        Parameters
+        ----------
+        pred_proba
+            Prediction probabilities of an instance.
+        Y
+            One-hot representation of instance labels.
+
+        Returns
+        -------
+        Loss of the attack.
+        """
+        # probability of target label prediction
+        target_proba = torch.sum(pred_proba * Y)
+        # max probability of non target label prediction
+        nontarget_proba_max = torch.max((1 - Y) * pred_proba - 10000 * Y)
+        # loss term f(x,d)
+        loss = torch.maximum(
+            torch.tensor([0.0]), -nontarget_proba_max + target_proba + self.kappa
+        )
+        # c * f(x,d)
+        loss_attack = torch.sum(self.const * loss)
+        return loss_attack
+
     def setup_training(self, learning_rate_init):
         """Set up the training parameters."""
         self.optimizer = optim.SGD([self.adv_s], lr=learning_rate_init)
-        lambda_poly_decay = (
-            lambda epoch: learning_rate_init * (1 - epoch / self.max_iterations) ** 0.5
-        )
+        lambda_poly_decay = lambda epoch: (1 - epoch / self.max_iterations) ** 0.5
         self.learning_rate = optim.lr_scheduler.LambdaLR(
             optimizer=self.optimizer, lr_lambda=lambda_poly_decay
         )
 
     def fit(
         self,
         train_data: np.ndarray = np.array([]),
@@ -370,14 +399,82 @@
             #     "No encoder specified. Using k-d trees to represent class prototypes."
             # )
             ts = load_object(self.trustscore)
             self.kdtrees = ts.kdtrees
             self.X_by_class = ts.X_kdtree
         return self
 
+    def get_gradients(
+        self, X: np.ndarray, Y: np.ndarray, grads_shape: tuple
+    ) -> np.ndarray:
+        """
+        Compute numerical gradients of the attack loss term:
+        `dL/dx = (dL/dP)*(dP/dx)` with `L = loss_attack_s; P = predict; x = adv_s`.
+
+        Parameters
+        ----------
+        X
+            Instance around which gradient is evaluated.
+        Y
+            One-hot representation of instance labels.
+        grads_shape
+            Shape of gradients.
+
+        Returns
+        -------
+        Array with gradients.
+        """
+        X_pred = X.clone().detach()
+        # N = gradient batch size; F = nb of features; P = nb of prediction classes; B = instance batch size
+        # dL/dP -> BxP
+        preds = self.predict(X_pred).detach().numpy()  # NxP
+        preds_pert_pos, preds_pert_neg = perturb(
+            preds, self.eps[0], proba=True
+        )  # (N*P)xP
+
+        def f(preds_pert):
+            return np.sum(Y * preds_pert, axis=1)
+
+        def g(preds_pert):
+            return np.max((1 - Y) * preds_pert, axis=1)
+
+        # find instances where the gradient is 0
+        idx_nograd = np.where(f(preds) - g(preds) <= -self.kappa)[0]
+        if len(idx_nograd) == X.shape[0]:
+            return np.zeros((1, *X.shape[1:]))
+        dl_df = f(preds_pert_pos) - f(preds_pert_neg)  # N*P
+        dl_dg = g(preds_pert_pos) - g(preds_pert_neg)  # N*P
+        dl_dp = dl_df - dl_dg  # N*P
+        dl_dp = np.reshape(dl_dp, (X.shape[0], -1)) / (2 * self.eps[0])  # NxP
+
+        # dP/dx -> PxF
+        X_pert_pos, X_pert_neg = perturb(
+            X, self.eps[1], proba=False
+        )  # (N*F)x(shape of X[0])
+        X_pert = np.concatenate([X_pert_pos, X_pert_neg], axis=0)
+        preds_concat = self.predict(torch.tensor(X_pert)).detach().numpy()  # (N*F)*P
+        n_pert = X_pert_pos.shape[0]
+        dp_dx = preds_concat[:n_pert] - preds_concat[n_pert:]  # (N*F)*P
+        dp_dx = np.reshape(
+            np.reshape(dp_dx, (X.shape[0], -1)),
+            (X.shape[0], preds.shape[1], -1),
+            order="F",
+        ) / (
+            2 * self.eps[1]
+        )  # NxPxF
+
+        # dL/dx -> Bx(shape of X[0])
+        grads = np.einsum("ij,ijk->ik", dl_dp, dp_dx)  # NxF
+        # set instances where gradient is 0 to 0
+        if len(idx_nograd) > 0:
+            grads[idx_nograd] = np.zeros(grads.shape[1:])
+        grads = np.mean(grads, axis=0)  # B*F
+        grads = np.reshape(grads, (self.batch_size,) + grads_shape)  # B*(shape of X[0])
+        return grads
+
     def score(
         self, X: np.ndarray, adv_class: int, orig_class: int, eps: float = 1e-10
     ) -> float:
         """
         Parameters
         ----------
         X
@@ -415,15 +512,14 @@
         self,
         X: np.ndarray,
         Y: np.ndarray,
         target_class: Optional[list] = None,
         k: Optional[int] = None,
         k_type: str = "mean",
         threshold: float = 0.0,
-        verbose: bool = False,
         print_every: int = 100,
     ) -> Tuple[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
         """
         Find a counterfactual (CF) for instance `X` using a fast iterative shrinkage-thresholding algorithm (FISTA).
 
         Parameters mk
         ----------
@@ -442,26 +538,25 @@
             the k-nearest encoding in the class (``k_type='point'``) to define the prototype of that class.
             Only relevant if an encoder is used to define the prototypes.
         threshold
             Threshold level for the ratio between the distance of the counterfactual to the prototype of the
             predicted class for the original instance over the distance to the prototype of the predicted class
             for the counterfactual. If the trust score is below the threshold, the proposed counterfactual does
             not meet the requirements.
-        verbose
-            Print intermediate results of optimization if ``True``.
+        verbosity
+            Print intermediate results of optimization if greater than 1.
         print_every
-            Print frequency if verbose is ``True``.
+            Print frequency if verbose is greater than 1.
         log_every
             `tensorboard` log frequency if write directory is specified.
 
         Returns
         -------
         Overall best attack and gradients for that attack.
         """
-
         # make sure nb of instances in X equals batch size
         assert self.batch_size == X.shape[0]
 
         def compare(x: Union[float, int, np.ndarray], y: int) -> bool:
             """
             Compare predictions with target labels and return whether counterfactual conditions hold.
 
@@ -484,15 +579,15 @@
                 x = torch.argmax(x)  # type: ignore
             return x != y
 
         # define target classes for prototype if not specified yet
         if target_class is None:
             target_class = list(range(self.classes))
             target_class.remove(np.argmax(Y, axis=1))
-            if self.verbose:
+            if self.verbosity > 1:
                 print("Predicted class: {}".format(np.argmax(Y, axis=1)))
                 print("Target classes: {}".format(target_class))
         X_num = X
 
         # find closest prototype in the target class list
         dist_proto = {}
         if self.enc_model:
@@ -521,25 +616,28 @@
         elif self.use_kdtree:
             if k is None:
                 k = 1
             self.class_proto = {}
             for c in range(self.classes):
                 if c not in target_class:
                     continue
-                dist_c, idx_c = self.kdtrees[c].query(X_num, k=k)
+                dist_c, idx_c = self.kdtrees[c].query(X_num.cpu(), k=k)
                 dist_proto[c] = dist_c[0][-1]
                 self.class_proto[c] = self.X_by_class[c][idx_c[0][-1]].reshape(1, -1)
 
         if self.enc_or_kdtree:
             self.id_proto = min(dist_proto, key=dist_proto.get)
-            proto_val = self.class_proto[self.id_proto]
-            if self.verbose:
+            proto_val = self.class_proto[self.id_proto].to(self.device)
+            if self.verbosity > 1:
                 print("Prototype class: {}".format(self.id_proto))
         else:  # no prototype loss term used
-            torch.zeros(self.shape_enc, dtype=torch.float32)
+            torch.zeros(self.shape_enc)
+
+        # set shape for perturbed instance and gradients
+        pert_shape = self.shape
 
         # set the lower and upper bounds for the constant 'c' to scale the attack loss term
         # these bounds are updated for each c_step iteration
         const_lb = torch.zeros(self.batch_size)
         const = torch.ones(self.batch_size) * self.c_init
         const_ub = torch.ones(self.batch_size) * 1e10
 
@@ -555,144 +653,202 @@
         for _ in range(self.c_steps):
 
             # init variables
             self.orig = X_num.clone().detach()
             self.target = Y.clone().detach()
             self.const = const.clone().detach()
             self.adv = X_num.clone().detach()
-            self.adv_s = X_num.clone().detach().requires_grad_()
+            self.adv_s = X_num.clone().requires_grad_()
             self.target_proto = proto_val.clone().detach()
 
             # init optimizer
             self.setup_training(self.learning_rate_init)
 
             # reset current best distances and scores
             current_best_dist = [1e10] * self.batch_size
             current_best_proba = [-1] * self.batch_size
             self.global_step = 0
 
+            X_der_batch, X_der_batch_s = [], []  # type: Any, Any
+
+            # Zero out the gradients before computation at every step
+            self.optimizer.zero_grad()
+
+            # Compute the forward loss
+            self.compute_attack_loss()
+            self.compute_regularizer_loss()
+
             for i in range(self.max_iterations):
-                # Zero out the gradients before computation at every step
-                self.optimizer.zero_grad()
 
-                # Compute the forward loss
-                self.compute_combined_loss()
+                # numerical gradients
+                grads_num = np.zeros(pert_shape)
+                grads_num_s = np.zeros(pert_shape)
+
+                # check if numerical gradient computation is needed
+                if self.numerical_diff and (self.c_init != 0.0 or self.c_steps > 1):
+                    X_der = self.adv.clone().detach()
+                    X_der_s = self.adv_s.clone().detach()
+                    Y_numpy = Y.clone().detach().numpy()
 
-                # Compute gradients in backward pass
-                self.loss_opt.backward()
+                    X_der_batch.append(X_der)
+                    X_der_batch_s.append(X_der_s)
+                    if (
+                        i % self.update_num_grad == 0 and i > 0
+                    ):  # compute numerical gradients
+                        c = self.const.numpy()
+                        X_der_batch = torch.cat(X_der_batch)
+                        X_der_batch_s = torch.cat(X_der_batch_s)
+                        grads_num = (
+                            self.get_gradients(
+                                X_der_batch, Y_numpy, grads_shape=pert_shape[1:]
+                            )
+                            * c
+                        )
+                        grads_num_s = (
+                            self.get_gradients(
+                                X_der_batch_s, Y_numpy, grads_shape=pert_shape[1:]
+                            )
+                            * c
+                        )
+                        # clip gradients
+                        grads_num = np.clip(grads_num, self.clip[0], self.clip[1])  # type: ignore
+                        grads_num_s = np.clip(grads_num_s, self.clip[0], self.clip[1])  # type: ignore
+                        X_der_batch, X_der_batch_s = [], []
+                elif not self.numerical_diff:
+                    self.loss_attack_s.backward()
+                    with torch.no_grad():
+                        self.adv_s.grad.clamp_(self.clip[0], self.clip[1])
 
-                # Clip the gradients
+                self.loss_reg.backward(retain_graph=True)
                 with torch.no_grad():
-                    self.adv_s.grad.clamp_(self.clip[0], self.clip[1])
-                gradients = self.adv_s.grad
+                    if self.numerical_diff:
+                        self.adv_s.grad.clamp_(self.clip[0], self.clip[1])
+                    else:
+                        self.adv_s.grad.clamp_(self.clip[0] * 2, self.clip[1] * 2)
+                    self.adv_s.grad.add_(torch.from_numpy(grads_num_s))
+                    gradients = self.adv_s.grad
 
                 # Apply the gradients
                 self.optimizer.step()
 
                 # Update the learning rate
                 self.learning_rate.step()
 
+                # Increment the global step
+                self.global_step += 1
+
                 # update adv and adv_s
                 with torch.no_grad():
                     self.compute_shrinkage_thresholding(self.feature_range)
                     self.compute_perturbation_projection()
                     self.update_counterfactuals()
 
                 # compute overall and attack loss, L1+L2 loss, prediction probabilities
                 # on perturbed instances and new adv
                 # L1+L2 and prediction probabilities used to see if adv is better than the current best adv under FISTA
-                self.compute_combined_loss()
+                self.optimizer.zero_grad()
 
-                if i % print_every == 0:
-                    target_proba = torch.sum(self.pred_proba * Y)
-                    nontarget_proba_max = torch.max((1 - Y) * self.pred_proba)
-
-                if self.verbose and i % print_every == 0:
-                    print("\nIteration: {}; Const: {}".format(i, const[0]))
-                    print(
-                        "Loss total: {:.3f}, loss attack: {:.3f}".format(
-                            self.loss_total, self.loss_attack
-                        )
-                    )
-                    print(
-                        "L2: {:.3f}, L1: {:.3f}, loss AE: {:.3f}".format(
-                            self.loss_l2, self.loss_l1, self.loss_ae
+                self.compute_attack_loss()
+                self.compute_regularizer_loss()
+
+                with torch.no_grad():
+                    if self.verbosity > 1 and i % print_every == 0:
+
+                        target_proba = torch.sum(self.pred_proba * Y)
+                        nontarget_proba_max = torch.max((1 - Y) * self.pred_proba)
+
+                        print("\nIteration: {}; Const: {}".format(i, const[0]))
+                        print(
+                            "Loss total: {:.3f}, loss attack: {:.3f}".format(
+                                self.loss_total, self.loss_attack
+                            )
                         )
-                    )
-                    print("Loss proto: {:.3f}".format(self.loss_proto))
-                    print(
-                        "Target proba: {:.2f}, max non target proba: {:.2f}".format(
-                            target_proba, nontarget_proba_max
+                        print(
+                            "L2: {:.3f}, L1: {:.3f}".format(self.loss_l2, self.loss_l1)
                         )
-                    )
-                    # Ensure gradients are not None
-                    if gradients is not None:
-                        # Convert gradients to a numpy array for printing if necessary
-                        gradients_np = gradients.detach().cpu().numpy()  # type: ignore
+                        print("Loss proto: {:.3f}".format(self.loss_proto))
                         print(
-                            "Gradient min/max: {:.3f}/{:.3f}".format(
-                                gradients_np.min(), gradients_np.max()
+                            "Target proba: {:.2f}, max non target proba: {:.2f}".format(
+                                target_proba, nontarget_proba_max
                             )
                         )
-                        print("Gradient mean/abs mean: {:.3f}/{:.3f}".format(gradients_np.mean(), np.mean(np.abs(gradients_np))))  # type: ignore
-                    else:
-                        print("Gradient min/max: None")
-                        print("Gradient mean/abs mean: None")
-                    sys.stdout.flush()
-
-                # update best perturbation (distance) and class probabilities
-                # if beta * L1 + L2 < current best and predicted label is different from the initial label:
-                # update best current step or global perturbations
-                for batch_idx, (dist, proba, adv_idx) in enumerate(
-                    zip(self.l1_l2, self.pred_proba, self.adv)
-                ):
-                    Y_class = torch.argmax(Y[batch_idx])
-                    adv_class = torch.argmax(proba)
-                    adv_idx = adv_idx.unsqueeze(0)
-
-                    # calculate trust score
-                    if threshold > 0.0:
-                        score = self.score(adv_idx, np.argmax(pred_proba), Y_class)  # type: ignore
-                        above_threshold = score > threshold
-                    else:
-                        above_threshold = True
-
-                    # current step
-                    if (
-                        dist < current_best_dist[batch_idx]
-                        and compare(proba, Y_class)  # type: ignore
-                        and above_threshold
-                        and adv_class in target_class
-                    ):
-                        current_best_dist[batch_idx] = dist
-                        current_best_proba[batch_idx] = adv_class  # type: ignore
-                        print(adv_class)
-
-                    # global
-                    if (
-                        dist < overall_best_dist[batch_idx]
-                        and compare(proba, Y_class)  # type: ignore
-                        and above_threshold
-                        and adv_class in target_class
+                        # Ensure gradients are not None
+                        if gradients is not None:
+                            # Convert gradients to a numpy array for printing if necessary
+                            gradients_np = gradients.detach().cpu().numpy()  # type: ignore
+                            print(
+                                "Gradient min/max: {:.3f}/{:.3f}".format(
+                                    gradients_np.min(), gradients_np.max()
+                                )
+                            )
+                            print("Gradient mean/abs mean: {:.3f}/{:.3f}".format(gradients_np.mean(), np.mean(np.abs(gradients_np))))  # type: ignore
+                        else:
+                            print("Gradient min/max: None")
+                            print("Gradient mean/abs mean: None")
+                        if self.numerical_diff:
+                            print(
+                                "Gradient numerical attack min/max: {:.3f}/{:.3f}".format(
+                                    grads_num.min(), grads_num.max()
+                                )
+                            )  # type: ignore
+                            print(
+                                "Gradient numerical mean/abs mean: {:.3f}/{:.3f}".format(
+                                    np.mean(grads_num), np.mean(np.abs(grads_num))
+                                )
+                            )  # type: ignore
+                        sys.stdout.flush()
+
+                    # update best perturbation (distance) and class probabilities
+                    # if beta * L1 + L2 < current best and predicted label is different from the initial label:
+                    # update best current step or global perturbations
+                    for batch_idx, (dist, proba, adv_idx) in enumerate(
+                        zip(self.l1_l2, self.pred_proba, self.adv)
                     ):
-                        if self.verbose:
-                            print("\nNew best counterfactual found!")
-                        overall_best_dist[batch_idx] = dist
-                        overall_best_attack[batch_idx] = adv_idx
-                        overall_best_grad = gradients
-                        self.best_attack = True
-                        self.cf_global[_].append(adv_idx)
-
-                # Increment the global step
-                self.global_step += 1
+                        Y_class = torch.argmax(Y[batch_idx])
+                        adv_class = torch.argmax(proba)
+                        adv_idx = adv_idx.unsqueeze(0)
+
+                        # calculate trust score
+                        if threshold > 0.0:
+                            score = self.score(adv_idx, np.argmax(pred_proba), Y_class)  # type: ignore
+                            above_threshold = score > threshold
+                        else:
+                            above_threshold = True
+
+                        # current step
+                        if (
+                            dist < current_best_dist[batch_idx]
+                            and compare(proba, Y_class)  # type: ignore
+                            and above_threshold
+                            and adv_class in target_class
+                        ):
+                            current_best_dist[batch_idx] = dist
+                            current_best_proba[batch_idx] = adv_class  # type: ignore
+
+                        # global
+                        if (
+                            dist < overall_best_dist[batch_idx]
+                            and compare(proba, Y_class)  # type: ignore
+                            and above_threshold
+                            and adv_class in target_class
+                        ):
+                            if self.verbosity > 1:
+                                print("\nNew best counterfactual found!")
+                            overall_best_dist[batch_idx] = dist
+                            overall_best_attack[batch_idx] = adv_idx
+                            overall_best_grad = gradients
+                            self.best_attack = True
+                            self.cf_global[_].append(adv_idx)
 
             # adjust the 'c' constant for the first loss term
             for batch_idx in range(self.batch_size):
                 if (
-                    compare(current_best_proba[batch_idx], np.argmax(Y[batch_idx]))
+                    compare(
+                        current_best_proba[batch_idx], np.argmax(Y[batch_idx].cpu())
+                    )
                     and current_best_proba[batch_idx] != -1  # type: ignore
                 ):
                     # want to refine the current best solution by putting more emphasis on the regularization terms
                     # of the loss by reducing 'c'; aiming to find a perturbation closer to the original instance
                     const_ub[batch_idx] = min(const_ub[batch_idx], const[batch_idx])
                     if const_ub[batch_idx] < 1e9:
                         const[batch_idx] = (
@@ -708,15 +864,17 @@
                         const[batch_idx] = (
                             const_lb[batch_idx] + const_ub[batch_idx]
                         ) / 2
                     else:
                         const[batch_idx] *= 10
 
         # return best overall attack
-        best_attack = np.concatenate(overall_best_attack, axis=0)
+        best_attack = np.concatenate(
+            [item.cpu() for item in overall_best_attack], axis=0
+        )
         if best_attack.shape != self.shape:
             best_attack = np.expand_dims(best_attack, axis=0)
 
         return best_attack, overall_best_grad
 
     def explain(
         self,
@@ -749,18 +907,18 @@
             the k-nearest encoding in the class (``k_type='point'``) to define the prototype of that class.
             Only relevant if an encoder is used to define the prototypes.
         threshold
             Threshold level for the ratio between the distance of the counterfactual to the prototype of the
             predicted class for the original instance over the distance to the prototype of the predicted class
             for the counterfactual. If the trust score is below the threshold, the proposed counterfactual does
             not meet the requirements.
-        verbose
-            Print intermediate results of optimization if ``True``.
+        verbosity
+            Print intermediate results of optimization if greater than 1.
         print_every
-            Print frequency if verbose is ``True``.
+            Print frequency if verbosity is greater than 1.
         log_every
             `tensorboard` log frequency if write directory is specified
 
         Returns
         -------
         explanation
             `Explanation` object containing the counterfactual with additional metadata as attributes.
@@ -772,55 +930,60 @@
                 X.shape[0],
             )
 
         # output explanation dictionary
         data = copy.deepcopy(DEFAULT_DATA)
 
         # add original prediction to explanation
-        Y_proba = self.predict(X)
-        if Y is None:
-            Y_ohe = np.zeros(Y_proba.shape)
-            Y_class = np.argmax(Y_proba, axis=1)
-            Y_ohe[np.arange(Y_proba.shape[0]), Y_class] = 1
-            Y = Y_ohe.clone()
+        Y_proba = self.predict(X).detach().cpu().numpy()
+        Y_ohe = np.zeros(Y_proba.shape)
+        Y_class = np.argmax(Y_proba, axis=1)
+        Y_ohe[np.arange(Y_proba.shape[0]), Y_class] = 1
+        Y = torch.from_numpy(Y_ohe).clone().to(self.device)
+
         data["orig_proba"] = Y_proba
-        data["orig_class"] = torch.argmax(Y_proba, dim=1)[0]
+        data["orig_class"] = np.argmax(Y_proba, axis=1)[0]
 
         # find best counterfactual
         self.best_attack = False  # flag to indicate whether a CF was found
         best_attack, grads = self.attack(
             X,
             Y=Y,
             target_class=target_class,
             k=k,
             k_type=k_type,
-            verbose=self.verbose,
             threshold=threshold,
             print_every=print_every,
         )
 
         # add id of prototype to explanation dict
         if self.enc_or_kdtree:
             data["id_proto"] = self.id_proto
 
         # add to explanation dict
         if not self.best_attack:
-            warnings.warn("No counterfactual found!")
+            if self.verbosity > 0:
+                warnings.warn("No counterfactual found!")
 
             # create explanation object
             explanation = Explanation(meta=copy.deepcopy(self.meta), data=data)
             return explanation
 
         data["all"] = self.cf_global
         data["cf"] = {}
         data["cf"]["X"] = best_attack
-        Y_pert = self.predict(torch.from_numpy(best_attack)).detach().numpy()
+        Y_pert = (
+            self.predict(torch.from_numpy(best_attack).to(self.device))
+            .detach()
+            .cpu()
+            .numpy()
+        )
         data["cf"]["proba"] = Y_pert
         data["cf"]["class"] = np.argmax(Y_pert, axis=1)[0]
-        data["cf"]["grads"] = grads.detach().numpy()
+        data["cf"]["grads"] = grads.detach().cpu().numpy()
 
         # create explanation object
         explanation = Explanation(meta=copy.deepcopy(self.meta), data=data)
 
         return explanation
```

### Comparing `morpheus_spatial-0.4.0/src/morpheus/counterfactual/generate.py` & `morpheus_spatial-0.5.0/src/morpheus/counterfactual/generate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 import os
 import json
 import _pickle as pickle
 import numpy as np
 import pandas as pd
 from typing import Optional
 import torch
+import multiprocessing
 
+import ray
 from tqdm import tqdm
 
-# import multiprocessing
-
-
 from ..datasets import SpatialDataset
 from .cf import Counterfactual
+from ..classification import load_model
 from ..confidence import TrustScore
 from ..configuration import (
     Splits,
     ColName,
     DefaultFolderName,
     DefaultFileName,
 )
 
 EPSILON = torch.tensor(1e-20, dtype=torch.float32)
 
 
 def get_counterfactual(
     dataset: SpatialDataset,
     target_class: int,
-    model: torch.nn.Module,
+    model_path: str,
     channel_to_perturb: list,
     optimization_params: dict,
     images: pd.DataFrame = None,
     threshold: float = 0.5,
     kdtree_path: str = None,
     save_dir: str = None,
     num_workers: int = 1,
     train_data: str = None,
-    verbose: bool = False,
+    verbosity: int = 0,
     trustscore_kwargs: Optional[dict] = None,
+    device: str = None,
 ):
     """
     Generate counterfactuals for the dataset.
 
     Args:
         dataset (SpatialDataset): Dataset to generate counterfactuals for.
         target_class (int): Target class for the counterfactuals.
@@ -51,15 +52,19 @@
         images (pd.DataFrame, optional): Images to generate counterfactuals for. Defaults to None.
         threshold (float, optional): Threshold for the prediction probability. Defaults to 0.5.
         kdtree_path (str, optional): Path to the kdtree file. Defaults to None.
         save_dir (str, optional): Directory where output will be saved. Defaults to None.
         num_workers (bool, optional): Number of workers to use for parallel processing. Defaults to None.
         train_data (str, optional): Path to the training data. Defaults to None.
     """
-    num_images = len(images)
+
+    # set default tensor type to cuda if available
+    torch.set_default_tensor_type(
+        torch.cuda.FloatTensor if torch.cuda.is_available() else torch.FloatTensor
+    )
 
     # Load normalization parameters
     with open(
         os.path.join(dataset.split_dir, "normalization_params.json")
     ) as json_file:
         normalization_params = json.load(json_file)
         mu = normalization_params["mean"]
@@ -75,82 +80,158 @@
 
     # Create save directory
     if save_dir is None:
         save_dir = os.path.join(
             dataset.root_dir, DefaultFolderName.counterfactual.value
         )
     os.makedirs(save_dir, exist_ok=True)
-    dataset.cf_dir = save_dir
 
     # Build kdtree if it does not exist
+    model = load_model(model_path)
     if not os.path.exists(kdtree_path):
         build_kdtree(kdtree_path, train_data, model, mu, stdev, trustscore_kwargs)
         print("kdtree saved")
 
-    # Prepare arguments for generate_one_cf function
-    generate_one_cf_args = []
-    for i in range(num_images):
+    # Organize arguments for counterfactual generation
+
+    # used across all images
+    general_args = {
+        "target_class": target_class,
+        "model_path": model_path,
+        "channel": dataset.channel_names,
+        "channel_to_perturb": channel_to_perturb,
+        "mu": mu,
+        "stdev": stdev,
+        "kdtree_path": kdtree_path,
+        "verbosity": verbosity,
+        "optimization_params": optimization_params,
+        "save_dir": save_dir,
+        "threshold": threshold,
+        "device": device,
+    }
+
+    # specific to each image
+    image_args = []
+    for i in range(len(images)):
         img_path = dataset.generate_patch_path(
             patch_id=images.iloc[i][ColName.patch_id.value],
             label=images.iloc[i][dataset.label_name],
             split=images.iloc[i][ColName.splits.value],
         )
         img, patch_id = SpatialDataset.load_single_image(img_path)
         label = dataset.metadata.iloc[patch_id][dataset.label_name]
-        generate_one_cf_args.append(
-            (
-                img,
-                label,
-                target_class,
-                model,
-                dataset.channel_names,
-                channel_to_perturb,
-                mu,
-                stdev,
-                kdtree_path,
-                verbose,
-                optimization_params,
-                save_dir,
-                patch_id,
-                threshold,
+        image_args.append(
+            {
+                "original_patch": img,
+                "original_class": label,
+                "patch_id": patch_id,
+            }
+        )
+
+    discard_mask = [
+        args["original_class"] == target_class
+        or model(
+            torch.from_numpy(
+                np.transpose((args["original_patch"] - mu) / stdev, (2, 0, 1))[None, :]
             )
+            .float()
+            .to(device)
+        )
+        .detach()
+        .cpu()
+        .numpy()[0, 1]
+        > threshold
+        for args in tqdm(image_args)
+    ]
+    image_args = [args for i, args in enumerate(image_args) if not discard_mask[i]]
+
+    # Save hyperparameters
+    with open(os.path.join(save_dir, "hyperparameters.json"), "w") as json_file:
+        json.dump(
+            {
+                "target_class": target_class,
+                "channel_to_perturb": channel_to_perturb,
+                "optimization_params": optimization_params,
+                "threshold": threshold,
+            },
+            json_file,
         )
 
     # Generate counterfactuals
-    parallel = True if num_workers > 1 else False
-    if parallel:
-        from dask import delayed
-        import dask.multiprocessing
-
-        @delayed
-        def generate_one_cf_delayed(args):
-            return generate_one_cf(*args)
-
-        dask_tasks = [generate_one_cf_delayed(args) for args in generate_one_cf_args]
-        _ = dask.compute(*dask_tasks, scheduler="processes", num_workers=num_workers)
+    if num_workers > 1:
+        # Initialize Ray
+        ray.shutdown()
+        ray.init()
+
+        # Get the number of available CPUs
+        num_cpus = ray.available_resources()["CPU"]
+        print(f"Number of available CPUs: {num_cpus}")
+
+        # Create a list of Ray object references
+        cf_refs = [
+            generate_one_cf_wrapper.remote({**args, **general_args})
+            for args in image_args
+        ]
+
+        # Use tqdm to display a progress bar
+        with tqdm(total=len(image_args)) as pbar:
+            # Retrieve the results as they become available
+            results = []
+            while cf_refs:
+                done_refs, cf_refs = ray.wait(cf_refs)
+                results.extend(ray.get(done_refs))
+                pbar.update(len(done_refs))
+
+        # Shutdown Ray
+        ray.shutdown()
+
+        # pool = multiprocessing.Pool(num_workers)
+
+        # Check the number of worker processes
+        # num_workers = pool._processes
+        # print(f"Number of worker processes: {num_workers}")
+
+        # _ = list(
+        #     tqdm(
+        #         pool.imap(
+        #             generate_one_cf_wrapper,
+        #             [{**args, **general_args} for args in image_args],
+        #         ),
+        #         total=len(image_args),
+        #     )
+        # )
+        # pool.close()
+        # pool.join()
     else:
-        for args in tqdm(generate_one_cf_args, total=num_images):
-            generate_one_cf(*args)
+        for args in tqdm(image_args, total=len(image_args)):
+            generate_one_cf(**{**args, **general_args})
+
+
+@ray.remote
+def generate_one_cf_wrapper(combined_args):
+    torch.set_num_threads(1)  # very important
+    return generate_one_cf(**combined_args)
 
 
 def generate_one_cf(
     original_patch: np.ndarray,
     original_class: np.ndarray,
+    patch_id: int,
     target_class: int,
-    model: torch.nn.Module,
+    model_path: str,
     channel: list,
     channel_to_perturb: list,
     mu: np.ndarray,
     stdev: np.ndarray,
     kdtree_path: str,
-    verbose: bool = False,
+    verbosity: int = 0,
     optimization_params: dict = None,
     save_dir: str = None,
-    patch_id: int = None,
     threshold: float = 0.5,
+    device: str = None,
 ) -> None:
     """
     Generate counterfactuals for a given image patch.
 
     Args:
          original_patch (np.ndarray): Original patch to be explained.
          original_class (np.ndarray): Original label of the patch.
@@ -162,24 +243,36 @@
          save_dir (str, optional): Directory where output will be saved. Defaults to None.
          patch_id (int, optional): Patch ID. Defaults to None.
          threshold (float, optional): Threshold for the prediction probability. Defaults to 0.5.
 
      Returns:
          None
     """
+    # load model
+    model = load_model(model_path)
+
     # Obtain data features
     stdev, mu = (
         torch.tensor(stdev).float(),
         torch.tensor(mu).float(),
     )
     H, _, C = original_patch.shape
-    original_patch = (torch.from_numpy(original_patch).float() - mu) / stdev
+    original_patch = torch.from_numpy(original_patch.copy()).float().to(device)
+    original_patch = (original_patch - mu) / stdev
     original_class = torch.tensor([original_class], dtype=torch.int64)
     X_mean = torch.mean(original_patch, dim=(0, 1))
 
+    # move variables to cuda if available
+    if torch.cuda.is_available():
+        original_patch = original_patch.cuda()
+        original_class = original_class.cuda()
+        X_mean = X_mean.cuda()
+        stdev = stdev.cuda()
+        mu = mu.cuda()
+
     if model.arch == "mlp":
         original_patch = X_mean
 
     # Adding init layer to model
     unnormed_mean = X_mean * stdev + mu
     if model.arch == "mlp":
         altered_model = lambda x: torch.nn.functional.softmax(model(x), dim=1)
@@ -189,84 +282,76 @@
         init_fun = lambda y: alter_image(y, unnormed_patch, mu, stdev, unnormed_mean)
         altered_model, input_transform = add_init_layer(init_fun, model)
 
     # Set range of each channel to perturb
     is_perturbed = np.array(
         [True if name in channel_to_perturb else False for name in channel]
     )
-    feature_range = (torch.maximum(-mu / stdev, torch.ones(C) * -4), torch.ones(C) * 4)
+    feature_range = (
+        torch.maximum(-mu / stdev, torch.ones(C) * -4),
+        torch.ones(C) * 4,
+    )
     feature_range[0][~is_perturbed] = X_mean[~is_perturbed] - EPSILON
     feature_range[1][~is_perturbed] = X_mean[~is_perturbed] + EPSILON
 
     # define predict function
     predict_fn = lambda x: altered_model(x)
 
-    # Terminate if model incorrectly classifies patch as the target class
-    orig_proba = predict_fn(X_mean[None, :]).detach().cpu().numpy()
-    if verbose:
-        print(f"Initial probability: {orig_proba}")
-    pred = orig_proba[0, 1] > threshold
-    if pred == target_class:
-        print("Instance already classified as target class, no counterfactual needed")
-        return
-
     # define counterfactual object
-    shape = (1,) + original_patch.shape
+    shape = (1,) + X_mean.shape
     cf = Counterfactual(
         predict_fn,
         input_transform,
         shape,
         feature_range=feature_range,
         trustscore=kdtree_path,
-        verbose=verbose,
+        verbosity=verbosity,
+        device=device,
         **optimization_params,
     )
     cf.fit()
 
     # generate counterfactual
     explanation = cf.explain(
         X=X_mean[None, :], Y=original_class[None, :], target_class=[target_class]
     )
 
     if explanation.cf is not None:
         cf_prob = explanation.cf["proba"][0]
-        cf = explanation.cf["X"][0]
+        if verbosity > 0:
+            print(f"Counterfactual probability: {cf_prob}")
 
-        # manually compute probability of cf
-        cf = input_transform(torch.from_numpy(cf[None, :]))
-        counterfactual_probabilities = (
-            altered_model(cf) if model.arch == "mlp" else model(cf)
-        )
-        if model.arch != "mlp":
-            cf = torch.permute(cf, (0, 2, 3, 1))
+        cf = explanation.cf["X"][0]
+        cf = input_transform(torch.from_numpy(cf[None, :]).to(device))
+        cf = torch.permute(cf, (0, 2, 3, 1))
 
-        print(f"Counterfactual probability: {counterfactual_probabilities}")
         X_perturbed = mean_preserve_dimensions(
             cf * stdev + mu, preserveAxis=cf.ndim - 1
         )
         original_patch = X_mean * stdev + mu
         cf_delta = (X_perturbed - original_patch) / original_patch * 100
-        cf_perturbed = dict(
+        percent_delta = dict(
             zip(
                 np.array(channel)[is_perturbed],
-                cf_delta[is_perturbed].numpy(),
+                cf_delta[is_perturbed].cpu().numpy(),
             )
         )
-        print(f"cf perturbed: {cf_perturbed}")
+        if verbosity > 0:
+            print(f"cf perturbed (%): {percent_delta}")
 
         if save_dir is not None:
             os.makedirs(save_dir, exist_ok=True)
             saved_file = os.path.join(save_dir, f"patch_{patch_id}.npz")
             np.savez(
                 saved_file,
-                explanation=explanation,
-                cf_perturbed=cf_perturbed,
-                channel_to_perturb=np.array(channel)[is_perturbed],
+                cf=X_perturbed,
+                proba=cf_prob,
+                delta_in_percentage=percent_delta,
             )
-    return explanation
+        return percent_delta
 
 
 def build_kdtree(
     kdtree_path,
     train_data: str,
     model: torch.nn.Module,
     mu: list,
```

### Comparing `morpheus_spatial-0.4.0/src/morpheus/datasets/__pycache__/spatial_dataset.cpython-39.pyc` & `morpheus_spatial-0.5.0/src/morpheus/datasets/__pycache__/spatial_dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Mar 24 22:30:27 2024 UTC, .py size: 18422 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 83a9 0066 f647 0000  a..........f.G..
+00000000: 610d 0d0a 0000 0000 ef38 1666 5448 0000  a........8.fTH..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a05 6400 6401 6c06 5a07 6402  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c08 6d09 5a09 0100 6402 6404 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
@@ -11,884 +11,888 @@
 000000a0: 0029 01da 1a67 656e 6572 6174 655f 7061  .)...generate_pa
 000000b0: 7463 6865 735f 6f70 7469 6d69 7a65 6429  tches_optimized)
 000000c0: 04da 0743 6f6c 4e61 6d65 da06 5370 6c69  ...ColName..Spli
 000000d0: 7473 da11 4465 6661 756c 7446 6f6c 6465  ts..DefaultFolde
 000000e0: 724e 616d 65da 0f44 6566 6175 6c74 4669  rName..DefaultFi
 000000f0: 6c65 4e61 6d65 6300 0000 0000 0000 0000  leNamec.........
 00000100: 0000 0000 0000 0009 0000 0040 0000 0073  ...........@...s
-00000110: 3001 0000 6500 5a01 6400 5a02 643c 6503  0...e.Z.d.Z.d<e.
-00000120: 6504 6503 6503 6503 6503 6402 9c06 6403  e.e.e.e.e.d...d.
-00000130: 6404 8405 5a05 6405 6406 8400 5a06 6507  d...Z.d.d...Z.e.
-00000140: 6a08 6504 6407 9c02 6408 6409 8404 5a09  j.e.d...d.d...Z.
-00000150: 640a 640b 8400 5a0a 6700 640c 640d 6401  d.d...Z.g.d.d.d.
-00000160: 640e 6401 6606 6504 650b 650b 6504 650c  d.d.f.e.e.e.e.e.
-00000170: 6503 640f 9c06 6410 6411 8405 5a0d 643d  e.d...d.d...Z.d=
-00000180: 6503 6412 9c01 6413 6414 8405 5a0e 643e  e.d...d.d...Z.d>
-00000190: 6503 6415 9c01 6416 6417 8405 5a0f 643f  e.d...d.d...Z.d?
-000001a0: 6503 6418 9c01 6419 641a 8405 5a10 6440  e.d...d.d...Z.d@
-000001b0: 6503 641b 9c01 641c 641d 8405 5a11 641e  e.d...d.d...Z.d.
-000001c0: 641f 8400 5a12 6420 6421 8400 5a13 6503  d...Z.d d!..Z.e.
-000001d0: 6422 9c01 6423 6424 8404 5a14 6441 6503  d"..d#d$..Z.dAe.
-000001e0: 6515 6515 6515 6427 9c04 6428 6429 8405  e.e.e.d'..d(d)..
-000001f0: 5a16 6517 6442 642c 642d 8401 8301 5a18  Z.e.dBd,d-....Z.
-00000200: 6443 6430 6431 8401 5a19 6432 6433 8400  dCd0d1..Z.d2d3..
-00000210: 5a1a 651b 6a1c 6a1d 6601 6434 6435 8401  Z.e.j.j.f.d4d5..
-00000220: 5a1e 6436 6437 8400 5a1f 6517 6444 6438  Z.d6d7..Z.e.dDd8
-00000230: 6439 8401 8301 5a20 643a 643b 8400 5a21  d9....Z d:d;..Z!
-00000240: 6401 5300 2945 da0e 5370 6174 6961 6c44  d.S.)E..SpatialD
-00000250: 6174 6173 6574 4e29 06da 0a69 6e70 7574  atasetN)...input
-00000260: 5f70 6174 68da 0d63 6861 6e6e 656c 5f6e  _path..channel_n
-00000270: 616d 6573 da0a 7061 7463 685f 7061 7468  ames..patch_path
-00000280: da09 7370 6c69 745f 6469 72da 096d 6f64  ..split_dir..mod
-00000290: 656c 5f64 6972 da06 6366 5f64 6972 6307  el_dir..cf_dirc.
-000002a0: 0000 0000 0000 0000 0000 0008 0000 0004  ................
-000002b0: 0000 0043 0000 0073 b200 0000 6400 7c00  ...C...s....d.|.
-000002c0: 5f00 6400 7c00 5f01 7c01 7c00 5f02 7403  _.d.|._.|.|._.t.
-000002d0: 6a04 a005 7c01 a101 7c00 5f06 7407 7c02  j...|...|._.t.|.
-000002e0: 8301 6401 6b02 7234 7408 6402 8301 8201  ..d.k.r4t.d.....
-000002f0: 7c00 a009 a100 7d07 7c00 a00a 7c07 7c02  |.....}.|...|.|.
-00000300: a102 0100 7c00 a00b 7c03 a101 7c00 5f0c  ....|...|...|._.
-00000310: 7c00 a00d 7c04 a101 7c00 5f0e 7c00 a00f  |...|...|._.|...
-00000320: 7c05 a101 7c00 5f10 7c00 a011 7c06 a101  |...|._.|...|...
-00000330: 7c00 5f12 7c00 6a0c 6400 7501 7292 7c00  |._.|.j.d.u.r.|.
-00000340: a013 a100 0100 7c00 a014 a100 0100 7c00  ......|.......|.
-00000350: 6a0e 6400 7501 72ae 7c00 6a0c 6400 7501  j.d.u.r.|.j.d.u.
-00000360: 72ae 7c00 a015 a100 0100 6400 5300 2903  r.|.......d.S.).
-00000370: 4e72 0100 0000 7a1e 4368 616e 6e65 6c20  Nr....z.Channel 
-00000380: 6e61 6d65 7320 6d75 7374 2062 6520 7072  names must be pr
-00000390: 6f76 6964 6564 2916 da08 6461 7461 5f64  ovided)...data_d
-000003a0: 696d da08 6d65 7461 6461 7461 7209 0000  im..metadatar...
-000003b0: 00da 026f 73da 0470 6174 68da 0764 6972  ...os..path..dir
-000003c0: 6e61 6d65 da08 726f 6f74 5f64 6972 da03  name..root_dir..
-000003d0: 6c65 6eda 0a56 616c 7565 4572 726f 72da  len..ValueError.
-000003e0: 0e6c 6f61 645f 696e 7075 745f 6373 76da  .load_input_csv.
-000003f0: 0f63 6865 636b 5f69 6e70 7574 5f63 7376  .check_input_csv
-00000400: da0e 7365 745f 7061 7463 685f 7061 7468  ..set_patch_path
-00000410: 720b 0000 00da 0d73 6574 5f73 706c 6974  r......set_split
-00000420: 5f64 6972 720c 0000 00da 0d73 6574 5f6d  _dirr......set_m
-00000430: 6f64 656c 5f64 6972 720d 0000 00da 1673  odel_dirr......s
-00000440: 6574 5f63 6f75 6e74 6572 6661 6374 7561  et_counterfactua
-00000450: 6c5f 6469 7272 0e00 0000 da0f 6c6f 6164  l_dirr......load
-00000460: 5f70 6174 6368 5f64 6174 61da 1263 6865  _patch_data..che
-00000470: 636b 5f6c 6f61 6465 645f 7061 7463 68da  ck_loaded_patch.
-00000480: 0e67 6574 5f73 706c 6974 5f69 6e66 6f29  .get_split_info)
-00000490: 08da 0473 656c 6672 0900 0000 720a 0000  ...selfr....r...
-000004a0: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-000004b0: 720e 0000 00da 0464 6174 61a9 0072 2200  r......data..r".
-000004c0: 0000 fa57 2f63 656e 7472 616c 2f68 6f6d  ...W/central/hom
-000004d0: 652f 7a77 616e 6732 2f6d 6f72 7068 6575  e/zwang2/morpheu
-000004e0: 732d 7370 6174 6961 6c2f 6d6f 7270 6865  s-spatial/morphe
-000004f0: 7573 2f73 7263 2f6d 6f72 7068 6575 732f  us/src/morpheus/
-00000500: 6461 7461 7365 7473 2f73 7061 7469 616c  datasets/spatial
-00000510: 5f64 6174 6173 6574 2e70 79da 085f 5f69  _dataset.py..__i
-00000520: 6e69 745f 5f13 0000 0073 2200 0000 0009  nit__....s".....
-00000530: 0601 0601 0601 0e02 0c01 0802 0801 0c03  ................
-00000540: 0c01 0c01 0c01 0c02 0a01 0801 0803 1401  ................
-00000550: 7a17 5370 6174 6961 6c44 6174 6173 6574  z.SpatialDataset
-00000560: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00000570: 0000 0000 0000 0200 0000 0600 0000 4300  ..............C.
-00000580: 0000 732c 0000 0074 0044 005d 227d 017c  ..s,...t.D.]"}.|
-00000590: 016a 017c 006a 026a 037c 00a0 047c 016a  .j.|.j.j.|...|.j
-000005a0: 01a1 0174 056a 066a 0166 023c 0071 0464  ...t.j.j.f.<.q.d
-000005b0: 0053 00a9 014e 2907 7205 0000 00da 0576  .S...N).r......v
-000005c0: 616c 7565 7210 0000 00da 036c 6f63 da0d  aluer......loc..
-000005d0: 6765 745f 7370 6c69 745f 6964 7372 0400  get_split_idsr..
-000005e0: 0000 da06 7370 6c69 7473 2902 7220 0000  ....splits).r ..
-000005f0: 00da 0573 706c 6974 7222 0000 0072 2200  ...splitr"...r".
-00000600: 0000 7223 0000 0072 1f00 0000 3500 0000  ..r#...r....5...
-00000610: 7306 0000 0000 0108 0204 ff7a 1d53 7061  s..........z.Spa
-00000620: 7469 616c 4461 7461 7365 742e 6765 745f  tialDataset.get_
-00000630: 7370 6c69 745f 696e 666f 2902 da09 696e  split_info)...in
-00000640: 7075 745f 6373 7672 0a00 0000 6303 0000  put_csvr....c...
-00000650: 0000 0000 0000 0000 0005 0000 0005 0000  ................
-00000660: 0003 0000 0073 6c00 0000 7400 6a01 6a02  .....sl...t.j.j.
-00000670: 7400 6a03 6a02 7400 6a04 6a02 7400 6a05  t.j.j.t.j.j.t.j.
-00000680: 6a02 7400 6a06 6a02 6705 8800 1700 7d03  j.t.j.j.g.....}.
-00000690: 7c03 4400 5d18 7d04 7c04 7c01 6a07 7601  |.D.].}.|.|.j.v.
-000006a0: 722a 7408 a009 6401 a101 0100 712a 8700  r*t...d.....q*..
-000006b0: 6601 6402 6403 8408 7c01 6a07 4400 8301  f.d.d...|.j.D...
-000006c0: 7c00 5f0a 7c01 6a0b 7268 740c 6404 8301  |._.|.j.rht.d...
-000006d0: 8201 6400 5300 2905 4e7a 3169 6e70 7574  ..d.S.).Nz1input
-000006e0: 2063 7376 2064 6f65 7320 6e6f 7420 636f   csv does not co
-000006f0: 6e74 6169 6e20 7265 7175 6972 6564 2063  ntain required c
-00000700: 6f6c 756d 6e3a 207b 636f 6c7d 6301 0000  olumn: {col}c...
-00000710: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000720: 0013 0000 0073 1800 0000 6700 7c00 5d10  .....s....g.|.].
-00000730: 7d01 7c01 8800 7600 7204 7c01 9102 7104  }.|...v.r.|...q.
-00000740: 5300 7222 0000 0072 2200 0000 2902 da02  S.r"...r"...)...
-00000750: 2e30 da03 636f 6ca9 0172 0a00 0000 7222  .0..col..r....r"
-00000760: 0000 0072 2300 0000 da0a 3c6c 6973 7463  ...r#.....<listc
-00000770: 6f6d 703e 4900 0000 f300 0000 007a 3253  omp>I........z2S
-00000780: 7061 7469 616c 4461 7461 7365 742e 6368  patialDataset.ch
-00000790: 6563 6b5f 696e 7075 745f 6373 762e 3c6c  eck_input_csv.<l
-000007a0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-000007b0: 3e7a 1249 6e70 7574 2043 5356 2069 7320  >z.Input CSV is 
-000007c0: 656d 7074 7929 0d72 0400 0000 da0a 7061  empty).r......pa
-000007d0: 7469 656e 745f 6964 7226 0000 00da 0869  tient_idr&.....i
-000007e0: 6d61 6765 5f69 64da 0963 656c 6c5f 7479  mage_id..cell_ty
-000007f0: 7065 da06 6365 6c6c 5f78 da06 6365 6c6c  pe..cell_x..cell
-00000800: 5f79 da07 636f 6c75 6d6e 73da 0877 6172  _y..columns..war
-00000810: 6e69 6e67 73da 0477 6172 6e72 0a00 0000  nings..warnr....
-00000820: da05 656d 7074 7972 1600 0000 2905 7220  ..emptyr....).r 
-00000830: 0000 0072 2b00 0000 720a 0000 00da 0d72  ...r+...r......r
-00000840: 6571 7569 7265 645f 636f 6c73 722d 0000  equired_colsr-..
-00000850: 0072 2200 0000 722e 0000 0072 2300 0000  .r"...r....r#...
-00000860: 7218 0000 003b 0000 0073 1e00 0000 0003  r....;...s......
-00000870: 0601 0601 0601 0601 06fb 0206 02fa 0407  ................
-00000880: 0801 0a01 0c03 1603 0601 0801 7a1e 5370  ............z.Sp
-00000890: 6174 6961 6c44 6174 6173 6574 2e63 6865  atialDataset.che
-000008a0: 636b 5f69 6e70 7574 5f63 7376 6301 0000  ck_input_csvc...
-000008b0: 0000 0000 0000 0000 0003 0000 000a 0000  ................
-000008c0: 0043 0000 0073 4800 0000 7a10 7400 a001  .C...sH...z.t...
-000008d0: 7c00 6a02 a101 7d01 5700 6e32 0400 7403  |.j...}.W.n2..t.
-000008e0: 7942 0100 7d02 0100 7a1a 7404 6401 7c02  yB..}...z.t.d.|.
-000008f0: 9b00 9d02 8301 0100 5700 5900 6400 7d02  ........W.Y.d.}.
-00000900: 7e02 6e0a 6400 7d02 7e02 3000 3000 7c01  ~.n.d.}.~.0.0.|.
-00000910: 5300 2902 4e7a 1945 7272 6f72 206c 6f61  S.).Nz.Error loa
-00000920: 6469 6e67 2069 6e70 7574 2043 5356 3a20  ding input CSV: 
-00000930: 2905 da02 7064 da08 7265 6164 5f63 7376  )...pd..read_csv
-00000940: 7209 0000 00da 0945 7863 6570 7469 6f6e  r......Exception
-00000950: da05 7072 696e 7429 0372 2000 0000 7221  ..print).r ...r!
-00000960: 0000 00da 0165 7222 0000 0072 2200 0000  .....er"...r"...
-00000970: 7223 0000 0072 1700 0000 5000 0000 730a  r#...r....P...s.
-00000980: 0000 0000 0102 0110 010e 0124 017a 1d53  ...........$.z.S
-00000990: 7061 7469 616c 4461 7461 7365 742e 6c6f  patialDataset.lo
-000009a0: 6164 5f69 6e70 7574 5f63 7376 e910 0000  ad_input_csv....
-000009b0: 00e9 0300 0000 5429 06da 0c63 656c 6c5f  ......T)...cell_
-000009c0: 746f 5f6d 6173 6bda 0a70 6174 6368 5f73  to_mask..patch_s
-000009d0: 697a 65da 0a70 6978 656c 5f73 697a 65da  ize..pixel_size.
-000009e0: 0a63 656c 6c5f 7479 7065 73da 0473 6176  .cell_types..sav
-000009f0: 65da 0973 6176 655f 7061 7468 6307 0000  e..save_pathc...
-00000a00: 0000 0000 0000 0000 0010 0000 0009 0000  ................
-00000a10: 0043 0000 0073 dc01 0000 7c05 725a 7c06  .C...s....|.rZ|.
-00000a20: 6401 7501 7210 7c06 6e12 7400 6a01 a002  d.u.r.|.n.t.j...
-00000a30: 7c00 6a03 7404 6a05 6a06 a102 7c00 5f07  |.j.t.j.j...|._.
-00000a40: 7400 6a01 a008 7c00 6a07 a101 725a 7409  t.j...|.j...rZt.
-00000a50: 6402 7c00 6a07 9b00 6403 9d03 8301 0100  d.|.j...d.......
-00000a60: 7c00 a00a a100 0100 7c00 a00b a100 0100  |.......|.......
-00000a70: 6401 5300 7409 6404 7c02 9b00 6405 7c02  d.S.t.d.|...d.|.
-00000a80: 9b00 6406 9d05 8301 0100 7409 6407 7c03  ..d.......t.d.|.
-00000a90: 9b00 6405 7c03 9b00 6408 9d05 8301 0100  ..d.|...d.......
-00000aa0: 7409 6409 7c04 9b00 9d02 8301 0100 7409  t.d.|.........t.
-00000ab0: 640a 7c01 9b00 9d02 8301 0100 7c00 a00c  d.|.........|...
-00000ac0: a100 7d07 740d 7c07 7c02 7c03 7c04 7c00  ..}.t.|.|.|.|.|.
-00000ad0: 6a0e 7c01 8306 5c02 7d08 7d09 7c09 a00f  j.|...\.}.}.|...
-00000ae0: a100 6a10 640b 7411 6a12 6a06 6901 640c  ..j.d.t.j.j.i.d.
-00000af0: 8d01 7d09 7c08 6a13 5c04 7d0a 7d0b 7d0c  ..}.|.j.\.}.}.}.
-00000b00: 7d0d 7c0d 7414 7c00 6a0e 8301 6b03 72fe  }.|.t.|.j...k.r.
-00000b10: 7415 640d 8301 8201 7c0b 7c02 6b03 9001  t.d.....|.|.k...
-00000b20: 7312 7c0c 7c02 6b03 9001 721a 7415 640e  s.|.|.k...r.t.d.
-00000b30: 8301 8201 7c0a 7414 7c09 8301 6b03 9001  ....|.t.|...k...
-00000b40: 7230 7415 640f 8301 8201 7c05 9001 72d8  r0t.d.....|...r.
-00000b50: 7416 a017 7c00 6a07 6410 a102 8f62 7d0e  t...|.j.d....b}.
-00000b60: 7c0e 6a18 6411 7c08 6412 7419 7c0a 6413  |.j.d.|.d.t.|.d.
-00000b70: 8302 7c0b 7c0c 7c0d 6604 7c08 6a1a 6414  ..|.|.|.f.|.j.d.
-00000b80: 8d05 0100 7c09 6a1b 6415 6416 8d01 7d0f  ....|.j.d.d...}.
-00000b90: 7c0e 6a18 6417 7c0f 7c0f 6a1a 6418 8d03  |.j.d.|.|.j.d...
-00000ba0: 0100 7c0e 6a18 6419 7c00 6a0e 641a 8d02  ..|.j.d.|.j.d...
-00000bb0: 0100 5700 6401 0400 0400 8303 0100 6e12  ..W.d.........n.
-00000bc0: 3100 9001 73ae 3000 0100 0100 0100 5900  1...s.0.......Y.
-00000bd0: 0100 7409 641b 7c00 6a07 9b00 9d02 8301  ..t.d.|.j.......
-00000be0: 0100 7c00 a00a a100 0100 7c00 a00b a100  ..|.......|.....
-00000bf0: 0100 6401 5300 291c 61ca 0100 000a 2020  ..d.S.).a.....  
-00000c00: 2020 2020 2020 4765 6e65 7261 7465 206d        Generate m
-00000c10: 6173 6b65 6420 7061 7463 6865 7320 6672  asked patches fr
-00000c20: 6f6d 2074 6865 2069 6e70 7574 2064 6174  om the input dat
-00000c30: 612e 0a0a 2020 2020 2020 2020 4172 6773  a...        Args
-00000c40: 3a0a 2020 2020 2020 2020 2020 2020 6365  :.            ce
-00000c50: 6c6c 5f74 6f5f 6d61 736b 2028 7374 7229  ll_to_mask (str)
-00000c60: 3a20 5468 6520 6365 6c6c 2074 7970 6520  : The cell type 
-00000c70: 746f 206d 6173 6b2e 0a20 2020 2020 2020  to mask..       
-00000c80: 2020 2020 2070 6174 6368 5f73 697a 6520       patch_size 
-00000c90: 2869 6e74 293a 2054 6865 2073 697a 6520  (int): The size 
-00000ca0: 6f66 2074 6865 2070 6174 6368 2069 6e20  of the patch in 
-00000cb0: 7069 7865 6c73 2e0a 2020 2020 2020 2020  pixels..        
-00000cc0: 2020 2020 7069 7865 6c5f 7369 7a65 2028      pixel_size (
-00000cd0: 696e 7429 3a20 5468 6520 7069 7865 6c20  int): The pixel 
-00000ce0: 7369 7a65 2069 6e20 6d69 6372 6f6e 732e  size in microns.
-00000cf0: 0a20 2020 2020 2020 2020 2020 2063 656c  .            cel
-00000d00: 6c5f 7479 7065 7320 286c 6973 7429 3a20  l_types (list): 
-00000d10: 5468 6520 6365 6c6c 2074 7970 6573 2074  The cell types t
-00000d20: 6f20 696e 636c 7564 6520 696e 2074 6865  o include in the
-00000d30: 206d 6574 6164 6174 612e 0a20 2020 2020   metadata..     
-00000d40: 2020 2020 2020 2073 6176 6520 2862 6f6f         save (boo
-00000d50: 6c29 3a20 5768 6574 6865 7220 746f 2073  l): Whether to s
-00000d60: 6176 6520 7468 6520 7061 7463 6865 732e  ave the patches.
-00000d70: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
-00000d80: 655f 7061 7468 2028 7374 7229 3a20 5468  e_path (str): Th
-00000d90: 6520 7061 7468 2074 6f20 7361 7665 2074  e path to save t
-00000da0: 6865 2070 6174 6368 6573 2e0a 0a20 2020  he patches...   
-00000db0: 2020 2020 2052 6574 7572 6e73 3a0a 0a20       Returns:.. 
-00000dc0: 2020 2020 2020 204e 7a05 4669 6c65 207a         Nz.File z
-00000dd0: 2320 616c 7265 6164 7920 6578 6973 7473  # already exists
-00000de0: 2c20 6e6f 7420 7361 7669 6e67 2070 6174  , not saving pat
-00000df0: 6368 6573 7a1b 4765 6e65 7261 7469 6e67  chesz.Generating
-00000e00: 2070 6174 6368 6573 206f 6620 7369 7a65   patches of size
-00000e10: 20da 0178 7a07 2070 6978 656c 737a 0c50   ..xz. pixelsz.P
-00000e20: 6978 656c 2073 697a 653a 207a 0820 6d69  ixel size: z. mi
-00000e30: 6372 6f6e 737a 1543 656c 6c20 7479 7065  cronsz.Cell type
-00000e40: 7320 7265 636f 7264 6564 3a20 7a13 4365  s recorded: z.Ce
-00000e50: 6c6c 2074 7970 6573 206d 6173 6b65 643a  ll types masked:
-00000e60: 20da 0569 6e64 6578 2901 7236 0000 00fa   ..index).r6....
-00000e70: 344e 756d 6265 7220 6f66 2063 6861 6e6e  4Number of chann
-00000e80: 656c 206e 616d 6573 2064 6f20 6e6f 7420  el names do not 
-00000e90: 6d61 7463 6820 6461 7461 2064 696d 656e  match data dimen
-00000ea0: 7369 6f6e 737a 3550 6174 6368 2064 696d  sionsz5Patch dim
-00000eb0: 656e 7369 6f6e 7320 646f 206e 6f74 206d  ensions do not m
-00000ec0: 6174 6368 2074 6865 2065 7870 6563 7465  atch the expecte
-00000ed0: 6420 6469 6d65 6e73 696f 6e73 7a33 4e75  d dimensionsz3Nu
-00000ee0: 6d62 6572 206f 6620 7061 7463 6865 7320  mber of patches 
-00000ef0: 6765 6e65 7261 7465 6420 646f 6573 206e  generated does n
-00000f00: 6f74 206d 6174 6368 206d 6574 6164 6174  ot match metadat
-00000f10: 61da 0177 da06 696d 6167 6573 da04 677a  a..w..images..gz
-00000f20: 6970 e964 0000 0029 0472 2100 0000 da0b  ip.d...).r!.....
-00000f30: 636f 6d70 7265 7373 696f 6eda 0663 6875  compression..chu
-00000f40: 6e6b 73da 0564 7479 7065 46a9 0172 4900  nks..dtypeF..rI.
-00000f50: 0000 7210 0000 0029 0272 2100 0000 7251  ..r....).r!...rQ
-00000f60: 0000 0072 0a00 0000 2901 7221 0000 007a  ...r....).r!...z
-00000f70: 1150 6174 6368 6573 2073 6176 6564 2074  .Patches saved t
-00000f80: 6f20 291c 7211 0000 0072 1200 0000 da04  o ).r....r......
-00000f90: 6a6f 696e 7214 0000 0072 0700 0000 da05  joinr....r......
-00000fa0: 7061 7463 6872 2600 0000 720b 0000 00da  patchr&...r.....
-00000fb0: 0669 7366 696c 6572 3e00 0000 721d 0000  .isfiler>...r...
-00000fc0: 0072 1e00 0000 7217 0000 0072 0300 0000  .r....r....r....
-00000fd0: 720a 0000 00da 0b72 6573 6574 5f69 6e64  r......reset_ind
-00000fe0: 6578 da06 7265 6e61 6d65 7204 0000 00da  ex..renamer.....
-00000ff0: 0870 6174 6368 5f69 64da 0573 6861 7065  .patch_id..shape
-00001000: 7215 0000 0072 1600 0000 da04 6835 7079  r....r......h5py
-00001010: da04 4669 6c65 da0e 6372 6561 7465 5f64  ..File..create_d
-00001020: 6174 6173 6574 da03 6d69 6e72 5100 0000  ataset..minrQ...
-00001030: da0a 746f 5f72 6563 6f72 6473 2910 7220  ..to_records).r 
-00001040: 0000 0072 4200 0000 7243 0000 0072 4400  ...rB...rC...rD.
-00001050: 0000 7245 0000 0072 4600 0000 7247 0000  ..rE...rF...rG..
-00001060: 00da 0264 66da 0d70 6174 6368 6573 5f61  ...df..patches_a
-00001070: 7272 6179 da0b 6d65 7461 6461 7461 5f64  rray..metadata_d
-00001080: 66da 016e da01 6872 4b00 0000 da01 63da  f..n..hrK.....c.
-00001090: 0166 da0e 6d65 7461 6461 7461 5f6e 756d  .f..metadata_num
-000010a0: 7079 7222 0000 0072 2200 0000 7223 0000  pyr"...r"...r#..
-000010b0: 00da 1567 656e 6572 6174 655f 6d61 736b  ...generate_mask
-000010c0: 6564 5f70 6174 6368 5700 0000 735c 0000  ed_patchW...s\..
-000010d0: 0000 1804 0306 ff06 0212 fd04 050e 0112  ................
-000010e0: 0108 0108 0104 0316 0116 010e 010e 0308  ................
-000010f0: 0302 010e ff08 0308 010a ff06 030e 030e  ................
-00001100: 0108 0314 0108 030e 0108 0206 0110 0204  ................
-00001110: 0102 0102 0102 0110 0104 fb06 090c 0104  ................
-00001120: 0108 ff06 0530 0110 0108 0108 017a 2453  .....0.......z$S
-00001130: 7061 7469 616c 4461 7461 7365 742e 6765  patialDataset.ge
-00001140: 6e65 7261 7465 5f6d 6173 6b65 645f 7061  nerate_masked_pa
-00001150: 7463 6829 0172 0b00 0000 6302 0000 0000  tch).r....c.....
-00001160: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00001170: 0000 0073 3400 0000 7c01 6400 7501 720c  ...s4...|.d.u.r.
-00001180: 7c01 6e12 7400 6a01 a002 7c00 6a03 7404  |.n.t.j...|.j.t.
-00001190: 6a05 6a06 a102 7d02 7400 6a01 a007 7c02  j.j...}.t.j...|.
-000011a0: a101 7230 7c02 5300 6400 5300 7225 0000  ..r0|.S.d.S.r%..
-000011b0: 0029 0872 1100 0000 7212 0000 0072 5300  .).r....r....rS.
-000011c0: 0000 7214 0000 0072 0700 0000 7254 0000  ..r....r....rT..
-000011d0: 0072 2600 0000 7255 0000 0029 0372 2000  .r&...rU...).r .
-000011e0: 0000 720b 0000 0072 1200 0000 7222 0000  ..r....r....r"..
-000011f0: 0072 2200 0000 7223 0000 0072 1900 0000  .r"...r#...r....
-00001200: b100 0000 730a 0000 0000 0306 ff06 0212  ....s...........
-00001210: fd02 057a 1d53 7061 7469 616c 4461 7461  ...z.SpatialData
-00001220: 7365 742e 7365 745f 7061 7463 685f 7061  set.set_patch_pa
-00001230: 7468 2901 720c 0000 0063 0200 0000 0000  th).r....c......
-00001240: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-00001250: 0000 7334 0000 007c 0164 0075 0172 0c7c  ..s4...|.d.u.r.|
-00001260: 016e 1274 006a 01a0 027c 006a 0374 046a  .n.t.j...|.j.t.j
-00001270: 056a 06a1 027d 0274 006a 01a0 077c 02a1  .j...}.t.j...|..
-00001280: 0172 307c 0253 0064 0053 0072 2500 0000  .r0|.S.d.S.r%...
-00001290: 2908 7211 0000 0072 1200 0000 7253 0000  ).r....r....rS..
-000012a0: 0072 1400 0000 7206 0000 0072 2a00 0000  .r....r....r*...
-000012b0: 7226 0000 00da 0569 7364 6972 2903 7220  r&.....isdir).r 
-000012c0: 0000 0072 0c00 0000 da03 6469 7272 2200  ...r......dirr".
-000012d0: 0000 7222 0000 0072 2300 0000 721a 0000  ..r"...r#...r...
-000012e0: 00b9 0000 0073 0a00 0000 0003 06ff 0602  .....s..........
-000012f0: 12fd 0205 7a1c 5370 6174 6961 6c44 6174  ....z.SpatialDat
-00001300: 6173 6574 2e73 6574 5f73 706c 6974 5f64  aset.set_split_d
-00001310: 6972 2901 720d 0000 0063 0200 0000 0000  ir).r....c......
-00001320: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-00001330: 0000 7334 0000 007c 0164 0075 0172 0c7c  ..s4...|.d.u.r.|
-00001340: 016e 1274 006a 01a0 027c 006a 0374 046a  .n.t.j...|.j.t.j
-00001350: 056a 06a1 027d 0274 006a 01a0 077c 02a1  .j...}.t.j...|..
-00001360: 0172 307c 0253 0064 0053 0072 2500 0000  .r0|.S.d.S.r%...
-00001370: 2908 7211 0000 0072 1200 0000 7253 0000  ).r....r....rS..
-00001380: 0072 1400 0000 7206 0000 00da 056d 6f64  .r....r......mod
-00001390: 656c 7226 0000 0072 6800 0000 2903 7220  elr&...rh...).r 
-000013a0: 0000 0072 0d00 0000 7269 0000 0072 2200  ...r....ri...r".
-000013b0: 0000 7222 0000 0072 2300 0000 721b 0000  ..r"...r#...r...
-000013c0: 00c1 0000 0073 0a00 0000 0003 06ff 0602  .....s..........
-000013d0: 12fd 0205 7a1c 5370 6174 6961 6c44 6174  ....z.SpatialDat
-000013e0: 6173 6574 2e73 6574 5f6d 6f64 656c 5f64  aset.set_model_d
-000013f0: 6972 2901 720e 0000 0063 0200 0000 0000  ir).r....c......
-00001400: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-00001410: 0000 7334 0000 007c 0164 0075 0172 0c7c  ..s4...|.d.u.r.|
-00001420: 016e 1274 006a 01a0 027c 006a 0374 046a  .n.t.j...|.j.t.j
-00001430: 056a 06a1 027d 0274 006a 01a0 077c 02a1  .j...}.t.j...|..
-00001440: 0172 307c 0253 0064 0053 0072 2500 0000  .r0|.S.d.S.r%...
-00001450: 2908 7211 0000 0072 1200 0000 7253 0000  ).r....r....rS..
-00001460: 0072 1400 0000 7206 0000 00da 0e63 6f75  .r....r......cou
-00001470: 6e74 6572 6661 6374 7561 6c72 2600 0000  nterfactualr&...
-00001480: 7268 0000 0029 0372 2000 0000 720e 0000  rh...).r ...r...
-00001490: 0072 6900 0000 7222 0000 0072 2200 0000  .ri...r"...r"...
-000014a0: 7223 0000 0072 1c00 0000 c900 0000 730a  r#...r........s.
-000014b0: 0000 0000 0306 ff06 0212 fd02 057a 2553  .............z%S
-000014c0: 7061 7469 616c 4461 7461 7365 742e 7365  patialDataset.se
-000014d0: 745f 636f 756e 7465 7266 6163 7475 616c  t_counterfactual
-000014e0: 5f64 6972 6301 0000 0000 0000 0000 0000  _dirc...........
-000014f0: 0002 0000 0004 0000 0043 0000 0073 9400  .........C...s..
-00001500: 0000 7400 7c00 6401 8302 7312 7401 6402  ..t.|.d...s.t.d.
-00001510: 8301 8201 7400 7c00 6403 8302 7324 7401  ....t.|.d...s$t.
-00001520: 6404 8301 8201 7402 7c00 6a03 8301 7c00  d.....t.|.j...|.
-00001530: 6a03 7404 6a05 6a06 1900 a007 a100 6b03  j.t.j.j.......k.
-00001540: 7248 7401 6405 8301 8201 7402 7c00 6a08  rHt.d.....t.|.j.
-00001550: 8301 7c00 6a09 6b03 7260 7401 6406 8301  ..|.j.k.r`t.d...
-00001560: 8201 7404 6a0a 6a06 7404 6a05 6a06 6602  ..t.j.j.t.j.j.f.
-00001570: 4400 5d1e 7d01 7c01 7c00 6a03 6a0b 7601  D.].}.|.|.j.j.v.
-00001580: 7270 7401 6407 7c01 9b00 9d02 8301 8201  rpt.d.|.........
-00001590: 7170 6400 5300 2908 4e72 1000 0000 7a13  qpd.S.).Nr....z.
-000015a0: 4d65 7461 6461 7461 206e 6f74 206c 6f61  Metadata not loa
-000015b0: 6465 6472 0a00 0000 7a18 4368 616e 6e65  dedr....z.Channe
-000015c0: 6c20 6e61 6d65 7320 6e6f 7420 6c6f 6164  l names not load
-000015d0: 6564 7a25 4d65 7461 6461 7461 2063 6f6e  edz%Metadata con
-000015e0: 7461 696e 7320 6475 706c 6963 6174 6520  tains duplicate 
-000015f0: 7061 7463 6820 4944 7372 4a00 0000 7a19  patch IDsrJ...z.
-00001600: 4d65 7461 6461 7461 206d 6973 7369 6e67  Metadata missing
-00001610: 2063 6f6c 756d 6e3a 2029 0cda 0768 6173   column: )...has
-00001620: 6174 7472 7216 0000 0072 1500 0000 7210  attrr....r....r.
-00001630: 0000 0072 0400 0000 7258 0000 0072 2600  ...r....rX...r&.
-00001640: 0000 da07 6e75 6e69 7175 6572 0a00 0000  ....nuniquer....
-00001650: da0a 6e5f 6368 616e 6e65 6c73 7231 0000  ..n_channelsr1..
-00001660: 0072 3600 0000 2902 7220 0000 0072 2d00  .r6...).r ...r-.
-00001670: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
-00001680: 0072 1e00 0000 d100 0000 7316 0000 0000  .r........s.....
-00001690: 020a 0108 010a 0108 031c 0108 0110 0108  ................
-000016a0: 0314 010c 017a 2153 7061 7469 616c 4461  .....z!SpatialDa
-000016b0: 7461 7365 742e 6368 6563 6b5f 6c6f 6164  taset.check_load
-000016c0: 6564 5f70 6174 6368 6301 0000 0000 0000  ed_patchc.......
-000016d0: 0000 0000 0004 0000 000a 0000 0043 0000  .............C..
-000016e0: 0073 ce00 0000 7a96 7400 a001 7c00 6a02  .s....z.t...|.j.
-000016f0: 6401 a102 8f74 7d01 7403 a004 7c01 6402  d....t}.t...|.d.
-00001700: 1900 6400 6400 8502 1900 a101 7c00 5f05  ..d.d.......|._.
-00001710: 6403 6404 8400 7c01 6405 1900 6400 6400  d.d...|.d...d.d.
-00001720: 8502 1900 4400 8301 7c00 5f06 7c01 6406  ....D...|._.|.d.
-00001730: 1900 6a07 7d02 7c02 6407 1900 7c02 6408  ..j.}.|.d...|.d.
-00001740: 6409 8502 1900 7c02 6409 1900 0300 0200  d.....|.d.......
-00001750: 7c00 5f08 7c00 5f09 7c00 5f0a 5700 6400  |._.|._.|._.W.d.
-00001760: 0400 0400 8303 0100 6e10 3100 738a 3000  ........n.1.s.0.
-00001770: 0100 0100 0100 5900 0100 5700 6e32 0400  ......Y...W.n2..
-00001780: 740b 79c8 0100 7d03 0100 7a1a 740c 640a  t.y...}...z.t.d.
-00001790: 7c03 9b00 9d02 8301 0100 5700 5900 6400  |.........W.Y.d.
-000017a0: 7d03 7e03 6e0a 6400 7d03 7e03 3000 3000  }.~.n.d.}.~.0.0.
-000017b0: 6400 5300 290b 4eda 0172 7210 0000 0063  d.S.).N..rr....c
-000017c0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000017d0: 0500 0000 5300 0000 7316 0000 0067 007c  ....S...s....g.|
-000017e0: 005d 0e7d 017c 01a0 0064 00a1 0191 0271  .].}.|...d.....q
-000017f0: 0453 0029 017a 0575 7466 2d38 2901 da06  .S.).z.utf-8)...
-00001800: 6465 636f 6465 2902 722c 0000 00da 046e  decode).r,.....n
-00001810: 616d 6572 2200 0000 7222 0000 0072 2300  amer"...r"...r#.
-00001820: 0000 722f 0000 00e7 0000 0073 0200 0000  ..r/.......s....
-00001830: 0601 7a32 5370 6174 6961 6c44 6174 6173  ..z2SpatialDatas
-00001840: 6574 2e6c 6f61 645f 7061 7463 685f 6461  et.load_patch_da
-00001850: 7461 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ta.<locals>.<lis
-00001860: 7463 6f6d 703e 720a 0000 0072 4c00 0000  tcomp>r....rL...
-00001870: 7201 0000 00e9 0100 0000 7241 0000 007a  r.........rA...z
-00001880: 1445 7272 6f72 206c 6f61 6469 6e67 2064  .Error loading d
-00001890: 6174 613a 2029 0d72 5a00 0000 725b 0000  ata: ).rZ...r[..
-000018a0: 0072 0b00 0000 723b 0000 00da 0944 6174  .r....r;.....Dat
-000018b0: 6146 7261 6d65 7210 0000 0072 0a00 0000  aFramer....r....
-000018c0: 7259 0000 00da 096e 5f70 6174 6368 6573  rY.....n_patches
-000018d0: da08 696d 675f 7369 7a65 726e 0000 0072  ..img_sizern...r
-000018e0: 3d00 0000 723e 0000 0029 0472 2000 0000  =...r>...).r ...
-000018f0: 7265 0000 00da 0a64 6174 615f 7368 6170  re.....data_shap
-00001900: 6572 3f00 0000 7222 0000 0072 2200 0000  er?...r"...r"...
-00001910: 7223 0000 0072 1d00 0000 e300 0000 731a  r#...r........s.
-00001920: 0000 0000 0102 0110 0118 0106 010e ff08  ................
-00001930: 030a 0206 010a 0106 fd32 050e 017a 1e53  .........2...z.S
-00001940: 7061 7469 616c 4461 7461 7365 742e 6c6f  patialDataset.lo
-00001950: 6164 5f70 6174 6368 5f64 6174 6129 01da  ad_patch_data)..
-00001960: 0a73 706c 6974 5f6e 616d 6563 0200 0000  .split_namec....
-00001970: 0000 0000 0000 0000 0400 0000 0a00 0000  ................
-00001980: 4300 0000 736a 0000 0074 006a 01a0 027c  C...sj...t.j...|
-00001990: 006a 037c 0174 046a 056a 06a1 037d 027a  .j.|.t.j.j...}.z
-000019a0: 1674 07a0 087c 02a1 0174 096a 0a6a 0619  .t...|...t.j.j..
-000019b0: 006a 0b57 0053 0004 0074 0c79 6401 007d  .j.W.S...t.yd..}
-000019c0: 0301 007a 2074 0d64 017c 019b 0064 027c  ...z t.d.|...d.|
-000019d0: 039b 009d 0483 0101 0057 0059 0064 007d  .........W.Y.d.}
-000019e0: 037e 036e 0a64 007d 037e 0330 0030 0064  .~.n.d.}.~.0.0.d
-000019f0: 0053 0029 034e 7a14 4572 726f 7220 6c6f  .S.).Nz.Error lo
-00001a00: 6164 696e 6720 7370 6c69 7420 fa02 3a20  ading split ..: 
-00001a10: 290e 7211 0000 0072 1200 0000 7253 0000  ).r....r....rS..
-00001a20: 0072 0c00 0000 7207 0000 00da 056c 6162  .r....r......lab
-00001a30: 656c 7226 0000 0072 3b00 0000 723c 0000  elr&...r;...r<..
-00001a40: 0072 0400 0000 7258 0000 00da 0676 616c  .r....rX.....val
-00001a50: 7565 7372 3d00 0000 723e 0000 0029 0472  uesr=...r>...).r
-00001a60: 2000 0000 7277 0000 00da 0a6c 6162 656c   ...rw.....label
-00001a70: 5f70 6174 6872 3f00 0000 7222 0000 0072  _pathr?...r"...r
-00001a80: 2200 0000 7223 0000 0072 2800 0000 f300  "...r#...r(.....
-00001a90: 0000 730e 0000 0000 0106 010c ff04 0302  ..s.............
-00001aa0: 0116 010e 017a 1c53 7061 7469 616c 4461  .....z.SpatialDa
-00001ab0: 7461 7365 742e 6765 745f 7370 6c69 745f  taset.get_split_
-00001ac0: 6964 73e7 3333 3333 3333 e33f e79a 9999  ids.333333.?....
-00001ad0: 9999 99c9 3f29 04da 0b73 7472 6174 6966  ....?)...stratif
-00001ae0: 795f 6279 da0a 7472 6169 6e5f 7369 7a65  y_by..train_size
-00001af0: da08 7661 6c5f 7369 7a65 da09 7465 7374  ..val_size..test
-00001b00: 5f73 697a 6563 0b00 0000 0000 0000 0000  _sizec..........
-00001b10: 0000 0c00 0000 0700 0000 0300 0000 73fa  ..............s.
-00001b20: 0000 007c 017c 005f 007c 0864 0175 0072  ...|.|._.|.d.u.r
-00001b30: 1a64 0264 0364 0464 059c 037d 087c 0564  .d.d.d.d...}.|.d
-00001b40: 0175 0072 3a74 016a 02a0 037c 006a 0474  .u.r:t.j...|.j.t
-00001b50: 056a 066a 07a1 027c 005f 086e 067c 057c  .j.j...|._.n.|.|
-00001b60: 005f 0874 016a 02a0 0974 016a 02a0 037c  ._.t.j...t.j...|
-00001b70: 006a 0874 0a6a 0b6a 07a1 02a1 0172 7074  .j.t.j.j.....rpt
-00001b80: 0c64 067c 006a 089b 009d 0283 0101 0064  .d.|.j.........d
-00001b90: 0153 0074 0c64 0783 0101 0088 0064 0175  .S.t.d.......d.u
-00001ba0: 0172 9887 0066 0164 0864 0984 0874 0d74  .r...f.d.d...t.t
-00001bb0: 0a83 0144 0083 017d 0b6e 1c7c 006a 0e7c  ...D...}.n.|.j.|
-00001bc0: 017c 027c 037c 047c 067c 0766 0669 007c  .|.|.|.|.|.f.i.|
-00001bd0: 08a4 018e 017d 0b7c 0b64 0175 0072 c474  .....}.|.d.u.r.t
-00001be0: 0f64 0a83 0182 017c 0a72 f674 0c64 0b83  .d.....|.r.t.d..
-00001bf0: 0101 007c 006a 107c 0b7c 0164 0c8d 0201  ...|.j.|.|.d....
-00001c00: 0074 0c64 0d7c 006a 089b 009d 0283 0101  .t.d.|.j........
-00001c10: 007c 00a0 11a1 0001 007c 0b53 0029 0e61  .|.......|.S.).a
-00001c20: 0305 0000 0a20 2020 2020 2020 2047 656e  .....        Gen
-00001c30: 6572 6174 6520 7472 6169 6e2c 2076 616c  erate train, val
-00001c40: 6964 6174 696f 6e2c 2061 6e64 2074 6573  idation, and tes
-00001c50: 7420 6461 7461 2073 706c 6974 732c 2061  t data splits, a
-00001c60: 6e64 2073 6176 6520 7468 6520 6461 7461  nd save the data
-00001c70: 2073 706c 6974 7320 746f 2074 6865 2067   splits to the g
-00001c80: 6976 656e 2064 6972 6563 746f 7279 0a0a  iven directory..
-00001c90: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00001ca0: 2020 2020 2020 7374 7261 7469 6679 5f62        stratify_b
-00001cb0: 793a 2073 7472 0a20 2020 2020 2020 2020  y: str.         
-00001cc0: 2020 2054 6865 2063 6f6c 756d 6e20 6e61     The column na
-00001cd0: 6d65 2074 6f20 7374 7261 7469 6679 2074  me to stratify t
-00001ce0: 6865 2064 6174 6120 6279 0a20 2020 2020  he data by.     
-00001cf0: 2020 2073 6176 655f 6469 723a 2073 7472     save_dir: str
-00001d00: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00001d10: 2064 6972 6563 746f 7279 2074 6f20 7361   directory to sa
-00001d20: 7665 2074 6865 2064 6174 6120 7370 6c69  ve the data spli
-00001d30: 7473 0a20 2020 2020 2020 2074 7261 696e  ts.        train
-00001d40: 5f73 697a 653a 2066 6c6f 6174 0a20 2020  _size: float.   
-00001d50: 2020 2020 2020 2020 2054 6865 2070 726f           The pro
-00001d60: 706f 7274 696f 6e20 6f66 2074 6865 2064  portion of the d
-00001d70: 6174 6173 6574 2074 6f20 696e 636c 7564  ataset to includ
-00001d80: 6520 696e 2074 6865 2074 7261 696e 2073  e in the train s
-00001d90: 706c 6974 0a20 2020 2020 2020 2076 616c  plit.        val
-00001da0: 5f73 697a 653a 2066 6c6f 6174 0a20 2020  _size: float.   
-00001db0: 2020 2020 2020 2020 2054 6865 2070 726f           The pro
-00001dc0: 706f 7274 696f 6e20 6f66 2074 6865 2064  portion of the d
-00001dd0: 6174 6173 6574 2074 6f20 696e 636c 7564  ataset to includ
-00001de0: 6520 696e 2074 6865 2076 616c 6964 6174  e in the validat
-00001df0: 696f 6e20 7370 6c69 740a 2020 2020 2020  ion split.      
-00001e00: 2020 7465 7374 5f73 697a 653a 2066 6c6f    test_size: flo
-00001e10: 6174 0a20 2020 2020 2020 2020 2020 2054  at.            T
-00001e20: 6865 2070 726f 706f 7274 696f 6e20 6f66  he proportion of
-00001e30: 2074 6865 2064 6174 6173 6574 2074 6f20   the dataset to 
-00001e40: 696e 636c 7564 6520 696e 2074 6865 2074  include in the t
-00001e50: 6573 7420 7370 6c69 740a 2020 2020 2020  est split.      
-00001e60: 2020 7261 6e64 6f6d 5f73 7461 7465 3a20    random_state: 
-00001e70: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00001e80: 436f 6e74 726f 6c73 2074 6865 2073 6875  Controls the shu
-00001e90: 6666 6c69 6e67 2061 7070 6c69 6564 2074  ffling applied t
-00001ea0: 6f20 7468 6520 6461 7461 2062 6566 6f72  o the data befor
-00001eb0: 6520 6170 706c 7969 6e67 2074 6865 2073  e applying the s
-00001ec0: 706c 6974 2e0a 2020 2020 2020 2020 7368  plit..        sh
-00001ed0: 7566 666c 653a 2062 6f6f 6c0a 2020 2020  uffle: bool.    
-00001ee0: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-00001ef0: 746f 2073 6875 6666 6c65 2074 6865 2064  to shuffle the d
-00001f00: 6174 6120 6265 666f 7265 2073 706c 6974  ata before split
-00001f10: 7469 6e67 0a20 2020 2020 2020 2074 6f6c  ting.        tol
-00001f20: 6572 616e 6365 3a20 6469 6374 0a20 2020  erance: dict.   
-00001f30: 2020 2020 2020 2020 2041 2064 6963 7469           A dicti
-00001f40: 6f6e 6172 7920 6f66 2074 6f6c 6572 616e  onary of toleran
-00001f50: 6365 2070 6172 616d 6574 6572 7320 746f  ce parameters to
-00001f60: 2063 6f6e 7472 6f6c 2074 6865 2064 6174   control the dat
-00001f70: 6120 7370 6c69 7420 6765 6e65 7261 7469  a split generati
-00001f80: 6f6e 0a20 2020 2020 2020 2020 2020 202d  on.            -
-00001f90: 2065 7073 3a20 666c 6f61 740a 2020 2020   eps: float.    
-00001fa0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00001fb0: 746f 6c65 7261 6e63 6520 666f 7220 7468  tolerance for th
-00001fc0: 6520 6469 6666 6572 656e 6365 2069 6e20  e difference in 
-00001fd0: 7072 6f70 6f72 7469 6f6e 7320 6265 7477  proportions betw
-00001fe0: 6565 6e20 7468 6520 7472 6169 6e20 616e  een the train an
-00001ff0: 6420 7465 7374 2f76 616c 6964 6174 6520  d test/validate 
-00002000: 7370 6c69 7473 0a20 2020 2020 2020 2020  splits.         
-00002010: 2020 202d 2074 7261 696e 5f6c 623a 2066     - train_lb: f
-00002020: 6c6f 6174 0a20 2020 2020 2020 2020 2020  loat.           
-00002030: 2020 2020 2054 6865 206c 6f77 6572 2062       The lower b
-00002040: 6f75 6e64 2066 6f72 2074 6865 2070 726f  ound for the pro
-00002050: 706f 7274 696f 6e20 6f66 2074 6865 2074  portion of the t
-00002060: 7261 696e 2073 706c 6974 0a20 2020 2020  rain split.     
-00002070: 2020 2020 2020 202d 206e 5f74 6f6c 3a20         - n_tol: 
-00002080: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00002090: 2020 2020 5468 6520 6e75 6d62 6572 206f      The number o
-000020a0: 6620 6174 7465 6d70 7473 2074 6f20 6765  f attempts to ge
-000020b0: 6e65 7261 7465 2061 2076 616c 6964 2064  nerate a valid d
-000020c0: 6174 6120 7370 6c69 740a 2020 2020 2020  ata split.      
-000020d0: 2020 7361 7665 3a20 626f 6f6c 0a20 2020    save: bool.   
-000020e0: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
-000020f0: 2074 6f20 7361 7665 2074 6865 2064 6174   to save the dat
-00002100: 6120 7370 6c69 7473 2074 6f20 7468 6520  a splits to the 
-00002110: 7361 7665 2064 6972 6563 746f 7279 0a20  save directory. 
-00002120: 2020 2020 2020 204e e77b 14ae 47e1 7a84         N.{..G.z.
-00002130: 3f67 0000 0000 0000 e03f 724e 0000 0029  ?g.......?rN...)
-00002140: 03da 0365 7073 da08 7472 6169 6e5f 6c62  ...eps..train_lb
-00002150: da05 6e5f 746f 6c7a 1d44 6174 6120 7370  ..n_tolz.Data sp
-00002160: 6c69 7473 2061 6c72 6561 6479 2065 7869  lits already exi
-00002170: 7374 2069 6e20 7a19 4765 6e65 7261 7469  st in z.Generati
-00002180: 6e67 2064 6174 6120 7370 6c69 7473 2e2e  ng data splits..
-00002190: 2e63 0100 0000 0000 0000 0000 0000 0300  .c..............
-000021a0: 0000 0700 0000 1300 0000 7322 0000 0069  ..........s"...i
-000021b0: 007c 005d 1a5c 027d 017d 027c 026a 0074  .|.].\.}.}.|.j.t
-000021c0: 01a0 0288 007c 0119 00a1 0193 0271 0453  .....|.......q.S
-000021d0: 0072 2200 0000 2903 7226 0000 00da 026e  .r"...).r&.....n
-000021e0: 70da 0561 7272 6179 2903 722c 0000 00da  p..array).r,....
-000021f0: 0369 6478 7271 0000 00a9 01da 0c67 6976  .idxrq.......giv
-00002200: 656e 5f73 706c 6974 7372 2200 0000 7223  en_splitsr"...r#
-00002210: 0000 00da 0a3c 6469 6374 636f 6d70 3e37  .....<dictcomp>7
-00002220: 0100 0073 0400 0000 0602 06ff 7a37 5370  ...s........z7Sp
-00002230: 6174 6961 6c44 6174 6173 6574 2e67 656e  atialDataset.gen
-00002240: 6572 6174 655f 6461 7461 5f73 706c 6974  erate_data_split
-00002250: 732e 3c6c 6f63 616c 733e 2e3c 6469 6374  s.<locals>.<dict
-00002260: 636f 6d70 3e7a 4943 6f75 6c64 206e 6f74  comp>zICould not
-00002270: 2073 6174 6973 6679 2064 6174 6120 7370   satisfy data sp
-00002280: 6c69 7420 636f 6e73 7472 6169 6e74 732c  lit constraints,
-00002290: 2074 7279 2061 6761 696e 206f 7220 6164   try again or ad
-000022a0: 6a75 7374 2063 6f6e 7374 7261 696e 7473  just constraints
-000022b0: 7a10 5361 7669 6e67 2073 706c 6974 732e  z.Saving splits.
-000022c0: 2e2e 2901 da0a 6c61 6265 6c5f 6e61 6d65  ..)...label_name
-000022d0: 7a15 4461 7461 2073 706c 6974 7320 7361  z.Data splits sa
-000022e0: 7665 6420 746f 2029 1272 8c00 0000 7211  ved to ).r....r.
-000022f0: 0000 0072 1200 0000 7253 0000 0072 1400  ...r....rS...r..
-00002300: 0000 7206 0000 0072 2a00 0000 7226 0000  ..r....r*...r&..
-00002310: 0072 0c00 0000 7268 0000 0072 0500 0000  .r....rh...r....
-00002320: da05 7472 6169 6e72 3e00 0000 da09 656e  ..trainr>.....en
-00002330: 756d 6572 6174 65da 1267 6574 5f70 6174  umerate..get_pat
-00002340: 6965 6e74 5f73 706c 6974 7372 1600 0000  ient_splitsr....
-00002350: da0b 7361 7665 5f73 706c 6974 7372 1f00  ..save_splitsr..
-00002360: 0000 290c 7220 0000 0072 7e00 0000 727f  ..).r ...r~...r.
-00002370: 0000 0072 8000 0000 7281 0000 00da 0873  ...r....r......s
-00002380: 6176 655f 6469 72da 0c72 616e 646f 6d5f  ave_dir..random_
-00002390: 7374 6174 65da 0773 6875 6666 6c65 da09  state..shuffle..
-000023a0: 746f 6c65 7261 6e63 6572 8a00 0000 7246  tolerancer....rF
-000023b0: 0000 00da 0d70 6174 6965 6e74 5f73 706c  .....patient_spl
-000023c0: 6974 7222 0000 0072 8900 0000 7223 0000  itr"...r....r#..
-000023d0: 00da 1467 656e 6572 6174 655f 6461 7461  ...generate_data
-000023e0: 5f73 706c 6974 73fc 0000 0073 4400 0000  _splits....sD...
-000023f0: 002a 0602 0801 0c01 0801 0601 0aff 0804  .*..............
-00002400: 0602 1c01 1001 0402 0801 0801 0a02 06fe  ................
-00002410: 0805 0401 0201 0201 0201 0201 0201 02fa  ................
-00002420: 0407 02f9 060a 0801 0802 0401 0801 0e01  ................
-00002430: 1001 0801 7a23 5370 6174 6961 6c44 6174  ....z#SpatialDat
-00002440: 6173 6574 2e67 656e 6572 6174 655f 6461  aset.generate_da
-00002450: 7461 5f73 706c 6974 7372 8200 0000 e7cd  ta_splitsr......
-00002460: cccc cccc cce4 3f63 0300 0000 0000 0000  ......?c........
-00002470: 0000 0000 0600 0000 0400 0000 4300 0000  ............C...
-00002480: 7370 0000 007c 0074 006a 016a 0219 0064  sp...|.t.j.j...d
-00002490: 0119 007d 0374 037c 0074 006a 016a 0219  ...}.t.|.t.j.j..
-000024a0: 0064 0219 007c 0074 006a 046a 0219 0064  .d...|.t.j.j...d
-000024b0: 0219 0018 0083 017d 0474 037c 0074 006a  .......}.t.|.t.j
-000024c0: 016a 0219 0064 0219 007c 0074 006a 056a  .j...d...|.t.j.j
-000024d0: 0219 0064 0219 0018 0083 017d 057c 047c  ...d.......}.|.|
-000024e0: 016b 006f 6e7c 057c 016b 006f 6e7c 037c  .k.on|.|.k.on|.|
-000024f0: 026b 0453 0029 034e 7201 0000 0072 7200  .k.S.).Nr....rr.
-00002500: 0000 2906 7205 0000 0072 8d00 0000 7226  ..).r....r....r&
-00002510: 0000 00da 0361 6273 da04 7465 7374 da08  .....abs..test..
-00002520: 7661 6c69 6461 7465 2906 da0a 7370 6c69  validate)...spli
-00002530: 745f 696e 666f 7283 0000 0072 8400 0000  t_infor....r....
-00002540: da07 7472 5f70 726f 70da 0a74 725f 7465  ..tr_prop..tr_te
-00002550: 5f64 6966 66da 0a74 725f 7661 5f64 6966  _diff..tr_va_dif
-00002560: 6672 2200 0000 7222 0000 0072 2300 0000  fr"...r"...r#...
-00002570: da0e 6973 5f76 616c 6964 5f73 706c 6974  ..is_valid_split
-00002580: 5001 0000 7310 0000 0000 0210 0102 011e  P...s...........
-00002590: ff04 0302 011e ff04 037a 1d53 7061 7469  .........z.Spati
-000025a0: 616c 4461 7461 7365 742e 6973 5f76 616c  alDataset.is_val
-000025b0: 6964 5f73 706c 6974 e92a 0000 0072 4e00  id_split.*...rN.
-000025c0: 0000 630a 0000 0000 0000 0000 0000 0017  ..c.............
-000025d0: 0000 0008 0000 0043 0000 0073 7001 0000  .......C...sp...
-000025e0: 7c02 7c03 1700 7c04 1700 6401 6b02 7318  |.|...|...d.k.s.
-000025f0: 4a00 6402 8301 8201 7400 a001 7c00 6a02  J.d.....t...|.j.
-00002600: 7403 6a04 6a05 1900 a101 7d0a 7406 7c00  t.j.j.....}.t.|.
-00002610: 6a02 8301 7d0b 6403 7d0c 6404 7d0d 7c0c  j...}.d.}.d.}.|.
-00002620: 9001 736c 7c0d 7c07 6b00 9001 726c 7c06  ..sl|.|.k...rl|.
-00002630: 7268 7400 6a07 a008 7c05 a101 7d0e 7c0e  rht.j...|...}.|.
-00002640: a009 7c0a a101 0100 740a 7406 7c0a 8301  ..|.....t.t.|...
-00002650: 7c02 1400 8301 7d0f 7c0f 740a 7406 7c0a  |.....}.|.t.t.|.
-00002660: 8301 7c03 1400 8301 1700 7d10 740b 6a0c  ..|.......}.t.j.
-00002670: 6a05 7c0a 6400 7c0f 8502 1900 740b 6a0d  j.|.d.|.....t.j.
-00002680: 6a05 7c0a 7c0f 7c10 8502 1900 740b 6a0e  j.|.|.|.....t.j.
-00002690: 6a05 7c0a 7c10 6400 8502 1900 6903 7d11  j.|.|.d.....i.}.
-000026a0: 6900 7d12 7c11 a00f a100 4400 5d3e 5c02  i.}.|.....D.]>\.
-000026b0: 7d13 7d14 7c00 6a02 7c00 6a02 7403 6a04  }.}.|.j.|.j.t.j.
-000026c0: 6a05 1900 a010 7c14 a101 1900 7d15 7406  j.....|.....}.t.
-000026d0: 7c15 8301 7c0b 1b00 7c15 7c01 1900 a011  |...|...|.|.....
-000026e0: a100 6702 7c12 7c13 3c00 71cc 7412 a013  ..g.|.|.<.q.t...
-000026f0: 7c12 7c08 7c09 a103 9001 7262 7414 6405  |.|.|.....rbt.d.
-00002700: 8301 0100 7c12 a00f a100 4400 5d30 5c02  ....|.....D.]0\.
-00002710: 7d13 7d16 7414 7c13 6406 9b04 6407 7c16  }.}.t.|.d...d.|.
-00002720: 6404 1900 6408 9b04 6409 7c16 6401 1900  d...d...d.|.d...
-00002730: 6408 9b04 9d05 8301 0100 9001 712c 7c11  d...........q,|.
-00002740: 5300 7c0d 6401 3700 7d0d 713e 6400 5300  S.|.d.7.}.q>d.S.
-00002750: 290a 4e72 7200 0000 7a33 7472 6169 6e5f  ).Nrr...z3train_
-00002760: 7369 7a65 2c20 7661 6c5f 7369 7a65 2c20  size, val_size, 
-00002770: 616e 6420 7465 7374 5f73 697a 6520 7368  and test_size sh
-00002780: 6f75 6c64 2073 756d 2074 6f20 3146 7201  ould sum to 1Fr.
-00002790: 0000 007a 4d53 706c 6974 2063 6f6e 7374  ...zMSplit const
-000027a0: 7261 696e 7473 2073 6174 6973 6669 6564  raints satisfied
-000027b0: 0a50 6174 6368 2070 726f 706f 7274 696f  .Patch proportio
-000027c0: 6e73 2061 6e64 2050 6f73 6974 6976 6520  ns and Positive 
-000027d0: 7061 7463 6820 7072 6f70 6f72 7469 6f6e  patch proportion
-000027e0: 733a 7a03 3c31 3072 7800 0000 7a05 3e35  s:z.<10rx...z.>5
-000027f0: 2e33 667a 022c 2029 1572 8600 0000 da06  .3fz., ).r......
-00002800: 756e 6971 7565 7210 0000 0072 0400 0000  uniquer....r....
-00002810: 7231 0000 0072 2600 0000 7215 0000 00da  r1...r&...r.....
-00002820: 0672 616e 646f 6dda 0b64 6566 6175 6c74  .random..default
-00002830: 5f72 6e67 7293 0000 00da 0369 6e74 7205  _rngr......intr.
-00002840: 0000 0072 8d00 0000 729a 0000 0072 9900  ...r....r....r..
-00002850: 0000 da05 6974 656d 73da 0469 7369 6eda  ....items..isin.
-00002860: 046d 6561 6e72 0800 0000 729f 0000 0072  .meanr....r....r
-00002870: 3e00 0000 2917 7220 0000 0072 7e00 0000  >...).r ...r~...
-00002880: 727f 0000 0072 8000 0000 7281 0000 0072  r....r....r....r
-00002890: 9200 0000 7293 0000 0072 8500 0000 7283  ....r....r....r.
-000028a0: 0000 0072 8400 0000 7231 0000 0072 7400  ...r....r1...rt.
-000028b0: 0000 da0c 6973 5661 6c69 6453 706c 6974  ....isValidSplit
-000028c0: da07 636f 756e 7465 72da 0372 6e67 da09  ..counter..rng..
-000028d0: 7472 6169 6e5f 656e 64da 0976 616c 6964  train_end..valid
-000028e0: 5f65 6e64 7295 0000 0072 9b00 0000 722a  _endr....r....r*
-000028f0: 0000 00da 0370 6174 da08 6461 7461 5f73  .....pat..data_s
-00002900: 7562 da03 6461 7472 2200 0000 7222 0000  ub..datr"...r"..
-00002910: 0072 2300 0000 728f 0000 005b 0100 0073  .r#...r....[...s
-00002920: 4600 0000 000d 0eff 0402 02fe 0404 1401  F...............
-00002930: 0a01 0401 0401 1001 0401 0c01 0a01 1001  ................
-00002940: 1402 1001 1001 10fd 0406 0401 1001 0401  ................
-00002950: 12ff 0404 0a01 0afe 0a05 1001 0201 02ff  ................
-00002960: 0403 1001 2a01 0402 0a01 7a21 5370 6174  ....*.....z!Spat
-00002970: 6961 6c44 6174 6173 6574 2e67 6574 5f70  ialDataset.get_p
-00002980: 6174 6965 6e74 5f73 706c 6974 7363 0100  atient_splitsc..
-00002990: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-000029a0: 0000 4300 0000 7304 0000 0064 0053 0072  ..C...s....d.S.r
-000029b0: 2500 0000 7222 0000 00a9 0172 2000 0000  %...r".....r ...
-000029c0: 7222 0000 0072 2200 0000 7223 0000 00da  r"...r"...r#....
-000029d0: 0f73 756d 6d61 7269 7a65 5f73 706c 6974  .summarize_split
-000029e0: 9001 0000 7302 0000 0000 017a 1e53 7061  ....s......z.Spa
-000029f0: 7469 616c 4461 7461 7365 742e 7375 6d6d  tialDataset.summ
-00002a00: 6172 697a 655f 7370 6c69 7463 0300 0000  arize_splitc....
-00002a10: 0000 0000 0000 0000 1200 0000 0900 0000  ................
-00002a20: 0300 0000 732c 0200 0064 0164 026c 006d  ....s,...d.d.l.m
-00002a30: 007d 0301 0087 0066 0164 0364 0484 087c  .}.....f.d.d...|
-00002a40: 01a0 01a1 0044 0083 017d 0474 02a0 0388  .....D...}.t....
-00002a50: 006a 0464 05a1 028f 207d 057c 0564 0619  .j.d.... }.|.d..
-00002a60: 0064 0064 0085 0219 007d 0657 0064 0004  .d.d.....}.W.d..
-00002a70: 0004 0083 0301 006e 1031 0073 5630 0001  .......n.1.sV0..
-00002a80: 0001 0001 0059 0001 0064 007d 077c 0374  .....Y...d.}.|.t
-00002a90: 0564 0764 088d 0244 0090 015d 707d 087c  .d.d...D...]p}.|
-00002aa0: 047c 086a 0619 007d 097c 067c 0964 0966  .|.j...}.|.|.d.f
-00002ab0: 0219 007d 0a88 006a 076a 087c 0919 007c  ...}...j.j.|...|
-00002ac0: 0219 006a 09a0 0a74 0ba1 017d 0b88 006a  ...j...t...}...j
-00002ad0: 076a 087c 0919 0074 0c6a 0d6a 0619 006a  .j.|...t.j.j...j
-00002ae0: 097d 0c88 006a 076a 087c 0919 0074 0c6a  .}...j.j.|...t.j
-00002af0: 0d6a 067c 0274 0c6a 0e6a 0674 0c6a 0f6a  .j.|.t.j.j.t.j.j
-00002b00: 0667 0419 007d 0d74 106a 11a0 1288 006a  .g...}.t.j.....j
-00002b10: 137c 086a 06a1 027d 0e74 106a 11a0 147c  .|.j...}.t.j...|
-00002b20: 0ea1 0190 0173 3074 10a0 157c 0ea1 0101  .....s0t...|....
-00002b30: 0074 10a0 1574 106a 11a0 127c 0e64 0aa1  .t...t.j...|.d..
-00002b40: 02a1 0101 0074 10a0 1574 106a 11a0 127c  .....t...t.j...|
-00002b50: 0e64 0ba1 02a1 0101 007c 0d6a 1674 106a  .d.......|.j.t.j
-00002b60: 11a0 127c 0e74 176a 186a 06a1 0264 0c64  ...|.t.j.j...d.d
-00002b70: 0d8d 0201 0074 197c 0b83 017d 0f7c 0374  .....t.|...}.|.t
-00002b80: 1a7c 0f83 0164 0e7c 086a 069b 0064 0f9d  .|...d.|.j...d..
-00002b90: 0364 0c64 108d 0344 005d 3c7d 1074 106a  .d.d...D.]<}.t.j
-00002ba0: 11a0 127c 0e7c 0b7c 1019 009b 0064 117c  ...|.|.|.....d.|
-00002bb0: 0c7c 1019 009b 0064 129d 04a1 027d 1174  .|.....d.....}.t
-00002bc0: 1ba0 1c7c 117c 0a7c 1064 0966 0219 00a1  ...|.|.|.d.f....
-00002bd0: 0201 0090 0171 707c 086a 0674 056a 1d6a  .....qp|.j.t.j.j
-00002be0: 066b 0272 7074 1b6a 1e7c 0a64 1364 148d  .k.rpt.j.|.d.d..
-00002bf0: 02a0 1fa1 0074 1b6a 207c 0a64 1364 148d  .....t.j |.d.d..
-00002c00: 02a0 1fa1 0064 159c 027d 0771 7074 2174  .....d...}.qpt!t
-00002c10: 106a 11a0 1288 006a 1364 16a1 0264 1783  .j.....j.d...d..
-00002c20: 028f 1c7d 0574 22a0 237c 077c 05a1 0201  ...}.t".#|.|....
-00002c30: 0057 0064 0004 0004 0083 0301 006e 1231  .W.d.........n.1
-00002c40: 0090 0273 1e30 0001 0001 0001 0059 0001  ...s.0.......Y..
-00002c50: 0064 0053 0029 184e 7201 0000 0029 01da  .d.S.).Nr....)..
-00002c60: 0474 7164 6d63 0100 0000 0000 0000 0000  .tqdmc..........
-00002c70: 0000 0300 0000 0700 0000 1300 0000 732e  ..............s.
-00002c80: 0000 0069 007c 005d 265c 027d 017d 027c  ...i.|.]&\.}.}.|
-00002c90: 0188 006a 0088 006a 0074 016a 026a 0319  ...j...j.t.j.j..
-00002ca0: 00a0 047c 02a1 0119 006a 0593 0271 0453  ...|.....j...q.S
-00002cb0: 0072 2200 0000 2906 7210 0000 0072 0400  .r"...).r....r..
-00002cc0: 0000 7231 0000 0072 2600 0000 72a6 0000  ..r1...r&...r...
-00002cd0: 0072 4900 0000 2903 722c 0000 00da 036b  .rI...).r,.....k
-00002ce0: 6579 da03 7661 6c72 b000 0000 7222 0000  ey..valr....r"..
-00002cf0: 0072 2300 0000 728b 0000 0098 0100 0073  .r#...r........s
-00002d00: 0400 0000 0602 06ff 7a2e 5370 6174 6961  ........z.Spatia
-00002d10: 6c44 6174 6173 6574 2e73 6176 655f 7370  lDataset.save_sp
-00002d20: 6c69 7473 2e3c 6c6f 6361 6c73 3e2e 3c64  lits.<locals>.<d
-00002d30: 6963 7463 6f6d 703e 726f 0000 0072 4c00  ictcomp>ro...rL.
-00002d40: 0000 7a0d 5361 7669 6e67 2073 706c 6974  ..z.Saving split
-00002d50: 7329 01da 0464 6573 632e da01 30da 0131  s)...desc...0..1
-00002d60: 4672 5200 0000 7a12 5361 7669 6e67 2069  FrR...z.Saving i
-00002d70: 6d61 6765 7320 666f 7220 7a06 2073 706c  mages for z. spl
-00002d80: 6974 2902 72b5 0000 00da 056c 6561 7665  it).r......leave
-00002d90: fa07 2f70 6174 6368 5ffa 042e 6e70 7929  ../patch_...npy)
-00002da0: 0372 0100 0000 7272 0000 0072 0200 0000  .r....rr...r....
-00002db0: a901 da04 6178 6973 2902 72a7 0000 00da  ....axis).r.....
-00002dc0: 0573 7464 6576 7a19 6e6f 726d 616c 697a  .stdevz.normaliz
-00002dd0: 6174 696f 6e5f 7061 7261 6d73 2e6a 736f  ation_params.jso
-00002de0: 6e72 4b00 0000 2924 72b2 0000 0072 a500  nrK...)$r....r..
-00002df0: 0000 725a 0000 0072 5b00 0000 720b 0000  ..rZ...r[...r...
-00002e00: 0072 0500 0000 7226 0000 0072 1000 0000  .r....r&...r....
-00002e10: da04 696c 6f63 727a 0000 00da 0661 7374  ..ilocrz.....ast
-00002e20: 7970 6572 a400 0000 7204 0000 0072 5800  yper....r....rX.
-00002e30: 0000 7231 0000 0072 3200 0000 7211 0000  ..r1...r2...r...
-00002e40: 0072 1200 0000 7253 0000 0072 0c00 0000  .r....rS...r....
-00002e50: 7268 0000 00da 086d 616b 6564 6972 73da  rh.....makedirs.
-00002e60: 0674 6f5f 6373 7672 0700 0000 7279 0000  .to_csvr....ry..
-00002e70: 0072 1500 0000 da05 7261 6e67 6572 8600  .r......ranger..
-00002e80: 0000 7246 0000 0072 8d00 0000 72a7 0000  ..rF...r....r...
-00002e90: 00da 0674 6f6c 6973 74da 0373 7464 da04  ...tolist..std..
-00002ea0: 6f70 656e da04 6a73 6f6e da04 6475 6d70  open..json..dump
-00002eb0: 2912 7220 0000 0072 9500 0000 728c 0000  ).r ...r....r...
-00002ec0: 0072 b200 0000 da0b 7370 6c69 745f 696e  .r......split_in
-00002ed0: 6465 7872 6500 0000 da07 7061 7463 6865  dexre.....patche
-00002ee0: 73da 146e 6f72 6d61 6c69 7a61 7469 6f6e  s..normalization
-00002ef0: 5f70 6172 616d 7372 7700 0000 7249 0000  _paramsrw...rI..
-00002f00: 00da 085f 7061 7463 6865 73da 075f 6c61  ..._patches.._la
-00002f10: 6265 6c73 da04 5f69 6473 da10 6d65 7461  bels.._ids..meta
-00002f20: 6461 7461 5f74 6f5f 7361 7665 da05 5f70  data_to_save.._p
-00002f30: 6174 68da 076e 5f69 6d61 6765 da01 6972  ath..n_image..ir
-00002f40: 4700 0000 7222 0000 0072 b000 0000 7223  G...r"...r....r#
-00002f50: 0000 0072 9000 0000 9301 0000 7358 0000  ...r........sX..
-00002f60: 0000 020c 030a 0206 fe06 0610 012e 0304  ................
-00002f70: 0102 0102 0102 fe0c 040a 010c 0118 0116  ................
-00002f80: 010a 0206 0102 0106 0106 fc02 ff04 0a12  ................
-00002f90: 010e 010a 0114 0114 0304 0112 ff06 0508  ................
-00002fa0: 0102 0106 010c 0102 fd0a 0622 0218 040e  ..........."....
-00002fb0: 0210 0110 fe08 0618 017a 1a53 7061 7469  .........z.Spati
-00002fc0: 616c 4461 7461 7365 742e 7361 7665 5f73  alDataset.save_s
-00002fd0: 706c 6974 7363 0200 0000 0000 0000 0000  plitsc..........
-00002fe0: 0000 0400 0000 0400 0000 0300 0000 7334  ..............s4
-00002ff0: 0000 007c 0174 006a 016a 0219 006a 0387  ...|.t.j.j...j..
-00003000: 0066 0164 0164 0284 0864 0364 048d 027d  .f.d.d...d.d...}
-00003010: 0287 0066 0164 0564 0684 087c 0244 0083  ...f.d.d...|.D..
-00003020: 017d 037c 0353 0029 077a 4e0a 2020 2020  .}.|.S.).zN.    
-00003030: 2020 2020 4c6f 6164 2061 6c6c 2069 6d61      Load all ima
-00003040: 6765 7320 7769 7468 2070 6174 6368 5f69  ges with patch_i
-00003050: 6473 2069 6e20 7468 6520 6c69 7374 2066  ds in the list f
-00003060: 726f 6d20 7468 6520 6461 7461 7365 742e  rom the dataset.
-00003070: 0a20 2020 2020 2020 2063 0100 0000 0000  .        c......
-00003080: 0000 0000 0000 0100 0000 0700 0000 1300  ................
-00003090: 0000 732a 0000 0074 006a 01a0 0288 006a  ..s*...t.j.....j
-000030a0: 037c 0088 006a 0419 009b 0064 017c 0074  .|...j.....d.|.t
-000030b0: 056a 066a 0719 009b 0064 029d 04a1 0253  .j.j.....d.....S
-000030c0: 00a9 034e 72b9 0000 0072 ba00 0000 2908  ...Nr....r....).
-000030d0: 7211 0000 0072 1200 0000 7253 0000 0072  r....r....rS...r
-000030e0: 0c00 0000 728c 0000 0072 0400 0000 7232  ....r....r....r2
-000030f0: 0000 0072 2600 0000 2901 7248 0000 0072  ...r&...).rH...r
-00003100: b000 0000 7222 0000 0072 2300 0000 da08  ....r"...r#.....
-00003110: 3c6c 616d 6264 613e de01 0000 7306 0000  <lambda>....s...
-00003120: 0006 0104 011c fe7a 3353 7061 7469 616c  .......z3Spatial
-00003130: 4461 7461 7365 742e 6c6f 6164 5f66 726f  Dataset.load_fro
-00003140: 6d5f 6d65 7461 6461 7461 2e3c 6c6f 6361  m_metadata.<loca
-00003150: 6c73 3e2e 3c6c 616d 6264 613e 7272 0000  ls>.<lambda>rr..
-00003160: 0072 bb00 0000 6301 0000 0000 0000 0000  .r....c.........
-00003170: 0000 0002 0000 0006 0000 0013 0000 0073  ...............s
-00003180: 1a00 0000 6700 7c00 5d12 7d01 8800 6a00  ....g.|.].}...j.
-00003190: 7c01 6400 6401 8d02 9102 7104 5300 2902  |.d.d.....q.S.).
-000031a0: 4629 01da 0269 6429 01da 116c 6f61 645f  F)...id)...load_
-000031b0: 7369 6e67 6c65 5f69 6d61 6765 2902 722c  single_image).r,
-000031c0: 0000 0072 1200 0000 72b0 0000 0072 2200  ...r....r....r".
-000031d0: 0000 7223 0000 0072 2f00 0000 e401 0000  ..r#...r/.......
-000031e0: 7230 0000 007a 3553 7061 7469 616c 4461  r0...z5SpatialDa
-000031f0: 7461 7365 742e 6c6f 6164 5f66 726f 6d5f  taset.load_from_
-00003200: 6d65 7461 6461 7461 2e3c 6c6f 6361 6c73  metadata.<locals
-00003210: 3e2e 3c6c 6973 7463 6f6d 703e 2904 7204  >.<listcomp>).r.
-00003220: 0000 0072 5800 0000 7226 0000 00da 0561  ...rX...r&.....a
-00003230: 7070 6c79 2904 7220 0000 0072 1000 0000  pply).r ...r....
-00003240: da0b 696d 6167 655f 7061 7468 7372 4c00  ..image_pathsrL.
-00003250: 0000 7222 0000 0072 b000 0000 7223 0000  ..r"...r....r#..
-00003260: 00da 126c 6f61 645f 6672 6f6d 5f6d 6574  ...load_from_met
-00003270: 6164 6174 61d8 0100 0073 0c00 0000 0005  adata....s......
-00003280: 0c01 0a04 02fb 0607 1201 7a21 5370 6174  ..........z!Spat
-00003290: 6961 6c44 6174 6173 6574 2e6c 6f61 645f  ialDataset.load_
-000032a0: 6672 6f6d 5f6d 6574 6164 6174 6163 0200  from_metadatac..
-000032b0: 0000 0000 0000 0000 0000 0300 0000 0700  ................
-000032c0: 0000 4300 0000 7340 0000 0074 00a0 017c  ..C...s@...t...|
-000032d0: 00a1 017d 027c 0172 387c 0274 0274 036a  ...}.|.r8|.t.t.j
-000032e0: 04a0 0574 036a 04a0 067c 00a1 01a1 0164  ...t.j...|.....d
-000032f0: 0119 00a0 0764 02a1 0164 0319 0083 0166  .....d...d.....f
-00003300: 0253 007c 0253 0064 0453 0029 057a e40a  .S.|.S.d.S.).z..
-00003310: 2020 2020 2020 2020 4c6f 6164 2061 2073          Load a s
-00003320: 696e 676c 6520 696d 6167 6520 6672 6f6d  ingle image from
-00003330: 2074 6865 2064 6174 6173 6574 2e0a 0a20   the dataset... 
-00003340: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00003350: 2020 2020 2020 2020 2070 6174 6820 2873           path (s
-00003360: 7472 293a 2050 6174 6820 746f 2074 6865  tr): Path to the
-00003370: 2069 6d61 6765 2066 696c 652e 0a20 2020   image file..   
-00003380: 2020 2020 2020 2020 2069 6420 2862 6f6f           id (boo
-00003390: 6c29 3a20 5768 6574 6865 7220 746f 2072  l): Whether to r
-000033a0: 6574 7572 6e20 7468 6520 696d 6167 6520  eturn the image 
-000033b0: 4944 2e0a 0a20 2020 2020 2020 2052 6574  ID...        Ret
-000033c0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-000033d0: 2020 6e70 2e6e 6461 7272 6179 3a20 496d    np.ndarray: Im
-000033e0: 6167 6520 6172 7261 792e 0a20 2020 2020  age array..     
-000033f0: 2020 2072 0100 0000 da01 5fe9 ffff ffff     r......_.....
-00003400: 4e29 0872 8600 0000 da04 6c6f 6164 72a4  N).r......loadr.
-00003410: 0000 0072 1100 0000 7212 0000 00da 0873  ...r....r......s
-00003420: 706c 6974 6578 74da 0862 6173 656e 616d  plitext..basenam
-00003430: 6572 2a00 0000 2903 7212 0000 0072 d400  er*...).r....r..
-00003440: 0000 da05 696d 6167 6572 2200 0000 7222  ....imager"...r"
-00003450: 0000 0072 2300 0000 72d5 0000 00e7 0100  ...r#...r.......
-00003460: 0073 0c00 0000 000c 0a01 0401 0401 20ff  .s............ .
-00003470: 0604 7a20 5370 6174 6961 6c44 6174 6173  ..z SpatialDatas
-00003480: 6574 2e6c 6f61 645f 7369 6e67 6c65 5f69  et.load_single_i
-00003490: 6d61 6765 6304 0000 0000 0000 0000 0000  magec...........
-000034a0: 0004 0000 0008 0000 0043 0000 0073 2600  .........C...s&.
-000034b0: 0000 7400 7c02 8301 7d02 7401 6a02 a003  ..t.|...}.t.j...
-000034c0: 7c00 6a04 7c03 7c02 9b00 6401 7c01 9b00  |.j.|.|...d.|...
-000034d0: 6402 9d04 a103 5300 72d2 0000 0029 0572  d.....S.r....).r
-000034e0: a400 0000 7211 0000 0072 1200 0000 7253  ....r....r....rS
-000034f0: 0000 0072 0c00 0000 2904 7220 0000 0072  ...r....).r ...r
-00003500: 5800 0000 7279 0000 0072 2a00 0000 7222  X...ry...r*...r"
-00003510: 0000 0072 2200 0000 7223 0000 00da 1367  ...r"...r#.....g
-00003520: 656e 6572 6174 655f 7061 7463 685f 7061  enerate_patch_pa
-00003530: 7468 fb01 0000 7304 0000 0000 0108 017a  th....s........z
-00003540: 2253 7061 7469 616c 4461 7461 7365 742e  "SpatialDataset.
-00003550: 6765 6e65 7261 7465 5f70 6174 6368 5f70  generate_patch_p
-00003560: 6174 6829 044e 4e4e 4e29 014e 2901 4e29  ath).NNNN).N).N)
-00003570: 014e 2901 4e29 0972 7c00 0000 727d 0000  .N).N).r|...r}..
-00003580: 0072 7d00 0000 4e4e 544e 4e54 2902 7282  .r}...NNTNNT).r.
-00003590: 0000 0072 9700 0000 2905 72a0 0000 0054  ...r....).r....T
-000035a0: 724e 0000 0072 8200 0000 7297 0000 0029  rN...r....r....)
-000035b0: 0154 2922 da08 5f5f 6e61 6d65 5f5f da0a  .T)"..__name__..
-000035c0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000035d0: 616c 6e61 6d65 5f5f da03 7374 72da 046c  alname__..str..l
-000035e0: 6973 7472 2400 0000 721f 0000 0072 3b00  istr$...r....r;.
-000035f0: 0000 7273 0000 0072 1800 0000 7217 0000  ..rs...r....r...
-00003600: 0072 a400 0000 da04 626f 6f6c 7267 0000  .r......boolrg..
-00003610: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00003620: 721c 0000 0072 1e00 0000 721d 0000 0072  r....r....r....r
-00003630: 2800 0000 da05 666c 6f61 7472 9600 0000  (.....floatr....
-00003640: da0c 7374 6174 6963 6d65 7468 6f64 729f  ..staticmethodr.
-00003650: 0000 0072 8f00 0000 72b1 0000 0072 0400  ...r....r....r..
-00003660: 0000 da0c 636f 6e74 6169 6e73 5f63 6438  ....contains_cd8
-00003670: 7226 0000 0072 9000 0000 72d8 0000 0072  r&...r....r....r
-00003680: d500 0000 72df 0000 0072 2200 0000 7222  ....r....r"...r"
-00003690: 0000 0072 2200 0000 7223 0000 0072 0800  ...r"...r#...r..
-000036a0: 0000 1200 0000 7382 0000 0008 0500 0100  ......s.........
-000036b0: 0100 0100 f902 0202 0102 0102 0102 0102  ................
-000036c0: 0102 f90c 2208 0612 1508 0902 0102 0102  ...."...........
-000036d0: 0102 0102 0102 f902 0202 0102 0102 0102  ................
-000036e0: 0102 0102 f90c 5a10 0810 0810 0810 0808  ......Z.........
-000036f0: 1208 100e 0c00 0100 0100 0100 0100 0100  ................
-00003700: 0100 0100 0100 f502 0202 0102 0102 0102  ................
-00003710: fb0c 5402 010c 1000 0100 0100 0100 0100  ..T.............
-00003720: f60a 3508 0310 4508 0f02 010c 1372 0800  ..5...E......r..
-00003730: 0000 2910 72c6 0000 0072 1100 0000 7237  ..).r....r....r7
-00003740: 0000 0072 5a00 0000 da05 6e75 6d70 7972  ...rZ.....numpyr
-00003750: 8600 0000 da06 7061 6e64 6173 723b 0000  ......pandasr;..
-00003760: 005a 0e75 7469 6c73 2e70 6174 6368 6966  .Z.utils.patchif
-00003770: 7972 0300 0000 da13 636f 6e66 6967 7572  yr......configur
-00003780: 6174 696f 6e2e 5479 7065 7372 0400 0000  ation.Typesr....
-00003790: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
-000037a0: 0800 0000 7222 0000 0072 2200 0000 7222  ....r"...r"...r"
-000037b0: 0000 0072 2300 0000 da08 3c6d 6f64 756c  ...r#.....<modul
-000037c0: 653e 0100 0000 7310 0000 0008 0108 0108  e>....s.........
-000037d0: 0208 0108 0108 020c 0118 08              ...........
+00000110: 3a01 0000 6500 5a01 6400 5a02 6700 6401  :...e.Z.d.Z.g.d.
+00000120: 6401 6401 6401 6605 6503 6504 6503 6503  d.d.d.f.e.e.e.e.
+00000130: 6503 6503 6402 9c06 6403 6404 8405 5a05  e.e.d...d.d...Z.
+00000140: 6405 6406 8400 5a06 6507 6a08 6504 6407  d.d...Z.e.j.e.d.
+00000150: 9c02 6408 6409 8404 5a09 640a 640b 8400  ..d.d...Z.d.d...
+00000160: 5a0a 6700 640c 640d 6401 640e 6401 6606  Z.g.d.d.d.d.d.f.
+00000170: 6504 650b 650b 6504 650c 6503 640f 9c06  e.e.e.e.e.e.d...
+00000180: 6410 6411 8405 5a0d 643c 6503 6412 9c01  d.d...Z.d<e.d...
+00000190: 6413 6414 8405 5a0e 643d 6503 6415 9c01  d.d...Z.d=e.d...
+000001a0: 6416 6417 8405 5a0f 643e 6503 6418 9c01  d.d...Z.d>e.d...
+000001b0: 6419 641a 8405 5a10 643f 6503 641b 9c01  d.d...Z.d?e.d...
+000001c0: 641c 641d 8405 5a11 641e 641f 8400 5a12  d.d...Z.d.d...Z.
+000001d0: 6420 6421 8400 5a13 6503 6422 9c01 6423  d d!..Z.e.d"..d#
+000001e0: 6424 8404 5a14 6440 6503 6515 6515 6515  d$..Z.d@e.e.e.e.
+000001f0: 6427 9c04 6428 6429 8405 5a16 6517 6441  d'..d(d)..Z.e.dA
+00000200: 642c 642d 8401 8301 5a18 6442 6430 6431  d,d-....Z.dBd0d1
+00000210: 8401 5a19 6432 6433 8400 5a1a 651b 6a1c  ..Z.d2d3..Z.e.j.
+00000220: 6a1d 6601 6434 6435 8401 5a1e 6436 6437  j.f.d4d5..Z.d6d7
+00000230: 8400 5a1f 6517 6443 6438 6439 8401 8301  ..Z.e.dCd8d9....
+00000240: 5a20 643a 643b 8400 5a21 6401 5300 2944  Z d:d;..Z!d.S.)D
+00000250: da0e 5370 6174 6961 6c44 6174 6173 6574  ..SpatialDataset
+00000260: 4e29 06da 0a69 6e70 7574 5f70 6174 68da  N)...input_path.
+00000270: 0d63 6861 6e6e 656c 5f6e 616d 6573 da0a  .channel_names..
+00000280: 7061 7463 685f 7061 7468 da09 7370 6c69  patch_path..spli
+00000290: 745f 6469 72da 096d 6f64 656c 5f64 6972  t_dir..model_dir
+000002a0: da06 6366 5f64 6972 6307 0000 0000 0000  ..cf_dirc.......
+000002b0: 0000 0000 0008 0000 0004 0000 0043 0000  .............C..
+000002c0: 0073 9e00 0000 6400 7c00 5f00 6400 7c00  .s....d.|._.d.|.
+000002d0: 5f01 7c01 7c00 5f02 7403 6a04 a005 7c01  _.|.|._.t.j...|.
+000002e0: a101 7c00 5f06 7c00 a007 a100 7d07 7c00  ..|._.|.....}.|.
+000002f0: a008 7c07 7c02 a102 0100 7c00 a009 7c03  ..|.|.....|...|.
+00000300: a101 7c00 5f0a 7c00 a00b 7c04 a101 7c00  ..|._.|...|...|.
+00000310: 5f0c 7c00 a00d 7c05 a101 7c00 5f0e 7c00  _.|...|...|._.|.
+00000320: a00f 7c06 a101 7c00 5f10 7c00 6a0a 6400  ..|...|._.|.j.d.
+00000330: 7501 727e 7c00 a011 a100 0100 7c00 a012  u.r~|.......|...
+00000340: a100 0100 7c00 6a0c 6400 7501 729a 7c00  ....|.j.d.u.r.|.
+00000350: 6a0a 6400 7501 729a 7c00 a013 a100 0100  j.d.u.r.|.......
+00000360: 6400 5300 a901 4e29 145a 0864 6174 615f  d.S...N).Z.data_
+00000370: 6469 6dda 086d 6574 6164 6174 6172 0900  dim..metadatar..
+00000380: 0000 da02 6f73 da04 7061 7468 da07 6469  ....os..path..di
+00000390: 726e 616d 65da 0872 6f6f 745f 6469 72da  rname..root_dir.
+000003a0: 0e6c 6f61 645f 696e 7075 745f 6373 76da  .load_input_csv.
+000003b0: 0f63 6865 636b 5f69 6e70 7574 5f63 7376  .check_input_csv
+000003c0: da0e 7365 745f 7061 7463 685f 7061 7468  ..set_patch_path
+000003d0: 720b 0000 00da 0d73 6574 5f73 706c 6974  r......set_split
+000003e0: 5f64 6972 720c 0000 00da 0d73 6574 5f6d  _dirr......set_m
+000003f0: 6f64 656c 5f64 6972 720d 0000 00da 1673  odel_dirr......s
+00000400: 6574 5f63 6f75 6e74 6572 6661 6374 7561  et_counterfactua
+00000410: 6c5f 6469 7272 0e00 0000 da0f 6c6f 6164  l_dirr......load
+00000420: 5f70 6174 6368 5f64 6174 61da 1263 6865  _patch_data..che
+00000430: 636b 5f6c 6f61 6465 645f 7061 7463 68da  ck_loaded_patch.
+00000440: 0e67 6574 5f73 706c 6974 5f69 6e66 6f29  .get_split_info)
+00000450: 08da 0473 656c 6672 0900 0000 720a 0000  ...selfr....r...
+00000460: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000470: 720e 0000 00da 0464 6174 61a9 0072 2000  r......data..r .
+00000480: 0000 fa57 2f63 656e 7472 616c 2f68 6f6d  ...W/central/hom
+00000490: 652f 7a77 616e 6732 2f6d 6f72 7068 6575  e/zwang2/morpheu
+000004a0: 732d 7370 6174 6961 6c2f 6d6f 7270 6865  s-spatial/morphe
+000004b0: 7573 2f73 7263 2f6d 6f72 7068 6575 732f  us/src/morpheus/
+000004c0: 6461 7461 7365 7473 2f73 7061 7469 616c  datasets/spatial
+000004d0: 5f64 6174 6173 6574 2e70 79da 085f 5f69  _dataset.py..__i
+000004e0: 6e69 745f 5f13 0000 0073 1e00 0000 0009  nit__....s......
+000004f0: 0601 0601 0601 0e02 0801 0c03 0c01 0c01  ................
+00000500: 0c01 0c02 0a01 0801 0803 1401 7a17 5370  ............z.Sp
+00000510: 6174 6961 6c44 6174 6173 6574 2e5f 5f69  atialDataset.__i
+00000520: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00000530: 0000 0200 0000 0600 0000 4300 0000 732c  ..........C...s,
+00000540: 0000 0074 0044 005d 227d 017c 016a 017c  ...t.D.]"}.|.j.|
+00000550: 006a 026a 037c 00a0 047c 016a 01a1 0174  .j.j.|...|.j...t
+00000560: 056a 066a 0166 023c 0071 0464 0053 0072  .j.j.f.<.q.d.S.r
+00000570: 0f00 0000 2907 7205 0000 00da 0576 616c  ....).r......val
+00000580: 7565 7210 0000 00da 036c 6f63 da0d 6765  uer......loc..ge
+00000590: 745f 7370 6c69 745f 6964 7372 0400 0000  t_split_idsr....
+000005a0: da06 7370 6c69 7473 2902 721e 0000 00da  ..splits).r.....
+000005b0: 0573 706c 6974 7220 0000 0072 2000 0000  .splitr ...r ...
+000005c0: 7221 0000 0072 1d00 0000 3200 0000 7306  r!...r....2...s.
+000005d0: 0000 0000 0108 0204 ff7a 1d53 7061 7469  .........z.Spati
+000005e0: 616c 4461 7461 7365 742e 6765 745f 7370  alDataset.get_sp
+000005f0: 6c69 745f 696e 666f 2902 da09 696e 7075  lit_info)...inpu
+00000600: 745f 6373 7672 0a00 0000 6303 0000 0000  t_csvr....c.....
+00000610: 0000 0000 0000 0004 0000 0005 0000 0003  ................
+00000620: 0000 0073 9e00 0000 7400 6a01 6a02 7400  ...s....t.j.j.t.
+00000630: 6a03 6a02 7400 6a04 6a02 7400 6a05 6a02  j.j.t.j.j.t.j.j.
+00000640: 7400 6a06 6a02 6705 8901 7407 8800 8301  t.j.j.g...t.....
+00000650: 6401 6b02 7250 8701 6601 6402 6403 8408  d.k.rP..f.d.d...
+00000660: 7c01 6a08 4400 8301 8900 7409 6404 8800  |.j.D.....t.d...
+00000670: 9b00 9d02 8301 0100 8801 8800 3700 8901  ............7...
+00000680: 8801 4400 5d18 7d03 7c03 7c01 6a08 7601  ..D.].}.|.|.j.v.
+00000690: 725c 740a a00b 6405 a101 0100 715c 8700  r\t...d.....q\..
+000006a0: 6601 6406 6403 8408 7c01 6a08 4400 8301  f.d.d...|.j.D...
+000006b0: 7c00 5f0c 7c01 6a0d 729a 740e 6407 8301  |._.|.j.r.t.d...
+000006c0: 8201 6400 5300 2908 4e72 0100 0000 6301  ..d.S.).Nr....c.
+000006d0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+000006e0: 0000 0013 0000 0073 1800 0000 6700 7c00  .......s....g.|.
+000006f0: 5d10 7d01 7c01 8800 7601 7204 7c01 9102  ].}.|...v.r.|...
+00000700: 7104 5300 7220 0000 0072 2000 0000 a902  q.S.r ...r .....
+00000710: da02 2e30 da03 636f 6c29 01da 0d72 6571  ...0..col)...req
+00000720: 7569 7265 645f 636f 6c73 7220 0000 0072  uired_colsr ...r
+00000730: 2100 0000 da0a 3c6c 6973 7463 6f6d 703e  !.....<listcomp>
+00000740: 4200 0000 7302 0000 0006 017a 3253 7061  B...s......z2Spa
+00000750: 7469 616c 4461 7461 7365 742e 6368 6563  tialDataset.chec
+00000760: 6b5f 696e 7075 745f 6373 762e 3c6c 6f63  k_input_csv.<loc
+00000770: 616c 733e 2e3c 6c69 7374 636f 6d70 3e7a  als>.<listcomp>z
+00000780: 2743 6861 6e6e 656c 206e 616d 6573 2069  'Channel names i
+00000790: 6e66 6572 7265 6420 6672 6f6d 2069 6e70  nferred from inp
+000007a0: 7574 2043 5356 3a20 7a31 696e 7075 7420  ut CSV: z1input 
+000007b0: 6373 7620 646f 6573 206e 6f74 2063 6f6e  csv does not con
+000007c0: 7461 696e 2072 6571 7569 7265 6420 636f  tain required co
+000007d0: 6c75 6d6e 3a20 7b63 6f6c 7d63 0100 0000  lumn: {col}c....
+000007e0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000007f0: 1300 0000 7318 0000 0067 007c 005d 107d  ....s....g.|.].}
+00000800: 017c 0188 0076 0072 047c 0191 0271 0453  .|...v.r.|...q.S
+00000810: 0072 2000 0000 7220 0000 0072 2900 0000  .r ...r ...r)...
+00000820: 2901 720a 0000 0072 2000 0000 7221 0000  ).r....r ...r!..
+00000830: 0072 2d00 0000 4d00 0000 f300 0000 007a  .r-...M........z
+00000840: 1249 6e70 7574 2043 5356 2069 7320 656d  .Input CSV is em
+00000850: 7074 7929 0f72 0400 0000 da0a 7061 7469  pty).r......pati
+00000860: 656e 745f 6964 7223 0000 00da 0869 6d61  ent_idr#.....ima
+00000870: 6765 5f69 64da 0963 656c 6c5f 7479 7065  ge_id..cell_type
+00000880: 5a06 6365 6c6c 5f78 5a06 6365 6c6c 5f79  Z.cell_xZ.cell_y
+00000890: da03 6c65 6eda 0763 6f6c 756d 6e73 da05  ..len..columns..
+000008a0: 7072 696e 74da 0877 6172 6e69 6e67 73da  print..warnings.
+000008b0: 0477 6172 6e72 0a00 0000 da05 656d 7074  .warnr......empt
+000008c0: 79da 0a56 616c 7565 4572 726f 7229 0472  y..ValueError).r
+000008d0: 1e00 0000 7228 0000 0072 0a00 0000 722b  ....r(...r....r+
+000008e0: 0000 0072 2000 0000 2902 720a 0000 0072  ...r ...).r....r
+000008f0: 2c00 0000 7221 0000 0072 1600 0000 3800  ,...r!...r....8.
+00000900: 0000 7326 0000 0000 0306 0106 0106 0106  ..s&............
+00000910: 0106 fb04 070c 010a 0104 ff06 030e 0108  ................
+00000920: 0208 010a 010c 0316 0306 0108 017a 1e53  .............z.S
+00000930: 7061 7469 616c 4461 7461 7365 742e 6368  patialDataset.ch
+00000940: 6563 6b5f 696e 7075 745f 6373 7663 0100  eck_input_csvc..
+00000950: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00000960: 0000 4300 0000 7310 0000 0074 00a0 017c  ..C...s....t...|
+00000970: 006a 02a1 017d 017c 0153 0072 0f00 0000  .j...}.|.S.r....
+00000980: 2903 da02 7064 da08 7265 6164 5f63 7376  )...pd..read_csv
+00000990: 7209 0000 0029 0272 1e00 0000 721f 0000  r....).r....r...
+000009a0: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
+000009b0: 7215 0000 0054 0000 0073 0400 0000 0001  r....T...s......
+000009c0: 0c01 7a1d 5370 6174 6961 6c44 6174 6173  ..z.SpatialDatas
+000009d0: 6574 2e6c 6f61 645f 696e 7075 745f 6373  et.load_input_cs
+000009e0: 76e9 1000 0000 e903 0000 0054 2906 da0c  v..........T)...
+000009f0: 6365 6c6c 5f74 6f5f 6d61 736b da0a 7061  cell_to_mask..pa
+00000a00: 7463 685f 7369 7a65 da0a 7069 7865 6c5f  tch_size..pixel_
+00000a10: 7369 7a65 da0a 6365 6c6c 5f74 7970 6573  size..cell_types
+00000a20: da04 7361 7665 da09 7361 7665 5f70 6174  ..save..save_pat
+00000a30: 6863 0700 0000 0000 0000 0000 0000 1000  hc..............
+00000a40: 0000 0900 0000 4300 0000 73dc 0100 007c  ......C...s....|
+00000a50: 0572 5a7c 0664 0175 0172 107c 066e 1274  .rZ|.d.u.r.|.n.t
+00000a60: 006a 01a0 027c 006a 0374 046a 056a 06a1  .j...|.j.t.j.j..
+00000a70: 027c 005f 0774 006a 01a0 087c 006a 07a1  .|._.t.j...|.j..
+00000a80: 0172 5a74 0964 027c 006a 079b 0064 039d  .rZt.d.|.j...d..
+00000a90: 0383 0101 007c 00a0 0aa1 0001 007c 00a0  .....|.......|..
+00000aa0: 0ba1 0001 0064 0153 0074 0964 047c 029b  .....d.S.t.d.|..
+00000ab0: 0064 057c 029b 0064 069d 0583 0101 0074  .d.|...d.......t
+00000ac0: 0964 077c 039b 0064 057c 039b 0064 089d  .d.|...d.|...d..
+00000ad0: 0583 0101 0074 0964 097c 049b 009d 0283  .....t.d.|......
+00000ae0: 0101 0074 0964 0a7c 019b 009d 0283 0101  ...t.d.|........
+00000af0: 007c 00a0 0ca1 007d 0774 0d7c 077c 027c  .|.....}.t.|.|.|
+00000b00: 037c 047c 006a 0e7c 0183 065c 027d 087d  .|.|.j.|...\.}.}
+00000b10: 097c 09a0 0fa1 006a 1064 0b74 116a 126a  .|.....j.d.t.j.j
+00000b20: 0669 0164 0c8d 017d 097c 086a 135c 047d  .i.d...}.|.j.\.}
+00000b30: 0a7d 0b7d 0c7d 0d7c 0d74 147c 006a 0e83  .}.}.}.|.t.|.j..
+00000b40: 016b 0372 fe74 1564 0d83 0182 017c 0b7c  .k.r.t.d.....|.|
+00000b50: 026b 0390 0173 127c 0c7c 026b 0390 0172  .k...s.|.|.k...r
+00000b60: 1a74 1564 0e83 0182 017c 0a74 147c 0983  .t.d.....|.t.|..
+00000b70: 016b 0390 0172 3074 1564 0f83 0182 017c  .k...r0t.d.....|
+00000b80: 0590 0172 d874 16a0 177c 006a 0764 10a1  ...r.t...|.j.d..
+00000b90: 028f 627d 0e7c 0e6a 1864 117c 0864 1274  ..b}.|.j.d.|.d.t
+00000ba0: 197c 0a64 1383 027c 0b7c 0c7c 0d66 047c  .|.d...|.|.|.f.|
+00000bb0: 086a 1a64 148d 0501 007c 096a 1b64 1564  .j.d.....|.j.d.d
+00000bc0: 168d 017d 0f7c 0e6a 1864 177c 0f7c 0f6a  ...}.|.j.d.|.|.j
+00000bd0: 1a64 188d 0301 007c 0e6a 1864 197c 006a  .d.....|.j.d.|.j
+00000be0: 0e64 1a8d 0201 0057 0064 0104 0004 0083  .d.....W.d......
+00000bf0: 0301 006e 1231 0090 0173 ae30 0001 0001  ...n.1...s.0....
+00000c00: 0001 0059 0001 0074 0964 1b7c 006a 079b  ...Y...t.d.|.j..
+00000c10: 009d 0283 0101 007c 00a0 0aa1 0001 007c  .......|.......|
+00000c20: 00a0 0ba1 0001 0064 0153 0029 1c61 ca01  .......d.S.).a..
+00000c30: 0000 0a20 2020 2020 2020 2047 656e 6572  ...        Gener
+00000c40: 6174 6520 6d61 736b 6564 2070 6174 6368  ate masked patch
+00000c50: 6573 2066 726f 6d20 7468 6520 696e 7075  es from the inpu
+00000c60: 7420 6461 7461 2e0a 0a20 2020 2020 2020  t data...       
+00000c70: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00000c80: 2020 2063 656c 6c5f 746f 5f6d 6173 6b20     cell_to_mask 
+00000c90: 2873 7472 293a 2054 6865 2063 656c 6c20  (str): The cell 
+00000ca0: 7479 7065 2074 6f20 6d61 736b 2e0a 2020  type to mask..  
+00000cb0: 2020 2020 2020 2020 2020 7061 7463 685f            patch_
+00000cc0: 7369 7a65 2028 696e 7429 3a20 5468 6520  size (int): The 
+00000cd0: 7369 7a65 206f 6620 7468 6520 7061 7463  size of the patc
+00000ce0: 6820 696e 2070 6978 656c 732e 0a20 2020  h in pixels..   
+00000cf0: 2020 2020 2020 2020 2070 6978 656c 5f73           pixel_s
+00000d00: 697a 6520 2869 6e74 293a 2054 6865 2070  ize (int): The p
+00000d10: 6978 656c 2073 697a 6520 696e 206d 6963  ixel size in mic
+00000d20: 726f 6e73 2e0a 2020 2020 2020 2020 2020  rons..          
+00000d30: 2020 6365 6c6c 5f74 7970 6573 2028 6c69    cell_types (li
+00000d40: 7374 293a 2054 6865 2063 656c 6c20 7479  st): The cell ty
+00000d50: 7065 7320 746f 2069 6e63 6c75 6465 2069  pes to include i
+00000d60: 6e20 7468 6520 6d65 7461 6461 7461 2e0a  n the metadata..
+00000d70: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00000d80: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
+00000d90: 2074 6f20 7361 7665 2074 6865 2070 6174   to save the pat
+00000da0: 6368 6573 2e0a 2020 2020 2020 2020 2020  ches..          
+00000db0: 2020 7361 7665 5f70 6174 6820 2873 7472    save_path (str
+00000dc0: 293a 2054 6865 2070 6174 6820 746f 2073  ): The path to s
+00000dd0: 6176 6520 7468 6520 7061 7463 6865 732e  ave the patches.
+00000de0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00000df0: 733a 0a0a 2020 2020 2020 2020 4e7a 0546  s:..        Nz.F
+00000e00: 696c 6520 7a23 2061 6c72 6561 6479 2065  ile z# already e
+00000e10: 7869 7374 732c 206e 6f74 2073 6176 696e  xists, not savin
+00000e20: 6720 7061 7463 6865 737a 1b47 656e 6572  g patchesz.Gener
+00000e30: 6174 696e 6720 7061 7463 6865 7320 6f66  ating patches of
+00000e40: 2073 697a 6520 da01 787a 0720 7069 7865   size ..xz. pixe
+00000e50: 6c73 7a0c 5069 7865 6c20 7369 7a65 3a20  lsz.Pixel size: 
+00000e60: 7a08 206d 6963 726f 6e73 7a15 4365 6c6c  z. micronsz.Cell
+00000e70: 2074 7970 6573 2072 6563 6f72 6465 643a   types recorded:
+00000e80: 207a 1343 656c 6c20 7479 7065 7320 6d61   z.Cell types ma
+00000e90: 736b 6564 3a20 da05 696e 6465 7829 0172  sked: ..index).r
+00000ea0: 3300 0000 fa34 4e75 6d62 6572 206f 6620  3....4Number of 
+00000eb0: 6368 616e 6e65 6c20 6e61 6d65 7320 646f  channel names do
+00000ec0: 206e 6f74 206d 6174 6368 2064 6174 6120   not match data 
+00000ed0: 6469 6d65 6e73 696f 6e73 7a35 5061 7463  dimensionsz5Patc
+00000ee0: 6820 6469 6d65 6e73 696f 6e73 2064 6f20  h dimensions do 
+00000ef0: 6e6f 7420 6d61 7463 6820 7468 6520 6578  not match the ex
+00000f00: 7065 6374 6564 2064 696d 656e 7369 6f6e  pected dimension
+00000f10: 737a 334e 756d 6265 7220 6f66 2070 6174  sz3Number of pat
+00000f20: 6368 6573 2067 656e 6572 6174 6564 2064  ches generated d
+00000f30: 6f65 7320 6e6f 7420 6d61 7463 6820 6d65  oes not match me
+00000f40: 7461 6461 7461 da01 77da 0669 6d61 6765  tadata..w..image
+00000f50: 73da 0467 7a69 70e9 6400 0000 2904 721f  s..gzip.d...).r.
+00000f60: 0000 00da 0b63 6f6d 7072 6573 7369 6f6e  .....compression
+00000f70: da06 6368 756e 6b73 da05 6474 7970 6546  ..chunks..dtypeF
+00000f80: a901 7244 0000 0072 1000 0000 2902 721f  ..rD...r....).r.
+00000f90: 0000 0072 4c00 0000 720a 0000 0029 0172  ...rL...r....).r
+00000fa0: 1f00 0000 7a11 5061 7463 6865 7320 7361  ....z.Patches sa
+00000fb0: 7665 6420 746f 2029 1c72 1100 0000 7212  ved to ).r....r.
+00000fc0: 0000 00da 046a 6f69 6e72 1400 0000 7207  .....joinr....r.
+00000fd0: 0000 00da 0570 6174 6368 7223 0000 0072  .....patchr#...r
+00000fe0: 0b00 0000 da06 6973 6669 6c65 7234 0000  ......isfiler4..
+00000ff0: 0072 1b00 0000 721c 0000 0072 1500 0000  .r....r....r....
+00001000: 7203 0000 0072 0a00 0000 5a0b 7265 7365  r....r....Z.rese
+00001010: 745f 696e 6465 78da 0672 656e 616d 6572  t_index..renamer
+00001020: 0400 0000 da08 7061 7463 685f 6964 da05  ......patch_id..
+00001030: 7368 6170 6572 3200 0000 7238 0000 00da  shaper2...r8....
+00001040: 0468 3570 79da 0446 696c 655a 0e63 7265  .h5py..FileZ.cre
+00001050: 6174 655f 6461 7461 7365 74da 036d 696e  ate_dataset..min
+00001060: 724c 0000 005a 0a74 6f5f 7265 636f 7264  rL...Z.to_record
+00001070: 7329 1072 1e00 0000 723d 0000 0072 3e00  s).r....r=...r>.
+00001080: 0000 723f 0000 0072 4000 0000 7241 0000  ..r?...r@...rA..
+00001090: 0072 4200 0000 da02 6466 5a0d 7061 7463  .rB.....dfZ.patc
+000010a0: 6865 735f 6172 7261 795a 0b6d 6574 6164  hes_arrayZ.metad
+000010b0: 6174 615f 6466 da01 6eda 0168 7246 0000  ata_df..n..hrF..
+000010c0: 00da 0163 da01 665a 0e6d 6574 6164 6174  ...c..fZ.metadat
+000010d0: 615f 6e75 6d70 7972 2000 0000 7220 0000  a_numpyr ...r ..
+000010e0: 0072 2100 0000 da15 6765 6e65 7261 7465  .r!.....generate
+000010f0: 5f6d 6173 6b65 645f 7061 7463 6858 0000  _masked_patchX..
+00001100: 0073 5c00 0000 0018 0403 06ff 0602 12fd  .s\.............
+00001110: 0405 0e01 1201 0801 0801 0403 1601 1601  ................
+00001120: 0e01 0e03 0803 0201 0eff 0803 0801 0aff  ................
+00001130: 0603 0e03 0e01 0803 1401 0803 0e01 0802  ................
+00001140: 0601 1002 0401 0201 0201 0201 1001 04fb  ................
+00001150: 0609 0c01 0401 08ff 0605 3001 1001 0801  ..........0.....
+00001160: 0801 7a24 5370 6174 6961 6c44 6174 6173  ..z$SpatialDatas
+00001170: 6574 2e67 656e 6572 6174 655f 6d61 736b  et.generate_mask
+00001180: 6564 5f70 6174 6368 2901 720b 0000 0063  ed_patch).r....c
+00001190: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+000011a0: 0400 0000 4300 0000 7334 0000 007c 0164  ....C...s4...|.d
+000011b0: 0075 0172 0c7c 016e 1274 006a 01a0 027c  .u.r.|.n.t.j...|
+000011c0: 006a 0374 046a 056a 06a1 027d 0274 006a  .j.t.j.j...}.t.j
+000011d0: 01a0 077c 02a1 0172 307c 0253 0064 0053  ...|...r0|.S.d.S
+000011e0: 0072 0f00 0000 2908 7211 0000 0072 1200  .r....).r....r..
+000011f0: 0000 724e 0000 0072 1400 0000 7207 0000  ..rN...r....r...
+00001200: 0072 4f00 0000 7223 0000 0072 5000 0000  .rO...r#...rP...
+00001210: 2903 721e 0000 0072 0b00 0000 7212 0000  ).r....r....r...
+00001220: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
+00001230: 7217 0000 00b2 0000 0073 0a00 0000 0003  r........s......
+00001240: 06ff 0602 12fd 0205 7a1d 5370 6174 6961  ........z.Spatia
+00001250: 6c44 6174 6173 6574 2e73 6574 5f70 6174  lDataset.set_pat
+00001260: 6368 5f70 6174 6829 0172 0c00 0000 6302  ch_path).r....c.
+00001270: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00001280: 0000 0043 0000 0073 3400 0000 7c01 6400  ...C...s4...|.d.
+00001290: 7501 720c 7c01 6e12 7400 6a01 a002 7c00  u.r.|.n.t.j...|.
+000012a0: 6a03 7404 6a05 6a06 a102 7d02 7400 6a01  j.t.j.j...}.t.j.
+000012b0: a007 7c02 a101 7230 7c02 5300 6400 5300  ..|...r0|.S.d.S.
+000012c0: 720f 0000 0029 0872 1100 0000 7212 0000  r....).r....r...
+000012d0: 0072 4e00 0000 7214 0000 0072 0600 0000  .rN...r....r....
+000012e0: 7227 0000 0072 2300 0000 da05 6973 6469  r'...r#.....isdi
+000012f0: 7229 0372 1e00 0000 720c 0000 00da 0364  r).r....r......d
+00001300: 6972 7220 0000 0072 2000 0000 7221 0000  irr ...r ...r!..
+00001310: 0072 1800 0000 ba00 0000 730a 0000 0000  .r........s.....
+00001320: 0306 ff06 0212 fd02 057a 1c53 7061 7469  .........z.Spati
+00001330: 616c 4461 7461 7365 742e 7365 745f 7370  alDataset.set_sp
+00001340: 6c69 745f 6469 7229 0172 0d00 0000 6302  lit_dir).r....c.
+00001350: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00001360: 0000 0043 0000 0073 3400 0000 7c01 6400  ...C...s4...|.d.
+00001370: 7501 720c 7c01 6e12 7400 6a01 a002 7c00  u.r.|.n.t.j...|.
+00001380: 6a03 7404 6a05 6a06 a102 7d02 7400 6a01  j.t.j.j...}.t.j.
+00001390: a007 7c02 a101 7230 7c02 5300 6400 5300  ..|...r0|.S.d.S.
+000013a0: 720f 0000 0029 0872 1100 0000 7212 0000  r....).r....r...
+000013b0: 0072 4e00 0000 7214 0000 0072 0600 0000  .rN...r....r....
+000013c0: da05 6d6f 6465 6c72 2300 0000 725d 0000  ..modelr#...r]..
+000013d0: 0029 0372 1e00 0000 720d 0000 0072 5e00  .).r....r....r^.
+000013e0: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
+000013f0: 0072 1900 0000 c200 0000 730a 0000 0000  .r........s.....
+00001400: 0306 ff06 0212 fd02 057a 1c53 7061 7469  .........z.Spati
+00001410: 616c 4461 7461 7365 742e 7365 745f 6d6f  alDataset.set_mo
+00001420: 6465 6c5f 6469 7229 0172 0e00 0000 6302  del_dir).r....c.
+00001430: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00001440: 0000 0043 0000 0073 3400 0000 7c01 6400  ...C...s4...|.d.
+00001450: 7501 720c 7c01 6e12 7400 6a01 a002 7c00  u.r.|.n.t.j...|.
+00001460: 6a03 7404 6a05 6a06 a102 7d02 7400 6a01  j.t.j.j...}.t.j.
+00001470: a007 7c02 a101 7230 7c02 5300 6400 5300  ..|...r0|.S.d.S.
+00001480: 720f 0000 0029 0872 1100 0000 7212 0000  r....).r....r...
+00001490: 0072 4e00 0000 7214 0000 0072 0600 0000  .rN...r....r....
+000014a0: 5a0e 636f 756e 7465 7266 6163 7475 616c  Z.counterfactual
+000014b0: 7223 0000 0072 5d00 0000 2903 721e 0000  r#...r]...).r...
+000014c0: 0072 0e00 0000 725e 0000 0072 2000 0000  .r....r^...r ...
+000014d0: 7220 0000 0072 2100 0000 721a 0000 00ca  r ...r!...r.....
+000014e0: 0000 0073 0a00 0000 0003 06ff 0602 12fd  ...s............
+000014f0: 0205 7a25 5370 6174 6961 6c44 6174 6173  ..z%SpatialDatas
+00001500: 6574 2e73 6574 5f63 6f75 6e74 6572 6661  et.set_counterfa
+00001510: 6374 7561 6c5f 6469 7263 0100 0000 0000  ctual_dirc......
+00001520: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+00001530: 0000 7394 0000 0074 007c 0064 0183 0273  ..s....t.|.d...s
+00001540: 1274 0164 0283 0182 0174 007c 0064 0383  .t.d.....t.|.d..
+00001550: 0273 2474 0164 0483 0182 0174 027c 006a  .s$t.d.....t.|.j
+00001560: 0383 017c 006a 0374 046a 056a 0619 00a0  ...|.j.t.j.j....
+00001570: 07a1 006b 0372 4874 0164 0583 0182 0174  ...k.rHt.d.....t
+00001580: 027c 006a 0883 017c 006a 096b 0372 6074  .|.j...|.j.k.r`t
+00001590: 0164 0683 0182 0174 046a 0a6a 0674 046a  .d.....t.j.j.t.j
+000015a0: 056a 0666 0244 005d 1e7d 017c 017c 006a  .j.f.D.].}.|.|.j
+000015b0: 036a 0b76 0172 7074 0164 077c 019b 009d  .j.v.rpt.d.|....
+000015c0: 0283 0182 0171 7064 0053 0029 084e 7210  .....qpd.S.).Nr.
+000015d0: 0000 007a 134d 6574 6164 6174 6120 6e6f  ...z.Metadata no
+000015e0: 7420 6c6f 6164 6564 720a 0000 007a 1843  t loadedr....z.C
+000015f0: 6861 6e6e 656c 206e 616d 6573 206e 6f74  hannel names not
+00001600: 206c 6f61 6465 647a 254d 6574 6164 6174   loadedz%Metadat
+00001610: 6120 636f 6e74 6169 6e73 2064 7570 6c69  a contains dupli
+00001620: 6361 7465 2070 6174 6368 2049 4473 7245  cate patch IDsrE
+00001630: 0000 007a 194d 6574 6164 6174 6120 6d69  ...z.Metadata mi
+00001640: 7373 696e 6720 636f 6c75 6d6e 3a20 290c  ssing column: ).
+00001650: da07 6861 7361 7474 7272 3800 0000 7232  ..hasattrr8...r2
+00001660: 0000 0072 1000 0000 7204 0000 0072 5200  ...r....r....rR.
+00001670: 0000 7223 0000 005a 076e 756e 6971 7565  ..r#...Z.nunique
+00001680: 720a 0000 00da 0a6e 5f63 6861 6e6e 656c  r......n_channel
+00001690: 7372 2f00 0000 7233 0000 0029 0272 1e00  sr/...r3...).r..
+000016a0: 0000 722b 0000 0072 2000 0000 7220 0000  ..r+...r ...r ..
+000016b0: 0072 2100 0000 721c 0000 00d2 0000 0073  .r!...r........s
+000016c0: 1600 0000 0002 0a01 0801 0a01 0803 1c01  ................
+000016d0: 0801 1001 0803 1401 0c01 7a21 5370 6174  ..........z!Spat
+000016e0: 6961 6c44 6174 6173 6574 2e63 6865 636b  ialDataset.check
+000016f0: 5f6c 6f61 6465 645f 7061 7463 6863 0100  _loaded_patchc..
+00001700: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
+00001710: 0000 4300 0000 73ce 0000 007a 9674 00a0  ..C...s....z.t..
+00001720: 017c 006a 0264 01a1 028f 747d 0174 03a0  .|.j.d....t}.t..
+00001730: 047c 0164 0219 0064 0064 0085 0219 00a1  .|.d...d.d......
+00001740: 017c 005f 0564 0364 0484 007c 0164 0519  .|._.d.d...|.d..
+00001750: 0064 0064 0085 0219 0044 0083 017c 005f  .d.d.....D...|._
+00001760: 067c 0164 0619 006a 077d 027c 0264 0719  .|.d...j.}.|.d..
+00001770: 007c 0264 0864 0985 0219 007c 0264 0919  .|.d.d.....|.d..
+00001780: 0003 0002 007c 005f 087c 005f 097c 005f  .....|._.|._.|._
+00001790: 0a57 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
+000017a0: 0073 8a30 0001 0001 0001 0059 0001 0057  .s.0.......Y...W
+000017b0: 006e 3204 0074 0b79 c801 007d 0301 007a  .n2..t.y...}...z
+000017c0: 1a74 0c64 0a7c 039b 009d 0283 0101 0057  .t.d.|.........W
+000017d0: 0059 0064 007d 037e 036e 0a64 007d 037e  .Y.d.}.~.n.d.}.~
+000017e0: 0330 0030 0064 0053 0029 0b4e da01 7272  .0.0.d.S.).N..rr
+000017f0: 1000 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00001800: 0002 0000 0005 0000 0053 0000 0073 1600  .........S...s..
+00001810: 0000 6700 7c00 5d0e 7d01 7c01 a000 6400  ..g.|.].}.|...d.
+00001820: a101 9102 7104 5300 2901 7a05 7574 662d  ....q.S.).z.utf-
+00001830: 3829 01da 0664 6563 6f64 6529 0272 2a00  8)...decode).r*.
+00001840: 0000 da04 6e61 6d65 7220 0000 0072 2000  ....namer ...r .
+00001850: 0000 7221 0000 0072 2d00 0000 e800 0000  ..r!...r-.......
+00001860: 7302 0000 0006 017a 3253 7061 7469 616c  s......z2Spatial
+00001870: 4461 7461 7365 742e 6c6f 6164 5f70 6174  Dataset.load_pat
+00001880: 6368 5f64 6174 612e 3c6c 6f63 616c 733e  ch_data.<locals>
+00001890: 2e3c 6c69 7374 636f 6d70 3e72 0a00 0000  .<listcomp>r....
+000018a0: 7247 0000 0072 0100 0000 e901 0000 0072  rG...r.........r
+000018b0: 3c00 0000 7a14 4572 726f 7220 6c6f 6164  <...z.Error load
+000018c0: 696e 6720 6461 7461 3a20 290d 7254 0000  ing data: ).rT..
+000018d0: 0072 5500 0000 720b 0000 0072 3900 0000  .rU...r....r9...
+000018e0: da09 4461 7461 4672 616d 6572 1000 0000  ..DataFramer....
+000018f0: 720a 0000 0072 5300 0000 da09 6e5f 7061  r....rS.....n_pa
+00001900: 7463 6865 735a 0869 6d67 5f73 697a 6572  tchesZ.img_sizer
+00001910: 6100 0000 da09 4578 6365 7074 696f 6e72  a.....Exceptionr
+00001920: 3400 0000 2904 721e 0000 0072 5b00 0000  4...).r....r[...
+00001930: 5a0a 6461 7461 5f73 6861 7065 da01 6572  Z.data_shape..er
+00001940: 2000 0000 7220 0000 0072 2100 0000 721b   ...r ...r!...r.
+00001950: 0000 00e4 0000 0073 1a00 0000 0001 0201  .......s........
+00001960: 1001 1801 0601 0eff 0803 0a02 0601 0a01  ................
+00001970: 06fd 3205 0e01 7a1e 5370 6174 6961 6c44  ..2...z.SpatialD
+00001980: 6174 6173 6574 2e6c 6f61 645f 7061 7463  ataset.load_patc
+00001990: 685f 6461 7461 2901 da0a 7370 6c69 745f  h_data)...split_
+000019a0: 6e61 6d65 6302 0000 0000 0000 0000 0000  namec...........
+000019b0: 0004 0000 000a 0000 0043 0000 0073 6a00  .........C...sj.
+000019c0: 0000 7400 6a01 a002 7c00 6a03 7c01 7404  ..t.j...|.j.|.t.
+000019d0: 6a05 6a06 a103 7d02 7a16 7407 a008 7c02  j.j...}.z.t...|.
+000019e0: a101 7409 6a0a 6a06 1900 6a0b 5700 5300  ..t.j.j...j.W.S.
+000019f0: 0400 740c 7964 0100 7d03 0100 7a20 740d  ..t.yd..}...z t.
+00001a00: 6401 7c01 9b00 6402 7c03 9b00 9d04 8301  d.|...d.|.......
+00001a10: 0100 5700 5900 6400 7d03 7e03 6e0a 6400  ..W.Y.d.}.~.n.d.
+00001a20: 7d03 7e03 3000 3000 6400 5300 2903 4e7a  }.~.0.0.d.S.).Nz
+00001a30: 1445 7272 6f72 206c 6f61 6469 6e67 2073  .Error loading s
+00001a40: 706c 6974 20fa 023a 2029 0e72 1100 0000  plit ..: ).r....
+00001a50: 7212 0000 0072 4e00 0000 720c 0000 0072  r....rN...r....r
+00001a60: 0700 0000 da05 6c61 6265 6c72 2300 0000  ......labelr#...
+00001a70: 7239 0000 0072 3a00 0000 7204 0000 0072  r9...r:...r....r
+00001a80: 5200 0000 da06 7661 6c75 6573 7268 0000  R.....valuesrh..
+00001a90: 0072 3400 0000 2904 721e 0000 0072 6a00  .r4...).r....rj.
+00001aa0: 0000 5a0a 6c61 6265 6c5f 7061 7468 7269  ..Z.label_pathri
+00001ab0: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
+00001ac0: 0000 7225 0000 00f4 0000 0073 0e00 0000  ..r%.......s....
+00001ad0: 0001 0601 0cff 0403 0201 1601 0e01 7a1c  ..............z.
+00001ae0: 5370 6174 6961 6c44 6174 6173 6574 2e67  SpatialDataset.g
+00001af0: 6574 5f73 706c 6974 5f69 6473 e733 3333  et_split_ids.333
+00001b00: 3333 33e3 3fe7 9a99 9999 9999 c93f 2904  333.?........?).
+00001b10: da0b 7374 7261 7469 6679 5f62 79da 0a74  ..stratify_by..t
+00001b20: 7261 696e 5f73 697a 65da 0876 616c 5f73  rain_size..val_s
+00001b30: 697a 65da 0974 6573 745f 7369 7a65 630b  ize..test_sizec.
+00001b40: 0000 0000 0000 0000 0000 000c 0000 0007  ................
+00001b50: 0000 0003 0000 0073 fa00 0000 7c01 7c00  .......s....|.|.
+00001b60: 5f00 7c08 6401 7500 721a 6402 6403 6404  _.|.d.u.r.d.d.d.
+00001b70: 6405 9c03 7d08 7c05 6401 7500 723a 7401  d...}.|.d.u.r:t.
+00001b80: 6a02 a003 7c00 6a04 7405 6a06 6a07 a102  j...|.j.t.j.j...
+00001b90: 7c00 5f08 6e06 7c05 7c00 5f08 7401 6a02  |._.n.|.|._.t.j.
+00001ba0: a009 7401 6a02 a003 7c00 6a08 740a 6a0b  ..t.j...|.j.t.j.
+00001bb0: 6a07 a102 a101 7270 740c 6406 7c00 6a08  j.....rpt.d.|.j.
+00001bc0: 9b00 9d02 8301 0100 6401 5300 740c 6407  ........d.S.t.d.
+00001bd0: 8301 0100 8800 6401 7501 7298 8700 6601  ......d.u.r...f.
+00001be0: 6408 6409 8408 740d 740a 8301 4400 8301  d.d...t.t...D...
+00001bf0: 7d0b 6e1c 7c00 6a0e 7c01 7c02 7c03 7c04  }.n.|.j.|.|.|.|.
+00001c00: 7c06 7c07 6606 6900 7c08 a401 8e01 7d0b  |.|.f.i.|.....}.
+00001c10: 7c0b 6401 7500 72c4 740f 640a 8301 8201  |.d.u.r.t.d.....
+00001c20: 7c0a 72f6 740c 640b 8301 0100 7c00 6a10  |.r.t.d.....|.j.
+00001c30: 7c0b 7c01 640c 8d02 0100 740c 640d 7c00  |.|.d.....t.d.|.
+00001c40: 6a08 9b00 9d02 8301 0100 7c00 a011 a100  j.........|.....
+00001c50: 0100 7c0b 5300 290e 6103 0500 000a 2020  ..|.S.).a.....  
+00001c60: 2020 2020 2020 4765 6e65 7261 7465 2074        Generate t
+00001c70: 7261 696e 2c20 7661 6c69 6461 7469 6f6e  rain, validation
+00001c80: 2c20 616e 6420 7465 7374 2064 6174 6120  , and test data 
+00001c90: 7370 6c69 7473 2c20 616e 6420 7361 7665  splits, and save
+00001ca0: 2074 6865 2064 6174 6120 7370 6c69 7473   the data splits
+00001cb0: 2074 6f20 7468 6520 6769 7665 6e20 6469   to the given di
+00001cc0: 7265 6374 6f72 790a 0a20 2020 2020 2020  rectory..       
+00001cd0: 2041 7267 733a 0a20 2020 2020 2020 2073   Args:.        s
+00001ce0: 7472 6174 6966 795f 6279 3a20 7374 720a  tratify_by: str.
+00001cf0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00001d00: 636f 6c75 6d6e 206e 616d 6520 746f 2073  column name to s
+00001d10: 7472 6174 6966 7920 7468 6520 6461 7461  tratify the data
+00001d20: 2062 790a 2020 2020 2020 2020 7361 7665   by.        save
+00001d30: 5f64 6972 3a20 7374 720a 2020 2020 2020  _dir: str.      
+00001d40: 2020 2020 2020 5468 6520 6469 7265 6374        The direct
+00001d50: 6f72 7920 746f 2073 6176 6520 7468 6520  ory to save the 
+00001d60: 6461 7461 2073 706c 6974 730a 2020 2020  data splits.    
+00001d70: 2020 2020 7472 6169 6e5f 7369 7a65 3a20      train_size: 
+00001d80: 666c 6f61 740a 2020 2020 2020 2020 2020  float.          
+00001d90: 2020 5468 6520 7072 6f70 6f72 7469 6f6e    The proportion
+00001da0: 206f 6620 7468 6520 6461 7461 7365 7420   of the dataset 
+00001db0: 746f 2069 6e63 6c75 6465 2069 6e20 7468  to include in th
+00001dc0: 6520 7472 6169 6e20 7370 6c69 740a 2020  e train split.  
+00001dd0: 2020 2020 2020 7661 6c5f 7369 7a65 3a20        val_size: 
+00001de0: 666c 6f61 740a 2020 2020 2020 2020 2020  float.          
+00001df0: 2020 5468 6520 7072 6f70 6f72 7469 6f6e    The proportion
+00001e00: 206f 6620 7468 6520 6461 7461 7365 7420   of the dataset 
+00001e10: 746f 2069 6e63 6c75 6465 2069 6e20 7468  to include in th
+00001e20: 6520 7661 6c69 6461 7469 6f6e 2073 706c  e validation spl
+00001e30: 6974 0a20 2020 2020 2020 2074 6573 745f  it.        test_
+00001e40: 7369 7a65 3a20 666c 6f61 740a 2020 2020  size: float.    
+00001e50: 2020 2020 2020 2020 5468 6520 7072 6f70          The prop
+00001e60: 6f72 7469 6f6e 206f 6620 7468 6520 6461  ortion of the da
+00001e70: 7461 7365 7420 746f 2069 6e63 6c75 6465  taset to include
+00001e80: 2069 6e20 7468 6520 7465 7374 2073 706c   in the test spl
+00001e90: 6974 0a20 2020 2020 2020 2072 616e 646f  it.        rando
+00001ea0: 6d5f 7374 6174 653a 2069 6e74 0a20 2020  m_state: int.   
+00001eb0: 2020 2020 2020 2020 2043 6f6e 7472 6f6c           Control
+00001ec0: 7320 7468 6520 7368 7566 666c 696e 6720  s the shuffling 
+00001ed0: 6170 706c 6965 6420 746f 2074 6865 2064  applied to the d
+00001ee0: 6174 6120 6265 666f 7265 2061 7070 6c79  ata before apply
+00001ef0: 696e 6720 7468 6520 7370 6c69 742e 0a20  ing the split.. 
+00001f00: 2020 2020 2020 2073 6875 6666 6c65 3a20         shuffle: 
+00001f10: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
+00001f20: 2057 6865 7468 6572 2074 6f20 7368 7566   Whether to shuf
+00001f30: 666c 6520 7468 6520 6461 7461 2062 6566  fle the data bef
+00001f40: 6f72 6520 7370 6c69 7474 696e 670a 2020  ore splitting.  
+00001f50: 2020 2020 2020 746f 6c65 7261 6e63 653a        tolerance:
+00001f60: 2064 6963 740a 2020 2020 2020 2020 2020   dict.          
+00001f70: 2020 4120 6469 6374 696f 6e61 7279 206f    A dictionary o
+00001f80: 6620 746f 6c65 7261 6e63 6520 7061 7261  f tolerance para
+00001f90: 6d65 7465 7273 2074 6f20 636f 6e74 726f  meters to contro
+00001fa0: 6c20 7468 6520 6461 7461 2073 706c 6974  l the data split
+00001fb0: 2067 656e 6572 6174 696f 6e0a 2020 2020   generation.    
+00001fc0: 2020 2020 2020 2020 2d20 6570 733a 2066          - eps: f
+00001fd0: 6c6f 6174 0a20 2020 2020 2020 2020 2020  loat.           
+00001fe0: 2020 2020 2054 6865 2074 6f6c 6572 616e       The toleran
+00001ff0: 6365 2066 6f72 2074 6865 2064 6966 6665  ce for the diffe
+00002000: 7265 6e63 6520 696e 2070 726f 706f 7274  rence in proport
+00002010: 696f 6e73 2062 6574 7765 656e 2074 6865  ions between the
+00002020: 2074 7261 696e 2061 6e64 2074 6573 742f   train and test/
+00002030: 7661 6c69 6461 7465 2073 706c 6974 730a  validate splits.
+00002040: 2020 2020 2020 2020 2020 2020 2d20 7472              - tr
+00002050: 6169 6e5f 6c62 3a20 666c 6f61 740a 2020  ain_lb: float.  
+00002060: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+00002070: 6520 6c6f 7765 7220 626f 756e 6420 666f  e lower bound fo
+00002080: 7220 7468 6520 7072 6f70 6f72 7469 6f6e  r the proportion
+00002090: 206f 6620 7468 6520 7472 6169 6e20 7370   of the train sp
+000020a0: 6c69 740a 2020 2020 2020 2020 2020 2020  lit.            
+000020b0: 2d20 6e5f 746f 6c3a 2069 6e74 0a20 2020  - n_tol: int.   
+000020c0: 2020 2020 2020 2020 2020 2020 2054 6865               The
+000020d0: 206e 756d 6265 7220 6f66 2061 7474 656d   number of attem
+000020e0: 7074 7320 746f 2067 656e 6572 6174 6520  pts to generate 
+000020f0: 6120 7661 6c69 6420 6461 7461 2073 706c  a valid data spl
+00002100: 6974 0a20 2020 2020 2020 2073 6176 653a  it.        save:
+00002110: 2062 6f6f 6c0a 2020 2020 2020 2020 2020   bool.          
+00002120: 2020 5768 6574 6865 7220 746f 2073 6176    Whether to sav
+00002130: 6520 7468 6520 6461 7461 2073 706c 6974  e the data split
+00002140: 7320 746f 2074 6865 2073 6176 6520 6469  s to the save di
+00002150: 7265 6374 6f72 790a 2020 2020 2020 2020  rectory.        
+00002160: 4ee7 7b14 ae47 e17a 843f 6700 0000 0000  N.{..G.z.?g.....
+00002170: 00e0 3f72 4900 0000 2903 da03 6570 73da  ..?rI...)...eps.
+00002180: 0874 7261 696e 5f6c 62da 056e 5f74 6f6c  .train_lb..n_tol
+00002190: 7a1d 4461 7461 2073 706c 6974 7320 616c  z.Data splits al
+000021a0: 7265 6164 7920 6578 6973 7420 696e 207a  ready exist in z
+000021b0: 1947 656e 6572 6174 696e 6720 6461 7461  .Generating data
+000021c0: 2073 706c 6974 732e 2e2e 6301 0000 0000   splits...c.....
+000021d0: 0000 0000 0000 0003 0000 0007 0000 0013  ................
+000021e0: 0000 0073 2200 0000 6900 7c00 5d1a 5c02  ...s"...i.|.].\.
+000021f0: 7d01 7d02 7c02 6a00 7401 a002 8800 7c01  }.}.|.j.t.....|.
+00002200: 1900 a101 9302 7104 5300 7220 0000 0029  ......q.S.r ...)
+00002210: 0372 2300 0000 da02 6e70 da05 6172 7261  .r#.....np..arra
+00002220: 7929 0372 2a00 0000 da03 6964 7872 6400  y).r*.....idxrd.
+00002230: 0000 a901 da0c 6769 7665 6e5f 7370 6c69  ......given_spli
+00002240: 7473 7220 0000 0072 2100 0000 da0a 3c64  tsr ...r!.....<d
+00002250: 6963 7463 6f6d 703e 3801 0000 7304 0000  ictcomp>8...s...
+00002260: 0006 0206 ff7a 3753 7061 7469 616c 4461  .....z7SpatialDa
+00002270: 7461 7365 742e 6765 6e65 7261 7465 5f64  taset.generate_d
+00002280: 6174 615f 7370 6c69 7473 2e3c 6c6f 6361  ata_splits.<loca
+00002290: 6c73 3e2e 3c64 6963 7463 6f6d 703e 7a49  ls>.<dictcomp>zI
+000022a0: 436f 756c 6420 6e6f 7420 7361 7469 7366  Could not satisf
+000022b0: 7920 6461 7461 2073 706c 6974 2063 6f6e  y data split con
+000022c0: 7374 7261 696e 7473 2c20 7472 7920 6167  straints, try ag
+000022d0: 6169 6e20 6f72 2061 646a 7573 7420 636f  ain or adjust co
+000022e0: 6e73 7472 6169 6e74 737a 1053 6176 696e  nstraintsz.Savin
+000022f0: 6720 7370 6c69 7473 2e2e 2e29 01da 0a6c  g splits...)...l
+00002300: 6162 656c 5f6e 616d 657a 1544 6174 6120  abel_namez.Data 
+00002310: 7370 6c69 7473 2073 6176 6564 2074 6f20  splits saved to 
+00002320: 2912 727e 0000 0072 1100 0000 7212 0000  ).r~...r....r...
+00002330: 0072 4e00 0000 7214 0000 0072 0600 0000  .rN...r....r....
+00002340: 7227 0000 0072 2300 0000 720c 0000 0072  r'...r#...r....r
+00002350: 5d00 0000 7205 0000 00da 0574 7261 696e  ]...r......train
+00002360: 7234 0000 00da 0965 6e75 6d65 7261 7465  r4.....enumerate
+00002370: da12 6765 745f 7061 7469 656e 745f 7370  ..get_patient_sp
+00002380: 6c69 7473 7238 0000 00da 0b73 6176 655f  litsr8.....save_
+00002390: 7370 6c69 7473 721d 0000 0029 0c72 1e00  splitsr....).r..
+000023a0: 0000 7270 0000 0072 7100 0000 7272 0000  ..rp...rq...rr..
+000023b0: 0072 7300 0000 da08 7361 7665 5f64 6972  .rs.....save_dir
+000023c0: da0c 7261 6e64 6f6d 5f73 7461 7465 da07  ..random_state..
+000023d0: 7368 7566 666c 65da 0974 6f6c 6572 616e  shuffle..toleran
+000023e0: 6365 727c 0000 0072 4100 0000 da0d 7061  cer|...rA.....pa
+000023f0: 7469 656e 745f 7370 6c69 7472 2000 0000  tient_splitr ...
+00002400: 727b 0000 0072 2100 0000 da14 6765 6e65  r{...r!.....gene
+00002410: 7261 7465 5f64 6174 615f 7370 6c69 7473  rate_data_splits
+00002420: fd00 0000 7348 0000 0000 2a06 0208 010c  ....sH....*.....
+00002430: 0108 0106 010a ff08 0406 021c 0110 0104  ................
+00002440: 0208 0108 010a 0206 fe08 0504 0102 0102  ................
+00002450: 0102 0102 0102 0102 fa04 0702 f906 0a08  ................
+00002460: 0102 0102 ff04 0404 0108 010e 0110 0108  ................
+00002470: 017a 2353 7061 7469 616c 4461 7461 7365  .z#SpatialDatase
+00002480: 742e 6765 6e65 7261 7465 5f64 6174 615f  t.generate_data_
+00002490: 7370 6c69 7473 7274 0000 00e7 cdcc cccc  splitsrt........
+000024a0: cccc e43f 6303 0000 0000 0000 0000 0000  ...?c...........
+000024b0: 0006 0000 0004 0000 0043 0000 0073 7000  .........C...sp.
+000024c0: 0000 7c00 7400 6a01 6a02 1900 6401 1900  ..|.t.j.j...d...
+000024d0: 7d03 7403 7c00 7400 6a01 6a02 1900 6402  }.t.|.t.j.j...d.
+000024e0: 1900 7c00 7400 6a04 6a02 1900 6402 1900  ..|.t.j.j...d...
+000024f0: 1800 8301 7d04 7403 7c00 7400 6a01 6a02  ....}.t.|.t.j.j.
+00002500: 1900 6402 1900 7c00 7400 6a05 6a02 1900  ..d...|.t.j.j...
+00002510: 6402 1900 1800 8301 7d05 7c04 7c01 6b00  d.......}.|.|.k.
+00002520: 6f6e 7c05 7c01 6b00 6f6e 7c03 7c02 6b04  on|.|.k.on|.|.k.
+00002530: 5300 2903 4e72 0100 0000 7265 0000 0029  S.).Nr....re...)
+00002540: 0672 0500 0000 727f 0000 0072 2300 0000  .r....r....r#...
+00002550: da03 6162 73da 0474 6573 74da 0876 616c  ..abs..test..val
+00002560: 6964 6174 6529 06da 0a73 706c 6974 5f69  idate)...split_i
+00002570: 6e66 6f72 7500 0000 7276 0000 005a 0774  nforu...rv...Z.t
+00002580: 725f 7072 6f70 5a0a 7472 5f74 655f 6469  r_propZ.tr_te_di
+00002590: 6666 5a0a 7472 5f76 615f 6469 6666 7220  ffZ.tr_va_diffr 
+000025a0: 0000 0072 2000 0000 7221 0000 00da 0e69  ...r ...r!.....i
+000025b0: 735f 7661 6c69 645f 7370 6c69 7453 0100  s_valid_splitS..
+000025c0: 0073 1000 0000 0002 1001 0201 1eff 0403  .s..............
+000025d0: 0201 1eff 0403 7a1d 5370 6174 6961 6c44  ......z.SpatialD
+000025e0: 6174 6173 6574 2e69 735f 7661 6c69 645f  ataset.is_valid_
+000025f0: 7370 6c69 74e9 2a00 0000 7249 0000 0063  split.*...rI...c
+00002600: 0a00 0000 0000 0000 0000 0000 1700 0000  ................
+00002610: 0800 0000 4300 0000 7370 0100 007c 027c  ....C...sp...|.|
+00002620: 0317 007c 0417 0064 016b 0273 184a 0064  ...|...d.k.s.J.d
+00002630: 0283 0182 0174 00a0 017c 006a 0274 036a  .....t...|.j.t.j
+00002640: 046a 0519 00a1 017d 0a74 067c 006a 0283  .j.....}.t.|.j..
+00002650: 017d 0b64 037d 0c64 047d 0d7c 0c90 0173  .}.d.}.d.}.|...s
+00002660: 6c7c 0d7c 076b 0090 0172 6c7c 0672 6874  l|.|.k...rl|.rht
+00002670: 006a 07a0 087c 05a1 017d 0e7c 0ea0 097c  .j...|...}.|...|
+00002680: 0aa1 0101 0074 0a74 067c 0a83 017c 0214  .....t.t.|...|..
+00002690: 0083 017d 0f7c 0f74 0a74 067c 0a83 017c  ...}.|.t.t.|...|
+000026a0: 0314 0083 0117 007d 1074 0b6a 0c6a 057c  .......}.t.j.j.|
+000026b0: 0a64 007c 0f85 0219 0074 0b6a 0d6a 057c  .d.|.....t.j.j.|
+000026c0: 0a7c 0f7c 1085 0219 0074 0b6a 0e6a 057c  .|.|.....t.j.j.|
+000026d0: 0a7c 1064 0085 0219 0069 037d 1169 007d  .|.d.....i.}.i.}
+000026e0: 127c 11a0 0fa1 0044 005d 3e5c 027d 137d  .|.....D.]>\.}.}
+000026f0: 147c 006a 027c 006a 0274 036a 046a 0519  .|.j.|.j.t.j.j..
+00002700: 00a0 107c 14a1 0119 007d 1574 067c 1583  ...|.....}.t.|..
+00002710: 017c 0b1b 007c 157c 0119 00a0 11a1 0067  .|...|.|.......g
+00002720: 027c 127c 133c 0071 cc74 12a0 137c 127c  .|.|.<.q.t...|.|
+00002730: 087c 09a1 0390 0172 6274 1464 0583 0101  .|.....rbt.d....
+00002740: 007c 12a0 0fa1 0044 005d 305c 027d 137d  .|.....D.]0\.}.}
+00002750: 1674 147c 1364 069b 0464 077c 1664 0419  .t.|.d...d.|.d..
+00002760: 0064 089b 0464 097c 1664 0119 0064 089b  .d...d.|.d...d..
+00002770: 049d 0583 0101 0090 0171 2c7c 1153 007c  .........q,|.S.|
+00002780: 0d64 0137 007d 0d71 3e64 0053 0029 0a4e  .d.7.}.q>d.S.).N
+00002790: 7265 0000 007a 3374 7261 696e 5f73 697a  re...z3train_siz
+000027a0: 652c 2076 616c 5f73 697a 652c 2061 6e64  e, val_size, and
+000027b0: 2074 6573 745f 7369 7a65 2073 686f 756c   test_size shoul
+000027c0: 6420 7375 6d20 746f 2031 4672 0100 0000  d sum to 1Fr....
+000027d0: 7a4d 5370 6c69 7420 636f 6e73 7472 6169  zMSplit constrai
+000027e0: 6e74 7320 7361 7469 7366 6965 640a 5061  nts satisfied.Pa
+000027f0: 7463 6820 7072 6f70 6f72 7469 6f6e 7320  tch proportions 
+00002800: 616e 6420 506f 7369 7469 7665 2070 6174  and Positive pat
+00002810: 6368 2070 726f 706f 7274 696f 6e73 3a7a  ch proportions:z
+00002820: 033c 3130 726b 0000 007a 053e 352e 3366  .<10rk...z.>5.3f
+00002830: 7a02 2c20 2915 7278 0000 00da 0675 6e69  z., ).rx.....uni
+00002840: 7175 6572 1000 0000 7204 0000 0072 2f00  quer....r....r/.
+00002850: 0000 7223 0000 0072 3200 0000 da06 7261  ..r#...r2.....ra
+00002860: 6e64 6f6d da0b 6465 6661 756c 745f 726e  ndom..default_rn
+00002870: 6772 8500 0000 da03 696e 7472 0500 0000  gr......intr....
+00002880: 727f 0000 0072 8c00 0000 728b 0000 00da  r....r....r.....
+00002890: 0569 7465 6d73 da04 6973 696e da04 6d65  .items..isin..me
+000028a0: 616e 7208 0000 0072 8e00 0000 7234 0000  anr....r....r4..
+000028b0: 0029 1772 1e00 0000 7270 0000 0072 7100  .).r....rp...rq.
+000028c0: 0000 7272 0000 0072 7300 0000 7284 0000  ..rr...rs...r...
+000028d0: 0072 8500 0000 7277 0000 0072 7500 0000  .r....rw...ru...
+000028e0: 7276 0000 0072 2f00 0000 7267 0000 005a  rv...r/...rg...Z
+000028f0: 0c69 7356 616c 6964 5370 6c69 74da 0763  .isValidSplit..c
+00002900: 6f75 6e74 6572 da03 726e 675a 0974 7261  ounter..rngZ.tra
+00002910: 696e 5f65 6e64 5a09 7661 6c69 645f 656e  in_endZ.valid_en
+00002920: 6472 8700 0000 728d 0000 0072 2700 0000  dr....r....r'...
+00002930: da03 7061 745a 0864 6174 615f 7375 62da  ..patZ.data_sub.
+00002940: 0364 6174 7220 0000 0072 2000 0000 7221  .datr ...r ...r!
+00002950: 0000 0072 8100 0000 5e01 0000 7346 0000  ...r....^...sF..
+00002960: 0000 0d0e ff04 0202 fe04 0414 010a 0104  ................
+00002970: 0104 0110 0104 010c 010a 0110 0114 0210  ................
+00002980: 0110 0110 fd04 0604 0110 0104 0112 ff04  ................
+00002990: 040a 010a fe0a 0510 0102 0102 ff04 0310  ................
+000029a0: 012a 0104 020a 017a 2153 7061 7469 616c  .*.....z!Spatial
+000029b0: 4461 7461 7365 742e 6765 745f 7061 7469  Dataset.get_pati
+000029c0: 656e 745f 7370 6c69 7473 6301 0000 0000  ent_splitsc.....
+000029d0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+000029e0: 0000 0073 0400 0000 6400 5300 720f 0000  ...s....d.S.r...
+000029f0: 0072 2000 0000 a901 721e 0000 0072 2000  .r .....r....r .
+00002a00: 0000 7220 0000 0072 2100 0000 da0f 7375  ..r ...r!.....su
+00002a10: 6d6d 6172 697a 655f 7370 6c69 7493 0100  mmarize_split...
+00002a20: 0073 0200 0000 0001 7a1e 5370 6174 6961  .s......z.Spatia
+00002a30: 6c44 6174 6173 6574 2e73 756d 6d61 7269  lDataset.summari
+00002a40: 7a65 5f73 706c 6974 6303 0000 0000 0000  ze_splitc.......
+00002a50: 0000 0000 0012 0000 0009 0000 0003 0000  ................
+00002a60: 0073 2c02 0000 6401 6402 6c00 6d00 7d03  .s,...d.d.l.m.}.
+00002a70: 0100 8700 6601 6403 6404 8408 7c01 a001  ....f.d.d...|...
+00002a80: a100 4400 8301 7d04 7402 a003 8800 6a04  ..D...}.t.....j.
+00002a90: 6405 a102 8f20 7d05 7c05 6406 1900 6400  d.... }.|.d...d.
+00002aa0: 6400 8502 1900 7d06 5700 6400 0400 0400  d.....}.W.d.....
+00002ab0: 8303 0100 6e10 3100 7356 3000 0100 0100  ....n.1.sV0.....
+00002ac0: 0100 5900 0100 6400 7d07 7c03 7405 6407  ..Y...d.}.|.t.d.
+00002ad0: 6408 8d02 4400 9001 5d70 7d08 7c04 7c08  d...D...]p}.|.|.
+00002ae0: 6a06 1900 7d09 7c06 7c09 6409 6602 1900  j...}.|.|.d.f...
+00002af0: 7d0a 8800 6a07 6a08 7c09 1900 7c02 1900  }...j.j.|...|...
+00002b00: 6a09 a00a 740b a101 7d0b 8800 6a07 6a08  j...t...}...j.j.
+00002b10: 7c09 1900 740c 6a0d 6a06 1900 6a09 7d0c  |...t.j.j...j.}.
+00002b20: 8800 6a07 6a08 7c09 1900 740c 6a0d 6a06  ..j.j.|...t.j.j.
+00002b30: 7c02 740c 6a0e 6a06 740c 6a0f 6a06 6704  |.t.j.j.t.j.j.g.
+00002b40: 1900 7d0d 7410 6a11 a012 8800 6a13 7c08  ..}.t.j.....j.|.
+00002b50: 6a06 a102 7d0e 7410 6a11 a014 7c0e a101  j...}.t.j...|...
+00002b60: 9001 7330 7410 a015 7c0e a101 0100 7410  ..s0t...|.....t.
+00002b70: a015 7410 6a11 a012 7c0e 640a a102 a101  ..t.j...|.d.....
+00002b80: 0100 7410 a015 7410 6a11 a012 7c0e 640b  ..t...t.j...|.d.
+00002b90: a102 a101 0100 7c0d 6a16 7410 6a11 a012  ......|.j.t.j...
+00002ba0: 7c0e 7417 6a18 6a06 a102 640c 640d 8d02  |.t.j.j...d.d...
+00002bb0: 0100 7419 7c0b 8301 7d0f 7c03 741a 7c0f  ..t.|...}.|.t.|.
+00002bc0: 8301 640e 7c08 6a06 9b00 640f 9d03 640c  ..d.|.j...d...d.
+00002bd0: 6410 8d03 4400 5d3c 7d10 7410 6a11 a012  d...D.]<}.t.j...
+00002be0: 7c0e 7c0b 7c10 1900 9b00 6411 7c0c 7c10  |.|.|.....d.|.|.
+00002bf0: 1900 9b00 6412 9d04 a102 7d11 741b a01c  ....d.....}.t...
+00002c00: 7c11 7c0a 7c10 6409 6602 1900 a102 0100  |.|.|.d.f.......
+00002c10: 9001 7170 7c08 6a06 7405 6a1d 6a06 6b02  ..qp|.j.t.j.j.k.
+00002c20: 7270 741b 6a1e 7c0a 6413 6414 8d02 a01f  rpt.j.|.d.d.....
+00002c30: a100 741b 6a20 7c0a 6413 6414 8d02 a01f  ..t.j |.d.d.....
+00002c40: a100 6415 9c02 7d07 7170 7421 7410 6a11  ..d...}.qpt!t.j.
+00002c50: a012 8800 6a13 6416 a102 6417 8302 8f1c  ....j.d...d.....
+00002c60: 7d05 7422 a023 7c07 7c05 a102 0100 5700  }.t".#|.|.....W.
+00002c70: 6400 0400 0400 8303 0100 6e12 3100 9002  d.........n.1...
+00002c80: 731e 3000 0100 0100 0100 5900 0100 6400  s.0.......Y...d.
+00002c90: 5300 2918 4e72 0100 0000 2901 da04 7471  S.).Nr....)...tq
+00002ca0: 646d 6301 0000 0000 0000 0000 0000 0003  dmc.............
+00002cb0: 0000 0007 0000 0013 0000 0073 2e00 0000  ...........s....
+00002cc0: 6900 7c00 5d26 5c02 7d01 7d02 7c01 8800  i.|.]&\.}.}.|...
+00002cd0: 6a00 8800 6a00 7401 6a02 6a03 1900 a004  j...j.t.j.j.....
+00002ce0: 7c02 a101 1900 6a05 9302 7104 5300 7220  |.....j...q.S.r 
+00002cf0: 0000 0029 0672 1000 0000 7204 0000 0072  ...).r....r....r
+00002d00: 2f00 0000 7223 0000 0072 9500 0000 7244  /...r#...r....rD
+00002d10: 0000 0029 0372 2a00 0000 da03 6b65 79da  ...).r*.....key.
+00002d20: 0376 616c 729b 0000 0072 2000 0000 7221  .valr....r ...r!
+00002d30: 0000 0072 7d00 0000 9b01 0000 7304 0000  ...r}.......s...
+00002d40: 0006 0206 ff7a 2e53 7061 7469 616c 4461  .....z.SpatialDa
+00002d50: 7461 7365 742e 7361 7665 5f73 706c 6974  taset.save_split
+00002d60: 732e 3c6c 6f63 616c 733e 2e3c 6469 6374  s.<locals>.<dict
+00002d70: 636f 6d70 3e72 6200 0000 7247 0000 007a  comp>rb...rG...z
+00002d80: 0d53 6176 696e 6720 7370 6c69 7473 2901  .Saving splits).
+00002d90: da04 6465 7363 2eda 0130 da01 3146 724d  ..desc...0..1FrM
+00002da0: 0000 007a 1253 6176 696e 6720 696d 6167  ...z.Saving imag
+00002db0: 6573 2066 6f72 207a 0620 7370 6c69 7429  es for z. split)
+00002dc0: 0272 a000 0000 da05 6c65 6176 65fa 072f  .r......leave../
+00002dd0: 7061 7463 685f fa04 2e6e 7079 2903 7201  patch_...npy).r.
+00002de0: 0000 0072 6500 0000 7202 0000 00a9 01da  ...re...r.......
+00002df0: 0461 7869 7329 0272 9600 0000 da05 7374  .axis).r......st
+00002e00: 6465 767a 196e 6f72 6d61 6c69 7a61 7469  devz.normalizati
+00002e10: 6f6e 5f70 6172 616d 732e 6a73 6f6e 7246  on_params.jsonrF
+00002e20: 0000 0029 2472 9d00 0000 7294 0000 0072  ...)$r....r....r
+00002e30: 5400 0000 7255 0000 0072 0b00 0000 7205  T...rU...r....r.
+00002e40: 0000 0072 2300 0000 7210 0000 00da 0469  ...r#...r......i
+00002e50: 6c6f 6372 6d00 0000 da06 6173 7479 7065  locrm.....astype
+00002e60: 7293 0000 0072 0400 0000 7252 0000 0072  r....r....rR...r
+00002e70: 2f00 0000 7230 0000 0072 1100 0000 7212  /...r0...r....r.
+00002e80: 0000 0072 4e00 0000 720c 0000 0072 5d00  ...rN...r....r].
+00002e90: 0000 da08 6d61 6b65 6469 7273 5a06 746f  ....makedirsZ.to
+00002ea0: 5f63 7376 7207 0000 0072 6c00 0000 7232  _csvr....rl...r2
+00002eb0: 0000 00da 0572 616e 6765 7278 0000 0072  .....rangerx...r
+00002ec0: 4100 0000 727f 0000 0072 9600 0000 da06  A...r....r......
+00002ed0: 746f 6c69 7374 da03 7374 64da 046f 7065  tolist..std..ope
+00002ee0: 6eda 046a 736f 6eda 0464 756d 7029 1272  n..json..dump).r
+00002ef0: 1e00 0000 7287 0000 0072 7e00 0000 729d  ....r....r~...r.
+00002f00: 0000 005a 0b73 706c 6974 5f69 6e64 6578  ...Z.split_index
+00002f10: 725b 0000 00da 0770 6174 6368 6573 5a14  r[.....patchesZ.
+00002f20: 6e6f 726d 616c 697a 6174 696f 6e5f 7061  normalization_pa
+00002f30: 7261 6d73 726a 0000 0072 4400 0000 5a08  ramsrj...rD...Z.
+00002f40: 5f70 6174 6368 6573 5a07 5f6c 6162 656c  _patchesZ._label
+00002f50: 735a 045f 6964 735a 106d 6574 6164 6174  sZ._idsZ.metadat
+00002f60: 615f 746f 5f73 6176 65da 055f 7061 7468  a_to_save.._path
+00002f70: 5a07 6e5f 696d 6167 65da 0169 7242 0000  Z.n_image..irB..
+00002f80: 0072 2000 0000 729b 0000 0072 2100 0000  .r ...r....r!...
+00002f90: 7282 0000 0096 0100 0073 5800 0000 0002  r........sX.....
+00002fa0: 0c03 0a02 06fe 0606 1001 2e03 0401 0201  ................
+00002fb0: 0201 02fe 0c04 0a01 0c01 1801 1601 0a02  ................
+00002fc0: 0601 0201 0601 06fc 02ff 040a 1201 0e01  ................
+00002fd0: 0a01 1401 1403 0401 12ff 0605 0801 0201  ................
+00002fe0: 0601 0c01 02fd 0a06 2202 1804 0e02 1001  ........".......
+00002ff0: 10fe 0806 1801 7a1a 5370 6174 6961 6c44  ......z.SpatialD
+00003000: 6174 6173 6574 2e73 6176 655f 7370 6c69  ataset.save_spli
+00003010: 7473 6302 0000 0000 0000 0000 0000 0004  tsc.............
+00003020: 0000 0004 0000 0003 0000 0073 3400 0000  ...........s4...
+00003030: 7c01 7400 6a01 6a02 1900 6a03 8700 6601  |.t.j.j...j...f.
+00003040: 6401 6402 8408 6403 6404 8d02 7d02 8700  d.d...d.d...}...
+00003050: 6601 6405 6406 8408 7c02 4400 8301 7d03  f.d.d...|.D...}.
+00003060: 7c03 5300 2907 7a4e 0a20 2020 2020 2020  |.S.).zN.       
+00003070: 204c 6f61 6420 616c 6c20 696d 6167 6573   Load all images
+00003080: 2077 6974 6820 7061 7463 685f 6964 7320   with patch_ids 
+00003090: 696e 2074 6865 206c 6973 7420 6672 6f6d  in the list from
+000030a0: 2074 6865 2064 6174 6173 6574 2e0a 2020   the dataset..  
+000030b0: 2020 2020 2020 6301 0000 0000 0000 0000        c.........
+000030c0: 0000 0001 0000 0007 0000 0013 0000 0073  ...............s
+000030d0: 2a00 0000 7400 6a01 a002 8800 6a03 7c00  *...t.j.....j.|.
+000030e0: 8800 6a04 1900 9b00 6401 7c00 7405 6a06  ..j.....d.|.t.j.
+000030f0: 6a07 1900 9b00 6402 9d04 a102 5300 a903  j.....d.....S...
+00003100: 4e72 a400 0000 72a5 0000 0029 0872 1100  Nr....r....).r..
+00003110: 0000 7212 0000 0072 4e00 0000 720c 0000  ..r....rN...r...
+00003120: 0072 7e00 0000 7204 0000 0072 3000 0000  .r~...r....r0...
+00003130: 7223 0000 0029 0172 4300 0000 729b 0000  r#...).rC...r...
+00003140: 0072 2000 0000 7221 0000 00da 083c 6c61  .r ...r!.....<la
+00003150: 6d62 6461 3ee1 0100 0073 0600 0000 0601  mbda>....s......
+00003160: 0401 1cfe 7a33 5370 6174 6961 6c44 6174  ....z3SpatialDat
+00003170: 6173 6574 2e6c 6f61 645f 6672 6f6d 5f6d  aset.load_from_m
+00003180: 6574 6164 6174 612e 3c6c 6f63 616c 733e  etadata.<locals>
+00003190: 2e3c 6c61 6d62 6461 3e72 6500 0000 72a6  .<lambda>re...r.
+000031a0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000031b0: 0200 0000 0600 0000 1300 0000 731a 0000  ............s...
+000031c0: 0067 007c 005d 127d 0188 006a 007c 0164  .g.|.].}...j.|.d
+000031d0: 0064 018d 0291 0271 0453 0029 0246 2901  .d.....q.S.).F).
+000031e0: da02 6964 2901 da11 6c6f 6164 5f73 696e  ..id)...load_sin
+000031f0: 676c 655f 696d 6167 6529 0272 2a00 0000  gle_image).r*...
+00003200: 7212 0000 0072 9b00 0000 7220 0000 0072  r....r....r ...r
+00003210: 2100 0000 722d 0000 00e7 0100 0072 2e00  !...r-.......r..
+00003220: 0000 7a35 5370 6174 6961 6c44 6174 6173  ..z5SpatialDatas
+00003230: 6574 2e6c 6f61 645f 6672 6f6d 5f6d 6574  et.load_from_met
+00003240: 6164 6174 612e 3c6c 6f63 616c 733e 2e3c  adata.<locals>.<
+00003250: 6c69 7374 636f 6d70 3e29 0472 0400 0000  listcomp>).r....
+00003260: 7252 0000 0072 2300 0000 da05 6170 706c  rR...r#.....appl
+00003270: 7929 0472 1e00 0000 7210 0000 005a 0b69  y).r....r....Z.i
+00003280: 6d61 6765 5f70 6174 6873 7247 0000 0072  mage_pathsrG...r
+00003290: 2000 0000 729b 0000 0072 2100 0000 da12   ...r....r!.....
+000032a0: 6c6f 6164 5f66 726f 6d5f 6d65 7461 6461  load_from_metada
+000032b0: 7461 db01 0000 730c 0000 0000 050c 010a  ta....s.........
+000032c0: 0402 fb06 0712 017a 2153 7061 7469 616c  .......z!Spatial
+000032d0: 4461 7461 7365 742e 6c6f 6164 5f66 726f  Dataset.load_fro
+000032e0: 6d5f 6d65 7461 6461 7461 6302 0000 0000  m_metadatac.....
+000032f0: 0000 0000 0000 0003 0000 0007 0000 0043  ...............C
+00003300: 0000 0073 4000 0000 7400 a001 7c00 a101  ...s@...t...|...
+00003310: 7d02 7c01 7238 7c02 7402 7403 6a04 a005  }.|.r8|.t.t.j...
+00003320: 7403 6a04 a006 7c00 a101 a101 6401 1900  t.j...|.....d...
+00003330: a007 6402 a101 6403 1900 8301 6602 5300  ..d...d.....f.S.
+00003340: 7c02 5300 6404 5300 2905 7ae4 0a20 2020  |.S.d.S.).z..   
+00003350: 2020 2020 204c 6f61 6420 6120 7369 6e67       Load a sing
+00003360: 6c65 2069 6d61 6765 2066 726f 6d20 7468  le image from th
+00003370: 6520 6461 7461 7365 742e 0a0a 2020 2020  e dataset...    
+00003380: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00003390: 2020 2020 2020 7061 7468 2028 7374 7229        path (str)
+000033a0: 3a20 5061 7468 2074 6f20 7468 6520 696d  : Path to the im
+000033b0: 6167 6520 6669 6c65 2e0a 2020 2020 2020  age file..      
+000033c0: 2020 2020 2020 6964 2028 626f 6f6c 293a        id (bool):
+000033d0: 2057 6865 7468 6572 2074 6f20 7265 7475   Whether to retu
+000033e0: 726e 2074 6865 2069 6d61 6765 2049 442e  rn the image ID.
+000033f0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00003400: 733a 0a20 2020 2020 2020 2020 2020 206e  s:.            n
+00003410: 702e 6e64 6172 7261 793a 2049 6d61 6765  p.ndarray: Image
+00003420: 2061 7272 6179 2e0a 2020 2020 2020 2020   array..        
+00003430: 7201 0000 00da 015f e9ff ffff ff4e 2908  r......_.....N).
+00003440: 7278 0000 00da 046c 6f61 6472 9300 0000  rx.....loadr....
+00003450: 7211 0000 0072 1200 0000 da08 7370 6c69  r....r......spli
+00003460: 7465 7874 da08 6261 7365 6e61 6d65 7227  text..basenamer'
+00003470: 0000 0029 0372 1200 0000 72b7 0000 00da  ...).r....r.....
+00003480: 0569 6d61 6765 7220 0000 0072 2000 0000  .imager ...r ...
+00003490: 7221 0000 0072 b800 0000 ea01 0000 730c  r!...r........s.
+000034a0: 0000 0000 0c0a 0104 0104 0120 ff06 047a  ........... ...z
+000034b0: 2053 7061 7469 616c 4461 7461 7365 742e   SpatialDataset.
+000034c0: 6c6f 6164 5f73 696e 676c 655f 696d 6167  load_single_imag
+000034d0: 6563 0400 0000 0000 0000 0000 0000 0400  ec..............
+000034e0: 0000 0800 0000 4300 0000 7326 0000 0074  ......C...s&...t
+000034f0: 007c 0283 017d 0274 016a 02a0 037c 006a  .|...}.t.j...|.j
+00003500: 047c 037c 029b 0064 017c 019b 0064 029d  .|.|...d.|...d..
+00003510: 04a1 0353 0072 b500 0000 2905 7293 0000  ...S.r....).r...
+00003520: 0072 1100 0000 7212 0000 0072 4e00 0000  .r....r....rN...
+00003530: 720c 0000 0029 0472 1e00 0000 7252 0000  r....).r....rR..
+00003540: 0072 6c00 0000 7227 0000 0072 2000 0000  .rl...r'...r ...
+00003550: 7220 0000 0072 2100 0000 da13 6765 6e65  r ...r!.....gene
+00003560: 7261 7465 5f70 6174 6368 5f70 6174 68fe  rate_patch_path.
+00003570: 0100 0073 0400 0000 0001 0801 7a22 5370  ...s........z"Sp
+00003580: 6174 6961 6c44 6174 6173 6574 2e67 656e  atialDataset.gen
+00003590: 6572 6174 655f 7061 7463 685f 7061 7468  erate_patch_path
+000035a0: 2901 4e29 014e 2901 4e29 014e 2909 726e  ).N).N).N).N).rn
+000035b0: 0000 0072 6f00 0000 726f 0000 004e 4e54  ...ro...ro...NNT
+000035c0: 4e4e 5429 0272 7400 0000 7289 0000 0029  NNT).rt...r....)
+000035d0: 0572 8f00 0000 5472 4900 0000 7274 0000  .r....TrI...rt..
+000035e0: 0072 8900 0000 2901 5429 22da 085f 5f6e  .r....).T)"..__n
+000035f0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00003600: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00003610: 0373 7472 da04 6c69 7374 7222 0000 0072  .str..listr"...r
+00003620: 1d00 0000 7239 0000 0072 6600 0000 7216  ....r9...rf...r.
+00003630: 0000 0072 1500 0000 7293 0000 00da 0462  ...r....r......b
+00003640: 6f6f 6c72 5c00 0000 7217 0000 0072 1800  oolr\...r....r..
+00003650: 0000 7219 0000 0072 1a00 0000 721c 0000  ..r....r....r...
+00003660: 0072 1b00 0000 7225 0000 00da 0566 6c6f  .r....r%.....flo
+00003670: 6174 7288 0000 00da 0c73 7461 7469 636d  atr......staticm
+00003680: 6574 686f 6472 8e00 0000 7281 0000 0072  ethodr....r....r
+00003690: 9c00 0000 7204 0000 005a 0c63 6f6e 7461  ....r....Z.conta
+000036a0: 696e 735f 6364 3872 2300 0000 7282 0000  ins_cd8r#...r...
+000036b0: 0072 ba00 0000 72b8 0000 0072 c100 0000  .r....r....r....
+000036c0: 7220 0000 0072 2000 0000 7220 0000 0072  r ...r ...r ...r
+000036d0: 2100 0000 7208 0000 0012 0000 0073 8400  !...r........s..
+000036e0: 0000 0804 0201 0201 0201 0201 02f9 0202  ................
+000036f0: 0201 0201 0201 0201 0201 02f9 0c1f 0806  ................
+00003700: 121c 0806 0201 0201 0201 0201 0201 02f9  ................
+00003710: 0202 0201 0201 0201 0201 0201 02f9 0c5a  ...............Z
+00003720: 1008 1008 1008 1008 0812 0810 0e0c 0001  ................
+00003730: 0001 0001 0001 0001 0001 0001 0001 00f5  ................
+00003740: 0202 0201 0201 0201 02fb 0c56 0201 0c10  ...........V....
+00003750: 0001 0001 0001 0001 00f6 0a35 0803 1045  ...........5...E
+00003760: 080f 0201 0c13 7208 0000 0029 1072 b000  ......r....).r..
+00003770: 0000 7211 0000 0072 3500 0000 7254 0000  ..r....r5...rT..
+00003780: 00da 056e 756d 7079 7278 0000 00da 0670  ...numpyrx.....p
+00003790: 616e 6461 7372 3900 0000 5a0e 7574 696c  andasr9...Z.util
+000037a0: 732e 7061 7463 6869 6679 7203 0000 005a  s.patchifyr....Z
+000037b0: 1363 6f6e 6669 6775 7261 7469 6f6e 2e54  .configuration.T
+000037c0: 7970 6573 7204 0000 0072 0500 0000 7206  ypesr....r....r.
+000037d0: 0000 0072 0700 0000 7208 0000 0072 2000  ...r....r....r .
+000037e0: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
+000037f0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00003800: 1000 0000 0801 0801 0802 0801 0801 0802  ................
+00003810: 0c01 1808                                ....
```

### Comparing `morpheus_spatial-0.4.0/src/morpheus/datasets/__pycache__/torch_dataset.cpython-39.pyc` & `morpheus_spatial-0.5.0/src/morpheus/datasets/__pycache__/torch_dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Mar 24 19:57:49 2024 UTC, .py size: 3360 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 bd85 0066 200d 0000  a..........f ...
+00000000: 610d 0d0a 0000 0000 2cb8 1166 200d 0000  a.......,..f ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c06 5a06 6400 6402 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6400 6403 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6404 6405 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
```

### Comparing `morpheus_spatial-0.4.0/src/morpheus/datasets/spatial_dataset.py` & `morpheus_spatial-0.5.0/src/morpheus/datasets/spatial_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,28 +15,25 @@
 )
 
 
 class SpatialDataset:
     def __init__(
         self,
         input_path: str,
-        channel_names: list,
+        channel_names: list = [],
         patch_path: str = None,
         split_dir: str = None,
         model_dir: str = None,
         cf_dir: str = None,
     ):
         self.data_dim = None
         self.metadata = None
         self.input_path = input_path
         self.root_dir = os.path.dirname(input_path)
 
-        if len(channel_names) == 0:
-            raise ValueError("Channel names must be provided")
-
         data = self.load_input_csv()
         self.check_input_csv(data, channel_names)  # also sets self.channel_names
 
         # set the directories where different outputs are saved
         self.patch_path = self.set_patch_path(patch_path)
         self.split_dir = self.set_split_dir(split_dir)
         self.model_dir = self.set_model_dir(model_dir)
@@ -60,32 +57,36 @@
         # check the input CSV contains the required columns
         required_cols = [
             ColName.patient_id.value,
             ColName.image_id.value,
             ColName.cell_type.value,
             ColName.cell_x.value,
             ColName.cell_y.value,
-        ] + channel_names
+        ]
+        if len(channel_names) == 0:
+            channel_names = [
+                col for col in input_csv.columns if col not in required_cols
+            ]
+            print(f"Channel names inferred from input CSV: {channel_names}")
+        required_cols += channel_names
+
         for col in required_cols:
             if col not in input_csv.columns:
                 warnings.warn("input csv does not contain required column: {col}")
 
         # reorder the channel names to match the order in the input CSV
         self.channel_names = [col for col in input_csv.columns if col in channel_names]
 
         # check that the input CSV is not empty
         if input_csv.empty:
             raise ValueError("Input CSV is empty")
         return
 
     def load_input_csv(self):
-        try:
-            data = pd.read_csv(self.input_path)
-        except Exception as e:
-            print(f"Error loading input CSV: {e}")
+        data = pd.read_csv(self.input_path)
         return data
 
     def generate_masked_patch(
         self,
         cell_to_mask: list = [],
         patch_size: int = 16,
         pixel_size: int = 3,
@@ -320,15 +321,17 @@
                 test_size,
                 random_state,
                 shuffle,
                 **tolerance,
             )
 
         if patient_split is None:
-            raise ValueError("Could not satisfy data split constraints, try again or adjust constraints")
+            raise ValueError(
+                "Could not satisfy data split constraints, try again or adjust constraints"
+            )
 
         if save:
             print("Saving splits...")
             self.save_splits(patient_split, label_name=stratify_by)
             print(f"Data splits saved to {self.split_dir}")
             self.get_split_info()
         return patient_split
```

### Comparing `morpheus_spatial-0.4.0/src/morpheus/datasets/torch_dataset.py` & `morpheus_spatial-0.5.0/src/morpheus/datasets/torch_dataset.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.4.0/src/morpheus/utils/__pycache__/saving.cpython-39.pyc` & `morpheus_spatial-0.5.0/src/morpheus/utils/__pycache__/saving.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.4.0/src/morpheus/utils/gradients.py` & `morpheus_spatial-0.5.0/src/morpheus/utils/gradients.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.4.0/src/morpheus/utils/patchify.py` & `morpheus_spatial-0.5.0/src/morpheus/utils/patchify.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.4.0/src/morpheus/utils/saving.py` & `morpheus_spatial-0.5.0/src/morpheus/utils/saving.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.4.0/PKG-INFO` & `morpheus_spatial-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: morpheus-spatial
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: neonine2
 Author-email: jerry.wang95@yahoo.ca
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.9.4)
 Requires-Dist: dill (>=0.3.8,<0.4.0)
 Requires-Dist: h5py (>=3.10.0,<4.0.0)
+Requires-Dist: idna (>=3.7)
 Requires-Dist: lightning (>=2.0.0,<3.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: pillow (>=10.3.0)
+Requires-Dist: ray (>=2.11.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
-Requires-Dist: tensorflow (==2.11.1)
 Requires-Dist: torch (==2.0.0)
 Requires-Dist: torchvision (>=0.15.1,<0.16.0)
 Description-Content-Type: text/markdown
 
 # Morpheus: Generating Therapeutic Strategies using Spatial Omics
 
 ## Introduction
```

