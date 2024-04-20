# Comparing `tmp/Pyphonic-0.9.1.tar.gz` & `tmp/pyphonic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\tomgr\pyphonic\dist\tmpdfytjfd4\Pyphonic-0.9.1.tar", last modified: Sat Jul 17 02:30:41 2021, max compression
+gzip compressed data, was "pyphonic-1.0.1.tar", last modified: Sat Apr 20 04:09:05 2024, max compression
```

## Comparing `Pyphonic-0.9.1.tar` & `pyphonic-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,28 @@
-drwxrwxrwx   0        0        0        0 2021-07-17 02:30:41.796797 Pyphonic-0.9.1/
--rw-rw-rw-   0        0        0     1129 2021-07-15 02:36:14.000000 Pyphonic-0.9.1/LICENSE
--rw-rw-rw-   0        0        0     3302 2021-07-17 02:30:41.796797 Pyphonic-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     2546 2021-07-17 02:30:18.000000 Pyphonic-0.9.1/README.md
--rw-rw-rw-   0        0        0      108 2021-06-29 02:11:33.000000 Pyphonic-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2021-07-17 02:30:41.797801 Pyphonic-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1090 2021-07-17 02:30:27.000000 Pyphonic-0.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-07-17 02:30:41.771797 Pyphonic-0.9.1/src/
-drwxrwxrwx   0        0        0        0 2021-07-17 02:30:41.794797 Pyphonic-0.9.1/src/Pyphonic.egg-info/
--rw-rw-rw-   0        0        0     3302 2021-07-17 02:30:41.000000 Pyphonic-0.9.1/src/Pyphonic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2021-07-17 02:30:41.000000 Pyphonic-0.9.1/src/Pyphonic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-17 02:30:41.000000 Pyphonic-0.9.1/src/Pyphonic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2021-07-17 02:30:41.000000 Pyphonic-0.9.1/src/Pyphonic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-07-17 02:30:41.000000 Pyphonic-0.9.1/src/Pyphonic.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-07-17 02:30:41.795797 Pyphonic-0.9.1/src/pyphonic/
--rw-rw-rw-   0        0        0     3167 2021-06-29 02:20:41.000000 Pyphonic-0.9.1/src/pyphonic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:09:05.341449 pyphonic-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-20 04:09:05.341449 pyphonic-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-20 04:09:00.000000 pyphonic-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-20 04:09:00.000000 pyphonic-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 04:09:05.341449 pyphonic-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:09:05.333449 pyphonic-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:09:05.337449 pyphonic-1.0.1/src/pyphonic/
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/arp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/butterworth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/circular_buffer_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/flipper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/midi_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/midirando.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/multithreaded_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/stretcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/syncd_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/torch_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/torch_saturator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:09:05.341449 pyphonic-1.0.1/src/pyphonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-20 04:09:05.000000 pyphonic-1.0.1/src/pyphonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-20 04:09:05.000000 pyphonic-1.0.1/src/pyphonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 04:09:05.000000 pyphonic-1.0.1/src/pyphonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 04:09:05.000000 pyphonic-1.0.1/src/pyphonic.egg-info/top_level.txt
```

