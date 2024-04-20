# Comparing `tmp/thepipe_api-0.2.7.tar.gz` & `tmp/thepipe_api-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.2.7.tar", last modified: Fri Apr 19 14:53:20 2024, max compression
+gzip compressed data, was "thepipe_api-0.2.8.tar", last modified: Sat Apr 20 03:44:38 2024, max compression
```

## Comparing `thepipe_api-0.2.7.tar` & `thepipe_api-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 14:53:20.733883 thepipe_api-0.2.7/
--rw-rw-rw-   0        0        0     1094 2024-04-18 07:46:31.000000 thepipe_api-0.2.7/LICENSE
--rw-rw-rw-   0        0        0    10866 2024-04-19 14:53:20.731881 thepipe_api-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    10109 2024-04-18 16:18:13.000000 thepipe_api-0.2.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 14:53:20.734882 thepipe_api-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-19 14:52:42.000000 thepipe_api-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:53:20.690881 thepipe_api-0.2.7/tests/
--rw-rw-rw-   0        0        0        0 2024-04-18 07:46:31.000000 thepipe_api-0.2.7/tests/__init__.py
--rw-rw-rw-   0        0        0     9265 2024-04-18 07:46:31.000000 thepipe_api-0.2.7/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:53:20.700883 thepipe_api-0.2.7/thepipe_api/
--rw-rw-rw-   0        0        0       86 2024-04-18 07:46:31.000000 thepipe_api-0.2.7/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4821 2024-04-18 07:46:31.000000 thepipe_api-0.2.7/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2778 2024-04-19 14:45:09.000000 thepipe_api-0.2.7/thepipe_api/core.py
--rw-rw-rw-   0        0        0    21113 2024-04-19 14:51:46.000000 thepipe_api-0.2.7/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3611 2024-04-19 14:51:46.000000 thepipe_api-0.2.7/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:53:20.729884 thepipe_api-0.2.7/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0    10866 2024-04-19 14:53:20.000000 thepipe_api-0.2.7/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-19 14:53:20.000000 thepipe_api-0.2.7/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 14:53:20.000000 thepipe_api-0.2.7/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-19 14:53:20.000000 thepipe_api-0.2.7/thepipe_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      118 2024-04-19 14:53:20.000000 thepipe_api-0.2.7/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-19 14:53:20.000000 thepipe_api-0.2.7/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 03:44:38.840412 thepipe_api-0.2.8/
+-rw-rw-rw-   0        0        0     1094 2024-04-18 07:46:31.000000 thepipe_api-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0    10866 2024-04-20 03:44:38.839413 thepipe_api-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    10109 2024-04-18 16:18:13.000000 thepipe_api-0.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 03:44:38.840412 thepipe_api-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-20 03:44:03.000000 thepipe_api-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 03:44:38.807690 thepipe_api-0.2.8/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-18 07:46:31.000000 thepipe_api-0.2.8/tests/__init__.py
+-rw-rw-rw-   0        0        0     9265 2024-04-18 07:46:31.000000 thepipe_api-0.2.8/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-20 03:44:38.812690 thepipe_api-0.2.8/thepipe_api/
+-rw-rw-rw-   0        0        0       86 2024-04-18 07:46:31.000000 thepipe_api-0.2.8/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4821 2024-04-18 07:46:31.000000 thepipe_api-0.2.8/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2778 2024-04-19 14:45:09.000000 thepipe_api-0.2.8/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    21113 2024-04-19 14:51:46.000000 thepipe_api-0.2.8/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3704 2024-04-20 03:43:57.000000 thepipe_api-0.2.8/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-20 03:44:38.838414 thepipe_api-0.2.8/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0    10866 2024-04-20 03:44:38.000000 thepipe_api-0.2.8/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-20 03:44:38.000000 thepipe_api-0.2.8/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 03:44:38.000000 thepipe_api-0.2.8/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-20 03:44:38.000000 thepipe_api-0.2.8/thepipe_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      118 2024-04-20 03:44:38.000000 thepipe_api-0.2.8/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-20 03:44:38.000000 thepipe_api-0.2.8/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.2.7/LICENSE` & `thepipe_api-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.7/PKG-INFO` & `thepipe_api-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.2.7
+Version: 0.2.8
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.7 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.8 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
```

### Comparing `thepipe_api-0.2.7/README.md` & `thepipe_api-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.7/setup.py` & `thepipe_api-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.2.7',
+    version='0.2.8',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
```

### Comparing `thepipe_api-0.2.7/tests/test_thepipe.py` & `thepipe_api-0.2.8/tests/test_thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.7/thepipe_api/compressor.py` & `thepipe_api-0.2.8/thepipe_api/compressor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.7/thepipe_api/core.py` & `thepipe_api-0.2.8/thepipe_api/core.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.7/thepipe_api/extractor.py` & `thepipe_api-0.2.8/thepipe_api/extractor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.7/thepipe_api/thepipe.py` & `thepipe_api-0.2.8/thepipe_api/thepipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,18 @@
         os.makedirs('outputs')
     # Save the chunks to files
     text = ""
     n_images = 0
     for i, chunk in enumerate(chunks):
         if chunk is None:
             continue
+        if chunk.path is not None:
+            text += f'{chunk.path}:\n'
         if chunk.text is not None:
-            text += chunk.text
+            text += f'```\n{chunk.text}```\n\n'
         if (chunk.image is not None) and (not text_only):
             if chunk.path is None:
                 clean_path = f"image"
             else:
                 clean_path = chunk.path.replace('/', '_').replace('\\', '_')
                 clean_path = re.sub(r"[^a-zA-Z0-9 _]", "", clean_path)
             chunk.image.convert('RGB').save(f'outputs/{clean_path}_{i}.jpg')
```

### Comparing `thepipe_api-0.2.7/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.2.8/thepipe_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.2.7
+Version: 0.2.8
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.7 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.8 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
```

