# Comparing `tmp/tui_dsg-202404201018.tar.gz` & `tmp/tui_dsg-202404201342.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsg-202404201018.tar", last modified: Sat Apr 20 10:18:45 2024, max compression
+gzip compressed data, was "tui_dsg-202404201342.tar", last modified: Sat Apr 20 11:42:50 2024, max compression
```

## Comparing `tui_dsg-202404201018.tar` & `tui_dsg-202404201342.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 10:18:45.120270 tui_dsg-202404201018/
--rw-r--r--   0 root         (0) root         (0)     1179 2024-04-20 10:18:45.120270 tui_dsg-202404201018/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 10:18:45.120270 tui_dsg-202404201018/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1463 2024-03-28 15:33:07.000000 tui_dsg-202404201018/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 10:18:45.116270 tui_dsg-202404201018/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 10:18:45.116270 tui_dsg-202404201018/src/tui_dsg/
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-03-28 13:23:09.000000 tui_dsg-202404201018/src/tui_dsg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 10:18:45.116270 tui_dsg-202404201018/src/tui_dsg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1179 2024-04-20 10:18:45.000000 tui_dsg-202404201018/src/tui_dsg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      206 2024-04-20 10:18:45.000000 tui_dsg-202404201018/src/tui_dsg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 10:18:45.000000 tui_dsg-202404201018/src/tui_dsg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      339 2024-04-20 10:18:45.000000 tui_dsg-202404201018/src/tui_dsg.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-20 10:18:45.000000 tui_dsg-202404201018/src/tui_dsg.egg-info/top_level.txt
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-04-20 11:42:50.596034 tui_dsg-202404201342/
+-rw-r--r--   0 eric      (1000) eric      (1000)     1179 2024-04-20 11:42:50.592034 tui_dsg-202404201342/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2024-04-20 11:42:50.596034 tui_dsg-202404201342/setup.cfg
+-rwxrwxr-x   0 eric      (1000) eric      (1000)     1463 2024-04-11 13:07:44.000000 tui_dsg-202404201342/setup.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-04-20 11:42:50.592034 tui_dsg-202404201342/src/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-04-20 11:42:50.592034 tui_dsg-202404201342/src/tui_dsg/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        5 2024-04-11 13:07:44.000000 tui_dsg-202404201342/src/tui_dsg/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-04-20 11:42:50.592034 tui_dsg-202404201342/src/tui_dsg.egg-info/
+-rw-r--r--   0 eric      (1000) eric      (1000)     1179 2024-04-20 11:42:50.000000 tui_dsg-202404201342/src/tui_dsg.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)      206 2024-04-20 11:42:50.000000 tui_dsg-202404201342/src/tui_dsg.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2024-04-20 11:42:50.000000 tui_dsg-202404201342/src/tui_dsg.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      339 2024-04-20 11:42:50.000000 tui_dsg-202404201342/src/tui_dsg.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        8 2024-04-20 11:42:50.000000 tui_dsg-202404201342/src/tui_dsg.egg-info/top_level.txt
```

### Comparing `tui_dsg-202404201018/PKG-INFO` & `tui_dsg-202404201342/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsg
-Version: 202404201018
+Version: 202404201342
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-grundlagen
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsg-202404201018/setup.py` & `tui_dsg-202404201342/setup.py`

 * *Files identical despite different names*

### Comparing `tui_dsg-202404201018/src/tui_dsg.egg-info/PKG-INFO` & `tui_dsg-202404201342/src/tui_dsg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsg
-Version: 202404201018
+Version: 202404201342
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-grundlagen
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

