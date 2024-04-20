# Comparing `tmp/mfs-styletts2-1.0.0.tar.gz` & `tmp/mfs-styletts2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfs-styletts2-1.0.0.tar", last modified: Sat Apr 20 01:53:48 2024, max compression
+gzip compressed data, was "mfs-styletts2-1.0.1.tar", last modified: Sat Apr 20 02:10:55 2024, max compression
```

## Comparing `mfs-styletts2-1.0.0.tar` & `mfs-styletts2-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 01:53:48.488398 mfs-styletts2-1.0.0/
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1094 2024-04-20 01:53:41.000000 mfs-styletts2-1.0.0/LICENSE
--rw-r--r--   0 benjaminlee   (501) staff       (20)      868 2024-04-20 01:53:48.487928 mfs-styletts2-1.0.0/PKG-INFO
--rw-r--r--   0 benjaminlee   (501) staff       (20)      128 2024-04-20 01:33:03.000000 mfs-styletts2-1.0.0/README.md
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 01:53:48.478973 mfs-styletts2-1.0.0/mfs_styletts2/
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 01:53:48.482826 mfs-styletts2-1.0.0/mfs_styletts2/Modules/
--rw-rw-r--   0 benjaminlee   (501) staff       (20)        1 2024-03-26 18:30:47.000000 mfs-styletts2-1.0.0/mfs_styletts2/Modules/__init__.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 01:53:48.484247 mfs-styletts2-1.0.0/mfs_styletts2/Modules/diffusion/
--rw-rw-r--   0 benjaminlee   (501) staff       (20)        1 2024-03-26 18:30:47.000000 mfs-styletts2-1.0.0/mfs_styletts2/Modules/diffusion/__init__.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)     2628 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.0/mfs_styletts2/Modules/diffusion/diffusion.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)    24280 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.0/mfs_styletts2/Modules/diffusion/modules.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)    22505 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.0/mfs_styletts2/Modules/diffusion/sampler.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)     2328 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.0/mfs_styletts2/Modules/diffusion/utils.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)     8136 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.0/mfs_styletts2/Modules/discriminators.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)    21831 2024-04-20 01:47:33.000000 mfs-styletts2-1.0.0/mfs_styletts2/Modules/hifigan.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)    24595 2024-04-20 01:47:35.000000 mfs-styletts2-1.0.0/mfs_styletts2/Modules/istftnet.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)     8494 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.0/mfs_styletts2/Modules/slmadv.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)      381 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.0/mfs_styletts2/Modules/utils.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 01:53:48.484974 mfs-styletts2-1.0.0/mfs_styletts2/Utils/
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 01:53:48.485806 mfs-styletts2-1.0.0/mfs_styletts2/Utils/ASR/
--rw-rw-r--   0 benjaminlee   (501) staff       (20)        1 2024-03-26 18:30:47.000000 mfs-styletts2-1.0.0/mfs_styletts2/Utils/ASR/__init__.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)    13890 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.0/mfs_styletts2/Utils/ASR/layers.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)     7594 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.0/mfs_styletts2/Utils/ASR/models.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 01:53:48.487185 mfs-styletts2-1.0.0/mfs_styletts2/Utils/JDC/
--rw-rw-r--   0 benjaminlee   (501) staff       (20)        1 2024-03-26 18:30:47.000000 mfs-styletts2-1.0.0/mfs_styletts2/Utils/JDC/__init__.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)     7765 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.0/mfs_styletts2/Utils/JDC/model.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)        1 2024-03-26 18:30:47.000000 mfs-styletts2-1.0.0/mfs_styletts2/Utils/__init__.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)        0 2024-04-20 01:50:41.000000 mfs-styletts2-1.0.0/mfs_styletts2/__init__.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     7919 2024-04-20 01:52:55.000000 mfs-styletts2-1.0.0/mfs_styletts2/lj.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)    27471 2024-04-20 01:47:19.000000 mfs-styletts2-1.0.0/mfs_styletts2/models.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)      931 2024-04-20 01:47:25.000000 mfs-styletts2-1.0.0/mfs_styletts2/text_utils.py
--rw-rw-r--   0 benjaminlee   (501) staff       (20)     1506 2024-04-20 01:52:55.000000 mfs-styletts2-1.0.0/mfs_styletts2/utils.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)    12733 2024-04-20 01:52:57.000000 mfs-styletts2-1.0.0/mfs_styletts2/zeroshot.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 01:53:48.480686 mfs-styletts2-1.0.0/mfs_styletts2.egg-info/
--rw-r--r--   0 benjaminlee   (501) staff       (20)      868 2024-04-20 01:53:48.000000 mfs-styletts2-1.0.0/mfs_styletts2.egg-info/PKG-INFO
--rw-r--r--   0 benjaminlee   (501) staff       (20)      982 2024-04-20 01:53:48.000000 mfs-styletts2-1.0.0/mfs_styletts2.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)        1 2024-04-20 01:53:48.000000 mfs-styletts2-1.0.0/mfs_styletts2.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)      192 2024-04-20 01:53:48.000000 mfs-styletts2-1.0.0/mfs_styletts2.egg-info/requires.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)       14 2024-04-20 01:53:48.000000 mfs-styletts2-1.0.0/mfs_styletts2.egg-info/top_level.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)       38 2024-04-20 01:53:48.488489 mfs-styletts2-1.0.0/setup.cfg
--rw-r--r--   0 benjaminlee   (501) staff       (20)      856 2024-04-20 01:35:14.000000 mfs-styletts2-1.0.0/setup.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 02:10:55.985586 mfs-styletts2-1.0.1/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1094 2024-04-20 01:53:41.000000 mfs-styletts2-1.0.1/LICENSE
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      868 2024-04-20 02:10:55.985175 mfs-styletts2-1.0.1/PKG-INFO
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      128 2024-04-20 01:33:03.000000 mfs-styletts2-1.0.1/README.md
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 02:10:55.979527 mfs-styletts2-1.0.1/mfs_styletts2/
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 02:10:55.981932 mfs-styletts2-1.0.1/mfs_styletts2/Modules/
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)        1 2024-03-26 18:30:47.000000 mfs-styletts2-1.0.1/mfs_styletts2/Modules/__init__.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 02:10:55.983392 mfs-styletts2-1.0.1/mfs_styletts2/Modules/diffusion/
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)        1 2024-03-26 18:30:47.000000 mfs-styletts2-1.0.1/mfs_styletts2/Modules/diffusion/__init__.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)     2628 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.1/mfs_styletts2/Modules/diffusion/diffusion.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)    24280 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.1/mfs_styletts2/Modules/diffusion/modules.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)    22505 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.1/mfs_styletts2/Modules/diffusion/sampler.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)     2328 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.1/mfs_styletts2/Modules/diffusion/utils.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)     8136 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.1/mfs_styletts2/Modules/discriminators.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)    21831 2024-04-20 01:47:33.000000 mfs-styletts2-1.0.1/mfs_styletts2/Modules/hifigan.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)    24595 2024-04-20 01:47:35.000000 mfs-styletts2-1.0.1/mfs_styletts2/Modules/istftnet.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)     8494 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.1/mfs_styletts2/Modules/slmadv.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)      381 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.1/mfs_styletts2/Modules/utils.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 02:10:55.983613 mfs-styletts2-1.0.1/mfs_styletts2/Utils/
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 02:10:55.984248 mfs-styletts2-1.0.1/mfs_styletts2/Utils/ASR/
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)        1 2024-03-26 18:30:47.000000 mfs-styletts2-1.0.1/mfs_styletts2/Utils/ASR/__init__.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)    13890 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.1/mfs_styletts2/Utils/ASR/layers.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)     7594 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.1/mfs_styletts2/Utils/ASR/models.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 02:10:55.984716 mfs-styletts2-1.0.1/mfs_styletts2/Utils/JDC/
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)        1 2024-03-26 18:30:47.000000 mfs-styletts2-1.0.1/mfs_styletts2/Utils/JDC/__init__.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)     7765 2024-04-20 01:24:25.000000 mfs-styletts2-1.0.1/mfs_styletts2/Utils/JDC/model.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)        1 2024-03-26 18:30:47.000000 mfs-styletts2-1.0.1/mfs_styletts2/Utils/__init__.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)        0 2024-04-20 01:50:41.000000 mfs-styletts2-1.0.1/mfs_styletts2/__init__.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     7871 2024-04-20 02:09:59.000000 mfs-styletts2-1.0.1/mfs_styletts2/lj.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)    27471 2024-04-20 01:47:19.000000 mfs-styletts2-1.0.1/mfs_styletts2/models.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)      931 2024-04-20 01:47:25.000000 mfs-styletts2-1.0.1/mfs_styletts2/text_utils.py
+-rw-rw-r--   0 benjaminlee   (501) staff       (20)     1506 2024-04-20 01:52:55.000000 mfs-styletts2-1.0.1/mfs_styletts2/utils.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)    12759 2024-04-20 02:10:36.000000 mfs-styletts2-1.0.1/mfs_styletts2/zeroshot.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 02:10:55.980535 mfs-styletts2-1.0.1/mfs_styletts2.egg-info/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      868 2024-04-20 02:10:55.000000 mfs-styletts2-1.0.1/mfs_styletts2.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      982 2024-04-20 02:10:55.000000 mfs-styletts2-1.0.1/mfs_styletts2.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)        1 2024-04-20 02:10:55.000000 mfs-styletts2-1.0.1/mfs_styletts2.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      192 2024-04-20 02:10:55.000000 mfs-styletts2-1.0.1/mfs_styletts2.egg-info/requires.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       14 2024-04-20 02:10:55.000000 mfs-styletts2-1.0.1/mfs_styletts2.egg-info/top_level.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       38 2024-04-20 02:10:55.985721 mfs-styletts2-1.0.1/setup.cfg
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      856 2024-04-20 02:07:23.000000 mfs-styletts2-1.0.1/setup.py
```

### Comparing `mfs-styletts2-1.0.0/LICENSE` & `mfs-styletts2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/PKG-INFO` & `mfs-styletts2-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfs-styletts2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial pip package for StyleTTS 2
 Home-page: https://github.com/ml-for-speech/mfs-styletts2
 Author: ML for Speech
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: SoundFile
 Requires-Dist: torchaudio
```

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/Modules/diffusion/diffusion.py` & `mfs-styletts2-1.0.1/mfs_styletts2/Modules/diffusion/diffusion.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/Modules/diffusion/modules.py` & `mfs-styletts2-1.0.1/mfs_styletts2/Modules/diffusion/modules.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/Modules/diffusion/sampler.py` & `mfs-styletts2-1.0.1/mfs_styletts2/Modules/diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/Modules/diffusion/utils.py` & `mfs-styletts2-1.0.1/mfs_styletts2/Modules/diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/Modules/discriminators.py` & `mfs-styletts2-1.0.1/mfs_styletts2/Modules/discriminators.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/Modules/hifigan.py` & `mfs-styletts2-1.0.1/mfs_styletts2/Modules/hifigan.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/Modules/istftnet.py` & `mfs-styletts2-1.0.1/mfs_styletts2/Modules/istftnet.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/Modules/slmadv.py` & `mfs-styletts2-1.0.1/mfs_styletts2/Modules/slmadv.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/Utils/ASR/layers.py` & `mfs-styletts2-1.0.1/mfs_styletts2/Utils/ASR/layers.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/Utils/ASR/models.py` & `mfs-styletts2-1.0.1/mfs_styletts2/Utils/ASR/models.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/Utils/JDC/model.py` & `mfs-styletts2-1.0.1/mfs_styletts2/Utils/JDC/model.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/lj.py` & `mfs-styletts2-1.0.1/mfs_styletts2/lj.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,41 +80,29 @@
 
 # load phonemizer
 from openphonemizer import OpenPhonemizer
 
 phonemizer = OpenPhonemizer()
 
 
-config = yaml.safe_load(
-    open(str(cached_path("hf://yl4579/StyleTTS2-LJSpeech/Models/LJSpeech/config.yml")))
-)
-
-paths_to_replace = [
-    "ASR_config",
-    "ASR_path",
-    "F0_path",
-]
-
-for i in paths_to_replace:
-    config[i] = os.path.join(os.path.dirname(__file__), config[i])
+config = yaml.safe_load(open(str(cached_path('hf://yl4579/StyleTTS2-LJSpeech/Models/LJSpeech/config.yml'))))
 
 # load pretrained ASR model
-ASR_config = config.get("ASR_config", False)
-ASR_path = config.get("ASR_path", False)
+ASR_config = str(cached_path('https://raw.githubusercontent.com/yl4579/StyleTTS2/main/Utils/ASR/config.yml'))
+ASR_path = str(cached_path('https://github.com/yl4579/StyleTTS2/raw/main/Utils/ASR/epoch_00080.pth'))
 text_aligner = load_ASR_models(ASR_path, ASR_config)
 
 # load pretrained F0 model
-F0_path = config.get("F0_path", False)
+F0_path = str(cached_path('https://github.com/yl4579/StyleTTS2/raw/main/Utils/JDC/bst.t7'))
 pitch_extractor = load_F0_models(F0_path)
 
 # load BERT model
 from .Utils.PLBERT.util import load_plbert
 
-BERT_path = config.get("PLBERT_dir", False)
-plbert = load_plbert(BERT_path)
+plbert = load_plbert()
 
 model = build_model(
     recursive_munch(config["model_params"]), text_aligner, pitch_extractor, plbert
 )
 _ = [model[key].eval() for key in model]
 _ = [model[key].to(device) for key in model]
```

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/models.py` & `mfs-styletts2-1.0.1/mfs_styletts2/models.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/text_utils.py` & `mfs-styletts2-1.0.1/mfs_styletts2/text_utils.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/utils.py` & `mfs-styletts2-1.0.1/mfs_styletts2/utils.py`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2/zeroshot.py` & `mfs-styletts2-1.0.1/mfs_styletts2/zeroshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,33 +85,29 @@
 from openphonemizer import OpenPhonemizer
 
 phonemizer = OpenPhonemizer()
 
 # phonemizer = Phonemizer.from_checkpoint(str(cached_path('https://public-asai-dl-models.s3.eu-central-1.amazonaws.com/DeepPhonemizer/en_us_cmudict_ipa_forward.pt')))
 
 
-# config = yaml.safe_load(open("Models/LibriTTS/config.yml"))
-config = yaml.safe_load(
-    open(str(cached_path("hf://yl4579/StyleTTS2-LibriTTS/Models/LibriTTS/config.yml")))
-)
+config = yaml.safe_load(open(str(cached_path('hf://yl4579/StyleTTS2-LibriTTS/Models/LibriTTS/config.yml'))))
 
 # load pretrained ASR model
-ASR_config = config.get("ASR_config", False)
-ASR_path = config.get("ASR_path", False)
+ASR_config = str(cached_path('https://raw.githubusercontent.com/yl4579/StyleTTS2/main/Utils/ASR/config.yml'))
+ASR_path = str(cached_path('https://github.com/yl4579/StyleTTS2/raw/main/Utils/ASR/epoch_00080.pth'))
 text_aligner = load_ASR_models(ASR_path, ASR_config)
 
 # load pretrained F0 model
-F0_path = config.get("F0_path", False)
+F0_path = str(cached_path('https://github.com/yl4579/StyleTTS2/raw/main/Utils/JDC/bst.t7'))
 pitch_extractor = load_F0_models(F0_path)
 
 # load BERT model
-from Utils.PLBERT.util import load_plbert
+from .Utils.PLBERT.util import load_plbert
 
-BERT_path = config.get("PLBERT_dir", False)
-plbert = load_plbert(BERT_path)
+plbert = load_plbert()
 
 model_params = recursive_munch(config["model_params"])
 model = build_model(model_params, text_aligner, pitch_extractor, plbert)
 _ = [model[key].eval() for key in model]
 _ = [model[key].to(device) for key in model]
 
 # params_whole = torch.load("Models/LibriTTS/epochs_2nd_00020.pth", map_location='cpu')
@@ -123,15 +119,14 @@
     ),
     map_location="cpu",
 )
 params = params_whole["net"]
 
 for key in model:
     if key in params:
-        print("%s loaded" % key)
         try:
             model[key].load_state_dict(params[key])
         except:
             from collections import OrderedDict
 
             state_dict = params[key]
             new_state_dict = OrderedDict()
```

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2.egg-info/PKG-INFO` & `mfs-styletts2-1.0.1/mfs_styletts2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfs-styletts2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial pip package for StyleTTS 2
 Home-page: https://github.com/ml-for-speech/mfs-styletts2
 Author: ML for Speech
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: SoundFile
 Requires-Dist: torchaudio
```

### Comparing `mfs-styletts2-1.0.0/mfs_styletts2.egg-info/SOURCES.txt` & `mfs-styletts2-1.0.1/mfs_styletts2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mfs-styletts2-1.0.0/setup.py` & `mfs-styletts2-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     longdesc = f.read()
 setup(
     name="mfs-styletts2",
-    version="1.0.0",
+    version="1.0.1",
     author="ML for Speech",
     description="Unofficial pip package for StyleTTS 2",
     long_description=longdesc,
     long_description_content_type="text/markdown",
     url="https://github.com/ml-for-speech/mfs-styletts2",
     packages=find_packages(),
     install_requires=[
```

