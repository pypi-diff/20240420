# Comparing `tmp/ultimapy-0.0.8.tar.gz` & `tmp/ultimapy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ultimapy-0.0.8.tar", last modified: Thu Aug  1 07:13:29 2019, max compression
+gzip compressed data, was "dist/ultimapy-0.0.9.tar", last modified: Fri Aug  2 11:24:39 2019, max compression
```

## Comparing `ultimapy-0.0.8.tar` & `ultimapy-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2019-08-01 07:13:29.000000 ultimapy-0.0.8/
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2019-08-01 07:13:29.000000 ultimapy-0.0.8/ultimapy.egg-info/
--rw-r--r--   0 jack      (1000) jack      (1000)       29 2019-08-01 07:13:29.000000 ultimapy-0.0.8/ultimapy.egg-info/requires.txt
--rw-r--r--   0 jack      (1000) jack      (1000)        1 2019-08-01 07:13:29.000000 ultimapy-0.0.8/ultimapy.egg-info/dependency_links.txt
--rw-r--r--   0 jack      (1000) jack      (1000)        9 2019-08-01 07:13:29.000000 ultimapy-0.0.8/ultimapy.egg-info/top_level.txt
--rw-r--r--   0 jack      (1000) jack      (1000)      545 2019-08-01 07:13:29.000000 ultimapy-0.0.8/ultimapy.egg-info/SOURCES.txt
--rw-r--r--   0 jack      (1000) jack      (1000)     3803 2019-08-01 07:13:29.000000 ultimapy-0.0.8/ultimapy.egg-info/PKG-INFO
--rw-r--r--   0 jack      (1000) jack      (1000)      703 2019-08-01 07:13:26.000000 ultimapy-0.0.8/setup.py
--rw-r--r--   0 jack      (1000) jack      (1000)     2860 2019-08-01 06:56:44.000000 ultimapy-0.0.8/README.md
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2019-08-01 07:13:29.000000 ultimapy-0.0.8/ultimapy/
--rw-rw-r--   0 jack      (1000) jack      (1000)       66 2019-08-01 06:21:25.000000 ultimapy-0.0.8/ultimapy/__init__.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2019-08-01 07:13:29.000000 ultimapy-0.0.8/ultimapy/sdk/
--rw-rw-r--   0 jack      (1000) jack      (1000)      233 2019-08-01 06:23:54.000000 ultimapy-0.0.8/ultimapy/sdk/__init__.py
--rw-r--r--   0 jack      (1000) jack      (1000)     2280 2019-08-01 06:34:52.000000 ultimapy-0.0.8/ultimapy/sdk/skills.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1636 2019-08-01 06:10:23.000000 ultimapy-0.0.8/ultimapy/sdk/utils.py
--rw-r--r--   0 jack      (1000) jack      (1000)     3412 2019-08-01 06:37:06.000000 ultimapy-0.0.8/ultimapy/sdk/tile_data.py
--rw-r--r--   0 jack      (1000) jack      (1000)      855 2019-08-01 06:10:23.000000 ultimapy-0.0.8/ultimapy/sdk/verdata.py
--rw-r--r--   0 jack      (1000) jack      (1000)     2875 2019-08-01 06:27:18.000000 ultimapy-0.0.8/ultimapy/sdk/file_index.py
--rw-r--r--   0 jack      (1000) jack      (1000)     8848 2019-08-01 06:08:14.000000 ultimapy-0.0.8/ultimapy/sdk/animations.py
--rw-r--r--   0 jack      (1000) jack      (1000)     2570 2019-08-01 06:39:18.000000 ultimapy-0.0.8/ultimapy/sdk/ascii_font.py
--rw-r--r--   0 jack      (1000) jack      (1000)     4402 2019-08-01 06:10:23.000000 ultimapy-0.0.8/ultimapy/sdk/bodies.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     2817 2019-08-01 06:36:31.000000 ultimapy-0.0.8/ultimapy/sdk/gumps.py
--rw-r--r--   0 jack      (1000) jack      (1000)     7271 2019-07-30 10:34:13.000000 ultimapy-0.0.8/ultimapy/sdk/art.py
--rw-r--r--   0 jack      (1000) jack      (1000)     2725 2019-08-01 06:10:23.000000 ultimapy-0.0.8/ultimapy/sdk/hues.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2019-08-01 07:13:29.000000 ultimapy-0.0.8/ultimapy/settings/
--rw-rw-r--   0 jack      (1000) jack      (1000)      118 2019-08-01 06:16:34.000000 ultimapy-0.0.8/ultimapy/settings/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1275 2019-08-01 06:43:20.000000 ultimapy-0.0.8/ultimapy/settings/settings.py
--rw-r--r--   0 jack      (1000) jack      (1000)       38 2019-08-01 07:13:29.000000 ultimapy-0.0.8/setup.cfg
--rw-r--r--   0 jack      (1000) jack      (1000)     3803 2019-08-01 07:13:29.000000 ultimapy-0.0.8/PKG-INFO
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2019-08-02 11:24:39.000000 ultimapy-0.0.9/
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2019-08-02 11:24:39.000000 ultimapy-0.0.9/ultimapy.egg-info/
+-rw-r--r--   0 jack      (1000) jack      (1000)       29 2019-08-02 11:24:39.000000 ultimapy-0.0.9/ultimapy.egg-info/requires.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)        1 2019-08-02 11:24:39.000000 ultimapy-0.0.9/ultimapy.egg-info/dependency_links.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)        9 2019-08-02 11:24:39.000000 ultimapy-0.0.9/ultimapy.egg-info/top_level.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)      545 2019-08-02 11:24:39.000000 ultimapy-0.0.9/ultimapy.egg-info/SOURCES.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)     3803 2019-08-02 11:24:39.000000 ultimapy-0.0.9/ultimapy.egg-info/PKG-INFO
+-rw-r--r--   0 jack      (1000) jack      (1000)      703 2019-08-02 11:24:10.000000 ultimapy-0.0.9/setup.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     2860 2019-08-01 07:15:22.000000 ultimapy-0.0.9/README.md
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2019-08-02 11:24:39.000000 ultimapy-0.0.9/ultimapy/
+-rw-r--r--   0 jack      (1000) jack      (1000)       66 2019-08-01 07:15:22.000000 ultimapy-0.0.9/ultimapy/__init__.py
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2019-08-02 11:24:39.000000 ultimapy-0.0.9/ultimapy/sdk/
+-rw-r--r--   0 jack      (1000) jack      (1000)      233 2019-08-01 07:15:22.000000 ultimapy-0.0.9/ultimapy/sdk/__init__.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     2280 2019-08-01 07:15:22.000000 ultimapy-0.0.9/ultimapy/sdk/skills.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     1636 2019-08-01 07:15:22.000000 ultimapy-0.0.9/ultimapy/sdk/utils.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     3573 2019-08-02 10:04:09.000000 ultimapy-0.0.9/ultimapy/sdk/tile_data.py
+-rw-r--r--   0 jack      (1000) jack      (1000)      855 2019-08-01 07:15:22.000000 ultimapy-0.0.9/ultimapy/sdk/verdata.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     3017 2019-08-02 11:23:33.000000 ultimapy-0.0.9/ultimapy/sdk/file_index.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     8871 2019-08-02 11:14:18.000000 ultimapy-0.0.9/ultimapy/sdk/animations.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     2570 2019-08-01 07:15:22.000000 ultimapy-0.0.9/ultimapy/sdk/ascii_font.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     4402 2019-08-01 07:15:22.000000 ultimapy-0.0.9/ultimapy/sdk/bodies.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     2817 2019-08-01 07:15:22.000000 ultimapy-0.0.9/ultimapy/sdk/gumps.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     7271 2019-08-01 07:15:22.000000 ultimapy-0.0.9/ultimapy/sdk/art.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     2725 2019-08-01 07:15:22.000000 ultimapy-0.0.9/ultimapy/sdk/hues.py
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2019-08-02 11:24:39.000000 ultimapy-0.0.9/ultimapy/settings/
+-rw-r--r--   0 jack      (1000) jack      (1000)      118 2019-08-01 07:15:22.000000 ultimapy-0.0.9/ultimapy/settings/__init__.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     1275 2019-08-01 07:15:22.000000 ultimapy-0.0.9/ultimapy/settings/settings.py
+-rw-r--r--   0 jack      (1000) jack      (1000)       38 2019-08-02 11:24:39.000000 ultimapy-0.0.9/setup.cfg
+-rw-r--r--   0 jack      (1000) jack      (1000)     3803 2019-08-02 11:24:39.000000 ultimapy-0.0.9/PKG-INFO
```

### Comparing `ultimapy-0.0.8/ultimapy.egg-info/SOURCES.txt` & `ultimapy-0.0.9/ultimapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ultimapy-0.0.8/ultimapy.egg-info/PKG-INFO` & `ultimapy-0.0.9/ultimapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultimapy
-Version: 0.0.8
+Version: 0.0.9
 Summary: UltimaPy - Extract information and images from the UO client files
 Home-page: https://github.com/jackuoll/ultima-py
 Author: Jack Ward
 Author-email: jackward84@gmail.com
 License: Beerware
 Description: [![PyPI version](https://badge.fury.io/py/ultimapy.svg)](https://badge.fury.io/py/ultimapy)
```

### Comparing `ultimapy-0.0.8/setup.py` & `ultimapy-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ultimapy",
-    version="0.0.8",
+    version="0.0.9",
     author="Jack Ward",
     author_email="jackward84@gmail.com",
     description="UltimaPy - Extract information and images from the UO client files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jackuoll/ultima-py",
     packages=setuptools.find_packages(),
```

### Comparing `ultimapy-0.0.8/README.md` & `ultimapy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ultimapy-0.0.8/ultimapy/sdk/skills.py` & `ultimapy-0.0.9/ultimapy/sdk/skills.py`

 * *Files identical despite different names*

### Comparing `ultimapy-0.0.8/ultimapy/sdk/utils.py` & `ultimapy-0.0.9/ultimapy/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ultimapy-0.0.8/ultimapy/sdk/tile_data.py` & `ultimapy-0.0.9/ultimapy/sdk/tile_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ultimapy.settings import ultima_file_path
 
+import functools
 from struct import unpack
 from .art import Art
 
 
 class TileData:
     loaded = False
     land_header = [0] * 512
@@ -63,28 +64,33 @@
     def from_stream(cls, stream):
         return NewLandMul(*unpack('iih20s', stream.read(4 + 4 + 2 + 20)))
 
 
 class OldItemMul:
     size = 4 + 1 * 9 + 2 * 2 + 20
 
+    @functools.lru_cache()
+    def partial_hue(self):
+        return self.flags & 0x00040000
+
     def __init__(self, flags, weight, quality, misc, unk2, amt, anim, unk3, hue, stacking_offset, value, height, name):
         self.flags = flags
         self.weight = int(weight)
         self.quality = int(quality)
         self.misc = misc
         self.unk2 = int(unk2)
         self.quantity = int(amt)
         self.animation = anim
         self.unk3 = int(unk3)
         self.hue = int(hue)
         self.stacking_offset = int(stacking_offset)
         self.value = int(value)
         self.height = int(height)
         self.name = name.decode('cp1252')
+        self.name = self.name.replace("\x00", "")
 
     @classmethod
     def from_stream(cls, stream):
         return OldItemMul(*unpack('ibbhbbhbbbbb20s', stream.read(cls.size)))
 
 
 class NewItemMul(OldItemMul):
```

### Comparing `ultimapy-0.0.8/ultimapy/sdk/verdata.py` & `ultimapy-0.0.9/ultimapy/sdk/verdata.py`

 * *Files identical despite different names*

### Comparing `ultimapy-0.0.8/ultimapy/sdk/file_index.py` & `ultimapy-0.0.9/ultimapy/sdk/file_index.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ultimapy.settings import ultima_file_path
-from io import FileIO
+from io import BytesIO
 from struct import unpack
 from .verdata import Verdata
 
 
 class FileIndex:
     """
         - No current UOP support.
@@ -13,17 +13,17 @@
         - Valid() method not implemented
         - Should be refactored -- files can be non existent.
     """
     def __init__(self, idx_filename, mul_filename, length, file_idx):
         try:
             index_file = None
             self.index_file_path = ultima_file_path(idx_filename)
-            index_file = FileIO(self.index_file_path, 'rb')
+            index_file = open(self.index_file_path, 'rb')
             self.mul_file_path = ultima_file_path(mul_filename)
-            mul_file = FileIO(self.mul_file_path, 'rb')
+            mul_file = open(self.mul_file_path, 'rb')
         except FileNotFoundError:
             print(f"No file for index {idx_filename if not index_file else mul_filename}")
             return
         idx_file_bytes = len(index_file.read())
         index_file.seek(0)
         count = int(idx_file_bytes / 12)
         length = length or count
@@ -54,22 +54,25 @@
         extra = entry.extra
         patched = False
 
         if (entry.length & (1 << 31)) != 0:
             patched = True
             stream = Verdata.FILE
             stream.seek(entry.lookup)
-            return stream, length, extra, patched
+            return BytesIO(stream.read(length)), length, extra, patched
 
         stream = self.stream
         if not self.stream:# or self.index_length < entry.lookup:
             return null_return
+
+        byte_stream = None  # return nothing if is validation
         if not is_validation:
             stream.seek(entry.lookup)
-        return stream, length, extra, patched
+            byte_stream = BytesIO(stream.read(length))
+        return byte_stream, length, extra, patched
 
     def valid(self, index):
         stream, length, extra, patched = self.seek(index, is_validation=True)
         return stream is not None, length, extra, patched
 
 
 class Entry3D:
```

### Comparing `ultimapy-0.0.8/ultimapy/sdk/animations.py` & `ultimapy-0.0.9/ultimapy/sdk/animations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from io import BytesIO
 from struct import unpack
 
 from PIL import Image
 
 from .bodies import *
 from .file_index import FileIndex
 from .tile_data import item_data
```

### Comparing `ultimapy-0.0.8/ultimapy/sdk/ascii_font.py` & `ultimapy-0.0.9/ultimapy/sdk/ascii_font.py`

 * *Files identical despite different names*

### Comparing `ultimapy-0.0.8/ultimapy/sdk/bodies.py` & `ultimapy-0.0.9/ultimapy/sdk/bodies.py`

 * *Files identical despite different names*

### Comparing `ultimapy-0.0.8/ultimapy/sdk/gumps.py` & `ultimapy-0.0.9/ultimapy/sdk/gumps.py`

 * *Files identical despite different names*

### Comparing `ultimapy-0.0.8/ultimapy/sdk/art.py` & `ultimapy-0.0.9/ultimapy/sdk/art.py`

 * *Files identical despite different names*

### Comparing `ultimapy-0.0.8/ultimapy/sdk/hues.py` & `ultimapy-0.0.9/ultimapy/sdk/hues.py`

 * *Files identical despite different names*

### Comparing `ultimapy-0.0.8/ultimapy/settings/settings.py` & `ultimapy-0.0.9/ultimapy/settings/settings.py`

 * *Files identical despite different names*

### Comparing `ultimapy-0.0.8/PKG-INFO` & `ultimapy-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultimapy
-Version: 0.0.8
+Version: 0.0.9
 Summary: UltimaPy - Extract information and images from the UO client files
 Home-page: https://github.com/jackuoll/ultima-py
 Author: Jack Ward
 Author-email: jackward84@gmail.com
 License: Beerware
 Description: [![PyPI version](https://badge.fury.io/py/ultimapy.svg)](https://badge.fury.io/py/ultimapy)
```

