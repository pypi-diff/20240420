# Comparing `tmp/cuxrft-0.0.8.tar.gz` & `tmp/cuxrft-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuxrft-0.0.8.tar", last modified: Fri Mar 15 11:34:06 2024, max compression
+gzip compressed data, was "cuxrft-0.0.9.tar", last modified: Fri Mar 15 12:19:29 2024, max compression
```

## Comparing `cuxrft-0.0.8.tar` & `cuxrft-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 11:34:06.148869 cuxrft-0.0.8/
--rw-rw-rw-   0        0        0     1091 2024-03-15 11:29:33.000000 cuxrft-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      855 2024-03-15 11:34:06.145647 cuxrft-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-03-15 11:29:33.000000 cuxrft-0.0.8/README.rst
--rw-rw-rw-   0        0        0      779 2024-03-15 11:31:03.000000 cuxrft-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-15 11:34:06.148869 cuxrft-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-15 11:34:06.030614 cuxrft-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-15 11:34:06.101876 cuxrft-0.0.8/src/cuxrft/
--rw-rw-rw-   0        0        0      143 2024-03-15 11:31:43.000000 cuxrft-0.0.8/src/cuxrft/__init__.py
--rw-rw-rw-   0        0        0     3111 2024-03-15 11:29:33.000000 cuxrft-0.0.8/src/cuxrft/byte_converter.py
--rw-rw-rw-   0        0        0      844 2024-03-15 11:29:33.000000 cuxrft-0.0.8/src/cuxrft/xarray.py
--rw-rw-rw-   0        0        0    48171 2024-03-15 11:30:31.000000 cuxrft-0.0.8/src/cuxrft/xr_controller_fft.py
-drwxrwxrwx   0        0        0        0 2024-03-15 11:34:06.135232 cuxrft-0.0.8/src/cuxrft.egg-info/
--rw-rw-rw-   0        0        0      855 2024-03-15 11:34:05.000000 cuxrft-0.0.8/src/cuxrft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-03-15 11:34:06.000000 cuxrft-0.0.8/src/cuxrft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 11:34:05.000000 cuxrft-0.0.8/src/cuxrft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-15 11:34:05.000000 cuxrft-0.0.8/src/cuxrft.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-15 12:19:29.937840 cuxrft-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2024-03-15 11:29:33.000000 cuxrft-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      855 2024-03-15 12:19:29.934850 cuxrft-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-03-15 11:29:33.000000 cuxrft-0.0.9/README.rst
+-rw-rw-rw-   0        0        0      779 2024-03-15 12:15:00.000000 cuxrft-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-15 12:19:29.937840 cuxrft-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-15 12:19:29.849586 cuxrft-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-03-15 12:19:29.891848 cuxrft-0.0.9/src/cuxrft/
+-rw-rw-rw-   0        0        0      143 2024-03-15 11:31:43.000000 cuxrft-0.0.9/src/cuxrft/__init__.py
+-rw-rw-rw-   0        0        0     3111 2024-03-15 11:29:33.000000 cuxrft-0.0.9/src/cuxrft/byte_converter.py
+-rw-rw-rw-   0        0        0      844 2024-03-15 11:29:33.000000 cuxrft-0.0.9/src/cuxrft/xarray.py
+-rw-rw-rw-   0        0        0    48199 2024-03-15 12:17:06.000000 cuxrft-0.0.9/src/cuxrft/xr_controller_fft.py
+drwxrwxrwx   0        0        0        0 2024-03-15 12:19:29.931826 cuxrft-0.0.9/src/cuxrft.egg-info/
+-rw-rw-rw-   0        0        0      855 2024-03-15 12:19:29.000000 cuxrft-0.0.9/src/cuxrft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-03-15 12:19:29.000000 cuxrft-0.0.9/src/cuxrft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-15 12:19:29.000000 cuxrft-0.0.9/src/cuxrft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-03-15 12:19:29.000000 cuxrft-0.0.9/src/cuxrft.egg-info/top_level.txt
```

### Comparing `cuxrft-0.0.8/LICENSE` & `cuxrft-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cuxrft-0.0.8/PKG-INFO` & `cuxrft-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuxrft
-Version: 0.0.8
+Version: 0.0.9
 Summary: Performs FFTs on xarray by making use of cuda. Chunking and multiple GPUs in parallel supported.
 Author-email: Tim Vogel <tim.vogel@physik.uni-kl.de>
 Project-URL: Homepage, https://cuxrft.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/timvgl/CuXRFT.git
 Project-URL: Issues, https://github.com/timvgl/CuXRFT/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cuxrft-0.0.8/pyproject.toml` & `cuxrft-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0", "xarray>=2023.1.0", "numpy>=1.24.4", "dask>=2023.5.0", "cupy>=12.2.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cuxrft"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Tim Vogel", email="tim.vogel@physik.uni-kl.de" },
 ]
 description = "Performs FFTs on xarray by making use of cuda. Chunking and multiple GPUs in parallel supported."
 readme = "README.rst"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cuxrft-0.0.8/src/cuxrft/byte_converter.py` & `cuxrft-0.0.9/src/cuxrft/byte_converter.py`

 * *Files identical despite different names*

### Comparing `cuxrft-0.0.8/src/cuxrft/xarray.py` & `cuxrft-0.0.9/src/cuxrft/xarray.py`

 * *Files identical despite different names*

### Comparing `cuxrft-0.0.8/src/cuxrft/xr_controller_fft.py` & `cuxrft-0.0.9/src/cuxrft/xr_controller_fft.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,15 +330,15 @@
                         GPU_avail = GPU_client({'requestGPU': useGPU})
                 print('Executing on GPU ' + str(GPU_avail['useGPU']))
             with cupy.cuda.Device(GPU_avail['useGPU']):
                 fft = cupy.array(data[resultDim].values)
                 # cp.fft.config.show_plan_cache_info()
                 #print("Current gpu memory usage: %s / %s" % (mempool.used_bytes()*1e-9, mempool.total_bytes()*1e-9))
                 if (fftDirection.lower() == "forward"):
-                    fft_d = cupy.fft.fft(fft, axis=fftAxis, norm=fftNorm) 
+                    fft_d = cupy.fft.fftshift(cupy.fft.fft(fft, axis=fftAxis, norm=fftNorm), axes=fftAxis)
                 elif (fftDirection.lower() == "inverse"):
                     fft_d = cupy.fft.ifft(fft, axis=fftAxis, norm=fftNorm) 
                 else:
                     raise ValueError("No proper direction provided.")
                 del fft
                 fftReturn = fft_d.get()
                 del fft_d
@@ -472,23 +472,23 @@
     mempool = cupy.get_default_memory_pool()
     pinned_mempool = cupy.get_default_pinned_memory_pool()
     if (multiple_GPUs == True):
         executor = concurrent.futures.ProcessPoolExecutor()
         if (len(GPUs) == 1):
             GPUs = 'all'
         try:
-            executor.submit(GPU_client, {'checkHealth': 0}).results(timeout=3)
+            executor.submit(GPU_client, {'checkHealth': 0}).result(timeout=3)
             GPUServerStarted = True
         except (ConnectionResetError, ConnectionRefusedError, FileNotFoundError, TimeoutError):
             GPUServerStarted = False
         if (GPUServerStarted == False):
             GPUcontrollingServerThread = executor.submit(GPUcontrollingServer)
             while not GPUServerStarted:
                 try:
-                    executor.submit(GPU_client, {'checkHealth': 0}).results(timeout=3)
+                    executor.submit(GPU_client, {'checkHealth': 0}).result(timeout=3)
                     GPUServerStarted = True
                 except (ConnectionResetError, ConnectionRefusedError, FileNotFoundError, TimeoutError):
                     GPUServerStarted = False
                 time.sleep(1)
     dataTransposed = False
     #transform axis has to be the 0th axis
     for data_var in data_vars:
@@ -698,23 +698,23 @@
     mempool = cupy.get_default_memory_pool()
     pinned_mempool = cupy.get_default_pinned_memory_pool()
     if (multiple_GPUs == True):
         executor = concurrent.futures.ProcessPoolExecutor()
         if (len(GPUs) == 1):
             GPUs = 'all'
         try:
-            executor.submit(GPU_client, {'checkHealth': 0}).results(timeout=3)
+            executor.submit(GPU_client, {'checkHealth': 0}).result(timeout=3)
             GPUServerStarted = True
         except (ConnectionResetError, ConnectionRefusedError, FileNotFoundError, TimeoutError):
             GPUServerStarted = False
         if (GPUServerStarted == False):
             GPUcontrollingServerThread = executor.submit(GPUcontrollingServer)
             while not GPUServerStarted:
                 try:
-                    executor.submit(GPU_client, {'checkHealth': 0}).results(timeout=3)
+                    executor.submit(GPU_client, {'checkHealth': 0}).result(timeout=3)
                     GPUServerStarted = True
                 except (ConnectionResetError, ConnectionRefusedError, FileNotFoundError, TimeoutError):
                     GPUServerStarted = False
                 time.sleep(1)
     dataTransposed = False
     #transform axis has to be the 0th axis
     for data_var in data_vars:
```

### Comparing `cuxrft-0.0.8/src/cuxrft.egg-info/PKG-INFO` & `cuxrft-0.0.9/src/cuxrft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuxrft
-Version: 0.0.8
+Version: 0.0.9
 Summary: Performs FFTs on xarray by making use of cuda. Chunking and multiple GPUs in parallel supported.
 Author-email: Tim Vogel <tim.vogel@physik.uni-kl.de>
 Project-URL: Homepage, https://cuxrft.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/timvgl/CuXRFT.git
 Project-URL: Issues, https://github.com/timvgl/CuXRFT/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

