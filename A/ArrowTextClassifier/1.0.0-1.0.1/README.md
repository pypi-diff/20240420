# Comparing `tmp/ArrowTextClassifier-1.0.0.tar.gz` & `tmp/ArrowTextClassifier-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ArrowTextClassifier-1.0.0.tar", last modified: Sat Apr 20 13:12:29 2024, max compression
+gzip compressed data, was "ArrowTextClassifier-1.0.1.tar", last modified: Sat Apr 20 13:39:17 2024, max compression
```

## Comparing `ArrowTextClassifier-1.0.0.tar` & `ArrowTextClassifier-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 13:12:29.062757 ArrowTextClassifier-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-04-20 13:12:29.028158 ArrowTextClassifier-1.0.0/ArrowTextClassifier.egg-info/
--rw-rw-rw-   0        0        0     3839 2024-04-20 13:12:28.000000 ArrowTextClassifier-1.0.0/ArrowTextClassifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-04-20 13:12:28.000000 ArrowTextClassifier-1.0.0/ArrowTextClassifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 13:12:28.000000 ArrowTextClassifier-1.0.0/ArrowTextClassifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-04-20 13:12:28.000000 ArrowTextClassifier-1.0.0/ArrowTextClassifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-20 13:12:28.000000 ArrowTextClassifier-1.0.0/ArrowTextClassifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2024-04-15 12:47:46.000000 ArrowTextClassifier-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3839 2024-04-20 13:12:29.056937 ArrowTextClassifier-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2437 2024-04-20 13:09:12.000000 ArrowTextClassifier-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-20 13:12:29.063336 ArrowTextClassifier-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1783 2024-04-20 12:47:09.000000 ArrowTextClassifier-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 13:12:29.053889 ArrowTextClassifier-1.0.0/src/
--rw-rw-rw-   0        0        0      307 2024-04-20 13:01:37.000000 ArrowTextClassifier-1.0.0/src/__init__.py
--rw-rw-rw-   0        0        0     2505 2024-04-20 12:36:05.000000 ArrowTextClassifier-1.0.0/src/classify_text.py
--rw-rw-rw-   0        0        0     1772 2024-04-20 13:01:26.000000 ArrowTextClassifier-1.0.0/src/main.py
--rw-rw-rw-   0        0        0     1317 2024-04-15 12:53:00.000000 ArrowTextClassifier-1.0.0/src/model.py
--rw-rw-rw-   0        0        0     1628 2024-04-20 10:43:28.000000 ArrowTextClassifier-1.0.0/src/summarize_model.py
--rw-rw-rw-   0        0        0      718 2024-04-15 12:53:00.000000 ArrowTextClassifier-1.0.0/src/tokenizer.py
--rw-rw-rw-   0        0        0     6955 2024-04-20 11:33:27.000000 ArrowTextClassifier-1.0.0/src/train.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:39:17.136318 ArrowTextClassifier-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:39:17.108240 ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/
+-rw-rw-rw-   0        0        0     3835 2024-04-20 13:39:16.000000 ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-04-20 13:39:17.000000 ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 13:39:16.000000 ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-04-20 13:39:16.000000 ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-20 13:39:16.000000 ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2024-04-15 12:47:46.000000 ArrowTextClassifier-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3835 2024-04-20 13:39:17.134753 ArrowTextClassifier-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2623 2024-04-20 13:28:04.000000 ArrowTextClassifier-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 13:39:17.136318 ArrowTextClassifier-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1783 2024-04-20 13:33:59.000000 ArrowTextClassifier-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:39:17.131500 ArrowTextClassifier-1.0.1/src/
+-rw-rw-rw-   0        0        0      307 2024-04-20 13:01:37.000000 ArrowTextClassifier-1.0.1/src/__init__.py
+-rw-rw-rw-   0        0        0     2505 2024-04-20 12:36:05.000000 ArrowTextClassifier-1.0.1/src/classify_text.py
+-rw-rw-rw-   0        0        0     1772 2024-04-20 13:01:26.000000 ArrowTextClassifier-1.0.1/src/main.py
+-rw-rw-rw-   0        0        0     1317 2024-04-15 12:53:00.000000 ArrowTextClassifier-1.0.1/src/model.py
+-rw-rw-rw-   0        0        0     1628 2024-04-20 10:43:28.000000 ArrowTextClassifier-1.0.1/src/summarize_model.py
+-rw-rw-rw-   0        0        0      718 2024-04-15 12:53:00.000000 ArrowTextClassifier-1.0.1/src/tokenizer.py
+-rw-rw-rw-   0        0        0     6955 2024-04-20 11:33:27.000000 ArrowTextClassifier-1.0.1/src/train.py
```

### Comparing `ArrowTextClassifier-1.0.0/ArrowTextClassifier.egg-info/PKG-INFO` & `ArrowTextClassifier-1.0.1/ArrowTextClassifier.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArrowTextClassifier
-Version: 1.0.0
+Version: 1.0.1
 Summary: ArrowTextClassifier is a simple text classification tool written in pytorch that allows you to train, summarize, and use text classification models for various tasks.
 Home-page: https://github.com/Bhargav230m/ArrowTextClassifier.git
 Author: techpowerb
 Author-email: technologypower24@gmail.com
 Keywords: text classification,natural language processing,NLP,PyTorch,machine learning,deep learning,text summarization,preprocessing,data science,artificial intelligence,dataset,discord
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -16,22 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch==2.2.2
-Requires-Dist: torchsummary==1.4.5
-Requires-Dist: pandas==2.2.2
-Requires-Dist: scikit-learn==1.4.2
-Requires-Dist: tqdm==4.66.2
-Requires-Dist: numpy==1.26.4
 
-```markdown
 # ArrowTextClassifier
 
 ArrowTextClassifier is a Python package for text classification tasks, offering functionalities to train, summarize, and classify text using convolutional neural network (CNN) architecture.
 
 ## Installation
 
 You can install ArrowTextClassifier via pip:
@@ -96,15 +89,15 @@
     vocabulary_path="path_to_vocabulary_file"
 )
 print(result)
 ```
 
 ## Getting Started
 
-This package provides tools for text classification tasks. You can explore and customize it according to your requirements. Refer to the documentation for detailed usage instructions.
+This package provides tools for text classification tasks. You can explore and customize it according to your requirements. Refer to the documentation for detailed usage instructions. We have also made our own colab [notebook](https://colab.research.google.com/drive/1fGDLICkctfdpTgLoh_Bouv-NY-q-kdlQ?usp=sharing) to help you train a custom offensive language classifier using this.
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ---
```

### Comparing `ArrowTextClassifier-1.0.0/LICENSE` & `ArrowTextClassifier-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ArrowTextClassifier-1.0.0/PKG-INFO` & `ArrowTextClassifier-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArrowTextClassifier
-Version: 1.0.0
+Version: 1.0.1
 Summary: ArrowTextClassifier is a simple text classification tool written in pytorch that allows you to train, summarize, and use text classification models for various tasks.
 Home-page: https://github.com/Bhargav230m/ArrowTextClassifier.git
 Author: techpowerb
 Author-email: technologypower24@gmail.com
 Keywords: text classification,natural language processing,NLP,PyTorch,machine learning,deep learning,text summarization,preprocessing,data science,artificial intelligence,dataset,discord
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -16,22 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch==2.2.2
-Requires-Dist: torchsummary==1.4.5
-Requires-Dist: pandas==2.2.2
-Requires-Dist: scikit-learn==1.4.2
-Requires-Dist: tqdm==4.66.2
-Requires-Dist: numpy==1.26.4
 
-```markdown
 # ArrowTextClassifier
 
 ArrowTextClassifier is a Python package for text classification tasks, offering functionalities to train, summarize, and classify text using convolutional neural network (CNN) architecture.
 
 ## Installation
 
 You can install ArrowTextClassifier via pip:
@@ -96,15 +89,15 @@
     vocabulary_path="path_to_vocabulary_file"
 )
 print(result)
 ```
 
 ## Getting Started
 
-This package provides tools for text classification tasks. You can explore and customize it according to your requirements. Refer to the documentation for detailed usage instructions.
+This package provides tools for text classification tasks. You can explore and customize it according to your requirements. Refer to the documentation for detailed usage instructions. We have also made our own colab [notebook](https://colab.research.google.com/drive/1fGDLICkctfdpTgLoh_Bouv-NY-q-kdlQ?usp=sharing) to help you train a custom offensive language classifier using this.
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ---
```

### Comparing `ArrowTextClassifier-1.0.0/README.md` & `ArrowTextClassifier-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,153 +1,164 @@
-00000000: 6060 606d 6172 6b64 6f77 6e0d 0a23 2041  ```markdown..# A
-00000010: 7272 6f77 5465 7874 436c 6173 7369 6669  rrowTextClassifi
-00000020: 6572 0d0a 0d0a 4172 726f 7754 6578 7443  er....ArrowTextC
-00000030: 6c61 7373 6966 6965 7220 6973 2061 2050  lassifier is a P
-00000040: 7974 686f 6e20 7061 636b 6167 6520 666f  ython package fo
-00000050: 7220 7465 7874 2063 6c61 7373 6966 6963  r text classific
-00000060: 6174 696f 6e20 7461 736b 732c 206f 6666  ation tasks, off
-00000070: 6572 696e 6720 6675 6e63 7469 6f6e 616c  ering functional
-00000080: 6974 6965 7320 746f 2074 7261 696e 2c20  ities to train, 
-00000090: 7375 6d6d 6172 697a 652c 2061 6e64 2063  summarize, and c
-000000a0: 6c61 7373 6966 7920 7465 7874 2075 7369  lassify text usi
-000000b0: 6e67 2063 6f6e 766f 6c75 7469 6f6e 616c  ng convolutional
-000000c0: 206e 6575 7261 6c20 6e65 7477 6f72 6b20   neural network 
-000000d0: 2843 4e4e 2920 6172 6368 6974 6563 7475  (CNN) architectu
-000000e0: 7265 2e0d 0a0d 0a23 2320 496e 7374 616c  re.....## Instal
-000000f0: 6c61 7469 6f6e 0d0a 0d0a 596f 7520 6361  lation....You ca
-00000100: 6e20 696e 7374 616c 6c20 4172 726f 7754  n install ArrowT
-00000110: 6578 7443 6c61 7373 6966 6965 7220 7669  extClassifier vi
-00000120: 6120 7069 703a 0d0a 0d0a 6060 6062 6173  a pip:....```bas
-00000130: 680d 0a70 6970 2069 6e73 7461 6c6c 2041  h..pip install A
-00000140: 7272 6f77 5465 7874 436c 6173 7369 6669  rrowTextClassifi
-00000150: 6572 0d0a 6060 600d 0a0d 0a23 2320 486f  er..```....## Ho
-00000160: 7720 6974 2057 6f72 6b73 0d0a 0d0a 4172  w it Works....Ar
-00000170: 726f 7754 6578 7443 6c61 7373 6966 6965  rowTextClassifie
-00000180: 7220 696d 706c 656d 656e 7473 2061 2063  r implements a c
-00000190: 6f6e 766f 6c75 7469 6f6e 616c 206e 6575  onvolutional neu
-000001a0: 7261 6c20 6e65 7477 6f72 6b20 2843 4e4e  ral network (CNN
-000001b0: 2920 6172 6368 6974 6563 7475 7265 2066  ) architecture f
-000001c0: 6f72 2074 6578 7420 636c 6173 7369 6669  or text classifi
-000001d0: 6361 7469 6f6e 2e20 4974 2074 6f6b 656e  cation. It token
-000001e0: 697a 6573 2069 6e70 7574 2074 6578 742c  izes input text,
-000001f0: 2065 6d62 6564 7320 7468 6520 746f 6b65   embeds the toke
-00000200: 6e73 2c20 6170 706c 6965 7320 636f 6e76  ns, applies conv
-00000210: 6f6c 7574 696f 6e61 6c20 6669 6c74 6572  olutional filter
-00000220: 7320 6f76 6572 2074 6865 2065 6d62 6564  s over the embed
-00000230: 6465 6420 746f 6b65 6e73 2074 6f20 6578  ded tokens to ex
-00000240: 7472 6163 7420 6665 6174 7572 6573 2c20  tract features, 
-00000250: 616e 6420 7468 656e 2063 6c61 7373 6966  and then classif
-00000260: 6965 7320 7468 6520 7465 7874 2069 6e74  ies the text int
-00000270: 6f20 7072 6564 6566 696e 6564 2063 6174  o predefined cat
-00000280: 6567 6f72 6965 732e 0d0a 0d0a 2323 2055  egories.....## U
-00000290: 7361 6765 0d0a 0d0a 2323 2320 5472 6169  sage....### Trai
-000002a0: 6e69 6e67 0d0a 0d0a 546f 2074 7261 696e  ning....To train
-000002b0: 2061 2074 6578 7420 636c 6173 7369 6669   a text classifi
-000002c0: 6361 7469 6f6e 206d 6f64 656c 2c20 796f  cation model, yo
-000002d0: 7520 6361 6e20 7574 696c 697a 6520 7468  u can utilize th
-000002e0: 6520 6074 7261 696e 5f6d 6f64 656c 6020  e `train_model` 
-000002f0: 6d65 7468 6f64 2070 726f 7669 6465 6420  method provided 
-00000300: 6279 2074 6865 2060 4d6f 6465 6c60 2063  by the `Model` c
-00000310: 6c61 7373 3a0d 0a0d 0a60 6060 7079 7468  lass:....```pyth
-00000320: 6f6e 0d0a 6672 6f6d 2041 7272 6f77 5465  on..from ArrowTe
-00000330: 7874 436c 6173 7369 6669 6572 2069 6d70  xtClassifier imp
-00000340: 6f72 7420 4d6f 6465 6c0d 0a0d 0a6d 6f64  ort Model....mod
-00000350: 656c 203d 204d 6f64 656c 286e 616d 653d  el = Model(name=
-00000360: 2279 6f75 725f 6d6f 6465 6c5f 6e61 6d65  "your_model_name
-00000370: 2229 0d0a 6d6f 6465 6c2e 7472 6169 6e5f  ")..model.train_
-00000380: 6d6f 6465 6c28 6461 7461 7365 7429 0d0a  model(dataset)..
-00000390: 6060 600d 0a0d 0a23 2323 2320 486f 7720  ```....#### How 
-000003a0: 746f 206d 616b 6520 6120 6461 7461 7365  to make a datase
-000003b0: 740d 0a0d 0a54 6f20 6d61 6b65 2079 6f75  t....To make you
-000003c0: 7220 6f77 6e20 6375 7374 6f6d 2064 6174  r own custom dat
-000003d0: 6173 6574 2066 6f72 2074 7261 696e 696e  aset for trainin
-000003e0: 6720 796f 7520 6e65 6564 2074 6f20 6372  g you need to cr
-000003f0: 6561 7465 2061 2070 6172 7175 6574 2066  eate a parquet f
-00000400: 696c 6520 7769 7468 2074 6865 2066 6f6c  ile with the fol
-00000410: 6c6f 7769 6e67 2066 6f72 6d61 743a 0d0a  lowing format:..
-00000420: 0d0a 2a45 7861 6d70 6c65 2050 6172 7175  ..*Example Parqu
-00000430: 6574 2046 696c 652a 0d0a 0d0a 6060 606a  et File*....```j
-00000440: 736f 6e0d 0a7b 226c 6162 656c 223a 226e  son..{"label":"n
-00000450: 6f72 6d61 6c22 2c22 6578 616d 706c 6522  ormal","example"
-00000460: 3a22 4865 7920 7468 6572 6521 227d 0d0a  :"Hey there!"}..
-00000470: 7b22 6c61 6265 6c22 3a22 6e6f 726d 616c  {"label":"normal
-00000480: 222c 2265 7861 6d70 6c65 223a 2248 6921  ","example":"Hi!
-00000490: 227d 0d0a 7b22 6c61 6265 6c22 3a22 746f  "}..{"label":"to
-000004a0: 7869 6322 2c22 6578 616d 706c 6522 3a22  xic","example":"
-000004b0: 596f 7520 7375 636b 2122 7d0d 0a60 6060  You suck!"}..```
-000004c0: 0d0a 0d0a 4166 7465 7220 796f 7520 6861  ....After you ha
-000004d0: 7665 2063 7265 6174 6564 2074 6865 2070  ve created the p
-000004e0: 6172 7175 6574 2066 696c 6520 7769 7468  arquet file with
-000004f0: 2074 6865 2064 6174 6120 696e 2074 6865   the data in the
-00000500: 2066 6f72 6d61 7420 6162 6f76 652c 2079   format above, y
-00000510: 6f75 2063 616e 2070 726f 7669 6465 2074  ou can provide t
-00000520: 6f20 7468 6520 6461 7461 7365 7420 746f  o the dataset to
-00000530: 2073 7461 7274 2074 7261 696e 696e 6720   start training 
-00000540: 7468 6520 6d6f 6465 6c2e 0d0a 0d0a 2323  the model.....##
-00000550: 2320 5375 6d6d 6172 697a 6174 696f 6e0d  # Summarization.
-00000560: 0a0d 0a54 6f20 7375 6d6d 6172 697a 6520  ...To summarize 
-00000570: 6120 7472 6169 6e65 6420 6d6f 6465 6c2c  a trained model,
-00000580: 2079 6f75 2063 616e 2075 7365 2074 6865   you can use the
-00000590: 2060 7375 6d6d 6172 697a 6560 206d 6574   `summarize` met
-000005a0: 686f 643a 0d0a 0d0a 6060 6070 7974 686f  hod:....```pytho
-000005b0: 6e0d 0a6d 6f64 656c 2e73 756d 6d61 7269  n..model.summari
-000005c0: 7a65 280d 0a20 2020 206d 6f64 656c 5f70  ze(..    model_p
-000005d0: 6174 683d 2270 6174 685f 746f 5f79 6f75  ath="path_to_you
-000005e0: 725f 6d6f 6465 6c22 2c0d 0a20 2020 2068  r_model",..    h
-000005f0: 7970 6572 7061 7261 6d73 5f70 6174 683d  yperparams_path=
-00000600: 2270 6174 685f 746f 5f68 7970 6572 7061  "path_to_hyperpa
-00000610: 7261 6d65 7465 7273 5f66 696c 6522 2c0d  rameters_file",.
-00000620: 0a20 2020 2076 6f63 6162 756c 6172 795f  .    vocabulary_
-00000630: 7061 7468 3d22 7061 7468 5f74 6f5f 766f  path="path_to_vo
-00000640: 6361 6275 6c61 7279 5f66 696c 6522 2c0d  cabulary_file",.
-00000650: 0a20 2020 206d 6f64 656c 5375 6d6d 6172  .    modelSummar
-00000660: 795f 7772 6974 655f 7061 7468 3d22 7061  y_write_path="pa
-00000670: 7468 5f74 6f5f 7772 6974 655f 6d6f 6465  th_to_write_mode
-00000680: 6c5f 7375 6d6d 6172 7922 0d0a 290d 0a60  l_summary"..)..`
-00000690: 6060 0d0a 0d0a 2323 2320 436c 6173 7369  ``....### Classi
-000006a0: 6669 6361 7469 6f6e 0d0a 0d0a 466f 7220  fication....For 
-000006b0: 636c 6173 7369 6679 696e 6720 7465 7874  classifying text
-000006c0: 2075 7369 6e67 2074 6865 2074 7261 696e   using the train
-000006d0: 6564 206d 6f64 656c 3a0d 0a0d 0a60 6060  ed model:....```
-000006e0: 7079 7468 6f6e 0d0a 7265 7375 6c74 203d  python..result =
-000006f0: 206d 6f64 656c 2e63 6c61 7373 6966 7928   model.classify(
-00000700: 0d0a 2020 2020 6d6f 6465 6c5f 7061 7468  ..    model_path
-00000710: 3d22 7061 7468 5f74 6f5f 796f 7572 5f6d  ="path_to_your_m
-00000720: 6f64 656c 222c 0d0a 2020 2020 6879 7065  odel",..    hype
-00000730: 7270 6172 616d 735f 7061 7468 3d22 7061  rparams_path="pa
-00000740: 7468 5f74 6f5f 6879 7065 7270 6172 616d  th_to_hyperparam
-00000750: 6574 6572 735f 6669 6c65 222c 0d0a 2020  eters_file",..  
-00000760: 2020 7465 7874 3d22 796f 7572 5f69 6e70    text="your_inp
-00000770: 7574 5f74 6578 7422 2c0d 0a20 2020 2076  ut_text",..    v
-00000780: 6f63 6162 756c 6172 795f 7061 7468 3d22  ocabulary_path="
-00000790: 7061 7468 5f74 6f5f 766f 6361 6275 6c61  path_to_vocabula
-000007a0: 7279 5f66 696c 6522 0d0a 290d 0a70 7269  ry_file"..)..pri
-000007b0: 6e74 2872 6573 756c 7429 0d0a 6060 600d  nt(result)..```.
-000007c0: 0a0d 0a23 2320 4765 7474 696e 6720 5374  ...## Getting St
-000007d0: 6172 7465 640d 0a0d 0a54 6869 7320 7061  arted....This pa
-000007e0: 636b 6167 6520 7072 6f76 6964 6573 2074  ckage provides t
-000007f0: 6f6f 6c73 2066 6f72 2074 6578 7420 636c  ools for text cl
-00000800: 6173 7369 6669 6361 7469 6f6e 2074 6173  assification tas
-00000810: 6b73 2e20 596f 7520 6361 6e20 6578 706c  ks. You can expl
-00000820: 6f72 6520 616e 6420 6375 7374 6f6d 697a  ore and customiz
-00000830: 6520 6974 2061 6363 6f72 6469 6e67 2074  e it according t
-00000840: 6f20 796f 7572 2072 6571 7569 7265 6d65  o your requireme
-00000850: 6e74 732e 2052 6566 6572 2074 6f20 7468  nts. Refer to th
-00000860: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
-00000870: 666f 7220 6465 7461 696c 6564 2075 7361  for detailed usa
-00000880: 6765 2069 6e73 7472 7563 7469 6f6e 732e  ge instructions.
-00000890: 0d0a 0d0a 2323 204c 6963 656e 7365 0d0a  ....## License..
-000008a0: 0d0a 5468 6973 2070 726f 6a65 6374 2069  ..This project i
-000008b0: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
-000008c0: 2074 6865 204d 4954 204c 6963 656e 7365   the MIT License
-000008d0: 202d 2073 6565 2074 6865 204c 4943 454e   - see the LICEN
-000008e0: 5345 2066 696c 6520 666f 7220 6465 7461  SE file for deta
-000008f0: 696c 732e 0d0a 0d0a 2d2d 2d0d 0a0d 0a23  ils.....---....#
-00000900: 2320 436f 6e74 6163 740d 0a0d 0a46 6f72  # Contact....For
-00000910: 2061 6e79 2071 7565 7374 696f 6e73 206f   any questions o
-00000920: 7220 6665 6564 6261 636b 2c20 706c 6561  r feedback, plea
-00000930: 7365 2063 6f6e 7461 6374 2074 6563 686e  se contact techn
-00000940: 6f6c 6f67 7970 6f77 6572 3234 4067 6d61  ologypower24@gma
-00000950: 696c 2e63 6f6d 206f 7220 796f 7520 6361  il.com or you ca
-00000960: 6e20 636f 6e74 6163 7420 6d65 2061 7420  n contact me at 
-00000970: 6469 7363 6f72 6420 2d20 7465 6368 706f  discord - techpo
-00000980: 7765 7262 2e                             werb.
+00000000: 2320 4172 726f 7754 6578 7443 6c61 7373  # ArrowTextClass
+00000010: 6966 6965 720d 0a0d 0a41 7272 6f77 5465  ifier....ArrowTe
+00000020: 7874 436c 6173 7369 6669 6572 2069 7320  xtClassifier is 
+00000030: 6120 5079 7468 6f6e 2070 6163 6b61 6765  a Python package
+00000040: 2066 6f72 2074 6578 7420 636c 6173 7369   for text classi
+00000050: 6669 6361 7469 6f6e 2074 6173 6b73 2c20  fication tasks, 
+00000060: 6f66 6665 7269 6e67 2066 756e 6374 696f  offering functio
+00000070: 6e61 6c69 7469 6573 2074 6f20 7472 6169  nalities to trai
+00000080: 6e2c 2073 756d 6d61 7269 7a65 2c20 616e  n, summarize, an
+00000090: 6420 636c 6173 7369 6679 2074 6578 7420  d classify text 
+000000a0: 7573 696e 6720 636f 6e76 6f6c 7574 696f  using convolutio
+000000b0: 6e61 6c20 6e65 7572 616c 206e 6574 776f  nal neural netwo
+000000c0: 726b 2028 434e 4e29 2061 7263 6869 7465  rk (CNN) archite
+000000d0: 6374 7572 652e 0d0a 0d0a 2323 2049 6e73  cture.....## Ins
+000000e0: 7461 6c6c 6174 696f 6e0d 0a0d 0a59 6f75  tallation....You
+000000f0: 2063 616e 2069 6e73 7461 6c6c 2041 7272   can install Arr
+00000100: 6f77 5465 7874 436c 6173 7369 6669 6572  owTextClassifier
+00000110: 2076 6961 2070 6970 3a0d 0a0d 0a60 6060   via pip:....```
+00000120: 6261 7368 0d0a 7069 7020 696e 7374 616c  bash..pip instal
+00000130: 6c20 4172 726f 7754 6578 7443 6c61 7373  l ArrowTextClass
+00000140: 6966 6965 720d 0a60 6060 0d0a 0d0a 2323  ifier..```....##
+00000150: 2048 6f77 2069 7420 576f 726b 730d 0a0d   How it Works...
+00000160: 0a41 7272 6f77 5465 7874 436c 6173 7369  .ArrowTextClassi
+00000170: 6669 6572 2069 6d70 6c65 6d65 6e74 7320  fier implements 
+00000180: 6120 636f 6e76 6f6c 7574 696f 6e61 6c20  a convolutional 
+00000190: 6e65 7572 616c 206e 6574 776f 726b 2028  neural network (
+000001a0: 434e 4e29 2061 7263 6869 7465 6374 7572  CNN) architectur
+000001b0: 6520 666f 7220 7465 7874 2063 6c61 7373  e for text class
+000001c0: 6966 6963 6174 696f 6e2e 2049 7420 746f  ification. It to
+000001d0: 6b65 6e69 7a65 7320 696e 7075 7420 7465  kenizes input te
+000001e0: 7874 2c20 656d 6265 6473 2074 6865 2074  xt, embeds the t
+000001f0: 6f6b 656e 732c 2061 7070 6c69 6573 2063  okens, applies c
+00000200: 6f6e 766f 6c75 7469 6f6e 616c 2066 696c  onvolutional fil
+00000210: 7465 7273 206f 7665 7220 7468 6520 656d  ters over the em
+00000220: 6265 6464 6564 2074 6f6b 656e 7320 746f  bedded tokens to
+00000230: 2065 7874 7261 6374 2066 6561 7475 7265   extract feature
+00000240: 732c 2061 6e64 2074 6865 6e20 636c 6173  s, and then clas
+00000250: 7369 6669 6573 2074 6865 2074 6578 7420  sifies the text 
+00000260: 696e 746f 2070 7265 6465 6669 6e65 6420  into predefined 
+00000270: 6361 7465 676f 7269 6573 2e0d 0a0d 0a23  categories.....#
+00000280: 2320 5573 6167 650d 0a0d 0a23 2323 2054  # Usage....### T
+00000290: 7261 696e 696e 670d 0a0d 0a54 6f20 7472  raining....To tr
+000002a0: 6169 6e20 6120 7465 7874 2063 6c61 7373  ain a text class
+000002b0: 6966 6963 6174 696f 6e20 6d6f 6465 6c2c  ification model,
+000002c0: 2079 6f75 2063 616e 2075 7469 6c69 7a65   you can utilize
+000002d0: 2074 6865 2060 7472 6169 6e5f 6d6f 6465   the `train_mode
+000002e0: 6c60 206d 6574 686f 6420 7072 6f76 6964  l` method provid
+000002f0: 6564 2062 7920 7468 6520 604d 6f64 656c  ed by the `Model
+00000300: 6020 636c 6173 733a 0d0a 0d0a 6060 6070  ` class:....```p
+00000310: 7974 686f 6e0d 0a66 726f 6d20 4172 726f  ython..from Arro
+00000320: 7754 6578 7443 6c61 7373 6966 6965 7220  wTextClassifier 
+00000330: 696d 706f 7274 204d 6f64 656c 0d0a 0d0a  import Model....
+00000340: 6d6f 6465 6c20 3d20 4d6f 6465 6c28 6e61  model = Model(na
+00000350: 6d65 3d22 796f 7572 5f6d 6f64 656c 5f6e  me="your_model_n
+00000360: 616d 6522 290d 0a6d 6f64 656c 2e74 7261  ame")..model.tra
+00000370: 696e 5f6d 6f64 656c 2864 6174 6173 6574  in_model(dataset
+00000380: 290d 0a60 6060 0d0a 0d0a 2323 2323 2048  )..```....#### H
+00000390: 6f77 2074 6f20 6d61 6b65 2061 2064 6174  ow to make a dat
+000003a0: 6173 6574 0d0a 0d0a 546f 206d 616b 6520  aset....To make 
+000003b0: 796f 7572 206f 776e 2063 7573 746f 6d20  your own custom 
+000003c0: 6461 7461 7365 7420 666f 7220 7472 6169  dataset for trai
+000003d0: 6e69 6e67 2079 6f75 206e 6565 6420 746f  ning you need to
+000003e0: 2063 7265 6174 6520 6120 7061 7271 7565   create a parque
+000003f0: 7420 6669 6c65 2077 6974 6820 7468 6520  t file with the 
+00000400: 666f 6c6c 6f77 696e 6720 666f 726d 6174  following format
+00000410: 3a0d 0a0d 0a2a 4578 616d 706c 6520 5061  :....*Example Pa
+00000420: 7271 7565 7420 4669 6c65 2a0d 0a0d 0a60  rquet File*....`
+00000430: 6060 6a73 6f6e 0d0a 7b22 6c61 6265 6c22  ``json..{"label"
+00000440: 3a22 6e6f 726d 616c 222c 2265 7861 6d70  :"normal","examp
+00000450: 6c65 223a 2248 6579 2074 6865 7265 2122  le":"Hey there!"
+00000460: 7d0d 0a7b 226c 6162 656c 223a 226e 6f72  }..{"label":"nor
+00000470: 6d61 6c22 2c22 6578 616d 706c 6522 3a22  mal","example":"
+00000480: 4869 2122 7d0d 0a7b 226c 6162 656c 223a  Hi!"}..{"label":
+00000490: 2274 6f78 6963 222c 2265 7861 6d70 6c65  "toxic","example
+000004a0: 223a 2259 6f75 2073 7563 6b21 227d 0d0a  ":"You suck!"}..
+000004b0: 6060 600d 0a0d 0a41 6674 6572 2079 6f75  ```....After you
+000004c0: 2068 6176 6520 6372 6561 7465 6420 7468   have created th
+000004d0: 6520 7061 7271 7565 7420 6669 6c65 2077  e parquet file w
+000004e0: 6974 6820 7468 6520 6461 7461 2069 6e20  ith the data in 
+000004f0: 7468 6520 666f 726d 6174 2061 626f 7665  the format above
+00000500: 2c20 796f 7520 6361 6e20 7072 6f76 6964  , you can provid
+00000510: 6520 746f 2074 6865 2064 6174 6173 6574  e to the dataset
+00000520: 2074 6f20 7374 6172 7420 7472 6169 6e69   to start traini
+00000530: 6e67 2074 6865 206d 6f64 656c 2e0d 0a0d  ng the model....
+00000540: 0a23 2323 2053 756d 6d61 7269 7a61 7469  .### Summarizati
+00000550: 6f6e 0d0a 0d0a 546f 2073 756d 6d61 7269  on....To summari
+00000560: 7a65 2061 2074 7261 696e 6564 206d 6f64  ze a trained mod
+00000570: 656c 2c20 796f 7520 6361 6e20 7573 6520  el, you can use 
+00000580: 7468 6520 6073 756d 6d61 7269 7a65 6020  the `summarize` 
+00000590: 6d65 7468 6f64 3a0d 0a0d 0a60 6060 7079  method:....```py
+000005a0: 7468 6f6e 0d0a 6d6f 6465 6c2e 7375 6d6d  thon..model.summ
+000005b0: 6172 697a 6528 0d0a 2020 2020 6d6f 6465  arize(..    mode
+000005c0: 6c5f 7061 7468 3d22 7061 7468 5f74 6f5f  l_path="path_to_
+000005d0: 796f 7572 5f6d 6f64 656c 222c 0d0a 2020  your_model",..  
+000005e0: 2020 6879 7065 7270 6172 616d 735f 7061    hyperparams_pa
+000005f0: 7468 3d22 7061 7468 5f74 6f5f 6879 7065  th="path_to_hype
+00000600: 7270 6172 616d 6574 6572 735f 6669 6c65  rparameters_file
+00000610: 222c 0d0a 2020 2020 766f 6361 6275 6c61  ",..    vocabula
+00000620: 7279 5f70 6174 683d 2270 6174 685f 746f  ry_path="path_to
+00000630: 5f76 6f63 6162 756c 6172 795f 6669 6c65  _vocabulary_file
+00000640: 222c 0d0a 2020 2020 6d6f 6465 6c53 756d  ",..    modelSum
+00000650: 6d61 7279 5f77 7269 7465 5f70 6174 683d  mary_write_path=
+00000660: 2270 6174 685f 746f 5f77 7269 7465 5f6d  "path_to_write_m
+00000670: 6f64 656c 5f73 756d 6d61 7279 220d 0a29  odel_summary"..)
+00000680: 0d0a 6060 600d 0a0d 0a23 2323 2043 6c61  ..```....### Cla
+00000690: 7373 6966 6963 6174 696f 6e0d 0a0d 0a46  ssification....F
+000006a0: 6f72 2063 6c61 7373 6966 7969 6e67 2074  or classifying t
+000006b0: 6578 7420 7573 696e 6720 7468 6520 7472  ext using the tr
+000006c0: 6169 6e65 6420 6d6f 6465 6c3a 0d0a 0d0a  ained model:....
+000006d0: 6060 6070 7974 686f 6e0d 0a72 6573 756c  ```python..resul
+000006e0: 7420 3d20 6d6f 6465 6c2e 636c 6173 7369  t = model.classi
+000006f0: 6679 280d 0a20 2020 206d 6f64 656c 5f70  fy(..    model_p
+00000700: 6174 683d 2270 6174 685f 746f 5f79 6f75  ath="path_to_you
+00000710: 725f 6d6f 6465 6c22 2c0d 0a20 2020 2068  r_model",..    h
+00000720: 7970 6572 7061 7261 6d73 5f70 6174 683d  yperparams_path=
+00000730: 2270 6174 685f 746f 5f68 7970 6572 7061  "path_to_hyperpa
+00000740: 7261 6d65 7465 7273 5f66 696c 6522 2c0d  rameters_file",.
+00000750: 0a20 2020 2074 6578 743d 2279 6f75 725f  .    text="your_
+00000760: 696e 7075 745f 7465 7874 222c 0d0a 2020  input_text",..  
+00000770: 2020 766f 6361 6275 6c61 7279 5f70 6174    vocabulary_pat
+00000780: 683d 2270 6174 685f 746f 5f76 6f63 6162  h="path_to_vocab
+00000790: 756c 6172 795f 6669 6c65 220d 0a29 0d0a  ulary_file"..)..
+000007a0: 7072 696e 7428 7265 7375 6c74 290d 0a60  print(result)..`
+000007b0: 6060 0d0a 0d0a 2323 2047 6574 7469 6e67  ``....## Getting
+000007c0: 2053 7461 7274 6564 0d0a 0d0a 5468 6973   Started....This
+000007d0: 2070 6163 6b61 6765 2070 726f 7669 6465   package provide
+000007e0: 7320 746f 6f6c 7320 666f 7220 7465 7874  s tools for text
+000007f0: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
+00000800: 7461 736b 732e 2059 6f75 2063 616e 2065  tasks. You can e
+00000810: 7870 6c6f 7265 2061 6e64 2063 7573 746f  xplore and custo
+00000820: 6d69 7a65 2069 7420 6163 636f 7264 696e  mize it accordin
+00000830: 6720 746f 2079 6f75 7220 7265 7175 6972  g to your requir
+00000840: 656d 656e 7473 2e20 5265 6665 7220 746f  ements. Refer to
+00000850: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
+00000860: 6f6e 2066 6f72 2064 6574 6169 6c65 6420  on for detailed 
+00000870: 7573 6167 6520 696e 7374 7275 6374 696f  usage instructio
+00000880: 6e73 2e20 5765 2068 6176 6520 616c 736f  ns. We have also
+00000890: 206d 6164 6520 6f75 7220 6f77 6e20 636f   made our own co
+000008a0: 6c61 6220 5b6e 6f74 6562 6f6f 6b5d 2868  lab [notebook](h
+000008b0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
+000008c0: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
+000008d0: 2f64 7269 7665 2f31 6647 444c 4943 6b63  /drive/1fGDLICkc
+000008e0: 7466 6470 5467 4c6f 685f 426f 7576 2d4e  tfdpTgLoh_Bouv-N
+000008f0: 592d 712d 6b64 6c51 3f75 7370 3d73 6861  Y-q-kdlQ?usp=sha
+00000900: 7269 6e67 2920 746f 2068 656c 7020 796f  ring) to help yo
+00000910: 7520 7472 6169 6e20 6120 6375 7374 6f6d  u train a custom
+00000920: 206f 6666 656e 7369 7665 206c 616e 6775   offensive langu
+00000930: 6167 6520 636c 6173 7369 6669 6572 2075  age classifier u
+00000940: 7369 6e67 2074 6869 732e 0d0a 0d0a 2323  sing this.....##
+00000950: 204c 6963 656e 7365 0d0a 0d0a 5468 6973   License....This
+00000960: 2070 726f 6a65 6374 2069 7320 6c69 6365   project is lice
+00000970: 6e73 6564 2075 6e64 6572 2074 6865 204d  nsed under the M
+00000980: 4954 204c 6963 656e 7365 202d 2073 6565  IT License - see
+00000990: 2074 6865 204c 4943 454e 5345 2066 696c   the LICENSE fil
+000009a0: 6520 666f 7220 6465 7461 696c 732e 0d0a  e for details...
+000009b0: 0d0a 2d2d 2d0d 0a0d 0a23 2320 436f 6e74  ..---....## Cont
+000009c0: 6163 740d 0a0d 0a46 6f72 2061 6e79 2071  act....For any q
+000009d0: 7565 7374 696f 6e73 206f 7220 6665 6564  uestions or feed
+000009e0: 6261 636b 2c20 706c 6561 7365 2063 6f6e  back, please con
+000009f0: 7461 6374 2074 6563 686e 6f6c 6f67 7970  tact technologyp
+00000a00: 6f77 6572 3234 4067 6d61 696c 2e63 6f6d  ower24@gmail.com
+00000a10: 206f 7220 796f 7520 6361 6e20 636f 6e74   or you can cont
+00000a20: 6163 7420 6d65 2061 7420 6469 7363 6f72  act me at discor
+00000a30: 6420 2d20 7465 6368 706f 7765 7262 2e    d - techpowerb.
```

### Comparing `ArrowTextClassifier-1.0.0/setup.py` & `ArrowTextClassifier-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="ArrowTextClassifier",
-    version="1.0.0",
+    version="1.0.1",
     author="techpowerb",
     author_email="technologypower24@gmail.com",
     description="ArrowTextClassifier is a simple text classification tool written in pytorch that allows you to train, summarize, and use text classification models for various tasks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bhargav230m/ArrowTextClassifier.git",
     packages=find_packages(),
@@ -25,15 +25,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     install_requires=[
         "torch==2.2.2",
-        "torchsummary==1.4.5",
+        "torchsummary==1.5.1",
         "pandas==2.2.2",
         "scikit-learn==1.4.2",
         "tqdm==4.66.2",
         "numpy==1.26.4",
     ],
     keywords=[
         "text classification",
```

### Comparing `ArrowTextClassifier-1.0.0/src/classify_text.py` & `ArrowTextClassifier-1.0.1/src/classify_text.py`

 * *Files identical despite different names*

### Comparing `ArrowTextClassifier-1.0.0/src/main.py` & `ArrowTextClassifier-1.0.1/src/main.py`

 * *Files identical despite different names*

### Comparing `ArrowTextClassifier-1.0.0/src/model.py` & `ArrowTextClassifier-1.0.1/src/model.py`

 * *Files identical despite different names*

### Comparing `ArrowTextClassifier-1.0.0/src/summarize_model.py` & `ArrowTextClassifier-1.0.1/src/summarize_model.py`

 * *Files identical despite different names*

### Comparing `ArrowTextClassifier-1.0.0/src/tokenizer.py` & `ArrowTextClassifier-1.0.1/src/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ArrowTextClassifier-1.0.0/src/train.py` & `ArrowTextClassifier-1.0.1/src/train.py`

 * *Files identical despite different names*

