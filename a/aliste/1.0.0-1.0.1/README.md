# Comparing `tmp/aliste-1.0.0.tar.gz` & `tmp/aliste-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliste-1.0.0.tar", max compression
+gzip compressed data, was "aliste-1.0.1.tar", max compression
```

## Comparing `aliste-1.0.0.tar` & `aliste-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2024-04-20 16:05:43.312360 aliste-1.0.0/LICENSE
--rw-r--r--   0        0        0      356 2024-04-20 16:05:43.312360 aliste-1.0.0/README.md
--rw-r--r--   0        0        0       25 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/__init__.py
--rw-r--r--   0        0        0     3642 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/broker.py
--rw-r--r--   0        0        0      517 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/constants.py
--rw-r--r--   0        0        0     1884 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/device.py
--rw-r--r--   0        0        0      136 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/enums.py
--rw-r--r--   0        0        0      333 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/home.py
--rw-r--r--   0        0        0     4705 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/hub.py
--rw-r--r--   0        0        0      420 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/user.py
--rw-r--r--   0        0        0      220 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/utils.py
--rw-r--r--   0        0        0      464 2024-04-20 16:05:43.312360 aliste-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 aliste-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-20 17:08:34.985540 aliste-1.0.1/LICENSE
+-rw-r--r--   0        0        0      356 2024-04-20 17:08:34.985540 aliste-1.0.1/README.md
+-rw-r--r--   0        0        0       25 2024-04-20 17:08:34.985540 aliste-1.0.1/aliste/__init__.py
+-rw-r--r--   0        0        0     3642 2024-04-20 17:08:34.985540 aliste-1.0.1/aliste/broker.py
+-rw-r--r--   0        0        0      517 2024-04-20 17:08:34.985540 aliste-1.0.1/aliste/constants.py
+-rw-r--r--   0        0        0     1884 2024-04-20 17:08:34.985540 aliste-1.0.1/aliste/device.py
+-rw-r--r--   0        0        0      136 2024-04-20 17:08:34.985540 aliste-1.0.1/aliste/enums.py
+-rw-r--r--   0        0        0      333 2024-04-20 17:08:34.985540 aliste-1.0.1/aliste/home.py
+-rw-r--r--   0        0        0     4705 2024-04-20 17:08:34.985540 aliste-1.0.1/aliste/hub.py
+-rw-r--r--   0        0        0      420 2024-04-20 17:08:34.985540 aliste-1.0.1/aliste/user.py
+-rw-r--r--   0        0        0      220 2024-04-20 17:08:34.985540 aliste-1.0.1/aliste/utils.py
+-rw-r--r--   0        0        0      449 2024-04-20 17:08:34.985540 aliste-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 aliste-1.0.1/PKG-INFO
```

### Comparing `aliste-1.0.0/LICENSE` & `aliste-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aliste-1.0.0/aliste/broker.py` & `aliste-1.0.1/aliste/broker.py`

 * *Files identical despite different names*

### Comparing `aliste-1.0.0/aliste/constants.py` & `aliste-1.0.1/aliste/constants.py`

 * *Files identical despite different names*

### Comparing `aliste-1.0.0/aliste/device.py` & `aliste-1.0.1/aliste/device.py`

 * *Files identical despite different names*

### Comparing `aliste-1.0.0/aliste/hub.py` & `aliste-1.0.1/aliste/hub.py`

 * *Files identical despite different names*

