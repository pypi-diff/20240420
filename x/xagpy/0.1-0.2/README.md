# Comparing `tmp/xagpy-0.1.tar.gz` & `tmp/xagpy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xagpy-0.1.tar", last modified: Tue Apr  2 16:36:11 2024, max compression
+gzip compressed data, was "xagpy-0.2.tar", last modified: Sat Apr 20 13:26:39 2024, max compression
```

## Comparing `xagpy-0.1.tar` & `xagpy-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 16:36:11.807155 xagpy-0.1/
--rw-rw-rw-   0        0        0     1083 2024-04-02 16:22:00.000000 xagpy-0.1/LICENSE
--rw-rw-rw-   0        0        0      222 2024-04-02 16:36:11.804057 xagpy-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       61 2024-04-02 16:22:00.000000 xagpy-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 16:36:11.808174 xagpy-0.1/setup.cfg
--rw-rw-rw-   0        0        0      304 2024-04-02 16:26:16.000000 xagpy-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 16:36:11.787048 xagpy-0.1/xagpy/
--rw-rw-rw-   0        0        0       24 2024-04-02 15:51:44.000000 xagpy-0.1/xagpy/__init__.py
--rw-rw-rw-   0        0        0     1497 2024-04-02 16:12:24.000000 xagpy-0.1/xagpy/api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 16:36:11.801485 xagpy-0.1/xagpy.egg-info/
--rw-rw-rw-   0        0        0      222 2024-04-02 16:36:11.000000 xagpy-0.1/xagpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-04-02 16:36:11.000000 xagpy-0.1/xagpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 16:36:11.000000 xagpy-0.1/xagpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 16:36:11.000000 xagpy-0.1/xagpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-02 16:36:11.000000 xagpy-0.1/xagpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:26:39.267424 xagpy-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-20 13:26:35.000000 xagpy-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-20 13:26:39.267424 xagpy-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-20 13:26:35.000000 xagpy-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:26:39.267424 xagpy-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-20 13:26:35.000000 xagpy-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:26:39.267424 xagpy-0.2/xagpy/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 13:26:35.000000 xagpy-0.2/xagpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-20 13:26:35.000000 xagpy-0.2/xagpy/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:26:39.267424 xagpy-0.2/xagpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-20 13:26:39.000000 xagpy-0.2/xagpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-20 13:26:39.000000 xagpy-0.2/xagpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:26:39.000000 xagpy-0.2/xagpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 13:26:39.000000 xagpy-0.2/xagpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 13:26:39.000000 xagpy-0.2/xagpy.egg-info/top_level.txt
```

