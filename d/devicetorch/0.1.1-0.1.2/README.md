# Comparing `tmp/devicetorch-0.1.1.tar.gz` & `tmp/devicetorch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devicetorch-0.1.1.tar", last modified: Sat Apr 20 20:03:14 2024, max compression
+gzip compressed data, was "devicetorch-0.1.2.tar", last modified: Sat Apr 20 21:08:50 2024, max compression
```

## Comparing `devicetorch-0.1.1.tar` & `devicetorch-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 20:03:14.139602 devicetorch-0.1.1/
--rw-r--r--   0 x          (501) staff       (20)       55 2024-04-20 20:03:14.139456 devicetorch-0.1.1/PKG-INFO
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 20:03:14.138469 devicetorch-0.1.1/devicetorch/
--rw-r--r--   0 x          (501) staff       (20)      155 2024-04-20 19:35:15.000000 devicetorch-0.1.1/devicetorch/__init__.py
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 20:03:14.139243 devicetorch-0.1.1/devicetorch.egg-info/
--rw-r--r--   0 x          (501) staff       (20)       55 2024-04-20 20:03:14.000000 devicetorch-0.1.1/devicetorch.egg-info/PKG-INFO
--rw-r--r--   0 x          (501) staff       (20)      172 2024-04-20 20:03:14.000000 devicetorch-0.1.1/devicetorch.egg-info/SOURCES.txt
--rw-r--r--   0 x          (501) staff       (20)        1 2024-04-20 20:03:14.000000 devicetorch-0.1.1/devicetorch.egg-info/dependency_links.txt
--rw-r--r--   0 x          (501) staff       (20)       12 2024-04-20 20:03:14.000000 devicetorch-0.1.1/devicetorch.egg-info/top_level.txt
--rw-r--r--   0 x          (501) staff       (20)       38 2024-04-20 20:03:14.139642 devicetorch-0.1.1/setup.cfg
--rw-r--r--   0 x          (501) staff       (20)      128 2024-04-20 20:03:05.000000 devicetorch-0.1.1/setup.py
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 21:08:50.045902 devicetorch-0.1.2/
+-rw-r--r--   0 x          (501) staff       (20)       55 2024-04-20 21:08:50.045769 devicetorch-0.1.2/PKG-INFO
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 21:08:50.045133 devicetorch-0.1.2/devicetorch/
+-rw-r--r--   0 x          (501) staff       (20)      150 2024-04-20 21:08:37.000000 devicetorch-0.1.2/devicetorch/__init__.py
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 21:08:50.045611 devicetorch-0.1.2/devicetorch.egg-info/
+-rw-r--r--   0 x          (501) staff       (20)       55 2024-04-20 21:08:49.000000 devicetorch-0.1.2/devicetorch.egg-info/PKG-INFO
+-rw-r--r--   0 x          (501) staff       (20)      172 2024-04-20 21:08:50.000000 devicetorch-0.1.2/devicetorch.egg-info/SOURCES.txt
+-rw-r--r--   0 x          (501) staff       (20)        1 2024-04-20 21:08:49.000000 devicetorch-0.1.2/devicetorch.egg-info/dependency_links.txt
+-rw-r--r--   0 x          (501) staff       (20)       12 2024-04-20 21:08:49.000000 devicetorch-0.1.2/devicetorch.egg-info/top_level.txt
+-rw-r--r--   0 x          (501) staff       (20)       38 2024-04-20 21:08:50.045939 devicetorch-0.1.2/setup.cfg
+-rw-r--r--   0 x          (501) staff       (20)      128 2024-04-20 21:08:44.000000 devicetorch-0.1.2/setup.py
```

