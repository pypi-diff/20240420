# Comparing `tmp/kvix-0.1.1.tar.gz` & `tmp/kvix-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvix-0.1.1.tar", last modified: Wed Mar 27 16:21:28 2024, max compression
+gzip compressed data, was "kvix-0.1.2.tar", last modified: Sat Apr 20 09:07:01 2024, max compression
```

## Comparing `kvix-0.1.1.tar` & `kvix-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:21:28.208014 kvix-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-27 16:21:16.000000 kvix-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-27 16:21:28.208014 kvix-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-03-27 16:21:16.000000 kvix-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:21:28.204014 kvix-0.1.1/kvix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-27 16:21:28.000000 kvix-0.1.1/kvix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-27 16:21:28.000000 kvix-0.1.1/kvix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 16:21:28.000000 kvix-0.1.1/kvix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-27 16:21:28.000000 kvix-0.1.1/kvix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-27 16:21:28.000000 kvix-0.1.1/kvix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-27 16:21:28.000000 kvix-0.1.1/kvix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-27 16:21:16.000000 kvix-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 16:21:28.208014 kvix-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:21:28.200014 kvix-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:21:28.204014 kvix-0.1.1/src/kvix/
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/l10n.py
--rw-r--r--   0 runner    (1001) docker     (127)    67399 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/logo.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:21:28.204014 kvix-0.1.1/src/kvix/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:21:28.208014 kvix-0.1.1/src/kvix/plugin/builtin/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/builtin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/builtin/add_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/builtin/base64decode.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/builtin/base64encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/builtin/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/builtin/edit_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/builtin/machinist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/builtin/openurl.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/builtin/quit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/builtin/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/builtin/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/builtin/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:21:28.208014 kvix-0.1.1/src/kvix/plugin/discovery/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/plugin/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/stor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:21:28.208014 kvix-0.1.1/src/kvix/ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:21:28.208014 kvix-0.1.1/src/kvix/ui/tk/
--rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/ui/tk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/ui/tk/plus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:21:28.208014 kvix-0.1.1/src/kvix/ui/tk/uni/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/ui/tk/uni/classic.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/ui/tk/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/ui/tray.py
--rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-03-27 16:21:16.000000 kvix-0.1.1/src/kvix/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:21:28.208014 kvix-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-27 16:21:16.000000 kvix-0.1.1/test/test_propty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:07:01.635272 kvix-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 09:06:51.000000 kvix-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-20 09:07:01.635272 kvix-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-20 09:06:51.000000 kvix-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:07:01.631272 kvix-0.1.2/kvix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-20 09:07:01.000000 kvix-0.1.2/kvix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-20 09:07:01.000000 kvix-0.1.2/kvix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:07:01.000000 kvix-0.1.2/kvix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-20 09:07:01.000000 kvix-0.1.2/kvix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-20 09:07:01.000000 kvix-0.1.2/kvix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 09:07:01.000000 kvix-0.1.2/kvix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-20 09:06:51.000000 kvix-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 09:07:01.635272 kvix-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:07:01.627272 kvix-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:07:01.631272 kvix-0.1.2/src/kvix/
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/l10n.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67399 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/logo.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:07:01.631272 kvix-0.1.2/src/kvix/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:07:01.635272 kvix-0.1.2/src/kvix/plugin/builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/builtin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/builtin/add_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/builtin/base64decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/builtin/base64encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/builtin/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/builtin/edit_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/builtin/machinist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/builtin/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/builtin/quit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/builtin/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/builtin/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/builtin/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:07:01.635272 kvix-0.1.2/src/kvix/plugin/discovery/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/plugin/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/stor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:07:01.635272 kvix-0.1.2/src/kvix/ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:07:01.635272 kvix-0.1.2/src/kvix/ui/tk/
+-rw-r--r--   0 runner    (1001) docker     (127)    17612 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/ui/tk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/ui/tk/plus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:07:01.635272 kvix-0.1.2/src/kvix/ui/tk/uni/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/ui/tk/uni/classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/ui/tk/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/ui/tray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-04-20 09:06:51.000000 kvix-0.1.2/src/kvix/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:07:01.635272 kvix-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-20 09:06:51.000000 kvix-0.1.2/test/test_propty.py
```

### Comparing `kvix-0.1.1/PKG-INFO` & `kvix-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvix
-Version: 0.1.1
+Version: 0.1.2
 Description-Content-Type: text/markdown
 Requires-Dist: funcy==1.17
 Requires-Dist: pynput==1.7.6
 Requires-Dist: pystray==0.19.4
 Requires-Dist: pygobject==3.46.0
 Requires-Dist: pkgconfig==1.5.5
 Requires-Dist: pyclip==0.7.0
```

### Comparing `kvix-0.1.1/README.md` & `kvix-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/kvix.egg-info/PKG-INFO` & `kvix-0.1.2/kvix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvix
-Version: 0.1.1
+Version: 0.1.2
 Description-Content-Type: text/markdown
 Requires-Dist: funcy==1.17
 Requires-Dist: pynput==1.7.6
 Requires-Dist: pystray==0.19.4
 Requires-Dist: pygobject==3.46.0
 Requires-Dist: pkgconfig==1.5.5
 Requires-Dist: pyclip==0.7.0
```

### Comparing `kvix-0.1.1/kvix.egg-info/SOURCES.txt` & `kvix-0.1.2/kvix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/pyproject.toml` & `kvix-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/__init__.py` & `kvix-0.1.2/src/kvix/__init__.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/app.py` & `kvix-0.1.2/src/kvix/app.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/conf.py` & `kvix-0.1.2/src/kvix/conf.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/impl.py` & `kvix-0.1.2/src/kvix/impl.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/l10n.py` & `kvix-0.1.2/src/kvix/l10n.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/logo.jpg` & `kvix-0.1.2/src/kvix/logo.jpg`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/builtin/__init__.py` & `kvix-0.1.2/src/kvix/plugin/builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/builtin/add_action.py` & `kvix-0.1.2/src/kvix/plugin/builtin/add_action.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/builtin/base64decode.py` & `kvix-0.1.2/src/kvix/plugin/builtin/base64decode.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/builtin/base64encode.py` & `kvix-0.1.2/src/kvix/plugin/builtin/base64encode.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/builtin/calculator.py` & `kvix-0.1.2/src/kvix/plugin/builtin/calculator.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/builtin/edit_action.py` & `kvix-0.1.2/src/kvix/plugin/builtin/edit_action.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/builtin/machinist.py` & `kvix-0.1.2/src/kvix/plugin/builtin/machinist.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/builtin/openurl.py` & `kvix-0.1.2/src/kvix/plugin/builtin/openurl.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/builtin/quit.py` & `kvix-0.1.2/src/kvix/plugin/builtin/quit.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/builtin/settings.py` & `kvix-0.1.2/src/kvix/plugin/builtin/settings.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/builtin/shell.py` & `kvix-0.1.2/src/kvix/plugin/builtin/shell.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/builtin/websearch.py` & `kvix-0.1.2/src/kvix/plugin/builtin/websearch.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/discovery/__init__.py` & `kvix-0.1.2/src/kvix/plugin/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/plugin/impl.py` & `kvix-0.1.2/src/kvix/plugin/impl.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/remote.py` & `kvix-0.1.2/src/kvix/remote.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/server.py` & `kvix-0.1.2/src/kvix/server.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/stor.py` & `kvix-0.1.2/src/kvix/stor.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/ui/tk/__init__.py` & `kvix-0.1.2/src/kvix/ui/tk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,33 +334,27 @@
                     self.parent.root.after_idle(lambda: alt.execute())
 
                 popup_menu.add_command(label=str(alt), command=execute)
             popup_menu.tk_popup(x, y)
 
     def _on_popup_key_press(self):
         item: Item | None = self._get_selected_item()
+        if not item and self._item_list:
+            item = self._item_list[0]
         if item:
             x: int = int(
                 (
                     int(self._result_listbox.winfo_rootx())
                     + int(self._result_listbox.winfo_width()) / 3
                 )
             )
 
-            selected_index: int | None = self._get_selected_index()
-            if isinstance(selected_index, int):
-                coords: tuple[int, int, int, int] = self._result_listbox.bbox(selected_index)
-                y: int = int(self._result_listbox.winfo_rooty() + (coords[1] + coords[3] / 2))
-            else:
-                y: int = int(
-                    (
-                        int(self._result_listbox.winfo_rooty())
-                        + int(self._result_listbox.winfo_height()) / 3
-                    )
-                )
+            selected_index: int = self._get_selected_index() or 0
+            coords: tuple[int, int, int, int] = self._result_listbox.bbox(selected_index)
+            y: int = int(self._result_listbox.winfo_rooty() + (coords[1] + coords[3] / 2))
             self._show_popup_menu(item, x, y)
 
     def _select_item_at_y_pos(self, y: int):
         self._result_listbox.selection_clear(0, uni.END)
         self._result_listbox.selection_set(self._result_listbox.nearest(y))
 
     def activate(
```

### Comparing `kvix-0.1.1/src/kvix/ui/tk/plus.py` & `kvix-0.1.2/src/kvix/ui/tk/plus.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/ui/tray.py` & `kvix-0.1.2/src/kvix/ui/tray.py`

 * *Files identical despite different names*

### Comparing `kvix-0.1.1/src/kvix/util.py` & `kvix-0.1.2/src/kvix/util.py`

 * *Files identical despite different names*

