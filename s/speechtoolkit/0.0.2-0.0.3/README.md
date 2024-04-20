# Comparing `tmp/speechtoolkit-0.0.2.tar.gz` & `tmp/speechtoolkit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechtoolkit-0.0.2.tar", last modified: Sat Apr 20 18:27:52 2024, max compression
+gzip compressed data, was "speechtoolkit-0.0.3.tar", last modified: Sat Apr 20 18:30:24 2024, max compression
```

## Comparing `speechtoolkit-0.0.2.tar` & `speechtoolkit-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.391742 speechtoolkit-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-20 18:27:52.391742 speechtoolkit-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:27:52.391742 speechtoolkit-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.383741 speechtoolkit-0.0.2/speechtoolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit/asr/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/asr/distilwhisper_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/asr/whisper_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/classification/accentclassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/classification/languageclassification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/data/languages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit/tts/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/tts/styletts2_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/utils/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit/vc/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/vc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/vc/lvc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-20 18:27:43.000000 speechtoolkit-0.0.2/speechtoolkit/vc/ns3vc_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:27:52.387742 speechtoolkit-0.0.2/speechtoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-20 18:27:52.000000 speechtoolkit-0.0.2/speechtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-20 18:27:52.000000 speechtoolkit-0.0.2/speechtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:27:52.000000 speechtoolkit-0.0.2/speechtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-20 18:27:52.000000 speechtoolkit-0.0.2/speechtoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 18:27:52.000000 speechtoolkit-0.0.2/speechtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 18:30:24.810075 speechtoolkit-0.0.3/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     3057 2024-04-20 18:30:24.809740 speechtoolkit-0.0.3/PKG-INFO
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     2018 2024-04-20 18:27:37.000000 speechtoolkit-0.0.3/README.md
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       38 2024-04-20 18:30:24.810163 speechtoolkit-0.0.3/setup.cfg
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1043 2024-04-20 18:30:18.000000 speechtoolkit-0.0.3/setup.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 18:30:24.804640 speechtoolkit-0.0.3/speechtoolkit/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)        0 2024-04-19 20:24:21.000000 speechtoolkit-0.0.3/speechtoolkit/__init__.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 18:30:24.806456 speechtoolkit-0.0.3/speechtoolkit/asr/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      122 2024-04-19 23:40:34.000000 speechtoolkit-0.0.3/speechtoolkit/asr/__init__.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     2644 2024-04-19 23:51:08.000000 speechtoolkit-0.0.3/speechtoolkit/asr/distilwhisper_lib.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1172 2024-04-19 23:51:08.000000 speechtoolkit-0.0.3/speechtoolkit/asr/whisper_lib.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 18:30:24.806979 speechtoolkit-0.0.3/speechtoolkit/classification/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)        0 2024-04-19 22:18:51.000000 speechtoolkit-0.0.3/speechtoolkit/classification/__init__.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1396 2024-04-20 00:09:10.000000 speechtoolkit-0.0.3/speechtoolkit/classification/accentclassifier.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1375 2024-04-20 00:07:07.000000 speechtoolkit-0.0.3/speechtoolkit/classification/languageclassification.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 18:30:24.807325 speechtoolkit-0.0.3/speechtoolkit/data/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)        0 2024-04-19 22:23:23.000000 speechtoolkit-0.0.3/speechtoolkit/data/__init__.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1016 2024-04-19 22:22:41.000000 speechtoolkit-0.0.3/speechtoolkit/data/languages.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 18:30:24.807722 speechtoolkit-0.0.3/speechtoolkit/tts/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       82 2024-04-20 02:16:32.000000 speechtoolkit-0.0.3/speechtoolkit/tts/__init__.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     3129 2024-04-20 02:20:11.000000 speechtoolkit-0.0.3/speechtoolkit/tts/styletts2_lib.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 18:30:24.808071 speechtoolkit-0.0.3/speechtoolkit/utils/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)        0 2024-04-19 22:23:26.000000 speechtoolkit-0.0.3/speechtoolkit/utils/__init__.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      212 2024-04-19 23:17:11.000000 speechtoolkit-0.0.3/speechtoolkit/utils/device.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 18:30:24.808643 speechtoolkit-0.0.3/speechtoolkit/vc/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       96 2024-04-19 23:17:11.000000 speechtoolkit-0.0.3/speechtoolkit/vc/__init__.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1402 2024-04-19 23:42:52.000000 speechtoolkit-0.0.3/speechtoolkit/vc/lvc_lib.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1125 2024-04-19 23:42:52.000000 speechtoolkit-0.0.3/speechtoolkit/vc/ns3vc_lib.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-20 18:30:24.805854 speechtoolkit-0.0.3/speechtoolkit.egg-info/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     3057 2024-04-20 18:30:24.000000 speechtoolkit-0.0.3/speechtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      752 2024-04-20 18:30:24.000000 speechtoolkit-0.0.3/speechtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)        1 2024-04-20 18:30:24.000000 speechtoolkit-0.0.3/speechtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      212 2024-04-20 18:30:24.000000 speechtoolkit-0.0.3/speechtoolkit.egg-info/requires.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       14 2024-04-20 18:30:24.000000 speechtoolkit-0.0.3/speechtoolkit.egg-info/top_level.txt
```

### Comparing `speechtoolkit-0.0.2/PKG-INFO` & `speechtoolkit-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtoolkit
-Version: 0.0.2
+Version: 0.0.3
 Summary: ML for Speech presents SpeechToolkit, a unified, all-in-one toolkit for TTS, ASR, VC, & other models.
 Home-page: https://github.com/ml-for-speech/speechtoolkit
 Author: ml-for-speech
 Description-Content-Type: text/markdown
 Requires-Dist: soundfile
 Requires-Dist: librosa
 Requires-Dist: transformers
```

### Comparing `speechtoolkit-0.0.2/README.md` & `speechtoolkit-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.2/setup.py` & `speechtoolkit-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,23 +21,23 @@
 }
 
 extra_pkgs = extras
 final = []
 
 for k in extras:
     if not k == "dev":
-        final.append(extras[k])
+        final += extras[k]
 
 extra_pkgs["all"] = final
 
 with open("README.md", "r") as f:
     longdesc = f.read()
 setup(
     name="speechtoolkit",
-    version="0.0.2",
+    version="0.0.3",
     author="ml-for-speech",
     description="ML for Speech presents SpeechToolkit, a unified, all-in-one toolkit for TTS, ASR, VC, & other models.",
     long_description=longdesc,
     long_description_content_type="text/markdown",
     url="https://github.com/ml-for-speech/speechtoolkit",
     packages=find_packages(),
     install_requires=[
```

### Comparing `speechtoolkit-0.0.2/speechtoolkit/asr/distilwhisper_lib.py` & `speechtoolkit-0.0.3/speechtoolkit/asr/distilwhisper_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.2/speechtoolkit/asr/whisper_lib.py` & `speechtoolkit-0.0.3/speechtoolkit/asr/whisper_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.2/speechtoolkit/classification/accentclassifier.py` & `speechtoolkit-0.0.3/speechtoolkit/classification/accentclassifier.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.2/speechtoolkit/classification/languageclassification.py` & `speechtoolkit-0.0.3/speechtoolkit/classification/languageclassification.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.2/speechtoolkit/data/languages.py` & `speechtoolkit-0.0.3/speechtoolkit/data/languages.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.2/speechtoolkit/tts/styletts2_lib.py` & `speechtoolkit-0.0.3/speechtoolkit/tts/styletts2_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.2/speechtoolkit/vc/lvc_lib.py` & `speechtoolkit-0.0.3/speechtoolkit/vc/lvc_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.2/speechtoolkit/vc/ns3vc_lib.py` & `speechtoolkit-0.0.3/speechtoolkit/vc/ns3vc_lib.py`

 * *Files identical despite different names*

### Comparing `speechtoolkit-0.0.2/speechtoolkit.egg-info/PKG-INFO` & `speechtoolkit-0.0.3/speechtoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtoolkit
-Version: 0.0.2
+Version: 0.0.3
 Summary: ML for Speech presents SpeechToolkit, a unified, all-in-one toolkit for TTS, ASR, VC, & other models.
 Home-page: https://github.com/ml-for-speech/speechtoolkit
 Author: ml-for-speech
 Description-Content-Type: text/markdown
 Requires-Dist: soundfile
 Requires-Dist: librosa
 Requires-Dist: transformers
```

### Comparing `speechtoolkit-0.0.2/speechtoolkit.egg-info/SOURCES.txt` & `speechtoolkit-0.0.3/speechtoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

