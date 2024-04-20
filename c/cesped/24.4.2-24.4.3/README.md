# Comparing `tmp/cesped-24.4.2.tar.gz` & `tmp/cesped-24.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesped-24.4.2.tar", last modified: Wed Apr 17 11:00:24 2024, max compression
+gzip compressed data, was "cesped-24.4.3.tar", last modified: Sat Apr 20 13:57:14 2024, max compression
```

## Comparing `cesped-24.4.2.tar` & `cesped-24.4.3.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.622914 cesped-24.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-17 10:43:36.000000 cesped-24.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 10:43:36.000000 cesped-24.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-17 11:00:24.622914 cesped-24.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-04-17 10:43:36.000000 cesped-24.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.610914 cesped-24.4.2/cesped/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.614914 cesped-24.4.2/cesped/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultDataAugmentation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultDataConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultInferenceConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultModelConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultOptimizerConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultRelionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/configs/defaultTrainerConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.618914 cesped-24.4.2/cesped/datamanager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/datamanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/datamanager/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/datamanager/ctf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/datamanager/plDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    22286 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/evaluateEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/inferEntry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.618914 cesped-24.4.2/cesped/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/network/featureExtractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/network/image2sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/network/plModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    28525 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/particlesDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/trainEntry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.618914 cesped-24.4.2/cesped/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/angles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/anglesStats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/cliBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/fsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/gaussianFilters.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/tensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/utils/volumeStats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.622914 cesped-24.4.2/cesped/zenodo/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/zenodo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/zenodo/bechmarkUrls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/zenodo/downloadFromZenodo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-17 10:43:36.000000 cesped-24.4.2/cesped/zenodo/uploadToZenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.622914 cesped-24.4.2/cesped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-17 11:00:24.000000 cesped-24.4.2/cesped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-17 11:00:24.000000 cesped-24.4.2/cesped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:00:24.000000 cesped-24.4.2/cesped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-17 11:00:24.000000 cesped-24.4.2/cesped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 11:00:24.000000 cesped-24.4.2/cesped.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-17 10:43:36.000000 cesped-24.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 11:00:24.622914 cesped-24.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-17 10:43:36.000000 cesped-24.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:00:24.622914 cesped-24.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:43:36.000000 cesped-24.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-17 10:43:36.000000 cesped-24.4.2/tests/test_anglesStats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-17 10:43:36.000000 cesped-24.4.2/tests/test_particlesDataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.107537 cesped-24.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-20 13:46:10.000000 cesped-24.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-20 13:46:10.000000 cesped-24.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-04-20 13:57:14.107537 cesped-24.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-20 13:46:10.000000 cesped-24.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.099537 cesped-24.4.3/cesped/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.103537 cesped-24.4.3/cesped/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultDataAugmentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultDataConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultInferenceConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultModelConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultOptimizerConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultRelionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultTrainerConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.103537 cesped-24.4.3/cesped/datamanager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/datamanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/datamanager/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/datamanager/ctf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/datamanager/plDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22286 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/evaluateEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/inferEntry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.103537 cesped-24.4.3/cesped/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/network/featureExtractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/network/image2sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/network/plModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28525 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/particlesDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/trainEntry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.107537 cesped-24.4.3/cesped/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/angles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/anglesStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/cliBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/fsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/gaussianFilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/tensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/volumeStats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.107537 cesped-24.4.3/cesped/zenodo/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/zenodo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/zenodo/bechmarkUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/zenodo/downloadFromZenodo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/zenodo/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/zenodo/uploadToZenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.107537 cesped-24.4.3/cesped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-04-20 13:57:14.000000 cesped-24.4.3/cesped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-20 13:57:14.000000 cesped-24.4.3/cesped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:57:14.000000 cesped-24.4.3/cesped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-20 13:57:14.000000 cesped-24.4.3/cesped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 13:57:14.000000 cesped-24.4.3/cesped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-20 13:46:10.000000 cesped-24.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:57:14.107537 cesped-24.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-20 13:46:10.000000 cesped-24.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.107537 cesped-24.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 13:46:10.000000 cesped-24.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-20 13:46:10.000000 cesped-24.4.3/tests/test_anglesStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-20 13:46:10.000000 cesped-24.4.3/tests/test_particlesDataset.py
```

### Comparing `cesped-24.4.2/LICENSE` & `cesped-24.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/PKG-INFO` & `cesped-24.4.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: cesped
-Version: 24.4.2
-Summary: Code utilities for the CESPED (Cryo-EM Supervised Pose Estimation Dataset) benchmark
-Home-page: https://github.com/rsanchezgarc/cesped
-Author: Ruben Sanchez-Garcia
-Author-email: ruben.sanchez-garcia@stats.ox.ac.uk
-Keywords: deep learning cryoem pose estimation
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: argParseFromDoc>=0.1.2
-Requires-Dist: e3nn>=0.5.1
-Requires-Dist: healpy>=1.16.5
-Requires-Dist: joblib>=1.3
-Requires-Dist: mrcfile<2.0.0,>=1.4.3
-Requires-Dist: numpy>=1.25.2
-Requires-Dist: omegaconf>=2.3.0
-Requires-Dist: pandas>=2.1.0
-Requires-Dist: pdoc3>=0.10.0
-Requires-Dist: lightning[pytorch-extra]<3.0.0,>=2.0.0
-Requires-Dist: requests>=2.31.0
-Requires-Dist: scipy>=1.11.2
-Requires-Dist: starfile>=0.4.12
-Requires-Dist: starstack>=0.2.0
-Requires-Dist: tensorboard>=2.12.1
-Requires-Dist: torch<3.0.0,>=2.0.0
-Requires-Dist: torchvision>=0.15.2
-
 # CESPED: Utilities for the Cryo-EM Supervised Pose Estimation Dataset
 
 CESPED, is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check our manuscript at https://arxiv.org/abs/2311.06194.
 
 ## Installation
 cesped has been tested on python 3.11. Installation should be automatic using pip
 ```
@@ -59,15 +31,15 @@
 2. Load a given entry
 ```
 targetName, halfset = listOfEntries[0] #We will work with the first entry only
 
 dataset = ParticlesDataset(targetName, halfset)
 ```
 For a rapid test, use `targetName="TEST"` and `halfset=0`. If the dataset is not yet available in the benchmarkDir (defined in [defaultDataConfig.yaml](cesped%2Fconfigs%2FdefaultDataConfig.yaml),
-it will be automatically downloaded. Metadta (Euler angles, CTf,...) are stored using Relion starfile format, and images are stored as .mrcs stacks.
+it will be automatically downloaded. Metadata (Euler angles, CTF,...) are stored using Relion starfile format, and images are stored as .mrcs stacks.
 
 3. Use it as a regular dataset
 ```
 dl = DataLoader(dataset, batch_size=32)
 for batch in dl:
   iid, img, (rotMat, xyShiftAngs, confidence), metadata = batch
   
@@ -163,21 +135,33 @@
 cesped.default_configs_dir
 ```
 ### Train
 In order to train the model on one target, you run
 ```
 python -m cesped.trainEntry --data.halfset <HALFSET> --data.targetName <TARGETNAME> --trainer.default_root_dir <OUTDIR>
 ```
-with `<HALFSET>` 0 or 1 and `<TARGETNAME>` one of the list that can be found using `ParticlesDataset.getCESPEDEntries()`
-Some available targets include
-- TEST. A small subset of EMPIAR-11120
-- EMPIAR-10166.
-- EMPIAR-11120
-- EMPIAR-10280
-- EMPIAR-10409
+with `<HALFSET>` 0 or 1 and `<TARGETNAME>` one of the list that can be found using `ParticlesDataset.getCESPEDEntries()` 
+<br><br>
+The included targets are:
+
+
+| EMPIAR ID | Composition | Symmetry | Image Pixels | FSCR<sub>0.143</sub> (Å) | Masked FSCR<sub>0.143</sub> (Å) | # Particles |
+|-----------|-------------|----------|--------------|-------------------------|---------------------------------|-------------|
+| 10166     | Human 26S proteasome bound to the chemotherapeutic Oprozomib | C1 | 284 | 5.0 | 3.9 | 238631 |
+| 10786     | Substance P-Neurokinin Receptor G protein complexes (SP-NK1R-miniGs399) | C1 | 184 | 3.3 | 3.0* | 288659 |
+| 10280     | Calcium-bound TMEM16F in nanodisc with supplement of PIP2 | C2 | 182 | 3.6 | 3.0* | 459504 |
+| 11120     | M22 bound TSHR Gs 7TM G protein | C1 | 232 | 3.4 | 3.0* | 244973 |
+| 10647     | PKM2 in complex with L-threonine | D2 | 222 | 3.7 | 3.3 | 234956 |
+| 10409     | Replicating SARS-CoV-2 polymerase (Map 1) | C1 | 240 | 3.3 | 3.0* | 406001 |
+| 10374     | Human ABCG2 transporter with inhibitor MZ29 and 5D3-Fab | C2 | 216 | 3.7 | 3.0* | 323681 |
+
+`*` Nyquist Frequency at 1.5 Å/pixel; Resolution is estimated at the usual threshold 0.143.  
+Reported FSCR<sub>0.143</sub> values were obtained directly from the relion_refine logs while Masked FSCR<sub>0.143</sub> values were collected from the relion_postprocess logs.
+
+In addition, the entry TEST is a small subset of EMPIAR-11120
 
 Do not forget to change the configuration files or to provide different values via the command line or environmental 
 variables. In addition, `[--config CONFIG_NAME.yaml]` also allows overwriting the default values using (a/several) custom
 yaml file(s). Use `-h` to see the list of configurable parameters. Some of the most important ones are.
 - trainer.default_root_dir. Directory where the checkpoints and the logs will be saved, 
 from [defaultTrainerConfig.yaml](cesped%2Fconfigs%2FdefaultTrainerConfig.yaml)
 - optimizer.lr. The learning rate, from [defaultOptimizerConfig.yaml](cesped%2Fconfigs%2FdefaultOptimizerConfig.yaml)
@@ -199,19 +183,17 @@
 5. As before, evaluation can be computed if the predictions for the halfset 0 and halfset 1 were saved using the evaluateEntry script.
 ```
 python -m cesped.evaluateEntry  --predictionType SO3 --targetName 11120  \
 --half0PredsFname particles_preds_0.star  --half1PredsFname particles_preds_1.star \
 --n_cpus 12 --outdir evaluation/
 ```
 
-##API
-For API documentation run
-pdoc --http : .
-
+## API
 
+For API documentation check the [docs folder](https://rsanchezgarc.github.io/cesped/cesped/)
 
 
 ## Relion Singularity
 
 A singularity container for relion_reconstruct with MPI support can be built with the following command. 
 ```
 singularity build relionSingulary.sif relionSingulary.def
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cesped-24.4.2/README.md` & `cesped-24.4.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: cesped
+Version: 24.4.3
+Summary: Code utilities for the CESPED (Cryo-EM Supervised Pose Estimation Dataset) benchmark
+Home-page: https://github.com/rsanchezgarc/cesped
+Author: Ruben Sanchez-Garcia
+Author-email: ruben.sanchez-garcia@stats.ox.ac.uk
+Keywords: deep learning cryoem pose estimation
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: argParseFromDoc>=0.1.2
+Requires-Dist: e3nn>=0.5.1
+Requires-Dist: healpy>=1.16.5
+Requires-Dist: joblib>=1.3
+Requires-Dist: mrcfile<2.0.0,>=1.4.3
+Requires-Dist: numpy>=1.25.2
+Requires-Dist: omegaconf>=2.3.0
+Requires-Dist: pandas>=2.1.0
+Requires-Dist: pdoc3>=0.10.0
+Requires-Dist: psutil>=5.9.5
+Requires-Dist: lightning[pytorch-extra]<3.0.0,>=2.0.0
+Requires-Dist: requests>=2.31.0
+Requires-Dist: scipy>=1.11.2
+Requires-Dist: starfile>=0.4.12
+Requires-Dist: starstack>=0.2.0
+Requires-Dist: tensorboard>=2.12.1
+Requires-Dist: torch<3.0.0,>=2.0.0
+Requires-Dist: torchvision>=0.15.2
+
 # CESPED: Utilities for the Cryo-EM Supervised Pose Estimation Dataset
 
 CESPED, is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check our manuscript at https://arxiv.org/abs/2311.06194.
 
 ## Installation
 cesped has been tested on python 3.11. Installation should be automatic using pip
 ```
@@ -31,15 +60,15 @@
 2. Load a given entry
 ```
 targetName, halfset = listOfEntries[0] #We will work with the first entry only
 
 dataset = ParticlesDataset(targetName, halfset)
 ```
 For a rapid test, use `targetName="TEST"` and `halfset=0`. If the dataset is not yet available in the benchmarkDir (defined in [defaultDataConfig.yaml](cesped%2Fconfigs%2FdefaultDataConfig.yaml),
-it will be automatically downloaded. Metadta (Euler angles, CTf,...) are stored using Relion starfile format, and images are stored as .mrcs stacks.
+it will be automatically downloaded. Metadata (Euler angles, CTF,...) are stored using Relion starfile format, and images are stored as .mrcs stacks.
 
 3. Use it as a regular dataset
 ```
 dl = DataLoader(dataset, batch_size=32)
 for batch in dl:
   iid, img, (rotMat, xyShiftAngs, confidence), metadata = batch
   
@@ -135,21 +164,33 @@
 cesped.default_configs_dir
 ```
 ### Train
 In order to train the model on one target, you run
 ```
 python -m cesped.trainEntry --data.halfset <HALFSET> --data.targetName <TARGETNAME> --trainer.default_root_dir <OUTDIR>
 ```
-with `<HALFSET>` 0 or 1 and `<TARGETNAME>` one of the list that can be found using `ParticlesDataset.getCESPEDEntries()`
-Some available targets include
-- TEST. A small subset of EMPIAR-11120
-- EMPIAR-10166.
-- EMPIAR-11120
-- EMPIAR-10280
-- EMPIAR-10409
+with `<HALFSET>` 0 or 1 and `<TARGETNAME>` one of the list that can be found using `ParticlesDataset.getCESPEDEntries()` 
+<br><br>
+The included targets are:
+
+
+| EMPIAR ID | Composition | Symmetry | Image Pixels | FSCR<sub>0.143</sub> (Å) | Masked FSCR<sub>0.143</sub> (Å) | # Particles |
+|-----------|-------------|----------|--------------|-------------------------|---------------------------------|-------------|
+| 10166     | Human 26S proteasome bound to the chemotherapeutic Oprozomib | C1 | 284 | 5.0 | 3.9 | 238631 |
+| 10786     | Substance P-Neurokinin Receptor G protein complexes (SP-NK1R-miniGs399) | C1 | 184 | 3.3 | 3.0* | 288659 |
+| 10280     | Calcium-bound TMEM16F in nanodisc with supplement of PIP2 | C2 | 182 | 3.6 | 3.0* | 459504 |
+| 11120     | M22 bound TSHR Gs 7TM G protein | C1 | 232 | 3.4 | 3.0* | 244973 |
+| 10647     | PKM2 in complex with L-threonine | D2 | 222 | 3.7 | 3.3 | 234956 |
+| 10409     | Replicating SARS-CoV-2 polymerase (Map 1) | C1 | 240 | 3.3 | 3.0* | 406001 |
+| 10374     | Human ABCG2 transporter with inhibitor MZ29 and 5D3-Fab | C2 | 216 | 3.7 | 3.0* | 323681 |
+
+`*` Nyquist Frequency at 1.5 Å/pixel; Resolution is estimated at the usual threshold 0.143.  
+Reported FSCR<sub>0.143</sub> values were obtained directly from the relion_refine logs while Masked FSCR<sub>0.143</sub> values were collected from the relion_postprocess logs.
+
+In addition, the entry TEST is a small subset of EMPIAR-11120
 
 Do not forget to change the configuration files or to provide different values via the command line or environmental 
 variables. In addition, `[--config CONFIG_NAME.yaml]` also allows overwriting the default values using (a/several) custom
 yaml file(s). Use `-h` to see the list of configurable parameters. Some of the most important ones are.
 - trainer.default_root_dir. Directory where the checkpoints and the logs will be saved, 
 from [defaultTrainerConfig.yaml](cesped%2Fconfigs%2FdefaultTrainerConfig.yaml)
 - optimizer.lr. The learning rate, from [defaultOptimizerConfig.yaml](cesped%2Fconfigs%2FdefaultOptimizerConfig.yaml)
@@ -171,19 +212,17 @@
 5. As before, evaluation can be computed if the predictions for the halfset 0 and halfset 1 were saved using the evaluateEntry script.
 ```
 python -m cesped.evaluateEntry  --predictionType SO3 --targetName 11120  \
 --half0PredsFname particles_preds_0.star  --half1PredsFname particles_preds_1.star \
 --n_cpus 12 --outdir evaluation/
 ```
 
-##API
-For API documentation run
-pdoc --http : .
-
+## API
 
+For API documentation check the [docs folder](https://rsanchezgarc.github.io/cesped/cesped/)
 
 
 ## Relion Singularity
 
 A singularity container for relion_reconstruct with MPI support can be built with the following command. 
 ```
 singularity build relionSingulary.sif relionSingulary.def
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cesped-24.4.2/cesped/configs/defaultDataAugmentation.yaml` & `cesped-24.4.3/cesped/configs/defaultDataAugmentation.yaml`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/configs/defaultDataConfig.yaml` & `cesped-24.4.3/cesped/configs/defaultDataConfig.yaml`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/configs/defaultTrainerConfig.yaml` & `cesped-24.4.3/cesped/configs/defaultTrainerConfig.yaml`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/constants.py` & `cesped-24.4.3/cesped/constants.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/datamanager/augmentations.py` & `cesped-24.4.3/cesped/datamanager/augmentations.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/datamanager/ctf.py` & `cesped-24.4.3/cesped/datamanager/ctf.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/datamanager/plDataset.py` & `cesped-24.4.3/cesped/datamanager/plDataset.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/evaluateEntry.py` & `cesped-24.4.3/cesped/evaluateEntry.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/inferEntry.py` & `cesped-24.4.3/cesped/inferEntry.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/network/featureExtractors.py` & `cesped-24.4.3/cesped/network/featureExtractors.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/network/image2sphere.py` & `cesped-24.4.3/cesped/network/image2sphere.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/network/plModule.py` & `cesped-24.4.3/cesped/network/plModule.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/particlesDataset.py` & `cesped-24.4.3/cesped/particlesDataset.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/trainEntry.py` & `cesped-24.4.3/cesped/trainEntry.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/utils/angles.py` & `cesped-24.4.3/cesped/utils/angles.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/utils/anglesStats.py` & `cesped-24.4.3/cesped/utils/anglesStats.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/utils/cliBuilder.py` & `cesped-24.4.3/cesped/utils/cliBuilder.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/utils/fsc.py` & `cesped-24.4.3/cesped/utils/fsc.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/utils/gaussianFilters.py` & `cesped-24.4.3/cesped/utils/gaussianFilters.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/utils/tensors.py` & `cesped-24.4.3/cesped/utils/tensors.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/utils/volumeStats.py` & `cesped-24.4.3/cesped/utils/volumeStats.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped/zenodo/bechmarkUrls.py` & `cesped-24.4.3/cesped/zenodo/bechmarkUrls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 ROOT_URL_PATTERN="https://zenodo.org/api/records/"
 
 NAME_PARTITION_TO_RECORID ={
-    ("TEST", 0): "8363635",
-    ("TEST", 1): "8363677",
+    ("TEST", 0): "10998049",
+    ("TEST", 1): "10998591",
 
     ("10786", 0): "8352275",
     ("10786", 1): "8352281",
 
     ("11120", 0): "8352296",
     ("11120", 1): "8352300",
 
@@ -26,21 +26,21 @@
     ("10409", 0): "8386582",
     ("10409", 1): "8386660",
 
 }
 
 _masks_base_url = "https://zenodo.org/record/8392782/files/"
 NAME_TO_MASK_URL={
-    "TEST":  f"{_masks_base_url}/10166_mask.mrc",
+    "TEST":  f"{_masks_base_url}/11120_mask.mrc",
     "10166": f"{_masks_base_url}/10166_mask.mrc",
 
     "10647": f"{_masks_base_url}/10647_mask.mrc",
     "astex-5534": f"{_masks_base_url}/10647_mask.mrc",
 
     "10280": f"{_masks_base_url}/10280_mask.mrc",
     "10786": f"{_masks_base_url}/10786_mask.mrc",
     "10409": f"{_masks_base_url}/10409_mask.mrc",
     "11120": f"{_masks_base_url}/11120_mask.mrc",
 
     "10374": f"{_masks_base_url}/10374_mask.mrc",
 
-}
+}
```

### Comparing `cesped-24.4.2/cesped/zenodo/downloadFromZenodo.py` & `cesped-24.4.3/cesped/zenodo/downloadFromZenodo.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,29 @@
 from tqdm import tqdm
 
 from cesped.zenodo.bechmarkUrls import ROOT_URL_PATTERN, NAME_TO_MASK_URL
 
 
 def getDoneFname(destination_dir, record_id):
     return os.path.join(destination_dir, f"SUCCESSFUL_DOWNLOAD_{record_id}.txt")
-def download_record(record_id, destination_dir, root_url=ROOT_URL_PATTERN):
+def download_record(record_id:str, destination_dir:str, root_url:str=ROOT_URL_PATTERN):
+    """
+
+    @param record_id:
+    @param destination_dir:
+    @param root_url:
+
+    """
 
     donefname = getDoneFname(destination_dir, record_id)
     if os.path.isfile(donefname):
         return
     root_url = f"{root_url}/{record_id}"
     r = requests.get(root_url)
-    assert r.status_code == 200, f"Error, bad request response {r}"
+    assert r.status_code == 200, f"Error, bad request response {r} for {root_url}"
     # print(r.json())
     os.makedirs(destination_dir, exist_ok=True)
 
 
     def check_checksum(content, expected_checksum):
         m = md5()
         m.update(content)
@@ -136,8 +143,12 @@
     assert response.status_code == 200, (f"Error downloading mask {mask_url}. {response} If you cannot download it "
                                          f"after retrying, place a "
                                          f"mask named {os.path.basename(mask_fname)} "
                                          f"on {os.path.split(mask_fname)[0]}")
     with tempfile.NamedTemporaryFile() as tmpf:
         for chunk in response.iter_content(chunk_size=100 * 1024 * 2):  # 100MB chunks
             tmpf.write(chunk)
-        shutil.copyfile(tmpf.name, mask_fname)
+        shutil.copyfile(tmpf.name, mask_fname)
+
+if __name__ == "__main__":
+    from argParseFromDoc import parse_function_and_call
+    parse_function_and_call(download_record)
```

### Comparing `cesped-24.4.2/cesped/zenodo/uploadToZenodo.py` & `cesped-24.4.3/cesped/zenodo/uploadToZenodo.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/cesped.egg-info/PKG-INFO` & `cesped-24.4.3/cesped.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesped
-Version: 24.4.2
+Version: 24.4.3
 Summary: Code utilities for the CESPED (Cryo-EM Supervised Pose Estimation Dataset) benchmark
 Home-page: https://github.com/rsanchezgarc/cesped
 Author: Ruben Sanchez-Garcia
 Author-email: ruben.sanchez-garcia@stats.ox.ac.uk
 Keywords: deep learning cryoem pose estimation
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,14 +13,15 @@
 Requires-Dist: healpy>=1.16.5
 Requires-Dist: joblib>=1.3
 Requires-Dist: mrcfile<2.0.0,>=1.4.3
 Requires-Dist: numpy>=1.25.2
 Requires-Dist: omegaconf>=2.3.0
 Requires-Dist: pandas>=2.1.0
 Requires-Dist: pdoc3>=0.10.0
+Requires-Dist: psutil>=5.9.5
 Requires-Dist: lightning[pytorch-extra]<3.0.0,>=2.0.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: scipy>=1.11.2
 Requires-Dist: starfile>=0.4.12
 Requires-Dist: starstack>=0.2.0
 Requires-Dist: tensorboard>=2.12.1
 Requires-Dist: torch<3.0.0,>=2.0.0
@@ -59,15 +60,15 @@
 2. Load a given entry
 ```
 targetName, halfset = listOfEntries[0] #We will work with the first entry only
 
 dataset = ParticlesDataset(targetName, halfset)
 ```
 For a rapid test, use `targetName="TEST"` and `halfset=0`. If the dataset is not yet available in the benchmarkDir (defined in [defaultDataConfig.yaml](cesped%2Fconfigs%2FdefaultDataConfig.yaml),
-it will be automatically downloaded. Metadta (Euler angles, CTf,...) are stored using Relion starfile format, and images are stored as .mrcs stacks.
+it will be automatically downloaded. Metadata (Euler angles, CTF,...) are stored using Relion starfile format, and images are stored as .mrcs stacks.
 
 3. Use it as a regular dataset
 ```
 dl = DataLoader(dataset, batch_size=32)
 for batch in dl:
   iid, img, (rotMat, xyShiftAngs, confidence), metadata = batch
   
@@ -163,21 +164,33 @@
 cesped.default_configs_dir
 ```
 ### Train
 In order to train the model on one target, you run
 ```
 python -m cesped.trainEntry --data.halfset <HALFSET> --data.targetName <TARGETNAME> --trainer.default_root_dir <OUTDIR>
 ```
-with `<HALFSET>` 0 or 1 and `<TARGETNAME>` one of the list that can be found using `ParticlesDataset.getCESPEDEntries()`
-Some available targets include
-- TEST. A small subset of EMPIAR-11120
-- EMPIAR-10166.
-- EMPIAR-11120
-- EMPIAR-10280
-- EMPIAR-10409
+with `<HALFSET>` 0 or 1 and `<TARGETNAME>` one of the list that can be found using `ParticlesDataset.getCESPEDEntries()` 
+<br><br>
+The included targets are:
+
+
+| EMPIAR ID | Composition | Symmetry | Image Pixels | FSCR<sub>0.143</sub> (Å) | Masked FSCR<sub>0.143</sub> (Å) | # Particles |
+|-----------|-------------|----------|--------------|-------------------------|---------------------------------|-------------|
+| 10166     | Human 26S proteasome bound to the chemotherapeutic Oprozomib | C1 | 284 | 5.0 | 3.9 | 238631 |
+| 10786     | Substance P-Neurokinin Receptor G protein complexes (SP-NK1R-miniGs399) | C1 | 184 | 3.3 | 3.0* | 288659 |
+| 10280     | Calcium-bound TMEM16F in nanodisc with supplement of PIP2 | C2 | 182 | 3.6 | 3.0* | 459504 |
+| 11120     | M22 bound TSHR Gs 7TM G protein | C1 | 232 | 3.4 | 3.0* | 244973 |
+| 10647     | PKM2 in complex with L-threonine | D2 | 222 | 3.7 | 3.3 | 234956 |
+| 10409     | Replicating SARS-CoV-2 polymerase (Map 1) | C1 | 240 | 3.3 | 3.0* | 406001 |
+| 10374     | Human ABCG2 transporter with inhibitor MZ29 and 5D3-Fab | C2 | 216 | 3.7 | 3.0* | 323681 |
+
+`*` Nyquist Frequency at 1.5 Å/pixel; Resolution is estimated at the usual threshold 0.143.  
+Reported FSCR<sub>0.143</sub> values were obtained directly from the relion_refine logs while Masked FSCR<sub>0.143</sub> values were collected from the relion_postprocess logs.
+
+In addition, the entry TEST is a small subset of EMPIAR-11120
 
 Do not forget to change the configuration files or to provide different values via the command line or environmental 
 variables. In addition, `[--config CONFIG_NAME.yaml]` also allows overwriting the default values using (a/several) custom
 yaml file(s). Use `-h` to see the list of configurable parameters. Some of the most important ones are.
 - trainer.default_root_dir. Directory where the checkpoints and the logs will be saved, 
 from [defaultTrainerConfig.yaml](cesped%2Fconfigs%2FdefaultTrainerConfig.yaml)
 - optimizer.lr. The learning rate, from [defaultOptimizerConfig.yaml](cesped%2Fconfigs%2FdefaultOptimizerConfig.yaml)
@@ -199,19 +212,17 @@
 5. As before, evaluation can be computed if the predictions for the halfset 0 and halfset 1 were saved using the evaluateEntry script.
 ```
 python -m cesped.evaluateEntry  --predictionType SO3 --targetName 11120  \
 --half0PredsFname particles_preds_0.star  --half1PredsFname particles_preds_1.star \
 --n_cpus 12 --outdir evaluation/
 ```
 
-##API
-For API documentation run
-pdoc --http : .
-
+## API
 
+For API documentation check the [docs folder](https://rsanchezgarc.github.io/cesped/cesped/)
 
 
 ## Relion Singularity
 
 A singularity container for relion_reconstruct with MPI support can be built with the following command. 
 ```
 singularity build relionSingulary.sif relionSingulary.def
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cesped-24.4.2/cesped.egg-info/SOURCES.txt` & `cesped-24.4.3/cesped.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,11 +36,12 @@
 cesped/utils/fsc.py
 cesped/utils/gaussianFilters.py
 cesped/utils/tensors.py
 cesped/utils/volumeStats.py
 cesped/zenodo/__init__.py
 cesped/zenodo/bechmarkUrls.py
 cesped/zenodo/downloadFromZenodo.py
+cesped/zenodo/tokens.py
 cesped/zenodo/uploadToZenodo.py
 tests/__init__.py
 tests/test_anglesStats.py
 tests/test_particlesDataset.py
```

### Comparing `cesped-24.4.2/setup.py` & `cesped-24.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/tests/test_anglesStats.py` & `cesped-24.4.3/tests/test_anglesStats.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.2/tests/test_particlesDataset.py` & `cesped-24.4.3/tests/test_particlesDataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     def test__download(self):
         ds = ParticlesDataset(testTargetName, 0, benchmarkDir=benchmarkDir)
         print(len(ds))
         ds = ParticlesDataset(testTargetName, 1, benchmarkDir=benchmarkDir)
         print(len(ds))
         iid, img, (rotMat, xyShiftAngs, confidence), metadata = ds[0]
         print([x.shape for x in [img, rotMat, xyShiftAngs]])
-        self.assertEqual(img.shape, (1, 284,284))
+        self.assertEqual(img.shape, (1, 232,232))
 
     def test_addNewEntry(self):
         ds = ParticlesDataset(testTargetName, 0, benchmarkDir=benchmarkDir)
         starFname = ds.starFname
         newTargetName="NewTarget_test_registerNewEntry"
         newTargetDir = os.path.join(benchmarkDir, newTargetName)
         if os.path.exists(newTargetDir):
             shutil.rmtree(newTargetDir)
         ParticlesDataset.addNewEntryLocally(starFname, particlesRootDir=os.path.split(starFname)[0],
                                             newTargetName=newTargetName, halfset=0, symmetry=ds.symmetry,
                                             benchmarkDir=benchmarkDir)
         ds = ParticlesDataset(newTargetName, 0, benchmarkDir=benchmarkDir)
         print(len(ds))
-        print(ParticlesDataset.getLocallyAvailableEntries(benchmarkDir))
+        print(ParticlesDataset.getLocallyAvailableEntries(benchmarkDir))
```

