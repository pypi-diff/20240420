# Comparing `tmp/galapy-fit-0.5.2.tar.gz` & `tmp/galapy_fit-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galapy-fit-0.5.2.tar", last modified: Mon Feb 19 14:36:59 2024, max compression
+gzip compressed data, was "galapy_fit-0.5.3.tar", last modified: Sat Apr 20 16:21:32 2024, max compression
```

## Comparing `galapy-fit-0.5.2.tar` & `galapy_fit-0.5.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.422378 galapy-fit-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    50785 2024-02-19 14:36:59.422378 galapy-fit-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.410378 galapy-fit-0.5.2/c++/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.410378 galapy-fit-0.5.2/c++/csp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.410378 galapy-fit-0.5.2/c++/csp/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/c++/csp/src/csp.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.410378 galapy-fit-0.5.2/c++/ism/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.410378 galapy-fit-0.5.2/c++/ism/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/c++/ism/src/ism.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.410378 galapy-fit-0.5.2/c++/sfh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.414378 galapy-fit-0.5.2/c++/sfh/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/c++/sfh/src/sfh_base.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/c++/sfh/src/sfh_insitu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.414378 galapy-fit-0.5.2/galapy/
--rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/ActiveGalacticNucleus.py
--rw-r--r--   0 runner    (1001) docker     (127)    15457 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/CompositeStellarPopulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/Cosmology.py
--rw-r--r--   0 runner    (1001) docker     (127)    37590 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/Galaxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/Handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/InterGalacticMedium.py
--rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/InterStellarMedium.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/NebularFreeFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/Noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/PhotometricSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/StarFormationHistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/Synchrotron.py
--rw-r--r--   0 runner    (1001) docker     (127)    14491 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/XRayBinaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.414378 galapy-fit-0.5.2/galapy/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/analysis/funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29135 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/analysis/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.414378 galapy-fit-0.5.2/galapy/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/configuration/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/configuration/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.418378 galapy-fit-0.5.2/galapy/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/internal/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/internal/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/internal/globs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24524 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.418378 galapy-fit-0.5.2/galapy/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/io/hdf5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.418378 galapy-fit-0.5.2/galapy/sampling/
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/sampling/Observation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/sampling/Results.py
--rw-r--r--   0 runner    (1001) docker     (127)    29268 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/sampling/Run.py
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/sampling/Sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/sampling/Statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/galapy/sampling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.418378 galapy-fit-0.5.2/galapy_fit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50785 2024-02-19 14:36:59.000000 galapy-fit-0.5.2/galapy_fit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-02-19 14:36:59.000000 galapy-fit-0.5.2/galapy_fit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 14:36:59.000000 galapy-fit-0.5.2/galapy_fit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-19 14:36:59.000000 galapy-fit-0.5.2/galapy_fit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-19 14:36:59.000000 galapy-fit-0.5.2/galapy_fit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-19 14:36:59.000000 galapy-fit-0.5.2/galapy_fit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:36:59.418378 galapy-fit-0.5.2/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/pybind11/pyb11_CCSP.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/pybind11/pyb11_CISM.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/pybind11/pyb11_CNFF.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/pybind11/pyb11_CSFH.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/pybind11/pyb11_CSYN.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/pybind11/pyb11_interpolation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/pybind11/pyb11_transmission.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 14:36:59.422378 galapy-fit-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-02-19 14:36:46.000000 galapy-fit-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.038207 galapy_fit-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    50956 2024-04-20 16:21:32.038207 galapy_fit-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.026207 galapy_fit-0.5.3/c++/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.026207 galapy_fit-0.5.3/c++/csp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.026207 galapy_fit-0.5.3/c++/csp/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/c++/csp/src/csp.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.026207 galapy_fit-0.5.3/c++/ism/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.026207 galapy_fit-0.5.3/c++/ism/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/c++/ism/src/ism.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.026207 galapy_fit-0.5.3/c++/sfh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.026207 galapy_fit-0.5.3/c++/sfh/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/c++/sfh/src/sfh_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/c++/sfh/src/sfh_insitu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.030207 galapy_fit-0.5.3/galapy/
+-rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/ActiveGalacticNucleus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15457 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/CompositeStellarPopulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/Cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37590 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/Galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/Handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/InterGalacticMedium.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/InterStellarMedium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/NebularFreeFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/Noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/PhotometricSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/StarFormationHistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/Synchrotron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14491 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/XRayBinaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.030207 galapy_fit-0.5.3/galapy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/analysis/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29135 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/analysis/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.030207 galapy_fit-0.5.3/galapy/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/configuration/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/configuration/filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.034207 galapy_fit-0.5.3/galapy/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/internal/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/internal/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/internal/globs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24524 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.034207 galapy_fit-0.5.3/galapy/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/io/hdf5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.034207 galapy_fit-0.5.3/galapy/sampling/
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/sampling/Observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/sampling/Results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29268 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/sampling/Run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/sampling/Sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/sampling/Statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/galapy/sampling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.034207 galapy_fit-0.5.3/galapy_fit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50956 2024-04-20 16:21:32.000000 galapy_fit-0.5.3/galapy_fit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-20 16:21:32.000000 galapy_fit-0.5.3/galapy_fit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 16:21:32.000000 galapy_fit-0.5.3/galapy_fit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-20 16:21:32.000000 galapy_fit-0.5.3/galapy_fit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-20 16:21:32.000000 galapy_fit-0.5.3/galapy_fit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 16:21:32.000000 galapy_fit-0.5.3/galapy_fit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:21:32.034207 galapy_fit-0.5.3/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/pybind11/pyb11_CCSP.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/pybind11/pyb11_CISM.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/pybind11/pyb11_CNFF.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/pybind11/pyb11_CSFH.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/pybind11/pyb11_CSYN.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/pybind11/pyb11_interpolation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/pybind11/pyb11_transmission.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 16:21:32.038207 galapy_fit-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-20 16:21:27.000000 galapy_fit-0.5.3/setup.py
```

### Comparing `galapy-fit-0.5.2/LICENSE` & `galapy_fit-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/PKG-INFO` & `galapy_fit-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galapy-fit
-Version: 0.5.2
+Version: 0.5.3
 Summary: GalaPy - Spectral modelling tool for galaxies in Python
 Author-email: Tommaso Ronconi <tronconi@sissa.it>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,15 +690,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: emcee
 Requires-Dist: dynesty
-Requires-Dist: matplotlib
+Requires-Dist: matplotlib>=3.6
 Requires-Dist: getdist
 Requires-Dist: requests
 Requires-Dist: h5py
 Provides-Extra: dev
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: test
@@ -719,15 +719,19 @@
 .. |build-badge| image:: https://github.com/TommasoRonconi/galapy/actions/workflows/build-wheels.yml/badge.svg
    :alt: Building
 
 .. |docs-badge| image:: https://readthedocs.org/projects/galapy/badge/?version=latest
    :target: https://galapy.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
-|test-badge| |build-badge| |docs-badge|
+.. |arxiv-badge| image:: https://img.shields.io/badge/arXiv-2402.12427-b31b1b.svg
+   :target: https://arxiv.org/abs/2402.12427
+   :alt: ArXiV preprint
+
+|test-badge| |build-badge| |docs-badge| |arxiv-badge|
 	 
 GalaPy is an open source, extensible API for modelling and fitting the Spectral Energy Distribution (SED) of galaxies from the X-ray to the radio band,
 as well as the evolution of their components and dust attenuation/reradiation.
 It provides functions, classes and terminal commands for Bayesian inference of galaxy properties from panchromatic photometric data,
 as well as for the analysis and simulation of galaxies spectral properties.
 
 .. image:: https://raw.githubusercontent.com/TommasoRonconi/galapy_database/main/images/GalaPy_Example.png
```

### Comparing `galapy-fit-0.5.2/README.rst` & `galapy_fit-0.5.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 .. |build-badge| image:: https://github.com/TommasoRonconi/galapy/actions/workflows/build-wheels.yml/badge.svg
    :alt: Building
 
 .. |docs-badge| image:: https://readthedocs.org/projects/galapy/badge/?version=latest
    :target: https://galapy.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
-|test-badge| |build-badge| |docs-badge|
+.. |arxiv-badge| image:: https://img.shields.io/badge/arXiv-2402.12427-b31b1b.svg
+   :target: https://arxiv.org/abs/2402.12427
+   :alt: ArXiV preprint
+
+|test-badge| |build-badge| |docs-badge| |arxiv-badge|
 	 
 GalaPy is an open source, extensible API for modelling and fitting the Spectral Energy Distribution (SED) of galaxies from the X-ray to the radio band,
 as well as the evolution of their components and dust attenuation/reradiation.
 It provides functions, classes and terminal commands for Bayesian inference of galaxy properties from panchromatic photometric data,
 as well as for the analysis and simulation of galaxies spectral properties.
 
 .. image:: https://raw.githubusercontent.com/TommasoRonconi/galapy_database/main/images/GalaPy_Example.png
```

### Comparing `galapy-fit-0.5.2/c++/csp/src/csp.cpp` & `galapy_fit-0.5.3/c++/csp/src/csp.cpp`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/c++/ism/src/ism.cpp` & `galapy_fit-0.5.3/c++/ism/src/ism.cpp`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/c++/sfh/src/sfh_base.cpp` & `galapy_fit-0.5.3/c++/sfh/src/sfh_base.cpp`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/c++/sfh/src/sfh_insitu.cpp` & `galapy_fit-0.5.3/c++/sfh/src/sfh_insitu.cpp`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/ActiveGalacticNucleus.py` & `galapy_fit-0.5.3/galapy/ActiveGalacticNucleus.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/CompositeStellarPopulation.py` & `galapy_fit-0.5.3/galapy/CompositeStellarPopulation.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/Cosmology.py` & `galapy_fit-0.5.3/galapy/Cosmology.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/Galaxy.py` & `galapy_fit-0.5.3/galapy/Galaxy.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/Handlers.py` & `galapy_fit-0.5.3/galapy/Handlers.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/InterGalacticMedium.py` & `galapy_fit-0.5.3/galapy/InterGalacticMedium.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/InterStellarMedium.py` & `galapy_fit-0.5.3/galapy/InterStellarMedium.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/NebularFreeFree.py` & `galapy_fit-0.5.3/galapy/NebularFreeFree.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/Noise.py` & `galapy_fit-0.5.3/galapy/Noise.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/PhotometricSystem.py` & `galapy_fit-0.5.3/galapy/PhotometricSystem.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/StarFormationHistory.py` & `galapy_fit-0.5.3/galapy/StarFormationHistory.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/Synchrotron.py` & `galapy_fit-0.5.3/galapy/Synchrotron.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/XRayBinaries.py` & `galapy_fit-0.5.3/galapy/XRayBinaries.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/__init__.py` & `galapy_fit-0.5.3/galapy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 __all__ = [
     'StarFormationHistory', 'CompositeStellarPopulation', 'InterStellarMedium',
     'NebularFreeFree', 'Synchrotron', 'XRayBinaries', 'ActiveGalacticNucleus',
     'Cosmology', 'Galaxy', 'InterGalacticMedium', 'PhotometricSystem',
     'Noise', 'Handlers',
     'sampling', 'internal', 'io', 'analysis',
 ]
-__version__ = 'v0.5.2'
+__version__ = 'v0.5.3'
```

### Comparing `galapy-fit-0.5.2/galapy/analysis/funcs.py` & `galapy_fit-0.5.3/galapy/analysis/funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ######################################################################################
 # Internal imports
 
 from galapy.sampling.Results import Results
 from galapy.Handlers import ModelParameters 
 from galapy.Galaxy import gxy_params_defaults 
 from galapy.Noise import noise_params_defaults
+from galapy.internal.utils import get_credible_interval
 param_defaults = dict( **{'.'.join(['galaxy',k]):v for k,v in gxy_params_defaults.items()},
                        **{'.'.join(['noise',k]):v for k,v in noise_params_defaults.items()} )
 
 ######################################################################################
 
 def get_parameters_summary_statistics ( res, stat_type = 'quantiles', quantile = None ) :
     """ Function returning a dictionary with summary statistics of the samples in 
@@ -39,14 +40,22 @@
     : ndarray
         - if ``stat_type='bestfit_and_interval'`` each row is an array with size = 3 
           where the first element is the best-fit value, the second and third are the 
           lower and upper uncertainties, respectively.
         - if ``stat_type='quantiles'`` each row is an array with size = ``len(quantile)``
         - if ``stat_type='mean_and_std'`` each row is an array of size = 2 where the
           first element is the mean and the second element is the standard deviation.
+
+    Note
+    ----
+    When choosing stat_type='bestfit_and_interval' infinite values could appear either
+    in the lower uncertainty or in the higher untertainty. This happens when it was not possible
+    to close the requested quantile region (default = 0.68, i.e. 68 per cent) around the best-fit
+    value. In this case then, the constraint has to be interpreted as an higher or lower limit, 
+    respectively.
     """
     
     if stat_type not in ('bestfit_and_interval', 'mean_and_std', 'quantiles') :
         raise ValueError(
             "Allowed values for argument ``stat_type`` are "
             "'bestfit_and_interval', 'mean_and_std' and 'quantiles'"
         )
@@ -55,20 +64,20 @@
         if quantile is None :
             print( 'Falling back to default percentile: 0.68')
             quantile = 0.68
         try :
             quantile = float( quantile )
         except :
             raise
-        summary = numpy.empty([self.ndim,3], dtype=float)
-        idcentre = self.logl[self.wnot0].argmax()
-        for i, sample in enumerate( self.samples.T ) :
-            summary[i,0] = sample[idcentre]
+        summary = numpy.empty([res.ndim,3], dtype=float)
+        idcentre = res.logl[res.wnot0].argmax()
+        for i, sample in enumerate( res.samples.T ) :
+            summary[i,0] = sample[res.wnot0][idcentre]
             low, upp = get_credible_interval(
-                sample, idcentre, quantile, self.weights[self.wnot0]
+                sample[res.wnot0], idcentre, quantile, res.weights[res.wnot0]
             )
             if low is None : low = -numpy.inf
             if upp is None : upp = +numpy.inf
             summary[i,1] = low
             summary[i,2] = upp
         
     if stat_type == 'quantiles' :
```

### Comparing `galapy-fit-0.5.2/galapy/analysis/plot.py` & `galapy_fit-0.5.3/galapy/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/configuration/configure.py` & `galapy_fit-0.5.3/galapy/configuration/configure.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/configuration/filesystem.py` & `galapy_fit-0.5.3/galapy/configuration/filesystem.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/internal/abc.py` & `galapy_fit-0.5.3/galapy/internal/abc.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/internal/data.py` & `galapy_fit-0.5.3/galapy/internal/data.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/internal/globs.py` & `galapy_fit-0.5.3/galapy/internal/globs.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/internal/utils.py` & `galapy_fit-0.5.3/galapy/internal/utils.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/io/hdf5.py` & `galapy_fit-0.5.3/galapy/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/sampling/Observation.py` & `galapy_fit-0.5.3/galapy/sampling/Observation.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/sampling/Results.py` & `galapy_fit-0.5.3/galapy/sampling/Results.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/sampling/Run.py` & `galapy_fit-0.5.3/galapy/sampling/Run.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/sampling/Sampler.py` & `galapy_fit-0.5.3/galapy/sampling/Sampler.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy/sampling/Statistics.py` & `galapy_fit-0.5.3/galapy/sampling/Statistics.py`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/galapy_fit.egg-info/PKG-INFO` & `galapy_fit-0.5.3/galapy_fit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galapy-fit
-Version: 0.5.2
+Version: 0.5.3
 Summary: GalaPy - Spectral modelling tool for galaxies in Python
 Author-email: Tommaso Ronconi <tronconi@sissa.it>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,15 +690,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: emcee
 Requires-Dist: dynesty
-Requires-Dist: matplotlib
+Requires-Dist: matplotlib>=3.6
 Requires-Dist: getdist
 Requires-Dist: requests
 Requires-Dist: h5py
 Provides-Extra: dev
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: test
@@ -719,15 +719,19 @@
 .. |build-badge| image:: https://github.com/TommasoRonconi/galapy/actions/workflows/build-wheels.yml/badge.svg
    :alt: Building
 
 .. |docs-badge| image:: https://readthedocs.org/projects/galapy/badge/?version=latest
    :target: https://galapy.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
-|test-badge| |build-badge| |docs-badge|
+.. |arxiv-badge| image:: https://img.shields.io/badge/arXiv-2402.12427-b31b1b.svg
+   :target: https://arxiv.org/abs/2402.12427
+   :alt: ArXiV preprint
+
+|test-badge| |build-badge| |docs-badge| |arxiv-badge|
 	 
 GalaPy is an open source, extensible API for modelling and fitting the Spectral Energy Distribution (SED) of galaxies from the X-ray to the radio band,
 as well as the evolution of their components and dust attenuation/reradiation.
 It provides functions, classes and terminal commands for Bayesian inference of galaxy properties from panchromatic photometric data,
 as well as for the analysis and simulation of galaxies spectral properties.
 
 .. image:: https://raw.githubusercontent.com/TommasoRonconi/galapy_database/main/images/GalaPy_Example.png
```

### Comparing `galapy-fit-0.5.2/galapy_fit.egg-info/SOURCES.txt` & `galapy_fit-0.5.3/galapy_fit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/pybind11/pyb11_CCSP.cpp` & `galapy_fit-0.5.3/pybind11/pyb11_CCSP.cpp`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/pybind11/pyb11_CISM.cpp` & `galapy_fit-0.5.3/pybind11/pyb11_CISM.cpp`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/pybind11/pyb11_CNFF.cpp` & `galapy_fit-0.5.3/pybind11/pyb11_CNFF.cpp`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/pybind11/pyb11_CSFH.cpp` & `galapy_fit-0.5.3/pybind11/pyb11_CSFH.cpp`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/pybind11/pyb11_CSYN.cpp` & `galapy_fit-0.5.3/pybind11/pyb11_CSYN.cpp`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/pybind11/pyb11_interpolation.cpp` & `galapy_fit-0.5.3/pybind11/pyb11_interpolation.cpp`

 * *Files identical despite different names*

### Comparing `galapy-fit-0.5.2/pyproject.toml` & `galapy_fit-0.5.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 dynamic = ["version", "description"]
 dependencies = [
     'numpy',
     'scipy',
     'tqdm',
     'emcee',
     'dynesty',
-    'matplotlib',
+    'matplotlib>=3.6',
     'getdist',
     'requests',
     'h5py'
 ]
 requires-python = ">=3.7"
 
 [project.urls]
@@ -53,14 +53,14 @@
 
 [project.scripts]
 galapy-fit = "galapy.sampling.Run:_run"
 galapy-genparams = "galapy.sampling.Run:_generate_parameter_file"
 galapy-download-database = "galapy.internal.data:_entrypoint_download_database"
 
 [bumpver]
-current_version = "v0.5.2"
+current_version = "v0.5.3"
 version_pattern = "vMAJOR.MINOR.PATCH"
 
 [bumpver.file_patterns]
 "galapy/__init__.py" = [
     "__version__ = '{version}'",
 ]
```

### Comparing `galapy-fit-0.5.2/setup.py` & `galapy_fit-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
            install_requires = [
                'pybind11',
                'numpy',
                'scipy',
                'tqdm',
                'emcee',
                'dynesty',
-               'matplotlib',
+               'matplotlib>=3.6',
                'getdist',
                'requests',
                'h5py',
                'pytest'
            ]
     )
```

