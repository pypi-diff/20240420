# Comparing `tmp/aqlm-1.1.4.tar.gz` & `tmp/aqlm-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqlm-1.1.4.tar", last modified: Tue Apr  2 22:02:42 2024, max compression
+gzip compressed data, was "aqlm-1.1.5.tar", last modified: Sat Apr 20 17:16:12 2024, max compression
```

## Comparing `aqlm-1.1.4.tar` & `aqlm-1.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-02 22:02:42.418248 aqlm-1.1.4/
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)       81 2024-02-16 15:38:52.000000 aqlm-1.1.4/MANIFEST.in
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1679 2024-04-02 22:02:42.418248 aqlm-1.1.4/PKG-INFO
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      333 2024-02-16 15:38:52.000000 aqlm-1.1.4/pyproject.toml
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1418 2024-04-02 22:02:42.422248 aqlm-1.1.4/setup.cfg
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-02 22:02:42.398247 aqlm-1.1.4/src/
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-02 22:02:42.402247 aqlm-1.1.4/src/aqlm/
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      130 2024-02-22 09:29:16.000000 aqlm-1.1.4/src/aqlm/__init__.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     4747 2024-04-02 21:27:23.000000 aqlm-1.1.4/src/aqlm/inference.py
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-02 22:02:42.410247 aqlm-1.1.4/src/aqlm/inference_kernels/
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      102 2024-02-22 09:29:16.000000 aqlm-1.1.4/src/aqlm/inference_kernels/__init__.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)    10888 2024-04-02 21:27:23.000000 aqlm-1.1.4/src/aqlm/inference_kernels/cuda_kernel.cpp
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)    14569 2024-04-02 21:55:38.000000 aqlm-1.1.4/src/aqlm/inference_kernels/cuda_kernel.cu
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     3350 2024-04-02 21:27:23.000000 aqlm-1.1.4/src/aqlm/inference_kernels/cuda_kernel.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      716 2024-02-22 09:29:16.000000 aqlm-1.1.4/src/aqlm/inference_kernels/dequantization.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     4334 2024-04-02 21:27:23.000000 aqlm-1.1.4/src/aqlm/inference_kernels/kernel_selector.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     2499 2024-03-06 14:39:27.000000 aqlm-1.1.4/src/aqlm/inference_kernels/numba_kernel.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     7238 2024-02-22 09:29:16.000000 aqlm-1.1.4/src/aqlm/inference_kernels/triton_kernel.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     3022 2024-02-16 15:38:52.000000 aqlm-1.1.4/src/aqlm/utils.py
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-02 22:02:42.418248 aqlm-1.1.4/src/aqlm.egg-info/
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1679 2024-04-02 22:02:42.000000 aqlm-1.1.4/src/aqlm.egg-info/PKG-INFO
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      600 2024-04-02 22:02:42.000000 aqlm-1.1.4/src/aqlm.egg-info/SOURCES.txt
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)        1 2024-04-02 22:02:42.000000 aqlm-1.1.4/src/aqlm.egg-info/dependency_links.txt
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      199 2024-04-02 22:02:42.000000 aqlm-1.1.4/src/aqlm.egg-info/requires.txt
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)        5 2024-04-02 22:02:42.000000 aqlm-1.1.4/src/aqlm.egg-info/top_level.txt
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-20 17:16:12.263104 aqlm-1.1.5/
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)       81 2024-02-16 15:38:52.000000 aqlm-1.1.5/MANIFEST.in
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1679 2024-04-20 17:16:12.263104 aqlm-1.1.5/PKG-INFO
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      333 2024-02-16 15:38:52.000000 aqlm-1.1.5/pyproject.toml
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1418 2024-04-20 17:16:12.267104 aqlm-1.1.5/setup.cfg
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-20 17:16:12.239104 aqlm-1.1.5/src/
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-20 17:16:12.243104 aqlm-1.1.5/src/aqlm/
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      130 2024-02-22 09:29:16.000000 aqlm-1.1.5/src/aqlm/__init__.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     4747 2024-04-02 21:27:23.000000 aqlm-1.1.5/src/aqlm/inference.py
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-20 17:16:12.251104 aqlm-1.1.5/src/aqlm/inference_kernels/
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      102 2024-02-22 09:29:16.000000 aqlm-1.1.5/src/aqlm/inference_kernels/__init__.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)    10906 2024-04-20 14:40:20.000000 aqlm-1.1.5/src/aqlm/inference_kernels/cuda_kernel.cpp
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)    14569 2024-04-20 14:12:20.000000 aqlm-1.1.5/src/aqlm/inference_kernels/cuda_kernel.cu
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     3350 2024-04-02 21:27:23.000000 aqlm-1.1.5/src/aqlm/inference_kernels/cuda_kernel.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      716 2024-02-22 09:29:16.000000 aqlm-1.1.5/src/aqlm/inference_kernels/dequantization.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     4334 2024-04-02 21:27:23.000000 aqlm-1.1.5/src/aqlm/inference_kernels/kernel_selector.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     2499 2024-03-06 14:39:27.000000 aqlm-1.1.5/src/aqlm/inference_kernels/numba_kernel.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     7238 2024-02-22 09:29:16.000000 aqlm-1.1.5/src/aqlm/inference_kernels/triton_kernel.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     3022 2024-02-16 15:38:52.000000 aqlm-1.1.5/src/aqlm/utils.py
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-20 17:16:12.259104 aqlm-1.1.5/src/aqlm.egg-info/
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1679 2024-04-20 17:16:12.000000 aqlm-1.1.5/src/aqlm.egg-info/PKG-INFO
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      600 2024-04-20 17:16:12.000000 aqlm-1.1.5/src/aqlm.egg-info/SOURCES.txt
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)        1 2024-04-20 17:16:12.000000 aqlm-1.1.5/src/aqlm.egg-info/dependency_links.txt
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      199 2024-04-20 17:16:12.000000 aqlm-1.1.5/src/aqlm.egg-info/requires.txt
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)        5 2024-04-20 17:16:12.000000 aqlm-1.1.5/src/aqlm.egg-info/top_level.txt
```

### Comparing `aqlm-1.1.4/PKG-INFO` & `aqlm-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqlm
-Version: 1.1.4
+Version: 1.1.5
 Summary: Efficiently run models quantized with AQLM
 Home-page: https://github.com/Vahe1994/AQLM
 Author: AQLM paper authors
 Author-email: vahe527887@yandex.ru
 Project-URL: Bug Tracker, https://github.com/Vahe1994/AQLM/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `aqlm-1.1.4/setup.cfg` & `aqlm-1.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aqlm
-version = 1.1.4
+version = 1.1.5
 author = AQLM paper authors
 author_email = vahe527887@yandex.ru
 description = Efficiently run models quantized with AQLM
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Vahe1994/AQLM
 project_urls =
```

### Comparing `aqlm-1.1.4/src/aqlm/inference.py` & `aqlm-1.1.5/src/aqlm/inference.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.4/src/aqlm/inference_kernels/cuda_kernel.cpp` & `aqlm-1.1.5/src/aqlm/inference_kernels/cuda_kernel.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
   flat_output *= scales.flatten().unsqueeze(0);
   if (bias.has_value()) {
     flat_output += bias->unsqueeze(0);
   }
 
   auto output_sizes = input_sizes.vec();
   output_sizes.pop_back();
-  output_sizes.push_back(-1);
+  output_sizes.push_back(flat_output.size(-1));
   auto output = flat_output.reshape(output_sizes).clone();
   return output;
 }
 
 void code1x16_matvec(
   const torch::Tensor& A,
   const torch::Tensor& B,
```

### Comparing `aqlm-1.1.4/src/aqlm/inference_kernels/cuda_kernel.cu` & `aqlm-1.1.5/src/aqlm/inference_kernels/cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.4/src/aqlm/inference_kernels/cuda_kernel.py` & `aqlm-1.1.5/src/aqlm/inference_kernels/cuda_kernel.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.4/src/aqlm/inference_kernels/dequantization.py` & `aqlm-1.1.5/src/aqlm/inference_kernels/dequantization.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.4/src/aqlm/inference_kernels/kernel_selector.py` & `aqlm-1.1.5/src/aqlm/inference_kernels/kernel_selector.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.4/src/aqlm/inference_kernels/numba_kernel.py` & `aqlm-1.1.5/src/aqlm/inference_kernels/numba_kernel.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.4/src/aqlm/inference_kernels/triton_kernel.py` & `aqlm-1.1.5/src/aqlm/inference_kernels/triton_kernel.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.4/src/aqlm/utils.py` & `aqlm-1.1.5/src/aqlm/utils.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.4/src/aqlm.egg-info/PKG-INFO` & `aqlm-1.1.5/src/aqlm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqlm
-Version: 1.1.4
+Version: 1.1.5
 Summary: Efficiently run models quantized with AQLM
 Home-page: https://github.com/Vahe1994/AQLM
 Author: AQLM paper authors
 Author-email: vahe527887@yandex.ru
 Project-URL: Bug Tracker, https://github.com/Vahe1994/AQLM/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `aqlm-1.1.4/src/aqlm.egg-info/SOURCES.txt` & `aqlm-1.1.5/src/aqlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

