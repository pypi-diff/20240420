# Comparing `tmp/devicetorch-0.1.2.tar.gz` & `tmp/devicetorch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devicetorch-0.1.2.tar", last modified: Sat Apr 20 21:08:50 2024, max compression
+gzip compressed data, was "devicetorch-0.1.3.tar", last modified: Sat Apr 20 21:16:28 2024, max compression
```

## Comparing `devicetorch-0.1.2.tar` & `devicetorch-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 21:08:50.045902 devicetorch-0.1.2/
--rw-r--r--   0 x          (501) staff       (20)       55 2024-04-20 21:08:50.045769 devicetorch-0.1.2/PKG-INFO
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 21:08:50.045133 devicetorch-0.1.2/devicetorch/
--rw-r--r--   0 x          (501) staff       (20)      150 2024-04-20 21:08:37.000000 devicetorch-0.1.2/devicetorch/__init__.py
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 21:08:50.045611 devicetorch-0.1.2/devicetorch.egg-info/
--rw-r--r--   0 x          (501) staff       (20)       55 2024-04-20 21:08:49.000000 devicetorch-0.1.2/devicetorch.egg-info/PKG-INFO
--rw-r--r--   0 x          (501) staff       (20)      172 2024-04-20 21:08:50.000000 devicetorch-0.1.2/devicetorch.egg-info/SOURCES.txt
--rw-r--r--   0 x          (501) staff       (20)        1 2024-04-20 21:08:49.000000 devicetorch-0.1.2/devicetorch.egg-info/dependency_links.txt
--rw-r--r--   0 x          (501) staff       (20)       12 2024-04-20 21:08:49.000000 devicetorch-0.1.2/devicetorch.egg-info/top_level.txt
--rw-r--r--   0 x          (501) staff       (20)       38 2024-04-20 21:08:50.045939 devicetorch-0.1.2/setup.cfg
--rw-r--r--   0 x          (501) staff       (20)      128 2024-04-20 21:08:44.000000 devicetorch-0.1.2/setup.py
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 21:16:28.298102 devicetorch-0.1.3/
+-rw-r--r--   0 x          (501) staff       (20)       55 2024-04-20 21:16:28.297852 devicetorch-0.1.3/PKG-INFO
+-rw-r--r--   0 x          (501) staff       (20)      278 2024-04-20 21:16:18.000000 devicetorch-0.1.3/README.md
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 21:16:28.297096 devicetorch-0.1.3/devicetorch/
+-rw-r--r--   0 x          (501) staff       (20)      150 2024-04-20 21:08:37.000000 devicetorch-0.1.3/devicetorch/__init__.py
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 21:16:28.297695 devicetorch-0.1.3/devicetorch.egg-info/
+-rw-r--r--   0 x          (501) staff       (20)       55 2024-04-20 21:16:28.000000 devicetorch-0.1.3/devicetorch.egg-info/PKG-INFO
+-rw-r--r--   0 x          (501) staff       (20)      182 2024-04-20 21:16:28.000000 devicetorch-0.1.3/devicetorch.egg-info/SOURCES.txt
+-rw-r--r--   0 x          (501) staff       (20)        1 2024-04-20 21:16:28.000000 devicetorch-0.1.3/devicetorch.egg-info/dependency_links.txt
+-rw-r--r--   0 x          (501) staff       (20)       12 2024-04-20 21:16:28.000000 devicetorch-0.1.3/devicetorch.egg-info/top_level.txt
+-rw-r--r--   0 x          (501) staff       (20)       38 2024-04-20 21:16:28.298205 devicetorch-0.1.3/setup.cfg
+-rw-r--r--   0 x          (501) staff       (20)      128 2024-04-20 21:16:23.000000 devicetorch-0.1.3/setup.py
```

