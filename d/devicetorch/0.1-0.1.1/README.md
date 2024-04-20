# Comparing `tmp/devicetorch-0.1.tar.gz` & `tmp/devicetorch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devicetorch-0.1.tar", last modified: Sat Apr 20 19:44:06 2024, max compression
+gzip compressed data, was "devicetorch-0.1.1.tar", last modified: Sat Apr 20 20:03:14 2024, max compression
```

## Comparing `devicetorch-0.1.tar` & `devicetorch-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 19:44:06.185334 devicetorch-0.1/
--rw-r--r--   0 x          (501) staff       (20)       53 2024-04-20 19:44:06.185135 devicetorch-0.1/PKG-INFO
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 19:44:06.184610 devicetorch-0.1/devicetorch.egg-info/
--rw-r--r--   0 x          (501) staff       (20)       53 2024-04-20 19:44:06.000000 devicetorch-0.1/devicetorch.egg-info/PKG-INFO
--rw-r--r--   0 x          (501) staff       (20)      148 2024-04-20 19:44:06.000000 devicetorch-0.1/devicetorch.egg-info/SOURCES.txt
--rw-r--r--   0 x          (501) staff       (20)        1 2024-04-20 19:44:06.000000 devicetorch-0.1/devicetorch.egg-info/dependency_links.txt
--rw-r--r--   0 x          (501) staff       (20)        1 2024-04-20 19:44:06.000000 devicetorch-0.1/devicetorch.egg-info/top_level.txt
--rw-r--r--   0 x          (501) staff       (20)       38 2024-04-20 19:44:06.185429 devicetorch-0.1/setup.cfg
--rw-r--r--   0 x          (501) staff       (20)      126 2024-04-20 19:43:17.000000 devicetorch-0.1/setup.py
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 20:03:14.139602 devicetorch-0.1.1/
+-rw-r--r--   0 x          (501) staff       (20)       55 2024-04-20 20:03:14.139456 devicetorch-0.1.1/PKG-INFO
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 20:03:14.138469 devicetorch-0.1.1/devicetorch/
+-rw-r--r--   0 x          (501) staff       (20)      155 2024-04-20 19:35:15.000000 devicetorch-0.1.1/devicetorch/__init__.py
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 20:03:14.139243 devicetorch-0.1.1/devicetorch.egg-info/
+-rw-r--r--   0 x          (501) staff       (20)       55 2024-04-20 20:03:14.000000 devicetorch-0.1.1/devicetorch.egg-info/PKG-INFO
+-rw-r--r--   0 x          (501) staff       (20)      172 2024-04-20 20:03:14.000000 devicetorch-0.1.1/devicetorch.egg-info/SOURCES.txt
+-rw-r--r--   0 x          (501) staff       (20)        1 2024-04-20 20:03:14.000000 devicetorch-0.1.1/devicetorch.egg-info/dependency_links.txt
+-rw-r--r--   0 x          (501) staff       (20)       12 2024-04-20 20:03:14.000000 devicetorch-0.1.1/devicetorch.egg-info/top_level.txt
+-rw-r--r--   0 x          (501) staff       (20)       38 2024-04-20 20:03:14.139642 devicetorch-0.1.1/setup.cfg
+-rw-r--r--   0 x          (501) staff       (20)      128 2024-04-20 20:03:05.000000 devicetorch-0.1.1/setup.py
```

