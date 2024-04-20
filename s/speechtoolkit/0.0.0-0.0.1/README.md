# Comparing `tmp/speechtoolkit-0.0.0.tar.gz` & `tmp/speechtoolkit-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechtoolkit-0.0.0.tar", last modified: Sat Apr 20 00:40:40 2024, max compression
+gzip compressed data, was "speechtoolkit-0.0.1.tar", last modified: Sat Apr 20 00:49:22 2024, max compression
```

## Comparing `speechtoolkit-0.0.0.tar` & `speechtoolkit-0.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 00:40:40.482674 speechtoolkit-0.0.0/
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1458 2024-04-20 00:40:40.482163 speechtoolkit-0.0.0/PKG-INFO
--rw-r--r--   0 benjaminlee   (501) staff       (20)      552 2024-04-19 21:48:37.000000 speechtoolkit-0.0.0/README.md
--rw-r--r--   0 benjaminlee   (501) staff       (20)       38 2024-04-20 00:40:40.482799 speechtoolkit-0.0.0/setup.cfg
--rw-r--r--   0 benjaminlee   (501) staff       (20)      968 2024-04-19 23:37:03.000000 speechtoolkit-0.0.0/setup.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 00:40:40.475134 speechtoolkit-0.0.0/speechtoolkit/
--rw-r--r--   0 benjaminlee   (501) staff       (20)        0 2024-04-19 20:24:21.000000 speechtoolkit-0.0.0/speechtoolkit/__init__.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 00:40:40.477384 speechtoolkit-0.0.0/speechtoolkit/asr/
--rw-r--r--   0 benjaminlee   (501) staff       (20)      122 2024-04-19 23:40:34.000000 speechtoolkit-0.0.0/speechtoolkit/asr/__init__.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     2644 2024-04-19 23:51:08.000000 speechtoolkit-0.0.0/speechtoolkit/asr/distilwhisper_lib.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1172 2024-04-19 23:51:08.000000 speechtoolkit-0.0.0/speechtoolkit/asr/whisper_lib.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 00:40:40.479135 speechtoolkit-0.0.0/speechtoolkit/classification/
--rw-r--r--   0 benjaminlee   (501) staff       (20)        0 2024-04-19 22:18:51.000000 speechtoolkit-0.0.0/speechtoolkit/classification/__init__.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1396 2024-04-20 00:09:10.000000 speechtoolkit-0.0.0/speechtoolkit/classification/accentclassification.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1375 2024-04-20 00:07:07.000000 speechtoolkit-0.0.0/speechtoolkit/classification/languageclassification.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 00:40:40.479684 speechtoolkit-0.0.0/speechtoolkit/data/
--rw-r--r--   0 benjaminlee   (501) staff       (20)        0 2024-04-19 22:23:23.000000 speechtoolkit-0.0.0/speechtoolkit/data/__init__.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1016 2024-04-19 22:22:41.000000 speechtoolkit-0.0.0/speechtoolkit/data/languages.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 00:40:40.480145 speechtoolkit-0.0.0/speechtoolkit/utils/
--rw-r--r--   0 benjaminlee   (501) staff       (20)        0 2024-04-19 22:23:26.000000 speechtoolkit-0.0.0/speechtoolkit/utils/__init__.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)      212 2024-04-19 23:17:11.000000 speechtoolkit-0.0.0/speechtoolkit/utils/device.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 00:40:40.480835 speechtoolkit-0.0.0/speechtoolkit/vc/
--rw-r--r--   0 benjaminlee   (501) staff       (20)       96 2024-04-19 23:17:11.000000 speechtoolkit-0.0.0/speechtoolkit/vc/__init__.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1402 2024-04-19 23:42:52.000000 speechtoolkit-0.0.0/speechtoolkit/vc/lvc_lib.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1125 2024-04-19 23:42:52.000000 speechtoolkit-0.0.0/speechtoolkit/vc/ns3vc_lib.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 00:40:40.476301 speechtoolkit-0.0.0/speechtoolkit.egg-info/
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1458 2024-04-20 00:40:40.000000 speechtoolkit-0.0.0/speechtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 benjaminlee   (501) staff       (20)      691 2024-04-20 00:40:40.000000 speechtoolkit-0.0.0/speechtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)        1 2024-04-20 00:40:40.000000 speechtoolkit-0.0.0/speechtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)      168 2024-04-20 00:40:40.000000 speechtoolkit-0.0.0/speechtoolkit.egg-info/requires.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)       14 2024-04-20 00:40:40.000000 speechtoolkit-0.0.0/speechtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.415701 speechtoolkit-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-20 00:49:22.415701 speechtoolkit-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 00:49:22.415701 speechtoolkit-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.411701 speechtoolkit-0.0.1/speechtoolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.411701 speechtoolkit-0.0.1/speechtoolkit/asr/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/asr/distilwhisper_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/asr/whisper_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.411701 speechtoolkit-0.0.1/speechtoolkit/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/classification/accentclassification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/classification/languageclassification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.411701 speechtoolkit-0.0.1/speechtoolkit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/data/languages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.415701 speechtoolkit-0.0.1/speechtoolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/utils/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.415701 speechtoolkit-0.0.1/speechtoolkit/vc/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/vc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/vc/lvc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/vc/ns3vc_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.415701 speechtoolkit-0.0.1/speechtoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-20 00:49:22.000000 speechtoolkit-0.0.1/speechtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-20 00:49:22.000000 speechtoolkit-0.0.1/speechtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 00:49:22.000000 speechtoolkit-0.0.1/speechtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-20 00:49:22.000000 speechtoolkit-0.0.1/speechtoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 00:49:22.000000 speechtoolkit-0.0.1/speechtoolkit.egg-info/top_level.txt
```

### Comparing `speechtoolkit-0.0.0/PKG-INFO` & `speechtoolkit-0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtoolkit
-Version: 0.0.0
+Version: 0.0.1
 Summary: ML for Speech presents SpeechToolkit, a unified, all-in-one toolkit for TTS, ASR, VC, & other models.
 Home-page: https://github.com/ml-for-speech/speechtoolkit
 Author: ml-for-speech
 Description-Content-Type: text/markdown
 Requires-Dist: soundfile
 Requires-Dist: librosa
 Requires-Dist: torch
@@ -24,16 +24,18 @@
 Requires-Dist: lvc; extra == "all"
 Requires-Dist: ns3vc; extra == "all"
 Requires-Dist: flash-attn; extra == "all"
 Requires-Dist: openai-whisper; extra == "all"
 
 # SpeechToolkit
 
+**NOTE: This project is still in an early alpha stage and is not ready for production yet.**
+
 ML for Speech presents SpeechToolkit, a unified framework for text-to-speech, voice conversion, automatic speech recognition, audio classification, voice activity detection, and more!
 
 Please note that this toolkit is currently in an early alpha and not all features have been implemented.
 
 If you prefer not to use SpeechToolkit but would like to interact with models individually and separately, please check out the [ML for Speech](https://github.com/ml-for-speech) page.
 
 ## Installation & Usage
 
-Documentation is available online.
+Documentation is available [online](https://ml-for-speech.github.io/speechtoolkit).
```

### Comparing `speechtoolkit-0.0.0/setup.py` & `speechtoolkit-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 extra_pkgs["all"] = final
 
 with open("README.md", "r") as f:
     longdesc = f.read()
 setup(
     name="speechtoolkit",
-    version="0.0.0",
+    version="0.0.1",
     author="ml-for-speech",
     description="ML for Speech presents SpeechToolkit, a unified, all-in-one toolkit for TTS, ASR, VC, & other models.",
     long_description=longdesc,
     long_description_content_type="text/markdown",
     url="https://github.com/ml-for-speech/speechtoolkit",
     packages=find_packages(),
     install_requires=[
```

### Comparing `speechtoolkit-0.0.0/speechtoolkit/asr/distilwhisper_lib.py` & `speechtoolkit-0.0.1/speechtoolkit/asr/distilwhisper_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.0/speechtoolkit/asr/whisper_lib.py` & `speechtoolkit-0.0.1/speechtoolkit/asr/whisper_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.0/speechtoolkit/classification/accentclassification.py` & `speechtoolkit-0.0.1/speechtoolkit/classification/accentclassification.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.0/speechtoolkit/classification/languageclassification.py` & `speechtoolkit-0.0.1/speechtoolkit/classification/languageclassification.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.0/speechtoolkit/data/languages.py` & `speechtoolkit-0.0.1/speechtoolkit/data/languages.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.0/speechtoolkit/vc/lvc_lib.py` & `speechtoolkit-0.0.1/speechtoolkit/vc/lvc_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.0/speechtoolkit/vc/ns3vc_lib.py` & `speechtoolkit-0.0.1/speechtoolkit/vc/ns3vc_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.0/speechtoolkit.egg-info/PKG-INFO` & `speechtoolkit-0.0.1/speechtoolkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtoolkit
-Version: 0.0.0
+Version: 0.0.1
 Summary: ML for Speech presents SpeechToolkit, a unified, all-in-one toolkit for TTS, ASR, VC, & other models.
 Home-page: https://github.com/ml-for-speech/speechtoolkit
 Author: ml-for-speech
 Description-Content-Type: text/markdown
 Requires-Dist: soundfile
 Requires-Dist: librosa
 Requires-Dist: torch
@@ -24,16 +24,18 @@
 Requires-Dist: lvc; extra == "all"
 Requires-Dist: ns3vc; extra == "all"
 Requires-Dist: flash-attn; extra == "all"
 Requires-Dist: openai-whisper; extra == "all"
 
 # SpeechToolkit
 
+**NOTE: This project is still in an early alpha stage and is not ready for production yet.**
+
 ML for Speech presents SpeechToolkit, a unified framework for text-to-speech, voice conversion, automatic speech recognition, audio classification, voice activity detection, and more!
 
 Please note that this toolkit is currently in an early alpha and not all features have been implemented.
 
 If you prefer not to use SpeechToolkit but would like to interact with models individually and separately, please check out the [ML for Speech](https://github.com/ml-for-speech) page.
 
 ## Installation & Usage
 
-Documentation is available online.
+Documentation is available [online](https://ml-for-speech.github.io/speechtoolkit).
```

### Comparing `speechtoolkit-0.0.0/speechtoolkit.egg-info/SOURCES.txt` & `speechtoolkit-0.0.1/speechtoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

