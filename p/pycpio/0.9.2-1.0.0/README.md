# Comparing `tmp/pycpio-0.9.2.tar.gz` & `tmp/pycpio-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycpio-0.9.2.tar", last modified: Mon Apr 15 01:11:07 2024, max compression
+gzip compressed data, was "pycpio-1.0.0.tar", last modified: Sat Apr 20 00:26:07 2024, max compression
```

## Comparing `pycpio-0.9.2.tar` & `pycpio-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.958554 pycpio-0.9.2/
--rw-r--r--   0 desu      (1000) desu      (1000)    18092 2023-11-26 02:38:37.000000 pycpio-0.9.2/LICENSE
--rw-r--r--   0 desu      (1000) desu      (1000)      648 2024-04-15 01:11:07.958554 pycpio-0.9.2/PKG-INFO
--rw-r--r--   0 desu      (1000) desu      (1000)      687 2024-04-15 01:03:04.000000 pycpio-0.9.2/pyproject.toml
--rw-r--r--   0 desu      (1000) desu      (1000)       84 2023-11-25 18:42:57.000000 pycpio-0.9.2/readme.md
--rw-r--r--   0 desu      (1000) desu      (1000)       38 2024-04-15 01:11:07.958554 pycpio-0.9.2/setup.cfg
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.953554 pycpio-0.9.2/src/
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.954554 pycpio-0.9.2/src/pycpio/
--rw-r--r--   0 desu      (1000) desu      (1000)       49 2023-11-26 16:53:57.000000 pycpio-0.9.2/src/pycpio/__init__.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.956554 pycpio-0.9.2/src/pycpio/cpio/
--rw-r--r--   0 desu      (1000) desu      (1000)      172 2023-12-02 22:27:03.000000 pycpio-0.9.2/src/pycpio/cpio/__init__.py
--rw-r--r--   0 desu      (1000) desu      (1000)     4902 2024-01-11 19:47:06.000000 pycpio-0.9.2/src/pycpio/cpio/archive.py
--rw-r--r--   0 desu      (1000) desu      (1000)      843 2023-12-03 02:12:07.000000 pycpio-0.9.2/src/pycpio/cpio/chardev.py
--rw-r--r--   0 desu      (1000) desu      (1000)      447 2023-11-27 04:09:12.000000 pycpio-0.9.2/src/pycpio/cpio/common.py
--rw-r--r--   0 desu      (1000) desu      (1000)     6611 2024-03-24 23:10:29.000000 pycpio-0.9.2/src/pycpio/cpio/data.py
--rw-r--r--   0 desu      (1000) desu      (1000)      624 2023-12-03 02:30:33.000000 pycpio-0.9.2/src/pycpio/cpio/dir.py
--rw-r--r--   0 desu      (1000) desu      (1000)      814 2023-11-28 01:13:44.000000 pycpio-0.9.2/src/pycpio/cpio/file.py
--rw-r--r--   0 desu      (1000) desu      (1000)     1285 2023-12-19 03:06:17.000000 pycpio-0.9.2/src/pycpio/cpio/symlink.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.957554 pycpio-0.9.2/src/pycpio/header/
--rw-r--r--   0 desu      (1000) desu      (1000)      228 2023-11-27 19:50:55.000000 pycpio-0.9.2/src/pycpio/header/__init__.py
--rw-r--r--   0 desu      (1000) desu      (1000)     7950 2024-03-24 23:35:31.000000 pycpio-0.9.2/src/pycpio/header/cpioheader.py
--rw-r--r--   0 desu      (1000) desu      (1000)      701 2023-11-27 22:10:56.000000 pycpio-0.9.2/src/pycpio/header/header_funcs.py
--rw-r--r--   0 desu      (1000) desu      (1000)      411 2023-11-27 22:28:21.000000 pycpio-0.9.2/src/pycpio/header/headers.py
--rwxr-xr-x   0 desu      (1000) desu      (1000)     3257 2024-04-15 01:04:10.000000 pycpio-0.9.2/src/pycpio/main.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.957554 pycpio-0.9.2/src/pycpio/masks/
--rw-r--r--   0 desu      (1000) desu      (1000)      277 2023-11-27 19:37:46.000000 pycpio-0.9.2/src/pycpio/masks/__init__.py
--rw-r--r--   0 desu      (1000) desu      (1000)     1378 2024-03-24 23:37:22.000000 pycpio-0.9.2/src/pycpio/masks/modes.py
--rw-r--r--   0 desu      (1000) desu      (1000)     1499 2023-11-27 18:36:51.000000 pycpio-0.9.2/src/pycpio/masks/permissions.py
--rw-r--r--   0 desu      (1000) desu      (1000)     3704 2024-01-20 23:48:13.000000 pycpio-0.9.2/src/pycpio/pycpio.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.957554 pycpio-0.9.2/src/pycpio/reader/
--rw-r--r--   0 desu      (1000) desu      (1000)       57 2023-11-27 19:34:23.000000 pycpio-0.9.2/src/pycpio/reader/__init__.py
--rw-r--r--   0 desu      (1000) desu      (1000)     3700 2024-01-11 19:46:36.000000 pycpio-0.9.2/src/pycpio/reader/reader.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.958554 pycpio-0.9.2/src/pycpio/writer/
--rw-r--r--   0 desu      (1000) desu      (1000)       57 2023-11-27 19:34:07.000000 pycpio-0.9.2/src/pycpio/writer/__init__.py
--rw-r--r--   0 desu      (1000) desu      (1000)     1584 2024-03-24 22:50:18.000000 pycpio-0.9.2/src/pycpio/writer/writer.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.958554 pycpio-0.9.2/src/pycpio.egg-info/
--rw-r--r--   0 desu      (1000) desu      (1000)      648 2024-04-15 01:11:07.000000 pycpio-0.9.2/src/pycpio.egg-info/PKG-INFO
--rw-r--r--   0 desu      (1000) desu      (1000)      835 2024-04-15 01:11:07.000000 pycpio-0.9.2/src/pycpio.egg-info/SOURCES.txt
--rw-r--r--   0 desu      (1000) desu      (1000)        1 2024-04-15 01:11:07.000000 pycpio-0.9.2/src/pycpio.egg-info/dependency_links.txt
--rw-r--r--   0 desu      (1000) desu      (1000)       44 2024-04-15 01:11:07.000000 pycpio-0.9.2/src/pycpio.egg-info/entry_points.txt
--rw-r--r--   0 desu      (1000) desu      (1000)       14 2024-04-15 01:11:07.000000 pycpio-0.9.2/src/pycpio.egg-info/requires.txt
--rw-r--r--   0 desu      (1000) desu      (1000)        7 2024-04-15 01:11:07.000000 pycpio-0.9.2/src/pycpio.egg-info/top_level.txt
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:26:07.336378 pycpio-1.0.0/
+-rw-r--r--   0 desu      (1000) desu      (1000)    18092 2023-11-26 02:38:37.000000 pycpio-1.0.0/LICENSE
+-rw-r--r--   0 desu      (1000) desu      (1000)      648 2024-04-20 00:26:07.336378 pycpio-1.0.0/PKG-INFO
+-rw-r--r--   0 desu      (1000) desu      (1000)      687 2024-04-19 19:42:18.000000 pycpio-1.0.0/pyproject.toml
+-rw-r--r--   0 desu      (1000) desu      (1000)       84 2023-11-25 18:42:57.000000 pycpio-1.0.0/readme.md
+-rw-r--r--   0 desu      (1000) desu      (1000)       38 2024-04-20 00:26:07.336378 pycpio-1.0.0/setup.cfg
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:26:07.334378 pycpio-1.0.0/src/
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:26:07.334378 pycpio-1.0.0/src/pycpio/
+-rw-r--r--   0 desu      (1000) desu      (1000)       49 2023-11-26 16:53:57.000000 pycpio-1.0.0/src/pycpio/__init__.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:26:07.335378 pycpio-1.0.0/src/pycpio/cpio/
+-rw-r--r--   0 desu      (1000) desu      (1000)      172 2023-12-02 22:27:03.000000 pycpio-1.0.0/src/pycpio/cpio/__init__.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     4902 2024-01-11 19:47:06.000000 pycpio-1.0.0/src/pycpio/cpio/archive.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      843 2023-12-03 02:12:07.000000 pycpio-1.0.0/src/pycpio/cpio/chardev.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      447 2023-11-27 04:09:12.000000 pycpio-1.0.0/src/pycpio/cpio/common.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     6680 2024-04-19 20:06:37.000000 pycpio-1.0.0/src/pycpio/cpio/data.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      624 2023-12-03 02:30:33.000000 pycpio-1.0.0/src/pycpio/cpio/dir.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      814 2023-11-28 01:13:44.000000 pycpio-1.0.0/src/pycpio/cpio/file.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     1285 2023-12-19 03:06:17.000000 pycpio-1.0.0/src/pycpio/cpio/symlink.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:26:07.335378 pycpio-1.0.0/src/pycpio/header/
+-rw-r--r--   0 desu      (1000) desu      (1000)      228 2023-11-27 19:50:55.000000 pycpio-1.0.0/src/pycpio/header/__init__.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     8188 2024-04-19 20:08:07.000000 pycpio-1.0.0/src/pycpio/header/cpioheader.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      701 2023-11-27 22:10:56.000000 pycpio-1.0.0/src/pycpio/header/header_funcs.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      411 2023-11-27 22:28:21.000000 pycpio-1.0.0/src/pycpio/header/headers.py
+-rwxr-xr-x   0 desu      (1000) desu      (1000)     3276 2024-04-19 19:45:20.000000 pycpio-1.0.0/src/pycpio/main.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:26:07.335378 pycpio-1.0.0/src/pycpio/masks/
+-rw-r--r--   0 desu      (1000) desu      (1000)      277 2023-11-27 19:37:46.000000 pycpio-1.0.0/src/pycpio/masks/__init__.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     1378 2024-03-24 23:37:22.000000 pycpio-1.0.0/src/pycpio/masks/modes.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     1499 2024-04-19 20:08:51.000000 pycpio-1.0.0/src/pycpio/masks/permissions.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     3704 2024-01-20 23:48:13.000000 pycpio-1.0.0/src/pycpio/pycpio.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:26:07.336378 pycpio-1.0.0/src/pycpio/reader/
+-rw-r--r--   0 desu      (1000) desu      (1000)       57 2023-11-27 19:34:23.000000 pycpio-1.0.0/src/pycpio/reader/__init__.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     3700 2024-01-11 19:46:36.000000 pycpio-1.0.0/src/pycpio/reader/reader.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:26:07.336378 pycpio-1.0.0/src/pycpio/writer/
+-rw-r--r--   0 desu      (1000) desu      (1000)       57 2023-11-27 19:34:07.000000 pycpio-1.0.0/src/pycpio/writer/__init__.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     1584 2024-03-24 22:50:18.000000 pycpio-1.0.0/src/pycpio/writer/writer.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:26:07.336378 pycpio-1.0.0/src/pycpio.egg-info/
+-rw-r--r--   0 desu      (1000) desu      (1000)      648 2024-04-20 00:26:07.000000 pycpio-1.0.0/src/pycpio.egg-info/PKG-INFO
+-rw-r--r--   0 desu      (1000) desu      (1000)      835 2024-04-20 00:26:07.000000 pycpio-1.0.0/src/pycpio.egg-info/SOURCES.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)        1 2024-04-20 00:26:07.000000 pycpio-1.0.0/src/pycpio.egg-info/dependency_links.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)       44 2024-04-20 00:26:07.000000 pycpio-1.0.0/src/pycpio.egg-info/entry_points.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)       14 2024-04-20 00:26:07.000000 pycpio-1.0.0/src/pycpio.egg-info/requires.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)        7 2024-04-20 00:26:07.000000 pycpio-1.0.0/src/pycpio.egg-info/top_level.txt
```

### Comparing `pycpio-0.9.2/LICENSE` & `pycpio-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycpio-0.9.2/PKG-INFO` & `pycpio-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pycpio
-Version: 0.9.2
+Version: 1.0.0
 Summary: A Python library for reading and writing cpio archives.
 Author-email: Desultory <dev@pyl.onl>
 Project-URL: Homepage, https://github.com/desultory/pycpio
 Project-URL: Issues, https://github.com/desultory/pycpio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: zenlib>=1.7.3
+Requires-Dist: zenlib>=2.0.0
 
 # pycpio
 
 A library for working with CPIO files using python
 
 In active development
```

### Comparing `pycpio-0.9.2/pyproject.toml` & `pycpio-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pycpio"
-version = "0.9.2"
+version = "1.0.0"
 authors = [
   { name="Desultory", email="dev@pyl.onl" },
 ]
 description = "A Python library for reading and writing cpio archives."
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Operating System :: OS Independent",
 ]
-dependencies = ["zenlib >= 1.7.3"]
+dependencies = ["zenlib >= 2.0.0"]
 
 [project.scripts]
 pycpio = "pycpio.main:main"
 
 [project.urls]
 Homepage = "https://github.com/desultory/pycpio"
 Issues = "https://github.com/desultory/pycpio/issues"
```

### Comparing `pycpio-0.9.2/src/pycpio/cpio/archive.py` & `pycpio-1.0.0/src/pycpio/cpio/archive.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.9.2/src/pycpio/cpio/chardev.py` & `pycpio-1.0.0/src/pycpio/cpio/chardev.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.9.2/src/pycpio/cpio/data.py` & `pycpio-1.0.0/src/pycpio/cpio/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,13 +180,15 @@
 
     def __init__(self, data: bytes, header, *args, **kwargs):
         self.header = header
         self.hash = None
         self.data = data if data is not None else b''
 
     def __str__(self):
-        return f"\n{self.header}\nSHA256: {self.hash}\n{self.__class__.__name__}"
+        out_str = f"{self.__class__.__name__} {self.header}"
+        out_str += f"\nSHA256: {self.hash} " if self.hash else " "
+        return out_str
 
     def __bytes__(self):
         """ Convert the data to bytes """
         return bytes(self.header) + self.data
```

### Comparing `pycpio-0.9.2/src/pycpio/cpio/dir.py` & `pycpio-1.0.0/src/pycpio/cpio/dir.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.9.2/src/pycpio/cpio/file.py` & `pycpio-1.0.0/src/pycpio/cpio/file.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.9.2/src/pycpio/cpio/symlink.py` & `pycpio-1.0.0/src/pycpio/cpio/symlink.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.9.2/src/pycpio/header/cpioheader.py` & `pycpio-1.0.0/src/pycpio/header/cpioheader.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,23 +172,29 @@
         """ Returns a string representation of the object. """
         from datetime import datetime
 
         out_str = f"[{int(self.ino, 16)}] "
         out_str += "Header:\n" if not hasattr(self, 'name') else f"{self.name}:\n"
 
         for attr in self.structure:
-            if attr in ['ino', 'mode', 'devmajor', 'devminor',
+            if attr in ['ino', 'mode', 'devmajor', 'devminor', 'uid', 'gid',
                         'rdevmajor', 'rdevminor', 'namesize', 'filesize', 'check']:
                 continue
             elif attr == 'nlink':
                 if int(self.nlink, 16) > 1:
                     out_str += f"    {attr}: {int(self.nlink, 16)}\n"
             elif attr == 'magic':
-                out_str += f"    {attr}: {self.magic}\n"
+                if self.logger.level < 20:
+                    out_str += f"    {attr}: {self.magic}\n"
+                else:
+                    continue
             elif attr == 'mtime':
-                out_str += f"    {attr}: {datetime.fromtimestamp(int(self.mtime, 16))}\n"
+                if self.logger.level < 20:
+                    out_str += f"    {attr}: {datetime.fromtimestamp(int(self.mtime, 16))}\n"
+                else:
+                    continue
             else:
-                out_str += f"    {attr}: {int(getattr(self, attr), 16)}\n"
+                out_str += f"    {attr}: {int(getattr(self, attr), 16)}"
 
-        out_str += f"    Permissions: {print_permissions(self.permissions)}\n"
+        out_str += f"    Permissions: {print_permissions(self.permissions)} {int(self.uid)} {int(self.gid)}"
         return out_str
```

### Comparing `pycpio-0.9.2/src/pycpio/header/header_funcs.py` & `pycpio-1.0.0/src/pycpio/header/header_funcs.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.9.2/src/pycpio/main.py` & `pycpio-1.0.0/src/pycpio/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                  {'flags': ['-u', '--set-owner'], 'action': 'store', 'help': 'set UID on all files', 'type': int, 'dest': 'uid'},
                  {'flags': ['-g', '--set-group'], 'action': 'store', 'help': 'set GID on all files', 'type': int, 'dest': 'gid'},
                  {'flags': ['-m', '--set-mode'], 'action': 'store', 'help': 'set mode on all files', 'type': int, 'dest': 'mode'},
                  {'flags': ['-o', '--output'], 'help': 'output file'},
                  {'flags': ['-l', '--list'], 'action': 'store_true', 'help': 'list CPIO contents'},
                  {'flags': ['-p', '--print'], 'action': 'store_true', 'help': 'print CPIO contents'}]
 
-    args, logger = get_args_n_logger(package=__package__, description='PyCPIO', arguments=arguments)
+    args, logger = get_args_n_logger(package=__package__, description='PyCPIO', arguments=arguments, drop_default=True)
     kwargs = get_kwargs_from_args(args, logger=logger)
 
     c = PyCPIO(**kwargs)
     if 'input' in args:
         c.read_cpio_file(Path(args.input))
 
     if 'rm' in args:
```

### Comparing `pycpio-0.9.2/src/pycpio/masks/modes.py` & `pycpio-1.0.0/src/pycpio/masks/modes.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.9.2/src/pycpio/masks/permissions.py` & `pycpio-1.0.0/src/pycpio/masks/permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,11 +49,11 @@
         # Check if the permission is in the set, if so add it to the output
         if permission in passed_perms:
             out += permission.name[0].lower()
         else:
             out += "-"
 
         if permission.name[0].lower() == 'x':
-            out += " "
+            out += "-"
 
     return out.rstrip()
```

### Comparing `pycpio-0.9.2/src/pycpio/pycpio.py` & `pycpio-1.0.0/src/pycpio/pycpio.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.9.2/src/pycpio/reader/reader.py` & `pycpio-1.0.0/src/pycpio/reader/reader.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.9.2/src/pycpio/writer/writer.py` & `pycpio-1.0.0/src/pycpio/writer/writer.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.9.2/src/pycpio.egg-info/PKG-INFO` & `pycpio-1.0.0/src/pycpio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pycpio
-Version: 0.9.2
+Version: 1.0.0
 Summary: A Python library for reading and writing cpio archives.
 Author-email: Desultory <dev@pyl.onl>
 Project-URL: Homepage, https://github.com/desultory/pycpio
 Project-URL: Issues, https://github.com/desultory/pycpio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: zenlib>=1.7.3
+Requires-Dist: zenlib>=2.0.0
 
 # pycpio
 
 A library for working with CPIO files using python
 
 In active development
```

### Comparing `pycpio-0.9.2/src/pycpio.egg-info/SOURCES.txt` & `pycpio-1.0.0/src/pycpio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

