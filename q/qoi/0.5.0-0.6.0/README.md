# Comparing `tmp/qoi-0.5.0.tar.gz` & `tmp/qoi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoi-0.5.0.tar", last modified: Wed Dec 13 08:12:15 2023, max compression
+gzip compressed data, was "qoi-0.6.0.tar", last modified: Sat Apr 20 11:18:00 2024, max compression
```

## Comparing `qoi-0.5.0.tar` & `qoi-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 08:12:15.205910 qoi-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 08:12:15.189910 qoi-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 08:12:15.193910 qoi-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2023-12-13 08:12:02.000000 qoi-0.5.0/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-12-13 08:12:02.000000 qoi-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-13 08:12:02.000000 qoi-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-13 08:12:02.000000 qoi-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2023-12-13 08:12:15.205910 qoi-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8788 2023-12-13 08:12:02.000000 qoi-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2023-12-13 08:12:02.000000 qoi-0.5.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)       32 2023-12-13 08:12:02.000000 qoi-0.5.0/requirements-dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       13 2023-12-13 08:12:02.000000 qoi-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-12-13 08:12:15.205910 qoi-0.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2023-12-13 08:12:02.000000 qoi-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 08:12:15.189910 qoi-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 08:12:15.201910 qoi-0.5.0/src/qoi/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-13 08:12:02.000000 qoi-0.5.0/src/qoi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-13 08:12:15.000000 qoi-0.5.0/src/qoi/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2023-12-13 08:12:02.000000 qoi-0.5.0/src/qoi/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-13 08:12:02.000000 qoi-0.5.0/src/qoi/implementation.c
--rw-r--r--   0 runner    (1001) docker     (127)  3107003 2023-12-13 08:12:02.000000 qoi-0.5.0/src/qoi/koi.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 08:12:15.201910 qoi-0.5.0/src/qoi/phoboslab_qoi/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-13 08:12:02.000000 qoi-0.5.0/src/qoi/phoboslab_qoi/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    18331 2023-12-13 08:12:02.000000 qoi-0.5.0/src/qoi/phoboslab_qoi/qoi.h
--rw-r--r--   0 runner    (1001) docker     (127)  1256352 2023-12-13 08:12:14.000000 qoi-0.5.0/src/qoi/qoi.c
--rwxr-xr-x   0 runner    (1001) docker     (127)      547 2023-12-13 08:12:02.000000 qoi-0.5.0/src/qoi/qoi.pxd
--rwxr-xr-x   0 runner    (1001) docker     (127)     4916 2023-12-13 08:12:02.000000 qoi-0.5.0/src/qoi/qoi.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 08:12:15.201910 qoi-0.5.0/src/qoi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2023-12-13 08:12:15.000000 qoi-0.5.0/src/qoi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2023-12-13 08:12:15.000000 qoi-0.5.0/src/qoi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 08:12:15.000000 qoi-0.5.0/src/qoi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 08:12:14.000000 qoi-0.5.0/src/qoi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-13 08:12:15.000000 qoi-0.5.0/src/qoi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-13 08:12:15.000000 qoi-0.5.0/src/qoi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 08:12:15.201910 qoi-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2023-12-13 08:12:02.000000 qoi-0.5.0/tests/test_multithread.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2377 2023-12-13 08:12:02.000000 qoi-0.5.0/tests/test_qoi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:00.283815 qoi-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:00.271815 qoi-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:00.275815 qoi-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-20 11:17:51.000000 qoi-0.6.0/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-20 11:17:51.000000 qoi-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-20 11:17:51.000000 qoi-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-20 11:17:51.000000 qoi-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-04-20 11:18:00.283815 qoi-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8718 2024-04-20 11:17:51.000000 qoi-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-20 11:17:51.000000 qoi-0.6.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-20 11:17:51.000000 qoi-0.6.0/requirements-dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       13 2024-04-20 11:17:51.000000 qoi-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-20 11:18:00.283815 qoi-0.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2024-04-20 11:17:51.000000 qoi-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:00.271815 qoi-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:00.279815 qoi-0.6.0/src/qoi/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-20 11:17:51.000000 qoi-0.6.0/src/qoi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 11:18:00.000000 qoi-0.6.0/src/qoi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-04-20 11:17:51.000000 qoi-0.6.0/src/qoi/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 11:17:51.000000 qoi-0.6.0/src/qoi/implementation.c
+-rw-r--r--   0 runner    (1001) docker     (127)  3107003 2024-04-20 11:17:51.000000 qoi-0.6.0/src/qoi/koi.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:00.283815 qoi-0.6.0/src/qoi/phoboslab_qoi/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-20 11:17:51.000000 qoi-0.6.0/src/qoi/phoboslab_qoi/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18331 2024-04-20 11:17:51.000000 qoi-0.6.0/src/qoi/phoboslab_qoi/qoi.h
+-rw-r--r--   0 runner    (1001) docker     (127)  1256651 2024-04-20 11:17:59.000000 qoi-0.6.0/src/qoi/qoi.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)      547 2024-04-20 11:17:51.000000 qoi-0.6.0/src/qoi/qoi.pxd
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4911 2024-04-20 11:17:51.000000 qoi-0.6.0/src/qoi/qoi.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:00.283815 qoi-0.6.0/src/qoi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-04-20 11:18:00.000000 qoi-0.6.0/src/qoi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-20 11:18:00.000000 qoi-0.6.0/src/qoi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 11:18:00.000000 qoi-0.6.0/src/qoi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 11:17:59.000000 qoi-0.6.0/src/qoi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-20 11:18:00.000000 qoi-0.6.0/src/qoi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-20 11:18:00.000000 qoi-0.6.0/src/qoi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:00.283815 qoi-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-20 11:17:51.000000 qoi-0.6.0/tests/test_multithread.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2377 2024-04-20 11:17:51.000000 qoi-0.6.0/tests/test_qoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-20 11:17:51.000000 qoi-0.6.0/tests/test_ro_issue26.py
```

### Comparing `qoi-0.5.0/.github/workflows/wheels.yml` & `qoi-0.6.0/.github/workflows/wheels.yml`

 * *Files 6% similar despite different names*

```diff
@@ -11,78 +11,79 @@
       - main
 
 jobs:
   build_sdist:
     name: Build source distribution
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0 # Optional, use if you use setuptools_scm https://stackoverflow.com/a/68959339
           submodules: true # Optional, use if you have submodules
 
-      - name: Set up Python 3.8
-        uses: actions/setup-python@v2
+      - name: Set up Python 3.9
+        uses: actions/setup-python@v5
         with:
-          python-version: 3.8
+          python-version: 3.9
 
       - name: Install pypa/build
         run: pip install build
 
       - name: Build sdist *and* wheel (even though we ignore it) to check we can confirm wheels from source.
         run: USE_CYTHON=1 python -m build
 
-      - uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v4
         with:
           path: dist/*.tar.gz
 
   build_wheels:
     needs: build_sdist
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-20.04, windows-2019, macos-12]
+        os: [ubuntu-latest, windows-latest, macos-13, macos-14]
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0 # Optional, use if you use setuptools_scm https://stackoverflow.com/a/68959339
           submodules: true # Optional, use if you have submodules
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.16.2
-      - uses: actions/upload-artifact@v2
+        uses: pypa/cibuildwheel@v2.17.0
+      - uses: actions/upload-artifact@v4
         with:
+          name: cibw-wheels-${{ matrix.os }}-${{ strategy.job-index }}
           path: ./wheelhouse/*.whl
 
   create_release:
     needs: build_wheels
     runs-on: ubuntu-latest
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags/v')
     steps:
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v4
         with:
           name: artifact
           path: dist
 
       - name: Release
-        uses: softprops/action-gh-release@v1
+        uses: softprops/action-gh-release@v2.0.4
         with:
           files: dist/*
 
   upload_pypi:
     needs: build_wheels
     runs-on: ubuntu-latest
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags/v')
     steps:
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v4
         with:
           name: artifact
           path: dist
-      - uses: pypa/gh-action-pypi-publish@v1.4.2
+      - uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           user: __token__
           password: ${{ secrets.test_pypi_password }}
           repository_url: https://test.pypi.org/legacy/
-      - uses: pypa/gh-action-pypi-publish@v1.4.2
+      - uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           user: __token__
           password: ${{ secrets.pypi_password }}
```

### Comparing `qoi-0.5.0/LICENSE` & `qoi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qoi-0.5.0/PKG-INFO` & `qoi-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoi
-Version: 0.5.0
+Version: 0.6.0
 Summary: A simpler wrapper around qoi (https://github.com/phoboslab/qoi)
 Home-page: https://github.com/kodonnell/qoi
 Author: kodonnell
 Author-email: kodonnell@users.noreply.github.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kodonnell/qoi/issues
 Keywords: qoi
@@ -15,14 +15,16 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22.4
 Provides-Extra: dev
 Requires-Dist: Cython>=3.0.0; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pillow; extra == "dev"
+Requires-Dist: opencv-python-headless; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 [![PyPI version fury.io](https://badge.fury.io/py/qoi.svg)](https://pypi.python.org/pypi/qoi/)
 
 # QOI
 
@@ -40,15 +42,15 @@
 
 ## Example
 
 ```python
 import numpy as np
 import qoi
 
-# Get your image as a numpy array (OpenCV, Pillow, etc. but here we just create a bunch of noise)
+# Get your image as a numpy array (OpenCV, Pillow, etc. but here we just create a bunch of noise). Note: HWC ordering
 rgb = np.random.randint(low=0, high=255, size=(224, 244, 3)).astype(np.uint8)
 
 # Write it:
 _ = qoi.write("/tmp/img.qoi", rgb)
 
 # Read it and check it matches (it should, as we're lossless)
 rgb_read = qoi.read("/tmp/img.qoi")
@@ -104,20 +106,20 @@
 > NB:
 >
 > 1. There's additional overhead here with PIL images being converted back to an array as the return type, to be consistent. In some sense, this isn't fair, as PIL will be faster if you're dealing with PIL images. On the other hand, if your common use case involves arrays (e.g. for computer vision) then it's reasonable.
 > 2. Produced with `python src/qoi/benchmark.py --implementations=qoi,opencv,pil --formats=png,qoi` on an i7-9750H. Not going to the point of optimised OpenCV/PIL (e.g. SIMD, or `pillow-simd`) as the results are clear enough for this 'normal' scenario. If you want to dig further, go for it! You can easily run these tests yourself.
 
 If we consider lossy compression, again, JPEG is usually what we're comparing with. Normally, it'd be unfair to compare QOI with JPEG as QOI is lossless, however we can do a slight trick to make QOI lossy - downscale the image, then encode it, then upsample it by the same amount after decoding. You can see we've implemented that below with a downscaling to 40% and JPEG quality of 80 (which results in them having the same visual compression i.e. SSIM). So, results (only on `koi photo` as the rest are less meaningful/fair for lossy):
 
-| Test image                | Method              | Format   | Input (kb) | Encode (ms) | Encode (kb) | Decode (ms) | SSIM |
-| ------------------------- | ------------------- | -------- | ---------- | ----------- | ----------- | ----------- | ---- |
-| koi photo                 | PIL                 | jpg @ 80 | 6075.0     | 47.67       | 275.2       | 24.01       | 0.94 |
-| koi photo                 | opencv              | jpg @ 80 | 6075.0     | 24.03       | 275.3       | 19.58       | 0.94 |
-| koi photo                 | qoi                 | qoi      | 6075.0     | 23.17       | 3489.0      | 12.94       | 1.00 |
-| koi photo                 | qoi-lossy-0.40x0.40 | qoi      | 6075.0     | 4.38        | 667.5       | 2.96        | 0.94 |
+| Test image | Method              | Format   | Input (kb) | Encode (ms) | Encode (kb) | Decode (ms) | SSIM |
+| ---------- | ------------------- | -------- | ---------- | ----------- | ----------- | ----------- | ---- |
+| koi photo  | PIL                 | jpg @ 80 | 6075.0     | 47.67       | 275.2       | 24.01       | 0.94 |
+| koi photo  | opencv              | jpg @ 80 | 6075.0     | 24.03       | 275.3       | 19.58       | 0.94 |
+| koi photo  | qoi                 | qoi      | 6075.0     | 23.17       | 3489.0      | 12.94       | 1.00 |
+| koi photo  | qoi-lossy-0.40x0.40 | qoi      | 6075.0     | 4.38        | 667.5       | 2.96        | 0.94 |
 
 Here we see that lossless `qoi` is losing out considerably in compression, as expected for lossy vs lossless. Also, `qoi` is only 1x-2x faster of encoding, and 1.5x-2x faster for decoding. However, it's important to note that this varies a lot depending on the jpeg quality specified - here it's 80 but the default for OpenCV is actually 95 which is 3x worse compression and a bit slower.
 
 However, that's still lossy vs lossless! If you look at `qoi-lossy-0.40x0.40` where we downscale as above, you can see that it can perform really well. The compression ratio is now only 3x that of JPEG (and 5x better than lossless QOI, and also the same as the default OpenCV JPEG encoding at a quality of 95), but it's so fast - 5x-10x faster encoding, and 7x-8x faster decoding.
 
 Anyway, there are definitely use cases where `qoi` may still make sense over JPEG. Even lossless QOI can be worth it if size isn't an issue, as it's a bit faster. But if you use the "lossy" QOI, you're getting "comparable" (depending on JPEG quality) compression but much faster.
```

### Comparing `qoi-0.5.0/README.md` & `qoi-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ## Example
 
 ```python
 import numpy as np
 import qoi
 
-# Get your image as a numpy array (OpenCV, Pillow, etc. but here we just create a bunch of noise)
+# Get your image as a numpy array (OpenCV, Pillow, etc. but here we just create a bunch of noise). Note: HWC ordering
 rgb = np.random.randint(low=0, high=255, size=(224, 244, 3)).astype(np.uint8)
 
 # Write it:
 _ = qoi.write("/tmp/img.qoi", rgb)
 
 # Read it and check it matches (it should, as we're lossless)
 rgb_read = qoi.read("/tmp/img.qoi")
@@ -80,20 +80,20 @@
 > NB:
 >
 > 1. There's additional overhead here with PIL images being converted back to an array as the return type, to be consistent. In some sense, this isn't fair, as PIL will be faster if you're dealing with PIL images. On the other hand, if your common use case involves arrays (e.g. for computer vision) then it's reasonable.
 > 2. Produced with `python src/qoi/benchmark.py --implementations=qoi,opencv,pil --formats=png,qoi` on an i7-9750H. Not going to the point of optimised OpenCV/PIL (e.g. SIMD, or `pillow-simd`) as the results are clear enough for this 'normal' scenario. If you want to dig further, go for it! You can easily run these tests yourself.
 
 If we consider lossy compression, again, JPEG is usually what we're comparing with. Normally, it'd be unfair to compare QOI with JPEG as QOI is lossless, however we can do a slight trick to make QOI lossy - downscale the image, then encode it, then upsample it by the same amount after decoding. You can see we've implemented that below with a downscaling to 40% and JPEG quality of 80 (which results in them having the same visual compression i.e. SSIM). So, results (only on `koi photo` as the rest are less meaningful/fair for lossy):
 
-| Test image                | Method              | Format   | Input (kb) | Encode (ms) | Encode (kb) | Decode (ms) | SSIM |
-| ------------------------- | ------------------- | -------- | ---------- | ----------- | ----------- | ----------- | ---- |
-| koi photo                 | PIL                 | jpg @ 80 | 6075.0     | 47.67       | 275.2       | 24.01       | 0.94 |
-| koi photo                 | opencv              | jpg @ 80 | 6075.0     | 24.03       | 275.3       | 19.58       | 0.94 |
-| koi photo                 | qoi                 | qoi      | 6075.0     | 23.17       | 3489.0      | 12.94       | 1.00 |
-| koi photo                 | qoi-lossy-0.40x0.40 | qoi      | 6075.0     | 4.38        | 667.5       | 2.96        | 0.94 |
+| Test image | Method              | Format   | Input (kb) | Encode (ms) | Encode (kb) | Decode (ms) | SSIM |
+| ---------- | ------------------- | -------- | ---------- | ----------- | ----------- | ----------- | ---- |
+| koi photo  | PIL                 | jpg @ 80 | 6075.0     | 47.67       | 275.2       | 24.01       | 0.94 |
+| koi photo  | opencv              | jpg @ 80 | 6075.0     | 24.03       | 275.3       | 19.58       | 0.94 |
+| koi photo  | qoi                 | qoi      | 6075.0     | 23.17       | 3489.0      | 12.94       | 1.00 |
+| koi photo  | qoi-lossy-0.40x0.40 | qoi      | 6075.0     | 4.38        | 667.5       | 2.96        | 0.94 |
 
 Here we see that lossless `qoi` is losing out considerably in compression, as expected for lossy vs lossless. Also, `qoi` is only 1x-2x faster of encoding, and 1.5x-2x faster for decoding. However, it's important to note that this varies a lot depending on the jpeg quality specified - here it's 80 but the default for OpenCV is actually 95 which is 3x worse compression and a bit slower.
 
 However, that's still lossy vs lossless! If you look at `qoi-lossy-0.40x0.40` where we downscale as above, you can see that it can perform really well. The compression ratio is now only 3x that of JPEG (and 5x better than lossless QOI, and also the same as the default OpenCV JPEG encoding at a quality of 95), but it's so fast - 5x-10x faster encoding, and 7x-8x faster decoding.
 
 Anyway, there are definitely use cases where `qoi` may still make sense over JPEG. Even lossless QOI can be worth it if size isn't an issue, as it's a bit faster. But if you use the "lossy" QOI, you're getting "comparable" (depending on JPEG quality) compression but much faster.
```

### Comparing `qoi-0.5.0/pyproject.toml` & `qoi-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [build-system]
 requires = [
     "setuptools >= 60",
     "wheel >= 0.30.0",
     "setuptools_scm >= 8.0",
-
+    "Cython>=3.0.8",
     # Below copied from scipy https://github.com/scipy/scipy/blob/main/pyproject.toml
-    "Cython>=0.29.35,!=3.0.3",  # when updating version, also update check in meson.build
 
     # default numpy requirements
     "numpy==1.22.4; python_version<='3.10' and platform_python_implementation != 'PyPy'",
     "numpy==1.23.2; python_version=='3.11' and platform_python_implementation != 'PyPy'",
     "numpy>=1.26.0,<1.27; python_version=='3.12'",
 
     # PyPy requirements; 1.25.0 was the first version to have pypy-3.9 wheels,
@@ -26,15 +25,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "src/qoi/_version.py"
 write_to_template = "__version__ = \"{version}\""
 
 [tool.cibuildwheel]
-test-requires = "pytest"
+test-requires = "pytest pillow"
 test-command = "pytest {project}/tests"
 build = "cp38-* cp39-* cp310-* cp311-* cp312-*"
 # skip musl and ignore the non-standard linux builds
-skip = "*-musllinux_* *s390x* *ppc64le*"
+skip = "*-musllinux_* *s390x* *ppc64le* *i686*"
 build-frontend = "build"
-environment = "USE_CYTHON=1"
+environment = {USE_CYTHON="1"}
 build-verbosity = 3
```

### Comparing `qoi-0.5.0/setup.cfg` & `qoi-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `qoi-0.5.0/setup.py` & `qoi-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `qoi-0.5.0/src/qoi/benchmark.py` & `qoi-0.6.0/src/qoi/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 def bench_qoi(rgb, test_name, warmup=3, tests=10):
     encode_ms, bites = timeit(lambda: qoi.encode(rgb), warmup=warmup, tests=tests)
     decode_ms, decoded = timeit(lambda: qoi.decode(bites), warmup=warmup, tests=tests)
     yield TestResult(
         "qoi",
         test=test_name,
         format="qoi",
-        raw_size=np.product(rgb.shape),
+        raw_size=np.prod(rgb.shape),
         encode_ms=encode_ms,
         encode_size=len(bites),
         decode_ms=decode_ms,
         img_similarity=img_similarity(rgb, decoded, channel_axis=2),
     )
 
 
@@ -91,15 +91,15 @@
         return cv2.resize(qoi.decode(bites), dsize=None, fx=1 / scale, fy=1 / scale)
 
     decode_ms, decoded = timeit(decode, warmup=warmup, tests=tests)
     yield TestResult(
         f"qoi-lossy-{scale:0.2f}x{scale:0.2f}",
         test=test_name,
         format="qoi",
-        raw_size=np.product(rgb.shape),
+        raw_size=np.prod(rgb.shape),
         encode_ms=encode_ms,
         encode_size=len(bites),
         decode_ms=decode_ms,
         img_similarity=img_similarity(rgb, decoded, channel_axis=2),
     )
 
 
@@ -108,15 +108,14 @@
 
     fmts = []
     if jpg:
         fmts.append("JPEG")
     if png:
         fmts.append("PNG")
     for fmt in fmts:
-
         if fmt == "JPEG":
             format = f"jpg @ {jpeg_quality}"
 
             def encode():
                 bites = io.BytesIO()
                 img.save(bites, format=fmt, quality=jpeg_quality)
                 return bites.getbuffer()
@@ -132,30 +131,29 @@
         encode_ms, bites = timeit(encode, warmup=warmup, tests=tests)
         bites_ = io.BytesIO(bites)
         decode_ms, decoded = timeit(lambda: np.asarray(Image.open(bites_)), warmup=warmup, tests=tests)
         yield TestResult(
             "PIL",
             test=test_name,
             format=format,
-            raw_size=np.product(rgb.shape),
+            raw_size=np.prod(rgb.shape),
             encode_ms=encode_ms,
             encode_size=len(bites),
             decode_ms=decode_ms,
             img_similarity=img_similarity(rgb, decoded, channel_axis=2),
         )
 
 
 def bench_opencv(rgb, test_name, warmup=3, tests=10, jpg=True, png=True, jpeg_quality=80):
     exts = []
     if jpg:
         exts.append(".jpg")
     if png:
         exts.append(".png")
     for ext in exts:
-
         # Don't worry about RGB -> BGR as if we're using opencv we'd be using BGR anyway
         if ext == ".jpg":
             format = f"jpg @ {jpeg_quality}"
 
             def encode():
                 return cv2.imencode(ext, rgb, [int(cv2.IMWRITE_JPEG_QUALITY), jpeg_quality])[1].tobytes()
 
@@ -169,15 +167,15 @@
         decode_ms, decoded = timeit(
             lambda: cv2.imdecode(np.frombuffer(bites, np.uint8), cv2.IMREAD_COLOR), warmup=warmup, tests=tests
         )
         yield TestResult(
             "opencv",
             test=test_name,
             format=format,
-            raw_size=np.product(rgb.shape),
+            raw_size=np.prod(rgb.shape),
             encode_ms=encode_ms,
             encode_size=len(bites),
             decode_ms=decode_ms,
             img_similarity=img_similarity(rgb, decoded, channel_axis=2),
         )
 
 
@@ -202,15 +200,14 @@
     if qoi and (implementations is None or "qoi" in implementations):
         yield from bench_qoi(rgb, test_name=name, warmup=warmup, tests=tests)
     if qoi and (implementations is None or "qoi-lossy" in implementations) and OPENCV_AVAILABLE:
         yield from bench_qoi_lossy(rgb, test_name=name, warmup=warmup, tests=tests, scale=qoi_lossy_scale)
 
 
 def totable(results: List[TestResult]):
-
     # Sort:
     results = sorted(results, key=lambda x: (x.test, x.method, x.format))
 
     pretty_names = OrderedDict(
         test="Test image",
         method="Method",
         format="Format",
```

### Comparing `qoi-0.5.0/src/qoi/koi.png` & `qoi-0.6.0/src/qoi/koi.png`

 * *Files identical despite different names*

### Comparing `qoi-0.5.0/src/qoi/phoboslab_qoi/qoi.h` & `qoi-0.6.0/src/qoi/phoboslab_qoi/qoi.h`

 * *Files identical despite different names*

### Comparing `qoi-0.5.0/src/qoi/qoi.c` & `qoi-0.6.0/src/qoi/qoi.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.6 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "QOI_MALLOC",
@@ -53,18 +53,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_6" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030006F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -148,14 +148,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -209,14 +211,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -270,60 +274,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -406,14 +433,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -598,22 +628,22 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
         #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
         Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
@@ -663,15 +693,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -749,16 +779,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1102,15 +1137,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1189,15 +1224,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1305,32 +1340,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1372,15 +1390,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1662,195 +1680,195 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":735
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":735
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":742
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":742
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":746
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":747
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":747
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":756
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":762
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":762
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1893,42 +1911,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_3qoi_3qoi_PixelWrapper;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":772
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":775
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":775
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1936,15 +1954,15 @@
 struct __pyx_opt_args_3qoi_3qoi_read;
 struct __pyx_opt_args_3qoi_3qoi_encode;
 struct __pyx_opt_args_3qoi_3qoi_decode;
 
 /* "qoi/qoi.pyx":31
  *         PyMem_RawFree(self.pixels)
  * 
- * cpdef int write(filename, unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:             # <<<<<<<<<<<<<<
+ * cpdef int write(filename, const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:             # <<<<<<<<<<<<<<
  *     cdef bytes filename_bytes
  *     cdef const char* _filename
  */
 struct __pyx_opt_args_3qoi_3qoi_write {
   int __pyx_n;
   PyObject *colorspace;
 };
@@ -1961,15 +1979,15 @@
   int channels;
   __Pyx_memviewslice colorspace;
 };
 
 /* "qoi/qoi.pyx":86
  *             PyMem_RawFree(pixels)
  * 
- * cpdef bytes encode(unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):             # <<<<<<<<<<<<<<
+ * cpdef bytes encode(const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):             # <<<<<<<<<<<<<<
  *     cdef qoi.qoi_desc desc
  *     cdef int ret, size
  */
 struct __pyx_opt_args_3qoi_3qoi_encode {
   int __pyx_n;
   PyObject *colorspace;
 };
@@ -2308,16 +2326,16 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
@@ -2325,16 +2343,17 @@
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
     CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
   #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
   #endif
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2808,30 +2827,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_6
-#define __PYX_HAVE_RT_ImportType_proto_3_0_6
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_6(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_6(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_6 {
-   __Pyx_ImportType_CheckSize_Error_3_0_6 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_6 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_6 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_6(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_6 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Py3UpdateBases.proto */
 static PyObject* __Pyx_PEP560_update_bases(PyObject *bases);
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
@@ -2952,15 +2971,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -3076,15 +3095,15 @@
                 int ndim,
                 __Pyx_TypeInfo *dtype,
                 __Pyx_BufFmt_StackElem stack[],
                 __Pyx_memviewslice *memviewslice,
                 PyObject *original_obj);
 
 /* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_d_dc_unsigned_char(PyObject *, int writable_flag);
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_d_dc_unsigned_char__const__(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_unsigned_char(PyObject *, int writable_flag);
 
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_unsigned_char(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_unsigned_char(const char *itemp, PyObject *obj);
@@ -3352,16 +3371,16 @@
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
 /* #### Code section: typeinfo ### */
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_3qoi_3qoi_DTYPE_t = { "DTYPE_t", NULL, sizeof(__pyx_t_3qoi_3qoi_DTYPE_t), { 0 }, 0, __PYX_IS_UNSIGNED(__pyx_t_3qoi_3qoi_DTYPE_t) ? 'U' : 'I', __PYX_IS_UNSIGNED(__pyx_t_3qoi_3qoi_DTYPE_t), 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_unsigned_char = { "unsigned char", NULL, sizeof(unsigned char), { 0 }, 0, __PYX_IS_UNSIGNED(unsigned char) ? 'U' : 'I', __PYX_IS_UNSIGNED(unsigned char), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_unsigned_char__const__ = { "const unsigned char", NULL, sizeof(unsigned char const ), { 0 }, 0, __PYX_IS_UNSIGNED(unsigned char const ) ? 'U' : 'I', __PYX_IS_UNSIGNED(unsigned char const ), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_unsigned_char = { "unsigned char", NULL, sizeof(unsigned char), { 0 }, 0, __PYX_IS_UNSIGNED(unsigned char) ? 'U' : 'I', __PYX_IS_UNSIGNED(unsigned char), 0 };
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "qoi.qoi"
 extern int __pyx_module_is_main_qoi__qoi;
 int __pyx_module_is_main_qoi__qoi = 0;
 
 /* Implementation of "qoi.qoi" */
 /* #### Code section: global_var ### */
@@ -18313,261 +18332,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":246
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":246
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":249
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":249
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":246
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":246
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":252
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":252
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":255
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":255
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":252
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":252
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":258
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":258
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":261
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":261
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":258
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":258
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":264
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":264
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":269
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":269
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":264
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":264
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":272
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":272
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":276
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":276
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":272
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":272
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":279
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":279
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":282
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":282
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":279
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":279
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":285
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":285
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":291
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":291
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":285
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":285
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18576,29 +18595,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":778
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":778
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 778, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18609,15 +18628,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18626,29 +18645,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":781
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":781
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 781, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18659,15 +18678,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18676,29 +18695,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":784
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":784
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 784, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18709,15 +18728,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18726,29 +18745,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":787
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":787
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 787, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18759,15 +18778,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18776,29 +18795,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":790
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 790, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18809,209 +18828,209 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":793
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":794
+    /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":794
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":793
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":796
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":796
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":971
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":971
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":977
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":978
+    /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":978
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":977
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":979
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19027,15 +19046,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19043,68 +19062,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":985
+      /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":985
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 985, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 986, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 987, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 987, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+    /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19112,15 +19131,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19135,15 +19154,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19159,15 +19178,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19175,68 +19194,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":991
+      /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":991
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 991, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 992, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 993, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 993, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+    /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19244,15 +19263,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19267,15 +19286,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19291,15 +19310,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19307,68 +19326,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":997
+      /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":997
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 997, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":998
+    /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":998
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 998, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":999
+      /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 999, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 999, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+    /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19376,15 +19395,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19399,170 +19418,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1002
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1002
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1002
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1002
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1017
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1017
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1017
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1017
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1032
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1032
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1032
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1032
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1042
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1042
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1042
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1049
+/* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1049
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1053
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1053
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1049
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19734,15 +19753,15 @@
 static void __pyx_pf_3qoi_3qoi_12PixelWrapper___dealloc__(struct __pyx_obj_3qoi_3qoi_PixelWrapper *__pyx_v_self) {
 
   /* "qoi/qoi.pyx":29
  * 
  *     def __dealloc__(self):
  *         PyMem_RawFree(self.pixels)             # <<<<<<<<<<<<<<
  * 
- * cpdef int write(filename, unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:
+ * cpdef int write(filename, const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:
  */
   PyMem_RawFree(__pyx_v_self->pixels);
 
   /* "qoi/qoi.pyx":28
  *         return ndarray
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
@@ -19968,15 +19987,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "qoi/qoi.pyx":31
  *         PyMem_RawFree(self.pixels)
  * 
- * cpdef int write(filename, unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:             # <<<<<<<<<<<<<<
+ * cpdef int write(filename, const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:             # <<<<<<<<<<<<<<
  *     cdef bytes filename_bytes
  *     cdef const char* _filename
  */
 
 static PyObject *__pyx_pw_3qoi_3qoi_1write(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
@@ -20207,15 +20226,15 @@
  *         bytes_written = qoi.qoi_write(_filename, &rgb[0, 0, 0], &desc)             # <<<<<<<<<<<<<<
  *     if bytes_written == 0:
  *         raise RuntimeError("Failed to write!")
  */
         __pyx_t_9 = 0;
         __pyx_t_10 = 0;
         __pyx_t_11 = 0;
-        __pyx_v_bytes_written = qoi_write(__pyx_v__filename, (&(*((unsigned char *) ( /* dim=2 */ ((char *) (((unsigned char *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rgb.data + __pyx_t_9 * __pyx_v_rgb.strides[0]) ) + __pyx_t_10 * __pyx_v_rgb.strides[1]) )) + __pyx_t_11)) )))), (&__pyx_v_desc));
+        __pyx_v_bytes_written = qoi_write(__pyx_v__filename, (&(*((unsigned char const  *) ( /* dim=2 */ ((char *) (((unsigned char const  *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rgb.data + __pyx_t_9 * __pyx_v_rgb.strides[0]) ) + __pyx_t_10 * __pyx_v_rgb.strides[1]) )) + __pyx_t_11)) )))), (&__pyx_v_desc));
       }
 
       /* "qoi/qoi.pyx":55
  * 
  *     cdef int bytes_written
  *     with nogil:             # <<<<<<<<<<<<<<
  *         bytes_written = qoi.qoi_write(_filename, &rgb[0, 0, 0], &desc)
@@ -20274,15 +20293,15 @@
  */
   __pyx_r = __pyx_v_bytes_written;
   goto __pyx_L0;
 
   /* "qoi/qoi.pyx":31
  *         PyMem_RawFree(self.pixels)
  * 
- * cpdef int write(filename, unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:             # <<<<<<<<<<<<<<
+ * cpdef int write(filename, const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:             # <<<<<<<<<<<<<<
  *     cdef bytes filename_bytes
  *     cdef const char* _filename
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -20300,15 +20319,15 @@
 static PyObject *__pyx_pw_3qoi_3qoi_1write(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_3qoi_3qoi_write, "write(filename, unsigned char[:, :, ::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) -> int");
+PyDoc_STRVAR(__pyx_doc_3qoi_3qoi_write, "write(filename, const unsigned char[:, :, ::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) -> int");
 static PyMethodDef __pyx_mdef_3qoi_3qoi_1write = {"write", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3qoi_3qoi_1write, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_3qoi_3qoi_write};
 static PyObject *__pyx_pw_3qoi_3qoi_1write(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
@@ -20388,15 +20407,15 @@
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_filename = values[0];
-    __pyx_v_rgb = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc_unsigned_char(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_rgb.memview)) __PYX_ERR(1, 31, __pyx_L3_error)
+    __pyx_v_rgb = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc_unsigned_char__const__(values[1], 0); if (unlikely(!__pyx_v_rgb.memview)) __PYX_ERR(1, 31, __pyx_L3_error)
     __pyx_v_colorspace = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("write", 0, 2, 3, __pyx_nargs); __PYX_ERR(1, 31, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
@@ -20768,15 +20787,15 @@
       if (__pyx_t_3) {
 
         /* "qoi/qoi.pyx":84
  *     except:
  *         if pixels is not NULL:
  *             PyMem_RawFree(pixels)             # <<<<<<<<<<<<<<
  * 
- * cpdef bytes encode(unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):
+ * cpdef bytes encode(const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):
  */
         PyMem_RawFree(__pyx_v_pixels);
 
         /* "qoi/qoi.pyx":83
  *         return PixelWrapper().as_ndarray(desc.height, desc.width, desc.channels if channels == 0 else channels, pixels)
  *     except:
  *         if pixels is not NULL:             # <<<<<<<<<<<<<<
@@ -21006,15 +21025,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "qoi/qoi.pyx":86
  *             PyMem_RawFree(pixels)
  * 
- * cpdef bytes encode(unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):             # <<<<<<<<<<<<<<
+ * cpdef bytes encode(const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):             # <<<<<<<<<<<<<<
  *     cdef qoi.qoi_desc desc
  *     cdef int ret, size
  */
 
 static PyObject *__pyx_pw_3qoi_3qoi_5encode(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
@@ -21154,15 +21173,15 @@
  *         encoded = <char *>qoi.qoi_encode(&rgb[0, 0, 0], &desc, &size)             # <<<<<<<<<<<<<<
  *     if encoded is NULL or size <= 0:
  *         raise RuntimeError("Failed to encode!")
  */
         __pyx_t_5 = 0;
         __pyx_t_6 = 0;
         __pyx_t_7 = 0;
-        __pyx_v_encoded = ((char *)qoi_encode((&(*((unsigned char *) ( /* dim=2 */ ((char *) (((unsigned char *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rgb.data + __pyx_t_5 * __pyx_v_rgb.strides[0]) ) + __pyx_t_6 * __pyx_v_rgb.strides[1]) )) + __pyx_t_7)) )))), (&__pyx_v_desc), (&__pyx_v_size)));
+        __pyx_v_encoded = ((char *)qoi_encode((&(*((unsigned char const  *) ( /* dim=2 */ ((char *) (((unsigned char const  *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rgb.data + __pyx_t_5 * __pyx_v_rgb.strides[0]) ) + __pyx_t_6 * __pyx_v_rgb.strides[1]) )) + __pyx_t_7)) )))), (&__pyx_v_desc), (&__pyx_v_size)));
       }
 
       /* "qoi/qoi.pyx":101
  *     # if not rgb.flags['C_CONTIGUOUS']:
  *     #     rgb = np.ascontiguousarray(rgb) # makes a contiguous copy of the numpy array so we can read memory directly
  *     with nogil:             # <<<<<<<<<<<<<<
  *         encoded = <char *>qoi.qoi_encode(&rgb[0, 0, 0], &desc, &size)
@@ -21293,15 +21312,15 @@
       goto __pyx_L0;
     }
   }
 
   /* "qoi/qoi.pyx":86
  *             PyMem_RawFree(pixels)
  * 
- * cpdef bytes encode(unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):             # <<<<<<<<<<<<<<
+ * cpdef bytes encode(const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):             # <<<<<<<<<<<<<<
  *     cdef qoi.qoi_desc desc
  *     cdef int ret, size
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -21317,15 +21336,15 @@
 static PyObject *__pyx_pw_3qoi_3qoi_5encode(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_3qoi_3qoi_4encode, "encode(unsigned char[:, :, ::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) -> bytes");
+PyDoc_STRVAR(__pyx_doc_3qoi_3qoi_4encode, "encode(const unsigned char[:, :, ::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) -> bytes");
 static PyMethodDef __pyx_mdef_3qoi_3qoi_5encode = {"encode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3qoi_3qoi_5encode, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_3qoi_3qoi_4encode};
 static PyObject *__pyx_pw_3qoi_3qoi_5encode(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
@@ -21390,15 +21409,15 @@
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_rgb = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc_unsigned_char(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_rgb.memview)) __PYX_ERR(1, 86, __pyx_L3_error)
+    __pyx_v_rgb = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc_unsigned_char__const__(values[0], 0); if (unlikely(!__pyx_v_rgb.memview)) __PYX_ERR(1, 86, __pyx_L3_error)
     __pyx_v_colorspace = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("encode", 0, 1, 2, __pyx_nargs); __PYX_ERR(1, 86, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
@@ -23238,26 +23257,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 987, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-g51l8uhy/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-djb17rtw/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 993, __pyx_L1_error)
@@ -23445,15 +23464,15 @@
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
   __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "qoi/qoi.pyx":31
  *         PyMem_RawFree(self.pixels)
  * 
- * cpdef int write(filename, unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:             # <<<<<<<<<<<<<<
+ * cpdef int write(filename, const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:             # <<<<<<<<<<<<<<
  *     cdef bytes filename_bytes
  *     cdef const char* _filename
  */
   __pyx_tuple__36 = PyTuple_Pack(3, __pyx_n_s_filename, __pyx_n_s_rgb, __pyx_n_s_colorspace); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(1, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__36);
   __Pyx_GIVEREF(__pyx_tuple__36);
   __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_qoi_qoi_pyx, __pyx_n_s_write, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(1, 31, __pyx_L1_error)
@@ -23472,15 +23491,15 @@
   __Pyx_GOTREF(__pyx_tuple__39);
   __Pyx_GIVEREF(__pyx_tuple__39);
   __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_qoi_qoi_pyx, __pyx_n_s_read, 61, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(1, 61, __pyx_L1_error)
 
   /* "qoi/qoi.pyx":86
  *             PyMem_RawFree(pixels)
  * 
- * cpdef bytes encode(unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):             # <<<<<<<<<<<<<<
+ * cpdef bytes encode(const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):             # <<<<<<<<<<<<<<
  *     cdef qoi.qoi_desc desc
  *     cdef int ret, size
  */
   __pyx_tuple__41 = PyTuple_Pack(2, __pyx_n_s_rgb, __pyx_n_s_colorspace); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__41);
   __Pyx_GIVEREF(__pyx_tuple__41);
   __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_qoi_qoi_pyx, __pyx_n_s_encode, 86, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(1, 86, __pyx_L1_error)
@@ -23760,41 +23779,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_6(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_6); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 203, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_6); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_6); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 230, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_6); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 829, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 831, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_6); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 869, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 203, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 230, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 829, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 831, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 869, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -24009,15 +24028,15 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("qoi", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(1, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to qoi pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "qoi" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(1, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
@@ -24756,15 +24775,15 @@
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_7) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "qoi/qoi.pyx":31
  *         PyMem_RawFree(self.pixels)
  * 
- * cpdef int write(filename, unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:             # <<<<<<<<<<<<<<
+ * cpdef int write(filename, const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:             # <<<<<<<<<<<<<<
  *     cdef bytes filename_bytes
  *     cdef const char* _filename
  */
   __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_QOIColorSpace); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_SRGB); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
@@ -24830,15 +24849,15 @@
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_read, __pyx_t_10) < 0) __PYX_ERR(1, 61, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "qoi/qoi.pyx":86
  *             PyMem_RawFree(pixels)
  * 
- * cpdef bytes encode(unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):             # <<<<<<<<<<<<<<
+ * cpdef bytes encode(const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):             # <<<<<<<<<<<<<<
  *     cdef qoi.qoi_desc desc
  *     cdef int ret, size
  */
   __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_QOIColorSpace); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_SRGB); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
@@ -25341,19 +25360,19 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
 CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
     Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
     PyObject *dict;
     dict = PyDict_New();
     if (unlikely(!dict))
@@ -25458,15 +25477,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -25477,15 +25496,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -25509,15 +25528,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -28591,18 +28610,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_6
-#define __PYX_HAVE_RT_ImportType_3_0_6
-static PyTypeObject *__Pyx_ImportType_3_0_6(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_6 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -28648,23 +28667,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_6 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_6 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -30011,15 +30030,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -30470,15 +30489,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -30828,26 +30847,26 @@
     retval = -1;
 no_fail:
     __Pyx_RefNannyFinishContext();
     return retval;
 }
 
 /* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_d_dc_unsigned_char(PyObject *obj, int writable_flag) {
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_d_dc_unsigned_char__const__(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
     int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_FOLLOW), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_FOLLOW), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
     int retcode;
     if (obj == Py_None) {
         result.memview = (struct __pyx_memoryview_obj *) Py_None;
         return result;
     }
     retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
                                                  (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 3,
-                                                 &__Pyx_TypeInfo_unsigned_char, stack,
+                                                 &__Pyx_TypeInfo_unsigned_char__const__, stack,
                                                  &result, obj);
     if (unlikely(retcode == -1))
         goto __pyx_fail;
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
```

### Comparing `qoi-0.5.0/src/qoi/qoi.pxd` & `qoi-0.6.0/src/qoi/qoi.pxd`

 * *Files identical despite different names*

### Comparing `qoi-0.5.0/src/qoi/qoi.pyx` & `qoi-0.6.0/src/qoi/qoi.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -24,37 +24,37 @@
         ndarray = np.PyArray_SimpleNewFromData(3, shape, np.NPY_UINT8, self.pixels)
         np.set_array_base(ndarray, self)
         return ndarray
 
     def __dealloc__(self):
         PyMem_RawFree(self.pixels)
 
-cpdef int write(filename, unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:
-    cdef bytes filename_bytes 
+cpdef int write(filename, const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB) except? -1:
+    cdef bytes filename_bytes
     cdef const char* _filename
     cdef qoi.qoi_desc desc
     cdef int ret
 
     if not isinstance(colorspace, QOIColorSpace):
         raise ValueError("colorspace should be an instance of QOIColorSpace")
     if not isinstance(filename, (str, Path)):
         raise ValueError("filename should be a str or Path")
 
     filename_bytes = str(filename).encode('utf8')
     _filename = filename_bytes
-    
+
     desc.height = <unsigned int>rgb.shape[0]
     desc.width = <unsigned int>rgb.shape[1]
     desc.channels = <unsigned char>rgb.shape[2]
     desc.colorspace = colorspace.value
-    
+
     # if not rgb.flags['C_CONTIGUOUS']:
         # Makes a contiguous copy of the numpy array so we can process bytes directly:
         # rgb = np.ascontiguousarray(rgb)
-    
+
     cdef int bytes_written
     with nogil:
         bytes_written = qoi.qoi_write(_filename, &rgb[0, 0, 0], &desc)
     if bytes_written == 0:
         raise RuntimeError("Failed to write!")
     return bytes_written
 
@@ -67,27 +67,27 @@
     cdef char* pixels
 
     if not isinstance(filename, (str, Path)):
         raise ValueError("filename should be a str or Path")
 
     filename_bytes = str(filename).encode('utf8')
     _filename = filename_bytes
-    
+
     with nogil:
         pixels = <char *>qoi.qoi_read(_filename, &desc, channels)
     if pixels is NULL:
         raise RuntimeError("Failed to read!")
     try:
         colorspace[0] = desc.colorspace
         return PixelWrapper().as_ndarray(desc.height, desc.width, desc.channels if channels == 0 else channels, pixels)
     except:
         if pixels is not NULL:
             PyMem_RawFree(pixels)
 
-cpdef bytes encode(unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):
+cpdef bytes encode(const unsigned char[:,:,::1] rgb, colorspace: QOIColorSpace = QOIColorSpace.SRGB):
     cdef qoi.qoi_desc desc
     cdef int ret, size
     cdef char * encoded
 
     if not isinstance(colorspace, QOIColorSpace):
         raise ValueError("colorspace should be an instance of QOIColorSpace")
```

### Comparing `qoi-0.5.0/src/qoi.egg-info/PKG-INFO` & `qoi-0.6.0/src/qoi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoi
-Version: 0.5.0
+Version: 0.6.0
 Summary: A simpler wrapper around qoi (https://github.com/phoboslab/qoi)
 Home-page: https://github.com/kodonnell/qoi
 Author: kodonnell
 Author-email: kodonnell@users.noreply.github.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kodonnell/qoi/issues
 Keywords: qoi
@@ -15,14 +15,16 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22.4
 Provides-Extra: dev
 Requires-Dist: Cython>=3.0.0; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pillow; extra == "dev"
+Requires-Dist: opencv-python-headless; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 [![PyPI version fury.io](https://badge.fury.io/py/qoi.svg)](https://pypi.python.org/pypi/qoi/)
 
 # QOI
 
@@ -40,15 +42,15 @@
 
 ## Example
 
 ```python
 import numpy as np
 import qoi
 
-# Get your image as a numpy array (OpenCV, Pillow, etc. but here we just create a bunch of noise)
+# Get your image as a numpy array (OpenCV, Pillow, etc. but here we just create a bunch of noise). Note: HWC ordering
 rgb = np.random.randint(low=0, high=255, size=(224, 244, 3)).astype(np.uint8)
 
 # Write it:
 _ = qoi.write("/tmp/img.qoi", rgb)
 
 # Read it and check it matches (it should, as we're lossless)
 rgb_read = qoi.read("/tmp/img.qoi")
@@ -104,20 +106,20 @@
 > NB:
 >
 > 1. There's additional overhead here with PIL images being converted back to an array as the return type, to be consistent. In some sense, this isn't fair, as PIL will be faster if you're dealing with PIL images. On the other hand, if your common use case involves arrays (e.g. for computer vision) then it's reasonable.
 > 2. Produced with `python src/qoi/benchmark.py --implementations=qoi,opencv,pil --formats=png,qoi` on an i7-9750H. Not going to the point of optimised OpenCV/PIL (e.g. SIMD, or `pillow-simd`) as the results are clear enough for this 'normal' scenario. If you want to dig further, go for it! You can easily run these tests yourself.
 
 If we consider lossy compression, again, JPEG is usually what we're comparing with. Normally, it'd be unfair to compare QOI with JPEG as QOI is lossless, however we can do a slight trick to make QOI lossy - downscale the image, then encode it, then upsample it by the same amount after decoding. You can see we've implemented that below with a downscaling to 40% and JPEG quality of 80 (which results in them having the same visual compression i.e. SSIM). So, results (only on `koi photo` as the rest are less meaningful/fair for lossy):
 
-| Test image                | Method              | Format   | Input (kb) | Encode (ms) | Encode (kb) | Decode (ms) | SSIM |
-| ------------------------- | ------------------- | -------- | ---------- | ----------- | ----------- | ----------- | ---- |
-| koi photo                 | PIL                 | jpg @ 80 | 6075.0     | 47.67       | 275.2       | 24.01       | 0.94 |
-| koi photo                 | opencv              | jpg @ 80 | 6075.0     | 24.03       | 275.3       | 19.58       | 0.94 |
-| koi photo                 | qoi                 | qoi      | 6075.0     | 23.17       | 3489.0      | 12.94       | 1.00 |
-| koi photo                 | qoi-lossy-0.40x0.40 | qoi      | 6075.0     | 4.38        | 667.5       | 2.96        | 0.94 |
+| Test image | Method              | Format   | Input (kb) | Encode (ms) | Encode (kb) | Decode (ms) | SSIM |
+| ---------- | ------------------- | -------- | ---------- | ----------- | ----------- | ----------- | ---- |
+| koi photo  | PIL                 | jpg @ 80 | 6075.0     | 47.67       | 275.2       | 24.01       | 0.94 |
+| koi photo  | opencv              | jpg @ 80 | 6075.0     | 24.03       | 275.3       | 19.58       | 0.94 |
+| koi photo  | qoi                 | qoi      | 6075.0     | 23.17       | 3489.0      | 12.94       | 1.00 |
+| koi photo  | qoi-lossy-0.40x0.40 | qoi      | 6075.0     | 4.38        | 667.5       | 2.96        | 0.94 |
 
 Here we see that lossless `qoi` is losing out considerably in compression, as expected for lossy vs lossless. Also, `qoi` is only 1x-2x faster of encoding, and 1.5x-2x faster for decoding. However, it's important to note that this varies a lot depending on the jpeg quality specified - here it's 80 but the default for OpenCV is actually 95 which is 3x worse compression and a bit slower.
 
 However, that's still lossy vs lossless! If you look at `qoi-lossy-0.40x0.40` where we downscale as above, you can see that it can perform really well. The compression ratio is now only 3x that of JPEG (and 5x better than lossless QOI, and also the same as the default OpenCV JPEG encoding at a quality of 95), but it's so fast - 5x-10x faster encoding, and 7x-8x faster decoding.
 
 Anyway, there are definitely use cases where `qoi` may still make sense over JPEG. Even lossless QOI can be worth it if size isn't an issue, as it's a bit faster. But if you use the "lossy" QOI, you're getting "comparable" (depending on JPEG quality) compression but much faster.
```

### Comparing `qoi-0.5.0/src/qoi.egg-info/SOURCES.txt` & `qoi-0.6.0/src/qoi.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 src/qoi.egg-info/dependency_links.txt
 src/qoi.egg-info/not-zip-safe
 src/qoi.egg-info/requires.txt
 src/qoi.egg-info/top_level.txt
 src/qoi/phoboslab_qoi/README.md
 src/qoi/phoboslab_qoi/qoi.h
 tests/test_multithread.py
-tests/test_qoi.py
+tests/test_qoi.py
+tests/test_ro_issue26.py
```

### Comparing `qoi-0.5.0/tests/test_multithread.py` & `qoi-0.6.0/tests/test_multithread.py`

 * *Files identical despite different names*

### Comparing `qoi-0.5.0/tests/test_qoi.py` & `qoi-0.6.0/tests/test_qoi.py`

 * *Files identical despite different names*

