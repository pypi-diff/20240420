# Comparing `tmp/basic-pitch-0.3.0.tar.gz` & `tmp/basic_pitch-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic-pitch-0.3.0.tar", last modified: Mon Mar 25 14:49:44 2024, max compression
+gzip compressed data, was "basic_pitch-0.3.1.tar", last modified: Fri Apr 19 23:47:08 2024, max compression
```

## Comparing `basic-pitch-0.3.0.tar` & `basic_pitch-0.3.1.tar`

### file list

```diff
@@ -1,65 +1,62 @@
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.039175 basic-pitch-0.3.0/
--rw-r--r--   0 drubinstein   (501) staff       (20)     7365 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 drubinstein   (501) staff       (20)     3559 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 drubinstein   (501) staff       (20)    11384 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/LICENSE
--rw-r--r--   0 drubinstein   (501) staff       (20)      254 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/MANIFEST.in
--rw-r--r--   0 drubinstein   (501) staff       (20)     1034 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/NOTICE
--rw-r--r--   0 drubinstein   (501) staff       (20)     1110 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/OWNERS.md
--rw-r--r--   0 drubinstein   (501) staff       (20)     2201 2024-03-25 14:49:44.038850 basic-pitch-0.3.0/PKG-INFO
--rw-r--r--   0 drubinstein   (501) staff       (20)    10100 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/README.md
--rw-r--r--   0 drubinstein   (501) staff       (20)      970 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/SECURITY.md
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.028541 basic-pitch-0.3.0/basic_pitch/
--rw-r--r--   0 drubinstein   (501) staff       (20)     2495 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/__init__.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     2299 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/commandline_printing.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     2243 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/constants.py
--rw-r--r--   0 drubinstein   (501) staff       (20)    22468 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/inference.py
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.030234 basic-pitch-0.3.0/basic_pitch/layers/
--rw-r--r--   0 drubinstein   (501) staff       (20)        0 2022-07-11 03:34:09.000000 basic-pitch-0.3.0/basic_pitch/layers/__init__.py
--rw-r--r--   0 drubinstein   (501) staff       (20)      981 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/layers/math.py
--rw-r--r--   0 drubinstein   (501) staff       (20)    26130 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/layers/nnaudio.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     7258 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/layers/signal.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     9870 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/models.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     3988 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/nn.py
--rw-r--r--   0 drubinstein   (501) staff       (20)    18921 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/note_creation.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     5995 2024-03-25 14:47:57.000000 basic-pitch-0.3.0/basic_pitch/predict.py
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.023559 basic-pitch-0.3.0/basic_pitch/saved_models/
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.030801 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.031123 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp/
--rw-r--r--   0 drubinstein   (501) staff       (20)  1084140 2023-09-12 18:15:16.000000 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.033373 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp/variables/
--rw-r--r--   0 drubinstein   (501) staff       (20)   219309 2022-07-11 03:34:10.000000 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001
--rw-r--r--   0 drubinstein   (501) staff       (20)     4794 2022-07-11 03:34:10.000000 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.032361 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.024233 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.032557 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/
--rw-r--r--   0 drubinstein   (501) staff       (20)   123027 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/model.mlmodel
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.032807 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/weights/
--rw-r--r--   0 drubinstein   (501) staff       (20)   145956 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/weights/weight.bin
--rw-r--r--   0 drubinstein   (501) staff       (20)      617 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Manifest.json
--rw-r--r--   0 drubinstein   (501) staff       (20)   230444 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.onnx
--rw-r--r--   0 drubinstein   (501) staff       (20)   204448 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.tflite
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.036909 basic-pitch-0.3.0/basic_pitch.egg-info/
--rw-r--r--   0 drubinstein   (501) staff       (20)     2201 2024-03-25 14:49:43.000000 basic-pitch-0.3.0/basic_pitch.egg-info/PKG-INFO
--rw-r--r--   0 drubinstein   (501) staff       (20)     1473 2024-03-25 14:49:43.000000 basic-pitch-0.3.0/basic_pitch.egg-info/SOURCES.txt
--rw-r--r--   0 drubinstein   (501) staff       (20)        1 2024-03-25 14:49:43.000000 basic-pitch-0.3.0/basic_pitch.egg-info/dependency_links.txt
--rw-r--r--   0 drubinstein   (501) staff       (20)       57 2024-03-25 14:49:43.000000 basic-pitch-0.3.0/basic_pitch.egg-info/entry_points.txt
--rw-r--r--   0 drubinstein   (501) staff       (20)      838 2024-03-25 14:49:43.000000 basic-pitch-0.3.0/basic_pitch.egg-info/requires.txt
--rw-r--r--   0 drubinstein   (501) staff       (20)       12 2024-03-25 14:49:43.000000 basic-pitch-0.3.0/basic_pitch.egg-info/top_level.txt
--rw-r--r--   0 drubinstein   (501) staff       (20)      115 2022-07-11 02:52:39.000000 basic-pitch-0.3.0/catalog-info.yaml
--rw-r--r--   0 drubinstein   (501) staff       (20)     2281 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/pyproject.toml
--rw-r--r--   0 drubinstein   (501) staff       (20)       38 2024-03-25 14:49:44.039261 basic-pitch-0.3.0/setup.cfg
--rw-r--r--   0 drubinstein   (501) staff       (20)      686 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/setup.py
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.034064 basic-pitch-0.3.0/tests/
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.034920 basic-pitch-0.3.0/tests/resources/
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2024-03-25 14:49:44.036649 basic-pitch-0.3.0/tests/resources/vocadito_10/
--rw-r--r--   0 drubinstein   (501) staff       (20)  1376949 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/tests/resources/vocadito_10/model_output.npz
--rw-r--r--   0 drubinstein   (501) staff       (20)    19044 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/tests/resources/vocadito_10/note_events.npz
--rw-r--r--   0 drubinstein   (501) staff       (20)   802472 2022-07-11 03:34:19.000000 basic-pitch-0.3.0/tests/resources/vocadito_10.wav
--rw-r--r--   0 drubinstein   (501) staff       (20)  1075892 2023-09-12 18:15:16.000000 basic-pitch-0.3.0/tests/resources/vocadito_14.wav
--rw-r--r--   0 drubinstein   (501) staff       (20)     6839 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/tests/test_inference.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     3861 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/tests/test_nn.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     2115 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/tests/test_note_creation.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     1491 2024-03-25 14:47:20.000000 basic-pitch-0.3.0/tox.ini
--rw-r--r--   0 drubinstein   (501) staff       (20)     3150 2024-03-12 19:03:05.000000 basic-pitch-0.3.0/tox.txt
--rw-r--r--   0 drubinstein   (501) staff       (20)        0 2024-03-12 19:18:57.000000 basic-pitch-0.3.0/with-tf.txt
--rw-r--r--   0 drubinstein   (501) staff       (20)     6237 2024-03-12 19:00:59.000000 basic-pitch-0.3.0/without-tf.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.086096 basic_pitch-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/OWNERS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12299 2024-04-19 23:47:08.086096 basic_pitch-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.074096 basic_pitch-0.3.1/basic_pitch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/commandline_printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22468 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.078096 basic_pitch-0.3.1/basic_pitch/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/layers/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26130 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/layers/nnaudio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/layers/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18929 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/note_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.070096 basic_pitch-0.3.1/basic_pitch/saved_models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.078096 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.078096 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp/
+-rw-r--r--   0 runner    (1001) docker     (127)  1084140 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.082096 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)   219309 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.078096 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.070096 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.078096 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/
+-rw-r--r--   0 runner    (1001) docker     (127)   123027 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/model.mlmodel
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.078096 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/weights/
+-rw-r--r--   0 runner    (1001) docker     (127)   145956 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/weights/weight.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)   230444 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.onnx
+-rw-r--r--   0 runner    (1001) docker     (127)   204448 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.tflite
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.086096 basic_pitch-0.3.1/basic_pitch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12299 2024-04-19 23:47:08.000000 basic_pitch-0.3.1/basic_pitch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-19 23:47:08.000000 basic_pitch-0.3.1/basic_pitch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 23:47:08.000000 basic_pitch-0.3.1/basic_pitch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 23:47:08.000000 basic_pitch-0.3.1/basic_pitch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-19 23:47:08.000000 basic_pitch-0.3.1/basic_pitch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 23:47:08.000000 basic_pitch-0.3.1/basic_pitch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/catalog-info.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 23:47:08.086096 basic_pitch-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.082096 basic_pitch-0.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.082096 basic_pitch-0.3.1/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:47:08.086096 basic_pitch-0.3.1/tests/resources/vocadito_10/
+-rw-r--r--   0 runner    (1001) docker     (127)  1376949 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/tests/resources/vocadito_10/model_output.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/tests/resources/vocadito_10/note_events.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   802472 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/tests/resources/vocadito_10.wav
+-rw-r--r--   0 runner    (1001) docker     (127)  1075892 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/tests/resources/vocadito_14.wav
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/tests/test_note_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-19 23:46:58.000000 basic_pitch-0.3.1/tox.ini
```

### Comparing `basic-pitch-0.3.0/CODE_OF_CONDUCT.md` & `basic_pitch-0.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/CONTRIBUTING.md` & `basic_pitch-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/LICENSE` & `basic_pitch-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/NOTICE` & `basic_pitch-0.3.1/NOTICE`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/OWNERS.md` & `basic_pitch-0.3.1/OWNERS.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/README.md` & `basic_pitch-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/SECURITY.md` & `basic_pitch-0.3.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/__init__.py` & `basic_pitch-0.3.1/basic_pitch/__init__.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/commandline_printing.py` & `basic_pitch-0.3.1/basic_pitch/commandline_printing.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/constants.py` & `basic_pitch-0.3.1/basic_pitch/constants.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/inference.py` & `basic_pitch-0.3.1/basic_pitch/inference.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/layers/math.py` & `basic_pitch-0.3.1/basic_pitch/layers/math.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/layers/nnaudio.py` & `basic_pitch-0.3.1/basic_pitch/layers/nnaudio.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/layers/signal.py` & `basic_pitch-0.3.1/basic_pitch/layers/signal.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/models.py` & `basic_pitch-0.3.1/basic_pitch/models.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/nn.py` & `basic_pitch-0.3.1/basic_pitch/nn.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/note_creation.py` & `basic_pitch-0.3.1/basic_pitch/note_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         note_events: note event tuple
         n_bins_tolerance: Pitch bend estimation range. Defaults to 25.
 
     Returns:
         note events with pitch bends
     """
     window_length = n_bins_tolerance * 2 + 1
-    freq_gaussian = scipy.signal.gaussian(window_length, std=5)
+    freq_gaussian = scipy.signal.windows.gaussian(window_length, std=5)
     note_events_with_pitch_bends = []
     for start_idx, end_idx, pitch_midi, amplitude in note_events:
         freq_idx = int(np.round(midi_pitch_to_contour_bin(pitch_midi)))
         freq_start_idx = np.max([freq_idx - n_bins_tolerance, 0])
         freq_end_idx = np.min([N_FREQ_BINS_CONTOURS, freq_idx + n_bins_tolerance + 1])
 
         pitch_bend_submatrix = (
```

### Comparing `basic-pitch-0.3.0/basic_pitch/predict.py` & `basic_pitch-0.3.1/basic_pitch/predict.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb` & `basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001` & `basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index` & `basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/model.mlmodel` & `basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/model.mlmodel`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/weights/weight.bin` & `basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/weights/weight.bin`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Manifest.json` & `basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Manifest.json`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.onnx` & `basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.onnx`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch/saved_models/icassp_2022/nmp.tflite` & `basic_pitch-0.3.1/basic_pitch/saved_models/icassp_2022/nmp.tflite`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/basic_pitch.egg-info/SOURCES.txt` & `basic_pitch-0.3.1/basic_pitch.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 OWNERS.md
 README.md
 SECURITY.md
 catalog-info.yaml
 pyproject.toml
 setup.py
 tox.ini
-tox.txt
-with-tf.txt
-without-tf.txt
 basic_pitch/__init__.py
 basic_pitch/commandline_printing.py
 basic_pitch/constants.py
 basic_pitch/inference.py
 basic_pitch/models.py
 basic_pitch/nn.py
 basic_pitch/note_creation.py
```

### Comparing `basic-pitch-0.3.0/basic_pitch.egg-info/requires.txt` & `basic_pitch-0.3.1/basic_pitch.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 pretty_midi>=0.2.9
 resampy<0.4.3,>=0.2.2
 scikit-learn
 scipy>=1.4.1
 typing_extensions
 
 [:platform_system != "Darwin" and python_version >= "3.11"]
-tensorflow<2.16,>=2.4.1
+tensorflow<2.15.1,>=2.4.1
 
-[:platform_system == "Darwin" and python_version < "3.11"]
+[:platform_system == "Darwin"]
 coremltools
-
-[:platform_system == "Darwin" and python_version >= "3.11"]
-tensorflow-macos>=2.4.1
+tensorflow-macos<2.15.1,>=2.4.1
 
 [:platform_system == "Linux" and python_version < "3.11"]
 tflite-runtime
 
 [:platform_system == "Windows" and python_version < "3.11"]
 onnxruntime
 
@@ -40,11 +38,11 @@
 coverage>=5.0.2
 pytest>=6.1.1
 pytest-mock
 
 [tf]
 
 [tf:platform_system != "Darwin"]
-tensorflow<2.16,>=2.4.1
+tensorflow<2.15.1,>=2.4.1
 
 [tf:platform_system == "Darwin" and python_version > "3.7"]
-tensorflow-macos<2.16,>=2.4.1
+tensorflow-macos<2.15.1,>=2.4.1
```

### Comparing `basic-pitch-0.3.0/pyproject.toml` & `basic_pitch-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [project]
 name = "basic-pitch"
-version = "0.3.0"
+version = "0.3.1"
 description = "Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection."
+readme = "README.md"
 keywords = []
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
 	"Natural Language :: English",
 	"Operating System :: POSIX :: Linux",
 	"Operating System :: MacOS :: MacOS X",
 	"Operating System :: Microsoft :: Windows",
@@ -13,37 +14,37 @@
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = [
-	"coremltools; platform_system == 'Darwin' and python_version < '3.11'",
+	"coremltools; platform_system == 'Darwin'",
 	"librosa>=0.8.0",
 	"mir_eval>=0.6",
 	"numpy>=1.18",
 	"onnxruntime; platform_system == 'Windows' and python_version < '3.11'",
 	"pretty_midi>=0.2.9",
 	"resampy>=0.2.2,<0.4.3",
 	"scikit-learn",
 	"scipy>=1.4.1",
-	"tensorflow>=2.4.1,<2.16; platform_system != 'Darwin' and python_version >= '3.11'",
-	"tensorflow-macos>=2.4.1; platform_system == 'Darwin' and python_version >= '3.11'",
+	"tensorflow>=2.4.1,<2.15.1; platform_system != 'Darwin' and python_version >= '3.11'",
+	"tensorflow-macos>=2.4.1,<2.15.1; platform_system == 'Darwin'",
 	"tflite-runtime; platform_system == 'Linux' and python_version < '3.11'",
 	"typing_extensions",
 ]
 
 [metadata]
 author = "Spotify"
 author_email = "basic-pitch@spotify.com"
 maintainer = "Spotify"
 maintainer_email = "basic-pitch@spotify.com"
 url = "https://github.com/spotify/basic-pitch"
 long_description = "Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection. See https://github.com/spotify/basic-pitch for more details."
-license = "Apache 2.0"
+license = { file = "LICENSE" }
 
 [tool.setuptools.packages.find]
 where = ["."]
 exclude = ["tests"]
 namespaces = false
 
 [project.scripts]
@@ -52,16 +53,16 @@
 [project.optional-dependencies]
 test = [
 	"coverage>=5.0.2",
 	"pytest>=6.1.1",
 	"pytest-mock",
 ]
 tf = [
-	"tensorflow>=2.4.1,<2.16; platform_system != 'Darwin'",
-	"tensorflow-macos>=2.4.1,<2.16; platform_system == 'Darwin' and python_version > '3.7'",
+	"tensorflow>=2.4.1,<2.15.1; platform_system != 'Darwin'",
+	"tensorflow-macos>=2.4.1,<2.15.1; platform_system == 'Darwin' and python_version > '3.7'",
 ]
 coreml = ["coremltools"] 
 onnx = ["onnxruntime"]
 docs = ["mkdocs>=1.0.4"]
 dev = [
 	"basic_pitch[test,tf,coreml,onnx,docs]",
 	"mypy",
```

### Comparing `basic-pitch-0.3.0/setup.py` & `basic_pitch-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/tests/resources/vocadito_10/model_output.npz` & `basic_pitch-0.3.1/tests/resources/vocadito_10/model_output.npz`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/tests/resources/vocadito_10/note_events.npz` & `basic_pitch-0.3.1/tests/resources/vocadito_10/note_events.npz`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/tests/resources/vocadito_10.wav` & `basic_pitch-0.3.1/tests/resources/vocadito_10.wav`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/tests/resources/vocadito_14.wav` & `basic_pitch-0.3.1/tests/resources/vocadito_14.wav`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/tests/test_inference.py` & `basic_pitch-0.3.1/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/tests/test_nn.py` & `basic_pitch-0.3.1/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/tests/test_note_creation.py` & `basic_pitch-0.3.1/tests/test_note_creation.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.3.0/tox.ini` & `basic_pitch-0.3.1/tox.ini`

 * *Files identical despite different names*

