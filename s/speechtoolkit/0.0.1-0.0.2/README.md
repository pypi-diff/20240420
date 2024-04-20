# Comparing `tmp/speechtoolkit-0.0.1.tar.gz` & `tmp/speechtoolkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechtoolkit-0.0.1.tar", last modified: Sat Apr 20 00:49:22 2024, max compression
+gzip compressed data, was "speechtoolkit-0.0.2.tar", last modified: Sat Apr 20 18:27:52 2024, max compression
```

## Comparing `speechtoolkit-0.0.1.tar` & `speechtoolkit-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.415701 speechtoolkit-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-20 00:49:22.415701 speechtoolkit-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 00:49:22.415701 speechtoolkit-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.411701 speechtoolkit-0.0.1/speechtoolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.411701 speechtoolkit-0.0.1/speechtoolkit/asr/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/asr/distilwhisper_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/asr/whisper_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.411701 speechtoolkit-0.0.1/speechtoolkit/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/classification/accentclassification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/classification/languageclassification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.411701 speechtoolkit-0.0.1/speechtoolkit/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/data/languages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.415701 speechtoolkit-0.0.1/speechtoolkit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/utils/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.415701 speechtoolkit-0.0.1/speechtoolkit/vc/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/vc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/vc/lvc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-20 00:49:05.000000 speechtoolkit-0.0.1/speechtoolkit/vc/ns3vc_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:49:22.415701 speechtoolkit-0.0.1/speechtoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-20 00:49:22.000000 speechtoolkit-0.0.1/speechtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-20 00:49:22.000000 speechtoolkit-0.0.1/speechtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 00:49:22.000000 speechtoolkit-0.0.1/speechtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-20 00:49:22.000000 speechtoolkit-0.0.1/speechtoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 00:49:22.000000 speechtoolkit-0.0.1/speechtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.391742 speechtoolkit-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-20 18:27:52.391742 speechtoolkit-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:27:52.391742 speechtoolkit-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.383741 speechtoolkit-0.0.2/speechtoolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit/asr/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/asr/distilwhisper_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/asr/whisper_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/classification/accentclassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/classification/languageclassification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/data/languages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/tts/styletts2_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/utils/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit/vc/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/vc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/vc/lvc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/vc/ns3vc_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-20 18:27:52.000000 speechtoolkit-0.0.2/speechtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-20 18:27:52.000000 speechtoolkit-0.0.2/speechtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:27:52.000000 speechtoolkit-0.0.2/speechtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-20 18:27:52.000000 speechtoolkit-0.0.2/speechtoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 18:27:52.000000 speechtoolkit-0.0.2/speechtoolkit.egg-info/top_level.txt
```

### Comparing `speechtoolkit-0.0.1/setup.py` & `speechtoolkit-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from setuptools import setup, find_packages
 
 extras = {
     "vc": [
         "lvc",
         "ns3vc",
     ],
-    "fa2": ["flash-attn"],
+    "fa2": [
+        "flash-attn",
+    ],
     "asr": [
         "openai-whisper",
     ],
+    "tts": [
+        "mfs-styletts2",
+    ],
     "dev": [
         "mkdocs",
         "mkautodoc",
     ],
 }
 
 extra_pkgs = extras
@@ -24,23 +29,24 @@
 
 extra_pkgs["all"] = final
 
 with open("README.md", "r") as f:
     longdesc = f.read()
 setup(
     name="speechtoolkit",
-    version="0.0.1",
+    version="0.0.2",
     author="ml-for-speech",
     description="ML for Speech presents SpeechToolkit, a unified, all-in-one toolkit for TTS, ASR, VC, & other models.",
     long_description=longdesc,
     long_description_content_type="text/markdown",
     url="https://github.com/ml-for-speech/speechtoolkit",
     packages=find_packages(),
     install_requires=[
         "soundfile",
         "librosa",
-        "torch",
         "transformers",
+        "torch",
         "optimum",
+        "txtsplit",
     ],
     extras_require=extra_pkgs,
 )
```

### Comparing `speechtoolkit-0.0.1/speechtoolkit/asr/distilwhisper_lib.py` & `speechtoolkit-0.0.2/speechtoolkit/asr/distilwhisper_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.1/speechtoolkit/asr/whisper_lib.py` & `speechtoolkit-0.0.2/speechtoolkit/asr/whisper_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.1/speechtoolkit/classification/accentclassification.py` & `speechtoolkit-0.0.2/speechtoolkit/classification/accentclassifier.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.1/speechtoolkit/classification/languageclassification.py` & `speechtoolkit-0.0.2/speechtoolkit/classification/languageclassification.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.1/speechtoolkit/data/languages.py` & `speechtoolkit-0.0.2/speechtoolkit/data/languages.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.1/speechtoolkit/vc/lvc_lib.py` & `speechtoolkit-0.0.2/speechtoolkit/vc/lvc_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.1/speechtoolkit/vc/ns3vc_lib.py` & `speechtoolkit-0.0.2/speechtoolkit/vc/ns3vc_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.1/speechtoolkit.egg-info/SOURCES.txt` & `speechtoolkit-0.0.2/speechtoolkit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 speechtoolkit.egg-info/dependency_links.txt
 speechtoolkit.egg-info/requires.txt
 speechtoolkit.egg-info/top_level.txt
 speechtoolkit/asr/__init__.py
 speechtoolkit/asr/distilwhisper_lib.py
 speechtoolkit/asr/whisper_lib.py
 speechtoolkit/classification/__init__.py
-speechtoolkit/classification/accentclassification.py
+speechtoolkit/classification/accentclassifier.py
 speechtoolkit/classification/languageclassification.py
 speechtoolkit/data/__init__.py
 speechtoolkit/data/languages.py
+speechtoolkit/tts/__init__.py
+speechtoolkit/tts/styletts2_lib.py
 speechtoolkit/utils/__init__.py
 speechtoolkit/utils/device.py
 speechtoolkit/vc/__init__.py
 speechtoolkit/vc/lvc_lib.py
 speechtoolkit/vc/ns3vc_lib.py
```

