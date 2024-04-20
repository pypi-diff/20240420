# Comparing `tmp/pyiptables-2.0.6.tar.gz` & `tmp/pyiptables-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiptables-2.0.6.tar", last modified: Tue Feb 20 01:37:54 2024, max compression
+gzip compressed data, was "pyiptables-2.0.7.tar", last modified: Sat Apr 20 07:30:32 2024, max compression
```

## Comparing `pyiptables-2.0.6.tar` & `pyiptables-2.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 01:37:54.529951 pyiptables-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-02-20 01:37:54.529951 pyiptables-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-02-20 01:37:32.000000 pyiptables-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 01:37:54.529951 pyiptables-2.0.6/pyiptables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 01:37:32.000000 pyiptables-2.0.6/pyiptables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-02-20 01:37:32.000000 pyiptables-2.0.6/pyiptables/securitygroup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 01:37:54.529951 pyiptables-2.0.6/pyiptables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-02-20 01:37:54.000000 pyiptables-2.0.6/pyiptables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-20 01:37:54.000000 pyiptables-2.0.6/pyiptables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 01:37:54.000000 pyiptables-2.0.6/pyiptables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-20 01:37:54.000000 pyiptables-2.0.6/pyiptables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 01:37:54.529951 pyiptables-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-20 01:37:32.000000 pyiptables-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:30:32.786749 pyiptables-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-20 07:30:32.786749 pyiptables-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-20 07:30:22.000000 pyiptables-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:30:32.786749 pyiptables-2.0.7/pyiptables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 07:30:22.000000 pyiptables-2.0.7/pyiptables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-20 07:30:22.000000 pyiptables-2.0.7/pyiptables/securitygroup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:30:32.786749 pyiptables-2.0.7/pyiptables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-20 07:30:32.000000 pyiptables-2.0.7/pyiptables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-20 07:30:32.000000 pyiptables-2.0.7/pyiptables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 07:30:32.000000 pyiptables-2.0.7/pyiptables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 07:30:32.000000 pyiptables-2.0.7/pyiptables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 07:30:32.786749 pyiptables-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-20 07:30:22.000000 pyiptables-2.0.7/setup.py
```

### Comparing `pyiptables-2.0.6/PKG-INFO` & `pyiptables-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyiptables
-Version: 2.0.6
+Version: 2.0.7
 Summary: Simple Python client library for Iptables
-Home-page: https://github.com/xizhendu/iptables
+Home-page: https://github.com/xizhendu/pyiptables
 Author: Xizhen Du
 Author-email: xizhendu@gmail.com
 Description-Content-Type: text/markdown
 
 # iptables
```

### Comparing `pyiptables-2.0.6/README.md` & `pyiptables-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyiptables-2.0.6/pyiptables/securitygroup.py` & `pyiptables-2.0.7/pyiptables/securitygroup.py`

 * *Files identical despite different names*

### Comparing `pyiptables-2.0.6/pyiptables.egg-info/PKG-INFO` & `pyiptables-2.0.7/pyiptables.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyiptables
-Version: 2.0.6
+Version: 2.0.7
 Summary: Simple Python client library for Iptables
-Home-page: https://github.com/xizhendu/iptables
+Home-page: https://github.com/xizhendu/pyiptables
 Author: Xizhen Du
 Author-email: xizhendu@gmail.com
 Description-Content-Type: text/markdown
 
 # iptables
```

