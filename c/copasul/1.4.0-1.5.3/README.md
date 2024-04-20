# Comparing `tmp/copasul-1.4.0.tar.gz` & `tmp/copasul-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copasul-1.4.0.tar", last modified: Mon Dec 11 15:24:38 2023, max compression
+gzip compressed data, was "copasul-1.5.3.tar", last modified: Sat Apr 20 17:55:20 2024, max compression
```

## Comparing `copasul-1.4.0.tar` & `copasul-1.5.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 ureichel (767601236) domain users (767600513)        0 2023-12-11 15:24:38.177340 copasul-1.4.0/
--rw-r--r--   0 ureichel (767601236) domain users (767600513)     1068 2023-05-16 11:51:34.000000 copasul-1.4.0/LICENSE
--rw-r--r--   0 ureichel (767601236) domain users (767600513)     4934 2023-12-11 15:24:38.177340 copasul-1.4.0/PKG-INFO
--rw-r--r--   0 ureichel (767601236) domain users (767600513)     4089 2023-12-11 09:34:24.000000 copasul-1.4.0/README.md
-drwxr-xr-x   0 ureichel (767601236) domain users (767600513)        0 2023-12-11 15:24:38.177340 copasul-1.4.0/copasul/
--rw-r--r--   0 ureichel (767601236) domain users (767600513)        0 2023-12-11 09:34:24.000000 copasul-1.4.0/copasul/__init__.py
--rw-r--r--   0 ureichel (767601236) domain users (767600513)     7807 2023-12-11 09:34:24.000000 copasul-1.4.0/copasul/copasul.py
--rw-r--r--   0 ureichel (767601236) domain users (767600513)    84998 2023-12-11 09:34:24.000000 copasul-1.4.0/copasul/copasul_augment.py
--rw-r--r--   0 ureichel (767601236) domain users (767600513)     4379 2023-12-11 09:34:24.000000 copasul-1.4.0/copasul/copasul_clst.py
--rw-r--r--   0 ureichel (767601236) domain users (767600513)    46463 2023-12-11 09:34:24.000000 copasul-1.4.0/copasul/copasul_export.py
--rw-r--r--   0 ureichel (767601236) domain users (767600513)    20701 2023-12-11 09:34:24.000000 copasul-1.4.0/copasul/copasul_init.py
--rw-r--r--   0 ureichel (767601236) domain users (767600513)    28166 2023-12-11 09:34:24.000000 copasul-1.4.0/copasul/copasul_plot.py
--rw-r--r--   0 ureichel (767601236) domain users (767600513)    65749 2023-12-11 12:39:04.000000 copasul-1.4.0/copasul/copasul_preproc.py
--rw-r--r--   0 ureichel (767601236) domain users (767600513)     2778 2023-12-11 09:34:24.000000 copasul-1.4.0/copasul/copasul_resyn.py
--rw-r--r--   0 ureichel (767601236) domain users (767600513)    40405 2023-12-11 12:39:04.000000 copasul-1.4.0/copasul/copasul_sigproc.py
--rw-r--r--   0 ureichel (767601236) domain users (767600513)    70905 2023-12-11 12:39:04.000000 copasul-1.4.0/copasul/copasul_styl.py
--rw-r--r--   0 ureichel (767601236) domain users (767600513)   107805 2023-12-11 12:39:04.000000 copasul-1.4.0/copasul/copasul_utils.py
-drwxr-xr-x   0 ureichel (767601236) domain users (767600513)        0 2023-12-11 15:24:38.177340 copasul-1.4.0/copasul.egg-info/
--rw-r--r--   0 ureichel (767601236) domain users (767600513)     4934 2023-12-11 15:24:38.000000 copasul-1.4.0/copasul.egg-info/PKG-INFO
--rw-r--r--   0 ureichel (767601236) domain users (767600513)      536 2023-12-11 15:24:38.000000 copasul-1.4.0/copasul.egg-info/SOURCES.txt
--rw-r--r--   0 ureichel (767601236) domain users (767600513)        1 2023-12-11 15:24:38.000000 copasul-1.4.0/copasul.egg-info/dependency_links.txt
--rw-r--r--   0 ureichel (767601236) domain users (767600513)       55 2023-12-11 15:24:38.000000 copasul-1.4.0/copasul.egg-info/requires.txt
--rw-r--r--   0 ureichel (767601236) domain users (767600513)        8 2023-12-11 15:24:38.000000 copasul-1.4.0/copasul.egg-info/top_level.txt
--rw-r--r--   0 ureichel (767601236) domain users (767600513)       94 2023-12-11 09:34:24.000000 copasul-1.4.0/pyproject.toml
--rw-r--r--   0 ureichel (767601236) domain users (767600513)      789 2023-12-11 15:24:38.177340 copasul-1.4.0/setup.cfg
--rw-r--r--   0 ureichel (767601236) domain users (767600513)       58 2023-12-11 09:34:24.000000 copasul-1.4.0/setup.py
-drwxr-xr-x   0 ureichel (767601236) domain users (767600513)        0 2023-12-11 15:24:38.177340 copasul-1.4.0/tests/
--rw-r--r--   0 ureichel (767601236) domain users (767600513)    18824 2023-12-11 09:34:24.000000 copasul-1.4.0/tests/tests_aug.py
--rw-r--r--   0 ureichel (767601236) domain users (767600513)     7322 2023-12-11 09:34:24.000000 copasul-1.4.0/tests/tests_styl.py
+drwxr-xr-x   0 ureichel (767601236) domain users (767600513)        0 2024-04-20 17:55:20.540751 copasul-1.5.3/
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)     1068 2023-05-16 11:51:34.000000 copasul-1.5.3/LICENSE
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)     5826 2024-04-20 17:55:20.540751 copasul-1.5.3/PKG-INFO
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)     4948 2024-04-20 17:15:43.000000 copasul-1.5.3/README.md
+drwxr-xr-x   0 ureichel (767601236) domain users (767600513)        0 2024-04-20 17:55:20.540751 copasul-1.5.3/copasul/
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)        0 2023-12-11 09:34:24.000000 copasul-1.5.3/copasul/__init__.py
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)     7807 2023-12-11 09:34:24.000000 copasul-1.5.3/copasul/copasul.py
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)    84998 2023-12-11 09:34:24.000000 copasul-1.5.3/copasul/copasul_augment.py
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)     4379 2023-12-11 09:34:24.000000 copasul-1.5.3/copasul/copasul_clst.py
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)    46463 2023-12-11 09:34:24.000000 copasul-1.5.3/copasul/copasul_export.py
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)    20701 2023-12-11 09:34:24.000000 copasul-1.5.3/copasul/copasul_init.py
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)    28166 2023-12-11 09:34:24.000000 copasul-1.5.3/copasul/copasul_plot.py
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)    65749 2023-12-11 12:39:04.000000 copasul-1.5.3/copasul/copasul_preproc.py
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)     2778 2023-12-11 09:34:24.000000 copasul-1.5.3/copasul/copasul_resyn.py
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)    40405 2023-12-11 12:39:04.000000 copasul-1.5.3/copasul/copasul_sigproc.py
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)    70905 2023-12-11 12:39:04.000000 copasul-1.5.3/copasul/copasul_styl.py
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)   107805 2023-12-11 12:39:04.000000 copasul-1.5.3/copasul/copasul_utils.py
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)    10550 2024-04-20 17:15:43.000000 copasul-1.5.3/copasul/praat_utils.py
+drwxr-xr-x   0 ureichel (767601236) domain users (767600513)        0 2024-04-20 17:55:20.540751 copasul-1.5.3/copasul.egg-info/
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)     5826 2024-04-20 17:55:20.000000 copasul-1.5.3/copasul.egg-info/PKG-INFO
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)      559 2024-04-20 17:55:20.000000 copasul-1.5.3/copasul.egg-info/SOURCES.txt
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)        1 2024-04-20 17:55:20.000000 copasul-1.5.3/copasul.egg-info/dependency_links.txt
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)       73 2024-04-20 17:55:20.000000 copasul-1.5.3/copasul.egg-info/requires.txt
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)        8 2024-04-20 17:55:20.000000 copasul-1.5.3/copasul.egg-info/top_level.txt
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)       94 2024-04-20 17:53:17.000000 copasul-1.5.3/pyproject.toml
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)      808 2024-04-20 17:55:20.540751 copasul-1.5.3/setup.cfg
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)       58 2023-12-11 09:34:24.000000 copasul-1.5.3/setup.py
+drwxr-xr-x   0 ureichel (767601236) domain users (767600513)        0 2024-04-20 17:55:20.540751 copasul-1.5.3/tests/
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)    18824 2023-12-11 09:34:24.000000 copasul-1.5.3/tests/tests_aug.py
+-rw-r--r--   0 ureichel (767601236) domain users (767600513)     7322 2023-12-11 09:34:24.000000 copasul-1.5.3/tests/tests_styl.py
```

### Comparing `copasul-1.4.0/LICENSE` & `copasul-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `copasul-1.4.0/PKG-INFO` & `copasul-1.5.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copasul
-Version: 1.4.0
+Version: 1.5.3
 Summary: Prosody stylization
 Home-page: https://github.com/reichelu/copasul
 Author: Uwe Reichel
 Author-email: uwe.reichel@nytud.mta.hu
 Project-URL: repository, https://github.com/reichelu/copasul
 Project-URL: documentation, https://github.com/reichelu/copasul
 Project-URL: article, https://arxiv.org/abs/1612.04765
@@ -16,14 +16,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: audeer
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: praat-parselmouth
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: tqdm
 
 # CoPaSul - Contour-based, parametric, and superpositional intonation stylization
 
 ## Author
@@ -71,25 +72,66 @@
 (venv_copasul) $ pip install -r requirements.txt
 ```
 
 ## Usage
 
 ### Required files
 * audio (wav), f0, pulse, and annotation files (Textgrid), see on GitHub: `tests/minex/input`
-    * f0 and pulse files can be generated with the help of the praat scripts on Github: `scripts/*praat`
 * a config file (json), see on GitHub `tests/minex/config/minex.json`
     * see on Github `docs/copasul_commented_config.json.txt` and the [article](https://arxiv.org/abs/1612.04765) for further details
 
-### Call from terminal (if cloned from GitHub)
+### Extract f0 and pulse by means of Praat
 
-* see on [GitHub project page](https://github.com/reichelu/copasul) `scripts/run_copasul.py [-c myConfigFile.json]`
-* `PROJECT_DIR`: directory where GitHub project has been cloned
+* see [example script](https://github.com/reichelu/copasul/scripts/run_praat.py)
+
+```python
+# add this line if you use the code from GitHub
+# sys.path.append(PROJECT_ROOT)
+
+from copasul import praat_utils
+
+# Praat pitch extractor
+piex = praat_utils.PraatPitchExtractor(
+    hopsize=0.01, minfreq=75, maxfreq=600)
+
+# process mono files
+piex.process_mono_files(
+    input_dir=INPUT_AUDIO_DIR,
+    output_dir=OUTPUT_PITCH_DIR,
+    input_ext="wav",
+    output_ext="f0"
+)
+
+# ... in order to process stereo files, use:
+# piex.process_stereo_files()
+
+# Praat pulse extractor
+puex = praat_utils.PraatPulseExtractor(
+    hopsize=0.01, minfreq=75, maxfreq=400)
+
+# process mono files
+puex.process_mono_files(
+    input_dir=INPUT_AUDIO_DIR,
+    output_dir=OUTPUT_PULSE_DIR,
+    input_ext="wav",
+    output_ext="pulse"
+)
+
+# ... in order to process stereo files, use:
+# puex.process_stereo_files()
+```
+
+### Call Copasul from terminal (if cloned from GitHub)
+
+* see on [example script](https://github.com/reichelu/copasul/scripts/run_copasul.py)
+* `python scripts/run_copasul.py [-c myConfigFile.json]`
+* `PROJECT_ROOT`: directory where GitHub project has been cloned
 
 ```bash
-(venv_copasul) $ cd PROJECT_DIR/scripts/
+(venv_copasul) $ cd PROJECT_ROOT/scripts/
 (venv_copasul) $ python run_copasul.py -c ../tests/minex/config/minex.json
 ```
 
 * if you use `../tests/minex/config/minex.json` as config file, CoPaSul
     * processes the files in `../tests/minex/input/`, and
     * outputs feature tables to `../tests/minex/output/test.FEATURESET.{csv, R}`
     * outputs the CoPaSul output dict to `../tests/minex/output/test.pickle`
@@ -99,16 +141,16 @@
 ### Example integration into python code
 
 ```python
 import json
 import pickle
 import sys
 
-# add this line if you use the cloned code from GitHub
-# sys.path.append(PROJECT_DIR)
+# add this line if you use the code from GitHub
+# sys.path.append(PROJECT_ROOT)
 
 from copasul import copasul
 
 # feature extractor
 fex = copasul.Copasul()
 
 # processing based on config file
```

### Comparing `copasul-1.4.0/README.md` & `copasul-1.5.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -45,25 +45,66 @@
 (venv_copasul) $ pip install -r requirements.txt
 ```
 
 ## Usage
 
 ### Required files
 * audio (wav), f0, pulse, and annotation files (Textgrid), see on GitHub: `tests/minex/input`
-    * f0 and pulse files can be generated with the help of the praat scripts on Github: `scripts/*praat`
 * a config file (json), see on GitHub `tests/minex/config/minex.json`
     * see on Github `docs/copasul_commented_config.json.txt` and the [article](https://arxiv.org/abs/1612.04765) for further details
 
-### Call from terminal (if cloned from GitHub)
+### Extract f0 and pulse by means of Praat
 
-* see on [GitHub project page](https://github.com/reichelu/copasul) `scripts/run_copasul.py [-c myConfigFile.json]`
-* `PROJECT_DIR`: directory where GitHub project has been cloned
+* see [example script](https://github.com/reichelu/copasul/scripts/run_praat.py)
+
+```python
+# add this line if you use the code from GitHub
+# sys.path.append(PROJECT_ROOT)
+
+from copasul import praat_utils
+
+# Praat pitch extractor
+piex = praat_utils.PraatPitchExtractor(
+    hopsize=0.01, minfreq=75, maxfreq=600)
+
+# process mono files
+piex.process_mono_files(
+    input_dir=INPUT_AUDIO_DIR,
+    output_dir=OUTPUT_PITCH_DIR,
+    input_ext="wav",
+    output_ext="f0"
+)
+
+# ... in order to process stereo files, use:
+# piex.process_stereo_files()
+
+# Praat pulse extractor
+puex = praat_utils.PraatPulseExtractor(
+    hopsize=0.01, minfreq=75, maxfreq=400)
+
+# process mono files
+puex.process_mono_files(
+    input_dir=INPUT_AUDIO_DIR,
+    output_dir=OUTPUT_PULSE_DIR,
+    input_ext="wav",
+    output_ext="pulse"
+)
+
+# ... in order to process stereo files, use:
+# puex.process_stereo_files()
+```
+
+### Call Copasul from terminal (if cloned from GitHub)
+
+* see on [example script](https://github.com/reichelu/copasul/scripts/run_copasul.py)
+* `python scripts/run_copasul.py [-c myConfigFile.json]`
+* `PROJECT_ROOT`: directory where GitHub project has been cloned
 
 ```bash
-(venv_copasul) $ cd PROJECT_DIR/scripts/
+(venv_copasul) $ cd PROJECT_ROOT/scripts/
 (venv_copasul) $ python run_copasul.py -c ../tests/minex/config/minex.json
 ```
 
 * if you use `../tests/minex/config/minex.json` as config file, CoPaSul
     * processes the files in `../tests/minex/input/`, and
     * outputs feature tables to `../tests/minex/output/test.FEATURESET.{csv, R}`
     * outputs the CoPaSul output dict to `../tests/minex/output/test.pickle`
@@ -73,16 +114,16 @@
 ### Example integration into python code
 
 ```python
 import json
 import pickle
 import sys
 
-# add this line if you use the cloned code from GitHub
-# sys.path.append(PROJECT_DIR)
+# add this line if you use the code from GitHub
+# sys.path.append(PROJECT_ROOT)
 
 from copasul import copasul
 
 # feature extractor
 fex = copasul.Copasul()
 
 # processing based on config file
```

### Comparing `copasul-1.4.0/copasul/copasul.py` & `copasul-1.5.3/copasul/copasul.py`

 * *Files identical despite different names*

### Comparing `copasul-1.4.0/copasul/copasul_augment.py` & `copasul-1.5.3/copasul/copasul_augment.py`

 * *Files identical despite different names*

### Comparing `copasul-1.4.0/copasul/copasul_clst.py` & `copasul-1.5.3/copasul/copasul_clst.py`

 * *Files identical despite different names*

### Comparing `copasul-1.4.0/copasul/copasul_export.py` & `copasul-1.5.3/copasul/copasul_export.py`

 * *Files identical despite different names*

### Comparing `copasul-1.4.0/copasul/copasul_init.py` & `copasul-1.5.3/copasul/copasul_init.py`

 * *Files identical despite different names*

### Comparing `copasul-1.4.0/copasul/copasul_plot.py` & `copasul-1.5.3/copasul/copasul_plot.py`

 * *Files identical despite different names*

### Comparing `copasul-1.4.0/copasul/copasul_preproc.py` & `copasul-1.5.3/copasul/copasul_preproc.py`

 * *Files identical despite different names*

### Comparing `copasul-1.4.0/copasul/copasul_resyn.py` & `copasul-1.5.3/copasul/copasul_resyn.py`

 * *Files identical despite different names*

### Comparing `copasul-1.4.0/copasul/copasul_sigproc.py` & `copasul-1.5.3/copasul/copasul_sigproc.py`

 * *Files identical despite different names*

### Comparing `copasul-1.4.0/copasul/copasul_styl.py` & `copasul-1.5.3/copasul/copasul_styl.py`

 * *Files identical despite different names*

### Comparing `copasul-1.4.0/copasul/copasul_utils.py` & `copasul-1.5.3/copasul/copasul_utils.py`

 * *Files identical despite different names*

### Comparing `copasul-1.4.0/copasul.egg-info/PKG-INFO` & `copasul-1.5.3/copasul.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copasul
-Version: 1.4.0
+Version: 1.5.3
 Summary: Prosody stylization
 Home-page: https://github.com/reichelu/copasul
 Author: Uwe Reichel
 Author-email: uwe.reichel@nytud.mta.hu
 Project-URL: repository, https://github.com/reichelu/copasul
 Project-URL: documentation, https://github.com/reichelu/copasul
 Project-URL: article, https://arxiv.org/abs/1612.04765
@@ -16,14 +16,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: audeer
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: praat-parselmouth
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: tqdm
 
 # CoPaSul - Contour-based, parametric, and superpositional intonation stylization
 
 ## Author
@@ -71,25 +72,66 @@
 (venv_copasul) $ pip install -r requirements.txt
 ```
 
 ## Usage
 
 ### Required files
 * audio (wav), f0, pulse, and annotation files (Textgrid), see on GitHub: `tests/minex/input`
-    * f0 and pulse files can be generated with the help of the praat scripts on Github: `scripts/*praat`
 * a config file (json), see on GitHub `tests/minex/config/minex.json`
     * see on Github `docs/copasul_commented_config.json.txt` and the [article](https://arxiv.org/abs/1612.04765) for further details
 
-### Call from terminal (if cloned from GitHub)
+### Extract f0 and pulse by means of Praat
 
-* see on [GitHub project page](https://github.com/reichelu/copasul) `scripts/run_copasul.py [-c myConfigFile.json]`
-* `PROJECT_DIR`: directory where GitHub project has been cloned
+* see [example script](https://github.com/reichelu/copasul/scripts/run_praat.py)
+
+```python
+# add this line if you use the code from GitHub
+# sys.path.append(PROJECT_ROOT)
+
+from copasul import praat_utils
+
+# Praat pitch extractor
+piex = praat_utils.PraatPitchExtractor(
+    hopsize=0.01, minfreq=75, maxfreq=600)
+
+# process mono files
+piex.process_mono_files(
+    input_dir=INPUT_AUDIO_DIR,
+    output_dir=OUTPUT_PITCH_DIR,
+    input_ext="wav",
+    output_ext="f0"
+)
+
+# ... in order to process stereo files, use:
+# piex.process_stereo_files()
+
+# Praat pulse extractor
+puex = praat_utils.PraatPulseExtractor(
+    hopsize=0.01, minfreq=75, maxfreq=400)
+
+# process mono files
+puex.process_mono_files(
+    input_dir=INPUT_AUDIO_DIR,
+    output_dir=OUTPUT_PULSE_DIR,
+    input_ext="wav",
+    output_ext="pulse"
+)
+
+# ... in order to process stereo files, use:
+# puex.process_stereo_files()
+```
+
+### Call Copasul from terminal (if cloned from GitHub)
+
+* see on [example script](https://github.com/reichelu/copasul/scripts/run_copasul.py)
+* `python scripts/run_copasul.py [-c myConfigFile.json]`
+* `PROJECT_ROOT`: directory where GitHub project has been cloned
 
 ```bash
-(venv_copasul) $ cd PROJECT_DIR/scripts/
+(venv_copasul) $ cd PROJECT_ROOT/scripts/
 (venv_copasul) $ python run_copasul.py -c ../tests/minex/config/minex.json
 ```
 
 * if you use `../tests/minex/config/minex.json` as config file, CoPaSul
     * processes the files in `../tests/minex/input/`, and
     * outputs feature tables to `../tests/minex/output/test.FEATURESET.{csv, R}`
     * outputs the CoPaSul output dict to `../tests/minex/output/test.pickle`
@@ -99,16 +141,16 @@
 ### Example integration into python code
 
 ```python
 import json
 import pickle
 import sys
 
-# add this line if you use the cloned code from GitHub
-# sys.path.append(PROJECT_DIR)
+# add this line if you use the code from GitHub
+# sys.path.append(PROJECT_ROOT)
 
 from copasul import copasul
 
 # feature extractor
 fex = copasul.Copasul()
 
 # processing based on config file
```

### Comparing `copasul-1.4.0/copasul.egg-info/SOURCES.txt` & `copasul-1.5.3/copasul.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 copasul/copasul_init.py
 copasul/copasul_plot.py
 copasul/copasul_preproc.py
 copasul/copasul_resyn.py
 copasul/copasul_sigproc.py
 copasul/copasul_styl.py
 copasul/copasul_utils.py
+copasul/praat_utils.py
 copasul.egg-info/PKG-INFO
 copasul.egg-info/SOURCES.txt
 copasul.egg-info/dependency_links.txt
 copasul.egg-info/requires.txt
 copasul.egg-info/top_level.txt
 tests/tests_aug.py
 tests/tests_styl.py
```

### Comparing `copasul-1.4.0/setup.cfg` & `copasul-1.5.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = copasul
-version = 1.4.0
+version = 1.5.3
 author = Uwe Reichel
 author_email = uwe.reichel@nytud.mta.hu
 description = Prosody stylization
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/reichelu/copasul
 project_urls = 
@@ -22,14 +22,15 @@
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	audeer
 	matplotlib
 	numpy
 	pandas
+	praat-parselmouth
 	scikit-learn
 	scipy
 	tqdm
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `copasul-1.4.0/tests/tests_aug.py` & `copasul-1.5.3/tests/tests_aug.py`

 * *Files identical despite different names*

### Comparing `copasul-1.4.0/tests/tests_styl.py` & `copasul-1.5.3/tests/tests_styl.py`

 * *Files identical despite different names*

