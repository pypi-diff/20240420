# Comparing `tmp/fftvis-0.0.4.tar.gz` & `tmp/fftvis-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fftvis-0.0.4.tar", last modified: Thu Apr 18 22:17:21 2024, max compression
+gzip compressed data, was "fftvis-0.0.6.tar", last modified: Sat Apr 20 01:00:48 2024, max compression
```

## Comparing `fftvis-0.0.4.tar` & `fftvis-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.226088 fftvis-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 22:17:11.000000 fftvis-0.0.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.222088 fftvis-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.222088 fftvis-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-18 22:17:11.000000 fftvis-0.0.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-18 22:17:11.000000 fftvis-0.0.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-18 22:17:11.000000 fftvis-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-18 22:17:11.000000 fftvis-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-18 22:17:21.226088 fftvis-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-18 22:17:11.000000 fftvis-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.222088 fftvis-0.0.4/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 22:17:11.000000 fftvis-0.0.4/ci/fftvis_tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.222088 fftvis-0.0.4/fftvis/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/beams.py
--rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.226088 fftvis-0.0.4/fftvis/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/tests/test_compare_matvis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/tests/test_compare_pyuvsim.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.226088 fftvis-0.0.4/fftvis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-18 22:17:21.000000 fftvis-0.0.4/fftvis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-18 22:17:21.000000 fftvis-0.0.4/fftvis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:17:21.000000 fftvis-0.0.4/fftvis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-18 22:17:21.000000 fftvis-0.0.4/fftvis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 22:17:21.000000 fftvis-0.0.4/fftvis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-18 22:17:11.000000 fftvis-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-18 22:17:21.226088 fftvis-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-18 22:17:11.000000 fftvis-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:00:48.271177 fftvis-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-20 01:00:43.000000 fftvis-0.0.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:00:48.263177 fftvis-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:00:48.267177 fftvis-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-20 01:00:43.000000 fftvis-0.0.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-20 01:00:43.000000 fftvis-0.0.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-20 01:00:43.000000 fftvis-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-20 01:00:43.000000 fftvis-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-20 01:00:48.271177 fftvis-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-20 01:00:43.000000 fftvis-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:00:48.267177 fftvis-0.0.6/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-20 01:00:43.000000 fftvis-0.0.6/ci/fftvis_tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:00:48.267177 fftvis-0.0.6/fftvis/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-20 01:00:43.000000 fftvis-0.0.6/fftvis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-20 01:00:43.000000 fftvis-0.0.6/fftvis/beams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-20 01:00:43.000000 fftvis-0.0.6/fftvis/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:00:48.267177 fftvis-0.0.6/fftvis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-20 01:00:43.000000 fftvis-0.0.6/fftvis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-20 01:00:43.000000 fftvis-0.0.6/fftvis/tests/test_compare_matvis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-20 01:00:43.000000 fftvis-0.0.6/fftvis/tests/test_compare_pyuvsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-20 01:00:43.000000 fftvis-0.0.6/fftvis/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-20 01:00:43.000000 fftvis-0.0.6/fftvis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:00:48.267177 fftvis-0.0.6/fftvis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-20 01:00:48.000000 fftvis-0.0.6/fftvis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-20 01:00:48.000000 fftvis-0.0.6/fftvis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:00:48.000000 fftvis-0.0.6/fftvis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-20 01:00:48.000000 fftvis-0.0.6/fftvis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 01:00:48.000000 fftvis-0.0.6/fftvis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-20 01:00:43.000000 fftvis-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-20 01:00:48.271177 fftvis-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-20 01:00:43.000000 fftvis-0.0.6/setup.py
```

### Comparing `fftvis-0.0.4/.github/workflows/ci.yml` & `fftvis-0.0.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.4/.github/workflows/publish-to-pypi.yml` & `fftvis-0.0.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.4/.gitignore` & `fftvis-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.4/LICENSE` & `fftvis-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.4/PKG-INFO` & `fftvis-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fftvis
-Version: 0.0.4
+Version: 0.0.6
 Summary: An FFT-based visibility simulator
 Home-page: https://github.com/tyler-a-cox/fftvis
 Author: Tyler Cox
 Author-email: tyler.a.cox@berkeley.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fftvis-0.0.4/README.md` & `fftvis-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.4/fftvis/beams.py` & `fftvis-0.0.6/fftvis/beams.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.4/fftvis/simulate.py` & `fftvis-0.0.6/fftvis/simulate.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 
         if nsim_sources == 0:
             continue
 
         # Form the visibility array
         _vis = np.zeros((nfeeds, nfeeds, nbls, nfreqs), dtype=complex_dtype)
 
-        if is_beam_complex:
+        if is_beam_complex and expand_vis:
             _vis_negatives = np.zeros(
                 (nfeeds, nfeeds, nbls, nfreqs), dtype=complex_dtype
             )
 
         # Compute azimuth and zenith angles
         az, za = conversions.enu_to_az_za(enu_e=tx, enu_n=ty, orientation="uvbeam")
 
@@ -276,15 +276,15 @@
                 eps=eps,
             )
 
             # Expand out the visibility array
             _vis[..., fi] = _vis_here.reshape(nfeeds, nfeeds, nbls)
 
             # If beam is complex, we need to compute the reverse negative frequencies
-            if is_beam_complex:
+            if is_beam_complex and expand_vis:
                 # Compute
                 _vis_here_neg = finufft.nufft2d3(
                     2 * np.pi * tx,
                     2 * np.pi * ty,
                     i_sky,
                     -u,
                     -v,
@@ -300,28 +300,31 @@
                     vis,
                     (ti, bl_to_red_map[bls][:, 0], bl_to_red_map[bls][:, 1]),
                     _vis[..., bi, :],
                 )
 
                 # Add the conjugate, avoid auto baselines twice
                 if bls[0] != bls[1]:
+                    # If beam is complex, we need to use the negative frequencies
+                    # otherwise, we can just use the conjugate
                     if is_beam_complex:
                         np.add.at(
                             vis,
                             (ti, bl_to_red_map[bls][:, 1], bl_to_red_map[bls][:, 0]),
                             _vis_negatives[..., bi, :],
                         )
                     else:
                         np.add.at(
                             vis,
                             (ti, bl_to_red_map[bls][:, 1], bl_to_red_map[bls][:, 0]),
                             _vis[..., bi, :].conj(),
                         )
 
         else:
+            # Baselines were provided, so we can just add the visibilities
             vis[ti] = np.swapaxes(_vis, 2, 0)
 
     if expand_vis:
         return (
             np.transpose(vis, (5, 0, 3, 4, 1, 2))
             if polarized
             else np.moveaxis(vis[..., 0, 0, :], 3, 0)
```

### Comparing `fftvis-0.0.4/fftvis/tests/__init__.py` & `fftvis-0.0.6/fftvis/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.4/fftvis/tests/test_compare_matvis.py` & `fftvis-0.0.6/fftvis/tests/test_compare_matvis.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.4/fftvis/tests/test_compare_pyuvsim.py` & `fftvis-0.0.6/fftvis/tests/test_compare_pyuvsim.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.4/fftvis/utils.py` & `fftvis-0.0.6/fftvis/utils.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.4/fftvis.egg-info/PKG-INFO` & `fftvis-0.0.6/fftvis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fftvis
-Version: 0.0.4
+Version: 0.0.6
 Summary: An FFT-based visibility simulator
 Home-page: https://github.com/tyler-a-cox/fftvis
 Author: Tyler Cox
 Author-email: tyler.a.cox@berkeley.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fftvis-0.0.4/setup.cfg` & `fftvis-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.4/setup.py` & `fftvis-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This file is used to install the package using pip.
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="fftvis",
-    version="0.0.4",
+    version="0.0.6",
     description="An FFT-based visibility simulator",
     author="Tyler Cox",
     author_email="tyler.a.cox@berkeley.edu",
     license="MIT",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

