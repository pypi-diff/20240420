# Comparing `tmp/fisspy-0.9.80.tar.gz` & `tmp/fisspy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fisspy-0.9.80.tar", last modified: Sun Jul 26 23:40:44 2020, max compression
+gzip compressed data, was "fisspy-1.0.0.tar", last modified: Sat Apr 20 03:14:42 2024, max compression
```

## Comparing `fisspy-0.9.80.tar` & `fisspy-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,58 @@
-drwxrwxrwx   0        0        0        0 2020-07-26 23:40:44.000000 fisspy-0.9.80/
--rw-rw-rw-   0        0        0      282 2020-07-26 23:40:44.000000 fisspy-0.9.80/PKG-INFO
--rw-rw-rw-   0        0        0     1253 2019-09-17 00:12:36.000000 fisspy-0.9.80/README.md
-drwxrwxrwx   0        0        0        0 2020-07-26 23:40:44.000000 fisspy-0.9.80/fisspy/
--rw-rw-rw-   0        0        0      381 2020-05-28 04:30:22.000000 fisspy-0.9.80/fisspy/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-26 23:40:44.000000 fisspy-0.9.80/fisspy/analysis/
--rw-rw-rw-   0        0        0      349 2019-09-17 00:12:36.000000 fisspy-0.9.80/fisspy/analysis/__init__.py
--rw-rw-rw-   0        0        0     7101 2020-05-28 04:30:22.000000 fisspy-0.9.80/fisspy/analysis/doppler.py
--rw-rw-rw-   0        0        0     1037 2020-05-28 04:30:22.000000 fisspy-0.9.80/fisspy/analysis/filter.py
--rw-rw-rw-   0        0        0     2730 2019-09-17 00:12:36.000000 fisspy-0.9.80/fisspy/analysis/forecast.py
--rw-rw-rw-   0        0        0    15571 2020-05-28 04:30:22.000000 fisspy-0.9.80/fisspy/analysis/ofe.py
--rw-rw-rw-   0        0        0    16259 2019-09-17 00:12:36.000000 fisspy-0.9.80/fisspy/analysis/tdmap.py
--rw-rw-rw-   0        0        0    34813 2020-07-26 23:23:21.000000 fisspy-0.9.80/fisspy/analysis/wavelet.py
--rw-rw-rw-   0        0        0    19322 2019-09-17 00:12:36.000000 fisspy-0.9.80/fisspy/cm.py
-drwxrwxrwx   0        0        0        0 2020-07-26 23:40:44.000000 fisspy-0.9.80/fisspy/data/
--rw-rw-rw-   0        0        0       94 2019-09-17 00:12:36.000000 fisspy-0.9.80/fisspy/data/__init__.py
--rw-rw-rw-   0        0        0     1134 2019-09-17 00:12:36.000000 fisspy-0.9.80/fisspy/data/_sample.py
--rw-rw-rw-   0        0        0      406 2019-09-17 00:12:36.000000 fisspy-0.9.80/fisspy/data/sample.py
-drwxrwxrwx   0        0        0        0 2020-07-26 23:40:44.000000 fisspy-0.9.80/fisspy/image/
--rw-rw-rw-   0        0        0       42 2019-09-17 00:12:36.000000 fisspy-0.9.80/fisspy/image/__init__.py
--rw-rw-rw-   0        0        0    15584 2020-05-28 04:30:22.000000 fisspy-0.9.80/fisspy/image/base.py
--rw-rw-rw-   0        0        0    30532 2020-05-28 04:30:22.000000 fisspy-0.9.80/fisspy/image/interactive_image.py
-drwxrwxrwx   0        0        0        0 2020-07-26 23:40:44.000000 fisspy-0.9.80/fisspy/io/
--rw-rw-rw-   0        0        0      330 2019-09-17 00:12:36.000000 fisspy-0.9.80/fisspy/io/__init__.py
--rw-rw-rw-   0        0        0    16346 2019-09-17 00:12:36.000000 fisspy-0.9.80/fisspy/io/read.py
--rw-rw-rw-   0        0        0     2849 2020-05-28 04:30:22.000000 fisspy-0.9.80/fisspy/makevideo.py
-drwxrwxrwx   0        0        0        0 2020-07-26 23:40:44.000000 fisspy-0.9.80/fisspy/read/
--rw-rw-rw-   0        0        0      218 2019-09-17 00:12:36.000000 fisspy-0.9.80/fisspy/read/__init__.py
--rw-rw-rw-   0        0        0    45066 2020-05-28 04:30:22.000000 fisspy-0.9.80/fisspy/read/read_factory.py
--rw-rw-rw-   0        0        0     6179 2020-05-28 04:30:22.000000 fisspy-0.9.80/fisspy/read/readbase.py
-drwxrwxrwx   0        0        0        0 2020-07-26 23:40:44.000000 fisspy-0.9.80/fisspy.egg-info/
--rw-rw-rw-   0        0        0      282 2020-07-26 23:40:44.000000 fisspy-0.9.80/fisspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2020-07-26 23:40:44.000000 fisspy-0.9.80/fisspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-26 23:40:44.000000 fisspy-0.9.80/fisspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-07-26 23:29:25.000000 fisspy-0.9.80/fisspy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      116 2020-07-26 23:40:44.000000 fisspy-0.9.80/fisspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2020-07-26 23:40:44.000000 fisspy-0.9.80/fisspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-07-26 23:40:44.000000 fisspy-0.9.80/setup.cfg
--rw-rw-rw-   0        0        0      615 2020-07-26 23:23:21.000000 fisspy-0.9.80/setup.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 03:14:42.298308 fisspy-1.0.0/
+-rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.0/LICENSE.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)      257 2024-04-20 03:14:42.298173 fisspy-1.0.0/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1195 2024-04-20 02:57:09.000000 fisspy-1.0.0/README.md
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 03:14:42.285107 fisspy-1.0.0/fisspy/
+-rw-r--r--   0 jhkang     (501) staff       (20)      386 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/__init__.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 03:14:42.287915 fisspy-1.0.0/fisspy/align/
+-rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/align/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    14644 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/align/alignment.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/align/base.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 03:14:42.290030 fisspy-1.0.0/fisspy/analysis/
+-rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/analysis/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/analysis/doppler.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/analysis/filter.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     3778 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/analysis/forecast.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/analysis/ofe.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    35499 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/analysis/tdmap.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    34055 2023-09-07 00:40:57.000000 fisspy-1.0.0/fisspy/analysis/wavelet.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.0/fisspy/cm.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 03:14:42.292060 fisspy-1.0.0/fisspy/correction/
+-rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/correction/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/correction/correction.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/correction/get_inform.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 03:14:42.293112 fisspy-1.0.0/fisspy/data/
+-rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.0/fisspy/data/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.0/fisspy/data/_sample.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.0/fisspy/data/download.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.0/fisspy/data/sample.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 03:14:42.294122 fisspy-1.0.0/fisspy/image/
+-rw-r--r--   0 jhkang     (501) staff       (20)      110 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/image/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12576 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/image/base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    29760 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/image/interactive_image.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     7860 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/image/raster_set.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 03:14:42.294478 fisspy-1.0.0/fisspy/inversion/
+-rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/inversion/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/inversion/_mlsi.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 03:14:42.294914 fisspy-1.0.0/fisspy/io/
+-rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.0/fisspy/io/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.0/fisspy/io/read.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/makevideo.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 03:14:42.296769 fisspy-1.0.0/fisspy/preprocess/
+-rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/preprocess/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    52473 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/preprocess/proc_base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)   143266 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/preprocess/proc_gui.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/preprocess/t_y_sh.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 03:14:42.297848 fisspy-1.0.0/fisspy/read/
+-rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/read/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    47710 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/read/read_factory.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     6813 2024-04-20 02:57:09.000000 fisspy-1.0.0/fisspy/read/readbase.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 03:14:42.287146 fisspy-1.0.0/fisspy.egg-info/
+-rw-r--r--   0 jhkang     (501) staff       (20)      257 2024-04-20 03:14:42.000000 fisspy-1.0.0/fisspy.egg-info/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1100 2024-04-20 03:14:42.000000 fisspy-1.0.0/fisspy.egg-info/SOURCES.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-20 03:14:42.000000 fisspy-1.0.0/fisspy.egg-info/dependency_links.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-20 03:04:24.000000 fisspy-1.0.0/fisspy.egg-info/not-zip-safe
+-rw-r--r--   0 jhkang     (501) staff       (20)      125 2024-04-20 03:14:42.000000 fisspy-1.0.0/fisspy.egg-info/requires.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-20 03:14:42.000000 fisspy-1.0.0/fisspy.egg-info/top_level.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-20 03:14:42.298358 fisspy-1.0.0/setup.cfg
+-rw-r--r--   0 jhkang     (501) staff       (20)      611 2024-04-20 02:57:09.000000 fisspy-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fisspy-0.9.80/fisspy/analysis/ofe.py` & `fisspy-1.0.0/fisspy/analysis/ofe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,381 +1,383 @@
-from __future__ import absolute_import, division
-import numpy as np
-from astropy.io import fits
-from scipy.signal import fftconvolve as conv
-from os import getcwd, mkdir, extsep
-from os.path import join, basename, dirname, isdir
-import matplotlib.pyplot as plt
-from matplotlib.gridspec import GridSpec
-from matplotlib.widgets import Slider
-
-__author__= "Juhyung Kang"
-__email__ = "jhkang@astro.snu.ac.kr"
-
-def runDAVE(data0, output=False, overwrite=False, fwhm=10, adv=1, source=0,
-            noise=1, winFunc='Gaussian', outSig=False):
-    """
-    Differential Affine Velocity Estimator for all spatial points.
-    This is the python function of dave_multi.pro IDL code written by J. Chae (2009).
-
-    Parameters
-    ----------
-    data0: `~numpy.ndarray` or fits file.
-        Three-dimensional input array with shape (nt, ny, nx) or
-        fits file with same dimension and shape.
-    output: `str`, optional
-        The name of the output fits file name.
-        If False, it makes OFE directory and write the *_dave.fits file.
-        Default is `False`.
-    fwhm: `int`, optional
-        FWHM of the window function (should be even positive integer)
-
-    Returns
-    -------
-    fits file:
-    """
-    if type(data0) == str:
-        data = fits.getdata(data0)
-        dirn = join(dirname(data0), 'ofe')
-        if not isdir(dirn):
-            mkdir(dirn)
-        fname = f'{basename(data0).split(extsep)[0]}_dave.fits'
-    else:
-        data = data0
-        dirn = getcwd()
-        fname = 'dave.fits'
-    if data.ndim != 3:
-        raise ValueError('data must be 3-D array.')
-    if not output:
-        output = join(dirn, fname)
-
-    dnt, dny, dnx = data.shape
-    psw = adv
-    qsw = source
-
-    # Construncting window function
-    winFunc = winFunc.capitalize()
-    h = int(fwhm/2)
-    if winFunc == 'Square':
-        mf = 1
-    else:
-        mf = 2
-    nx = 2*h*mf+1
-    ny = 2*h*mf+1
-    x = -(np.arange(nx)-nx//2)
-    y = -(np.arange(ny)-ny//2)
-
-    if winFunc == 'Square':
-        w = np.ones((ny, nx))
-    elif winFunc == 'Gaussian':
-        w = np.exp(-np.log(2)*((x/h)**2+(y[:,None]/h)**2))
-    elif winFunc == 'Hanning':
-        w = (1+np.cos(np.pi*x/h/2))*(1+np.cos(np.pi*y/h/2))/4
-    else:
-        raise ValueError("winFunc must be one of ('Square', 'Gaussian', "
-                         "'Hanning')")
-    w /= noise**2
-
-    # Construncting coefficent arrays
-    im = data
-    imT = (np.roll(im, -1, axis=0) - np.roll(im, 1, axis=0))/2
-    imY, imX = np.gradient(im, axis=(1, 2))
-
-    npar = 6+qsw
-    A = np.empty((npar, npar, dnt, dny, dnx))
-    A[0,0] = conv(imX*imX, w[None, :, :],
-                  'same', axes=(1, 2))                          # U0, U0
-    A[1,0] = A[0,1] = conv(imY*imX, w[None, :, :],
-                           'same', axes=(1, 2))                 # V0, U0
-    A[1,1] = conv(imY*imY, w[None, :, :],
-                  'same', axes=(1, 2))                          # V0, V0
-    A[2,0] = A[0,2] = conv(imX*imX, x*w[None, :, :],
-                           'same', axes=(1, 2)) \
-                    + psw*conv(imX*im, w[None, :, :],
-                               'same',axes=(1, 2))              # Ux, U0
-    A[2,1] = A[1,2] = conv(imX*imY, x*w[None, :, :],
-                           'same', axes=(1, 2)) \
-                    + psw*conv(imY*im, w[None, :, :],
-                               'same', axes=(1, 2))             # Ux, V0
-    A[2,2] = conv(imX*imX, x*x*w[None, :, :],
-                  'same', axes=(1, 2)) \
-           + 2*psw*conv(imX*im, x*w[None, :, :],
-                        'same', axes=(1, 2)) \
-           +  psw**2*conv(im*im, w[None, :, :],
-                          'same', axes=(1, 2))                  # Ux, Ux
-    A[3,0] = A[0,3] = conv(imY*imX, y[None,:,None]*w[None, :, :],
-                           'same', axes=(1, 2)) \
-                    + psw*conv(imX*im, w[None, :, :],
-                               'same', axes=(1, 2))             # Vy, U0
-    A[3,1] = A[1,3] = conv(imY*imY, y[None,:,None]*w[None, :, :],
-                           'same', axes=(1, 2)) \
-                    + psw*conv(imY*im, w[None, :, :],
-                               'same', axes=(1, 2))             # Vy, V0
-    A[3,2] = A[2,3] = conv(imY*imX, y[None,:,None]*x*w[None, :, :],
-                           'same', axes=(1, 2)) \
-                    + psw*conv(imY*im, y[None,:,None]*w[None, :, :],
-                               'same', axes=(1, 2)) + \
-                    + psw*conv(imX*im, x*w[None, :, :],
-                               'same', axes=(1, 2)) \
-                    + psw**2*conv(im*im, w[None, :, :],
-                                  'same', axes=(1, 2))          # Vy, Ux
-    A[3,3] = conv(imY*imY, y[None,:,None]*y[None,:,None]*w[None, :, :],
-                  'same', axes=(1, 2)) \
-           + 2*psw*conv(imY*im, y[None,:,None]*w[None, :, :],
-                        'same', axes=(1, 2)) \
-           + psw**2*conv(im*im, w[None, :, :],
-                         'same', axes=(1, 2))                   # Vy, Vy
-    A[4,0] = A[0,4] = conv(imX*imX, y[None,:,None]*w[None, :, :],
-                           'same', axes=(1, 2))                 # Uy, U0
-    A[4,1] = A[1,4] = conv(imX*imY, y[None,:,None]*w[None, :, :],
-                           'same', axes=(1, 2))                 # Uy, V0
-    A[4,2] = A[2,4] = conv(imX*imX, y[None,:,None]*x*w[None, :, :],
-                           'same', axes=(1, 2)) \
-                    + psw*conv(imX*im, y[None,:,None]*w[None, :, :],
-                               'same', axes=(1, 2))             # Uy, Ux
-    A[4,3] = A[3,4] = conv(imX*imY,
-                           y[None,:,None]*y[None,:,None]*w[None,:,:],
-                           'same', axes=(1, 2)) \
-                    + psw*conv(imX*im, y[None,:,None]*w[None,:,:],
-                               'same', axes=(1, 2))             # Uy, Vy
-    A[4,4] = conv(imX*imX, y[None,:,None]*y[None,:,None]*w[None,:,:],
-                  'same', axes=(1, 2))                          # Uy, Uy
-    A[5,0] = A[0,5] = conv(imY*imX, x*w[None,:,:],
-                           'same', axes=(1, 2))                 # Vx, U0
-    A[5,1] = A[1,5] = conv(imY*imY, x*w[None,:,:],
-                           'same', axes=(1, 2))                 # Vx, V0
-    A[5,2] = A[2,5] = conv(imY*imX, x*x*w[None,:,:],
-                           'same', axes=(1, 2)) \
-                    + psw*conv(im*imY, x*w[None,:,:],
-                               'same', axes=(1, 2))             # Vx, Ux
-    A[5,3] = A[3,5] = conv(imY*imY, x*y[None,:,None]*w[None,:,:],
-                           'same', axes=(1, 2)) \
-                    + psw*conv(im*imY, x*w[None,:,:],
-                               'same', axes=(1, 2))             # Vx, Vy
-    A[5,4] = A[4,5] = conv(imY*imX, x*y[None,:,None]*w[None,:,:],
-                           'same', axes=(1, 2))                 # Vx, Uy
-    A[5,5] = conv(imY*imY, x*x*w[None,:,:],
-                  'same', axes=(1, 2))                          #Vx, Vx
-
-    if qsw:
-        A[6,0] = A[0,6] = -qsw*conv(im*imX, w[None,:,:],
-                                    'same', axes=(1, 2))        # mu, U0
-        A[6,1] = A[1,6] = -qsw*conv(im*imY, w[None,:,:],
-                                    'same', axes=(1, 2))        # mu, V0
-        A[6,2] = A[2,6] = -qsw*conv(im*imX, x*w[None,:,:],
-                                    'same', axes=(1, 2)) \
-                        - qsw*psw*conv(im*im, w[None,:,:],
-                                       'same', axes=(1, 2))     # mu, Ux
-        A[6,3] = A[3,6] = -qsw*conv(im*imY, y[None,:,None]*w[None,:,:],
-                                    'same', axes=(1, 2)) \
-                        - qsw*psw*conv(im*im, w[None,:,:],
-                                       'same', axes=(1, 2))     # mu, Vy
-        A[6,4] = A[4,6] = -qsw*conv(im*imX, y[None,:,None]*w[None,:,:],
-                                    'same', axes=(1,2))         # mu, Uy
-        A[6,5] = A[5,6] = -qsw*conv(im*imY, x*w[None,:,:],
-                                    'same', axes=(1, 2))        # mu, Vx
-        A[6,6] = -qsw**2*conv(im*im, w[None,:,:],
-                              'same', axes=(1,2))               # mu, mu
-
-    B = np.empty((npar, dnt, dny, dnx))
-    B[0] = conv(imT*imX, -w[None,:,:], 'same', axes=(1,2))
-    B[1] = conv(imT*imY, -w[None,:,:], 'same', axes=(1,2))
-    B[2] = conv(imT*imX, -x*w[None,:,:], 'same', axes=(1,2)) \
-         + psw*conv(imT*im, -w[None,:,:], 'same', axes=(1,2))
-    B[3] = conv(imT*imY, -y[None,:,None]*w[None,:,:], 'same', axes=(1,2)) \
-         + psw*conv(imT*im, -w[None,:,:], 'same', axes=(1,2))
-    B[4] = conv(imT*imX, -y[None,:,None]*w[None,:,:], 'same', axes=(1,2))
-    B[5] = conv(imT*imY, -x*w[None,:,:], 'same', axes=(1,2))
-    if qsw:
-        B[6] = qsw*conv(imT*(-im), -w[None,:,:], 'same', axes=(1,2))
-
-    dave = np.linalg.solve(A.T, B.T).T
-
-
-    if not outSig:
-        hdu = fits.PrimaryHDU(dave)
-        hdu.header['type'] = 'DAVE'
-        hdu.writeto(output, overwrite=overwrite)
-#    else: #TODO sigma and chisq calculation
-    return output
-
-
-class readOFE:
-    def __init__(self, data0, ofeFile, scale=None, dt=None, gMethod=True):
-        """
-        Read the Optical Flow Estimated File.
-
-        Parameters
-        ----------
-        scale: float
-            Spatial pixel scale (arcsec).
-        """
-
-        if type(data0) == str:
-            data = fits.getdata(data0)
-            header = fits.getheader(data0)
-            nx = header['naxis1']
-            ny = header['naxis2']
-            cx = header['crval1']
-            cy = header['crval2']
-            cxp = header['crpix1']
-            cyp = header['crpix2']
-            dx = header['cdelt1']
-            dy = header['cdelt2']
-            dt = header['cdelt3']
-            l = -(cxp+0.5)*dx+cx
-            b = -(cyp+0.5)*dy+cy
-            r = (nx-(cxp+0.5))*dx+cx
-            t = (ny-(cyp+0.5))*dy+cy
-
-            scale = dx
-        else:
-            data = data0.copy()
-            l = -0.5
-            b = -0.5
-            r = nx-0.5
-            t = ny-0.5
-            dx = 1
-            dy = 1
-        self.extent = [l, r, b, t]
-        self.data = data
-        self.nt, self.ny, self.nx = self.data.shape
-
-        self._xarr = np.linspace(self.extent[0]+dx*0.5,
-                                 self.extent[1]-dx*0.5,
-                                 self.nx)
-        self._yarr = np.linspace(self.extent[2]+dy*0.5,
-                                 self.extent[3]-dy*0.5,
-                                 self.ny)
-
-        if self.data.ndim != 3:
-            raise ValueError("data must have 3 dimension")
-        if not scale or not dt:
-            raise KeyError("If data is an `~numpy.ndarray`, "
-                           "'scale' and 'dt' must be given.")
-        unit = scale*725/dt # km/s
-        self.ofe = fits.getdata(ofeFile)
-        self.oheader = fits.getheader(ofeFile)
-        self.otype = self.oheader['type']
-        self.U0 = self.ofe[0]*unit
-        self.V0 = self.ofe[1]*unit
-        self.Ux = self.ofe[2]*unit
-        self.Vy = self.ofe[3]*unit
-        self.Uy = self.ofe[4]*unit
-        self.Vx = self.ofe[5]*unit
-        self.C = np.arctan2(self.V0, self.U0)
-
-        if gMethod:
-            Uy, Ux = np.gradient(self.U0, axis=(1,2))
-            Vy, Vx = np.gradient(self.V0, axis=(1,2))
-        else:
-            Ux = self.Ux
-            Uy = self.Uy
-            Vx = self.Vx
-            Vy = self.Vy
-
-        self.div = Ux + Vy
-        self.curl = Vx - Uy
-
-    def imshow(self, t=1, div=True, curl=True, **kwargs):
-        """
-        Display an data with velocity vector field.
-
-        Parameters
-        ----------
-        t: int
-            Default is 1.
-        div: bool
-            If True, display divergence map.
-        curl: bool
-            If True, display curl map.
-        """
-
-        try:
-            plt.rcParams['keymap.back'].remove('left')
-            plt.rcParams['keymap.forward'].remove('right')
-        except:
-            pass
-
-        self.t = t
-        self._onDiv = div
-        self._onCurl = curl
-        kwargs['extent'] = kwargs.pop('extent', self.extent)
-        kwargs['origin'] = kwargs.pop('origin', 'lower')
-        width = kwargs.pop('width', 0.004)
-        scale = kwargs.pop('scale', 200)
-
-        if div or curl:
-            nw = div + curl + 1
-        else:
-            nw = 1
-        self.nw = nw
-        self.fig = plt.figure(self.otype, figsize=(6*nw,6), clear=True)
-        gs = GridSpec(11, nw, wspace=0, hspace=0)
-
-        self.axVec = self.fig.add_subplot(gs[:10, 0])
-        self.axSlider = self.fig.add_subplot(gs[10, :])
-        self.im = self.axVec.imshow(self.data[self.t], **kwargs)
-        self.vec = self.axVec.quiver(self._xarr, self._yarr,
-                                     self.U0[self.t],
-                                     self.V0[self.t],
-                                     self.C[self.t],
-                                     cmap=plt.cm.hsv,
-                                     width=width,
-                                     scale=scale)
-
-        self.axVec.set_title(r'$\mathbf{v}$')
-        self.axVec.set_xlabel('X')
-        self.axVec.set_ylabel('Y')
-        self.axVec.set_title(r'$\mathbf{v}$ field ' f'({self.otype})')
-        if div:
-            self.axDiv = self.fig.add_subplot(gs[:100, 1], sharex=self.axVec,
-                                              sharey=self.axVec)
-            self.imDiv = self.axDiv.imshow(self.div[self.t],
-                                           plt.cm.Seismic,
-                                           **kwargs)
-            self.axDiv.tick_params(labelbottom=False, labelleft=False)
-            self.axDiv.set_title(r'$\mathbf{\nabla} \cdot$'
-                                 r'$\mathbf{v}$')
-
-        if curl:
-            self.axCurl = self.fig.add_subplot(gs[:10, -1], sharex=self.axVec,
-                                               sharey=self.axVec)
-            self.imCurl = self.axCurl.imshow(self.curl[self.t],
-                                             plt.cm.PiYG,
-                                             **kwargs)
-            self.axCurl.tick_params(labelbottom=False, labelleft=False)
-            self.axCurl.set_title(r'$\mathbf{\nabla} \times \mathbf{V}$')
-
-        self.sT = Slider(self.axSlider, 'Time(pix)', 0, self.nt-1,
-                         valinit=self.t, valstep=1, valfmt="%i")
-        self.sT.on_changed(self._chTime)
-        self.fig.tight_layout()
-        self.fig.canvas.mpl_connect('key_press_event', self._onKey)
-
-    def _chTime(self, val):
-        self.t = int(self.sT.val)
-        self.im.set_data(self.data[self.t])
-        self.vec.set_UVC(self.U0[self.t], self.V0[self.t], self.C[self.t])
-        if self._onDiv:
-            self.imDiv.set_data(self.div[self.t])
-        if self._onCurl:
-            self.imCurl.set_data(self.curl[self.t])
-
-    def _onKey(self, event):
-        if event.key == 'left':
-            if self.t > 0:
-                self.t -= 1
-            else:
-                self.t = self.nt-1
-            self.sT.set_val(self.t)
-        elif event.key == 'right':
-            if self.t < self.nt-1:
-                self.t += 1
-            else:
-                self.t = 0
-            self.sT.set_val(self.t)
-
-
-
-
-#    def runNAVE():
+from __future__ import absolute_import, division
+import numpy as np
+from astropy.io import fits
+from scipy.signal import fftconvolve as conv
+from os import getcwd, mkdir, extsep
+from os.path import join, basename, dirname, isdir
+import matplotlib.pyplot as plt
+from matplotlib.gridspec import GridSpec
+from matplotlib.widgets import Slider
+
+__author__= "Juhyung Kang"
+__email__ = "jhkang@astro.snu.ac.kr"
+
+__all__ = ["runDAVE", "readOFE"]
+
+def runDAVE(data0, output=False, overwrite=False, fwhm=10, adv=1, source=0,
+            noise=1, winFunc='Gaussian', outSig=False):
+    """
+    Differential Affine Velocity Estimator for all spatial points.
+    This is the python function of dave_multi.pro IDL code written by J. Chae (2009).
+
+    Parameters
+    ----------
+    data0: `~numpy.ndarray` or fits file.
+        Three-dimensional input array with shape (nt, ny, nx) or
+        fits file with same dimension and shape.
+    output: `str`, optional
+        The name of the output fits file name.
+        If False, it makes OFE directory and write the *_dave.fits file.
+        Default is `False`.
+    fwhm: `int`, optional
+        FWHM of the window function (should be even positive integer)
+
+    Returns
+    -------
+    fits file:
+    """
+    if type(data0) == str:
+        data = fits.getdata(data0)
+        dirn = join(dirname(data0), 'ofe')
+        if not isdir(dirn):
+            mkdir(dirn)
+        fname = f'{basename(data0).split(extsep)[0]}_dave.fits'
+    else:
+        data = data0
+        dirn = getcwd()
+        fname = 'dave.fits'
+    if data.ndim != 3:
+        raise ValueError('data must be 3-D array.')
+    if not output:
+        output = join(dirn, fname)
+
+    dnt, dny, dnx = data.shape
+    psw = adv
+    qsw = source
+
+    # Construncting window function
+    winFunc = winFunc.capitalize()
+    h = int(fwhm/2)
+    if winFunc == 'Square':
+        mf = 1
+    else:
+        mf = 2
+    nx = 2*h*mf+1
+    ny = 2*h*mf+1
+    x = -(np.arange(nx)-nx//2)
+    y = -(np.arange(ny)-ny//2)
+
+    if winFunc == 'Square':
+        w = np.ones((ny, nx))
+    elif winFunc == 'Gaussian':
+        w = np.exp(-np.log(2)*((x/h)**2+(y[:,None]/h)**2))
+    elif winFunc == 'Hanning':
+        w = (1+np.cos(np.pi*x/h/2))*(1+np.cos(np.pi*y/h/2))/4
+    else:
+        raise ValueError("winFunc must be one of ('Square', 'Gaussian', "
+                         "'Hanning')")
+    w /= noise**2
+
+    # Construncting coefficent arrays
+    im = data
+    imT = (np.roll(im, -1, axis=0) - np.roll(im, 1, axis=0))/2
+    imY, imX = np.gradient(im, axis=(1, 2))
+
+    npar = 6+qsw
+    A = np.empty((npar, npar, dnt, dny, dnx))
+    A[0,0] = conv(imX*imX, w[None, :, :],
+                  'same', axes=(1, 2))                          # U0, U0
+    A[1,0] = A[0,1] = conv(imY*imX, w[None, :, :],
+                           'same', axes=(1, 2))                 # V0, U0
+    A[1,1] = conv(imY*imY, w[None, :, :],
+                  'same', axes=(1, 2))                          # V0, V0
+    A[2,0] = A[0,2] = conv(imX*imX, x*w[None, :, :],
+                           'same', axes=(1, 2)) \
+                    + psw*conv(imX*im, w[None, :, :],
+                               'same',axes=(1, 2))              # Ux, U0
+    A[2,1] = A[1,2] = conv(imX*imY, x*w[None, :, :],
+                           'same', axes=(1, 2)) \
+                    + psw*conv(imY*im, w[None, :, :],
+                               'same', axes=(1, 2))             # Ux, V0
+    A[2,2] = conv(imX*imX, x*x*w[None, :, :],
+                  'same', axes=(1, 2)) \
+           + 2*psw*conv(imX*im, x*w[None, :, :],
+                        'same', axes=(1, 2)) \
+           +  psw**2*conv(im*im, w[None, :, :],
+                          'same', axes=(1, 2))                  # Ux, Ux
+    A[3,0] = A[0,3] = conv(imY*imX, y[None,:,None]*w[None, :, :],
+                           'same', axes=(1, 2)) \
+                    + psw*conv(imX*im, w[None, :, :],
+                               'same', axes=(1, 2))             # Vy, U0
+    A[3,1] = A[1,3] = conv(imY*imY, y[None,:,None]*w[None, :, :],
+                           'same', axes=(1, 2)) \
+                    + psw*conv(imY*im, w[None, :, :],
+                               'same', axes=(1, 2))             # Vy, V0
+    A[3,2] = A[2,3] = conv(imY*imX, y[None,:,None]*x*w[None, :, :],
+                           'same', axes=(1, 2)) \
+                    + psw*conv(imY*im, y[None,:,None]*w[None, :, :],
+                               'same', axes=(1, 2)) + \
+                    + psw*conv(imX*im, x*w[None, :, :],
+                               'same', axes=(1, 2)) \
+                    + psw**2*conv(im*im, w[None, :, :],
+                                  'same', axes=(1, 2))          # Vy, Ux
+    A[3,3] = conv(imY*imY, y[None,:,None]*y[None,:,None]*w[None, :, :],
+                  'same', axes=(1, 2)) \
+           + 2*psw*conv(imY*im, y[None,:,None]*w[None, :, :],
+                        'same', axes=(1, 2)) \
+           + psw**2*conv(im*im, w[None, :, :],
+                         'same', axes=(1, 2))                   # Vy, Vy
+    A[4,0] = A[0,4] = conv(imX*imX, y[None,:,None]*w[None, :, :],
+                           'same', axes=(1, 2))                 # Uy, U0
+    A[4,1] = A[1,4] = conv(imX*imY, y[None,:,None]*w[None, :, :],
+                           'same', axes=(1, 2))                 # Uy, V0
+    A[4,2] = A[2,4] = conv(imX*imX, y[None,:,None]*x*w[None, :, :],
+                           'same', axes=(1, 2)) \
+                    + psw*conv(imX*im, y[None,:,None]*w[None, :, :],
+                               'same', axes=(1, 2))             # Uy, Ux
+    A[4,3] = A[3,4] = conv(imX*imY,
+                           y[None,:,None]*y[None,:,None]*w[None,:,:],
+                           'same', axes=(1, 2)) \
+                    + psw*conv(imX*im, y[None,:,None]*w[None,:,:],
+                               'same', axes=(1, 2))             # Uy, Vy
+    A[4,4] = conv(imX*imX, y[None,:,None]*y[None,:,None]*w[None,:,:],
+                  'same', axes=(1, 2))                          # Uy, Uy
+    A[5,0] = A[0,5] = conv(imY*imX, x*w[None,:,:],
+                           'same', axes=(1, 2))                 # Vx, U0
+    A[5,1] = A[1,5] = conv(imY*imY, x*w[None,:,:],
+                           'same', axes=(1, 2))                 # Vx, V0
+    A[5,2] = A[2,5] = conv(imY*imX, x*x*w[None,:,:],
+                           'same', axes=(1, 2)) \
+                    + psw*conv(im*imY, x*w[None,:,:],
+                               'same', axes=(1, 2))             # Vx, Ux
+    A[5,3] = A[3,5] = conv(imY*imY, x*y[None,:,None]*w[None,:,:],
+                           'same', axes=(1, 2)) \
+                    + psw*conv(im*imY, x*w[None,:,:],
+                               'same', axes=(1, 2))             # Vx, Vy
+    A[5,4] = A[4,5] = conv(imY*imX, x*y[None,:,None]*w[None,:,:],
+                           'same', axes=(1, 2))                 # Vx, Uy
+    A[5,5] = conv(imY*imY, x*x*w[None,:,:],
+                  'same', axes=(1, 2))                          #Vx, Vx
+
+    if qsw:
+        A[6,0] = A[0,6] = -qsw*conv(im*imX, w[None,:,:],
+                                    'same', axes=(1, 2))        # mu, U0
+        A[6,1] = A[1,6] = -qsw*conv(im*imY, w[None,:,:],
+                                    'same', axes=(1, 2))        # mu, V0
+        A[6,2] = A[2,6] = -qsw*conv(im*imX, x*w[None,:,:],
+                                    'same', axes=(1, 2)) \
+                        - qsw*psw*conv(im*im, w[None,:,:],
+                                       'same', axes=(1, 2))     # mu, Ux
+        A[6,3] = A[3,6] = -qsw*conv(im*imY, y[None,:,None]*w[None,:,:],
+                                    'same', axes=(1, 2)) \
+                        - qsw*psw*conv(im*im, w[None,:,:],
+                                       'same', axes=(1, 2))     # mu, Vy
+        A[6,4] = A[4,6] = -qsw*conv(im*imX, y[None,:,None]*w[None,:,:],
+                                    'same', axes=(1,2))         # mu, Uy
+        A[6,5] = A[5,6] = -qsw*conv(im*imY, x*w[None,:,:],
+                                    'same', axes=(1, 2))        # mu, Vx
+        A[6,6] = -qsw**2*conv(im*im, w[None,:,:],
+                              'same', axes=(1,2))               # mu, mu
+
+    B = np.empty((npar, dnt, dny, dnx))
+    B[0] = conv(imT*imX, -w[None,:,:], 'same', axes=(1,2))
+    B[1] = conv(imT*imY, -w[None,:,:], 'same', axes=(1,2))
+    B[2] = conv(imT*imX, -x*w[None,:,:], 'same', axes=(1,2)) \
+         + psw*conv(imT*im, -w[None,:,:], 'same', axes=(1,2))
+    B[3] = conv(imT*imY, -y[None,:,None]*w[None,:,:], 'same', axes=(1,2)) \
+         + psw*conv(imT*im, -w[None,:,:], 'same', axes=(1,2))
+    B[4] = conv(imT*imX, -y[None,:,None]*w[None,:,:], 'same', axes=(1,2))
+    B[5] = conv(imT*imY, -x*w[None,:,:], 'same', axes=(1,2))
+    if qsw:
+        B[6] = qsw*conv(imT*(-im), -w[None,:,:], 'same', axes=(1,2))
+
+    dave = np.linalg.solve(A.T, B.T).T
+
+
+    if not outSig:
+        hdu = fits.PrimaryHDU(dave)
+        hdu.header['type'] = 'DAVE'
+        hdu.writeto(output, overwrite=overwrite)
+#    else: #TODO sigma and chisq calculation
+    return output
+
+
+class readOFE:
+    def __init__(self, data0, ofeFile, scale=None, dt=None, gMethod=True):
+        """
+        Read the Optical Flow Estimated File.
+
+        Parameters
+        ----------
+        scale: float
+            Spatial pixel scale (arcsec).
+        """
+
+        if type(data0) == str:
+            data = fits.getdata(data0)
+            header = fits.getheader(data0)
+            nx = header['naxis1']
+            ny = header['naxis2']
+            cx = header['crval1']
+            cy = header['crval2']
+            cxp = header['crpix1']
+            cyp = header['crpix2']
+            dx = header['cdelt1']
+            dy = header['cdelt2']
+            dt = header['cdelt3']
+            l = -(cxp+0.5)*dx+cx
+            b = -(cyp+0.5)*dy+cy
+            r = (nx-(cxp+0.5))*dx+cx
+            t = (ny-(cyp+0.5))*dy+cy
+
+            scale = dx
+        else:
+            data = data0.copy()
+            l = -0.5
+            b = -0.5
+            r = nx-0.5
+            t = ny-0.5
+            dx = 1
+            dy = 1
+        self.extent = [l, r, b, t]
+        self.data = data
+        self.nt, self.ny, self.nx = self.data.shape
+
+        self._xarr = np.linspace(self.extent[0]+dx*0.5,
+                                 self.extent[1]-dx*0.5,
+                                 self.nx)
+        self._yarr = np.linspace(self.extent[2]+dy*0.5,
+                                 self.extent[3]-dy*0.5,
+                                 self.ny)
+
+        if self.data.ndim != 3:
+            raise ValueError("data must have 3 dimension")
+        if not scale or not dt:
+            raise KeyError("If data is an `~numpy.ndarray`, "
+                           "'scale' and 'dt' must be given.")
+        unit = scale*725/dt # km/s
+        self.ofe = fits.getdata(ofeFile)
+        self.oheader = fits.getheader(ofeFile)
+        self.otype = self.oheader['type']
+        self.U0 = self.ofe[0]*unit
+        self.V0 = self.ofe[1]*unit
+        self.Ux = self.ofe[2]*unit
+        self.Vy = self.ofe[3]*unit
+        self.Uy = self.ofe[4]*unit
+        self.Vx = self.ofe[5]*unit
+        self.C = np.arctan2(self.V0, self.U0)
+
+        if gMethod:
+            Uy, Ux = np.gradient(self.U0, axis=(1,2))
+            Vy, Vx = np.gradient(self.V0, axis=(1,2))
+        else:
+            Ux = self.Ux
+            Uy = self.Uy
+            Vx = self.Vx
+            Vy = self.Vy
+
+        self.div = Ux + Vy
+        self.curl = Vx - Uy
+
+    def imshow(self, t=1, div=True, curl=True, **kwargs):
+        """
+        Display an data with velocity vector field.
+
+        Parameters
+        ----------
+        t: int
+            Default is 1.
+        div: bool
+            If True, display divergence map.
+        curl: bool
+            If True, display curl map.
+        """
+
+        try:
+            plt.rcParams['keymap.back'].remove('left')
+            plt.rcParams['keymap.forward'].remove('right')
+        except:
+            pass
+
+        self.t = t
+        self._onDiv = div
+        self._onCurl = curl
+        kwargs['extent'] = kwargs.pop('extent', self.extent)
+        kwargs['origin'] = kwargs.pop('origin', 'lower')
+        width = kwargs.pop('width', 0.004)
+        scale = kwargs.pop('scale', 200)
+
+        if div or curl:
+            nw = div + curl + 1
+        else:
+            nw = 1
+        self.nw = nw
+        self.fig = plt.figure(self.otype, figsize=(6*nw,6), clear=True)
+        gs = GridSpec(11, nw, wspace=0, hspace=0)
+
+        self.axVec = self.fig.add_subplot(gs[:10, 0])
+        self.axSlider = self.fig.add_subplot(gs[10, :])
+        self.im = self.axVec.imshow(self.data[self.t], **kwargs)
+        self.vec = self.axVec.quiver(self._xarr, self._yarr,
+                                     self.U0[self.t],
+                                     self.V0[self.t],
+                                     self.C[self.t],
+                                     cmap=plt.cm.hsv,
+                                     width=width,
+                                     scale=scale)
+
+        self.axVec.set_title(r'$\mathbf{v}$')
+        self.axVec.set_xlabel('X')
+        self.axVec.set_ylabel('Y')
+        self.axVec.set_title(r'$\mathbf{v}$ field ' f'({self.otype})')
+        if div:
+            self.axDiv = self.fig.add_subplot(gs[:100, 1], sharex=self.axVec,
+                                              sharey=self.axVec)
+            self.imDiv = self.axDiv.imshow(self.div[self.t],
+                                           plt.cm.Seismic,
+                                           **kwargs)
+            self.axDiv.tick_params(labelbottom=False, labelleft=False)
+            self.axDiv.set_title(r'$\mathbf{\nabla} \cdot$'
+                                 r'$\mathbf{v}$')
+
+        if curl:
+            self.axCurl = self.fig.add_subplot(gs[:10, -1], sharex=self.axVec,
+                                               sharey=self.axVec)
+            self.imCurl = self.axCurl.imshow(self.curl[self.t],
+                                             plt.cm.PiYG,
+                                             **kwargs)
+            self.axCurl.tick_params(labelbottom=False, labelleft=False)
+            self.axCurl.set_title(r'$\mathbf{\nabla} \times \mathbf{V}$')
+
+        self.sT = Slider(self.axSlider, 'Time(pix)', 0, self.nt-1,
+                         valinit=self.t, valstep=1, valfmt="%i")
+        self.sT.on_changed(self._chTime)
+        self.fig.tight_layout()
+        self.fig.canvas.mpl_connect('key_press_event', self._onKey)
+
+    def _chTime(self, val):
+        self.t = int(self.sT.val)
+        self.im.set_data(self.data[self.t])
+        self.vec.set_UVC(self.U0[self.t], self.V0[self.t], self.C[self.t])
+        if self._onDiv:
+            self.imDiv.set_data(self.div[self.t])
+        if self._onCurl:
+            self.imCurl.set_data(self.curl[self.t])
+
+    def _onKey(self, event):
+        if event.key == 'left':
+            if self.t > 0:
+                self.t -= 1
+            else:
+                self.t = self.nt-1
+            self.sT.set_val(self.t)
+        elif event.key == 'right':
+            if self.t < self.nt-1:
+                self.t += 1
+            else:
+                self.t = 0
+            self.sT.set_val(self.t)
+
+
+
+
+#    def runNAVE():
```

### Comparing `fisspy-0.9.80/fisspy/analysis/wavelet.py` & `fisspy-1.0.0/fisspy/analysis/wavelet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,921 +1,926 @@
-"""
-Calculate the wavelet and its significance.
-"""
-from __future__ import division, absolute_import
-import numpy as np
-from scipy.special._ufuncs import gamma, gammainc
-from scipy.optimize import fminbound as fmin
-from scipy.fftpack import fft, ifft
-
-__author__ = "Juhyeong Kang"
-__email__ =  "jhkang@astro.snu.ac.kr"
-
-__all__ = ['Wavelet', 'WaveCoherency']
-
-class Wavelet:
-    """
-    Compute the wavelet transform of the given data
-    with sampling rate dt.
-    
-    By default, the MORLET wavelet (k0=6) is used.
-    The wavelet basis is normalized to have total energy=1
-    at all scales.
-            
-    Parameters
-    ----------
-    data : `~numpy.ndarray`
-        The time series N-D array.
-    dt : `float`
-        The time step between each y values.
-        i.e. the sampling time.
-    axis: `int`
-        The axis number to apply wavelet, i.e. temporal axis.
-            * Default is 0
-    dj : `float` (optional)
-        The spacing between discrete scales.
-        The smaller, the better scale resolution.
-            * Default is 0.25
-    s0 : `float` (optional)
-        The smallest scale of the wavelet.  
-            * Default is :math:`2 \cdot dt`.
-    j : `int` (optional)
-        The number of scales minus one.
-        Scales range from :math:`s0` up to :math:`s_0\cdot 2^{j\cdot dj}`, to give
-        a total of :math:`j+1` scales.
-            * Default is :math:`j=\log_2{(\\frac{n dt}{s_0 dj})}`.
-    mother : `str` (optional)
-        The mother wavelet function.
-        The choices are 'MORLET', 'PAUL', or 'DOG'
-            * Default is **'MORLET'**
-    param  : `int` (optional)
-        The mother wavelet parameter.\n
-        For **'MORLET'** param is k0, default is **6**.\n
-        For **'PAUL'** param is m, default is **4**.\n
-        For **'DOG'** param is m, default is **2**.\n
-    pad : `bool` (optional)
-        If set True, pad time series with enough zeros to get
-        N up to the next higher power of 2.
-        This prevents wraparound from the end of the time series
-        to the beginning, and also speeds up the FFT's 
-        used to do the wavelet transform.
-        This will not eliminate all edge effects.
-    
-    Notes
-    -----
-        This function based on the IDL code WAVELET.PRO written by C. Torrence, 
-        and Python code waveletFuncitions.py written by E. Predybayalo.
-    
-    References
-    ----------
-    Torrence, C. and Compo, G. P., 1998, A Practical Guide to Wavelet Analysis, 
-    *Bull. Amer. Meteor. Soc.*, `79, 61-78 <http://paos.colorado.edu/research/wavelets/bams_79_01_0061.pdf>`_.\n
-    http://paos.colorado.edu/research/wavelets/
-    
-    Example
-    -------
-    >>> from fisspy.analysis import wavelet
-    >>> res = wavelet.wavelet(data,dt,dj=dj,j=j,mother=mother,pad=True)
-    >>> wavelet = res.wavelet
-    >>> period = res.period
-    >>> scale = res.scale
-    >>> coi = res.coi
-    >>> power = res.power
-    >>> gws = res.gws
-    >>> res.plot()
-    """
-    
-    def __init__(self, data, dt, axis=0, dj=0.1, s0=None, j=None,
-                 mother='MORLET', param=False, pad=True):
-
-        
-        shape0 = np.array(data.shape)
-        self.n0 = shape0[axis]
-        shape = np.delete(shape0, axis)
-        self.axis = axis
-        
-        if not s0:
-            s0 = 2*dt
-        if not j:
-            j = int(np.log2(self.n0*dt/s0)/dj)
-        else:
-            j=int(j)
-        
-        self.s0 = s0
-        self.j = j
-        self.dt = dt
-        self.dj = dj
-        self.mother = mother.upper()
-        self.param = param
-        self.pad = pad
-        self.axis = axis
-        self.data = data
-        self.ndim = data.ndim
-        
-        #padding
-        if pad:
-#            power = int(np.log2(self.n0)+0.4999)
-            power = int(np.log2(self.n0))
-            self.npad = 2**(power+1)-self.n0
-            self.n = self.n0 + self.npad
-        else:
-            self.n = self.n0
-        
-        #wavenumber
-        k1 = np.arange(1,self.n//2+1)*2.*np.pi/self.n/dt
-        k2 = -k1[:int((self.n-1)/2)][::-1]
-        k = np.concatenate(([0.],k1,k2))
-        
-        #Scale array
-        self.scale = self.s0*2**(np.arange(self.j+1,dtype=float)*dj)
-        
-        #base return
-        self._motherFunc(k)
-        self.coi *= self.dt*np.append(np.arange((self.n0+1)//2),
-                                      np.arange(self.n0//2-1,-1,-1))
-        
-        #array handeling
-        order_ini = np.arange(data.ndim)
-        o1 = np.delete(order_ini, axis)
-        o2 = np.concatenate([o1, [axis]])
-        tdata = data.transpose(o2)
-        indata = tdata.reshape([shape.prod(), self.n0])
-        
-        wshape = np.concatenate([shape, [self.j+1, self.n0]])
-        self.wavelet = np.empty(np.concatenate([[shape.prod()], [self.j+1, self.n0]]),
-                             dtype=complex)
-        for i, y in enumerate(indata):
-            self.wavelet[i] = self._getWavelet(y)[:,:self.n0]
-#        self.wavelet = self._getWavelet(indata)[:,:,:self.n0]
-        
-        
-        self.wavelet = self.wavelet.reshape(wshape)
-        self.power = np.abs(self.wavelet)**2
-        self.gws = self.power.mean(axis=-1)
-        
-    def _getWavelet(self, y):
-
-#        x = y - y.mean(axis=-1)[:,None]
-        x = y - y.mean(axis=-1)
-        
-        #reconstruct the time series to analyze if set pad
-        if self.pad:
-#            shape = y.shape
-#            self.padding = np.zeros([shape[0], self.npad])
-            self.padding = np.zeros(self.npad)
-            x = np.concatenate((x, self.padding), axis=-1)
-        
-        # FFT
-        fx = fft(x)
-        
-#        res = ifft(fx[:,None,:]*self.nowf)
-        res = ifft(fx*self.nowf)
-        return res
-        
-    
-    def iwavelet(self, wavelet, scale):
-        #%% should be revised (period range option)
-        """
-        Inverse the wavelet to get the time-series
-        
-        Parameters
-        ----------
-        wavelet : ~numpy.ndarray
-            wavelet.
-        
-        Returns
-        -------
-        iwave : ~numpy.ndarray
-            Inverse wavelet.
-        
-        Notes
-        -----
-            This function based on the IDL code WAVELET.PRO written by C. Torrence, 
-            and Python code waveletFuncitions.py written by E. Predybayalo.
-        
-        References
-        ----------
-        Torrence, C. and Compo, G. P., 1998, A Practical Guide to Wavelet Analysis, 
-        *Bull. Amer. Meteor. Soc.*, `79, 61-78 <http://paos.colorado.edu/research/wavelets/bams_79_01_0061.pdf>`_.\n
-        http://paos.colorado.edu/research/wavelets/
-            
-        Example
-        -------
-        >>> iwave = res.iwavelet(wavelet)
-        """
-        scale2=1/scale**0.5
-        
-        self._motherParam()
-        if self.cdelta == -1:
-            raise ValueError('Cdelta undefined, cannot inverse with this wavelet')
-        
-        if self.mother == 'MORLET':
-            psi0=np.pi**(-0.25)
-        elif self.mother == 'PAUL':
-            psi0=2**self.param*gamma(self.param+1)/(np.pi*gamma(2*self.param+1))**0.5
-        elif self.mother == 'DOG':
-            if not self.param:
-                self.param=2
-            if self.param==2:
-                psi0=0.867325
-            elif self.param==6:
-                psi0=0.88406
-        
-        iwave=self.dj*self.dt**0.5/(self.cdelta*psi0)*np.dot(scale2, wavelet.real)
-        return iwave
-    
-    def _motherFunc(self, k):
-        """
-        Compute the Fourier factor and period.
-        
-        Parameters
-        ----------
-        mother : str
-            A string, Equal to 'MORLET' or 'PAUL' or 'DOG'.
-        k : 1d ndarray
-            The Fourier frequencies at which to calculate the wavelet.
-        scale : ~numpy.ndarray
-            The wavelet scale.
-        param : int
-            The nondimensional parameter for the wavelet function.
-        
-        Returns
-        -------
-        nowf : ~numpy.ndarray
-            The nonorthogonal wavelet function.
-        period : ~numpy.ndarrary
-            The vecotr of "Fourier" periods (in time units)
-        fourier_factor : float
-            the ratio of Fourier period to scale.
-        coi : int
-            The cone-of-influence size at the scale.
-        
-        Notes
-        -----
-            This function based on the IDL code WAVELET.PRO written by C. Torrence, 
-            and Python code waveletFuncitions.py written by E. Predybayalo.
-        
-        References
-        ----------
-        Torrence, C. and Compo, G. P., 1998, A Practical Guide to Wavelet Analysis, 
-        *Bull. Amer. Meteor. Soc.*, `79, 61-78 <http://paos.colorado.edu/research/wavelets/bams_79_01_0061.pdf>`_.\n
-        http://paos.colorado.edu/research/wavelets/
-            
-        """
-        kp = k > 0.
-        scale2 = self.scale[:, None]
-        pi = np.pi
-        
-        if self.mother == 'MORLET':
-            if not self.param:
-                self.param = 6.
-            expn = -(scale2*k-self.param)**2/2.*kp
-            norm = pi**(-0.25)*(self.n*k[1]*scale2)**0.5
-            self.nowf = norm*np.exp(expn)*kp*(expn > -100.)
-            self.fourier_factor = 4*pi/(self.param+(2+self.param**2)**0.5)
-            self.coi = self.fourier_factor/2**0.5
-            
-        elif self.mother == 'PAUL':
-            if not self.param:
-                self.param = 4.
-            expn = -scale2*k*kp
-            norm = 2**self.param*(scale2*k[1]*self.n/(self.param*gamma(2*self.param)))**0.5
-            self.nowf = norm*np.exp(expn)*((scale2*k)**self.param)*kp*(expn > -100.)
-            self.fourier_factor = 4*pi/(2*self.param+1)
-            self.coi = self.fourier_factor*2**0.5
-            
-        elif self.mother == 'DOG':
-            if not self.param:
-                self.param = 2.
-            expn = -(scale2*k)**2/2.
-            norm = (scale2*k[1]*self.n/gamma(self.param+0.5))**0.5
-            self.nowf = -norm*1j**self.param*(scale2*k)**self.param*np.exp(expn)
-            self.fourier_factor = 2*pi*(2./(2*self.param+1))**0.5
-            self.coi = self.fourier_factor/2**0.5
-        else:
-            raise ValueError('Mother must be one of MORLET, PAUL, DOG\n'
-                             'mother = %s' %repr(self.mother))
-        self.period = self.scale*self.fourier_factor
-        self.freq = self.dt/self.period
-    
-    def _motherParam(self):
-        """
-        Get the some values for given mother function of wavelet.
-        
-        Parameters
-        ----------
-        mother : str
-        param : int
-            The nondimensional parameter for the wavelet function.
-            
-        Returns
-        -------
-        fourier_factor : float
-            the ratio of Fourier period to scale.
-        dofmin : float
-            Degrees of freedom for each point in the wavelet power.
-            (either 2 for MORLET and PAUL, or 1 for the DOG)
-        cdelta : float
-            Reconstruction factor.
-        gamma_fac : float
-            decorrelation factor for time averaging.
-        dj0 : float
-            factor for scale averaging.
-        
-        Notes
-        -----
-            This function based on the IDL code WAVELET.PRO written by C. Torrence, 
-            and Python code waveletFuncitions.py written by E. Predybayalo.
-        
-        References
-        ----------
-        Torrence, C. and Compo, G. P., 1998, A Practical Guide to Wavelet Analysis, 
-        *Bull. Amer. Meteor. Soc.*, `79, 61-78 <http://paos.colorado.edu/research/wavelets/bams_79_01_0061.pdf>`_.\n
-        http://paos.colorado.edu/research/wavelets/
-        
-            
-        """
-        if self.mother == 'MORLET':
-            self.dofmin=2.
-            if self.param == 6.:
-                self.cdelta = 0.776
-                self.gamma_fac = 2.32
-                self.dj0 = 0.60
-            else:
-                self.cdelta = -1
-                self.gamma_fac = -1
-                self.dj0 = -1
-        elif self.mother == 'PAUL':
-            if not self.param:
-                self.param = 4.
-            self.dofmin = 2.
-            if self.param == 4.:
-                self.cdelta = 1.132
-                self.gamma_fac = 1.17
-                self.dj0 = 1.5
-            else:
-                self.cdelta = -1
-                self.gamma_fac = -1
-                self.dj0 = -1
-        elif self.mother == 'DOG':
-            if not self.param:
-                self.param = 2.
-            self.dofmin = 1.
-            if self.param == 2.:
-                self.cdelta = 3.541
-                self.gamma_fac = 1.43
-                self.dj0 = 1.4
-            elif self.param ==6.:
-                self.cdelta = 1.966
-                self.gamma_fac = 1.37
-                self.dj0 = 0.97
-            else:
-                self.cdelta = -1
-                self.gamma_fac = -1
-                self.dj0 = -1
-        else:
-            raise ValueError('Mother must be one of MORLET, PAUL, DOG')
-        
-        
-    def saveWavelet(self, savename):
-        """
-        Save the wavelet spectrum as .npz file.
-        
-        Parameters
-        ----------
-        savename: `str`
-            filename to save the wavelet data.
-        
-        Example
-        -------
-        >>> res.saveWavelet(r'c:\test\wavelet.npz')
-        """
-        
-        np.savez(savename, wavelet=self.wavelet,
-                 period=self.period, scale=self.scale,
-                 coi=self.coi, dt=self.dt, dj=self.dj, axis=self.axis,
-                 s0=self.s0, j=self.j, mother=self.mother,
-                 param=self.param)
-        
-    def waveSignif(self, y, sigtest=0, lag1=0., siglvl=0.95, dof=-1,
-                    gws=False, confidence=False):
-        """
-        Compute the significance levels for a wavelet transform.
-        
-        Parameters
-        ----------
-        y : float or ~numpy.ndarray
-            The time series, or the variance of the time series.
-            If this is a single number, it is assumed to be the variance.
-        sigtest : (optional) int
-            Allowable values are 0, 1, or 2
-            if 0 (default), then just do a regular chi-square test
-                i.e. Eqn (18) from Torrence & Compo.
-            If 1, then do a "time-average" test, i.e. Eqn (23).
-                in this case, dof should be set to False,
-                the nuber of local wavelet spectra 
-                that were averaged together.
-                For the Global Wavelet Spectrum(GWS), this would be N,
-                where N is the number of points in y
-            If 2, then do a "scale-average" test, i.e. Eqns (25)-(28).
-                In this case, dof should be set to a two-element vector,
-                which gives the scale range that was averaged together.
-                e.g. if one scale-averaged scales between 2 and 8,
-                then dof=[2,8]
-        lag1 : (optional) float
-            LAG 1 Autocorrelation, used for signif levels.
-                * Default is 0.
-        siglvl : (optional) float
-            Significance level to use.
-                * Default is 0.95
-        dof : (optional) float
-            degrees-of-freedom for sgnif test.
-                * Default is -1, and it means the False.
-    
-                
-        Returns
-        -------
-        signif : ~numpy.ndarray
-                Significance levels as a function of scale.
-            
-        Notes
-        -----
-        IF SIGTEST=1, then DOF can be a vector (same length as SCALEs), 
-        in which case NA is assumed to vary with SCALE. 
-        This allows one to average different numbers of times 
-        together at different scales, or to take into account 
-        things like the Cone of Influence.\n
-        See discussion following Eqn (23) in Torrence & Compo.\n
-        This function based on the IDL code WAVE_SIGNIF.PRO written by C. Torrence, 
-        and Python code waveletFuncitions.py written by E. Predybayalo.
-        
-        References
-        ----------
-        Torrence, C. and Compo, G. P., 1998, A Practical Guide to Wavelet Analysis, 
-        *Bull. Amer. Meteor. Soc.*, `79, 61-78 <http://paos.colorado.edu/research/wavelets/bams_79_01_0061.pdf>`_.\n
-        http://paos.colorado.edu/research/wavelets/
-        
-        Example
-        -------
-        >>> signif=wavelet.wave_signif(y,dt,scale,2,mother='morlet',dof=[s1,s2],gws=gws)
-        
-        """
-        if len(np.atleast_1d(y)) == 1:
-            var = y
-        else:
-            var = np.var(y)
-        
-        j = len(self.scale)
-        
-        self._motherParam()
-        try:
-            len(gws)
-            fft_theor = gws.copy()
-        except:
-            fft_theor = (1-lag1**2)/(1-2*lag1*np.cos(self.freq*2*np.pi)+lag1**2)
-            fft_theor*=var
-    
-    
-        signif = fft_theor.copy()
-        
-        if sigtest == 0:
-            dof = self.dofmin
-            signif = fft_theor * self._chisquareInv(siglvl, dof)/dof
-            if confidence:
-                sig = (1.-siglvl)/2.
-                chisqr = dof/np.array((self._chisquareInv(1-sig, dof),
-                                       self._chisquareInv(sig, dof)))
-                signif = np.dot(chisqr[:,None], fft_theor[None,:])
-        elif sigtest == 1:
-            if self.gamma_fac == -1:
-                raise ValueError('gamma_fac(decorrelation facotr) not defined for '
-                                 'mother = %s with param = %s'
-                                 %(repr(self.mother), repr(self.param)))
-            if len(np.atleast_1d(dof)) != 1:
-                pass
-            elif dof == -1:
-                dof = np.zeros(j)+self.dofmin
-            else:
-                dof = np.zeros(j)+dof
-            dof[dof <= 1] = 1
-            dof = self.dofmin * (1 + (dof * self.dt/self.gamma_fac/self.scale)**2)**0.5
-            dof[dof <= self.dofmin] = self.dofmin
-            if not confidence:
-                for i in range(j):
-                    chisqr = self._chisquareInv(siglvl, dof[i]) / dof[i]
-                    signif[i] = chisqr * fft_theor[i]
-            else:
-                signif = np.empty(2,j)
-                sig = (1-siglvl)/2.
-                for i in range(j):
-                    chisqr = dof[i]/np.array((self._chisquareInv(1-sig,dof[i]),
-                                            self._chisquareInv(sig, dof[i])))
-                    signif[:,i] = fft_theor[i]*chisqr
-        elif sigtest == 2:
-            if len(dof) != 2:
-                raise ValueError('DOF must be set to [s1,s2], the range of scale-averages')
-            if self.cdelta == -1:
-                raise ValueError('cdelta & dj0 not defined for'
-                                 'mother = %s with param = %s' %(repr(self.mother), repr(self.param)))
-            dj= np.log2(self.scale[1] / self.scale[0])
-            s1 = dof[0]
-            s2 = dof[1]
-            avg = (self.period >= s1)*(self.period <= s2)
-            navg = avg.sum()
-            if not navg:
-                raise ValueError('No valid scales between %s and %s' %(repr(s1), repr(s2)))
-            s1 = self.scale[avg].min()
-            s2 = self.scale[avg].max()
-            savg = 1./(1./self.scale[avg]).sum()
-            smid = np.exp(0.5*np.log(s1*s2))
-            dof = (self.dofmin*navg*savg/smid)*(1+(navg*dj/self.dj0)**2)**0.5
-            fft_theor = savg*(fft_theor[avg]/self.scale[avg]).sum()
-            chisqr = self._chisquareInv(siglvl,dof)/dof
-            if confidence:
-                sig = (1-siglvl)/2.
-                chisqr = dof/np.array((self._chisquareInv(1-sig, dof),
-                                       self._chisquareInv(sig, dof)))
-            signif = (self.dj*self.dt/self.cdelta/savg)*fft_theor*chisqr
-        else:
-            raise ValueError('Sigtest must be 0,1, or 2')
-        self.signif = signif
-        return signif
-    
-    def _chisquareInv(self,p,v):
-        """
-        Inverse of chi-square cumulative distribution function(CDF).
-        
-        Parameters
-        ----------
-        p : float
-            probability
-        v : float
-            degrees of freedom of the chi-square distribution
-        
-        Returns
-        -------
-        x : float
-            the inverse of chi-square cdf
-            
-        Example
-        -------
-        >>> result = chisquare_inv(p,v)
-        
-        """
-        if not 0<p<1:
-            raise ValueError('p must be 0<p<1')
-        minv = 0.01
-        maxv = 1
-        x = 1
-        tolerance = 1e-4
-        while x+tolerance >= maxv:
-            maxv*=10.
-            x = fmin(self._chisquareSolve, minv, maxv, args=(p,v), xtol=tolerance)
-            minv = maxv
-        x*=v
-        return x
-        
-    def _chisquareSolve(self,xguess,p,v):
-        """
-        Chisqure_solve
-        
-        Return the difference between calculated percentile and P.
-        
-        Written January 1998 by C. Torrence
-        """
-        pguess = gammainc(v/2,v*xguess/2)
-        pdiff = np.abs(pguess - p)
-        if pguess >= 1-1e-4:
-            pdiff = xguess
-        return pdiff
-    
-    def plot(self, lag1=0., levels=None, time=None, title=[None,None,None,None], figsize=(9,8)):
-        """
-        Plot Time Series, Wavelet Power Spectrum, 
-        Global Power Spectrum and Scale-average Time Series.
-        
-        Parameters
-        ---------
-        lag1: (optional) `float`
-            LAG 1 Autocorrelation, used for signif levels.
-                * Default is 0.
-        levels: list
-            Contour levels to plot the wavelet spectrum.
-        time: `~numpy.ndarray`
-            time array.
-        title: list
-            title of the each figure.
-        figsize: tuple
-            figure size
-        
-        Example
-        -------
-        >>> ww = Wavelet(data, 0.25, dj=0.1, s0=0.25, j=9/0.1)
-        >>> ww.plot()
-        """
-        
-        import matplotlib.pyplot as plt
-        from matplotlib.gridspec import GridSpec
-        from matplotlib import ticker
-        
-        n = len(self.data)
-        gs = GridSpec(7, 4)
-        self.fig = plt.figure(figsize=figsize)
-        self.axData = self.fig.add_subplot(gs[0:2, :3])
-        self.axWavelet = self.fig.add_subplot(gs[2:5, :3], sharex=self.axData)
-        self.axGlobal = self.fig.add_subplot(gs[2:5, 3], sharey=self.axWavelet)
-        self.axScaleAvg = self.fig.add_subplot(gs[5:7, :3], sharex=self.axData)
-        periodMax = self.period.max()
-        periodMax = periodMax if periodMax<64 else 64
-        
-        if time is None:
-            time = self.dt*np.arange(n)
-        if levels is None:
-            levels = [0.05, 0.12,0.229,
-                      0.45]
-            
-        # Plot Time Series
-        if title[0] is None:
-            self.axData.set_title('a) Time Series')
-        else:
-            self.axData.set_title(title)
-        self.axData.set_ylabel('Value')
-        self.axData.minorticks_on()
-        self.axData.tick_params(which='both', direction='in')
-        self.pData = self.axData.plot(time, self.data,
-                                      color='k', lw=1.5)[0]
-        self.axData.set_xlim(time[0], time[-1])
-        
-        # Contour Plot Wavelet Power Spectrum
-        if title[1] is None:
-            self.axWavelet.set_title('b) Wavelet Power Spectrum')
-        else:
-            self.axWavelet.set_title(title)
-        self.axWavelet.set_ylabel('Period')
-        self.axWavelet.minorticks_on()
-        
-        self.axWavelet.tick_params(which='both', direction='in')
-        self.axWavelet.set_yscale('symlog', basey=2)
-        self.axWavelet.yaxis.set_major_formatter(ticker.ScalarFormatter())
-        self.axWavelet.ticklabel_format(axis='y',style='plain')
-        self.axWavelet.set_ylim(periodMax, 0.5)
-        
-        wpower = self.power/self.power.max()
-        self.contour = self.axWavelet.contourf(time, self.period,
-                                               wpower, len(levels),
-                                               colors=['w'])
-        self.contourIm = self.axWavelet.contourf(self.contour,
-                                                 levels=levels,
-                                                 cmap=plt.cm.Spectral_r, extend='max')
-        signif = self.waveSignif(self.data, sigtest=0, lag1=lag1, siglvl=0.90,
-                                 gws=self.gws)
-        sig90 = signif[:,None]
-        sig90 = self.power/sig90
-        
-        self.axWavelet.contour(time, self.period, sig90, [-99,1] ,colors='r')
-        self.axWavelet.fill_between(time, self.coi,
-                                    self.period.max(), color='grey',
-                                    alpha=0.4, hatch='x')
-        
-        # Plot Global Wavelet Spectrum
-        if title[2] is None:
-            self.axGlobal.set_title('c) Global')
-        else:
-            self.axGlobal.set_title(title)
-        self.axGlobal.set_xlabel('Power')
-        self.axGlobal.set_ylabel('')
-        self.axGlobal.set_yscale('symlog', basey=2)
-        self.axGlobal.minorticks_on()
-        self.axGlobal.yaxis.set_major_formatter(ticker.ScalarFormatter())
-        self.axGlobal.ticklabel_format(axis='y',style='plain')
-        self.axGlobal.tick_params(which='both', direction='in')
-        self.pGlobal = self.axGlobal.plot(self.gws, self.period,
-                                          color='k', lw=1.5)[0]
-        
-        
-        dof = n - self.scale
-#        lag1 = 0.72
-        gsig = self.waveSignif(self.data, sigtest=1, lag1=0,
-                               dof=dof)
-        self.pSig = self.axGlobal.plot(gsig,
-                                       self.period, 
-                                       'r--',
-                                       lw=1.5)
-        
-        
-        # Plot Scale-average Time Series
-        if title[3] is None:
-            self.axScaleAvg.set_title('d) Scale-average Time Series')
-        else:
-            self.axScaleAvg.set_title(title)
-        self.axScaleAvg.set_xlabel('Time')
-        self.axScaleAvg.set_ylabel('Avg')
-        self.axScaleAvg.minorticks_on()
-        self.axScaleAvg.tick_params(which='both', direction='in')
-        
-        period_mask = (self.period >= 2)*(self.period < 8)
-        power_norm = self.power/self.scale[:,None]
-        power_avg = self.dj*self.dt/self.cdelta*power_norm[period_mask,:].sum(0)
-        self.pScaleAvg = self.axScaleAvg.plot(time,
-                                              power_avg,
-                                              color='k',
-                                              lw=1.5)
-        
-        self.fig.tight_layout()
-
-
-
-
-
-
-
-class WaveCoherency:
-    def __init__(self, wave1, time1, scale1, wave2, time2, scale2,
-                 dt=False, dj=False, coi=False, nosmooth=False):
-        """
-        Compute the wavelet coherency between two time series.
-        
-        Parameters
-        ----------
-        wave1 : ~numpy.ndarray
-            Wavelet power spectrum for time series 1.
-        time1 : ~numpy.ndarray
-            A vector of times for time series 1.
-        scale1 : ~numpy.ndarray
-            A vector of scales for time series 1.
-        wave2 : ~numpy.ndarray
-            Wavelet power spectrum for time series 2.
-        time2 : ~numpy.ndarray
-            A vector of times for time series 2.
-        scale2 : ~numpy.ndarray
-            A vector of scales for time series 2.
-        dt : (optional) float
-            Amount of time between each Y value, i.e. the sampling time.
-                If not input, then calculated from time1[1]-time1[0]
-        dj : (optional) float
-            The spacing between discrete scales.
-                If not input, then calculated from scale1
-        coi : (optional) ~numpy.ndarray
-            The array of the cone-of influence.
-        nosmooth : (optional) bool
-            If True, then just compute the global_coher, global_phase, and
-            the unsmoothed cross_wavelet and return.
-        
-        Returns
-        -------
-            
-        cross_wavelet : ~numpy.ndarray
-            The cross wavelet between the time series.
-        time : ~numpy.ndarray
-            The time array given by the overlap of time1 and time2.
-        scale : ~numpy.ndarray
-            The scale array of scale indices, given by the overlap of 
-            scale1 and scale2.
-        wave_phase : ~numpy.ndarray
-            The phase difference between time series 1 and time series 2.
-        wave_coher : ~numpy.ndarray
-            The wavelet coherency, as a function of time and scale.
-        global_phase : ~numpy.ndarray
-            The global (or mean) phase averaged over all times.
-        global_coher : ~numpy.ndarray
-            The global (or mean) coherence averaged over all times.
-        power1 : ~numpy.ndarray
-            The wavelet power spectrum should be the same as wave1
-            if time1 and time2 are identical, otherwise it is only the
-            overlapping portion. If nosmooth is set,
-            then this is unsmoothed, otherwise it is smoothed.
-        power2 : ~numpy.ndarray
-            same as power 1 but for time series 2.
-        coi : ~numpy.ndarray
-            The array of the cone-of influence.
-            
-        Notes
-        -----
-            This function based on the IDL code WAVE_COHERENCY.PRO written by C. Torrence, 
-        
-        References
-        ----------
-        Torrence, C. and Compo, G. P., 1998, A Practical Guide to Wavelet Analysis, 
-        *Bull. Amer. Meteor. Soc.*, `79, 61-78 <http://paos.colorado.edu/research/wavelets/bams_79_01_0061.pdf>`_.\n
-        http://paos.colorado.edu/research/wavelets/
-        
-        Example
-        -------
-        >>> res = wavelet.WaveCoherency(wave1,time1,scale1,wave2,time2,scale2,\
-                                       dt,dj,coi=coi)
-        >>> cross_wave = res.cross_wavelet
-        >>> phase = res.wave_phase
-        >>> coher = res.wave_coher
-        >>> gCoher = res.global_coher
-        >>> gCross = res.global_cross
-        >>> gPhase = res.global_phase
-        >>> power1 = res.power1
-        >>> power2 = res.power2
-        >>> time_out = res.time
-        >>> scale_out = res.scale
-        """
-        if not dt: dt = time1[1]-time1[0]
-        if not dj: dj = np.log2(scale1[1]/scale1[0])
-        if time1 is time2:
-            t1s = 0
-            t1e = len(time1)
-            t2s = t1s
-            t2e = t1e
-        else:
-            otime_start = min([time1.min(),time2.min()])
-            otime_end = max([time1.max(),time2.max()])
-            t1 = np.where((time1 >= otime_start)*(time1 <= otime_end))[0]
-            t1s = t1[0]
-            t1e = t1[-1]+1
-            t2 = np.where((time2 >= otime_start)*(time2 <= otime_end))[0]
-            t2s = t2[0]
-            t2e = t2[-1]+1
-        
-        oscale_start = min([scale1.min(),scale2.min()])
-        oscale_end = max([scale1.max(),scale2.max()])
-        s1 = np.where((scale1 >= oscale_start)*(scale1 <= oscale_end))[0]
-        s2 = np.where((scale2 >= oscale_start)*(scale2 <= oscale_end))[0]
-        s1s = s1[0]
-        s1e = s1[-1]+1
-        s2s = s2[0]
-        s2e = s2[-1]+1
-        
-        self.cross_wavelet = wave1[s1s:s1e,t1s:t1e]*wave2[s2s:s2e,t2s:t2e].conj()
-        self.power1 = np.abs(wave1[s1s:s1e,t1s:t1e])**2
-        self.power2 = np.abs(wave2[s2s:s2e,t2s:t2e])**2
-        
-        self.time = time1[t1s:t1e]
-        self.scale = scale1[s1s:s1e]
-        nj = s1e-s1s
-        
-        global1 = self.power1.sum(1)
-        global2 = self.power2.sum(1)
-        self.global_cross = self.cross_wavelet.sum(1)
-        self.global_coher = np.abs(self.global_cross)**2/(global1*global2)
-        self.global_phase = np.arctan(self.global_cross.imag/self.global_cross.real)*180./np.pi
-        
-        if not nosmooth:
-            nt = (4*self.scale/dt)//2*4+1
-            nt2 = nt[:,None]
-            ntmax = nt.max()
-            g = np.arange(ntmax) * np.ones((nj,1))
-            wh = g >= nt2
-            time_wavelet = (g-nt2//2)*dt/self.scale[:,None]
-            wave_func = np.exp(-time_wavelet**2/2)
-            wave_func[wh] = 0
-            wave_func = (wave_func/wave_func.sum(1)[:,None]).real
-            self.cross_wavelet = _fastConv(self.cross_wavelet, wave_func, nt2)
-            self.power1 = _fastConv(self.power1, wave_func, nt2)
-            self.power2 = _fastConv(self.power2, wave_func, nt2)
-            scales = self.scale[:, None]
-            self.cross_wavelet /= scales
-            self.power1 /= scales
-            self.power2 /= scales
-            
-            nw = int(0.6/dj/2 + 0.5)*2-1
-            weight = np.ones(nw)/nw
-            self.cross_wavelet = _fastConv2(self.cross_wavelet, weight)
-            self.power1 = _fastConv2(self.power1,weight)
-            self.power2 = _fastConv2(self.power2,weight)
-            
-            self.wave_phase = 180./np.pi*np.arctan(self.cross_wavelet.imag/self.cross_wavelet.real)
-            power3=self.power1*self.power2
-            whp=power3 < 1e-9
-            power3[whp]=1e-9
-            self.wave_coher = (np.abs(self.cross_wavelet)**2/power3).real
-    
-
-
-def _fastConv(f, g, nt):
-    """
-    Fast convolution two given function f and g (method 1)
-    """
-    nf=f.shape
-    ng=g.shape
-    npad=2**(int(np.log2(max([nf[1],ng[1]])))+1)
-    wh1=np.arange(nf[0],dtype=int)
-    wh2=np.arange(nf[1],dtype=int)*np.ones((nf[0],1),dtype=int)-(nt.astype(int)-1)//2-1
-    pf=np.zeros([nf[0],npad],dtype=complex)
-    pg=np.zeros([nf[0],npad],dtype=complex)
-    pf[:,:nf[1]]=f
-    pg[:,:ng[1]]=g
-    conv=ifft(fft(pf)*fft(pg[:,::-1]))
-    result=conv[wh1,wh2.T].T
-    return result
-
-def _fastConv2(f, g):
-    """
-    Fast convolution two given function f and g (method2)
-    """
-    nf=f.shape
-    ng=len(g)
-    npad=2**(int(np.log2(max([nf[0],ng])))+1)
-    
-    wh1=np.arange(nf[1],dtype=int)
-    wh2=np.arange(nf[0],dtype=int)*np.ones((nf[1],1),dtype=int)+ng//2
-    pf=np.zeros([npad,nf[1]],dtype=complex)
-    pg=np.zeros([npad,nf[1]],dtype=complex)
-    pf[:nf[0],:]=f
-    pg[:ng,:]=g[:,np.newaxis]
-    conv=ifft(fft(pf,axis=0)*fft(pg,axis=0),axis=0)
-    result=conv[wh2.T,wh1]
+"""
+Calculate the wavelet and its significance.
+"""
+from __future__ import division, absolute_import
+import numpy as np
+from scipy.special._ufuncs import gamma, gammainc
+from scipy.optimize import fminbound as fmin
+from scipy.fftpack import fft, ifft
+
+__author__ = "Juhyeong Kang"
+__email__ =  "jhkang@astro.snu.ac.kr"
+
+__all__ = ['Wavelet', 'WaveCoherency']
+
+class Wavelet:
+    """
+    Compute the wavelet transform of the given data
+    with sampling rate dt.
+    
+    By default, the MORLET wavelet (k0=6) is used.
+    The wavelet basis is normalized to have total energy=1
+    at all scales.
+            
+    Parameters
+    ----------
+    data : `~numpy.ndarray`
+        The time series N-D array.
+    dt : `float`
+        The time step between each y values.
+        i.e. the sampling time.
+    axis: `int`
+        The axis number to apply wavelet, i.e. temporal axis.
+            * Default is 0
+    dj : `float` (optional)
+        The spacing between discrete scales.
+        The smaller, the better scale resolution.
+            * Default is 0.25
+    s0 : `float` (optional)
+        The smallest scale of the wavelet.  
+            * Default is :math:`2 \cdot dt`.
+    j : `int` (optional)
+        The number of scales minus one.
+        Scales range from :math:`s0` up to :math:`s_0\cdot 2^{j\cdot dj}`, to give
+        a total of :math:`j+1` scales.
+            * Default is :math:`j=\log_2{(\\frac{n dt}{s_0 dj})}`.
+    mother : `str` (optional)
+        The mother wavelet function.
+        The choices are 'MORLET', 'PAUL', or 'DOG'
+            * Default is **'MORLET'**
+    param  : `int` (optional)
+        The mother wavelet parameter.\n
+        For **'MORLET'** param is k0, default is **6**.\n
+        For **'PAUL'** param is m, default is **4**.\n
+        For **'DOG'** param is m, default is **2**.\n
+    pad : `bool` (optional)
+        If set True, pad time series with enough zeros to get
+        N up to the next higher power of 2.
+        This prevents wraparound from the end of the time series
+        to the beginning, and also speeds up the FFT's 
+        used to do the wavelet transform.
+        This will not eliminate all edge effects.
+    
+    Notes
+    -----
+        This function based on the IDL code WAVELET.PRO written by C. Torrence, 
+        and Python code waveletFuncitions.py written by E. Predybayalo.
+    
+    References
+    ----------
+    Torrence, C. and Compo, G. P., 1998, A Practical Guide to Wavelet Analysis, 
+    *Bull. Amer. Meteor. Soc.*, `79, 61-78 <http://paos.colorado.edu/research/wavelets/bams_79_01_0061.pdf>`_.\n
+    http://paos.colorado.edu/research/wavelets/
+    
+    Example
+    -------
+    >>> from fisspy.analysis import wavelet
+    >>> res = wavelet.wavelet(data,dt,dj=dj,j=j,mother=mother,pad=True)
+    >>> wavelet = res.wavelet
+    >>> period = res.period
+    >>> scale = res.scale
+    >>> coi = res.coi
+    >>> power = res.power
+    >>> gws = res.gws
+    >>> res.plot()
+    """
+    
+    def __init__(self, data, dt, axis=0, dj=0.1, s0=None, j=None,
+                 mother='MORLET', param=False, pad=True):
+
+        
+        shape0 = np.array(data.shape)
+        self.n0 = shape0[axis]
+        shape = np.delete(shape0, axis)
+        self.axis = axis
+        
+        if not s0:
+            s0 = 2*dt
+        if not j:
+            j = int(np.log2(self.n0*dt/s0)/dj)
+        else:
+            j=int(j)
+        
+        self.s0 = s0
+        self.j = j
+        self.dt = dt
+        self.dj = dj
+        self.mother = mother.upper()
+        self.param = param
+        self.pad = pad
+        self.axis = axis
+        self.data = data
+        self.ndim = data.ndim
+        
+        #padding
+        if pad:
+#            power = int(np.log2(self.n0)+0.4999)
+            power = int(np.log2(self.n0))
+            self.npad = 2**(power+1)-self.n0
+            self.n = self.n0 + self.npad
+        else:
+            self.n = self.n0
+        
+        #wavenumber
+        k1 = np.arange(1,self.n//2+1)*2.*np.pi/self.n/dt
+        k2 = -k1[:int((self.n-1)/2)][::-1]
+        k = np.concatenate(([0.],k1,k2))
+        
+        #Scale array
+        self.scale = self.s0*2**(np.arange(self.j+1,dtype=float)*dj)
+        
+        #base return
+        self._motherFunc(k)
+        self.coi *= self.dt*np.append(np.arange((self.n0+1)//2),
+                                      np.arange(self.n0//2-1,-1,-1))
+        
+        #array handeling
+        order_ini = np.arange(data.ndim)
+        o1 = np.delete(order_ini, axis)
+        o2 = np.concatenate([o1, [axis]])
+        tdata = data.transpose(o2)
+        indata = tdata.reshape([shape.prod(), self.n0])
+        
+        wshape = np.concatenate([shape, [self.j+1, self.n0]])
+        self.wavelet = np.empty(np.concatenate([[shape.prod()], [self.j+1, self.n0]]),
+                             dtype=complex)
+        for i, y in enumerate(indata):
+            self.wavelet[i] = self._getWavelet(y)[:,:self.n0]
+#        self.wavelet = self._getWavelet(indata)[:,:,:self.n0]
+        
+        
+        self.wavelet = self.wavelet.reshape(wshape)
+        self.power = np.abs(self.wavelet)**2
+        self.gws = self.power.mean(axis=-1)
+        
+    def _getWavelet(self, y):
+
+#        x = y - y.mean(axis=-1)[:,None]
+        x = y - y.mean(axis=-1)
+        
+        #reconstruct the time series to analyze if set pad
+        if self.pad:
+#            shape = y.shape
+#            self.padding = np.zeros([shape[0], self.npad])
+            self.padding = np.zeros(self.npad)
+            x = np.concatenate((x, self.padding), axis=-1)
+        
+        # FFT
+        fx = fft(x)
+        
+#        res = ifft(fx[:,None,:]*self.nowf)
+        res = ifft(fx*self.nowf)
+        return res
+        
+    
+    def iwavelet(self, wavelet, scale):
+        #%% should be revised (period range option)
+        """
+        Inverse the wavelet to get the time-series
+        
+        Parameters
+        ----------
+        wavelet : ~numpy.ndarray
+            wavelet.
+        
+        Returns
+        -------
+        iwave : ~numpy.ndarray
+            Inverse wavelet.
+        
+        Notes
+        -----
+            This function based on the IDL code WAVELET.PRO written by C. Torrence, 
+            and Python code waveletFuncitions.py written by E. Predybayalo.
+        
+        References
+        ----------
+        Torrence, C. and Compo, G. P., 1998, A Practical Guide to Wavelet Analysis, 
+        *Bull. Amer. Meteor. Soc.*, `79, 61-78 <http://paos.colorado.edu/research/wavelets/bams_79_01_0061.pdf>`_.\n
+        http://paos.colorado.edu/research/wavelets/
+            
+        Example
+        -------
+        >>> iwave = res.iwavelet(wavelet)
+        """
+        scale2=1/scale**0.5
+        
+        self._motherParam()
+        if self.cdelta == -1:
+            raise ValueError('Cdelta undefined, cannot inverse with this wavelet')
+        
+        if self.mother == 'MORLET':
+            psi0=np.pi**(-0.25)
+        elif self.mother == 'PAUL':
+            psi0=2**self.param*gamma(self.param+1)/(np.pi*gamma(2*self.param+1))**0.5
+        elif self.mother == 'DOG':
+            if not self.param:
+                self.param=2
+            if self.param==2:
+                psi0=0.867325
+            elif self.param==6:
+                psi0=0.88406
+        
+        iwave=self.dj*self.dt**0.5/(self.cdelta*psi0)*np.dot(scale2, wavelet.real)
+        return iwave
+    
+    def _motherFunc(self, k):
+        """
+        Compute the Fourier factor and period.
+        
+        Parameters
+        ----------
+        mother : str
+            A string, Equal to 'MORLET' or 'PAUL' or 'DOG'.
+        k : 1d ndarray
+            The Fourier frequencies at which to calculate the wavelet.
+        scale : ~numpy.ndarray
+            The wavelet scale.
+        param : int
+            The nondimensional parameter for the wavelet function.
+        
+        Returns
+        -------
+        nowf : ~numpy.ndarray
+            The nonorthogonal wavelet function.
+        period : ~numpy.ndarrary
+            The vecotr of "Fourier" periods (in time units)
+        fourier_factor : float
+            the ratio of Fourier period to scale.
+        coi : int
+            The cone-of-influence size at the scale.
+        
+        Notes
+        -----
+            This function based on the IDL code WAVELET.PRO written by C. Torrence, 
+            and Python code waveletFuncitions.py written by E. Predybayalo.
+        
+        References
+        ----------
+        Torrence, C. and Compo, G. P., 1998, A Practical Guide to Wavelet Analysis, 
+        *Bull. Amer. Meteor. Soc.*, `79, 61-78 <http://paos.colorado.edu/research/wavelets/bams_79_01_0061.pdf>`_.\n
+        http://paos.colorado.edu/research/wavelets/
+            
+        """
+        kp = k > 0.
+        scale2 = self.scale[:, None]
+        pi = np.pi
+        
+        if self.mother == 'MORLET':
+            if not self.param:
+                self.param = 6.
+            expn = -(scale2*k-self.param)**2/2.*kp
+            norm = pi**(-0.25)*(self.n*k[1]*scale2)**0.5
+            self.nowf = norm*np.exp(expn)*kp*(expn > -100.)
+            self.fourier_factor = 4*pi/(self.param+(2+self.param**2)**0.5)
+            self.coi = self.fourier_factor/2**0.5
+            
+        elif self.mother == 'PAUL':
+            if not self.param:
+                self.param = 4.
+            expn = -scale2*k*kp
+            norm = 2**self.param*(scale2*k[1]*self.n/(self.param*gamma(2*self.param)))**0.5
+            self.nowf = norm*np.exp(expn)*((scale2*k)**self.param)*kp*(expn > -100.)
+            self.fourier_factor = 4*pi/(2*self.param+1)
+            self.coi = self.fourier_factor*2**0.5
+            
+        elif self.mother == 'DOG':
+            if not self.param:
+                self.param = 2.
+            expn = -(scale2*k)**2/2.
+            norm = (scale2*k[1]*self.n/gamma(self.param+0.5))**0.5
+            self.nowf = -norm*1j**self.param*(scale2*k)**self.param*np.exp(expn)
+            self.fourier_factor = 2*pi*(2./(2*self.param+1))**0.5
+            self.coi = self.fourier_factor/2**0.5
+        else:
+            raise ValueError('Mother must be one of MORLET, PAUL, DOG\n'
+                             'mother = %s' %repr(self.mother))
+        self.period = self.scale*self.fourier_factor
+        self.freq = self.dt/self.period
+    
+    def _motherParam(self):
+        """
+        Get the some values for given mother function of wavelet.
+        
+        Parameters
+        ----------
+        mother : str
+        param : int
+            The nondimensional parameter for the wavelet function.
+            
+        Returns
+        -------
+        fourier_factor : float
+            the ratio of Fourier period to scale.
+        dofmin : float
+            Degrees of freedom for each point in the wavelet power.
+            (either 2 for MORLET and PAUL, or 1 for the DOG)
+        cdelta : float
+            Reconstruction factor.
+        gamma_fac : float
+            decorrelation factor for time averaging.
+        dj0 : float
+            factor for scale averaging.
+        
+        Notes
+        -----
+            This function based on the IDL code WAVELET.PRO written by C. Torrence, 
+            and Python code waveletFuncitions.py written by E. Predybayalo.
+        
+        References
+        ----------
+        Torrence, C. and Compo, G. P., 1998, A Practical Guide to Wavelet Analysis, 
+        *Bull. Amer. Meteor. Soc.*, `79, 61-78 <http://paos.colorado.edu/research/wavelets/bams_79_01_0061.pdf>`_.\n
+        http://paos.colorado.edu/research/wavelets/
+        
+            
+        """
+        self.cdelta = -1
+        self.gamma_fac = -1
+        self.dj0 = -1
+        if self.mother == 'MORLET':
+            self.dofmin=2.
+            if self.param == 6.:
+                self.cdelta = 0.776
+                self.gamma_fac = 2.32
+                self.dj0 = 0.60
+            elif self.param == 12:
+                self.cdelta = 0.38
+                self.dj0 = 0.60
+            elif self.param == 18:
+                self.cdelta = 0.27
+                self.dj0 = 0.60
+        elif self.mother == 'PAUL':
+            if not self.param:
+                self.param = 4.
+            self.dofmin = 2.
+            if self.param == 4.:
+                self.cdelta = 1.132
+                self.gamma_fac = 1.17
+                self.dj0 = 1.5
+            else:
+                self.cdelta = -1
+                self.gamma_fac = -1
+                self.dj0 = -1
+        elif self.mother == 'DOG':
+            if not self.param:
+                self.param = 2.
+            self.dofmin = 1.
+            if self.param == 2.:
+                self.cdelta = 3.541
+                self.gamma_fac = 1.43
+                self.dj0 = 1.4
+            elif self.param ==6.:
+                self.cdelta = 1.966
+                self.gamma_fac = 1.37
+                self.dj0 = 0.97
+            else:
+                self.cdelta = -1
+                self.gamma_fac = -1
+                self.dj0 = -1
+        else:
+            raise ValueError('Mother must be one of MORLET, PAUL, DOG')
+        
+        
+    def saveWavelet(self, savename):
+        """
+        Save the wavelet spectrum as .npz file.
+        
+        Parameters
+        ----------
+        savename: `str`
+            filename to save the wavelet data.
+        
+        Example
+        -------
+        >>> res.saveWavelet(r'c:\test\wavelet.npz')
+        """
+        
+        np.savez(savename, wavelet=self.wavelet,
+                 period=self.period, scale=self.scale,
+                 coi=self.coi, dt=self.dt, dj=self.dj, axis=self.axis,
+                 s0=self.s0, j=self.j, mother=self.mother,
+                 param=self.param)
+        
+    def waveSignif(self, y, sigtest=0, lag1=0., siglvl=0.95, dof=-1,
+                    gws=False, confidence=False):
+        """
+        Compute the significance levels for a wavelet transform.
+        
+        Parameters
+        ----------
+        y : float or ~numpy.ndarray
+            The time series, or the variance of the time series.
+            If this is a single number, it is assumed to be the variance.
+        sigtest : (optional) int
+            Allowable values are 0, 1, or 2
+            if 0 (default), then just do a regular chi-square test
+                i.e. Eqn (18) from Torrence & Compo.
+            If 1, then do a "time-average" test, i.e. Eqn (23).
+                in this case, dof should be set to False,
+                the nuber of local wavelet spectra 
+                that were averaged together.
+                For the Global Wavelet Spectrum(GWS), this would be N,
+                where N is the number of points in y
+            If 2, then do a "scale-average" test, i.e. Eqns (25)-(28).
+                In this case, dof should be set to a two-element vector,
+                which gives the scale range that was averaged together.
+                e.g. if one scale-averaged scales between 2 and 8,
+                then dof=[2,8]
+        lag1 : (optional) float
+            LAG 1 Autocorrelation, used for signif levels.
+                * Default is 0.
+        siglvl : (optional) float
+            Significance level to use.
+                * Default is 0.95
+        dof : (optional) float
+            degrees-of-freedom for sgnif test.
+                * Default is -1, and it means the False.
+    
+                
+        Returns
+        -------
+        signif : ~numpy.ndarray
+                Significance levels as a function of scale.
+            
+        Notes
+        -----
+        IF SIGTEST=1, then DOF can be a vector (same length as SCALEs), 
+        in which case NA is assumed to vary with SCALE. 
+        This allows one to average different numbers of times 
+        together at different scales, or to take into account 
+        things like the Cone of Influence.\n
+        See discussion following Eqn (23) in Torrence & Compo.\n
+        This function based on the IDL code WAVE_SIGNIF.PRO written by C. Torrence, 
+        and Python code waveletFuncitions.py written by E. Predybayalo.
+        
+        References
+        ----------
+        Torrence, C. and Compo, G. P., 1998, A Practical Guide to Wavelet Analysis, 
+        *Bull. Amer. Meteor. Soc.*, `79, 61-78 <http://paos.colorado.edu/research/wavelets/bams_79_01_0061.pdf>`_.\n
+        http://paos.colorado.edu/research/wavelets/
+        
+        Example
+        -------
+        >>> signif=wavelet.wave_signif(y,dt,scale,2,mother='morlet',dof=[s1,s2],gws=gws)
+        
+        """
+        if len(np.atleast_1d(y)) == 1:
+            var = y
+        else:
+            var = np.var(y)
+        
+        j = len(self.scale)
+        
+        self._motherParam()
+        try:
+            len(gws)
+            fft_theor = gws.copy()
+        except:
+            fft_theor = (1-lag1**2)/(1-2*lag1*np.cos(self.freq*2*np.pi)+lag1**2)
+            fft_theor*=var
+    
+    
+        signif = fft_theor.copy()
+        
+        if sigtest == 0:
+            dof = self.dofmin
+            signif = fft_theor * self._chisquareInv(siglvl, dof)/dof
+            if confidence:
+                sig = (1.-siglvl)/2.
+                chisqr = dof/np.array((self._chisquareInv(1-sig, dof),
+                                       self._chisquareInv(sig, dof)))
+                signif = np.dot(chisqr[:,None], fft_theor[None,:])
+        elif sigtest == 1:
+            if self.gamma_fac == -1:
+                raise ValueError('gamma_fac(decorrelation facotr) not defined for '
+                                 'mother = %s with param = %s'
+                                 %(repr(self.mother), repr(self.param)))
+            if len(np.atleast_1d(dof)) != 1:
+                pass
+            elif dof == -1:
+                dof = np.zeros(j)+self.dofmin
+            else:
+                dof = np.zeros(j)+dof
+            dof[dof <= 1] = 1
+            dof = self.dofmin * (1 + (dof * self.dt/self.gamma_fac/self.scale)**2)**0.5
+            dof[dof <= self.dofmin] = self.dofmin
+            if not confidence:
+                for i in range(j):
+                    chisqr = self._chisquareInv(siglvl, dof[i]) / dof[i]
+                    signif[i] = chisqr * fft_theor[i]
+            else:
+                signif = np.empty(2,j)
+                sig = (1-siglvl)/2.
+                for i in range(j):
+                    chisqr = dof[i]/np.array((self._chisquareInv(1-sig,dof[i]),
+                                            self._chisquareInv(sig, dof[i])))
+                    signif[:,i] = fft_theor[i]*chisqr
+        elif sigtest == 2:
+            if len(dof) != 2:
+                raise ValueError('DOF must be set to [s1,s2], the range of scale-averages')
+            if self.cdelta == -1:
+                raise ValueError('cdelta & dj0 not defined for'
+                                 'mother = %s with param = %s' %(repr(self.mother), repr(self.param)))
+            dj= np.log2(self.scale[1] / self.scale[0])
+            s1 = dof[0]
+            s2 = dof[1]
+            avg = (self.period >= s1)*(self.period <= s2)
+            navg = avg.sum()
+            if not navg:
+                raise ValueError('No valid scales between %s and %s' %(repr(s1), repr(s2)))
+            s1 = self.scale[avg].min()
+            s2 = self.scale[avg].max()
+            savg = 1./(1./self.scale[avg]).sum()
+            smid = np.exp(0.5*np.log(s1*s2))
+            dof = (self.dofmin*navg*savg/smid)*(1+(navg*dj/self.dj0)**2)**0.5
+            fft_theor = savg*(fft_theor[avg]/self.scale[avg]).sum()
+            chisqr = self._chisquareInv(siglvl,dof)/dof
+            if confidence:
+                sig = (1-siglvl)/2.
+                chisqr = dof/np.array((self._chisquareInv(1-sig, dof),
+                                       self._chisquareInv(sig, dof)))
+            signif = (self.dj*self.dt/self.cdelta/savg)*fft_theor*chisqr
+        else:
+            raise ValueError('Sigtest must be 0,1, or 2')
+        self.signif = signif
+        return signif
+    
+    def _chisquareInv(self,p,v):
+        """
+        Inverse of chi-square cumulative distribution function(CDF).
+        
+        Parameters
+        ----------
+        p : float
+            probability
+        v : float
+            degrees of freedom of the chi-square distribution
+        
+        Returns
+        -------
+        x : float
+            the inverse of chi-square cdf
+            
+        Example
+        -------
+        >>> result = chisquare_inv(p,v)
+        
+        """
+        if not 0<p<1:
+            raise ValueError('p must be 0<p<1')
+        minv = 0.01
+        maxv = 1
+        x = 1
+        tolerance = 1e-4
+        while x+tolerance >= maxv:
+            maxv*=10.
+            x = fmin(self._chisquareSolve, minv, maxv, args=(p,v), xtol=tolerance)
+            minv = maxv
+        x*=v
+        return x
+        
+    def _chisquareSolve(self,xguess,p,v):
+        """
+        Chisqure_solve
+        
+        Return the difference between calculated percentile and P.
+        
+        Written January 1998 by C. Torrence
+        """
+        pguess = gammainc(v/2,v*xguess/2)
+        pdiff = np.abs(pguess - p)
+        if pguess >= 1-1e-4:
+            pdiff = xguess
+        return pdiff
+    
+    def plot(self, lag1=0., levels=None, time=None, title=[None,None,None,None], figsize=(9,8)):
+        """
+        Plot Time Series, Wavelet Power Spectrum, 
+        Global Power Spectrum and Scale-average Time Series.
+        
+        Parameters
+        ---------
+        lag1: (optional) `float`
+            LAG 1 Autocorrelation, used for signif levels.
+                * Default is 0.
+        levels: list
+            Contour levels to plot the wavelet spectrum.
+        time: `~numpy.ndarray`
+            time array.
+        title: list
+            title of the each figure.
+        figsize: tuple
+            figure size
+        
+        Example
+        -------
+        >>> ww = Wavelet(data, 0.25, dj=0.1, s0=0.25, j=9/0.1)
+        >>> ww.plot()
+        """
+        
+        import matplotlib.pyplot as plt
+        from matplotlib.gridspec import GridSpec
+        from matplotlib import ticker
+        
+        n = len(self.data)
+        gs = GridSpec(7, 4)
+        self.fig = plt.figure(figsize=figsize)
+        self.axData = self.fig.add_subplot(gs[0:2, :3])
+        self.axWavelet = self.fig.add_subplot(gs[2:5, :3], sharex=self.axData)
+        self.axGlobal = self.fig.add_subplot(gs[2:5, 3], sharey=self.axWavelet)
+        self.axScaleAvg = self.fig.add_subplot(gs[5:7, :3], sharex=self.axData)
+        periodMax = self.period.max()
+        periodMax = periodMax if periodMax<64 else 64
+        
+        if time is None:
+            time = self.dt*np.arange(n)
+        if levels is None:
+            levels = [0.05, 0.12,0.229,
+                      0.45]
+            
+        # Plot Time Series
+        if title[0] is None:
+            self.axData.set_title('a) Time Series')
+        else:
+            self.axData.set_title(title)
+        self.axData.set_ylabel('Value')
+        self.axData.minorticks_on()
+        self.axData.tick_params(which='both', direction='in')
+        self.pData = self.axData.plot(time, self.data,
+                                      color='k', lw=1.5)[0]
+        self.axData.set_xlim(time[0], time[-1])
+        
+        # Contour Plot Wavelet Power Spectrum
+        if title[1] is None:
+            self.axWavelet.set_title('b) Wavelet Power Spectrum')
+        else:
+            self.axWavelet.set_title(title)
+        self.axWavelet.set_ylabel('Period')
+        self.axWavelet.minorticks_on()
+        
+        self.axWavelet.tick_params(which='both', direction='in')
+        self.axWavelet.set_yscale('symlog', basey=2)
+        self.axWavelet.yaxis.set_major_formatter(ticker.ScalarFormatter())
+        self.axWavelet.ticklabel_format(axis='y',style='plain')
+        self.axWavelet.set_ylim(periodMax, 0.5)
+        
+        wpower = self.power/self.power.max()
+        self.contour = self.axWavelet.contourf(time, self.period,
+                                               wpower, len(levels),
+                                               colors=['w'])
+        self.contourIm = self.axWavelet.contourf(self.contour,
+                                                 levels=levels,
+                                                 cmap=plt.cm.Spectral_r, extend='max')
+        signif = self.waveSignif(self.data, sigtest=0, lag1=lag1, siglvl=0.90,
+                                 gws=self.gws)
+        sig90 = signif[:,None]
+        sig90 = self.power/sig90
+        
+        self.axWavelet.contour(time, self.period, sig90, [-99,1] ,colors='r')
+        self.axWavelet.fill_between(time, self.coi,
+                                    self.period.max(), color='grey',
+                                    alpha=0.4, hatch='x')
+        
+        # Plot Global Wavelet Spectrum
+        if title[2] is None:
+            self.axGlobal.set_title('c) Global')
+        else:
+            self.axGlobal.set_title(title)
+        self.axGlobal.set_xlabel('Power')
+        self.axGlobal.set_ylabel('')
+        self.axGlobal.set_yscale('symlog', basey=2)
+        self.axGlobal.minorticks_on()
+        self.axGlobal.yaxis.set_major_formatter(ticker.ScalarFormatter())
+        self.axGlobal.ticklabel_format(axis='y',style='plain')
+        self.axGlobal.tick_params(which='both', direction='in')
+        self.pGlobal = self.axGlobal.plot(self.gws, self.period,
+                                          color='k', lw=1.5)[0]
+        
+        
+        dof = n - self.scale
+#        lag1 = 0.72
+        gsig = self.waveSignif(self.data, sigtest=1, lag1=0,
+                               dof=dof)
+        self.pSig = self.axGlobal.plot(gsig,
+                                       self.period, 
+                                       'r--',
+                                       lw=1.5)
+        
+        
+        # Plot Scale-average Time Series
+        if title[3] is None:
+            self.axScaleAvg.set_title('d) Scale-average Time Series')
+        else:
+            self.axScaleAvg.set_title(title)
+        self.axScaleAvg.set_xlabel('Time')
+        self.axScaleAvg.set_ylabel('Avg')
+        self.axScaleAvg.minorticks_on()
+        self.axScaleAvg.tick_params(which='both', direction='in')
+        
+        period_mask = (self.period >= 2)*(self.period < 8)
+        power_norm = self.power/self.scale[:,None]
+        power_avg = self.dj*self.dt/self.cdelta*power_norm[period_mask,:].sum(0)
+        self.pScaleAvg = self.axScaleAvg.plot(time,
+                                              power_avg,
+                                              color='k',
+                                              lw=1.5)
+        
+        self.fig.tight_layout()
+
+
+
+
+
+
+
+class WaveCoherency:
+    def __init__(self, wave1, time1, scale1, wave2, time2, scale2,
+                 dt=False, dj=False, coi=False, nosmooth=False):
+        """
+        Compute the wavelet coherency between two time series.
+        
+        Parameters
+        ----------
+        wave1 : ~numpy.ndarray
+            Wavelet power spectrum for time series 1.
+        time1 : ~numpy.ndarray
+            A vector of times for time series 1.
+        scale1 : ~numpy.ndarray
+            A vector of scales for time series 1.
+        wave2 : ~numpy.ndarray
+            Wavelet power spectrum for time series 2.
+        time2 : ~numpy.ndarray
+            A vector of times for time series 2.
+        scale2 : ~numpy.ndarray
+            A vector of scales for time series 2.
+        dt : (optional) float
+            Amount of time between each Y value, i.e. the sampling time.
+                If not input, then calculated from time1[1]-time1[0]
+        dj : (optional) float
+            The spacing between discrete scales.
+                If not input, then calculated from scale1
+        coi : (optional) ~numpy.ndarray
+            The array of the cone-of influence.
+        nosmooth : (optional) bool
+            If True, then just compute the global_coher, global_phase, and
+            the unsmoothed cross_wavelet and return.
+        
+        Returns
+        -------
+            
+        cross_wavelet : ~numpy.ndarray
+            The cross wavelet between the time series.
+        time : ~numpy.ndarray
+            The time array given by the overlap of time1 and time2.
+        scale : ~numpy.ndarray
+            The scale array of scale indices, given by the overlap of 
+            scale1 and scale2.
+        wave_phase : ~numpy.ndarray
+            The phase difference between time series 1 and time series 2.
+        wave_coher : ~numpy.ndarray
+            The wavelet coherency, as a function of time and scale.
+        global_phase : ~numpy.ndarray
+            The global (or mean) phase averaged over all times.
+        global_coher : ~numpy.ndarray
+            The global (or mean) coherence averaged over all times.
+        power1 : ~numpy.ndarray
+            The wavelet power spectrum should be the same as wave1
+            if time1 and time2 are identical, otherwise it is only the
+            overlapping portion. If nosmooth is set,
+            then this is unsmoothed, otherwise it is smoothed.
+        power2 : ~numpy.ndarray
+            same as power 1 but for time series 2.
+        coi : ~numpy.ndarray
+            The array of the cone-of influence.
+            
+        Notes
+        -----
+            This function based on the IDL code WAVE_COHERENCY.PRO written by C. Torrence, 
+        
+        References
+        ----------
+        Torrence, C. and Compo, G. P., 1998, A Practical Guide to Wavelet Analysis, 
+        *Bull. Amer. Meteor. Soc.*, `79, 61-78 <http://paos.colorado.edu/research/wavelets/bams_79_01_0061.pdf>`_.\n
+        http://paos.colorado.edu/research/wavelets/
+        
+        Example
+        -------
+        >>> res = wavelet.WaveCoherency(wave1,time1,scale1,wave2,time2,scale2,\
+                                       dt,dj,coi=coi)
+        >>> cross_wave = res.cross_wavelet
+        >>> phase = res.wave_phase
+        >>> coher = res.wave_coher
+        >>> gCoher = res.global_coher
+        >>> gCross = res.global_cross
+        >>> gPhase = res.global_phase
+        >>> power1 = res.power1
+        >>> power2 = res.power2
+        >>> time_out = res.time
+        >>> scale_out = res.scale
+        """
+        if not dt: dt = time1[1]-time1[0]
+        if not dj: dj = np.log2(scale1[1]/scale1[0])
+        if time1 is time2:
+            t1s = 0
+            t1e = len(time1)
+            t2s = t1s
+            t2e = t1e
+        else:
+            otime_start = min([time1.min(),time2.min()])
+            otime_end = max([time1.max(),time2.max()])
+            t1 = np.where((time1 >= otime_start)*(time1 <= otime_end))[0]
+            t1s = t1[0]
+            t1e = t1[-1]+1
+            t2 = np.where((time2 >= otime_start)*(time2 <= otime_end))[0]
+            t2s = t2[0]
+            t2e = t2[-1]+1
+        
+        oscale_start = min([scale1.min(),scale2.min()])
+        oscale_end = max([scale1.max(),scale2.max()])
+        s1 = np.where((scale1 >= oscale_start)*(scale1 <= oscale_end))[0]
+        s2 = np.where((scale2 >= oscale_start)*(scale2 <= oscale_end))[0]
+        s1s = s1[0]
+        s1e = s1[-1]+1
+        s2s = s2[0]
+        s2e = s2[-1]+1
+        
+        self.cross_wavelet = wave1[s1s:s1e,t1s:t1e]*wave2[s2s:s2e,t2s:t2e].conj()
+        self.power1 = np.abs(wave1[s1s:s1e,t1s:t1e])**2
+        self.power2 = np.abs(wave2[s2s:s2e,t2s:t2e])**2
+        
+        self.time = time1[t1s:t1e]
+        self.scale = scale1[s1s:s1e]
+        nj = s1e-s1s
+        
+        global1 = self.power1.sum(1)
+        global2 = self.power2.sum(1)
+        self.global_cross = self.cross_wavelet.sum(1)
+        self.global_coher = np.abs(self.global_cross)**2/(global1*global2)
+        self.global_phase = np.arctan(self.global_cross.imag/self.global_cross.real)*180./np.pi
+        
+        if not nosmooth:
+            nt = (4*self.scale/dt)//2*4+1
+            nt2 = nt[:,None]
+            ntmax = nt.max()
+            g = np.arange(ntmax) * np.ones((nj,1))
+            wh = g >= nt2
+            time_wavelet = (g-nt2//2)*dt/self.scale[:,None]
+            wave_func = np.exp(-time_wavelet**2/2)
+            wave_func[wh] = 0
+            wave_func = (wave_func/wave_func.sum(1)[:,None]).real
+            self.cross_wavelet = _fastConv(self.cross_wavelet, wave_func, nt2)
+            self.power1 = _fastConv(self.power1, wave_func, nt2)
+            self.power2 = _fastConv(self.power2, wave_func, nt2)
+            scales = self.scale[:, None]
+            self.cross_wavelet /= scales
+            self.power1 /= scales
+            self.power2 /= scales
+            
+            nw = int(0.6/dj/2 + 0.5)*2-1
+            weight = np.ones(nw)/nw
+            self.cross_wavelet = _fastConv2(self.cross_wavelet, weight)
+            self.power1 = _fastConv2(self.power1,weight)
+            self.power2 = _fastConv2(self.power2,weight)
+            
+            self.wave_phase = 180./np.pi*np.arctan(self.cross_wavelet.imag/self.cross_wavelet.real)
+            power3=self.power1*self.power2
+            whp=power3 < 1e-9
+            power3[whp]=1e-9
+            self.wave_coher = (np.abs(self.cross_wavelet)**2/power3).real
+    
+
+
+def _fastConv(f, g, nt):
+    """
+    Fast convolution two given function f and g (method 1)
+    """
+    nf=f.shape
+    ng=g.shape
+    npad=2**(int(np.log2(max([nf[1],ng[1]])))+1)
+    wh1=np.arange(nf[0],dtype=int)
+    wh2=np.arange(nf[1],dtype=int)*np.ones((nf[0],1),dtype=int)-(nt.astype(int)-1)//2-1
+    pf=np.zeros([nf[0],npad],dtype=complex)
+    pg=np.zeros([nf[0],npad],dtype=complex)
+    pf[:,:nf[1]]=f
+    pg[:,:ng[1]]=g
+    conv=ifft(fft(pf)*fft(pg[:,::-1]))
+    result=conv[wh1,wh2.T].T
+    return result
+
+def _fastConv2(f, g):
+    """
+    Fast convolution two given function f and g (method2)
+    """
+    nf=f.shape
+    ng=len(g)
+    npad=2**(int(np.log2(max([nf[0],ng])))+1)
+    
+    wh1=np.arange(nf[1],dtype=int)
+    wh2=np.arange(nf[0],dtype=int)*np.ones((nf[1],1),dtype=int)+ng//2
+    pf=np.zeros([npad,nf[1]],dtype=complex)
+    pg=np.zeros([npad,nf[1]],dtype=complex)
+    pf[:nf[0],:]=f
+    pg[:ng,:]=g[:,np.newaxis]
+    conv=ifft(fft(pf,axis=0)*fft(pg,axis=0),axis=0)
+    result=conv[wh2.T,wh1]
     return result
```

### Comparing `fisspy-0.9.80/fisspy/data/_sample.py` & `fisspy-1.0.0/fisspy/data/_sample.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-"""FISSPy sample data file set"""
-from __future__ import absolute_import, print_function
-
-from astropy.utils.data import download_file
-from sunpy.util.net import url_exists
-import os.path
-from os import mkdir
-from shutil import move
-
-__author__ = "Juhyeong Kang"
-__email = "jhkang@astro.snu.ac.kr"
-
-
-url='http://fiss.snu.ac.kr/sample-data/'
-files=['FISS_20140603_164842_B1_p.fts',
-      'mFISS_20140603_164842_B1_c.fts']
-
-home=os.path.expanduser("~")
-if not home:
-    raise RuntimeError('Environment variable $HOME is not defined.')
-
-fissdir=os.path.join(home,'fisspy')
-if not os.path.isdir(fissdir):
-    mkdir(fissdir)
-    
-sampledir=os.path.join(fissdir,'sample_data')
-if not os.path.isdir(sampledir):
-    mkdir(sampledir)
-    
-def download_sample_data():
-    """
-    Download the sample data.
-    
-    Parameters
-    ----------
-    None
-    
-    Returns
-    -------
-    None
-    """
-    print("Downloading sample fiss files to {}".format(sampledir))
-    for f in files:
-        if url_exists(url+f):
-            df = download_file(url+f)
-            move(df,os.path.join(sampledir,f))
+"""FISSPy sample data file set"""
+from __future__ import absolute_import, print_function
+
+from astropy.utils.data import download_file
+from sunpy.util.net import url_exists
+import os.path
+from os import mkdir
+from shutil import move
+
+__author__ = "Juhyeong Kang"
+__email = "jhkang@astro.snu.ac.kr"
+
+
+url='http://fiss.snu.ac.kr/sample-data/'
+files=['FISS_20140603_164842_B1_p.fts',
+      'mFISS_20140603_164842_B1_c.fts']
+
+home=os.path.expanduser("~")
+if not home:
+    raise RuntimeError('Environment variable $HOME is not defined.')
+
+fissdir=os.path.join(home,'fisspy')
+if not os.path.isdir(fissdir):
+    mkdir(fissdir)
+
+sampledir=os.path.join(fissdir,'sample_data')
+if not os.path.isdir(sampledir):
+    mkdir(sampledir)
+
+def download_sample_data():
+    """
+    Download the sample data.
+
+    Parameters
+    ----------
+    None
+
+    Returns
+    -------
+    None
+    """
+    print("Downloading sample fiss files to {}".format(sampledir))
+    for f in files:
+        if url_exists(url+f):
+            df = download_file(url+f)
+            move(df,os.path.join(sampledir,f))
```

### Comparing `fisspy-0.9.80/fisspy/image/base.py` & `fisspy-1.0.0/fisspy/image/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,509 +1,434 @@
-"""
-Basic image process tool.
-"""
-
-from __future__ import absolute_import, division
-
-import numpy as np
-from interpolation.splines import LinearSpline
-from scipy.fftpack import ifft2, fft2
-from sunpy.coordinates import frames
-from astropy.coordinates import SkyCoord
-from sunpy.coordinates.ephemeris import get_earth
-from sunpy.physics.differential_rotation import solar_rotate_coordinate
-
-__author__ = "Juhyung Kang"
-__email__ = "jhkang@astro.snu.ac.kr"
-__all__ = ['alignoffset', 'rot_trans', 'img_interpol',
-           'rotation', 'rot', 'shift', 'shift3d',
-           'diff_rot_correct']
-
-def alignoffset(image0, template0, cor= None):
-    """
-    Align the two images
-
-    Parameters
-    ----------
-    image0 : `~numpy.ndarray`
-        Images for coalignment with the template
-        A 2 or 3 Dimensional array ex) image[t,y,x]
-    template0 : `~numpy.ndarray`
-        The reference image for coalignment
-        2D Dimensional arry ex) template[y,x]
-    cor: `bool`
-        If True, return the correlation between template0 and result.
-
-    Returns
-    -------
-    sh : `~numpy.ndarray`
-        Shifted value of the image0
-        np.array([yshift, xshift])
-
-    Notes
-    -----
-        This code is based on the IDL code ALIGNOFFSET.PRO
-        written by J. Chae 2004.
-        Using for loop is faster than inputing the 3D array as,
-            >>> res=np.array([alignoffset(image[i],template) for i in range(nt)])
-        where nt is the number of elements for the first axis.
-
-    Example
-    -------
-    >>> sh = alignoffset(image,template)
-    """
-    st=template0.shape
-    si=image0.shape
-    ndim=image0.ndim
-
-    if ndim>3 or ndim==1:
-        raise ValueError('Image must be 2 or 3 dimensional array.')
-
-    if not st[-1]==si[-1] and st[-2]==si[-2]:
-        raise ValueError('Image and template are incompatible\n'
-        'The shape of image = %s\n The shape of template = %s.'
-        %(repr(si[-2:]),repr(st)))
-
-    if not ('float' in str(image0.dtype) and 'float' in str(template0.dtype)):
-        image0=image0.astype(float)
-        template0=template0.astype(float)
-
-    nx=st[-1]
-    ny=st[-2]
-
-    template=template0.copy()
-    image=image0.copy()
-
-    image=(image.T-image.mean(axis=(-1,-2))).T
-    template-=template.mean()
-
-    sigx=nx/6.
-    sigy=ny/6.
-    gx=np.arange(-nx/2,nx/2,1)
-    gy=np.arange(-ny/2,ny/2,1)[:,np.newaxis]
-    gauss=np.exp(-0.5*((gx/sigx)**2+(gy/sigy)**2))**0.5
-
-    #give the cross-correlation weight on the image center
-    #to avoid the fast change the image by the granular motion or strong flow
-
-    corr=ifft2(ifft2(template*gauss)*fft2(image*gauss)).real
-
-    # calculate the cross-correlation values by using convolution theorem and
-    # DFT-IDFT relation
-
-    s=np.where((corr.T==corr.max(axis=(-1,-2))).T)
-    x0=s[-1]-nx*(s[-1]>nx/2)
-    y0=s[-2]-ny*(s[-2]>ny/2)
-
-    if ndim==2:
-        cc=np.empty((3,3))
-        cc[0,1]=corr[s[0]-1,s[1]]
-        cc[1,0]=corr[s[0],s[1]-1]
-        cc[1,1]=corr[s[0],s[1]]
-        cc[1,2]=corr[s[0],s[1]+1-nx]
-        cc[2,1]=corr[s[0]+1-ny,s[1]]
-        x1=0.5*(cc[1,0]-cc[1,2])/(cc[1,2]+cc[1,0]-2.*cc[1,1])
-        y1=0.5*(cc[0,1]-cc[2,1])/(cc[2,1]+cc[0,1]-2.*cc[1,1])
-    else:
-        cc=np.empty((si[0],3,3))
-        cc[:,0,1]=corr[s[0],s[1]-1,s[2]]
-        cc[:,1,0]=corr[s[0],s[1],s[2]-1]
-        cc[:,1,1]=corr[s[0],s[1],s[2]]
-        cc[:,1,2]=corr[s[0],s[1],s[2]+1-nx]
-        cc[:,2,1]=corr[s[0],s[1]+1-ny,s[2]]
-        x1=0.5*(cc[:,1,0]-cc[:,1,2])/(cc[:,1,2]+cc[:,1,0]-2.*cc[:,1,1])
-        y1=0.5*(cc[:,0,1]-cc[:,2,1])/(cc[:,2,1]+cc[:,0,1]-2.*cc[:,1,1])
-
-
-    x=x0+x1
-    y=y0+y1
-
-    if cor and ndim == 3:
-        img = shift3d(image, [-y, -x])
-        xx = np.arange(nx) + x[:,None,None]
-        yy = np.arange(ny)[:,None] + y[:,None,None]
-        kx = np.logical_and(xx >= 0, xx <= nx - 1)
-        ky = np.logical_and(yy >= 0, yy <= ny - 1)
-        roi = np.logical_and(kx, ky)
-        cor = (img * template * roi).sum((1,2)) / np.sqrt(
-                        (img **2 * roi).sum((1,2)) *
-                        (template **2 * roi).sum((1,2)))
-        return np.array([y, x]), cor
-    elif cor and ndim == 2:
-        img = shift(image, [-y, -x])
-        xx = np.arange(nx) + x
-        yy = np.arange(ny) + y
-        kx = np.logical_and(xx >= 0, xx <= nx - 1)
-        ky = np.logical_and(yy >= 0, yy <= ny - 1)
-        roi = np.logical_and(kx, ky[:,None])
-        cor = (img*template)[roi].sum()/np.sqrt((img[roi]**2).sum() *
-                      (template[roi]**2).sum())
-        return np.array([y, x]), cor
-    else:
-        return np.array([y, x])
-
-def rot_trans(x, y, xc, yc, angle, dx=0, dy=0, inv=False):
-    """
-    Rotational transpose for input array of x, y and angle.
-
-    Parameters
-    ----------
-    x : `~numpy.ndarray`
-        Row vector of x.
-    y : `~numpy.ndarray`
-        Colomn vector of y.
-    xc : `float`
-        x-axis value of roatation center.
-    yc : `float`
-        y-axis value of rotation center.
-    angle : `float`
-        Roation angle in 'radian' unit.
-    dx : (optional) `float`
-        The relative displacement along x-axis
-        of the rotated images to the reference image.
-    dy : (optional) `float`
-        The relative displacement along y-axis
-        of the rotated images to the reference image.
-    inv : (optional) `bool`
-        If True, the do inverse roattion transpose.
-
-    Returns
-    -------
-    xt : ~numpy.ndarray
-        Transposed coordinates of the positions in the observed frame
-    yt : ~numpy.ndarray
-        Transposed coordinates of the positions in the observed frame
-
-    Notes
-    -----
-    The input angle must be in radian.
-    """
-
-    if not inv:
-        xt=(x-xc)*np.cos(angle)+(y-yc)*np.sin(angle)+xc+dx
-        yt=-(x-xc)*np.sin(angle)+(y-yc)*np.cos(angle)+yc+dy
-    else:
-        xt=(x-xc-dx)*np.cos(angle)-(y-yc-dy)*np.sin(angle)+xc
-        yt=(x-xc-dx)*np.sin(angle)+(y-yc-dy)*np.cos(angle)+yc
-    return xt,yt
-
-def img_interpol(img, xa, ya, xt, yt, missing=-1):
-    """
-    Interpolate the image for a given coordinates.
-
-    Parameters
-    ----------
-    img : `~numpy.ndarray`
-        2 dimensional array of image.
-    xa : `~numpy.ndarray`
-        Row vector of x.
-    ya : `~numpy.ndarray`
-        Colomn vector of y.
-    xt : `~numpy.ndarray`
-        Coordinates of the positions in the observed frame.
-    yt : `~numpy.ndarray`
-        Coordinates of the positions in the observed frame.
-    missing : (optional) `float`
-        The value of extrapolated position.
-        Default is -1, and it means the False.
-        If False, then extrapolate the given position.
-
-    Returns
-    -------
-    res : ~numpy.ndarray
-        2 dimensional interpolated image.
-        The size of res is same as input img.
-
-    """
-    shape=xt.shape
-    size=xt.size
-    smin=[ya[0,0],xa[0]]
-    smax=[ya[-1,0],xa[-1]]
-    order=[len(ya),len(xa)]
-    interp=LinearSpline(smin,smax,order,img)
-    a=np.array((yt.reshape(size),xt.reshape(size)))
-    b=interp(a.T)
-    res=b.reshape(shape)
-    if missing!=-1:
-        mask=np.invert((xt<=xa.max())*(xt>=xa.min())*(yt<=ya.max())*(yt>=ya.min()))
-        res[mask]=missing
-    return res
-
-def img_interpol3d(img, ta, ya, xa,
-                   tt, yt, xt, missing=-1):
-    """
-    Interpolate the image for a given coordinates.
-
-    Parameters
-    ----------
-    img : `~numpy.ndarray`
-        3 dimensional array of image.
-    xa : `~numpy.ndarray`
-        Row vector of x.
-    ya : `~numpy.ndarray`
-        Colomn vector of y.
-    ta : `~numpy.ndarray`
-        Frame vector.
-    tt : `~numpy.ndarray`
-        Coordinates of the positions in the observed frame.
-    yt : `~numpy.ndarray`
-        Coordinates of the positions in the observed frame.
-    xt : `~numpy.ndarray`
-        Coordinates of the positions in the observed frame.
-    missing : (optional) `float`
-        The value of extrapolated position.
-        Default is -1, and it means the False.
-        If False, then extrapolate the given position.
-
-    Returns
-    -------
-    res : ~numpy.ndarray
-        3 dimensional interpolated image.
-        The size of res is same as input img.
-
-    """
-    shape = xt.shape
-    size = xt.size
-    smin = [ta[0,0,0], ya[0,0,0], xa[0]]
-    smax = [ta[-1,0,0],ya[0,-1,0], xa[-1]]
-    order = [ta.size, ya.size, xa.size]
-    interp = LinearSpline(smin, smax, order, img)
-    a = np.array((tt.reshape(size), yt.reshape(size), xt.reshape(size)))
-    b=interp(a.T)
-    res=b.reshape(shape)
-    if missing!=-1:
-        mask=np.invert((xt<=xa.max())*(xt>=xa.min())*(yt<=ya.max())*(yt>=ya.min()))
-        res[mask]=missing
-    return res
-
-def rotation(img, angle, x, y, xc, yc,
-             dx=0, dy=0, inv=False, missing=-1):
-    """
-    Rotate the input image with angle and center position.
-
-    Parameters
-    ----------
-    img : `~numpy.ndarray`
-        2 dimensional array of image.
-    x : `~numpy.ndarray`
-        Row vector of x.
-    y : `~numpy.ndarray`
-        Colomn vector of y.
-    xc : `float`
-        x-axis value of roatation center.
-    yc : `float`
-        y-axis value of rotation center.
-    angle : `float`
-        Roation angle in 'radian' unit.
-    dx : (optional) `float`
-        The relative displacement along x-axis
-        of the rotated images to the reference image.
-    dy : (optional) `float`
-        The relative displacement along y-axis
-        of the rotated images to the reference image.
-    inv : (optional) `bool`
-        If True, the do inverse roattion transpose.
-    missing : (optional) `float`
-        The value of extrapolated position.
-        Default is -1, and it means the False.
-        If False, then extrapolate the given position.
-
-    Returns
-    -------
-    result : `~numpy.ndarray`
-        rotated image.
-
-    Notes
-    -----
-    It is not conventional rotation.
-    It is just used for the coalignment module.
-
-    """
-    xt,yt=rot_trans(x, y, xc, yc, angle,
-                    dx, dy, inv)
-    return img_interpol(img, x, y, xt, yt,
-                        missing=missing)
-
-def rot(img, angle, xc=False, yc=False,
-        dx=0, dy=0, xmargin=0, ymargin=0, missing=0):
-    """
-    Rotate the input image.
-
-    Parameters
-    ----------
-    img : `~numpy.ndarray`
-        2 dimensional array of image.
-    angle : `float`
-        Roation angle in 'radian' unit.
-    xc : (optional) `float`
-        x-axis value of roatation center.
-        Default is the image center.
-    yc : (optional) `float`
-        y-axis value of rotation center.
-        Default is the image center.
-    dx : (optional) `float`
-        The relative displacement along x-axis
-        of the rotated images to the reference image.
-    dy : (optional) `float`
-        The relative displacement along y-axis
-        of the rotated images to the reference image.
-    xmargin : (optional) `float`
-        The margin value of x-axis
-    ymargin : (optional) `float`
-        The margin value of y-axis
-    missing : (optional) `float`
-        The value of extrapolated position.
-        Default is -1, and it means the False.
-        If False, then extrapolate the given position.
-
-    Returns
-    -------
-    result : `~numpy.ndarray`
-        rotated image.
-
-    Notes
-    -----
-    The input angle must be in radian unit.
-
-    """
-    ny,nx=img.shape
-    nx1=int(nx+2*xmargin)
-    ny1=int(ny+2*ymargin)
-    x=np.arange(nx)
-    y=np.arange(ny)[:,None]
-    xa=np.arange(nx1)-xmargin
-    ya=(np.arange(ny1)-ymargin)[:,None]
-
-
-    if not xc:
-        xc=nx/2
-    if not yc:
-        yc=ny/2
-    xt, yt=rot_trans(xa,ya,xc,yc,angle,dx=dx,dy=dy)
-    return img_interpol(img,x,y,xt,yt,missing=missing)
-
-def shift(image, sh, missing=0):
-    """
-    Shift the given image.
-
-    Parameters
-    ----------
-    image :  `~numpy.ndarray`
-        2 dimensional array.
-    sh : tuple, list or ndarray
-        tuple, list or ndarray of shifting value set (y,x)
-    missing: `float`
-        The value of extrapolated position.
-        Default is -1, and it means the False.
-        If False, then extrapolate the given position.
-
-    Returns
-    -------
-    simage : ~numpy.ndarray
-        shifted image.
-    """
-    ny, nx =image.shape
-    x=np.arange(nx)
-    y=np.arange(ny)[:,None]
-    xt=x-sh[1]+y*0
-    yt=y-sh[0]+x*0
-
-    return img_interpol(image,x,y,xt,yt,missing=missing)
-
-def shift3d(img, sh):
-    """
-    Shift the given image.
-
-    Parameters
-    ----------
-    image :  `~numpy.ndarray`
-        3 dimensional array.
-    sh : tuple, list or ndarray
-        tuple, list or ndarray of shifting value set (y,x)
-
-    Returns
-    -------
-    simage : ~numpy.ndarray
-        shifted image.
-    """
-    nt, ny, nx =img.shape
-
-    t = np.arange(nt)[:,None,None]
-    y = np.arange(ny)[None,:,None]
-    x = np.arange(nx)
-    tt = t + y*0 + x*0
-    yt = y - sh[0][:, None, None] + t*0 + x*0
-    xt = x - sh[1][:, None, None] + t*0 + y*0
-
-    return img_interpol3d(img, t, y, x, tt, yt, xt, missing=0)
-
-
-def diff_rot_correct(mmap, refx, refy, reftime):
-    """
-    Correct the solar rotation.
-
-    Parameters
-    ----------
-    mmap : sunpy.map.GenericMap
-        Single map class.
-    refx : astropy.units.Quantity
-        Horizontal wcs information of reference frame.
-    refy : astropy.units.Quantity
-        Vertical wcs information of reference frame.
-    reftime : astropy.time.Time
-        Time for the reference frame.
-
-    Returns
-    -------
-    smap : sunpy.map.GenericMap
-        Solar rotation corrected map class.
-
-    """
-
-    refc = SkyCoord(refx, refy, obstime= reftime,
-                    observer= get_earth(reftime),
-                    frame= frames.Helioprojective)
-
-    date = mmap.date
-    res = solar_rotate_coordinate(refc, time=date ,frame_time='synodic')
-    x = res.Tx.value
-    y = res.Ty.value
-
-    sx = x - refx.value
-    sy = y - refy.value
-    mmap.shift
-    smap = _mapShift(mmap, sx, sy)
-    return smap
-
-def _mapShift(map1, sx, sy):
-
-    new_meta = map1.meta.copy()
-    new_meta['crval1'] = ((map1.meta['crval1']*
-                           map1.spatial_units[0] +
-                           sx * map1.spatial_units[0]).to(map1.spatial_units[0])).value
-    new_meta['crval2'] = ((map1.meta['crval2']*
-                           map1.spatial_units[0] +
-                           sy * map1.spatial_units[0]).to(map1.spatial_units[0])).value
-    delx = sx/map1.meta['cdelt1']
-    dely = sy/map1.meta['cdelt2']
-
-    smin = [0, 0]
-    smax = [new_meta['naxis2']-1, new_meta['naxis1']-1]
-    order = map1.data.shape
-    interp = LinearSpline(smin, smax, order, map1.data)
-
-    x = np.arange(new_meta['naxis1'], dtype=float)
-    xx0 = x * np.ones([new_meta['naxis2'],1])
-    xx = xx0 + delx
-    y = np.arange(new_meta['naxis2'], dtype=float)
-    yy0 = y[:,None] + np.ones(new_meta['naxis1'])
-    yy = yy0 + dely
-    size = new_meta['naxis1']*new_meta['naxis2']
-    inp = np.array([yy.reshape(size), xx.reshape(size)])
-    out = interp(inp.T)
-
-    out = out.reshape(new_meta['naxis2'], new_meta['naxis1'])
-    mask = np.invert((xx<=xx0.max())*(xx>=xx0.min())*(yy<=yy0.max())*(yy>=yy0.min()))
-    out[mask] = 0
-    newMap = map1._new_instance(out, new_meta, map1.plot_settings)
-
-    return newMap
+"""
+Basic image process tool.
+"""
+
+from __future__ import absolute_import, division
+
+import numpy as np
+from interpolation.splines import LinearSpline, CubicSpline
+from scipy.fftpack import ifft2, fft2
+# from sunpy.coordinates import frames
+# from astropy.coordinates import SkyCoord
+# from sunpy.coordinates.ephemeris import get_earth
+# from sunpy.physics.differential_rotation import solar_rotate_coordinate
+
+__author__ = "Juhyung Kang"
+__email__ = "jhkang@astro.snu.ac.kr"
+__all__ = ['alignoffset', 'rot_trans', 'img_interpol',
+           'rotation', 'rot', 'shift']
+
+def alignoffset(image0, template0, cor= None, test=False):
+    """
+    Calculate the align offset between two two-dimensional images
+
+    Parameters
+    ----------
+    image0 : `~numpy.ndarray`
+        Images for coalignment with the template
+        2 Dimensional array
+    template0 : `~numpy.ndarray`
+        The reference image for coalignment
+        2-Dimensional arry ex) template[y,x]
+    cor: `bool`
+        If True, return the correlation between template0 and result.
+
+    Returns
+    -------
+    sh : `~numpy.ndarray`
+        Shifted value of the image0
+        np.array([yshift, xshift])
+
+    Notes
+    -----
+        This code is based on the IDL code ALIGNOFFSET.PRO
+        written by J. Chae 2004.
+        Using for loop is faster than inputing the 3D array as,
+            >>> res=np.array([alignoffset(image[i],template) for i in range(nt)])
+        where nt is the number of elements for the first axis.
+
+    Example
+    -------
+    >>> sh = alignoffset(image,template)
+    """
+    st=template0.shape
+    si=image0.shape
+    ndim=image0.ndim
+
+    if ndim>=3 or ndim==1:
+        raise ValueError('Image must be 2 or 3 dimensional array.')
+
+    if not st[-1]==si[-1] and st[-2]==si[-2]:
+        raise ValueError('Image and template are incompatible\n'
+        'The shape of image = %s\n The shape of template = %s.'
+        %(repr(si[-2:]),repr(st)))
+
+    if not ('float' in str(image0.dtype) and 'float' in str(template0.dtype)):
+        image0=image0.astype(float)
+        template0=template0.astype(float)
+
+    nx=st[-1]
+    ny=st[-2]
+
+    template=template0.copy()
+    image=image0.copy()
+
+    image=(image.T-image.mean(axis=(-1,-2))).T
+    template-=template.mean()
+
+    sigx=nx/6.
+    sigy=ny/6.
+    gx=np.arange(-nx/2,nx/2,1)
+    gy=np.arange(-ny/2,ny/2,1)[:,np.newaxis]
+    gauss=np.exp(-0.5*((gx/sigx)**2+(gy/sigy)**2))**0.5
+
+    #give the cross-correlation weight on the image center
+    #to avoid the fast change the image by the granular motion or strong flow
+
+    corr=ifft2(ifft2(template*gauss)*fft2(image*gauss)).real
+    # calculate the cross-correlation values by using convolution theorem and
+    # DFT-IDFT relation
+
+    s=np.where((corr.T==corr.max(axis=(-1,-2))).T)
+    x0=s[-1]-nx*(s[-1]>nx/2)
+    y0=s[-2]-ny*(s[-2]>ny/2)
+
+    cc=np.empty((3,3))
+    cc[0,1]=corr[s[0]-1,s[1]]
+    cc[1,0]=corr[s[0],s[1]-1]
+    cc[1,1]=corr[s[0],s[1]]
+    cc[1,2]=corr[s[0],s[1]+1-nx]
+    cc[2,1]=corr[s[0]+1-ny,s[1]]
+    x1=0.5*(cc[1,0]-cc[1,2])/(cc[1,2]+cc[1,0]-2.*cc[1,1])
+    y1=0.5*(cc[0,1]-cc[2,1])/(cc[2,1]+cc[0,1]-2.*cc[1,1])
+
+
+    x=x0+x1
+    y=y0+y1
+    if test:
+        return corr
+    if cor:
+        img = shift(image, [-y, -x])
+        xx = np.arange(nx) + x
+        yy = np.arange(ny) + y
+        kx = np.logical_and(xx >= 0, xx <= nx - 1)
+        ky = np.logical_and(yy >= 0, yy <= ny - 1)
+        roi = np.logical_and(kx, ky[:,None])
+        cor = (img*template)[roi].sum()/np.sqrt((img[roi]**2).sum() *
+                      (template[roi]**2).sum())
+        return np.array([y, x]), cor
+    else:
+        return np.array([y, x])
+
+def rot_trans(x, y, xc, yc, angle, dx=0, dy=0, inv=False):
+    """
+    Rotational transpose for input array of x, y and angle.
+
+    Parameters
+    ----------
+    x : `~numpy.ndarray`
+        Row vector of x.
+    y : `~numpy.ndarray`
+        Colomn vector of y.
+    xc : `float`
+        x-axis value of roatation center.
+    yc : `float`
+        y-axis value of rotation center.
+    angle : `float`
+        Roation angle in 'radian' unit.
+    dx : (optional) `float`
+        The relative displacement along x-axis
+        of the rotated images to the reference image.
+    dy : (optional) `float`
+        The relative displacement along y-axis
+        of the rotated images to the reference image.
+    inv : (optional) `bool`
+        If True, the do inverse roattion transpose.
+
+    Returns
+    -------
+    xt : ~numpy.ndarray
+        Transposed coordinates of the positions in the observed frame
+    yt : ~numpy.ndarray
+        Transposed coordinates of the positions in the observed frame
+
+    Notes
+    -----
+    The input angle must be in radian.
+    """
+
+    if not inv:
+        xt=(x-xc)*np.cos(angle)+(y-yc)*np.sin(angle)+xc+dx
+        yt=-(x-xc)*np.sin(angle)+(y-yc)*np.cos(angle)+yc+dy
+    else:
+        xt=(x-xc-dx)*np.cos(angle)-(y-yc-dy)*np.sin(angle)+xc
+        yt=(x-xc-dx)*np.sin(angle)+(y-yc-dy)*np.cos(angle)+yc
+    return xt,yt
+
+def img_interpol(img, xa, ya, xt, yt, missing=-1, cubic=False):
+    """
+    Interpolate the image for a given coordinates.
+
+    Parameters
+    ----------
+    img : `~numpy.ndarray`
+        N-dimensional array of image.
+    xa : `~numpy.ndarray`
+        Row vector of x.
+    ya : `~numpy.ndarray`
+        Colomn vector of y.
+    xt : `~numpy.ndarray`
+        Coordinates of the positions in the observed frame.
+    yt : `~numpy.ndarray`
+        Coordinates of the positions in the observed frame.
+    missing : (optional) `float`
+        The value of extrapolated position.
+        Default is -1, and it means the False.
+        If False, then extrapolate the given position.
+
+    Returns
+    -------
+    res : ~numpy.ndarray
+        N-dimensional interpolated image.
+        The size of res is same as input img.
+
+    """
+    shape = img.shape
+    ndim = img.ndim
+    size = img.size
+    ones = np.ones(shape)
+
+    smin = np.zeros(ndim)
+    smax = np.array(shape)-1
+    smin[-1] = xa[0]
+    smin[-2] = ya[0,0]
+    smax[-1] = xa[-1]
+    smax[-2] = ya[-1,0]
+    order = shape
+    if cubic:
+        interp = CubicSpline(smin, smax, order, img)
+    else:
+        interp = LinearSpline(smin, smax, order, img)
+
+    inp = np.zeros((ndim,size))
+    for i, sh in enumerate(shape[:-2]):
+        tmp = np.arange(sh)[tuple([None]*i + [Ellipsis] + [None]*(ndim-1-i))]*ones
+        inp[i] = tmp.reshape(size)
+        
+    inp[-2] = (yt * ones).reshape(size)
+    inp[-1] = (xt * ones).reshape(size)
+    # a = np.array((yt.reshape(size),xt.reshape(size)))
+    b = interp(inp.T)
+    res=b.reshape(shape)
+    if missing!=-1:
+        mask=np.invert((xt<=xa.max())*(xt>=xa.min())*(yt<=ya.max())*(yt>=ya.min()))*ones.astype(bool)
+        res[mask]=missing
+    return res
+
+def rotation(img, angle, x, y, xc, yc,
+             dx=0, dy=0, inv=False, missing=-1, cubic=False):
+    """
+    Rotate the input image with angle and center position.
+
+    Parameters
+    ----------
+    img : `~numpy.ndarray`
+        N-dimensional array of image.
+    x : `~numpy.ndarray`
+        Row vector of x.
+    y : `~numpy.ndarray`
+        Colomn vector of y.
+    xc : `float`
+        x-axis value of roatation center.
+    yc : `float`
+        y-axis value of rotation center.
+    angle : `float`
+        Roation angle in 'radian' unit.
+    dx : (optional) `float`
+        The relative displacement along x-axis
+        of the rotated images to the reference image.
+    dy : (optional) `float`
+        The relative displacement along y-axis
+        of the rotated images to the reference image.
+    inv : (optional) `bool`
+        If True, the do inverse roattion transpose.
+    missing : (optional) `float`
+        The value of extrapolated position.
+        Default is -1, and it means the False.
+        If False, then extrapolate the given position.
+
+    Returns
+    -------
+    result : `~numpy.ndarray`
+        rotated image.
+
+    Notes
+    -----
+    It is not conventional rotation.
+    It is just used for the coalignment module.
+
+    """
+    xt,yt=rot_trans(x, y, xc, yc, angle,
+                    dx, dy, inv)
+    return img_interpol(img, x, y, xt, yt,
+                        missing=missing, cubic=cubic)
+
+def rot(img, angle, xc=False, yc=False,
+        dx=0, dy=0, xmargin=0, ymargin=0, missing=0, cubic=False):
+    """
+    Rotate the input image.
+
+    Parameters
+    ----------
+    img : `~numpy.ndarray`
+        N-dimensional array of image.
+    angle : `float`
+        Roation angle in 'radian' unit.
+    xc : (optional) `float`
+        x-axis value of roatation center.
+        Default is the image center.
+    yc : (optional) `float`
+        y-axis value of rotation center.
+        Default is the image center.
+    dx : (optional) `float`
+        The relative displacement along x-axis
+        of the rotated images to the reference image.
+    dy : (optional) `float`
+        The relative displacement along y-axis
+        of the rotated images to the reference image.
+    xmargin : (optional) `float`
+        The margin value of x-axis
+    ymargin : (optional) `float`
+        The margin value of y-axis
+    missing : (optional) `float`
+        The value of extrapolated position.
+        Default is -1, and it means the False.
+        If False, then extrapolate the given position.
+
+    Returns
+    -------
+    result : `~numpy.ndarray`
+        rotated image.
+
+    Notes
+    -----
+    The input angle must be in radian unit.
+
+    """
+    nx = img.shape[-1]
+    ny = img.shape[-2]
+    nx1=int(nx+2*xmargin)
+    ny1=int(ny+2*ymargin)
+    x=np.arange(nx)
+    y=np.arange(ny)[:,None]
+    xa=np.arange(nx1)-xmargin
+    ya=(np.arange(ny1)-ymargin)[:,None]
+
+
+    if not xc:
+        xc=nx/2
+    if not yc:
+        yc=ny/2
+    xt, yt=rot_trans(xa,ya,xc,yc,angle,dx=dx,dy=dy)
+    return img_interpol(img,x,y,xt,yt,missing=missing, cubic=cubic)
+
+def shift(image, sh, missing=0, cubic=False):
+    """
+    Shift the given image.
+
+    Parameters
+    ----------
+    image :  `~numpy.ndarray`
+        2 dimensional array.
+    sh : tuple, list or ndarray
+        tuple, list or ndarray of shifting value set (y,x)
+    missing: `float`
+        The value of extrapolated position.
+        Default is -1, and it means the False.
+        If False, then extrapolate the given position.
+
+    Returns
+    -------
+    simage : ~numpy.ndarray
+        shifted image.
+    """
+    ny, nx = image.shape
+    x=np.arange(nx)
+    y=np.arange(ny)[:,None]
+    xt=x-sh[1]+y*0
+    yt=y-sh[0]+x*0
+
+    return img_interpol(image,x,y,xt,yt,missing=missing,cubic=cubic)
+
+def shift3d(img, sh):
+    """
+    Shift the given image.
+
+    Parameters
+    ----------
+    image :  `~numpy.ndarray`
+        3 dimensional array.
+    sh : tuple, list or ndarray
+        tuple, list or ndarray of shifting value set (y,x)
+
+    Returns
+    -------
+    simage : ~numpy.ndarray
+        shifted image.
+    """
+    nt, ny, nx =img.shape
+
+    t = np.arange(nt)[:,None,None]
+    y = np.arange(ny)[None,:,None]
+    x = np.arange(nx)
+    tt = t + y*0 + x*0
+    yt = y - sh[0][:, None, None] + t*0 + x*0
+    xt = x - sh[1][:, None, None] + t*0 + y*0
+
+    return img_interpol3d(img, t, y, x, tt, yt, xt, missing=0)
+
+def img_interpol3d(img, ta, ya, xa,
+                   tt, yt, xt, missing=None):
+    """
+    Interpolate the image for a given coordinates.
+
+    Parameters
+    ----------
+    img : `~numpy.ndarray`
+        3 dimensional array of image.
+    xa : `~numpy.ndarray`
+        Row vector of x.
+    ya : `~numpy.ndarray`
+        Colomn vector of y.
+    ta : `~numpy.ndarray`
+        Frame vector.
+    tt : `~numpy.ndarray`
+        Coordinates of the positions in the observed frame.
+    yt : `~numpy.ndarray`
+        Coordinates of the positions in the observed frame.
+    xt : `~numpy.ndarray`
+        Coordinates of the positions in the observed frame.
+    missing : (optional) `float`
+        The value of extrapolated position.
+        Default is -1, and it means the False.
+        If False, then extrapolate the given position.
+
+    Returns
+    -------
+    res : ~numpy.ndarray
+        3 dimensional interpolated image.
+        The size of res is same as input img.
+
+    """
+    shape = xt.shape
+    size = xt.size
+    smin = [ta[0,0,0], ya[0,0,0], xa[0]]
+    smax = [ta[-1,0,0],ya[0,-1,0], xa[-1]]
+    order = [ta.size, ya.size, xa.size]
+    interp = LinearSpline(smin, smax, order, img)
+    a = np.array((tt.reshape(size), yt.reshape(size), xt.reshape(size)))
+    b=interp(a.T)
+    res=b.reshape(shape)
+    if missing is not None:
+        mask=np.invert((xt<=xa.max())*(xt>=xa.min())*(yt<=ya.max())*(yt>=ya.min()))
+        res[mask]=missing
+    return res
```

### Comparing `fisspy-0.9.80/fisspy/image/interactive_image.py` & `fisspy-1.0.0/fisspy/image/interactive_image.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,731 +1,724 @@
-from __future__ import absolute_import, division
-import numpy as np
-import matplotlib.pyplot as plt
-from matplotlib import gridspec
-from fisspy.read.readbase import getRaster as _getRaster
-from fisspy.image.base import alignoffset, shift3d
-
-__author__ = "Juhyung Kang"
-__email__ = "jhkang@astro.snu.ac.kr"
-
-
-class singleBand:
-    """
-    Draw interactive FISS raster, spectrogram and profile for single band.
-
-    Parameters
-    ----------
-    fiss: `fisspy.read.FISS`
-        FISS class.
-    x : `float`
-        X position that you draw a spectral profile.
-        Default is image center.
-    y : `float`
-        Y position that you draw a spectral profile.
-        Default is image center.
-    wv : `float`
-        Wavelength positin that you draw a raster images.
-        Default is central wavelength.
-    scale : `string`
-        Scale method of colarbar limit.
-        Default is minMax.
-        option: 'minMax', 'std', 'log'
-    sigFactor : `float`
-        Factor of standard deviation.
-        This is worked if scale is set to be 'std'
-    helpBox : `bool`
-        Show the interacitve key and simple explanation.
-        Default is True
-
-    Other Parameters
-    ----------------
-    **kwargs : `~matplotlib.pyplot` properties
-    """
-
-    def __init__(self, fiss, x=None, y=None, wv=None, scale='minMax',
-                 sigFactor=3, helpBox=True, **kwargs):
-
-        try:
-            plt.rcParams['keymap.back'].remove('left')
-            plt.rcParams['keymap.forward'].remove('right')
-        except:
-            pass
-
-        if not x:
-            x = fiss.nx//2*fiss.xDelt
-        if not y:
-            y = fiss.ny//2*fiss.yDelt
-        if not wv:
-            wv = fiss.centralWavelength
-        self.extentRaster = fiss.extentRaster
-        self.extentSpectro = fiss.extentSpectro
-        self.scale = scale
-        self.sigFactor = sigFactor
-        self.hw = kwargs.pop('hw', 0.05)
-        self.xpix = round((x-fiss.xDelt/2)/fiss.xDelt)
-        self.x = self.xpix*fiss.xDelt+fiss.xDelt/2
-        self.ypix = round((y-fiss.yDelt/2)/fiss.yDelt)
-        self.y = self.ypix*fiss.yDelt+fiss.yDelt/2
-        self.wv = wv
-        self.x0 = self.x
-        self.y0 = self.y
-        self.wv0 = self.wv
-        self.xH = self.x
-        self.yH = self.y
-        self.wvH = self.wv
-        self.centralWavelength = fiss.centralWavelength
-        self.xDelt = fiss.xDelt
-        self.yDelt = fiss.yDelt
-        self.wvDelt = fiss.wvDelt
-        self.wave = fiss.wave
-        self.data = fiss.data
-        self.band = fiss.band
-        self.cam = fiss.cam
-        self._xMin = self.extentRaster[0]
-        self._xMax = self.extentRaster[1]
-        self._yMin = self.extentRaster[2]
-        self._yMax = self.extentRaster[3]
-        self._wvMin = self.extentSpectro[0]
-        self._wvMax = self.extentSpectro[1]
-
-
-        #Keyboard helpBox
-        if helpBox:
-            helpFig = plt.figure('Keyboard Help Box', figsize=[3.5,3])
-            ax = helpFig.add_subplot(111)
-            ax.set_position([0,0,1,1])
-            ax.set_axis_off()
-            ax.text(0.05,0.9,'ctrl+h: Reset to original setting')
-            ax.text(0.05,0.8,'ctrl+right: Move to right')
-            ax.text(0.05,0.7,'ctrl+left: Move to left')
-            ax.text(0.05,0.6,'ctrl+up: Move to up')
-            ax.text(0.05,0.5,'ctrl+down: Move to down')
-            ax.text(0.05,0.4,'right: Increase the wavelength')
-            ax.text(0.05,0.3,'left: Decrease the wavelength')
-            ax.text(0.05,0.2,'spacebar: Change to current mouse point')
-
-
-        #figure setting
-        figsize = kwargs.pop('figsize', [10, 6])
-        self.cmap = kwargs.pop('cmap', fiss.cmap)
-        self.fig = plt.figure(figsize=figsize)
-        self.fig.canvas.set_window_title(self.band)
-        self.imInterp = kwargs.get('interpolation', fiss.imInterp)
-        gs = gridspec.GridSpec(2, 3)
-        self.axRaster = self.fig.add_subplot(gs[:, 0])
-        self.axSpectro = self.fig.add_subplot(gs[0, 1:])
-        self.axProfile = self.fig.add_subplot(gs[1, 1:])
-        fiss.axRaster = self.axRaster
-        fiss.axSpectro = self.axSpectro
-        fiss.axProfile = self.axProfile
-        self.axRaster.set_xlabel('X (arcsec)')
-        self.axRaster.set_ylabel('Y (arcsec)')
-        self.axSpectro.set_xlabel(r'Wavelength ($\AA$)')
-        self.axSpectro.set_ylabel('Y (arcsec)')
-        self.axProfile.set_xlabel(r'Wavelength ($\AA$)')
-        self.axProfile.set_ylabel('Intensity (Count)')
-        self.axRaster.set_title(fiss.date)
-        self.axSpectro.set_title(r"X = %.2f'', Y = %.2f'' (X$_{pix}$ = %i, Y$_{pix}$ = %i)"%(self.x, self.y, self.xpix, self.ypix))
-        self.axRaster.set_xlim(fiss.extentRaster[0], fiss.extentRaster[1])
-        self.axRaster.set_ylim(fiss.extentRaster[2], fiss.extentRaster[3])
-        self.axSpectro.set_xlim(fiss.extentSpectro[0], fiss.extentSpectro[1])
-        self.axSpectro.set_ylim(fiss.extentSpectro[2], fiss.extentSpectro[3])
-        self.axProfile.set_title(r'%s Band (wv = %.2f $\AA$)'%(fiss.band, self.wv))
-        self.axProfile.set_xlim(fiss.wave.min(), fiss.wave.max())
-        self.axProfile.set_ylim(self.data[self.ypix, self.xpix].min()-100,
-                                self.data[self.ypix, self.xpix].max()+100)
-        self.axProfile.minorticks_on()
-        self.axProfile.tick_params(which='both', direction='in')
-
-
-        # Draw
-        raster = _getRaster(self.data, self.wave, self.wv, self.wvDelt,
-                            hw=self.hw)
-
-        if self.cam == 'A':
-            spectro = self.data[:, self.xpix]
-        elif self.cam == 'B':
-            spectro = self.data[:, self.xpix,::-1]
-        if self.scale == 'log':
-            raster = np.log10(raster)
-            spectro = np.log10(spectro)
-        self.imRaster = self.axRaster.imshow(raster,
-                                             fiss.cmap,
-                                             origin='lower',
-                                             extent=fiss.extentRaster,
-                                             **kwargs)
-        self.imSpectro = self.axSpectro.imshow(spectro,
-                                               fiss.cmap,
-                                               origin='lower',
-                                               extent=fiss.extentSpectro,
-                                               **kwargs)
-        self.plotProfile = self.axProfile.plot(self.wave,
-                                               self.data[self.ypix, self.xpix],
-                                               color='k')[0]
-
-        if self.scale == 'std':
-            self.imRaster.set_clim(np.median(raster)-raster.std()*self.sigFactor,
-                                   np.median(raster)+raster.std()*self.sigFactor)
-            self.imSpectro.set_clim(np.median(spectro)-spectro.std()*self.sigFactor,
-                                    np.median(spectro)+spectro.std()*self.sigFactor)
-        else:
-            self.imRaster.set_clim(raster.min(), raster.max())
-            self.imSpectro.set_clim(spectro.min(), spectro.max())
-
-        # Reference
-        self.vlineRaster = self.axRaster.axvline(self.x,
-                                                 linestyle='dashed',
-                                                 color='lime')
-        self.vlineProfile = self.axProfile.axvline(self.wv,
-                                                   ls='dashed',
-                                                   c='b')
-        self.vlineSpectro = self.axSpectro.axvline(self.wv,
-                                                   ls='dashed',
-                                                   c='lime')
-        self.hlineSpectro = self.axSpectro.axhline(self.y,
-                                                   ls='dashed',
-                                                   c='lime')
-        self.pointRaster = self.axRaster.scatter(self.x, self.y, 50,
-                                                 marker='x',
-                                                 color='r')
-        self.axSpectro.set_aspect(adjustable='box', aspect='auto')
-        self.fig.tight_layout()
-        self.fig.canvas.mpl_connect('key_press_event', self._on_key)
-
-        plt.show()
-
-    def _on_key(self, event):
-
-        ### Interactive keyboard input
-        # Position
-        if event.key == 'ctrl+right':
-            if self.x < self._xMax:
-                self.x += self.xDelt
-            else:
-                self.x = self._xMin
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
-        elif event.key == 'ctrl+left':
-            if self.x > self._xMin:
-                self.x -= self.xDelt
-            else:
-                self.x = self._xMax
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
-        elif event.key == 'ctrl+up':
-            if self.y < self._yMax:
-                self.y += self.yDelt
-            else:
-                self.y = self._yMin
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
-        elif event.key == 'ctrl+down':
-            if self.y > self._yMin:
-                self.y -= self.yDelt
-            else:
-                self.y = self._yMax
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
-        elif event.key == 'right':
-            if self.wv < self._wvMax:
-                self.wv += abs(self.wvDelt)
-            else:
-                self.wv = self._wvMin
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
-        elif event.key == 'left':
-            if self.wv > self._wvMin:
-                self.wv -= abs(self.wvDelt)
-            else:
-                self.wv = self._wvMax
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
-        elif event.key == ' ' and event.inaxes == self.axRaster:
-            self.x = event.xdata
-            self.y = event.ydata
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
-        elif event.key == ' ' and event.inaxes == self.axProfile:
-            self.wv = event.xdata
-            self.wvb = self.wv0
-            self.xb = self.x0
-            self.yb = self.y0
-        elif event.key == ' ' and event.inaxes == self.axSpectro:
-            self.wv = event.xdata
-            self.y = event.ydata
-            self.wvb = self.wv0
-            self.xb = self.x0
-            self.yb = self.y0
-        elif event.key == 'ctrl+h':
-            self.wv = self.wvH
-            self.x = self.xH
-            self.y = self.yH
-        elif event.key == 'ctrl+b':
-            x = self.x
-            y = self.y
-            wv = self.wv
-            self.x = self.xb
-            self.y = self.yb
-            self.wv = self.wvb
-            self.xb = x
-            self.yb = y
-            self.wvb = wv
-        if self.x != self.x0 or self.y != self.y0:
-            self.xpix = int(round((self.x-self.xDelt/2)/self.xDelt))
-            self.ypix = int(round((self.y-self.yDelt/2)/self.yDelt))
-            self._chSpect()
-        if self.wv != self.wv0:
-            self._chRaster()
-        self.fig.canvas.draw_idle()
-
-
-    def _chRaster(self):
-        self.wv0 = self.wv
-        raster = _getRaster(self.data, self.wave, self.wv, self.wvDelt,
-                             hw=self.hw)
-        if self.scale == 'log':
-            raster = np.log10(raster)
-        self.imRaster.set_data(raster)
-        self.vlineProfile.set_xdata(self.wv)
-        self.vlineSpectro.set_xdata(self.wv)
-        self.axProfile.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.band, self.wv))
-        if self.scale == 'std':
-            self.imRaster.set_clim(np.median(raster)-raster.std()*self.sigFactor,
-                                   np.median(raster)+raster.std()*self.sigFactor)
-        else:
-            self.imRaster.set_clim(raster.min(), raster.max())
-
-    def _chSpect(self):
-        self.x0 = self.x
-        self.y0 = self.y
-
-        if self.cam == 'A':
-            spectro = self.data[:, self.xpix]
-        elif self.cam == 'B':
-            spectro = self.data[:, self.xpix,::-1]
-        if self.scale == 'log':
-            spectro = np.log10(spectro)
-        self.plotProfile.set_ydata(self.data[self.ypix, self.xpix])
-        self.imSpectro.set_data(spectro)
-        self.hlineSpectro.set_ydata(self.y)
-        self.vlineRaster.set_xdata(self.x)
-        self.pointRaster.set_offsets([self.x, self.y])
-
-        self.axProfile.set_ylim(self.data[self.ypix, self.xpix].min()-100,
-                                self.data[self.ypix, self.xpix].max()+100)
-        self.axSpectro.set_title(r"X = %.2f'', Y = %.2f'' (X$_{pix}$ = %i, Y$_{pix}$ = %i)"%(self.x, self.y, self.xpix, self.ypix))
-        if self.scale == 'std':
-            self.imSpectro.set_clim(np.median(spectro)-spectro.std()*self.sigFactor,
-                                    np.median(spectro)+spectro.std()*self.sigFactor)
-        else:
-            self.imSpectro.set_clim(spectro.min(), spectro.max())
-
-    def chRasterClim(self, cmin, cmax):
-        self.imRaster.set_clim(cmin, cmax)
-
-    def chSpectroClim(self, cmin, cmax):
-        self.imSpectro.set_clim(cmin, cmax)
-
-    def chcmap(self, cmap):
-        self.imRaster.set_cmap(cmap)
-        self.imSpectro.set_cmap(cmap)
-
-class dualBand:
-    """
-    Draw interactive FISS raster, spectrogram and profile for dual band.
-
-    Parameters
-    ----------
-    fissA: `fisspy.read.FISS`
-        FISS class.
-    fissB: `fisspy.read.FISS`
-        FISS class.
-    x : `float`
-        X position that you draw a spectral profile.
-        Default is image center.
-    y : `float`
-        Y position that you draw a spectral profile.
-        Default is image center.
-    wvA : `float`
-        Wavelength positin that you draw a raster images.
-        Default is central wavelength.
-    wvB : `float`
-        Wavelength positin that you draw a raster images.
-        Default is central wavelength.
-    scale : `string`
-        Scale method of colarbar limit.
-        Default is minMax.
-        option: 'minMax', 'std', 'log'
-    sigFactor : `float`
-        Factor of standard deviation.
-        This is worked if scale is set to be 'std'
-    helpBox : `bool`
-        Show the interacitve key and simple explanation.
-        Default is True
-
-    Other Parameters
-    ----------------
-    **kwargs : `~matplotlib.pyplot` properties
-    """
-    def __init__(self, fissA, fissB, x=None, y=None, wvA=None, wvB=None,
-                 scale='minMax', sigFactor=3, helpBox=True, **kwargs):
-
-        try:
-            plt.rcParams['keymap.back'].remove('left')
-            plt.rcParams['keymap.forward'].remove('right')
-        except:
-            pass
-
-        kwargs['interpolation'] = kwargs.pop('interpolation', 'bilinear')
-        self.fissA = fissA
-        self.fissB = fissB
-        self.nx = self.fissA.nx
-        self.xDelt = self.fissA.xDelt
-        self.yDelt = self.fissA.yDelt
-        if self.fissA.ny >= self.fissB.ny:
-            self.fissA.data = self.fissA.data[:self.fissB.ny]
-            self.ny = self.fissB.ny
-            self.extentRaster = self.fissB.extentRaster
-        elif fissA.ny < fissB.ny:
-            self.fissB.data = self.fissB.data[:self.fissA.ny]
-            self.ny = self.fissA.ny
-            self.extentRaster = self.fissA.extentRaster
-        self._xMin = self.extentRaster[0]
-        self._xMax = self.extentRaster[1]
-        self._yMin = self.extentRaster[2]
-        self._yMax = self.extentRaster[3]
-
-        sh = alignoffset(self.fissB.data[:,:,50], self.fissA.data[:,:,-50])
-        tmp = shift3d(fissB.data.transpose(2, 0, 1), -sh).transpose(1,2,0)
-        self.fissB.data = tmp
-        tmp[tmp<10]=1
-        del tmp
-
-        if not x:
-            x = self.nx//2*self.xDelt
-        if not y:
-            y = self.ny//2*self.yDelt
-        if not wvA:
-            wvA = self.fissA.centralWavelength
-        if not wvB:
-            wvB = self.fissB.centralWavelength
-        xpix = round((x-self.xDelt/2)/self.xDelt)
-        ypix = round((y-self.yDelt/2)/self.yDelt)
-        self.x = xpix*self.xDelt+self.xDelt/2
-        self.y = ypix*self.yDelt+self.yDelt/2
-        self.scale = scale
-        self.sigFactor = sigFactor
-        self.hw = kwargs.pop('hw', 0.05)
-        self.wvA = wvA
-        self.wvB = wvB
-        self.x0 = self.x
-        self.y0 = self.y
-        self.wvA0 = self.wvA
-        self.wvB0 = self.wvB
-        self.xH = self.x
-        self.yH = self.y
-        self.wvAH = self.wvA
-        self.wvBH = self.wvB
-
-        #Keyboard helpBox
-        if helpBox:
-            helpFig = plt.figure('Keyboard Help Box', figsize=[3.5,3])
-            ax = helpFig.add_subplot(111)
-            ax.set_position([0,0,1,1])
-            ax.set_axis_off()
-            ax.text(0.05,0.92,'ctrl+h: Reset to original setting')
-            ax.text(0.05,0.82,'ctrl+right: Move to right')
-            ax.text(0.05,0.72,'ctrl+left: Move to left')
-            ax.text(0.05,0.62,'ctrl+up: Move to up')
-            ax.text(0.05,0.52,'ctrl+down: Move to down')
-            ax.text(0.05,0.42,'right: Increase the wavelength of the fissA')
-            ax.text(0.05,0.32,'left: Decrease the wavelength of the fissA')
-            ax.text(0.05,0.22,'up: Increase the wavelength of the fissB')
-            ax.text(0.05,0.12,'down: Decrease the wavelength of the fissB')
-            ax.text(0.05,0.02,'spacebar: Change to current mouse point')
-
-        #figure setting
-        figsize = kwargs.pop('figsize', [12, 6])
-        self.fig = plt.figure(figsize=figsize)
-        self.fig.canvas.set_window_title('Dual Band Image')
-        self.imInterp = kwargs.get('interpolation', 'bilinear')
-        gs = gridspec.GridSpec(2,4)
-        self.axRasterA = self.fig.add_subplot(gs[:,0])
-        self.axRasterB = self.fig.add_subplot(gs[:,1],
-                                              sharex=self.axRasterA,
-                                              sharey=self.axRasterA)
-        self.axProfileA = self.fig.add_subplot(gs[0,2:])
-        self.axProfileB = self.fig.add_subplot(gs[1,2:])
-        self.axRasterA.set_xlabel('X (arcsec)')
-        self.axRasterA.set_ylabel('Y (arcsec)')
-        self.axRasterB.set_xlabel('X (arcsec)')
-        self.axRasterB.set_ylabel('Y (arcsec)')
-        self.axProfileA.set_xlabel(r'Wavelength ($\AA$)')
-        self.axProfileA.set_ylabel('Intensity (Count)')
-        self.axProfileB.set_xlabel(r'Wavelength ($\AA$)')
-        self.axProfileB.set_ylabel('Intensity (Count)')
-        self.axRasterA.set_title(r'%s Band'%self.fissA.band)
-        self.axRasterB.set_title(r'%s Band'%self.fissB.band)
-        self.axProfileA.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissA.band, self.wvA))
-        self.axProfileB.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissB.band, self.wvB))
-        self.axRasterA.set_xlim(self.extentRaster[0], self.extentRaster[1])
-        self.axRasterB.set_xlim(self.extentRaster[0], self.extentRaster[1])
-        self.axRasterA.set_ylim(self.extentRaster[2], self.extentRaster[3])
-        self.axRasterB.set_ylim(self.extentRaster[2], self.extentRaster[3])
-        self.axProfileA.set_xlim(self.fissA.wave.min(), self.fissA.wave.max())
-        self.axProfileB.set_xlim(self.fissB.wave.min(), self.fissB.wave.max())
-        self.axProfileA.set_ylim(self.fissA.data[ypix, xpix].min()-100,
-                                 self.fissA.data[ypix, xpix].max()+100)
-        self.axProfileB.set_ylim(self.fissB.data[ypix, xpix].min()-100,
-                                 self.fissB.data[ypix, xpix].max()+100)
-        self.axProfileA.minorticks_on()
-        self.axProfileA.tick_params(which='both', direction='in')
-        self.axProfileB.minorticks_on()
-        self.axProfileB.tick_params(which='both', direction='in')
-
-        #Draw
-        rasterA = _getRaster(self.fissA.data, self.fissA.wave, self.wvA,
-                             self.fissA.wvDelt, hw=self.hw)
-        rasterB = _getRaster(self.fissB.data, self.fissB.wave, self.wvB,
-                             self.fissB.wvDelt, hw=self.hw)
-
-        whA = rasterA > 5
-        whB = rasterB > 5
-        if self.scale == 'log':
-            rasterA = np.log10(rasterA)
-            rasterB = np.log10(rasterB)
-        cminA = rasterB[whA].min()
-        cminB = rasterB[whB].min()
-        self.imRasterA = self.axRasterA.imshow(rasterA,
-                                               self.fissA.cmap,
-                                               origin='lower',
-                                               extent=self.extentRaster,
-                                               **kwargs)
-        self.imRasterB = self.axRasterB.imshow(rasterB,
-                                               self.fissB.cmap,
-                                               origin='lower',
-                                               extent=self.extentRaster,
-                                               **kwargs)
-        self.plotProfileA = self.axProfileA.plot(self.fissA.wave,
-                                                 self.fissA.data[ypix, xpix],
-                                                 color='k')[0]
-        self.plotProfileB = self.axProfileB.plot(self.fissB.wave,
-                                                 self.fissB.data[ypix, xpix],
-                                                 color='k')[0]
-
-        if self.scale == 'std':
-            self.imRasterA.set_clim(np.median(rasterA)-rasterA.std()*self.sigFactor,
-                                    np.median(rasterA)+rasterA.std()*self.sigFactor)
-            self.imRasterB.set_clim(np.median(rasterB)-rasterB.std()*self.sigFactor,
-                                    np.median(rasterB)+rasterB.std()*self.sigFactor)
-        else:
-            self.imRasterA.set_clim(cminA, rasterA.max())
-            self.imRasterB.set_clim(cminB, rasterB.max())
-
-        #Reference
-        self.vlineRasterA = self.axRasterA.axvline(self.x,
-                                                   linestyle='dashed',
-                                                   color='lime')
-        self.vlineRasterB = self.axRasterB.axvline(self.x,
-                                                   linestyle='dashed',
-                                                   color='lime')
-        self.vlineProfileA = self.axProfileA.axvline(self.wvA,
-                                                     ls='dashed',
-                                                     c='b')
-        self.vlineProfileB = self.axProfileB.axvline(self.wvB,
-                                                     ls='dashed',
-                                                     c='b')
-        self.pointRasterA = self.axRasterA.scatter(self.x, self.y, 50,
-                                                   marker='x',
-                                                   color='r')
-        self.pointRasterB = self.axRasterB.scatter(self.x, self.y, 50,
-                                                   marker='x',
-                                                   color='r')
-        self.fig.tight_layout()
-        self.fig.canvas.mpl_connect('key_press_event', self._on_key)
-
-
-        plt.show()
-    def _on_key(self, event):
-
-        if event.key == 'ctrl+right':
-            if self.x < self._xMax:
-                self.x += self.xDelt
-            else:
-                self.x = self._xMin+self.xDelt//2
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == 'ctrl+left':
-            if self.x > self._xMin:
-                self.x -= self.xDelt
-            else:
-                self.x = self._xMax-self.xDelt//2
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == 'ctrl+up':
-            if self.y < self._yMax:
-                self.y += self.yDelt
-            else:
-                self.y = self._yMin+self.yDelt//2
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == 'ctrl+down':
-            if self.y > self._yMin:
-                self.y -= self.yDelt
-            else:
-                self.y = self._yMax-self.yDelt//2
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == 'right':
-            if self.wvA < self.fissA.wave.max():
-                self.wvA += abs(self.fissA.wvDelt)
-            else:
-                self.wvA = self.fissA.wave.min()
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == 'left':
-            if self.wvA > self.fissA.wave.min():
-                self.wvA -= abs(self.fissA.wvDelt)
-            else:
-                self.wvA = self.fissA.wave.max()
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == 'up':
-            if self.wvB < self.fissB.wave.max():
-                self.wvB += abs(self.fissB.wvDelt)
-            else:
-                self.wvB = self.fissB.wave.min()
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == 'down':
-            if self.wvB > self.fissB.wave.min():
-                self.wvB -= abs(self.fissB.wvDelt)
-            else:
-                self.wvB = self.fissB.wave.max()
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == ' ' and (event.inaxes == self.axRasterA or
-                                        event.inaxes == self.axRasterB) :
-            self.x = event.xdata
-            self.y = event.ydata
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == ' ' and event.inaxes == self.axProfileA:
-            self.wvA = event.xdata
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == ' ' and event.inaxes == self.axProfileB:
-            self.wvB = event.xdata
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == 'ctrl+h':
-            self.wvA = self.wvAH
-            self.wvB = self.wvBH
-            self.x = self.xH
-            self.y = self.yH
-        elif event.key == 'ctrl+b':
-            x = self.x
-            y = self.y
-            wvA = self.wvA
-            wvB = self.wvB
-            self.x = self.xb
-            self.y = self.yb
-            self.wvA = self.wvAb
-            self.wvB = self.wvBb
-            self.xb = x
-            self.yb = y
-            self.wvAb = wvA
-            self.wvBb = wvB
-
-        if self.x != self.x0 or self.y != self.y0:
-            self._chSpect()
-        if self.wvA != self.wvA0:
-            self._chRasterA()
-        if self.wvB != self.wvB0:
-            self._chRasterB()
-        self.fig.canvas.draw_idle()
-
-    def _chSpect(self):
-        self.x0 = self.x
-        self.y0 = self.y
-        xpix = int(round((self.x-self.xDelt/2)/self.xDelt))
-        ypix = int(round((self.y-self.yDelt/2)/self.yDelt))
-
-        self.plotProfileA.set_ydata(self.fissA.data[ypix, xpix])
-        self.plotProfileB.set_ydata(self.fissB.data[ypix, xpix])
-        self.pointRasterA.set_offsets([self.x, self.y])
-        self.pointRasterB.set_offsets([self.x, self.y])
-        self.vlineRasterA.set_xdata(self.x)
-        self.vlineRasterB.set_xdata(self.x)
-
-        self.axProfileA.set_ylim(self.fissA.data[ypix, xpix].min()-100,
-                                 self.fissA.data[ypix, xpix].max()+100)
-        self.axProfileB.set_ylim(self.fissB.data[ypix, xpix].min()-100,
-                                 self.fissB.data[ypix, xpix].max()+100)
-
-    def _chRasterA(self):
-        self.wvA0 = self.wvA
-        rasterA = _getRaster(self.fissA.data, self.fissA.wave, self.wvA,
-                             self.fissA.wvDelt,
-                             hw=self.hw)
-        wh = rasterA > 5
-        if self.scale == 'log':
-            rasterA = np.log10(rasterA)
-        cmin = rasterA[wh].min()
-        self.imRasterA.set_data(rasterA)
-        self.vlineProfileA.set_xdata(self.wvA)
-        self.axProfileA.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissA.band,
-                                                                self.wvA))
-        if self.scale == 'std':
-            self.imRasterA.set_clim(np.median(rasterA)-rasterA.std()*self.sigFactor,
-                                    np.median(rasterA)+rasterA.std()*self.sigFactor)
-        else:
-            self.imRasterA.set_clim(cmin, rasterA.max())
-
-    def _chRasterB(self):
-        self.wvB0 = self.wvB
-        rasterB = _getRaster(self.fissB.data, self.fissB.wave, self.wvB,
-                             self.fissB.wvDelt,
-                             hw=self.hw)
-        wh = rasterB > 5
-        if self.scale == 'log':
-            rasterB = np.log10(rasterB)
-        cmin = rasterB[wh].min()
-        self.imRasterB.set_data(rasterB)
-        self.vlineProfileB.set_xdata(self.wvB)
-        self.axProfileB.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissB.band,
-                                                                self.wvB))
-        if self.scale == 'std':
-            self.imRasterB.set_clim(np.median(rasterB)-rasterB.std()*self.sigFactor,
-                                    np.median(rasterB)+rasterB.std()*self.sigFactor)
-        else:
-            self.imRasterB.set_clim(cmin, rasterB.max())
+from __future__ import absolute_import, division
+import numpy as np
+import matplotlib.pyplot as plt
+from matplotlib import gridspec
+from ..read.readbase import getRaster as _getRaster
+
+
+__author__ = "Juhyung Kang"
+__email__ = "jhkang@astro.snu.ac.kr"
+__all__ = ["singleBand", "dualBand"]
+
+class singleBand:
+    """
+    Draw interactive FISS raster, spectrogram and profile for single band.
+
+    Parameters
+    ----------
+    fiss: `fisspy.read.FISS`
+        FISS class.
+    x : `float`
+        X position that you draw a spectral profile.
+        Default is image center.
+    y : `float`
+        Y position that you draw a spectral profile.
+        Default is image center.
+    wv : `float`
+        Wavelength positin that you draw a raster images.
+        Default is central wavelength.
+    scale : `string`
+        Scale method of colarbar limit.
+        Default is minMax.
+        option: 'minMax', 'std', 'log'
+    sigFactor : `float`
+        Factor of standard deviation.
+        This is worked if scale is set to be 'std'
+    helpBox : `bool`
+        Show the interacitve key and simple explanation.
+        Default is True
+
+    Other Parameters
+    ----------------
+    **kwargs : `~matplotlib.pyplot` properties
+    """
+
+    def __init__(self, fiss, x=None, y=None, wv=None, scale='minMax',
+                 sigFactor=3, helpBox=True, **kwargs):
+
+        try:
+            plt.rcParams['keymap.back'].remove('left')
+            plt.rcParams['keymap.forward'].remove('right')
+        except:
+            pass
+
+        if not x:
+            x = fiss.nx//2*fiss.xDelt
+        if not y:
+            y = fiss.ny//2*fiss.yDelt
+        if not wv:
+            wv = fiss.centralWavelength
+        self.extentRaster = fiss.extentRaster
+        self.extentSpectro = fiss.extentSpectro
+        self.scale = scale
+        self.sigFactor = sigFactor
+        self.hw = kwargs.pop('hw', 0.05)
+        self.xpix = round((x-fiss.xDelt/2)/fiss.xDelt)
+        self.x = self.xpix*fiss.xDelt+fiss.xDelt/2
+        self.ypix = round((y-fiss.yDelt/2)/fiss.yDelt)
+        self.y = self.ypix*fiss.yDelt+fiss.yDelt/2
+        self.wv = wv
+        self.x0 = self.x
+        self.y0 = self.y
+        self.wv0 = self.wv
+        self.xH = self.x
+        self.yH = self.y
+        self.wvH = self.wv
+        self.centralWavelength = fiss.centralWavelength
+        self.xDelt = fiss.xDelt
+        self.yDelt = fiss.yDelt
+        self.wvDelt = fiss.wvDelt
+        self.wave = fiss.wave
+        self.data = fiss.data
+        self.band = fiss.band
+        self.cam = fiss.cam
+        self._xMin = self.extentRaster[0]
+        self._xMax = self.extentRaster[1]
+        self._yMin = self.extentRaster[2]
+        self._yMax = self.extentRaster[3]
+        self._wvMin = self.extentSpectro[0]
+        self._wvMax = self.extentSpectro[1]
+
+
+        #Keyboard helpBox
+        if helpBox:
+            helpFig = plt.figure('Keyboard Help Box', figsize=[3.5,3])
+            ax = helpFig.add_subplot(111)
+            ax.set_position([0,0,1,1])
+            ax.set_axis_off()
+            ax.text(0.05,0.9,'ctrl/cmd+h: Reset to original setting')
+            ax.text(0.05,0.8,'ctrl/cmd+right: Move to right')
+            ax.text(0.05,0.7,'ctrl/cmd+left: Move to left')
+            ax.text(0.05,0.6,'ctrl/cmd+up: Move to up')
+            ax.text(0.05,0.5,'ctrl/cmd+down: Move to down')
+            ax.text(0.05,0.4,'right: Increase the wavelength')
+            ax.text(0.05,0.3,'left: Decrease the wavelength')
+            ax.text(0.05,0.2,'spacebar: Change to current mouse point')
+            ax.text(0.05,0.1,'ctrl/cmd+b: Show previous point')
+
+
+        #figure setting
+        figsize = kwargs.pop('figsize', [15, 9])
+        self.cmap = kwargs.pop('cmap', fiss.cmap)
+        self.fig = plt.figure(figsize=figsize)
+        # self.fig.canvas.set_window_title(self.band)
+        self.imInterp = kwargs.get('interpolation', fiss.imInterp)
+        gs = gridspec.GridSpec(2, 3)
+        self.axRaster = self.fig.add_subplot(gs[:, 0])
+        self.axSpectro = self.fig.add_subplot(gs[0, 1:])
+        self.axProfile = self.fig.add_subplot(gs[1, 1:])
+        fiss.axRaster = self.axRaster
+        fiss.axSpectro = self.axSpectro
+        fiss.axProfile = self.axProfile
+        self.axRaster.set_xlabel('X (arcsec)')
+        self.axRaster.set_ylabel('Y (arcsec)')
+        self.axSpectro.set_xlabel(r'Wavelength ($\AA$)')
+        self.axSpectro.set_ylabel('Y (arcsec)')
+        self.axProfile.set_xlabel(r'Wavelength ($\AA$)')
+        self.axProfile.set_ylabel('Intensity (Count)')
+        self.axRaster.set_title(fiss.date)
+        self.axSpectro.set_title(r"X = %.2f'', Y = %.2f'' (X$_{pix}$ = %i, Y$_{pix}$ = %i)"%(self.x, self.y, self.xpix, self.ypix))
+        self.axRaster.set_xlim(fiss.extentRaster[0], fiss.extentRaster[1])
+        self.axRaster.set_ylim(fiss.extentRaster[2], fiss.extentRaster[3])
+        self.axSpectro.set_xlim(fiss.extentSpectro[0], fiss.extentSpectro[1])
+        self.axSpectro.set_ylim(fiss.extentSpectro[2], fiss.extentSpectro[3])
+        self.axProfile.set_title(r'%s Band (wv = %.2f $\AA$)'%(fiss.band, self.wv))
+        self.axProfile.set_xlim(fiss.wave.min(), fiss.wave.max())
+        self.axProfile.set_ylim(self.data[self.ypix, self.xpix].min()-100,
+                                self.data[self.ypix, self.xpix].max()+100)
+        self.axProfile.minorticks_on()
+        self.axProfile.tick_params(which='both', direction='in')
+
+
+        # Draw
+        raster = _getRaster(self.data, self.wave, self.wv, self.wvDelt,
+                            hw=self.hw)
+
+        if self.cam == 'A':
+            spectro = self.data[:, self.xpix]
+        elif self.cam == 'B':
+            spectro = self.data[:, self.xpix,::-1]
+        if self.scale == 'log':
+            raster = np.log10(raster)
+            spectro = np.log10(spectro)
+        self.imRaster = self.axRaster.imshow(raster,
+                                             fiss.cmap,
+                                             origin='lower',
+                                             extent=fiss.extentRaster,
+                                             **kwargs)
+        self.imSpectro = self.axSpectro.imshow(spectro,
+                                               fiss.cmap,
+                                               origin='lower',
+                                               extent=fiss.extentSpectro,
+                                               **kwargs)
+        self.plotProfile = self.axProfile.plot(self.wave,
+                                               self.data[self.ypix, self.xpix],
+                                               color='k')[0]
+
+        if self.scale == 'std':
+            self.imRaster.set_clim(np.median(raster)-raster.std()*self.sigFactor,
+                                   np.median(raster)+raster.std()*self.sigFactor)
+            self.imSpectro.set_clim(np.median(spectro)-spectro.std()*self.sigFactor,
+                                    np.median(spectro)+spectro.std()*self.sigFactor)
+        else:
+            self.imRaster.set_clim(raster.min(), raster.max())
+            self.imSpectro.set_clim(spectro.min(), spectro.max())
+
+        # Reference
+        self.vlineRaster = self.axRaster.axvline(self.x,
+                                                 linestyle='dashed',
+                                                 color='lime')
+        self.vlineProfile = self.axProfile.axvline(self.wv,
+                                                   ls='dashed',
+                                                   c='b')
+        self.vlineSpectro = self.axSpectro.axvline(self.wv,
+                                                   ls='dashed',
+                                                   c='lime')
+        self.hlineSpectro = self.axSpectro.axhline(self.y,
+                                                   ls='dashed',
+                                                   c='lime')
+        self.pointRaster = self.axRaster.scatter(self.x, self.y, 50,
+                                                 marker='x',
+                                                 color='r')
+        self.axSpectro.set_aspect(adjustable='box', aspect='auto')
+        self.fig.tight_layout()
+        self.fig.canvas.mpl_connect('key_press_event', self._on_key)
+
+        plt.show()
+
+    def _on_key(self, event):
+
+        ### Interactive keyboard input
+        # Position
+        if event.key == 'ctrl+right' or event.key == 'cmd+right':
+            if self.x < self._xMax:
+                self.x += self.xDelt
+            else:
+                self.x = self._xMin
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvb = self.wv0
+        elif event.key == 'ctrl+left' or event.key == 'cmd+left':
+            if self.x > self._xMin:
+                self.x -= self.xDelt
+            else:
+                self.x = self._xMax
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvb = self.wv0
+        elif event.key == 'ctrl+up' or event.key == 'cmd+up':
+            if self.y < self._yMax:
+                self.y += self.yDelt
+            else:
+                self.y = self._yMin
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvb = self.wv0
+        elif event.key == 'ctrl+down' or event.key == 'cmd+down':
+            if self.y > self._yMin:
+                self.y -= self.yDelt
+            else:
+                self.y = self._yMax
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvb = self.wv0
+        elif event.key == 'right':
+            if self.wv < self._wvMax:
+                self.wv += abs(self.wvDelt)
+            else:
+                self.wv = self._wvMin
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvb = self.wv0
+        elif event.key == 'left':
+            if self.wv > self._wvMin:
+                self.wv -= abs(self.wvDelt)
+            else:
+                self.wv = self._wvMax
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvb = self.wv0
+        elif event.key == ' ' and event.inaxes == self.axRaster:
+            self.x = event.xdata
+            self.y = event.ydata
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvb = self.wv0
+        elif event.key == ' ' and event.inaxes == self.axProfile:
+            self.wv = event.xdata
+            self.wvb = self.wv0
+            self.xb = self.x0
+            self.yb = self.y0
+        elif event.key == ' ' and event.inaxes == self.axSpectro:
+            self.wv = event.xdata
+            self.y = event.ydata
+            self.wvb = self.wv0
+            self.xb = self.x0
+            self.yb = self.y0
+        elif event.key == 'ctrl+h' or event.key == 'cmd+h':
+            self.wv = self.wvH
+            self.x = self.xH
+            self.y = self.yH
+        elif event.key == 'ctrl+b' or event.key == 'cmd+b':
+            x = self.x
+            y = self.y
+            wv = self.wv
+            self.x = self.xb
+            self.y = self.yb
+            self.wv = self.wvb
+            self.xb = x
+            self.yb = y
+            self.wvb = wv
+        if self.x != self.x0 or self.y != self.y0:
+            self.xpix = int(round((self.x-self.xDelt/2)/self.xDelt))
+            self.ypix = int(round((self.y-self.yDelt/2)/self.yDelt))
+            self._chSpect()
+        if self.wv != self.wv0:
+            self._chRaster()
+        self.fig.canvas.draw_idle()
+
+
+    def _chRaster(self):
+        self.wv0 = self.wv
+        raster = _getRaster(self.data, self.wave, self.wv, self.wvDelt,
+                             hw=self.hw)
+        if self.scale == 'log':
+            raster = np.log10(raster)
+        self.imRaster.set_data(raster)
+        self.vlineProfile.set_xdata(self.wv)
+        self.vlineSpectro.set_xdata(self.wv)
+        self.axProfile.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.band, self.wv))
+        if self.scale == 'std':
+            self.imRaster.set_clim(np.median(raster)-raster.std()*self.sigFactor,
+                                   np.median(raster)+raster.std()*self.sigFactor)
+        else:
+            self.imRaster.set_clim(raster.min(), raster.max())
+
+    def _chSpect(self):
+        self.x0 = self.x
+        self.y0 = self.y
+
+        if self.cam == 'A':
+            spectro = self.data[:, self.xpix]
+        elif self.cam == 'B':
+            spectro = self.data[:, self.xpix,::-1]
+        if self.scale == 'log':
+            spectro = np.log10(spectro)
+        self.plotProfile.set_ydata(self.data[self.ypix, self.xpix])
+        self.imSpectro.set_data(spectro)
+        self.hlineSpectro.set_ydata(self.y)
+        self.vlineRaster.set_xdata(self.x)
+        self.pointRaster.set_offsets([self.x, self.y])
+
+        self.axProfile.set_ylim(self.data[self.ypix, self.xpix].min()-100,
+                                self.data[self.ypix, self.xpix].max()+100)
+        self.axSpectro.set_title(r"X = %.2f'', Y = %.2f'' (X$_{pix}$ = %i, Y$_{pix}$ = %i)"%(self.x, self.y, self.xpix, self.ypix))
+        if self.scale == 'std':
+            self.imSpectro.set_clim(np.median(spectro)-spectro.std()*self.sigFactor,
+                                    np.median(spectro)+spectro.std()*self.sigFactor)
+        else:
+            self.imSpectro.set_clim(spectro.min(), spectro.max())
+
+    def chRasterClim(self, cmin, cmax):
+        self.imRaster.set_clim(cmin, cmax)
+
+    def chSpectroClim(self, cmin, cmax):
+        self.imSpectro.set_clim(cmin, cmax)
+
+    def chcmap(self, cmap):
+        self.imRaster.set_cmap(cmap)
+        self.imSpectro.set_cmap(cmap)
+
+class dualBand:
+    """
+    Draw interactive FISS raster, spectrogram and profile for dual band.
+
+    Parameters
+    ----------
+    fissA: `fisspy.read.FISS`
+        FISS class.
+    fissB: `fisspy.read.FISS`
+        FISS class.
+    x : `float`
+        X position that you draw a spectral profile.
+        Default is image center.
+    y : `float`
+        Y position that you draw a spectral profile.
+        Default is image center.
+    wvA : `float`
+        Wavelength positin that you draw a raster images.
+        Default is central wavelength.
+    wvB : `float`
+        Wavelength positin that you draw a raster images.
+        Default is central wavelength.
+    scale : `string`
+        Scale method of colarbar limit.
+        Default is minMax.
+        option: 'minMax', 'std', 'log'
+    sigFactor : `float`
+        Factor of standard deviation.
+        This is worked if scale is set to be 'std'
+    helpBox : `bool`
+        Show the interacitve key and simple explanation.
+        Default is True
+
+    Other Parameters
+    ----------------
+    **kwargs : `~matplotlib.pyplot` properties
+    """
+    def __init__(self, fissA, fissB, x=None, y=None, wvA=None, wvB=None,
+                 scale='minMax', sigFactor=3, helpBox=True, **kwargs):
+
+        try:
+            plt.rcParams['keymap.back'].remove('left')
+            plt.rcParams['keymap.forward'].remove('right')
+        except:
+            pass
+        from ..align import alignOffset, shiftImage3D
+        kwargs['interpolation'] = kwargs.pop('interpolation', 'bilinear')
+        self.fissA = fissA
+        self.fissB = fissB
+        self.nx = self.fissA.nx
+        self.xDelt = self.fissA.xDelt
+        self.yDelt = self.fissA.yDelt
+        if self.fissA.ny >= self.fissB.ny:
+            self.fissA.data = self.fissA.data[:self.fissB.ny]
+            self.ny = self.fissB.ny
+            self.extentRaster = self.fissB.extentRaster
+        elif fissA.ny < fissB.ny:
+            self.fissB.data = self.fissB.data[:self.fissA.ny]
+            self.ny = self.fissA.ny
+            self.extentRaster = self.fissA.extentRaster
+        self._xMin = self.extentRaster[0]
+        self._xMax = self.extentRaster[1]
+        self._yMin = self.extentRaster[2]
+        self._yMax = self.extentRaster[3]
+
+        sh = alignOffset(self.fissB.data[:,:,50], self.fissA.data[:,:,-50])
+        tmp = shiftImage3D(fissB.data.transpose(2, 0, 1), -sh).transpose(1,2,0)
+        self.fissB.data = tmp
+        tmp[tmp<10]=1
+        del tmp
+
+        if not x:
+            x = self.nx//2*self.xDelt
+        if not y:
+            y = self.ny//2*self.yDelt
+        if not wvA:
+            wvA = self.fissA.centralWavelength
+        if not wvB:
+            wvB = self.fissB.centralWavelength
+        xpix = round((x-self.xDelt/2)/self.xDelt)
+        ypix = round((y-self.yDelt/2)/self.yDelt)
+        self.x = xpix*self.xDelt+self.xDelt/2
+        self.y = ypix*self.yDelt+self.yDelt/2
+        self.scale = scale
+        self.sigFactor = sigFactor
+        self.hw = kwargs.pop('hw', 0.05)
+        self.wvA = wvA
+        self.wvB = wvB
+        self.x0 = self.x
+        self.y0 = self.y
+        self.wvA0 = self.wvA
+        self.wvB0 = self.wvB
+        self.xH = self.x
+        self.yH = self.y
+        self.wvAH = self.wvA
+        self.wvBH = self.wvB
+
+        #Keyboard helpBox
+        if helpBox:
+            helpFig = plt.figure('Keyboard Help Box', figsize=[3.5,3])
+            ax = helpFig.add_subplot(111)
+            ax.set_position([0,0,1,1])
+            ax.set_axis_off()
+            ax.text(0.05,0.92,'ctrl+h: Reset to original setting')
+            ax.text(0.05,0.82,'ctrl+right: Move to right')
+            ax.text(0.05,0.72,'ctrl+left: Move to left')
+            ax.text(0.05,0.62,'ctrl+up: Move to up')
+            ax.text(0.05,0.52,'ctrl+down: Move to down')
+            ax.text(0.05,0.42,'right: Increase the wavelength of the fissA')
+            ax.text(0.05,0.32,'left: Decrease the wavelength of the fissA')
+            ax.text(0.05,0.22,'up: Increase the wavelength of the fissB')
+            ax.text(0.05,0.12,'down: Decrease the wavelength of the fissB')
+            ax.text(0.05,0.02,'spacebar: Change to current mouse point')
+
+        #figure setting
+        figsize = kwargs.pop('figsize', [12, 6])
+        self.fig = plt.figure(figsize=figsize)
+        # self.fig.canvas.set_window_title('Dual Band Image')
+        self.imInterp = kwargs.get('interpolation', 'bilinear')
+        gs = gridspec.GridSpec(2,4)
+        self.axRasterA = self.fig.add_subplot(gs[:,0])
+        self.axRasterB = self.fig.add_subplot(gs[:,1],
+                                              sharex=self.axRasterA,
+                                              sharey=self.axRasterA)
+        self.axProfileA = self.fig.add_subplot(gs[0,2:])
+        self.axProfileB = self.fig.add_subplot(gs[1,2:])
+        self.axRasterA.set_xlabel('X (arcsec)')
+        self.axRasterA.set_ylabel('Y (arcsec)')
+        self.axRasterB.set_xlabel('X (arcsec)')
+        self.axRasterB.set_ylabel('Y (arcsec)')
+        self.axProfileA.set_xlabel(r'Wavelength ($\AA$)')
+        self.axProfileA.set_ylabel('Intensity (Count)')
+        self.axProfileB.set_xlabel(r'Wavelength ($\AA$)')
+        self.axProfileB.set_ylabel('Intensity (Count)')
+        self.axRasterA.set_title(r'%s Band'%self.fissA.band)
+        self.axRasterB.set_title(r'%s Band'%self.fissB.band)
+        self.axProfileA.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissA.band, self.wvA))
+        self.axProfileB.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissB.band, self.wvB))
+        self.axRasterA.set_xlim(self.extentRaster[0], self.extentRaster[1])
+        self.axRasterB.set_xlim(self.extentRaster[0], self.extentRaster[1])
+        self.axRasterA.set_ylim(self.extentRaster[2], self.extentRaster[3])
+        self.axRasterB.set_ylim(self.extentRaster[2], self.extentRaster[3])
+        self.axProfileA.set_xlim(self.fissA.wave.min(), self.fissA.wave.max())
+        self.axProfileB.set_xlim(self.fissB.wave.min(), self.fissB.wave.max())
+        self.axProfileA.set_ylim(self.fissA.data[ypix, xpix].min()-100,
+                                 self.fissA.data[ypix, xpix].max()+100)
+        self.axProfileB.set_ylim(self.fissB.data[ypix, xpix].min()-100,
+                                 self.fissB.data[ypix, xpix].max()+100)
+        self.axProfileA.minorticks_on()
+        self.axProfileA.tick_params(which='both', direction='in')
+        self.axProfileB.minorticks_on()
+        self.axProfileB.tick_params(which='both', direction='in')
+
+        #Draw
+        rasterA = _getRaster(self.fissA.data, self.fissA.wave, self.wvA,
+                             self.fissA.wvDelt, hw=self.hw)
+        rasterB = _getRaster(self.fissB.data, self.fissB.wave, self.wvB,
+                             self.fissB.wvDelt, hw=self.hw)
+
+        whA = rasterA > 5
+        whB = rasterB > 5
+        if self.scale == 'log':
+            rasterA = np.log10(rasterA)
+            rasterB = np.log10(rasterB)
+        cminA = rasterB[whA].min()
+        cminB = rasterB[whB].min()
+        self.imRasterA = self.axRasterA.imshow(rasterA,
+                                               self.fissA.cmap,
+                                               origin='lower',
+                                               extent=self.extentRaster,
+                                               **kwargs)
+        self.imRasterB = self.axRasterB.imshow(rasterB,
+                                               self.fissB.cmap,
+                                               origin='lower',
+                                               extent=self.extentRaster,
+                                               **kwargs)
+        self.plotProfileA = self.axProfileA.plot(self.fissA.wave,
+                                                 self.fissA.data[ypix, xpix],
+                                                 color='k')[0]
+        self.plotProfileB = self.axProfileB.plot(self.fissB.wave,
+                                                 self.fissB.data[ypix, xpix],
+                                                 color='k')[0]
+
+        if self.scale == 'std':
+            self.imRasterA.set_clim(np.median(rasterA)-rasterA.std()*self.sigFactor,
+                                    np.median(rasterA)+rasterA.std()*self.sigFactor)
+            self.imRasterB.set_clim(np.median(rasterB)-rasterB.std()*self.sigFactor,
+                                    np.median(rasterB)+rasterB.std()*self.sigFactor)
+        else:
+            self.imRasterA.set_clim(cminA, rasterA.max())
+            self.imRasterB.set_clim(cminB, rasterB.max())
+
+        #Reference
+        self.vlineProfileA = self.axProfileA.axvline(self.wvA,
+                                                     ls='dashed',
+                                                     c='b')
+        self.vlineProfileB = self.axProfileB.axvline(self.wvB,
+                                                     ls='dashed',
+                                                     c='b')
+        self.pointRasterA = self.axRasterA.scatter(self.x, self.y, 50,
+                                                   marker='x',
+                                                   color='r')
+        self.pointRasterB = self.axRasterB.scatter(self.x, self.y, 50,
+                                                   marker='x',
+                                                   color='r')
+        self.fig.tight_layout()
+        self.fig.canvas.mpl_connect('key_press_event', self._on_key)
+
+
+        plt.show()
+    def _on_key(self, event):
+
+        if event.key == 'ctrl+right' or event.key == 'cmd+right':
+            if self.x < self._xMax:
+                self.x += self.xDelt
+            else:
+                self.x = self._xMin+self.xDelt//2
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvAb = self.wvA0
+            self.wvBb = self.wvB0
+        elif event.key == 'ctrl+left' or event.key == 'cmd+left':
+            if self.x > self._xMin:
+                self.x -= self.xDelt
+            else:
+                self.x = self._xMax-self.xDelt//2
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvAb = self.wvA0
+            self.wvBb = self.wvB0
+        elif event.key == 'ctrl+up' or event.key == 'cmd+up':
+            if self.y < self._yMax:
+                self.y += self.yDelt
+            else:
+                self.y = self._yMin+self.yDelt//2
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvAb = self.wvA0
+            self.wvBb = self.wvB0
+        elif event.key == 'ctrl+down' or event.key == 'cmd+down':
+            if self.y > self._yMin:
+                self.y -= self.yDelt
+            else:
+                self.y = self._yMax-self.yDelt//2
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvAb = self.wvA0
+            self.wvBb = self.wvB0
+        elif event.key == 'right':
+            if self.wvA < self.fissA.wave.max():
+                self.wvA += abs(self.fissA.wvDelt)
+            else:
+                self.wvA = self.fissA.wave.min()
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvAb = self.wvA0
+            self.wvBb = self.wvB0
+        elif event.key == 'left':
+            if self.wvA > self.fissA.wave.min():
+                self.wvA -= abs(self.fissA.wvDelt)
+            else:
+                self.wvA = self.fissA.wave.max()
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvAb = self.wvA0
+            self.wvBb = self.wvB0
+        elif event.key == 'up':
+            if self.wvB < self.fissB.wave.max():
+                self.wvB += abs(self.fissB.wvDelt)
+            else:
+                self.wvB = self.fissB.wave.min()
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvAb = self.wvA0
+            self.wvBb = self.wvB0
+        elif event.key == 'down':
+            if self.wvB > self.fissB.wave.min():
+                self.wvB -= abs(self.fissB.wvDelt)
+            else:
+                self.wvB = self.fissB.wave.max()
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvAb = self.wvA0
+            self.wvBb = self.wvB0
+        elif event.key == ' ' and (event.inaxes == self.axRasterA or
+                                        event.inaxes == self.axRasterB) :
+            self.x = event.xdata
+            self.y = event.ydata
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvAb = self.wvA0
+            self.wvBb = self.wvB0
+        elif event.key == ' ' and event.inaxes == self.axProfileA:
+            self.wvA = event.xdata
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvAb = self.wvA0
+            self.wvBb = self.wvB0
+        elif event.key == ' ' and event.inaxes == self.axProfileB:
+            self.wvB = event.xdata
+            self.xb = self.x0
+            self.yb = self.y0
+            self.wvAb = self.wvA0
+            self.wvBb = self.wvB0
+        elif event.key == 'ctrl+h' or event.key == 'cmd+h':
+            self.wvA = self.wvAH
+            self.wvB = self.wvBH
+            self.x = self.xH
+            self.y = self.yH
+        elif event.key == 'ctrl+b' or event.key == 'cmd+b':
+            x = self.x
+            y = self.y
+            wvA = self.wvA
+            wvB = self.wvB
+            self.x = self.xb
+            self.y = self.yb
+            self.wvA = self.wvAb
+            self.wvB = self.wvBb
+            self.xb = x
+            self.yb = y
+            self.wvAb = wvA
+            self.wvBb = wvB
+
+        if self.x != self.x0 or self.y != self.y0:
+            self._chSpect()
+        if self.wvA != self.wvA0:
+            self._chRasterA()
+        if self.wvB != self.wvB0:
+            self._chRasterB()
+        self.fig.canvas.draw_idle()
+
+    def _chSpect(self):
+        self.x0 = self.x
+        self.y0 = self.y
+        xpix = int(round((self.x-self.xDelt/2)/self.xDelt))
+        ypix = int(round((self.y-self.yDelt/2)/self.yDelt))
+
+        self.plotProfileA.set_ydata(self.fissA.data[ypix, xpix])
+        self.plotProfileB.set_ydata(self.fissB.data[ypix, xpix])
+        self.pointRasterA.set_offsets([self.x, self.y])
+        self.pointRasterB.set_offsets([self.x, self.y])
+
+        self.axProfileA.set_ylim(self.fissA.data[ypix, xpix].min()-100,
+                                 self.fissA.data[ypix, xpix].max()+100)
+        self.axProfileB.set_ylim(self.fissB.data[ypix, xpix].min()-100,
+                                 self.fissB.data[ypix, xpix].max()+100)
+
+    def _chRasterA(self):
+        self.wvA0 = self.wvA
+        rasterA = _getRaster(self.fissA.data, self.fissA.wave, self.wvA,
+                             self.fissA.wvDelt,
+                             hw=self.hw)
+        wh = rasterA > 5
+        if self.scale == 'log':
+            rasterA = np.log10(rasterA)
+        cmin = rasterA[wh].min()
+        self.imRasterA.set_data(rasterA)
+        self.vlineProfileA.set_xdata(self.wvA)
+        self.axProfileA.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissA.band,
+                                                                self.wvA))
+        if self.scale == 'std':
+            self.imRasterA.set_clim(np.median(rasterA)-rasterA.std()*self.sigFactor,
+                                    np.median(rasterA)+rasterA.std()*self.sigFactor)
+        else:
+            self.imRasterA.set_clim(cmin, rasterA.max())
+
+    def _chRasterB(self):
+        self.wvB0 = self.wvB
+        rasterB = _getRaster(self.fissB.data, self.fissB.wave, self.wvB,
+                             self.fissB.wvDelt,
+                             hw=self.hw)
+        wh = rasterB > 5
+        if self.scale == 'log':
+            rasterB = np.log10(rasterB)
+        cmin = rasterB[wh].min()
+        self.imRasterB.set_data(rasterB)
+        self.vlineProfileB.set_xdata(self.wvB)
+        self.axProfileB.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissB.band,
+                                                                self.wvB))
+        if self.scale == 'std':
+            self.imRasterB.set_clim(np.median(rasterB)-rasterB.std()*self.sigFactor,
+                                    np.median(rasterB)+rasterB.std()*self.sigFactor)
+        else:
+            self.imRasterB.set_clim(cmin, rasterB.max())
```

### Comparing `fisspy-0.9.80/fisspy/io/read.py` & `fisspy-1.0.0/fisspy/io/read.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,507 +1,507 @@
-"""
-Read the FISS fts file and its header.
-
-"""
-from __future__ import absolute_import, division
-
-__author__ = "Juhyeong Kang"
-__email__ = "jhkang@astro.snu.ac.kr"
-
-from astropy.io import fits
-from scipy.signal import savgol_filter
-from scipy.signal import fftconvolve as conv
-import numpy as np
-import os
-
-__all__ = ['frame', 'pca_read', 'raster', 'getheader', 'frame2raster',
-           'sp_av', 'sp_med', 'wavecalib', 'simple_wvcalib']
-
-def frame(file, x1=0, x2=False, pca=True, ncoeff=False, xmax=False,
-          smooth=False, **kwargs):
-    """Read the FISS fts file.
-
-    Parameters
-    ----------
-    file : str
-        A string of file name to be read.
-    x1 : int
-        A starting index of the frame along the scanning direction.
-    x2 : (optional) int
-        An ending index of the frame along the scanning direction.
-        If not, then the only x1 frame is read.
-    pca : (optional) bool
-        If True, the frame is read from the PCA file.
-        Default is True, but the function automatically check
-        the existance of the pca file.
-    ncoeff : (optional) int
-        The number of coefficients to be used for
-        the construction of frame in a pca file.
-    xmax : (optional) bool
-        If True, the x2 value is set as the maximum end point of the frame.
-            * Default is False.
-    smooth : (optional) bool
-        If True, apply the Savitzky-Golay filter to increase the signal to
-        noise without greatly distorting the signal of the given fts file.
-            * Default is False.
-    nsmooth : (optional) int
-        The number of smooting.
-        Default is 1 for the case of the compressed file,
-        and is 2 for the case of the uncompresseed file.
-    kwargs 
-        The parameters for smooth (savitzky-golay filter), \n
-        See the docstring of the `scipy.signal.savgol_filter`.
-        
-    Returns
-    -------
-    frame : ~numpy.ndarray
-        FISS data frame with the information of (wavelength, y, x).
-
-    References
-    ----------
-    `Savitzky-Golay filter <https://en.wikipedia.org/wiki/Savitzky%E2%80%93Golay_filter>`_.\n
-    `scipy.signal.savgol_filter <https://docs.scipy.org/doc/scipy-0.18.1/reference/generated/scipy.signal.savgol_filter.html#scipy.signal.savgol_filter>`_
-    
-    Notes
-    -----
-        This function is based on the IDL code FISS_READ_FRAME.PRO 
-        written by J. Chae, 2013.
-    
-        This function automatically check the existance of the pca
-        file by reading the fts header.
-        
-    Example
-    -------
-    .. plot::
-        :include-source:
-            
-        import matplotlib.pyplot as plt
-        from fisspy.io import read
-        import fisspy
-        import fisspy.data.sample
-        data=read.frame(fisspy.data.sample.FISS_IMAGE,xmax=True)
-        plt.imshow(data[:,75],cmap=fisspy.cm.ca,origin='lower',interpolation='bilinear')
-        plt.title(r"GST/FISS 8542 $\AA$ Spectrogram")
-        plt.show()
-    """
-    if not file:
-        raise ValueError('Empty filename')
-    if x2 and x2 <= x1:
-        raise ValueError('x2 must be larger than x1')
-    
-    header=fits.getheader(file)
-    
-    try:
-        header['pfile']
-    except:
-        pca=False
-    
-    if xmax and not x2:
-        x2=header['naxis3']
-    elif not x2:
-        x2=x1+1
-    
-    if pca:
-        spec=pca_read(file,header,x1,x2,ncoeff=ncoeff)
-    else:        
-        spec=fits.getdata(file)[x1:x2]
-    if x1+1 == x2:
-        spec=spec[0]
-        return spec
-    spec=spec.transpose((1,0,2)).astype(float)
-    
-    if smooth:
-        winl=kwargs.pop('window_length',7)
-        pord=kwargs.pop('polyorder',3)
-        deriv=kwargs.pop('deriv',0)
-        delta=kwargs.pop('delta',1.0)
-        mode=kwargs.pop('mode','interp')
-        cval=kwargs.pop('cval',0.0)
-        nsmooth=kwargs.pop('nsmooth',int(not pca)+1)
-            
-        for i in range(nsmooth):
-            spec=savgol_filter(spec,winl,pord,deriv=deriv,
-                               delta=delta,mode=mode,cval=cval)
-    return spec
-
-
-def pca_read(file,header,x1,x2=False,ncoeff=False):
-    """
-    Read the pca compressed FISS fts file.
-    
-    Parameters
-    ----------
-    file : str
-        A string of file name to be read.
-    header : astropy.io.fits.header.Header
-        The fts file header.
-    x1   : int
-        A starting index of the frame along the scanning direction.
-    x2   : (optional) int
-        An ending index of the frame along the scanning direction.
-        If not, then the only x1 frame is read.
-    ncoeff : (optional) int
-        The number of coefficients to be used for
-        the construction of frame in a pca file.
-    
-    Returns
-    -------
-    frame : ~numpy.ndarry
-        FISS data frame with the information of (wavelength, y, x).
-        
-    Notes
-    -----
-        This function is based on the IDL code FISS_PCA_READ.PRO
-        written by J. Chae, 2013.
-        The required fts data are two. One is the "_c.fts",
-        and the other is "_p.fts"
-    
-    """
-    if not file:
-        raise ValueError('Empty filename')
-    if not x2:
-        x2 = x1+1
-        
-    dir = os.path.dirname(file)
-    pfile = header['pfile']
-    
-    if dir:
-        pfile = os.path.join(dir, pfile)
-        
-    pdata = fits.getdata(pfile)
-    data = fits.getdata(file)[x1:x2]
-    ncoeff1 = data.shape[2]-1
-    if not ncoeff:
-        ncoeff = ncoeff1
-    elif ncoeff > ncoeff1:
-        ncoeff = ncoeff1
-    
-    spec = np.dot(data[:,:,0:ncoeff],pdata[0:ncoeff,:])
-    spec *= 10.**data[:,:,ncoeff][:,:,None]
-    return spec
-
-def raster(file, wv, hw=0.05, x1=0, x2=False, y1=0, y2=False,
-           pca=True, smooth=False, absScale = False, **kwargs):
-    """
-    Make raster images for a given file at wv of wavelength within width hw
-    
-    Parameters
-    ----------
-    file : str
-        A string of file name to be read.
-    wv   : float or 1d ndarray
-        Referenced wavelengths.
-    hw   : float
-        A half-width of wavelength integration in unit of Angstrom.
-        Default is 0.05
-    x1   : (optional) int
-        A starting index of the frame along the scanning direction.
-    x2   : (optional) int
-        An ending index of the frame along the scanning direction.
-        If not, x2 is set to the maximum end point of the frame.
-    y1   : (optional) int
-        A starting index of the frame along the slit position.
-    y2   : (optional0 int
-        A ending index of the frame along the slit position.
-    pca  : (optional) bool
-        If True, the frame is read from the PCA file.
-        Default is True, but the function automatically check
-        the existance of the pca file.
-    absScale : (optional) bool
-        If True, the wavelength should be given in absolute scale.
-        If Flase, the wavelength should be given in relative scale. 
-    smooth : (optional) bool
-        If True, apply the Savitzky-Golay filter to increase the signal to
-        noise without greatly distorting the signal of the given fts file.
-            * Default is False.
-    kwargs
-        Any additional keyword arguments to read frame.
-        See the docstring of `fisspy.io.read.frame`
-        
-    Returns
-    -------
-    Raster : ~numpy.ndarray
-        Raster image at given wavelengths.
-        
-    Notes
-    -----
-        This function is based on the IDL code FISS_RASTER.PRO
-        written by J. Chae, 2013.
-        This function automatically check the existance of the pca file by
-        reading the fts header.
-    
-    Example
-    -------
-    .. plot::
-        :include-source:
-            
-        import matplotlib.pyplot as plt
-        from fisspy.io import read
-        from fisspy import cm
-        import fisspy.data.sample
-        raster=read.raster(fisspy.data.sample.FISS_IMAGE,0.3)
-        plt.imshow(raster, cmap=cm.ca, origin='lower', interpolation='bilinear')
-        plt.title(r"GST/FISS 8542+0.3 $\AA$ Spectrogram")
-        plt.show()
-    """
-    header = getheader(file,pca)
-    ny = header['NAXIS2']
-    nx = header['NAXIS3']
-    dldw = header['CDELT1']
-    
-    if not file:
-        raise ValueError('Empty filename')
-    if x2 and x2 <= x1+1:
-        raise ValueError('x2 must be larger than x1+1')
-    
-    try:
-        num = wv.shape[0]    
-    except:
-        num = 1
-        wv = np.array([wv])
-    
-    if not x2:
-        x2 = int(nx)
-    if not y2:
-        y2 = int(ny)
-    
-    wl = simple_wvcalib(header, absScale= absScale)
-    if hw < abs(dldw)/2.:
-        hw = abs(dldw)/2.
-    
-    s = np.abs(wl-wv[:,None])<=hw
-    sp = frame(file,x1,x2,pca=pca,smooth=smooth,**kwargs)
-    leng = s.sum(1)
-    if num == 1:
-        img = sp[y1:y2,:,s[0,:]].sum(2)/leng[0]
-        return img.reshape((y2-y1,x2-x1))
-    else:
-        img=np.array([sp[y1:y2,:,s[i,:]].sum(2)/leng[i] for i in range(num)])
-        return img.reshape((num,y2-y1,x2-x1))
-
-
-def getheader(file,pca=True):
-    """
-    Get the FISS fts file header.
-    
-    Parameters
-    ----------
-    file : str
-        A string of file name to be read.
-    pca  : (optional) bool
-        If True, the frame is read from the PCA file.
-        Default is True, but the function automatically check
-        the existance of the pca file.
-    
-    Returns
-    -------
-    header : astropy.io.fits.Header
-        The fts file header.
-    
-    Notes
-    -----
-        This function automatically check the existance of the pca file by
-        reading the fts header.
-    
-    Example
-    -------
-    >>> from fisspy.io import read
-    >>> h=read.getheader(file)
-    >>> h['date']
-    '2014-06-03T16:49:42'
-    """
-    header0 = fits.getheader(file)
-    
-    pfile = header0.pop('pfile',False)
-    if not pfile:
-        return header0
-        
-    header = fits.Header()
-    if pca:
-        header['pfile']=pfile
-        for i in header0['comment']:
-            sori = i.split('=')
-            if len(sori) == 1:
-                skv = sori[0].split(None,1)
-                if len(skv) == 1:
-                    pass
-                else:
-                    header[skv[0]] = skv[1]
-            else:
-                key = sori[0]
-                svc = sori[1].split('/')
-                try:
-                    item = float(svc[0])
-                except:
-                    item = svc[0].split("'")
-                    if len(item) != 1:
-                        item = item[1].split(None,0)[0]
-                    else:
-                        item = item[0].split(None,0)[0]
-                try:
-                    if item-int(svc[0]) == 0:
-                        item = int(item)
-                except:
-                    pass
-                if len(svc) == 1:
-                    header[key] = item
-                else:
-                    header[key] = (item,svc[1])
-                    
-    header['simple'] = True
-    alignl=header0.pop('alignl',-1)
-    
-    if alignl == 0:
-        keys=['reflect','reffr','reffi','cdelt2','cdelt3','crota2',
-              'crpix3','shift3','crpix2','shift2','margin2','margin3']
-        header['alignl'] = (alignl,'Alignment level')
-        for i in keys:
-            header[i] = (header0[i],header0.comments[i])
-        header['history'] = str(header0['history'])
-    if alignl == 1:
-        keys=['reflect','reffr','reffi','cdelt2','cdelt3','crota1',
-              'crota2','crpix3','crval3','shift3','crpix2','crval2',
-              'shift2','margin2','margin3']
-        header['alignl'] = (alignl,'Alignment level')
-        for i in keys:
-            header[i] = (header0[i],header0.comments[i])
-        header['history'] = str(header0['history'])
-        
-    return header
-
-def frame2raster(frame, header, wv, absScale = False):
-    """
-    Make a raster image by using the frame data.
-    
-    Parameters
-    ----------
-    frame : ~numpy.ndarray
-        Data which is read from the fisspy.io.read.frame
-    header : astropy.io.fits.Header
-        FISS data header
-    wv : float or ~numpy.ndarray
-        Referenced wavelengths to draw raster image. It must be the one single float,
-        or 1D array
-    absScale : (optional) bool
-        If True, the wavelength should be given in absolute scale.
-        If Flase, the wavelength should be given in relative scale. 
-    Returns
-    -------
-    Raster : ~numpy.ndarray
-        Raster image at gieven wavelength.
-    """
-    hw = 0.05
-    wl = simple_wvcalib(header, absScale= absScale)
-    s = np.abs(wl - wv) <= hw
-    img = frame[:, :, s].sum(2) / s.sum()
-    return img
-
-def sp_av(file) :
-    a = frame(file, xmax = True)
-    return a.mean(axis = 1)
-
-def sp_med(file) :
-    a = frame(file, xmax = True)
-    return np.median(a, axis = 1)
-
-def wavecalib(band,profile,method=True):
-    """
-    Calibrate the wavelength for FISS spectrum profile.
-    
-    Parameters
-    ----------
-    band : str
-        A string to identify the wavelength.
-        Allowable wavelength bands are '6562','8542','5890','5434'
-    profile : ~numpy.ndarray
-        A 1 dimensional numpy array of spectral profile.
-    Method : (optional) bool
-        * Default is True.
-        If true, the reference lines for calibration are the telluric lines.
-        Else if False, the reference lines are the solar absorption lines.
-    
-    Returns
-    -------
-    wavelength : ~numpy.ndarray
-        Calibrated wavelength.
-    
-    Notes
-    -----
-        This function is based on the FISS IDL code FISS_WV_CALIB.PRO
-        written by J. Chae, 2013.
-    
-    Example
-    -------
-    >>> from fisspy.analysis import doppler
-    >>> wv=doppler.wavecalib('6562',profile)
-    
-    """
-    band=band[0:4]
-    nw=profile.shape[0]
-    
-    if method:
-        if band == '6562':
-            line=np.array([6561.097,6564.206])
-            lamb0=6562.817
-            dldw=0.019182
-        elif band == '8542':
-            line=np.array([8540.817,8546.222])
-            lamb0=8542.090
-            dldw=-0.026252
-        elif band == '5890':
-            line=np.array([5889.951,5892.898])
-            lamb0=5889.9509
-            dldw=0.016847
-        elif band == '5434':
-            line=np.array([5434.524,5436.596])
-            lamb0=5434.5235
-            dldw=-0.016847
-        else:
-            raise ValueError("The wavelength band value is not allowable.\n"+
-                             "Please select the wavelenth "+
-                             "among '6562','8542','5890','5434'")
-    else:
-        if band == '6562':
-            line=np.array([6562.817,6559.580])
-            lamb0=6562.817
-            dldw=0.019182
-        elif band == '8542':
-            line=np.array([8542.089,8537.930])
-            lamb0=8542.090
-            dldw=-0.026252
-        else:
-            raise ValueError("The wavelength band value is not allowable.\n"
-                             "Please select the wavelenth "
-                             "among '6562','8542','5890','5434'")
-    
-    w=np.arange(nw)
-    wl=np.zeros(2)
-    wc=profile[20:nw-20].argmin()+20
-    lamb=(w-wc)*dldw+lamb0
-    
-    for i in range(2):
-        mask=np.abs(lamb-line[i]) <= 0.3
-        wtmp=w[mask]
-        ptmp=conv(profile[mask],[-1,2,-1],'same')
-        mask2=ptmp[1:-1].argmin()+1
-        try:
-            wtmp=wtmp[mask2-3:mask2+4]
-            ptmp=ptmp[mask2-3:mask2+4]
-        except:
-            raise ValueError('Fail to wavelength calibration\n'
-            'please change the method %s to %s' %(repr(method), repr(not method)))
-        c=np.polyfit(wtmp-np.median(wtmp),ptmp,2)
-        wl[i]=np.median(wtmp)-c[1]/(2*c[0])    #local minimum of the profile
-    
-    dldw=(line[1]-line[0])/(wl[1]-wl[0])
-    wc=wl[0]-(line[0]-lamb0)/dldw
-    wavelength=(w-wc)*dldw
-    
-    return wavelength
-
-def simple_wvcalib(header, absScale = False):
-    if absScale:
-        return (np.arange(header['naxis1']) -
-                header['crpix1'])*header['cdelt1'] + header['crval1']
-    else:
-        return (np.arange(header['naxis1']) -
+"""
+Read the FISS fts file and its header.
+
+"""
+from __future__ import absolute_import, division
+
+__author__ = "Juhyeong Kang"
+__email__ = "jhkang@astro.snu.ac.kr"
+
+from astropy.io import fits
+from scipy.signal import savgol_filter
+from scipy.signal import fftconvolve as conv
+import numpy as np
+import os
+
+__all__ = ['frame', 'pca_read', 'raster', 'getheader', 'frame2raster',
+           'sp_av', 'sp_med', 'wavecalib', 'simple_wvcalib']
+
+def frame(file, x1=0, x2=False, pca=True, ncoeff=False, xmax=False,
+          smooth=False, **kwargs):
+    """Read the FISS fts file.
+
+    Parameters
+    ----------
+    file : str
+        A string of file name to be read.
+    x1 : int
+        A starting index of the frame along the scanning direction.
+    x2 : (optional) int
+        An ending index of the frame along the scanning direction.
+        If not, then the only x1 frame is read.
+    pca : (optional) bool
+        If True, the frame is read from the PCA file.
+        Default is True, but the function automatically check
+        the existance of the pca file.
+    ncoeff : (optional) int
+        The number of coefficients to be used for
+        the construction of frame in a pca file.
+    xmax : (optional) bool
+        If True, the x2 value is set as the maximum end point of the frame.
+            * Default is False.
+    smooth : (optional) bool
+        If True, apply the Savitzky-Golay filter to increase the signal to
+        noise without greatly distorting the signal of the given fts file.
+            * Default is False.
+    nsmooth : (optional) int
+        The number of smooting.
+        Default is 1 for the case of the compressed file,
+        and is 2 for the case of the uncompresseed file.
+    kwargs 
+        The parameters for smooth (savitzky-golay filter), \n
+        See the docstring of the `scipy.signal.savgol_filter`.
+        
+    Returns
+    -------
+    frame : ~numpy.ndarray
+        FISS data frame with the information of (wavelength, y, x).
+
+    References
+    ----------
+    `Savitzky-Golay filter <https://en.wikipedia.org/wiki/Savitzky%E2%80%93Golay_filter>`_.\n
+    `scipy.signal.savgol_filter <https://docs.scipy.org/doc/scipy-0.18.1/reference/generated/scipy.signal.savgol_filter.html#scipy.signal.savgol_filter>`_
+    
+    Notes
+    -----
+        This function is based on the IDL code FISS_READ_FRAME.PRO 
+        written by J. Chae, 2013.
+    
+        This function automatically check the existance of the pca
+        file by reading the fts header.
+        
+    Example
+    -------
+    .. plot::
+        :include-source:
+            
+        import matplotlib.pyplot as plt
+        from fisspy.io import read
+        import fisspy
+        import fisspy.data.sample
+        data=read.frame(fisspy.data.sample.FISS_IMAGE,xmax=True)
+        plt.imshow(data[:,75],cmap=fisspy.cm.ca,origin='lower',interpolation='bilinear')
+        plt.title(r"GST/FISS 8542 $\AA$ Spectrogram")
+        plt.show()
+    """
+    if not file:
+        raise ValueError('Empty filename')
+    if x2 and x2 <= x1:
+        raise ValueError('x2 must be larger than x1')
+    
+    header=fits.getheader(file)
+    
+    try:
+        header['pfile']
+    except:
+        pca=False
+    
+    if xmax and not x2:
+        x2=header['naxis3']
+    elif not x2:
+        x2=x1+1
+    
+    if pca:
+        spec=pca_read(file,header,x1,x2,ncoeff=ncoeff)
+    else:        
+        spec=fits.getdata(file)[x1:x2]
+    if x1+1 == x2:
+        spec=spec[0]
+        return spec
+    spec=spec.transpose((1,0,2)).astype(float)
+    
+    if smooth:
+        winl=kwargs.pop('window_length',7)
+        pord=kwargs.pop('polyorder',3)
+        deriv=kwargs.pop('deriv',0)
+        delta=kwargs.pop('delta',1.0)
+        mode=kwargs.pop('mode','interp')
+        cval=kwargs.pop('cval',0.0)
+        nsmooth=kwargs.pop('nsmooth',int(not pca)+1)
+            
+        for i in range(nsmooth):
+            spec=savgol_filter(spec,winl,pord,deriv=deriv,
+                               delta=delta,mode=mode,cval=cval)
+    return spec
+
+
+def pca_read(file,header,x1,x2=False,ncoeff=False):
+    """
+    Read the pca compressed FISS fts file.
+    
+    Parameters
+    ----------
+    file : str
+        A string of file name to be read.
+    header : astropy.io.fits.header.Header
+        The fts file header.
+    x1   : int
+        A starting index of the frame along the scanning direction.
+    x2   : (optional) int
+        An ending index of the frame along the scanning direction.
+        If not, then the only x1 frame is read.
+    ncoeff : (optional) int
+        The number of coefficients to be used for
+        the construction of frame in a pca file.
+    
+    Returns
+    -------
+    frame : ~numpy.ndarry
+        FISS data frame with the information of (wavelength, y, x).
+        
+    Notes
+    -----
+        This function is based on the IDL code FISS_PCA_READ.PRO
+        written by J. Chae, 2013.
+        The required fts data are two. One is the "_c.fts",
+        and the other is "_p.fts"
+    
+    """
+    if not file:
+        raise ValueError('Empty filename')
+    if not x2:
+        x2 = x1+1
+        
+    dir = os.path.dirname(file)
+    pfile = header['pfile']
+    
+    if dir:
+        pfile = os.path.join(dir, pfile)
+        
+    pdata = fits.getdata(pfile)
+    data = fits.getdata(file)[x1:x2]
+    ncoeff1 = data.shape[2]-1
+    if not ncoeff:
+        ncoeff = ncoeff1
+    elif ncoeff > ncoeff1:
+        ncoeff = ncoeff1
+    
+    spec = np.dot(data[:,:,0:ncoeff],pdata[0:ncoeff,:])
+    spec *= 10.**data[:,:,ncoeff][:,:,None]
+    return spec
+
+def raster(file, wv, hw=0.05, x1=0, x2=False, y1=0, y2=False,
+           pca=True, smooth=False, absScale = False, **kwargs):
+    """
+    Make raster images for a given file at wv of wavelength within width hw
+    
+    Parameters
+    ----------
+    file : str
+        A string of file name to be read.
+    wv   : float or 1d ndarray
+        Referenced wavelengths.
+    hw   : float
+        A half-width of wavelength integration in unit of Angstrom.
+        Default is 0.05
+    x1   : (optional) int
+        A starting index of the frame along the scanning direction.
+    x2   : (optional) int
+        An ending index of the frame along the scanning direction.
+        If not, x2 is set to the maximum end point of the frame.
+    y1   : (optional) int
+        A starting index of the frame along the slit position.
+    y2   : (optional0 int
+        A ending index of the frame along the slit position.
+    pca  : (optional) bool
+        If True, the frame is read from the PCA file.
+        Default is True, but the function automatically check
+        the existance of the pca file.
+    absScale : (optional) bool
+        If True, the wavelength should be given in absolute scale.
+        If Flase, the wavelength should be given in relative scale. 
+    smooth : (optional) bool
+        If True, apply the Savitzky-Golay filter to increase the signal to
+        noise without greatly distorting the signal of the given fts file.
+            * Default is False.
+    kwargs
+        Any additional keyword arguments to read frame.
+        See the docstring of `fisspy.io.read.frame`
+        
+    Returns
+    -------
+    Raster : ~numpy.ndarray
+        Raster image at given wavelengths.
+        
+    Notes
+    -----
+        This function is based on the IDL code FISS_RASTER.PRO
+        written by J. Chae, 2013.
+        This function automatically check the existance of the pca file by
+        reading the fts header.
+    
+    Example
+    -------
+    .. plot::
+        :include-source:
+            
+        import matplotlib.pyplot as plt
+        from fisspy.io import read
+        from fisspy import cm
+        import fisspy.data.sample
+        raster=read.raster(fisspy.data.sample.FISS_IMAGE,0.3)
+        plt.imshow(raster, cmap=cm.ca, origin='lower', interpolation='bilinear')
+        plt.title(r"GST/FISS 8542+0.3 $\AA$ Spectrogram")
+        plt.show()
+    """
+    header = getheader(file,pca)
+    ny = header['NAXIS2']
+    nx = header['NAXIS3']
+    dldw = header['CDELT1']
+    
+    if not file:
+        raise ValueError('Empty filename')
+    if x2 and x2 <= x1+1:
+        raise ValueError('x2 must be larger than x1+1')
+    
+    try:
+        num = wv.shape[0]    
+    except:
+        num = 1
+        wv = np.array([wv])
+    
+    if not x2:
+        x2 = int(nx)
+    if not y2:
+        y2 = int(ny)
+    
+    wl = simple_wvcalib(header, absScale= absScale)
+    if hw < abs(dldw)/2.:
+        hw = abs(dldw)/2.
+    
+    s = np.abs(wl-wv[:,None])<=hw
+    sp = frame(file,x1,x2,pca=pca,smooth=smooth,**kwargs)
+    leng = s.sum(1)
+    if num == 1:
+        img = sp[y1:y2,:,s[0,:]].sum(2)/leng[0]
+        return img.reshape((y2-y1,x2-x1))
+    else:
+        img=np.array([sp[y1:y2,:,s[i,:]].sum(2)/leng[i] for i in range(num)])
+        return img.reshape((num,y2-y1,x2-x1))
+
+
+def getheader(file,pca=True):
+    """
+    Get the FISS fts file header.
+    
+    Parameters
+    ----------
+    file : str
+        A string of file name to be read.
+    pca  : (optional) bool
+        If True, the frame is read from the PCA file.
+        Default is True, but the function automatically check
+        the existance of the pca file.
+    
+    Returns
+    -------
+    header : astropy.io.fits.Header
+        The fts file header.
+    
+    Notes
+    -----
+        This function automatically check the existance of the pca file by
+        reading the fts header.
+    
+    Example
+    -------
+    >>> from fisspy.io import read
+    >>> h=read.getheader(file)
+    >>> h['date']
+    '2014-06-03T16:49:42'
+    """
+    header0 = fits.getheader(file)
+    
+    pfile = header0.pop('pfile',False)
+    if not pfile:
+        return header0
+        
+    header = fits.Header()
+    if pca:
+        header['pfile']=pfile
+        for i in header0['comment']:
+            sori = i.split('=')
+            if len(sori) == 1:
+                skv = sori[0].split(None,1)
+                if len(skv) == 1:
+                    pass
+                else:
+                    header[skv[0]] = skv[1]
+            else:
+                key = sori[0]
+                svc = sori[1].split('/')
+                try:
+                    item = float(svc[0])
+                except:
+                    item = svc[0].split("'")
+                    if len(item) != 1:
+                        item = item[1].split(None,0)[0]
+                    else:
+                        item = item[0].split(None,0)[0]
+                try:
+                    if item-int(svc[0]) == 0:
+                        item = int(item)
+                except:
+                    pass
+                if len(svc) == 1:
+                    header[key] = item
+                else:
+                    header[key] = (item,svc[1])
+                    
+    header['simple'] = True
+    alignl=header0.pop('alignl',-1)
+    
+    if alignl == 0:
+        keys=['reflect','reffr','reffi','cdelt2','cdelt3','crota2',
+              'crpix3','shift3','crpix2','shift2','margin2','margin3']
+        header['alignl'] = (alignl,'Alignment level')
+        for i in keys:
+            header[i] = (header0[i],header0.comments[i])
+        header['history'] = str(header0['history'])
+    if alignl == 1:
+        keys=['reflect','reffr','reffi','cdelt2','cdelt3','crota1',
+              'crota2','crpix3','crval3','shift3','crpix2','crval2',
+              'shift2','margin2','margin3']
+        header['alignl'] = (alignl,'Alignment level')
+        for i in keys:
+            header[i] = (header0[i],header0.comments[i])
+        header['history'] = str(header0['history'])
+        
+    return header
+
+def frame2raster(frame, header, wv, absScale = False):
+    """
+    Make a raster image by using the frame data.
+    
+    Parameters
+    ----------
+    frame : ~numpy.ndarray
+        Data which is read from the fisspy.io.read.frame
+    header : astropy.io.fits.Header
+        FISS data header
+    wv : float or ~numpy.ndarray
+        Referenced wavelengths to draw raster image. It must be the one single float,
+        or 1D array
+    absScale : (optional) bool
+        If True, the wavelength should be given in absolute scale.
+        If Flase, the wavelength should be given in relative scale. 
+    Returns
+    -------
+    Raster : ~numpy.ndarray
+        Raster image at gieven wavelength.
+    """
+    hw = 0.05
+    wl = simple_wvcalib(header, absScale= absScale)
+    s = np.abs(wl - wv) <= hw
+    img = frame[:, :, s].sum(2) / s.sum()
+    return img
+
+def sp_av(file) :
+    a = frame(file, xmax = True)
+    return a.mean(axis = 1)
+
+def sp_med(file) :
+    a = frame(file, xmax = True)
+    return np.median(a, axis = 1)
+
+def wavecalib(band,profile,method=True):
+    """
+    Calibrate the wavelength for FISS spectrum profile.
+    
+    Parameters
+    ----------
+    band : str
+        A string to identify the wavelength.
+        Allowable wavelength bands are '6562','8542','5890','5434'
+    profile : ~numpy.ndarray
+        A 1 dimensional numpy array of spectral profile.
+    Method : (optional) bool
+        * Default is True.
+        If true, the reference lines for calibration are the telluric lines.
+        Else if False, the reference lines are the solar absorption lines.
+    
+    Returns
+    -------
+    wavelength : ~numpy.ndarray
+        Calibrated wavelength.
+    
+    Notes
+    -----
+        This function is based on the FISS IDL code FISS_WV_CALIB.PRO
+        written by J. Chae, 2013.
+    
+    Example
+    -------
+    >>> from fisspy.analysis import doppler
+    >>> wv=doppler.wavecalib('6562',profile)
+    
+    """
+    band=band[0:4]
+    nw=profile.shape[0]
+    
+    if method:
+        if band == '6562':
+            line=np.array([6561.097,6564.206])
+            lamb0=6562.817
+            dldw=0.019182
+        elif band == '8542':
+            line=np.array([8540.817,8546.222])
+            lamb0=8542.090
+            dldw=-0.026252
+        elif band == '5890':
+            line=np.array([5889.951,5892.898])
+            lamb0=5889.9509
+            dldw=0.016847
+        elif band == '5434':
+            line=np.array([5434.524,5436.596])
+            lamb0=5434.5235
+            dldw=-0.016847
+        else:
+            raise ValueError("The wavelength band value is not allowable.\n"+
+                             "Please select the wavelenth "+
+                             "among '6562','8542','5890','5434'")
+    else:
+        if band == '6562':
+            line=np.array([6562.817,6559.580])
+            lamb0=6562.817
+            dldw=0.019182
+        elif band == '8542':
+            line=np.array([8542.089,8537.930])
+            lamb0=8542.090
+            dldw=-0.026252
+        else:
+            raise ValueError("The wavelength band value is not allowable.\n"
+                             "Please select the wavelenth "
+                             "among '6562','8542','5890','5434'")
+    
+    w=np.arange(nw)
+    wl=np.zeros(2)
+    wc=profile[20:nw-20].argmin()+20
+    lamb=(w-wc)*dldw+lamb0
+    
+    for i in range(2):
+        mask=np.abs(lamb-line[i]) <= 0.3
+        wtmp=w[mask]
+        ptmp=conv(profile[mask],[-1,2,-1],'same')
+        mask2=ptmp[1:-1].argmin()+1
+        try:
+            wtmp=wtmp[mask2-3:mask2+4]
+            ptmp=ptmp[mask2-3:mask2+4]
+        except:
+            raise ValueError('Fail to wavelength calibration\n'
+            'please change the method %s to %s' %(repr(method), repr(not method)))
+        c=np.polyfit(wtmp-np.median(wtmp),ptmp,2)
+        wl[i]=np.median(wtmp)-c[1]/(2*c[0])    #local minimum of the profile
+    
+    dldw=(line[1]-line[0])/(wl[1]-wl[0])
+    wc=wl[0]-(line[0]-lamb0)/dldw
+    wavelength=(w-wc)*dldw
+    
+    return wavelength
+
+def simple_wvcalib(header, absScale = False):
+    if absScale:
+        return (np.arange(header['naxis1']) -
+                header['crpix1'])*header['cdelt1'] + header['crval1']
+    else:
+        return (np.arange(header['naxis1']) -
                 header['crpix1'])*header['cdelt1']
```

### Comparing `fisspy-0.9.80/fisspy/read/read_factory.py` & `fisspy-1.0.0/fisspy/read/read_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1206 +1,1302 @@
-from __future__ import absolute_import, division
-import numpy as np
-from astropy.io import fits
-from scipy.signal import savgol_filter
-from scipy.signal import fftconvolve as conv
-from fisspy import cm
-import matplotlib.pyplot as plt
-from astropy.constants import c
-from fisspy.analysis.doppler import lambdameter
-from fisspy.image import interactive_image as IAI
-from fisspy.read.readbase import getRaster, getHeader, readFrame
-from fisspy.analysis.filter import FourierFilter
-from astropy.time import Time
-import astropy.units as u
-from matplotlib import gridspec
-from fisspy.analysis.wavelet import Wavelet
-from matplotlib import ticker
-from fisspy.analysis.tdmap import TDmap
-#from mpl_toolkits.axes_grid1 import make_axes_locatable
-
-__author__= "Juhyung Kang"
-__email__ = "jhkang@astro.snu.ac.kr"
-__all__ = ["rawData", "FISS", "FD"]
-
-class rawData:
-    """
-    Read a raw file of the FISS.
-
-    Parameters
-    ----------
-    file : `str`
-        File name of the raw fts data file of the FISS.
-
-    Examples
-    --------
-    >>> from fisspy.read import rawData
-    >>> f = 'D:/fisspy_examples/raw_A.fts'
-    >>> raw = rawData(f)
-    >>> raw.imshow()
-    """
-    def __init__(self, file):
-
-
-        if file.find('A.fts') != -1 or  file.find('B.fts') != -1:
-            self.ftype = 'raw'
-        scale = 0.16
-        self.filename = file
-        self.xDelt = scale
-        self.yDelt = scale
-
-        self.header = fits.getheader(file)
-        self.data = fits.getdata(file)
-        self.data = self.data.transpose([1, 0, 2])
-        self.ndim = self.header['naxis']
-        self.cam = file.split('.fts')[0][-1]
-        if self.cam == 'A':
-            self.wvDelt = 0.019
-        elif self.cam == 'B':
-            self.wvDelt = -0.026
-        self.nwv = self.header['naxis1']
-        self.ny = self.header['naxis2']
-        self.nx = self.header['naxis3']
-        self.date = self.header['date']
-        self.band = self.header['wavelen'][:4]
-        #simple wavelength calibration
-        self.wave = (np.arange(self.nwv)-self.nwv//2)*self.wvDelt
-        self.centralWavelength = 0.
-        self.extentRaster = [0, self.nx*self.xDelt,
-                             0, self.ny*self.yDelt]
-        self.extentSpectro = [self.wave.min()-self.wvDelt/2,
-                              self.wave.max()+self.wvDelt/2,
-                              0, self.ny*self.yDelt]
-
-        if self.band == '6562' or self.band =='8542':
-            self.set = '1'
-        elif self.band == '5889' or self.band == '5434':
-            self.set = '2'
-        self.cmap = plt.cm.gray
-
-    def getRaster(self, wv, hw=0.05):
-        """
-        Make a raster image for a given wavelength with in width 2*hw
-
-        Parameters
-        ----------
-        wv : float
-            Referenced wavelength.
-        hw : float
-            A half-width of wavelength to be integrated
-            Default is 0.05
-
-        Example
-        -------
-        >>> raster = raw.getRaster(0.5)
-
-        """
-        self.wv = wv
-        return getRaster(self.data, self.wave, wv, self.wvDelt, hw=hw)
-
-    def imshow(self, x=None, y=None, wv=None, scale='minMax',
-               sigFactor=3, helpBox=True, **kwargs):
-        """
-        Draw the interactive image for single band FISS raw data.
-
-        Parameters
-        ----------
-        x : `float`
-            X position that you draw a spectral profile.
-            Default is image center.
-        y : `float`
-            Y position that you draw a spectral profile.
-            Default is image center.
-        wv : `float`
-            Wavelength positin that you draw a raster images.
-            Default is central wavelength.
-        scale : `string`
-            Scale method of colarbar limit.
-            Default is minMax.
-            option: 'minMax', 'std', 'log'
-        sigFactor : `float`
-            Factor of standard deviation.
-            This is worked if scale is set to be 'std'
-        helpBox : `bool`
-            Show the interacitve key and simple explanation.
-            Default is True
-
-        Other Parameters
-        ----------------
-        **kwargs : `~matplotlib.pyplot` properties
-        """
-        try:
-            plt.rcParams['keymap.back'].remove('left')
-            plt.rcParams['keymap.forward'].remove('right')
-        except:
-            pass
-
-        if not x:
-            x = self.nx//2*self.xDelt
-        if not y:
-            y = self.ny//2*self.yDelt
-        if not wv:
-            wv = self.centralWavelength
-        self.x = x
-        self.y = y
-        self.wv = wv
-        self.imInterp = kwargs.get('interpolation', 'bilinear')
-        kwargs['interpolation'] = self.imInterp
-        self.iIm = IAI.singleBand(self, x, y, wv,
-                                  scale=scale, sigFactor=sigFactor,
-                                  helpBox=helpBox, **kwargs)  # Basic resource to make interactive image is `~fisspy.image.tdmap.TDmap`
-        plt.show()
-
-    def chRasterClim(self, cmin, cmax):
-        self.iIm.chRasterClim(cmin, cmax)
-
-    def chSpectroClim(self, cmin, cmax):
-        self.iIm.chSpectroClim(cmin, cmax)
-
-    def chcmap(self, cmap):
-        self.iIm.chcmap(cmap)
-
-    def chRaster(self, wv):
-        self.iIm.wv = wv
-        self.iIm._chRaster()
-
-    def chSpect(self, x, y):
-        self.iIm.x = x
-        self.iIm.y = y
-        self.iIm._chSpect()
-
-class FISS:
-    """
-    Read a FISS data file (proc or comp).
-
-    Parameters
-    ----------
-    file : `str`
-        File name of the FISS fts data.
-    x1 : `int`, optional
-        A left limit index of the frame along the scan direction
-    x2 : `int`, optional
-        A right limit index of the frame along the scan direction
-        If None, read all data from x1 to the end of the scan direction.
-    y1 : `int`, optional
-        A left limit index of the frame along the scan direction
-    y2 : `int`, optional
-        A right limit index of the frame along the scan direction
-        If None, read all data from x1 to the end of the scan direction.
-    noceff : `int`, optional
-        he number of coefficients to be used for
-        the construction of frame in a pca file.
-    noiseSuprresion : `bool`, optional
-        If True Savitzky-Golay noise filter is applied in the wavelength axis.
-        Default is False.
-    simpleWvCalib : `bool`, optional
-        If True wavelength is simply calibrated by using the header parameters.
-        Default is True.
-    absScale : `bool`, optional
-        If False the central wavelength is set to be zero.
-        If True the central wavelength is set to be wavelength at lab frame.
-        It works if simpleWvCalibration is True.
-        Default is True
-
-    Other Parameters
-    ----------------
-    **kwargs : `~scipy.signal.svagol_filter` properties
-
-    See also
-    --------
-    `~scipy.signal.savgol_filter`
-
-    Examples
-    --------
-    >>> from fisspy import read
-    >>> import fisspy.data.sample
-    >>> fiss = read.FISS(fisspy.data.sample.FISS_IMAGE)
-    """
-
-    def __init__(self, file, x1=0, x2=None, y1=0, y2=None, ncoeff=False, noiseSuppression=False,
-                 simpleWaveCalib=True, absScale=True, **kwargs):
-        if file.find('1.fts') != -1:
-            self.ftype = 'proc'
-        elif file.find('c.fts') != -1:
-            self.ftype = 'comp'
-
-        if self.ftype != 'proc' and self.ftype != 'comp':
-            raise ValueError("Input file is neither proc nor comp data")
-
-        self.x1 = x1
-        self.x2 = x2
-        self.y1 = y1
-        self.y2 = y2
-        self.filename = file
-        self.xDelt = 0.16
-        self.yDelt = 0.16
-
-        self.header = getHeader(file)
-        self.pfile = self.header.pop('pfile', False)
-        self.data = readFrame(file, self.pfile, x1=x1, x2=x2, y1=y1, y2=y2, ncoeff=ncoeff)
-        self.ndim = self.header['naxis']
-        self.ny, self.nx, self.nwv = self.data.shape
-        self.wvDelt = self.header['cdelt1']
-        self.date = self.header['date']
-        self.band = self.header['wavelen'][:4]
-
-        self.refProfile = self.data.mean((0,1))
-        self.wave = self._waveCalibration(simpleWaveCalib= simpleWaveCalib,
-                                        absScale= absScale, **kwargs)
-
-        self.noiseSuppression = noiseSuppression
-        if noiseSuppression:
-            self._noiseSuppression()
-
-        if self.band == '6562':
-            self.cam = 'A'
-            self.set = '1'
-            self.cmap = cm.ha
-        elif self.band == '8542':
-            self.cam = 'B'
-            self.set = '1'
-            self.cmap = cm.ca
-        elif self.band == '5889':
-            self.cam = 'A'
-            self.set = '2'
-            self.cmap = cm.na
-        elif self.band == '5434':
-            self.cam = 'B'
-            self.set = '2'
-            self.cmap = cm.fe
-
-        self.extentRaster = [0, self.nx*self.xDelt,
-                             0, self.ny*self.yDelt]
-        self.extentSpectro = [self.wave.min()-self.wvDelt/2,
-                              self.wave.max()+self.wvDelt/2,
-                              0, self.ny*self.yDelt]
-
-    def reload(self, x1=0, x2=None, y1=0, y2=None, ncoeff=False, noiseSuppression=False):
-        """
-        Reload the FISS data.
-
-        Parameters
-        ----------
-        x1 : `int`, optional
-            A left limit index of the frame along the scan direction
-        x2 : `int`, optional
-            A right limit index of the frame along the scan direction
-            If None, read all data from x1 to the end of the scan direction.
-        y1 : `int`, optional
-            A left limit index of the frame along the scan direction
-        y2 : `int`, optional
-            A right limit index of the frame along the scan direction
-            If None, read all data from x1 to the end of the scan direction.
-        noceff : `int`, optional
-            he number of coefficients to be used for
-            the construction of frame in a pca file.
-        noiseSuprresion : `bool`, optional
-            If True Savitzky-Golay noise filter is applied in the wavelength axis.
-            Default is False.
-        """
-        self.data = readFrame(self.filename, self.pfile, x1=x1, x2=x2, y1=y1, y2=y2, ncoeff=ncoeff)
-        self.ny, self.nx, self.nwv = self.data.shape
-        self.x1 = x1
-        self.x2 = x2
-        self.y1 = y1
-        self.y2 = y2
-        self.extentRaster = [0, self.nx*self.xDelt,
-                             0, self.ny*self.yDelt]
-        self.extentSpectro = [self.wave.min()-self.wvDelt/2,
-                              self.wave.max()+self.wvDelt/2,
-                              0, self.ny*self.yDelt]
-        if noiseSuppression:
-            self._noiseSuppression()
-
-    def getRaster(self, wv, hw=0.05):
-        """
-        Make a raster image for a given wavelength with in width 2*hw
-
-        Parameters
-        ----------
-        wv : float
-            Referenced wavelength.
-        hw : float
-            A half-width of wavelength to be integrated
-            Default is 0.05
-
-        Example
-        -------
-        >>> from fisspy.read import FISS
-        >>> fiss = FISS(file)
-        >>> raster = fiss.getRaster(0.5)
-        """
-
-        self.wv = wv
-        return getRaster(self.data, self.wave, wv, self.wvDelt, hw=hw)
-
-
-    def _waveCalibration(self, simpleWaveCalib= True, absScale= True,
-                         **kwargs):
-        """
-        Wavelength calibration
-
-        If SimpleWvCalib is True, the wavelength is calibrated by using information in header.
-        If absScale is True, the central wavelength is set to be wavelength in the lab frame,
-        but if absScale is False, the central wavelength is set to be zero.
-        """
-        method = kwargs.pop('method', True)
-        if simpleWaveCalib:
-            self.lamb0 = self.header['crval1']
-            if absScale:
-                self.centralWavelength = self.header['crval1']
-                return (np.arange(self.nwv) -
-                        self.header['crpix1']) * self.header['cdelt1'] + self.header['crval1']
-            else:
-                self.centralWavelength = 0
-                return (np.arange(self.nwv) -
-                        self.header['crpix1']) * self.header['cdelt1']
-        else:
-            if method:
-                if self.band == '6562':
-                    line=np.array([6561.097,6564.206])
-                    lamb0=6562.817
-                    dldw=0.019182
-                elif self.band == '8542':
-                    line=np.array([8540.817,8546.222])
-                    lamb0=8542.090
-                    dldw=-0.026252
-                elif self.band == '5889':
-                    line=np.array([5889.951,5892.898])
-                    lamb0=5889.9509
-                    dldw=0.016847
-                elif self.band == '5434':
-                    line=np.array([5434.524,5436.596])
-                    lamb0=5434.5235
-                    dldw=-0.016847
-            else:
-                if self.band == '6562':
-                    line=np.array([6562.817,6559.580])
-                    lamb0=6562.817
-                    dldw=0.019182
-                elif self.band == '8542':
-                    line=np.array([8542.089,8537.930])
-                    lamb0=8542.090
-                    dldw=-0.026252
-
-        w = np.arange(self.nwv)
-        wl = np.zeros(2)
-        wc = self.refProfile[20:self.nwv-20].argmin() + 20
-        lamb = (w - wc) * dldw + lamb0
-
-        for i in range(2):
-            mask = np.abs(lamb - line[i]) <= 0.3
-            wtmp = w[mask]
-            ptmp = conv(self.refProfile[mask], [-1, 2, -1], 'same')
-            mask2 = ptmp[1:-1].argmin() + 1
-            try:
-                wtmp = wtmp[mask2-3:mask2+4]
-                ptmp = ptmp[mask2-3:mask2+4]
-            except:
-                raise ValueError('Fail to wavelength calibration\n'
-                'please change the method %s to %s' %(repr(method), repr(not method)))
-            c = np.polyfit(wtmp - np.median(wtmp), ptmp, 2)
-            wl[i] = np.median(wtmp) - c[1]/(2*c[0])
-
-        dldw = (line[1] - line[0])/(wl[1] - wl[0])
-        wc = wl[0] - (line[0] - lamb0)/dldw
-        return (w - wc) * dldw
-
-    def _noiseSuppression(self, **kwargs):
-        window_length = kwargs.pop('window_length', 7)
-        polyorder = kwargs.pop('polyorder', 2)
-        deriv = kwargs.pop('deriv', 0)
-        delta = kwargs.pop('delta', 1.0)
-        mode = kwargs.pop('mode', 'interp')
-        cval = kwargs.pop('cval', 0.0)
-
-        self.data = savgol_filter(self.data, window_length, polyorder,
-                                   deriv= deriv, delta= delta, cval= cval,
-                                   mode= mode)
-        self.noiseSuppression = True
-
-
-    def lambdaMeter(self, hw= 0.03, sp= 5e3, wvRange= False,
-                    wvinput= True, shift2velocity= True):
-        """
-        Calculate the doppler shift by using lambda-meter (bisector) method.
-
-        Parameters
-        ----------
-        shift2velocity: `bool`
-            Convert doppler shift value with the velocity (unit: km s^-1)
-        wvinput : bool
-            There are two cases.
-
-        * Case wvinput==True
-
-                hw : float
-                    A half width of the horizontal line segment.
-
-            Returns
-            -------
-            wc : nd ndarray
-                n dimensional array of central wavelength values.
-            intc : nd ndarray
-                n dimensional array of intensies of the line segment.\\
-
-        * Case wvinput==False
-
-                sp : float
-                    An intensity of the horiznotal segment.
-
-            Returns
-            -------
-            wc : nd ndarray
-                n dimensional array of central wavelength values.
-            hwc : nd ndarray
-                n dimensional array of half widths of the line segment.
-
-        """
-        lineShift, intensity = lambdameter(self.wave, self.data,
-                                           ref_spectrum= self.refProfile,
-                                           wvRange= wvRange, hw= hw,
-                                           wvinput= wvinput)
-
-        if shift2velocity:
-            LOSvelocity = (lineShift-self.centralWavelength) * c.to('km/s').value/self.lamb0
-            return LOSvelocity, intensity
-        else:
-            return lineShift, intensity
-
-    def imshow(self, x=None, y=None, wv=None, scale='minMax',
-               sigFactor=3, helpBox=True, **kwargs):
-        """
-        Draw interactive FISS raster, spectrogram and profile for single band.
-
-        Parameters
-        ----------
-        x : `float`
-            X position that you draw a spectral profile.
-            Default is image center.
-        y : `float`
-            Y position that you draw a spectral profile.
-            Default is image center.
-        wv : `float`
-            Wavelength positin that you draw a raster images.
-            Default is central wavelength.
-        scale : `string`
-            Scale method of colarbar limit.
-            Default is minMax.
-            option: 'minMax', 'std', 'log'
-        sigFactor : `float`
-            Factor of standard deviation.
-            This is worked if scale is set to be 'std'
-        helpBox : `bool`
-            Show the interacitve key and simple explanation.
-            Default is True
-
-        Other Parameters
-        ----------------
-        **kwargs : `~matplotlib.pyplot` properties
-        """
-        try:
-            plt.rcParams['keymap.back'].remove('left')
-            plt.rcParams['keymap.forward'].remove('right')
-        except:
-            pass
-
-        if not x:
-            x = self.nx//2*self.xDelt
-        if not y:
-            y = self.ny//2*self.yDelt
-        if not wv:
-            wv = self.centralWavelength
-        self.x = x
-        self.y = y
-        self.wv = wv
-        self.imInterp = kwargs.get('interpolation', 'bilinear')
-        self.cmap = kwargs.pop('cmap', self.cmap)
-        kwargs['interpolation'] = self.imInterp
-        self.iIm = IAI.singleBand(self, x, y, wv,
-                                  scale=scale, sigFactor=sigFactor,
-                                  helpBox=helpBox, **kwargs)  # Basic resource to make interactive image is `~fisspy.image.tdmap.TDmap`
-
-    def chRasterClim(self, cmin, cmax):
-        self.iIm.chRasterClim(cmin, cmax)
-
-    def chSpectroClim(self, cmin, cmax):
-        self.iIm.chSpectroClim(cmin, cmax)
-
-    def chcmap(self, cmap):
-        self.iIm.chcmap(cmap)
-
-    def chRaster(self, wv):
-        self.iIm.wv = wv
-        self.iIm._chRaster()
-
-    def chSpect(self, x, y):
-        self.iIm.x = x
-        self.iIm.y = y
-        self.iIm._chSpect()
-
-class FD:
-    """
-    Read the FISS Data (FD) file.
-
-    Parameters
-    ----------
-    fdFile: `str`
-        File name of the FISS Data file.
-    maskFile: `str`
-        File name of the mask file.
-    timeFile: `str`
-        File name of the time file.
-    maskValue: `float`
-        Value of the mask pixel.
-    spatialAvg: `bool`
-        Subtract the spatially averaged value to all pixels.
-    timeAvg: `bool`
-        Subtract the temporal averaged value to all pixels.
-    """
-    def __init__(self, fdFile, maskFile, timeFile, maskValue=-1,
-                 spatialAvg=False, timeAvg=False):
-        self.maskValue = maskValue
-        self._spAvg = spatialAvg
-        self._timeAvg = timeAvg
-        self.ftype = 'FD'
-        self.data = fits.getdata(fdFile).astype(float)
-        self.fdFile = fdFile
-        self.header = fits.getheader(fdFile)
-        self.time = fits.getdata(timeFile)
-        self.reftpix = np.abs(self.time-0).argmin()
-        self.xDelt = self.yDelt = 0.16
-        self.min0 = np.min(self.data, axis=(1,2))
-        self.max0 = np.max(self.data, axis=(1,2))
-        unit = fits.getheader(timeFile)['unit']
-        if unit == 'min':
-            self.time *= 60
-
-        self.mask = fits.getdata(maskFile).astype(bool)
-        self.dt = np.median(self.time-np.roll(self.time, 1))
-        self.nt, self.ny, self.nx, self.nid = self.data.shape
-
-        reftime = self.header['reftime']
-        self.reftime = _isoRefTime(reftime)
-        self.Time = self.reftime + self.time * u.second
-        self.timei = self.time-self.time[0]
-        self.header['sttime'] = self.Time[0].value
-        wid = self.header['ID1'][:2]
-        if wid == 'HI':
-            self.cmap = [cm.ha]*self.nid
-
-        elif wid == 'Ca':
-            self.cmap = [cm.ca]*self.nid
-        elif wid == 'Na':
-            self.cmap = [cm.na]*self.nid
-        elif wid == 'Fe':
-            self.cmap = [cm.fe]*self.nid
-
-        try:
-            xpos = self.header['xpos']
-            ypos = self.header['ypos']
-        except:
-            xpos = self.header.get('crval1', 0)
-            ypos = self.header.get('crval2', 0)
-        self.xpos = xpos
-        self.ypos = ypos
-        xm = xpos - self.nx/2*self.xDelt
-        xM = xpos + self.nx/2*self.xDelt
-        ym = ypos - self.ny/2*self.yDelt
-        yM = ypos + self.ny/2*self.yDelt
-        self.extent = [xm, xM, ym, yM]
-        self._xar = np.linspace(xm+self.xDelt/2,
-                                xM-self.xDelt/2, self.nx)
-        self._yar = np.linspace(ym+self.yDelt/2,
-                                yM-self.yDelt/2, self.ny)
-        if maskValue != -1:
-            self._mask(maskValue)
-        if spatialAvg:
-            self.spatialAverage()
-        if timeAvg:
-            self.timeAverage()
-        self.min = self.min0[self.reftpix]
-        self.max = self.max0[self.reftpix]
-        self.idh = self.header['ID*']
-        for i in range(self.nid):
-            if self.idh[i][-1] == 'V':
-                self.cmap[i] = plt.cm.RdBu_r
-                tmp = np.abs(self.max[i]-self.min[i])/2*0.7
-                if tmp > 15:
-                    tmp = 0.8
-                self.min[i] = -tmp
-                self.max[i] = tmp
-
-    def _mask(self, val):
-        self.data[np.invert(self.mask),:] = val
-
-    def spatialAverage(self):
-        for i in range(self.nt):
-            med = np.median(self.data[i,self.mask[i]], 0)
-            self.data[i] -= med
-            self.min0[i] -= med
-            self.max0[i] -= med
-
-    def timeAverage(self):
-        med = np.median(self.data, 0)
-        self.data -= med
-        self.min0 -= np.median(med, (0,1))
-        self.max0 -= np.median(med, (0,1))
-
-    def originalData(self, maskValue=-1, spatialAvg=False, timeAvg=False):
-        self.data = fits.getdata(self.fdFile).astype(float)
-        self.min0 = np.min(self.data, axis=(1,2))
-        self.max0 = np.max(self.data, axis=(1,2))
-        if maskValue != -1:
-            self.maskValue = maskValue
-            self._mask(maskValue)
-        if spatialAvg:
-            self.spatialAverage()
-        if timeAvg:
-            self.timeAverage()
-
-        self.min = self.min0[self.reftpix]
-        self.max = self.max0[self.reftpix]
-        for i in range(self.nid):
-            if self.idh[i][-1] == 'V':
-                self.cmap[i] = plt.cm.RdBu_r
-                tmp = np.abs(self.max[i]-self.min[i])/2*0.7
-                if tmp > 15:
-                    tmp = 0.8
-                self.min[i] = -tmp
-                self.max[i] = tmp
-
-    def bandpassFilter(self, filterRange):
-        for n, i in enumerate(filterRange):
-            filterRange[n] = i*1e-3
-        self.data = FourierFilter(self.data, self.nt, self.dt, filterRange)
-        if self.maskValue != -1:
-            self._mask(self.maskValue)
-        self.min0 = np.min(self.data, axis=(1,2))
-        self.max0 = np.max(self.data, axis=(1,2))
-        self.min = self.min0[self.reftpix]
-        self.max = self.max0[self.reftpix]
-        for i in range(self.nid):
-            if self.idh[i][-1] == 'V':
-                self.cmap[i] = plt.cm.RdBu_r
-                tmp = np.abs(self.max[i]-self.min[i])/2*0.7
-                if tmp > 15:
-                    tmp = 0.8
-                self.min[i] = -tmp
-                self.max[i] = tmp
-
-    def imshow(self, x=0, y=0, t=0, cid=0,
-               levels=None, maxPeriod=32, helpBox=True, **kwargs):
-
-        self.kwargs = kwargs
-        try:
-            plt.rcParams['keymap.back'].remove('left')
-            plt.rcParams['keymap.forward'].remove('right')
-        except:
-            pass
-
-
-        # transpose to pixel position.
-        xpix, ypix, tpix = self._pixelPosition(x, y, t)
-        self._x0 = self.x
-        self._y0 = self.y
-        self._t0 = self.t
-        self._xh = self.x
-        self._yh = self.y
-        self._th = self.t
-        self.cid = cid
-        self._cidh = cid
-        self.maxPeriod = maxPeriod
-
-
-        #Keyboard helpBox
-        if helpBox:
-            helpFig = plt.figure('Key Help Box', figsize=[3.5, 3])
-            ax = helpFig.add_subplot(111)
-            ax.set_position([0,0,1,1])
-            ax.set_axis_off()
-            ax.text(0.05, 0.91, 'ctrl+h: Reset to original setting')
-            ax.text(0.05, 0.81, 'ctrl+num: Draw the plot ID = num')
-            ax.text(0.05, 0.71, 'ctrl+right: Move to right')
-            ax.text(0.05, 0.61, 'ctrl+left: Move to left')
-            ax.text(0.05, 0.51, 'ctrl+up: Move to up')
-            ax.text(0.05, 0.41, 'ctrl+down: Move to down')
-            ax.text(0.05, 0.31, 'right: Next time data')
-            ax.text(0.05, 0.21, 'right: Previous time data')
-            ax.text(0.05, 0.11, 'spacebar: change to current mouse point')
-            ax.text(0.05, 0.01, 'ctrl+b: back to the previous image')
-
-
-        # Figure setting
-        figsize = kwargs.pop('figsize', [10, 8])
-        self.fig = plt.figure(figsize=figsize)
-        self.fig.canvas.set_window_title('FISS Data')
-        self.imInterp = kwargs.get('interpolation', 'bilinear')
-        gs = gridspec.GridSpec(5,5)
-
-        self.axRaster = self.fig.add_subplot(gs[0:3, :2]) # Raster
-        self.axRaster.set_xlabel('X (arcsec)')
-        self.axRaster.set_ylabel('Y (arcsec)')
-        self.axRaster.set_title(self.idh[0])
-
-        self.axTS = self.fig.add_subplot(gs[1:3, 2:]) # TimeSeries
-        self.axTS.set_xlabel('Time (sec)')
-        self.axTS.set_ylabel('Intensity (count)')
-        self.axTS.set_xlim(self.timei[0], self.timei[-1])
-        self.axTS.minorticks_on()
-        self.axTS.tick_params(which='both', direction='in')
-        self.axTS.set_title('Time series')
-
-        self.axWavelet = self.fig.add_subplot(gs[3:, 2:])
-        self.axWavelet.set_title('Wavelet Power Spectrum')
-        self.axWavelet.set_xlabel('Time (sec)')
-        self.axWavelet.set_ylabel('Period (minute)')
-        self.axWavelet.set_xlim(self.timei[0], self.timei[-1])
-        self.axWavelet.set_yscale('symlog', basey=2)
-        self.axWavelet.yaxis.set_major_formatter(ticker.ScalarFormatter())
-        self.axWavelet.ticklabel_format(axis='y',style='plain')
-        self.axWavelet.set_ylim(self.maxPeriod, 0.5)
-
-        self.axPower = self.fig.add_subplot(gs[3:, :2])
-        self.axPower.set_title('Power Spectrum')
-
-        self.axPower.set_ylabel('Period (minute)')
-        self.axPower.set_ylim(self.maxPeriod, 0.5)
-        self.axPower.set_yscale('symlog', basey=2)
-        self.axPower.yaxis.set_major_formatter(ticker.ScalarFormatter())
-        self.axPower.ticklabel_format(axis='x',style='sci', scilimits=(0,1))
-        self.axPower.minorticks_on()
-        self.axPower.tick_params(which='both', direction='in')
-
-        # Plot
-        data = self.data[:, ypix, xpix, self.cid]
-        self.imRaster = self.axRaster.imshow(self.data[tpix,:,:,cid],
-                                             self.cmap[cid],
-                                             origin='lower',
-                                             extent=self.extent,
-                                             clim=[self.min[cid],
-                                                   self.max[cid]],
-                                             interpolation=self.imInterp)
-        self.timeseries = self.axTS.plot(self.timei,
-                                         data,
-                                         color='k')[0]
-
-        #wavelet
-        if not levels:
-            levels = [0.1, 0.25, 0.4,
-                      0.55, 0.7, 1]
-        self.levels = levels
-        self._plotWavelet(xpix, ypix)
-#        divider = make_axes_locatable(self.axWavelet)
-#        cax = divider.append_axes('right', size='5%', pad=0.1)
-#        plt.colorbar(self.contourIm, cax=cax)
-
-        #gws
-        self.powerGWS = self.axPower.plot(self.gws, self.period, color='k',
-                                          label='GWS')[0]
-        #lws
-        self.lws = self.wavelet.power[:, tpix]
-        self.powerLWS = self.axPower.plot(self.lws, self.period,
-                                          color='r', label='LWS')[0]
-        self.axPower.legend()
-
-        # marker
-        self.point = self.axRaster.scatter(self.x, self.y, 50,
-                                           marker='x',
-                                           color='r')
-        self.vlineTS = self.axTS.axvline(self.t,
-                                         ls='dashed',
-                                         color='b')
-        self.vlineWavelet = self.axWavelet.axvline(self.t,
-                                                   ls='dashed',
-                                                   color='k')
-        peakPGWS = self.period[self.gws.argmax()]
-        peakPLWS = self.period[self.lws.argmax()]
-        self.hlineGWS = self.axPower.axhline(peakPGWS,
-                                             ls='dotted',
-                                             color='k')
-        self.hlineLWS = self.axPower.axhline(peakPLWS,
-                                             ls='dotted',
-                                             color='r')
-
-        #infoBox
-        self.axInfo = self.fig.add_subplot(gs[0, 2:])
-        self.axInfo.set_axis_off()
-        self.isotInfo = self.axInfo.text(0.05, 0.8,
-                                    '%s'%self.Time[self.tpix].value,
-                                    fontsize=12)
-        self.tInfo = self.axInfo.text(0.05, 0.55,
-                                 't=%i sec (tpix=%i)'%(self.t, self.tpix),
-                                 fontsize=12)
-        self.posiInfo = self.axInfo.text(0.05, 0.3,
-                        "X=%.1f'', Y=%.1f'' (xpix=%i, ypix=%i)"%(self.x,
-                                                                 self.y,
-                                                                 xpix,
-                                                                 ypix),
-                                            fontsize=12)
-        self.peakPeriodGWS = self.axInfo.text(0.05, -0.1,
-                                         r'P$_{peak, GWS}$=%.2f min'%peakPGWS,
-                                         fontsize=12)
-        self.peakPeriodLWS = self.axInfo.text(0.05, -0.35,
-                                         r'P$_{peak, LWS}$=%.2f min'%peakPLWS,
-                                         fontsize=12)
-
-        #Axis limit
-        self.axTS.set_ylim(data.min(), data.max())
-        self.axPower.set_xlim(0, self.lpmax)
-        self.axWavelet.set_aspect(adjustable='box', aspect='auto')
-        self.fig.tight_layout()
-        self.fig.canvas.mpl_connect('key_press_event', self._on_key)
-
-        plt.show()
-
-    def _on_key(self, event):
-        if event.key == 'ctrl+right':
-            if self.x < self._xar[-1]:
-                self.x += self.xDelt
-            else:
-                self.x = self._xar[0]
-            self._xb = self._x0
-            self._yb = self._y0
-            self._tb = self._t0
-        elif event.key == 'ctrl+left':
-            if self.x > self._xar[0]:
-                self.x -= self.xDelt
-            else:
-                self.x = self._xar[-1]
-            self._xb = self._x0
-            self._yb = self._y0
-            self._tb = self._t0
-        elif event.key == 'ctrl+up':
-            if self.y < self._yar[-1]:
-                self.y += self.yDelt
-            else:
-                self.y = self._yar[0]
-            self._xb = self._x0
-            self._yb = self._y0
-            self._tb = self._t0
-        elif event.key == 'ctrl+down':
-            if self.y > self._yar[0]:
-                self.y -= self.yDelt
-            else:
-                self.y = self._yar[-1]
-            self._xb = self._x0
-            self._yb = self._y0
-            self._tb = self._t0
-        elif event.key == 'right':
-            if self.tpix < self.nt-1:
-                self.tpix += 1
-            else:
-                self.tpix = 0
-            self.t = self.timei[self.tpix]
-            self._xb = self._x0
-            self._yb = self._y0
-            self._tb = self._t0
-        elif event.key == 'left':
-            if self.tpix > 0:
-                self.tpix -= 1
-            else:
-                self.tpix = self.nt-1
-            self.t = self.timei[self.tpix]
-            self._xb = self._x0
-            self._yb = self._y0
-            self._tb = self._t0
-        elif event.key == ' ' and event.inaxes == self.axRaster:
-            self._xb = self._x0
-            self._yb = self._y0
-            self._tb = self._t0
-            self.x = event.xdata
-            self.y = event.ydata
-        elif event.key == ' ' and (event.inaxes == self.axTS or
-                                   event.inaxes == self.axWavelet):
-            self.t = event.xdata
-            self._xb = self._x0
-            self._yb = self._y0
-            self._tb = self._t0
-            self.tpix = np.abs(self.timei-self.t).argmin()
-            self.t = self.timei[self.tpix]
-        elif event.key == 'ctrl+b':
-            x = self.x
-            y = self.y
-            t = self.t
-            self.x = self._xb
-            self.y = self._yb
-            self.t = self._tb
-            self._xb = x
-            self._yb = y
-            self._tb = t
-            self.tpix = np.abs(self.timei-self.t).argmin()
-        elif event.key == 'ctrl+h':
-            self.x = self._xh
-            self.y = self._yh
-            self.t = self._th
-            self.tpix = np.abs(self.timei-self.t).argmin()
-            self.cid = self._cidh
-            self._changeID()
-            self.axRaster.set_title(self.idh[self.cid])
-            self.imRaster.set_cmap(self.cmap[self.cid])
-        for iid in range(self.nid):
-            if event.key == 'ctrl+%i'%iid:
-                self.cid = iid
-                self._changeID()
-                self.axRaster.set_title(self.idh[iid])
-                self.imRaster.set_cmap(self.cmap[self.cid])
-                if self.idh[iid][-1] == 'V':
-                    self.axTS.set_ylabel('Velocity (km/s)')
-                else:
-                    self.axTS.set_ylabel('Intensity (Count)')
-
-        if self.x != self._x0 or self.y != self._y0:
-            xpix, ypix, tpix = self._pixelPosition(self.x, self.y,
-                                                   self.t)
-            self._changeWavelet(xpix, ypix)
-            self._changePlot(xpix, ypix)
-            self._x0 = self.x
-            self._y0 = self.y
-            self.posiInfo.set_text(
-                    "X=%.1f'', Y=%.1f'' (xpix=%i, ypix=%i)"%(self.x,
-                                                             self.y,
-                                                             xpix,
-                                                             ypix))
-        if self.t != self._t0:
-            self._changeRaster()
-            self.lws = self.wavelet.power[:, self.tpix]
-            self.powerLWS.set_xdata(self.lws)
-            self.vlineTS.set_xdata(self.t)
-            self.vlineWavelet.set_xdata(self.t)
-            peakPLWS = self.period[self.lws.argmax()]
-            self.hlineLWS.set_ydata(peakPLWS)
-            self._t0 = self.t
-            self.isotInfo.set_text('%s'%self.Time[self.tpix].value)
-            self.tInfo.set_text('t=%i sec (tpix=%i)'%(self.t, self.tpix))
-            self.peakPeriodLWS.set_text(
-                    r'P$_{peak, LWS}$=%.2f min'%peakPLWS)
-        self.fig.canvas.draw_idle()
-
-    def _changeID(self):
-        xpix, ypix, tpix = self._pixelPosition(self.x, self.y,
-                                                   self.t)
-        self._changeWavelet(xpix, ypix)
-        self._changePlot(xpix, ypix)
-        self._changeRaster()
-        self.imRaster.set_clim(self.min[self.cid],
-                               self.max[self.cid])
-
-    def _changePlot(self, xpix, ypix):
-        data = self.data[:, ypix, xpix, self.cid]
-        self.timeseries.set_ydata(data)
-        self.axTS.set_ylim(data.min(), data.max())
-        self.powerGWS.set_xdata(self.gws)
-        self.lws = self.wavelet.power[:, self.tpix]
-        self.powerLWS.set_xdata(self.lws)
-        self.point.set_offsets([self.x, self.y])
-        peakPGWS = self.period[self.gws.argmax()]
-        peakPLWS = self.period[self.lws.argmax()]
-        self.hlineGWS.set_ydata(peakPGWS)
-        self.hlineLWS.set_ydata(peakPLWS)
-        self.peakPeriodGWS.set_text(
-                    r'P$_{peak, GWS}$=%.2f min'%peakPGWS)
-        self.peakPeriodLWS.set_text(
-                    r'$P_{peak, LWS}$=%.2f min'%peakPLWS)
-        self.axPower.set_xlim(0, self.lpmax)
-
-    def _changeRaster(self):
-        self.imRaster.set_data(self.data[self.tpix, :, :, self.cid])
-
-    def _pixelPosition(self, x, y, t):
-        tpix = np.abs(self.timei-t).argmin()
-        xpix = np.abs(self._xar-x).argmin()
-        ypix = np.abs(self._yar-y).argmin()
-        self.x = self._xar[xpix]
-        self.y = self._yar[ypix]
-        self.t = self.timei[tpix]
-        self.tpix = tpix
-        return xpix, ypix, tpix
-
-    def _changeWavelet(self, xpix, ypix):
-        self.axWavelet.cla()
-        self._plotWavelet(xpix, ypix)
-
-    def _plotWavelet(self, xpix, ypix):
-        self.wavelet = Wavelet(self.data[:, ypix, xpix, self.cid],
-                       self.dt, **self.kwargs)
-        self.lpmax = self.wavelet.power.max()
-        self.period = self.wavelet.period/60
-        self.gws = self.wavelet.gws
-        wpower = self.wavelet.power/self.wavelet.power.max()
-        self.contour = self.axWavelet.contourf(self.timei, self.period,
-                                               wpower, len(self.levels),
-                                               colors=['w'])
-        self.contourIm = self.axWavelet.contourf(self.contour,
-                                                 levels=self.levels
-                                                 )
-        self.axWavelet.fill_between(self.timei, self.wavelet.coi/60,
-                                    self.period.max(), color='grey',
-                                    alpha=0.4, hatch='x')
-        self.axWavelet.set_title('Wavelet Power Spectrum')
-        self.axWavelet.set_xlabel('Time (sec)')
-        self.axWavelet.set_ylabel('Period (minute)')
-        self.axWavelet.set_xlim(self.timei[0], self.timei[-1])
-        self.axWavelet.set_yscale('symlog', basey=2)
-        self.axWavelet.yaxis.set_major_formatter(ticker.ScalarFormatter())
-        self.axWavelet.ticklabel_format(axis='y',style='plain')
-        self.vlineWavelet = self.axWavelet.axvline(self.t,
-                                                   ls='dashed',
-                                                   color='k')
-        self.axWavelet.set_ylim(self.maxPeriod, 0.5)
-
-    def chLevels(self, levels):
-        """
-        """
-        self.levels = levels
-        xpix, ypix, tpix = self._pixelPosition(self.x, self.y, self.t)
-        self._changeWavelet(xpix, ypix)
-
-    def chInterp(self, interp):
-        """
-        """
-        self.imInterp = interp
-        self.imRaster.set_interpolation(interp)
-
-    def chBPFilter(self, filterRange):
-        """
-        """
-        self.originalData(maskValue=self.maskValue, spatialAvg=self._spAvg,
-                          timeAvg=self._timeAvg)
-        self.bandpassFilter(filterRange)
-
-    def chRasterClim(self, cmin, cmax):
-        """
-        """
-        self.imRaster.set_clim(cmin, cmax)
-
-    def chPosition(self, x, y):
-        """
-        """
-        self.x = x
-        self.y = y
-        self._x0 = x
-        self._y0 =y
-        xpix, ypix, tpix = self._pixelPosition(x, y, self.t)
-        self._changeWavelet(xpix, ypix)
-        self._changePlot(xpix, ypix)
-        self.posiInfo.set_text(
-                    "X=%.1f'', Y=%.1f'' (xpix=%i, ypix=%i)"%(self.x,
-                                                             self.y,
-                                                             xpix,
-                                                             ypix))
-
-    def chtime(self, t):
-        """
-        """
-        self.t = t
-        self._t0 = t
-        self._changeRaster()
-        self.lws = self.wavelet.power[:, self.tpix]
-        self.LWS.set_xdata(self.lws)
-        self.vlineTS.set_xdata(self.t)
-        self.vlineWavelet.set_xdata(self.t)
-        peakPLWS = self.period[self.lws.argmax()]
-        self.hlineLWS.set_ydata(peakPLWS)
-        self._t0 = self.t
-        self.isotInfo.set_text('%s'%self.Time[self.tpix].value)
-        self.tInfo.set_text('t=%i sec (tpix=%i)'%(self.t, self.tpix))
-        self.peakPeriodLWS.set_text(
-                r'P$_{peak, LWS}$=%.2f min'%peakPLWS)
-
-    def TD(self, ID=0, filterRange=None):
-        hdu = fits.PrimaryHDU(self.data[:,:,:,ID])
-        h= hdu.header
-        h['cdelt1'] = self.xDelt
-        h['cdelt2'] = self.yDelt
-        h['cdelt3'] = self.dt
-        h['crval1'] = self.xpos
-        h['crval2'] = self.ypos
-        h['sttime'] = self.Time[0].value
-
-        return TDmap(self.data[:,:,:,ID], h, self.time,
-                     filterRange=filterRange, cmap=self.cmap[ID])
-
-    def set_clim(self, cmin, cmax):
-        self.imRaster.set_clim(cmin, cmax)
-
-class calibData:
-    """
-    Read the calibration file such as 'BiasDark', 'Flat', 'FLAT' and 'SLIT'.
-
-    Parameters
-    ----------
-    file : str
-
-    """
-
-    def __init__(self, file):
-
-        if file.find('BiasDark') != -1:
-            self.ftype = 'BiasDark'
-        elif file.find('Flat') != -1:
-            self.ftype = 'Flat'
-        elif file.find('FLAT') != -1:
-            self.ftype = 'FLAT'
-        elif file.find('SLIT') != -1:
-            self.ftype = 'SLIT'
-
-        self.data = fits.getdata(file)
-        self.header = fits.getheader(file)
-
-        self.nx = self.header['naxis1']
-        self.ny = self.header['naxis2']
-        if self.ftype == 'Flat':
-            self.nf = self.header['naxis3']
-
-        if file.find('_A') != -1:
-            self.cam = 'A'
-        elif file.find('_B') != -1:
-            self.cam = 'B'
-
-    def imshow(self):
-        """
-        """
-        try:
-            plt.rcParams['keymap.back'].remove('left')
-            plt.rcParams['keymap.forward'].remove('right')
-        except:
-            pass
-
-        self.fig, self.ax = plt.subplots(figsize=[10, 6])
-        if self.ftype != 'Flat':
-            self.image = self.ax.imshow(self.data, origin='lower',
-                                        cmap = plt.cm.gray)
-            self.fig.tight_layout()
-        else:
-            self.num = 0
-            self.num0 = self.num
-            self.image = self.ax.imshow(self.data[self.num], origin='lower',
-                                        cmap = plt.cm.gray)
-            self.fig.tight_layout()
-            self.fig.canvas.mpl_connect('key_press_event', self._onKey)
-
-    def _onKey(self, event):
-        if event.key == 'right':
-            if self.num < self.nf-1:
-                self.num += 1
-            else:
-                self.num = 0
-        elif event.key == 'left':
-            if self.num > 0:
-                self.num -= 1
-            else:
-                self.num = self.nf-1
-        if self.num != self.num0:
-            self.image.set_data(self.data[self.num])
-            self.num0 = self.num
-        self.fig.canvas.draw_idle()
-
-def _isoRefTime(refTime):
-    year = refTime[:4]
-    month = refTime[4:6]
-    day = refTime[6:8]
-    hour = refTime[9:11]
-    minute = refTime[11:13]
-    sec = refTime[13:15]
-    isot = '%s-%s-%sT%s:%s:%s'%(year, month, day, hour, minute, sec)
-    return Time(isot)
+from __future__ import absolute_import, division
+import numpy as np
+from astropy.io import fits
+from astropy.time import Time
+import astropy.constants as ac
+import astropy.units as u
+import matplotlib.pyplot as plt
+from matplotlib import gridspec
+from matplotlib import ticker
+from .. import cm
+from .readbase import getRaster, getHeader, readFrame
+from ..analysis import lambdameter
+from ..image import interactive_image as II
+from ..correction import LineName, wvCalib, smoothingProf
+from ..analysis import FourierFilter, Wavelet, makeTDmap
+
+__author__= "Juhyung Kang"
+__email__ = "jhkang0301@gmail.com"
+__all__ = ["rawData", "FISS", "FD", "calibData"]
+
+class rawData:
+    """
+    Read a raw file of the FISS.
+
+    Parameters
+    ----------
+    file : `str`
+        File name of the raw fts data file of the FISS.
+
+    Examples
+    --------
+    >>> from fisspy.read import rawData
+    >>> f = 'D:/fisspy_examples/raw_A.fts'
+    >>> raw = rawData(f)
+    >>> raw.imshow()
+    """
+    def __init__(self, file):
+
+
+        if file.find('A.fts') != -1 or  file.find('B.fts') != -1:
+            self.ftype = 'raw'
+        scale = 0.16
+        self.filename = file
+        self.xDelt = scale
+        self.yDelt = scale
+
+        self.header = fits.getheader(file)
+        self.data = fits.getdata(file)
+        self.data = self.data.transpose([1, 0, 2])
+        self.ndim = self.header['naxis']
+        self.cam = file.split('.fts')[0][-1]
+        if self.cam == 'A':
+            self.wvDelt = 0.019
+        elif self.cam == 'B':
+            self.wvDelt = -0.026
+        self.nwv = self.header['naxis1']
+        self.ny = self.header['naxis2']
+        self.nx = self.header['naxis3']
+        self.date = self.header['date']
+        try:
+            self.band = self.header['wavelen'][:4]
+        except:
+            self.band = str(self.header['gratwvln'])[:4]
+        #simple wavelength calibration
+        self.wave = (np.arange(self.nwv)-self.nwv//2)*self.wvDelt
+        self.centralWavelength = 0.
+        self.extentRaster = [0, self.nx*self.xDelt,
+                             0, self.ny*self.yDelt]
+        self.extentSpectro = [self.wave.min()-self.wvDelt/2,
+                              self.wave.max()+self.wvDelt/2,
+                              0, self.ny*self.yDelt]
+
+        if self.band == '6562' or self.band =='8542':
+            self.set = '1'
+        elif self.band == '5889' or self.band == '5434':
+            self.set = '2'
+        self.cmap = plt.cm.gray
+
+    def getRaster(self, wv, hw=0.05):
+        """
+        Make a raster image for a given wavelength with in width 2*hw
+
+        Parameters
+        ----------
+        wv : float
+            Referenced wavelength.
+        hw : float
+            A half-width of wavelength to be integrated
+            Default is 0.05
+
+        Example
+        -------
+        >>> raster = raw.getRaster(0.5)
+
+        """
+        self.wv = wv
+        return getRaster(self.data, self.wave, wv, self.wvDelt, hw=hw)
+
+    def imshow(self, x=None, y=None, wv=None, scale='minMax',
+               sigFactor=3, helpBox=True, **kwargs):
+        """
+        Draw the interactive image for single band FISS raw data.
+
+        Parameters
+        ----------
+        x : `float`
+            X position that you draw a spectral profile.
+            Default is image center.
+        y : `float`
+            Y position that you draw a spectral profile.
+            Default is image center.
+        wv : `float`
+            Wavelength positin that you draw a raster images.
+            Default is central wavelength.
+        scale : `string`
+            Scale method of colarbar limit.
+            Default is minMax.
+            option: 'minMax', 'std', 'log'
+        sigFactor : `float`
+            Factor of standard deviation.
+            This is worked if scale is set to be 'std'
+        helpBox : `bool`
+            Show the interacitve key and simple explanation.
+            Default is True
+
+        Other Parameters
+        ----------------
+        **kwargs : `~matplotlib.pyplot` properties
+        """
+        try:
+            plt.rcParams['keymap.back'].remove('left')
+            plt.rcParams['keymap.forward'].remove('right')
+        except:
+            pass
+
+        if not x:
+            x = self.nx//2*self.xDelt
+        if not y:
+            y = self.ny//2*self.yDelt
+        if not wv:
+            wv = self.centralWavelength
+        self.x = x
+        self.y = y
+        self.wv = wv
+        self.imInterp = kwargs.get('interpolation', 'bilinear')
+        kwargs['interpolation'] = self.imInterp
+        self.iIm = II.singleBand(self, x, y, wv,
+                                  scale=scale, sigFactor=sigFactor,
+                                  helpBox=helpBox, **kwargs)  # Basic resource to make interactive image is `~fisspy.image.tdmap.TDmap`
+        plt.show()
+
+    def chRasterClim(self, cmin, cmax):
+        self.iIm.chRasterClim(cmin, cmax)
+
+    def chSpectroClim(self, cmin, cmax):
+        self.iIm.chSpectroClim(cmin, cmax)
+
+    def chcmap(self, cmap):
+        self.iIm.chcmap(cmap)
+
+    def chRaster(self, wv):
+        self.iIm.wv = wv
+        self.iIm._chRaster()
+
+    def chSpect(self, x, y):
+        self.iIm.x = x
+        self.iIm.y = y
+        self.iIm._chSpect()
+
+class FISS:
+    """
+    Read a FISS data file (proc or comp).
+
+    Parameters
+    ----------
+    file: `str`
+        File name of the FISS fts data.
+    x1: `int`, optional
+        A left limit index of the frame along the scan direction
+    x2: `int`, optional
+        A right limit index of the frame along the scan direction
+        If None, read all data from x1 to the end of the scan direction.
+    y1: `int`, optional
+        A left limit index of the frame along the scan direction
+    y2: `int`, optional
+        A right limit index of the frame along the scan direction
+        If None, read all data from x1 to the end of the scan direction.
+    noceff: `int`, optional
+        The number of coefficients to be used for
+        the construction of frame in a pca file.
+    smoothingMethod: `str`, optional
+        If it is not given, do not apply the noise filter.
+        If 'savgol', apply the Savitzky-Golay noise filter in the wavelength axis.
+        If 'gauss', apply the Gaussian noise filter in the wavelength axis.
+        Default is None.
+    wvCalibMethod: `str`, optional
+        Method to calibrate wavelength.
+        'simple': calibration with the information of the header.
+        'center': calibration with the center of the main line.
+        'photo': calibration with the photospheric line and the main line.
+        Default is 'simple'.
+
+    Other Parameters
+    ----------------
+    **kwargs : `~scipy.signal.savgol_filter` properties or `~scipy.ndimage.gaussian_filter1d` properties.
+
+    See also
+    --------
+    `~scipy.signal.savgol_filter`.
+    `~scipy.ndimage.gaussian_filter1d`
+
+    Examples
+    --------
+    >>> from fisspy import read
+    >>> import fisspy.data.sample
+    >>> fiss = read.FISS(fisspy.data.sample.FISS_IMAGE)
+    """
+
+    def __init__(self, file, x1=0, x2=None, y1=0, y2=None, ncoeff=False, smoothingMethod=None, wvCalibMethod='photo', **kwargs):
+        if file.find('1.fts') != -1:
+            self.ftype = 'proc'
+        elif file.find('c.fts') != -1:
+            self.ftype = 'comp'
+
+        if self.ftype != 'proc' and self.ftype != 'comp':
+            raise ValueError("Input file is neither proc nor comp data")
+
+        self.x1 = x1
+        self.x2 = x2
+        self.y1 = y1
+        self.y2 = y2
+        self.filename = file
+        self.xDelt = 0.16
+        self.yDelt = 0.16
+
+        self.header = getHeader(file)
+        self.pfile = self.header.pop('pfile', False)
+        self.data = readFrame(file, self.pfile, x1=x1, x2=x2, y1=y1, y2=y2, ncoeff=ncoeff)
+        self.ndim = self.header['naxis']
+        self.ny, self.nx, self.nwv = self.data.shape
+        self.wvDelt = self.header['cdelt1']
+        self.date = self.header['date']
+        try:
+            self.band = self.header['wavelen'][:4]
+        except:
+            self.band = str(self.header['gratwvln'])[:4]
+
+        self.refProfile = self.data.mean((0,1))
+        self.wave = self.wvCalib(method=wvCalibMethod)
+        self.cwv = self.centralWavelength = cwv = self.header['crval1']
+
+        self.smoothing = False
+        if smoothingMethod is not None:
+            self.smoothing = True
+        if self.smoothing:
+            self.smoothingProf(method=smoothingMethod, **kwargs)
+        
+
+        self.line = LineName(cwv)
+        if self.line == 'Ha':
+            self.cam = 'A'
+            self.set = '1'
+            self.cmap = cm.ha
+        elif self.line == 'Ca':
+            self.cam = 'B'
+            self.set = '1'
+            self.cmap = cm.ca
+        elif self.line == 'Na':
+            self.cam = 'A'
+            self.set = '2'
+            self.cmap = cm.na
+        elif self.line == 'Fe':
+            self.cam = 'B'
+            self.set = '2'
+            self.cmap = cm.fe
+
+        self.extentRaster = [0, self.nx*self.xDelt,
+                             0, self.ny*self.yDelt]
+        self.extentSpectro = [self.wave.min()-self.wvDelt/2,
+                              self.wave.max()+self.wvDelt/2,
+                              0, self.ny*self.yDelt]
+        self.lv = None
+
+    def reload(self, x1=0, x2=None, y1=0, y2=None, ncoeff=False, smoothingMethod=None, **kwargs):
+        """
+        Reload the FISS data.
+
+        Parameters
+        ----------
+        x1 : `int`, optional
+            A left limit index of the frame along the scan direction
+        x2 : `int`, optional
+            A right limit index of the frame along the scan direction
+            If None, read all data from x1 to the end of the scan direction.
+        y1 : `int`, optional
+            A left limit index of the frame along the scan direction
+        y2 : `int`, optional
+            A right limit index of the frame along the scan direction
+            If None, read all data from x1 to the end of the scan direction.
+        noceff : `int`, optional
+            he number of coefficients to be used for
+            the construction of frame in a pca file.
+        smoothingMethod: `str`, optional
+            If it is not given, do not apply the noise filter.
+            If 'savgol', apply the Savitzky-Golay noise filter in the wavelength axis.
+            If 'gauss', apply the Gaussian noise filter in the wavelength axis.
+            Default is None.
+
+        Other Parameters
+        ----------------
+        **kwargs : `~scipy.signal.savgol_filter` properties or `~scipy.ndimage.gaussian_filter1d` properties.
+
+        See also
+        --------
+        `~scipy.signal.savgol_filter`.
+        `~scipy.ndimage.gaussian_filter1d`
+        """
+        self.data = readFrame(self.filename, self.pfile, x1=x1, x2=x2, y1=y1, y2=y2, ncoeff=ncoeff)
+        self.ny, self.nx, self.nwv = self.data.shape
+        self.x1 = x1
+        self.x2 = x2
+        self.y1 = y1
+        self.y2 = y2
+        self.extentRaster = [0, self.nx*self.xDelt,
+                             0, self.ny*self.yDelt]
+        self.extentSpectro = [self.wave.min()-self.wvDelt/2,
+                              self.wave.max()+self.wvDelt/2,
+                              0, self.ny*self.yDelt]
+        
+        if smoothingMethod is None:
+            self.smoothing = True
+        if self.smoothing:
+            self.smoothingProf(method=smoothingMethod, **kwargs)
+
+    def getRaster(self, wv, hw=0.05):
+        """
+        Make a raster image for a given wavelength with in width 2*hw
+
+        Parameters
+        ----------
+        wv : float
+            Referenced wavelength.
+        hw : float
+            A half-width of wavelength to be integrated
+            Default is 0.05
+
+        Example
+        -------
+        >>> from fisspy.read import FISS
+        >>> fiss = FISS(file)
+        >>> raster = fiss.getRaster(0.5)
+        """
+
+        self.wv = wv
+        return getRaster(self.data, self.wave, wv, self.wvDelt, hw=hw)
+
+
+    def wvCalib(self, profile=None, method='photo'):
+        """
+        Wavelength calibration
+
+        Parameters
+        ---------
+        profile: `~numpy.ndarray`
+            Spectrum
+        method: `str`
+            Method to calibrate wavelength.
+            'simple': calibration with the information of the header.
+            'center': calibration with the center of the main line.
+            'photo': calibration with the photospheric line and the main line.
+            Default is 'simple'.
+
+        Returns
+        -------
+        wv: `~numpy.ndarray`
+            Wavelength.
+        """
+        if profile is None:
+            pf = self.refProfile
+        else:
+            pf = profile
+        return wvCalib(pf, self.header, method=method)
+
+    def smoothingProf(self, method='savgol', **kwargs):
+        """
+        Parameters
+        ----------
+        method: `str`, optional
+            If 'savgol', apply the Savitzky-Golay noise filter in the wavelength axis.
+            If 'gauss', apply the Gaussian noise filter in the wavelength axis.
+            Default is 'savgol'.
+
+        Other Parameters
+        ----------------
+        **kwargs : `~scipy.signal.savgol_filter` properties or `~scipy.ndimage.gaussian_filter1d` properties.
+        """
+        self.data = smoothingProf(self.data, method=method, **kwargs)
+        self.smoothing = True
+
+    def lambdameter(self, **kw):
+        """
+        Calculate the doppler shift by using lambda-meter (bisector) method.
+
+        Parameters
+        ----------
+        **kw:
+            See `~fisspy.analysis.doppler.lambdameter`
+
+        Returns
+        -------
+        wc : `~numpy.ndarray`
+            n dimensional array of central wavelength values.
+        intc : `~numpy.ndarray`
+            n dimensional array of intensies of the line segment.
+
+        """
+        self.hw = kw.get('hw', 0.05)
+        self.lwc, self.lic = lambdameter(self.wave, self.data, **kw)
+        self.lv = (self.lwc-self.centralWavelength)/self.centralWavelength * ac.c.to('km/s').value
+        
+    def imshow(self, x=None, y=None, wv=None, scale='minMax',
+               sigFactor=3, helpBox=True, **kwargs):
+        """
+        Draw interactive FISS raster, spectrogram and profile for single band.
+
+        Parameters
+        ----------
+        x : `float`
+            X position that you draw a spectral profile.
+            Default is image center.
+        y : `float`
+            Y position that you draw a spectral profile.
+            Default is image center.
+        wv : `float`
+            Wavelength positin that you draw a raster images.
+            Default is central wavelength.
+        scale : `string`
+            Scale method of colarbar limit.
+            Default is minMax.
+            option: 'minMax', 'std', 'log'
+        sigFactor : `float`
+            Factor of standard deviation.
+            This is worked if scale is set to be 'std'
+        helpBox : `bool`
+            Show the interacitve key and simple explanation.
+            Default is True
+
+        Other Parameters
+        ----------------
+        **kwargs : `~matplotlib.pyplot` properties
+        """
+        try:
+            plt.rcParams['keymap.back'].remove('left')
+            plt.rcParams['keymap.forward'].remove('right')
+        except:
+            pass
+
+        if x is None:
+            x = self.nx//2*self.xDelt
+        if y is None:
+            y = self.ny//2*self.yDelt
+        if wv is None:
+            wv = self.centralWavelength
+        self.x = x
+        self.y = y
+        self.wv = wv
+        self.imInterp = kwargs.get('interpolation', 'bilinear')
+        self.cmap = kwargs.pop('cmap', self.cmap)
+        kwargs['interpolation'] = self.imInterp
+        self.iIm = II.singleBand(self, x, y, wv,
+                                  scale=scale, sigFactor=sigFactor,
+                                  helpBox=helpBox, **kwargs)  # Basic resource to make interactive image is `~fisspy.image.tdmap.TDmap`
+
+    def chRasterClim(self, cmin, cmax):
+        self.iIm.chRasterClim(cmin, cmax)
+
+    def chSpectroClim(self, cmin, cmax):
+        self.iIm.chSpectroClim(cmin, cmax)
+
+    def chcmap(self, cmap):
+        self.iIm.chcmap(cmap)
+
+    def chRaster(self, wv):
+        self.iIm.wv = wv
+        self.iIm._chRaster()
+
+    def chSpect(self, x, y):
+        self.iIm.x = x
+        self.iIm.y = y
+        self.iIm._chSpect()
+
+    def vshow(self, x=None, y=None, **kw):
+        try:
+            plt.rcParams['keymap.back'].remove('left')
+            plt.rcParams['keymap.forward'].remove('right')
+        except:
+            pass
+
+        if x is None:
+            x = self.nx//2*self.xDelt
+        if y is None:
+            y = self.ny//2*self.yDelt
+
+        self.xpix = round((x-self.xDelt/2)/self.xDelt)
+        self.x = self.xpix*self.xDelt+self.xDelt/2
+        self.ypix = round((y-self.yDelt/2)/self.yDelt)
+        self.y = self.ypix*self.yDelt+self.yDelt/2
+
+        self.lambdameter(**kw)
+        
+        # figure setting
+        self.fig = plt.figure(figsize=[18,7])
+        gs = gridspec.GridSpec(1, 5)
+        self.axI = self.fig.add_subplot(gs[0,0])
+        self.axV = self.fig.add_subplot(gs[0,1], sharex=self.axI, sharey=self.axI)
+        self.axSpec = self.fig.add_subplot(gs[0,2:])
+        self.axI.set_xlabel('X (arcsec)')
+        self.axI.set_ylabel('Y (arcsec)')
+        self.axSpec.set_xlabel(r'Wavelength ($\AA$)')
+        self.axSpec.set_ylabel('Intensity (Count)')
+        self.axI.set_title("Intensity")
+        self.axV.set_title("Velocity (km/s)")
+        self.axSpec.set_title(r"X = %.2f'', Y = %.2f'' (X$_{pix}$ = %i, Y$_{pix}$ = %i), $\Delta\lambda$ = %.2f"%(self.x, self.y, self.xpix, self.ypix, self.hw))
+        self.axI.set_xlim(self.extentRaster[0], self.extentRaster[1])
+        self.axI.set_ylim(self.extentRaster[2], self.extentRaster[3])
+        self.axSpec.set_xlim(self.wave.min(), self.wave.max())
+        self.axSpec.set_ylim(self.data[self.ypix, self.xpix].min()-100,
+                                self.data[self.ypix, self.xpix].max()+100)
+        self.axSpec.minorticks_on()
+        self.axSpec.tick_params(which='both', direction='in')
+
+        # Draw
+        self.imI = self.axI.imshow(self.lic, self.cmap, origin='lower', extent=self.extentRaster)
+        tmp = self.lic.copy().flatten()
+        tmp.sort()
+        m = tmp[200:-200].mean()
+        std = tmp[200:-200].std()
+        Imin = m-std*3
+        Imax = m+std*3
+        # Imin = tmp[200:-200].min()
+        # Imax = tmp[200:-200].max()
+        self.imI.set_clim(Imin, Imax)
+        self.imV = self.axV.imshow(self.lv, plt.cm.RdBu_r, origin='lower', extent=self.extentRaster, clim=[-10, 10])
+        self.pSpec = self.axSpec.plot(self.wave, self.data[self.ypix, self.xpix], color='k')[0]
+        self.pHL = self.axSpec.plot([self.lwc[self.ypix, self.xpix]-self.hw, self.lwc[self.ypix, self.xpix]+self.hw],
+                                    [self.lic[self.ypix, self.xpix], self.lic[self.ypix, self.xpix]], color='r')[0]
+        self.pVL = self.axSpec.plot([self.lwc[self.ypix, self.xpix], self.lwc[self.ypix, self.xpix]],
+                                    [1e4, 0], color='r')[0]
+        self.pointI = self.axI.scatter(self.x, self.y, 50, marker='x', color='r')
+        self.pointV = self.axV.scatter(self.x, self.y, 50, marker='x', color='r')
+
+        self.fig.tight_layout()
+        self.fig.canvas.mpl_connect('key_press_event', self._onKey_vs)
+        self.fig.show()
+
+    def _onKey_vs(self, event):
+        if event.key == 'left' or event.key == 'ctrl+left' or event.key == 'cmd+left':
+            if self.xpix > 0:
+                self.xpix -= 1
+            else:
+                self.xpix = self.nx-1
+            self.x = self.xpix*self.xDelt+self.xDelt/2
+            self._chPos()
+        elif event.key == 'right' or event.key == 'ctrl+right' or event.key == 'cmd+right':
+            if self.xpix < self.nx-1:
+                self.xpix += 1
+            else:
+                self.xpix = 0
+            self.x = self.xpix*self.xDelt+self.xDelt/2
+            self._chPos()
+        elif event.key == 'down' or event.key == 'ctrl+down' or event.key == 'cmd+down':
+            if self.ypix > 0:
+                self.ypix -= 1
+            else:
+                self.ypix = self.ny-1
+            self.y = self.ypix*self.yDelt+self.yDelt/2
+            self._chPos()
+        elif event.key == 'up' or event.key == 'ctrl+up' or event.key == 'cmd+up':
+            if self.ypix < self.ny-1:
+                self.ypix += 1
+            else:
+                self.ypix = 0
+            self.y = self.ypix*self.yDelt+self.yDelt/2
+            self._chPos()
+        elif event.key == ' ' and (event.inaxes == self.axI or event.inaxes == self.axV):
+            self.x = event.xdata
+            self.y = event.ydata
+            self.xpix = int(round((self.x-self.xDelt/2)/self.xDelt))
+            self.ypix = int(round((self.y-self.yDelt/2)/self.yDelt))
+            self._chPos()
+
+    def _chPos(self):
+        self.pSpec.set_ydata(self.data[self.ypix, self.xpix])
+        self.pHL.set_xdata([self.lwc[self.ypix, self.xpix]-self.hw, self.lwc[self.ypix, self.xpix]+self.hw])
+        self.pHL.set_ydata([self.lic[self.ypix, self.xpix], self.lic[self.ypix, self.xpix]])
+        self.pVL.set_xdata([self.lwc[self.ypix, self.xpix], self.lwc[self.ypix, self.xpix]])
+        self.pointI.set_offsets([self.x, self.y])
+        self.pointV.set_offsets([self.x, self.y])
+        self.axSpec.set_ylim(self.data[self.ypix, self.xpix].min()-100,
+                                self.data[self.ypix, self.xpix].max()+100)
+        self.fig.canvas.draw_idle()
+    
+    def chIclim(self, cmin, cmax):
+        self.imI.set_clim(cmin, cmax)
+        self.fig.canvas.draw_idle()
+    
+    def chVclim(self, cmin, cmax):
+        self.imV.set_clim(cmin, cmax)
+        self.fig.canvas.draw_idle()
+
+class FD:
+    """
+    Read the FISS Data (FD) file.
+
+    Parameters
+    ----------
+    fdFile: `str`
+        File name of the FISS Data file.
+    maskFile: `str`
+        File name of the mask file.
+    timeFile: `str`
+        File name of the time file.
+    maskValue: `float`
+        Value of the mask pixel.
+    spatialAvg: `bool`
+        Subtract the spatially averaged value to all pixels.
+    timeAvg: `bool`
+        Subtract the temporal averaged value to all pixels.
+    """
+    def __init__(self, fdFile, maskFile, timeFile, maskValue=-1,
+                 spatialAvg=False, timeAvg=False):
+        self.maskValue = maskValue
+        self._spAvg = spatialAvg
+        self._timeAvg = timeAvg
+        self.ftype = 'FD'
+        self.data = fits.getdata(fdFile).astype(float)
+        self.fdFile = fdFile
+        self.header = fits.getheader(fdFile)
+        self.time = fits.getdata(timeFile)
+        self.reftpix = np.abs(self.time-0).argmin()
+        self.xDelt = self.yDelt = 0.16
+        self.min0 = np.min(self.data, axis=(1,2))
+        self.max0 = np.max(self.data, axis=(1,2))
+        unit = fits.getheader(timeFile)['unit']
+        if unit == 'min':
+            self.time *= 60
+
+        self.mask = fits.getdata(maskFile).astype(bool)
+        self.dt = np.median(self.time-np.roll(self.time, 1))
+        self.nt, self.ny, self.nx, self.nid = self.data.shape
+
+        reftime = self.header['reftime']
+        self.reftime = _isoRefTime(reftime)
+        self.Time = self.reftime + self.time * u.second
+        self.timei = self.time-self.time[0]
+        self.header['sttime'] = self.Time[0].value
+        wid = self.header['ID1'][:2]
+        if wid == 'HI':
+            self.cmap = [cm.ha]*self.nid
+
+        elif wid == 'Ca':
+            self.cmap = [cm.ca]*self.nid
+        elif wid == 'Na':
+            self.cmap = [cm.na]*self.nid
+        elif wid == 'Fe':
+            self.cmap = [cm.fe]*self.nid
+
+        try:
+            xpos = self.header['xpos']
+            ypos = self.header['ypos']
+        except:
+            xpos = self.header.get('crval1', 0)
+            ypos = self.header.get('crval2', 0)
+        self.xpos = xpos
+        self.ypos = ypos
+        xm = xpos - self.nx/2*self.xDelt
+        xM = xpos + self.nx/2*self.xDelt
+        ym = ypos - self.ny/2*self.yDelt
+        yM = ypos + self.ny/2*self.yDelt
+        self.extent = [xm, xM, ym, yM]
+        self._xar = np.linspace(xm+self.xDelt/2,
+                                xM-self.xDelt/2, self.nx)
+        self._yar = np.linspace(ym+self.yDelt/2,
+                                yM-self.yDelt/2, self.ny)
+        if maskValue != -1:
+            self._mask(maskValue)
+        if spatialAvg:
+            self.spatialAverage()
+        if timeAvg:
+            self.timeAverage()
+        self.min = self.min0[self.reftpix]
+        self.max = self.max0[self.reftpix]
+        self.idh = self.header['ID*']
+        for i in range(self.nid):
+            if self.idh[i][-1] == 'V':
+                self.cmap[i] = plt.cm.RdBu_r
+                tmp = np.abs(self.max[i]-self.min[i])/2*0.7
+                if tmp > 15:
+                    tmp = 0.8
+                self.min[i] = -tmp
+                self.max[i] = tmp
+
+    def _mask(self, val):
+        self.data[np.invert(self.mask),:] = val
+
+    def spatialAverage(self):
+        for i in range(self.nt):
+            med = np.median(self.data[i,self.mask[i]], 0)
+            self.data[i] -= med
+            self.min0[i] -= med
+            self.max0[i] -= med
+
+    def timeAverage(self):
+        med = np.median(self.data, 0)
+        self.data -= med
+        self.min0 -= np.median(med, (0,1))
+        self.max0 -= np.median(med, (0,1))
+
+    def originalData(self, maskValue=-1, spatialAvg=False, timeAvg=False):
+        self.data = fits.getdata(self.fdFile).astype(float)
+        self.min0 = np.min(self.data, axis=(1,2))
+        self.max0 = np.max(self.data, axis=(1,2))
+        if maskValue != -1:
+            self.maskValue = maskValue
+            self._mask(maskValue)
+        if spatialAvg:
+            self.spatialAverage()
+        if timeAvg:
+            self.timeAverage()
+
+        self.min = self.min0[self.reftpix]
+        self.max = self.max0[self.reftpix]
+        for i in range(self.nid):
+            if self.idh[i][-1] == 'V':
+                self.cmap[i] = plt.cm.RdBu_r
+                tmp = np.abs(self.max[i]-self.min[i])/2*0.7
+                if tmp > 15:
+                    tmp = 0.8
+                self.min[i] = -tmp
+                self.max[i] = tmp
+
+    def bandpassFilter(self, filterRange):
+        for n, i in enumerate(filterRange):
+            filterRange[n] = i*1e-3
+        self.data = FourierFilter(self.data, self.nt, self.dt, filterRange)
+        if self.maskValue != -1:
+            self._mask(self.maskValue)
+        self.min0 = np.min(self.data, axis=(1,2))
+        self.max0 = np.max(self.data, axis=(1,2))
+        self.min = self.min0[self.reftpix]
+        self.max = self.max0[self.reftpix]
+        for i in range(self.nid):
+            if self.idh[i][-1] == 'V':
+                self.cmap[i] = plt.cm.RdBu_r
+                tmp = np.abs(self.max[i]-self.min[i])/2*0.7
+                if tmp > 15:
+                    tmp = 0.8
+                self.min[i] = -tmp
+                self.max[i] = tmp
+
+    def imshow(self, x=0, y=0, t=0, cid=0,
+               levels=None, maxPeriod=32, helpBox=True, **kwargs):
+
+        self.kwargs = kwargs
+        try:
+            plt.rcParams['keymap.back'].remove('left')
+            plt.rcParams['keymap.forward'].remove('right')
+        except:
+            pass
+
+
+        # transpose to pixel position.
+        xpix, ypix, tpix = self._pixelPosition(x, y, t)
+        self._x0 = self.x
+        self._y0 = self.y
+        self._t0 = self.t
+        self._xh = self.x
+        self._yh = self.y
+        self._th = self.t
+        self.cid = cid
+        self._cidh = cid
+        self.maxPeriod = maxPeriod
+
+
+        #Keyboard helpBox
+        if helpBox:
+            helpFig = plt.figure('Key Help Box', figsize=[3.5, 3])
+            ax = helpFig.add_subplot(111)
+            ax.set_position([0,0,1,1])
+            ax.set_axis_off()
+            ax.text(0.05, 0.91, 'ctrl+h: Reset to original setting')
+            ax.text(0.05, 0.81, 'ctrl+num: Draw the plot ID = num')
+            ax.text(0.05, 0.71, 'ctrl+right: Move to right')
+            ax.text(0.05, 0.61, 'ctrl+left: Move to left')
+            ax.text(0.05, 0.51, 'ctrl+up: Move to up')
+            ax.text(0.05, 0.41, 'ctrl+down: Move to down')
+            ax.text(0.05, 0.31, 'right: Next time data')
+            ax.text(0.05, 0.21, 'right: Previous time data')
+            ax.text(0.05, 0.11, 'spacebar: change to current mouse point')
+            ax.text(0.05, 0.01, 'ctrl+b: back to the previous image')
+
+
+        # Figure setting
+        figsize = kwargs.pop('figsize', [10, 8])
+        self.fig = plt.figure(figsize=figsize)
+        self.fig.canvas.set_window_title('FISS Data')
+        self.imInterp = kwargs.get('interpolation', 'bilinear')
+        gs = gridspec.GridSpec(5,5)
+
+        self.axRaster = self.fig.add_subplot(gs[0:3, :2]) # Raster
+        self.axRaster.set_xlabel('X (arcsec)')
+        self.axRaster.set_ylabel('Y (arcsec)')
+        self.axRaster.set_title(self.idh[0])
+
+        self.axTS = self.fig.add_subplot(gs[1:3, 2:]) # TimeSeries
+        self.axTS.set_xlabel('Time (sec)')
+        self.axTS.set_ylabel('Intensity (count)')
+        self.axTS.set_xlim(self.timei[0], self.timei[-1])
+        self.axTS.minorticks_on()
+        self.axTS.tick_params(which='both', direction='in')
+        self.axTS.set_title('Time series')
+
+        self.axWavelet = self.fig.add_subplot(gs[3:, 2:])
+        self.axWavelet.set_title('Wavelet Power Spectrum')
+        self.axWavelet.set_xlabel('Time (sec)')
+        self.axWavelet.set_ylabel('Period (minute)')
+        self.axWavelet.set_xlim(self.timei[0], self.timei[-1])
+        self.axWavelet.set_yscale('symlog', basey=2)
+        self.axWavelet.yaxis.set_major_formatter(ticker.ScalarFormatter())
+        self.axWavelet.ticklabel_format(axis='y',style='plain')
+        self.axWavelet.set_ylim(self.maxPeriod, 0.5)
+
+        self.axPower = self.fig.add_subplot(gs[3:, :2])
+        self.axPower.set_title('Power Spectrum')
+
+        self.axPower.set_ylabel('Period (minute)')
+        self.axPower.set_ylim(self.maxPeriod, 0.5)
+        self.axPower.set_yscale('symlog', basey=2)
+        self.axPower.yaxis.set_major_formatter(ticker.ScalarFormatter())
+        self.axPower.ticklabel_format(axis='x',style='sci', scilimits=(0,1))
+        self.axPower.minorticks_on()
+        self.axPower.tick_params(which='both', direction='in')
+
+        # Plot
+        data = self.data[:, ypix, xpix, self.cid]
+        self.imRaster = self.axRaster.imshow(self.data[tpix,:,:,cid],
+                                             self.cmap[cid],
+                                             origin='lower',
+                                             extent=self.extent,
+                                             clim=[self.min[cid],
+                                                   self.max[cid]],
+                                             interpolation=self.imInterp)
+        self.timeseries = self.axTS.plot(self.timei,
+                                         data,
+                                         color='k')[0]
+
+        #wavelet
+        if not levels:
+            levels = [0.1, 0.25, 0.4,
+                      0.55, 0.7, 1]
+        self.levels = levels
+        self._plotWavelet(xpix, ypix)
+#        divider = make_axes_locatable(self.axWavelet)
+#        cax = divider.append_axes('right', size='5%', pad=0.1)
+#        plt.colorbar(self.contourIm, cax=cax)
+
+        #gws
+        self.powerGWS = self.axPower.plot(self.gws, self.period, color='k',
+                                          label='GWS')[0]
+        #lws
+        self.lws = self.wavelet.power[:, tpix]
+        self.powerLWS = self.axPower.plot(self.lws, self.period,
+                                          color='r', label='LWS')[0]
+        self.axPower.legend()
+
+        # marker
+        self.point = self.axRaster.scatter(self.x, self.y, 50,
+                                           marker='x',
+                                           color='r')
+        self.vlineTS = self.axTS.axvline(self.t,
+                                         ls='dashed',
+                                         color='b')
+        self.vlineWavelet = self.axWavelet.axvline(self.t,
+                                                   ls='dashed',
+                                                   color='k')
+        peakPGWS = self.period[self.gws.argmax()]
+        peakPLWS = self.period[self.lws.argmax()]
+        self.hlineGWS = self.axPower.axhline(peakPGWS,
+                                             ls='dotted',
+                                             color='k')
+        self.hlineLWS = self.axPower.axhline(peakPLWS,
+                                             ls='dotted',
+                                             color='r')
+
+        #infoBox
+        self.axInfo = self.fig.add_subplot(gs[0, 2:])
+        self.axInfo.set_axis_off()
+        self.isotInfo = self.axInfo.text(0.05, 0.8,
+                                    '%s'%self.Time[self.tpix].value,
+                                    fontsize=12)
+        self.tInfo = self.axInfo.text(0.05, 0.55,
+                                 't=%i sec (tpix=%i)'%(self.t, self.tpix),
+                                 fontsize=12)
+        self.posiInfo = self.axInfo.text(0.05, 0.3,
+                        "X=%.1f'', Y=%.1f'' (xpix=%i, ypix=%i)"%(self.x,
+                                                                 self.y,
+                                                                 xpix,
+                                                                 ypix),
+                                            fontsize=12)
+        self.peakPeriodGWS = self.axInfo.text(0.05, -0.1,
+                                         r'P$_{peak, GWS}$=%.2f min'%peakPGWS,
+                                         fontsize=12)
+        self.peakPeriodLWS = self.axInfo.text(0.05, -0.35,
+                                         r'P$_{peak, LWS}$=%.2f min'%peakPLWS,
+                                         fontsize=12)
+
+        #Axis limit
+        self.axTS.set_ylim(data.min(), data.max())
+        self.axPower.set_xlim(0, self.lpmax)
+        self.axWavelet.set_aspect(adjustable='box', aspect='auto')
+        self.fig.tight_layout()
+        self.fig.canvas.mpl_connect('key_press_event', self._on_key)
+
+        plt.show()
+
+    def _on_key(self, event):
+        if event.key == 'ctrl+right':
+            if self.x < self._xar[-1]:
+                self.x += self.xDelt
+            else:
+                self.x = self._xar[0]
+            self._xb = self._x0
+            self._yb = self._y0
+            self._tb = self._t0
+        elif event.key == 'ctrl+left':
+            if self.x > self._xar[0]:
+                self.x -= self.xDelt
+            else:
+                self.x = self._xar[-1]
+            self._xb = self._x0
+            self._yb = self._y0
+            self._tb = self._t0
+        elif event.key == 'ctrl+up':
+            if self.y < self._yar[-1]:
+                self.y += self.yDelt
+            else:
+                self.y = self._yar[0]
+            self._xb = self._x0
+            self._yb = self._y0
+            self._tb = self._t0
+        elif event.key == 'ctrl+down':
+            if self.y > self._yar[0]:
+                self.y -= self.yDelt
+            else:
+                self.y = self._yar[-1]
+            self._xb = self._x0
+            self._yb = self._y0
+            self._tb = self._t0
+        elif event.key == 'right':
+            if self.tpix < self.nt-1:
+                self.tpix += 1
+            else:
+                self.tpix = 0
+            self.t = self.timei[self.tpix]
+            self._xb = self._x0
+            self._yb = self._y0
+            self._tb = self._t0
+        elif event.key == 'left':
+            if self.tpix > 0:
+                self.tpix -= 1
+            else:
+                self.tpix = self.nt-1
+            self.t = self.timei[self.tpix]
+            self._xb = self._x0
+            self._yb = self._y0
+            self._tb = self._t0
+        elif event.key == ' ' and event.inaxes == self.axRaster:
+            self._xb = self._x0
+            self._yb = self._y0
+            self._tb = self._t0
+            self.x = event.xdata
+            self.y = event.ydata
+        elif event.key == ' ' and (event.inaxes == self.axTS or
+                                   event.inaxes == self.axWavelet):
+            self.t = event.xdata
+            self._xb = self._x0
+            self._yb = self._y0
+            self._tb = self._t0
+            self.tpix = np.abs(self.timei-self.t).argmin()
+            self.t = self.timei[self.tpix]
+        elif event.key == 'ctrl+b':
+            x = self.x
+            y = self.y
+            t = self.t
+            self.x = self._xb
+            self.y = self._yb
+            self.t = self._tb
+            self._xb = x
+            self._yb = y
+            self._tb = t
+            self.tpix = np.abs(self.timei-self.t).argmin()
+        elif event.key == 'ctrl+h':
+            self.x = self._xh
+            self.y = self._yh
+            self.t = self._th
+            self.tpix = np.abs(self.timei-self.t).argmin()
+            self.cid = self._cidh
+            self._changeID()
+            self.axRaster.set_title(self.idh[self.cid])
+            self.imRaster.set_cmap(self.cmap[self.cid])
+        for iid in range(self.nid):
+            if event.key == 'ctrl+%i'%iid:
+                self.cid = iid
+                self._changeID()
+                self.axRaster.set_title(self.idh[iid])
+                self.imRaster.set_cmap(self.cmap[self.cid])
+                if self.idh[iid][-1] == 'V':
+                    self.axTS.set_ylabel('Velocity (km/s)')
+                else:
+                    self.axTS.set_ylabel('Intensity (Count)')
+
+        if self.x != self._x0 or self.y != self._y0:
+            xpix, ypix, tpix = self._pixelPosition(self.x, self.y,
+                                                   self.t)
+            self._changeWavelet(xpix, ypix)
+            self._changePlot(xpix, ypix)
+            self._x0 = self.x
+            self._y0 = self.y
+            self.posiInfo.set_text(
+                    "X=%.1f'', Y=%.1f'' (xpix=%i, ypix=%i)"%(self.x,
+                                                             self.y,
+                                                             xpix,
+                                                             ypix))
+        if self.t != self._t0:
+            self._changeRaster()
+            self.lws = self.wavelet.power[:, self.tpix]
+            self.powerLWS.set_xdata(self.lws)
+            self.vlineTS.set_xdata(self.t)
+            self.vlineWavelet.set_xdata(self.t)
+            peakPLWS = self.period[self.lws.argmax()]
+            self.hlineLWS.set_ydata(peakPLWS)
+            self._t0 = self.t
+            self.isotInfo.set_text('%s'%self.Time[self.tpix].value)
+            self.tInfo.set_text('t=%i sec (tpix=%i)'%(self.t, self.tpix))
+            self.peakPeriodLWS.set_text(
+                    r'P$_{peak, LWS}$=%.2f min'%peakPLWS)
+        self.fig.canvas.draw_idle()
+
+    def _changeID(self):
+        xpix, ypix, tpix = self._pixelPosition(self.x, self.y,
+                                                   self.t)
+        self._changeWavelet(xpix, ypix)
+        self._changePlot(xpix, ypix)
+        self._changeRaster()
+        self.imRaster.set_clim(self.min[self.cid],
+                               self.max[self.cid])
+
+    def _changePlot(self, xpix, ypix):
+        data = self.data[:, ypix, xpix, self.cid]
+        self.timeseries.set_ydata(data)
+        self.axTS.set_ylim(data.min(), data.max())
+        self.powerGWS.set_xdata(self.gws)
+        self.lws = self.wavelet.power[:, self.tpix]
+        self.powerLWS.set_xdata(self.lws)
+        self.point.set_offsets([self.x, self.y])
+        peakPGWS = self.period[self.gws.argmax()]
+        peakPLWS = self.period[self.lws.argmax()]
+        self.hlineGWS.set_ydata(peakPGWS)
+        self.hlineLWS.set_ydata(peakPLWS)
+        self.peakPeriodGWS.set_text(
+                    r'P$_{peak, GWS}$=%.2f min'%peakPGWS)
+        self.peakPeriodLWS.set_text(
+                    r'$P_{peak, LWS}$=%.2f min'%peakPLWS)
+        self.axPower.set_xlim(0, self.lpmax)
+
+    def _changeRaster(self):
+        self.imRaster.set_data(self.data[self.tpix, :, :, self.cid])
+
+    def _pixelPosition(self, x, y, t):
+        tpix = np.abs(self.timei-t).argmin()
+        xpix = np.abs(self._xar-x).argmin()
+        ypix = np.abs(self._yar-y).argmin()
+        self.x = self._xar[xpix]
+        self.y = self._yar[ypix]
+        self.t = self.timei[tpix]
+        self.tpix = tpix
+        return xpix, ypix, tpix
+
+    def _changeWavelet(self, xpix, ypix):
+        self.axWavelet.cla()
+        self._plotWavelet(xpix, ypix)
+
+    def _plotWavelet(self, xpix, ypix):
+        self.wavelet = Wavelet(self.data[:, ypix, xpix, self.cid],
+                       self.dt, **self.kwargs)
+        self.lpmax = self.wavelet.power.max()
+        self.period = self.wavelet.period/60
+        self.gws = self.wavelet.gws
+        wpower = self.wavelet.power/self.wavelet.power.max()
+        self.contour = self.axWavelet.contourf(self.timei, self.period,
+                                               wpower, len(self.levels),
+                                               colors=['w'])
+        self.contourIm = self.axWavelet.contourf(self.contour,
+                                                 levels=self.levels
+                                                 )
+        self.axWavelet.fill_between(self.timei, self.wavelet.coi/60,
+                                    self.period.max(), color='grey',
+                                    alpha=0.4, hatch='x')
+        self.axWavelet.set_title('Wavelet Power Spectrum')
+        self.axWavelet.set_xlabel('Time (sec)')
+        self.axWavelet.set_ylabel('Period (minute)')
+        self.axWavelet.set_xlim(self.timei[0], self.timei[-1])
+        self.axWavelet.set_yscale('symlog', basey=2)
+        self.axWavelet.yaxis.set_major_formatter(ticker.ScalarFormatter())
+        self.axWavelet.ticklabel_format(axis='y',style='plain')
+        self.vlineWavelet = self.axWavelet.axvline(self.t,
+                                                   ls='dashed',
+                                                   color='k')
+        self.axWavelet.set_ylim(self.maxPeriod, 0.5)
+
+    def chLevels(self, levels):
+        """
+        """
+        self.levels = levels
+        xpix, ypix, tpix = self._pixelPosition(self.x, self.y, self.t)
+        self._changeWavelet(xpix, ypix)
+
+    def chInterp(self, interp):
+        """
+        """
+        self.imInterp = interp
+        self.imRaster.set_interpolation(interp)
+
+    def chBPFilter(self, filterRange):
+        """
+        """
+        self.originalData(maskValue=self.maskValue, spatialAvg=self._spAvg,
+                          timeAvg=self._timeAvg)
+        self.bandpassFilter(filterRange)
+
+    def chRasterClim(self, cmin, cmax):
+        """
+        """
+        self.imRaster.set_clim(cmin, cmax)
+
+    def chPosition(self, x, y):
+        """
+        """
+        self.x = x
+        self.y = y
+        self._x0 = x
+        self._y0 =y
+        xpix, ypix, tpix = self._pixelPosition(x, y, self.t)
+        self._changeWavelet(xpix, ypix)
+        self._changePlot(xpix, ypix)
+        self.posiInfo.set_text(
+                    "X=%.1f'', Y=%.1f'' (xpix=%i, ypix=%i)"%(self.x,
+                                                             self.y,
+                                                             xpix,
+                                                             ypix))
+
+    def chtime(self, t):
+        """
+        """
+        self.t = t
+        self._t0 = t
+        self._changeRaster()
+        self.lws = self.wavelet.power[:, self.tpix]
+        self.LWS.set_xdata(self.lws)
+        self.vlineTS.set_xdata(self.t)
+        self.vlineWavelet.set_xdata(self.t)
+        peakPLWS = self.period[self.lws.argmax()]
+        self.hlineLWS.set_ydata(peakPLWS)
+        self._t0 = self.t
+        self.isotInfo.set_text('%s'%self.Time[self.tpix].value)
+        self.tInfo.set_text('t=%i sec (tpix=%i)'%(self.t, self.tpix))
+        self.peakPeriodLWS.set_text(
+                r'P$_{peak, LWS}$=%.2f min'%peakPLWS)
+
+    # def TD(self, ID=0, filterRange=None):
+    #     hdu = fits.PrimaryHDU(self.data[:,:,:,ID])
+    #     h= hdu.header
+    #     h['cdelt1'] = self.xDelt
+    #     h['cdelt2'] = self.yDelt
+    #     h['cdelt3'] = self.dt
+    #     h['crval1'] = self.xpos
+    #     h['crval2'] = self.ypos
+    #     h['sttime'] = self.Time[0].value
+
+    #     return TDmap(self.data[:,:,:,ID], h, self.time,
+    #                  filterRange=filterRange, cmap=self.cmap[ID])
+
+    def set_clim(self, cmin, cmax):
+        self.imRaster.set_clim(cmin, cmax)
+
+class calibData:
+    """
+    Read the calibration file such as 'BiasDark', 'Flat', 'FLAT' and 'SLIT'.
+
+    Parameters
+    ----------
+    file : str
+
+    """
+
+    def __init__(self, file):
+
+        if file.find('BiasDark') != -1:
+            self.ftype = 'BiasDark'
+        elif file.find('Flat') != -1:
+            self.ftype = 'Flat'
+        elif file.find('FLAT') != -1:
+            self.ftype = 'FLAT'
+        elif file.find('SLIT') != -1:
+            self.ftype = 'SLIT'
+
+        self.data = fits.getdata(file)
+        self.header = fits.getheader(file)
+
+        self.nx = self.header['naxis1']
+        self.ny = self.header['naxis2']
+        if self.ftype == 'Flat':
+            self.nf = self.header['naxis3']
+
+        if file.find('_A') != -1:
+            self.cam = 'A'
+        elif file.find('_B') != -1:
+            self.cam = 'B'
+
+    def imshow(self):
+        """
+        """
+        try:
+            plt.rcParams['keymap.back'].remove('left')
+            plt.rcParams['keymap.forward'].remove('right')
+        except:
+            pass
+
+        self.fig, self.ax = plt.subplots(figsize=[10, 6])
+        if self.ftype != 'Flat':
+            self.image = self.ax.imshow(self.data, origin='lower',
+                                        cmap = plt.cm.gray)
+            self.fig.tight_layout()
+        else:
+            self.num = 0
+            self.num0 = self.num
+            self.image = self.ax.imshow(self.data[self.num], origin='lower',
+                                        cmap = plt.cm.gray)
+            self.fig.tight_layout()
+            self.fig.canvas.mpl_connect('key_press_event', self._onKey)
+
+    def _onKey(self, event):
+        if event.key == 'right':
+            if self.num < self.nf-1:
+                self.num += 1
+            else:
+                self.num = 0
+        elif event.key == 'left':
+            if self.num > 0:
+                self.num -= 1
+            else:
+                self.num = self.nf-1
+        if self.num != self.num0:
+            self.image.set_data(self.data[self.num])
+            self.num0 = self.num
+        self.fig.canvas.draw_idle()
+
+class AlignCube:
+    """
+    Show align cube and make Time-Distance map.
+
+    Parameters
+    ----------
+    fname: `str`
+        File name of the align data cube.
+
+    Other Parameters
+    ----------------
+    **kwargs: `.makeTDmap` properties (optional)
+        Keyword arguments 
+    Returns
+    -------
+    """
+    def __init__(self, fname, **kwargs):
+        res = np.load(fname)
+        self.data = res['data']
+        self.time = res['time']
+        self.dt = res['dt']
+        self.dx = res['dx']
+        self.dy = res['dy']
+
+        self.td = makeTDmap(self.data, dx=self.dx, dy=self.dy, dt=self.dt, **kwargs)
+
+def _isoRefTime(refTime):
+    year = refTime[:4]
+    month = refTime[4:6]
+    day = refTime[6:8]
+    hour = refTime[9:11]
+    minute = refTime[11:13]
+    sec = refTime[13:15]
+    isot = '%s-%s-%sT%s:%s:%s'%(year, month, day, hour, minute, sec)
+    return Time(isot)
```

### Comparing `fisspy-0.9.80/fisspy/read/readbase.py` & `fisspy-1.0.0/fisspy/read/readbase.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,198 +1,229 @@
-"""
-"""
-
-from __future__ import absolute_import, division
-import numpy as np
-from astropy.io import fits
-from os.path import join, dirname
-
-
-__author__= "Juhyung Kang"
-__email__ = "jhkang@astro.snu.ac.kr"
-__all__ = ["readFrame", "_readPCA", "getHeader", "getRaster"]
-
-def readFrame(file, pfile=False, x1=0, x2=None, y1=0, y2=None, ncoeff=False):
-    """
-    Read the FISS fts file.
-
-    Parameters
-    ----------
-    file : `str`
-        File name of the FISS fts data.
-    pfile : `str`
-        File name of the _p.fts file of the compressed data
-    x1 : `int`, optional
-        A left limit index of the frame along the scan direction
-    x2 : `int`, optional
-        A right limit index of the frame along the scan direction
-        If None, read all data from x1 to the end of the scan direction.
-    y1 : `int`, optional
-        A left limit index of the frame along the scan direction
-    y2 : `int`, optional
-        A right limit index of the frame along the scan direction
-        If None, read all data from x1 to the end of the scan direction.
-    noceff : `int`, optional
-        he number of coefficients to be used for
-        the construction of frame in a pca file.
-    """
-    if not x2 is None:
-        if x2 > 0 and x2 <= x1:
-            raise ValueError('x2 must be larger than x1')
-    if not y2 is None:
-        if y2 > 0 and y2 <= y1:
-            raise ValueError('y2 must be larger than y1')
-
-
-    if pfile:
-        spec = _readPCA(file, pfile, x1=x1, x2=x2, y1=y1, y2=y2, ncoeff=ncoeff)
-    else:
-        if x2 is None:
-            spec = fits.getdata(file)[x1:]
-        else:
-            spec = fits.getdata(file)[x1:x2]
-        if y2 is None:
-            spec = spec[:, y1:]
-        else:
-            spec = spec[:, y1:y2]
-
-    spec = spec.transpose((1,0,2)).astype(float)
-
-    return spec
-
-
-def _readPCA(file, pfile, x1=0, x2=None, y1=0, y2=None, ncoeff=False):
-    """
-    Read the PCA compressed FISS fts file.
-
-    Parameters
-    ----------
-    file : `str`
-        File name of the FISS fts data.
-    pfile : `str`
-        File name of the _p.fts file of the compressed data
-    x1 : `int`, optional
-        A left limit index of the frame along the scan direction
-    x2 : `int`, optional
-        A right limit index of the frame along the scan direction
-        If None, read all data from x1 to the end of the scan direction.
-    y1 : `int`, optional
-        A left limit index of the frame along the scan direction
-    y2 : `int`, optional
-        A right limit index of the frame along the scan direction
-        If None, read all data from x1 to the end of the scan direction.
-    noceff : `int`, optional
-        he number of coefficients to be used for
-        the construction of frame in a pca file.
-    """
-
-    pdata = fits.getdata(join(dirname(file), pfile))
-    if x2 is None:
-        data = fits.getdata(file)[x1:]
-    else:
-        data = fits.getdata(file)[x1:x2]
-    if y2 is None:
-        data = data[:, y1:]
-    else:
-        data = data[:, y1:y2]
-    ncoeff1 = data.shape[2] - 1
-    if not ncoeff:
-        ncoeff = ncoeff1
-    elif ncoeff > ncoeff1:
-        ncoeff = ncoeff1
-
-    spec = np.dot(data[:,:,0:ncoeff], pdata[0:ncoeff,:])
-    spec *= 10.**data[:,:,ncoeff][:,:,None]
-    return spec
-
-def getHeader(file):
-    """
-    Get the FISS fts file header.
-
-    Returns
-    -------
-    header : `astropy.io.fits.Header`
-        The fts file header.
-
-    Notes
-    -----
-        This function automatically check the existance of the pca file by
-        reading the fts header.
-    """
-    header0 = fits.getheader(file)
-
-    pfile = header0.pop('pfile',False)
-    if not pfile:
-        return header0
-    else:
-        header = fits.Header()
-        header['pfile']=pfile
-        for i in header0['comment']:
-            sori = i.split('=')
-            if len(sori) == 1:
-                skv = sori[0].split(None,1)
-                if len(skv) == 1:
-                    pass
-                else:
-                    header[skv[0]] = skv[1]
-            else:
-                key = sori[0]
-                svc = sori[1].split('/')
-                try:
-                    item = float(svc[0])
-                except:
-                    item = svc[0].split("'")
-                    if len(item) != 1:
-                        item = item[1].split(None,0)[0]
-                    else:
-                        item = item[0].split(None,0)[0]
-                try:
-                    if item-int(svc[0]) == 0:
-                        item = int(item)
-                except:
-                    pass
-                if len(svc) == 1:
-                    header[key] = item
-                else:
-                    header[key] = (item,svc[1])
-
-    header['simple'] = True
-    alignl=header0.pop('alignl',-1)
-
-    if alignl == 0:
-        keys=['reflect','reffr','reffi','cdelt2','cdelt3','crota2',
-              'crpix3','shift3','crpix2','shift2','margin2','margin3']
-        header['alignl'] = (alignl,'Alignment level')
-        for i in keys:
-            header[i] = (header0[i],header0.comments[i])
-        header['history'] = str(header0['history'])
-    if alignl == 1:
-        keys=['reflect','reffr','reffi','cdelt2','cdelt3','crota1',
-              'crota2','crpix3','crval3','shift3','crpix2','crval2',
-              'shift2','margin2','margin3']
-        header['alignl'] = (alignl,'Alignment level')
-        for i in keys:
-            header[i] = (header0[i],header0.comments[i])
-        header['history'] = str(header0['history'])
-
-    return header
-
-def getRaster(data, wave, wvPoint, wvDelt, hw=0.05):
-    """
-    getRaster(wv, hw)
-
-    Make a raster image for a given wavelength with in width 2*hw
-
-    Parameters
-    ----------
-    wv : float
-        Referenced wavelengths.
-    hw   : float
-        A half-width of wavelength integration in unit of Angstrom.
-        Default is 0.05
-
-    """
-    if hw < abs(wvDelt)/2.:
-        hw = abs(wvDelt)/2.
-
-    s = np.abs(wave - wvPoint) <= hw
-    return data[:,:,s].mean(2)
+"""
+"""
+
+from __future__ import absolute_import, division
+import numpy as np
+from astropy.io import fits
+from os.path import join, dirname
+
+
+__author__= "Juhyung Kang"
+__email__ = "jhkang0301@gmail.com"
+
+__all__ = ["Photolinewv", "readFrame", "_readPCA", "getHeader", "getRaster"]
+
+
+def Photolinewv(line, wvmin, wvmax):
+    """
+    To specicy the spectral line used to determine photospheric velocity 
+
+    Parameters
+    ----------
+    line : `str`
+        spectral band designation.
+    wvmin : `float`
+        minimum wavelength of the spectral band.
+    wvmax : `float`
+        maximum wavelength of the spectral band.
+
+    Returns
+    -------
+    wvp : `float`
+        laboratory wavelength of the photosperic line.
+    dwv : `float`
+        half of the wavelength range to be used 
+    """
+    if line == 'Ha':
+        wvp, dwv = 6559.580, 0.25
+    if line == 'Ca':
+        wvp,dwv = 8536.165, 0.25 
+        if (wvp > (wvmin+2*dwv))*(wvp < (wvmax-2*dwv)):
+            return wvp, dwv
+        wvp,dwv = 8548.079*(1+(-0.62)/3.e5), 0.25
+
+    return wvp, dwv
+
+def readFrame(file, pfile=False, x1=0, x2=None, y1=0, y2=None, ncoeff=False):
+    """
+    Read the FISS fts file.
+
+    Parameters
+    ----------
+    file : `str`
+        File name of the FISS fts data.
+    pfile : `str`
+        File name of the _p.fts file of the compressed data
+    x1 : `int`, optional
+        A left limit index of the frame along the scan direction
+    x2 : `int`, optional
+        A right limit index of the frame along the scan direction
+        If None, read all data from x1 to the end of the scan direction.
+    y1 : `int`, optional
+        A left limit index of the frame along the scan direction
+    y2 : `int`, optional
+        A right limit index of the frame along the scan direction
+        If None, read all data from x1 to the end of the scan direction.
+    noceff : `int`, optional
+        he number of coefficients to be used for
+        the construction of frame in a pca file.
+    """
+    if not x2 is None:
+        if x2 > 0 and x2 <= x1:
+            raise ValueError('x2 must be larger than x1')
+    if not y2 is None:
+        if y2 > 0 and y2 <= y1:
+            raise ValueError('y2 must be larger than y1')
+
+
+    if pfile:
+        spec = _readPCA(file, pfile, x1=x1, x2=x2, y1=y1, y2=y2, ncoeff=ncoeff)
+    else:
+        if x2 is None:
+            spec = fits.getdata(file)[x1:]
+        else:
+            spec = fits.getdata(file)[x1:x2]
+        if y2 is None:
+            spec = spec[:, y1:]
+        else:
+            spec = spec[:, y1:y2]
+
+    spec = spec.transpose((1,0,2)).astype(float)
+    return spec
+
+def _readPCA(file, pfile, x1=0, x2=None, y1=0, y2=None, ncoeff=False):
+    """
+    Read the PCA compressed FISS fts file.
+
+    Parameters
+    ----------
+    file : `str`
+        File name of the FISS fts data.
+    pfile : `str`
+        File name of the _p.fts file of the compressed data
+    x1 : `int`, optional
+        A left limit index of the frame along the scan direction
+    x2 : `int`, optional
+        A right limit index of the frame along the scan direction
+        If None, read all data from x1 to the end of the scan direction.
+    y1 : `int`, optional
+        A left limit index of the frame along the scan direction
+    y2 : `int`, optional
+        A right limit index of the frame along the scan direction
+        If None, read all data from x1 to the end of the scan direction.
+    noceff : `int`, optional
+        he number of coefficients to be used for
+        the construction of frame in a pca file.
+    """
+
+    pdata = fits.getdata(join(dirname(file), pfile))
+    if x2 is None:
+        data = fits.getdata(file)[x1:]
+    else:
+        data = fits.getdata(file)[x1:x2]
+    if y2 is None:
+        data = data[:, y1:]
+    else:
+        data = data[:, y1:y2]
+    ncoeff1 = data.shape[2] - 1
+    if not ncoeff:
+        ncoeff = ncoeff1
+    elif ncoeff > ncoeff1:
+        ncoeff = ncoeff1
+
+    spec = np.dot(data[:,:,:ncoeff], pdata[:ncoeff,:])
+    # spec *= 10.**data[:,:,ncoeff][:,:,None]
+    spec *= 10.**data[:,:,-1][:,:,None]
+    return spec
+
+def getHeader(file):
+    """
+    Get the FISS fts file header.
+
+    Returns
+    -------
+    header : `astropy.io.fits.Header`
+        The fts file header.
+
+    Notes
+    -----
+        This function automatically check the existance of the pca file by
+        reading the fts header.
+    """
+    header0 = fits.getheader(file)
+
+    pfile = header0.pop('pfile',False)
+    if not pfile:
+        return header0
+    else:
+        header = fits.Header()
+        header['pfile']=pfile
+        for i in header0['comment']:
+            sori = i.split('=')
+            if len(sori) == 1:
+                skv = sori[0].split(None,1)
+                if len(skv) == 1:
+                    pass
+                else:
+                    header[skv[0]] = skv[1]
+            else:
+                key = sori[0]
+                svc = sori[1].split('/')
+                try:
+                    item = float(svc[0])
+                except:
+                    item = svc[0].split("'")
+                    if len(item) != 1:
+                        item = item[1].split(None,0)[0]
+                    else:
+                        item = item[0].split(None,0)[0]
+                try:
+                    if item-int(svc[0]) == 0:
+                        item = int(item)
+                except:
+                    pass
+                if len(svc) == 1:
+                    header[key] = item
+                else:
+                    header[key] = (item,svc[1])
+
+    header['simple'] = True
+    alignl=header0.pop('alignl',-1)
+
+    if alignl == 0:
+        keys=['reflect','reffr','reffi','cdelt2','cdelt3','crota2',
+              'crpix3','shift3','crpix2','shift2','margin2','margin3']
+        header['alignl'] = (alignl,'Alignment level')
+        for i in keys:
+            header[i] = (header0[i],header0.comments[i])
+        header['history'] = str(header0['history'])
+    if alignl == 1:
+        keys=['reflect','reffr','reffi','cdelt2','cdelt3','crota1',
+              'crota2','crpix3','crval3','shift3','crpix2','crval2',
+              'shift2','margin2','margin3']
+        header['alignl'] = (alignl,'Alignment level')
+        for i in keys:
+            header[i] = (header0[i],header0.comments[i])
+        header['history'] = str(header0['history'])
+
+    return header
+
+def getRaster(data, wave, wvPoint, wvDelt, hw=0.05):
+    """
+    getRaster(wv, hw)
+
+    Make a raster image for a given wavelength with in width 2*hw
+
+    Parameters
+    ----------
+    wv : float
+        Referenced wavelengths.
+    hw   : float
+        A half-width of wavelength integration in unit of Angstrom.
+        Default is 0.05
+
+    """
+    if hw < abs(wvDelt)/2.:
+        hw = abs(wvDelt)/2.
+
+    s = np.abs(wave - wvPoint) <= hw
+    return data[:,:,s].mean(2)
```

