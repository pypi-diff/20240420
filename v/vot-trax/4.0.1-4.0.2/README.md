# Comparing `tmp/vot-trax-4.0.1.tar.gz` & `tmp/vot-trax-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vot-trax-4.0.1.tar", last modified: Tue May 23 12:36:22 2023, max compression
+gzip compressed data, was "vot-trax-4.0.2.tar", last modified: Sat Apr 20 15:43:40 2024, max compression
```

## Comparing `vot-trax-4.0.1.tar` & `vot-trax-4.0.2.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-23 12:36:22.460717 vot-trax-4.0.1/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1053 2023-05-23 12:36:22.460717 vot-trax-4.0.1/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      544 2023-05-04 21:26:46.047421 vot-trax-4.0.1/README.rst
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        6 2023-05-23 12:34:41.272537 vot-trax-4.0.1/VERSION
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3126 2023-05-04 21:26:06.363611 vot-trax-4.0.1/setup.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-23 12:36:22.460717 vot-trax-4.0.1/trax/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9243 2023-05-23 12:13:30.166442 vot-trax-4.0.1/trax/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    54378 2023-05-04 21:26:46.067421 vot-trax-4.0.1/trax/_ctypes.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6953 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/base64.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      335 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/base64.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4548 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/buffer.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7944 2023-05-23 12:13:16.466424 vot-trax-4.0.1/trax/client.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1562 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/debug.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      971 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/debug.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8029 2023-05-04 21:26:46.067421 vot-trax-4.0.1/trax/image.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    23442 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/message.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1810 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/message.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    30473 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/region.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3364 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/region.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8687 2023-05-04 21:26:46.067421 vot-trax-4.0.1/trax/region.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5967 2023-05-04 21:26:46.067421 vot-trax-4.0.1/trax/server.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14754 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/strmap.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12968 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/strmap.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    58455 2023-05-23 12:11:45.642304 vot-trax-4.0.1/trax/trax.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    36170 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/trax.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    24834 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/traxpp.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:43:40.277926 vot-trax-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-20 15:43:12.000000 vot-trax-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-20 15:43:40.277926 vot-trax-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-20 15:43:12.000000 vot-trax-4.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 15:43:12.000000 vot-trax-4.0.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 15:43:40.277926 vot-trax-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-20 15:43:12.000000 vot-trax-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:43:40.277926 vot-trax-4.0.2/trax/
+-rw-r--r--   0 runner    (1001) docker     (127)    15802 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54274 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/base64.c
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/base64.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/debug.c
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/debug.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23442 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/message.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/message.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30473 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/region.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/region.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/strmap.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12968 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/strmap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    58455 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/trax.c
+-rw-r--r--   0 runner    (1001) docker     (127)    36170 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/trax.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24833 2024-04-20 15:43:12.000000 vot-trax-4.0.2/trax/traxpp.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:43:40.277926 vot-trax-4.0.2/vot_trax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-20 15:43:40.000000 vot-trax-4.0.2/vot_trax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-20 15:43:40.000000 vot-trax-4.0.2/vot_trax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 15:43:40.000000 vot-trax-4.0.2/vot_trax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 15:43:40.000000 vot-trax-4.0.2/vot_trax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 15:43:40.000000 vot-trax-4.0.2/vot_trax.egg-info/top_level.txt
```

### Comparing `vot-trax-4.0.1/PKG-INFO` & `vot-trax-4.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: vot-trax
-Version: 4.0.1
+Version: 4.0.2
 Summary: TraX protocol reference implementation wrapper for Python
 Home-page: https://github.com/votchallenge/trax/
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
 Description: 
         `Visual Tracking eXchange protocol <http://prints.vicos.si/publications/311/>`_ is a simple protocol that enables easier evaluation of computer vision tracking algorithms. The basic idea is that a tracker communicates with the evaluation software using a set of text commands over the (standard) input/output streams or TCP sockets. 
         
         This package contains a Python wrapper to C library (using CTypes) available in the `support/python` directory. More information and source code available at `Github <https://github.com/votchallenge/trax/>`_.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
+Description-Content-Type: text/markdown
```

### Comparing `vot-trax-4.0.1/README.rst` & `vot-trax-4.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.1/setup.py` & `vot-trax-4.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python
 
 import os, sys, glob
-from distutils.core import setup, Extension
+
+from setuptools import setup, Extension
+
+#from distutils.core import setup, Extension
 from distutils.command.build_ext import build_ext
 
 root = os.path.abspath(os.path.dirname(__file__))
 platform = os.getenv("TRAX_PYTHON_PLATFORM", sys.platform)
 
 if platform.startswith('linux'):
     library_prefix = 'lib'
@@ -49,14 +52,15 @@
         def get_tag(self):
             python, abi, plat = _bdist_wheel.get_tag(self)
             # We don't contain any python source
             python, abi = 'py2.py3', 'none'
             return python, abi, plat
 
 except ImportError:
+    print("Warning: wheel package not found, bdist_wheel command will not be available")
     bdist_wheel = None
 try:
     with open(os.path.join(root, "VERSION"), encoding='utf-8') as fp:
         VERSION = fp.readline().strip()
 
 except IOError:
     VERSION = os.getenv("TRAX_VERSION", "unknown")
@@ -68,20 +72,21 @@
     long_description = ""
 
 
 varargs = dict()
 
 if os.path.isfile(os.path.join("trax", library_prefix + "trax" + library_suffix)):
     varargs["package_data"] = {"trax" : [library_prefix + "trax" + library_suffix]}
-    varargs["cmdclass"] = {'bdist_wheel': bdist_wheel}
+    varargs["cmdclass"] = {'bdist_wheel': bdist_wheel, 'build_ext': build_ext_ctypes}
     varargs["setup_requires"] = ['wheel']
 elif os.path.isfile(os.path.join("trax", "trax.c")):
     sources = glob.glob("trax/*.c") + glob.glob("trax/*.cpp")
     varargs["ext_modules"] = [CTypes("trax.trax", sources=sources, define_macros=[("trax_EXPORTS", "1")])]
-    varargs["cmdclass"] = {'build_ext': build_ext_ctypes}
+    varargs["cmdclass"] = { 'build_ext': build_ext_ctypes, 'bdist_wheel': bdist_wheel}
+    varargs["setup_requires"] = ['wheel']
 
 setup(name='vot-trax',
     version=VERSION,
     description='TraX protocol reference implementation wrapper for Python',
     author='Luka Cehovin Zajc',
     author_email='luka.cehovin@gmail.com',
     long_description=long_description,
```

### Comparing `vot-trax-4.0.1/trax/__init__.py` & `vot-trax-4.0.2/trax/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,291 +1,288 @@
+"""
+Bindings for the TraX client object.
+"""
 
-import sys, os
-import traceback
-import weakref
-from ctypes import py_object, c_void_p, cast, byref, POINTER
-
-from ._ctypes import \
-    trax_properties_enumerate, trax_properties_create, trax_enumerator, \
-    trax_properties_get, trax_properties_set, trax_object_list, \
-    trax_image_release, trax_region_release, trax_object_list_release, \
-    trax_cleanup, trax_properties_release, trax_image_list_release, \
-    struct_trax_handle, struct_trax_image, struct_trax_image_list, \
-    struct_trax_properties, struct_trax_object_list, POINTER
-
-trax_image_p = POINTER(struct_trax_image)
-trax_image_list_p = POINTER(struct_trax_image_list)
-trax_region_p = c_void_p
-trax_object_list_p = POINTER(trax_object_list)
-trax_properties_p = POINTER(struct_trax_properties)
-class TraxException(Exception):
-    pass
-
-class TraxStatus(object):
-    """ The message type container class """
-    ERROR = "error"
-    OK = "ok"
-    HELLO = "hello"
-    INITIALIZE = "initialize"
-    FRAME = "frame"
-    QUIT = "quit"
-    STATE = "state"
-
-    @staticmethod
-    def decode(intcode):
-        if intcode == -1:
-            return TraxStatus.ERROR
-        elif intcode == 0:
-            return TraxStatus.OK
-        elif intcode == 1:
-            return TraxStatus.HELLO
-        elif intcode == 2:
-            return TraxStatus.INITIALIZE
-        elif intcode == 3:
-            return TraxStatus.FRAME
-        elif intcode == 4:
-            return TraxStatus.QUIT
-        elif intcode == 5:
-            return TraxStatus.STATE
-
-class Logger(object):
-
-    def __init__(self):
-        self._interrupted = False
-
-    def __call__(self, buffer, length, _):
-        try:
-            if not buffer:
-                return
-            message = buffer[:length].decode("utf-8")
-            self.handle(message)
-        except KeyboardInterrupt:
-            self._interrupted = True
-
-    def handle(self, message):
-        pass
-
-    @property
-    def interrupted(self):
-        return self._interrupted
-
-class ConsoleLogger(Logger):
-
-    def handle(self, message):
-        print(message, end='')
-
-class FileLogger(Logger):
-
-    def __init__(self, filename):
-        super().__init__()
-        os.makedirs(os.path.dirname(filename), exist_ok=True)
-        self._fp = open(filename, "w")
-
-    def handle(self, message):
-        self._fp.write(message)
-
-    def __del__(self):
-        self._fp.close()
-
-class ProxyLogger(Logger):
-
-    def __init__(self, hook):
-        super().__init__()
-        self._hook = hook
-
-    def handle(self, message):
-        self._hook(message)
-
-def _run_finalizer(ref):
-    """Internal weakref callback to run finalizers"""
-    del _finalize_refs[id(ref)]
-    finalizer = ref.finalizer
-    item = ref.item
-    if finalizer:
-        try:
-            finalizer(item)
-        except Exception:
-            print("Exception {}:".format(finalizer))
-            traceback.print_exc()
-
-class OwnerRef(weakref.ref):
-
-    __slots__ = "item", "finalizer"
-
-    def __new__(type, ob, item, finalizer):
-        return weakref.ref.__new__(type, ob, _run_finalizer)
-
-    def __init__(self, owner, item, callback):
-        super(OwnerRef, self).__init__(owner)
-        self.item = item
-        self.finalizer = callback
-
-_finalize_refs = {}
+__all__ = \
+    ['Client']
 
-def _track_for_finalization(owner, item, finalizer):
-    """Register an object for finalization.
+import time
 
-    ``owner`` is the the object which is responsible for ``item``.
-    ``finalizer`` will be called with ``item`` as its only argument when
-    ``owner`` is destroyed by the garbage collector.
-    """
-    ref = OwnerRef(owner, item, finalizer)
-    _finalize_refs[id(ref)] = ref
-    return ref
+from ctypes import byref, c_int
 
-class Wrapper(object):
+from . import TraxException, TraxStatus, Properties, HandleWrapper, \
+    ConsoleLogger, FileLogger, ProxyLogger, trax_object_list_p
+    
+from . import wrap_images, wrap_objects, wrap_object_list, ObjectListWrapper
 
-    def __init__(self, ctype, reference, finalizer):
-        if not reference is None:
-            if not isinstance(reference, ctype):
-                raise RuntimeError("Not a ctype {}".format(type(ctype)))
-            self.ref = _track_for_finalization(self, reference, finalizer)
+from ._ctypes import \
+    trax_client_initialize, \
+    trax_client_wait, trax_client_frame, \
+    trax_client_setup_file, trax_client_setup_socket, \
+    trax_logger_setup, trax_logger, trax_get_parameter, \
+    trax_terminate, trax_get_error, trax_is_alive, TRAX_PARAMETER_MULTIOBJECT
+
+from .image import ImageChannel, Image
+from .region import Region
+
+class Client(object):
+    """ TraX client object. """
+
+    def __init__(self, stream=None, timeout=30, log=False):
+        """ Create a new client object.
+        
+        Args:
+            stream: A tuple (host, port) or a port number to connect to.
+            timeout: A timeout in seconds.
+            log: A boolean value or a string. If True, the log is written to the console. If False, no log is written. If a string, the log is written to the file with the given name.
+        """
+
+        if isinstance(log, bool) and log:
+            self._logger = ConsoleLogger()
+        elif isinstance(log, str):
+            self._logger = FileLogger(log)
+        elif callable(log):
+            self._logger = ProxyLogger(log)
         else:
-            self.ref = None
-
-    @property
-    def reference(self):
-        if not self.ref:
-            return None
-        return self.ref.item
-
-    def __nonzero__(self):
-        return not self.ref is None
-
-def _debug_wrapper(cb, message):
-    def wrapper(*args, **kwargs):
-        print(message, args, kwargs)
-        cb(*args, **kwargs)
-    return wrapper
-class ImageWrapper(Wrapper):
-
-    def __init__(self, reference, owner=True):
-        super().__init__(POINTER(struct_trax_image), reference, lambda x: trax_image_release(byref(x)) if owner else None)
-
-class ImageListWrapper(Wrapper):
-
-    def __init__(self, reference, owner=True):
-        super().__init__(POINTER(struct_trax_image_list), reference, lambda x: trax_image_list_release(byref(x)) if owner else None)
-
-class ObjectListWrapper(Wrapper):
-
-    def __init__(self, reference, owner=True):
-        super().__init__(POINTER(struct_trax_object_list), reference, lambda x: trax_object_list_release(byref(x)) if owner else None)
-
-class RegionWrapper(Wrapper):
+            self._logger = None
 
-    def __init__(self, reference, owner=True):
-        super().__init__(c_void_p, reference, lambda x: trax_region_release(byref(cast(x, c_void_p))) if owner else None)
+        self._clogger = trax_logger(self._logger) if not self._logger is None else None
 
-class PropertiesWrapper(Wrapper):
+        logger = trax_logger_setup(self._clogger, 0, 0)
 
-    def __init__(self, reference, owner=True):
-        super().__init__(POINTER(struct_trax_properties), reference, lambda x: trax_properties_release(byref(x)) if owner else None)
+        if isinstance(stream, tuple):
 
-class HandleWrapper(Wrapper):
+            assert(len(stream) == 2)
 
-    def __init__(self, reference, owner=True):
-        super().__init__(POINTER(struct_trax_handle), reference, lambda x: trax_cleanup(byref(x)) if owner else None)
+            handle = trax_client_setup_file(
+                stream[1],
+                stream[0],
+                logger)
 
-def wrap_image_list(list):
-    from ._ctypes import trax_image_list_get
+        elif isinstance(stream, int):
 
-    channels = [ImageChannel.COLOR, ImageChannel.DEPTH, ImageChannel.IR]
-    wrapped = {}
+            handle = trax_client_setup_socket(
+                stream,
+                timeout,
+                logger)
 
-    for channel in channels:
-        img = trax_image_list_get(list, ImageChannel.encode(channel))
-        if not img:
-            continue
-        wrapped[channel] = Image.wrap(img)
-
-    return wrapped
-
-def wrap_object_list(list):
-    from ._ctypes import trax_object_list_count, \
-        trax_object_list_get, trax_object_list_properties, \
-        trax_region_clone
-    import ctypes
+        else:
+            raise TraxException("Invalid parameters")
 
-    objects = []
-    for i in range(trax_object_list_count(list)):
-        region = trax_object_list_get(list, i)
-        properties = Properties(trax_object_list_properties(list, i), False).dict()
-        r = trax_region_clone(region)
-        objects.append((Region.wrap(ctypes.cast(r, c_void_p)), properties))
-    return objects
+        if self._logger and self._logger.interrupted:
+            raise KeyboardInterrupt("Interrupted by user in log callback")
 
+        if not handle:
+            raise TraxException("Unable to connect to tracker")
 
-def wrap_images(images):
-    from ._ctypes import trax_image_list_create, trax_image_list_set
+        if trax_is_alive(handle) == 0:
+            message = trax_get_error(handle.reference)
+            message = message.decode('utf-8') if not message is None else "Unknown"
+            raise TraxException("Exception when connecting to tracker: {}".format(message))
 
-    channels = [ImageChannel.COLOR, ImageChannel.DEPTH, ImageChannel.IR]
-    tlist = ImageListWrapper(trax_image_list_create())
+        self._handle = HandleWrapper(handle)
 
-    for channel in channels:
-        if not channel in images:
-            continue
+        metadata = self._handle.reference.contents.metadata
 
-        trax_image_list_set(tlist.reference, images[channel].reference, ImageChannel.encode(channel))
+        self._format_region = Region.decode_list(metadata.contents.format_region)
+        self._format_image = Image.decode_list(metadata.contents.format_image)
+        self._channels = ImageChannel.decode_list(metadata.contents.channels)
+        
+        self._tracker_name = metadata.contents.tracker_name.decode("utf-8") \
+            if not metadata.contents.tracker_name is None else ""
+        self._tracker_family = metadata.contents.tracker_family.decode("utf-8") \
+            if not metadata.contents.tracker_family is None else ""
+        self._tracker_description = metadata.contents.tracker_description.decode("utf-8") \
+            if not metadata.contents.tracker_description is None else ""
 
-    return tlist
+        custom = Properties(metadata.contents.custom, False)
 
-def wrap_objects(objects):
-    from ._ctypes import trax_properties_append, trax_object_list_set, \
-         trax_object_list_properties, trax_object_list_create
-    tlist = ObjectListWrapper(trax_object_list_create(len(objects)))
+        self._custom = custom.dict()
 
-    for i, (region, properties) in enumerate(objects):
-        properties =  Properties(properties, False)
-        trax_object_list_set(tlist.reference, i, region.reference)
-        trax_properties_append(trax_object_list_properties(tlist.reference, i), properties.reference, 0)
+        value = c_int(value=0)   
+        trax_get_parameter(handle, TRAX_PARAMETER_MULTIOBJECT, byref(value))
 
-    return tlist
-class Properties(object):
+        self._custom["multiobject"] = bool(value.value)
 
-    def __init__(self, data=None, owner=True):
-        if not data:
-            self._ref = PropertiesWrapper(trax_properties_create())
-        elif isinstance(data, trax_properties_p):
-            self._ref = PropertiesWrapper(data, owner)
-        elif isinstance(data, dict):
-            self._ref = PropertiesWrapper(trax_properties_create())
-            for key, value in data.items():
-                trax_properties_set(self._ref.reference, key.encode('utf8'), str(value).encode('utf8'))
+    @property
+    def channels(self):
+        """ List of supported channels.
+        
+        Returns:
+            A list of ImageChannel objects.
+        """
+        return self._channels
 
-    def copy(self, source: "Properties"):
-        for k, v in source.dict().items():
-            self[k] = v
+    @property
+    def image_formats(self):
+        return self._format_image
 
     @property
-    def reference(self):
-        return self._ref.reference
+    def region_formats(self):
+        """ List of supported region formats.
+        
+        Returns:
+            A list of Region objects.
+        """
+        return self._format_region
 
-    def __getitem__(self, key):
-        return trax_properties_get(self._ref.reference, key)
+    @property
+    def tracker_name(self) -> str:
+        """ Tracker name.
+        
+        Returns:
+            A string with the tracker name.
+        """
+        return self._tracker_name
 
-    def __setitem__(self, key, value):
-        trax_properties_set(self._ref.reference, key.encode('utf8'), str(value).encode('utf8'))
+    @property
+    def tracker_family(self) -> str:
+        """ Tracker family property.
+        
+        Returns:
+            A string with the tracker family.
+        """
+        return self._tracker_family
 
-    def get(self, key, default = None):
-        value = trax_properties_get(self._ref.reference, key.encode('utf8'))
-        if value == None:
-            return default
-        return value.decode('utf8') if not value is None else None
-
-    def set(self, key, value):
-        trax_properties_set(self._ref.reference, key.encode('utf8'), str(value).encode('utf8'))
-
-    def dict(self):
-        result = dict()
-        fun = lambda key, value, obj: cast(obj, py_object).value.setdefault(key.decode("utf8"), value.decode("utf8"))
-        trax_properties_enumerate(self._ref.reference, trax_enumerator(fun), py_object(result))
-        return result
-
-from .server import Server
-from .region import *
-from .image import *
+    @property
+    def tracker_description(self) -> str:
+        """ Tracker description property.
+        
+        Returns:
+            A string with the tracker description.
+        """
+        return self._tracker_description
+
+    def get(self, key) -> str:
+        """ Get a custom property provided by the tracker.
+        
+        Args:
+            key: A string with the property name.
+            
+        Returns:
+            A string with the property value.
+        """
+        if key in self._custom:
+            return self._custom[key]
+        return None
+
+    def initialize(self, images, objects, properties):
+        """ Initialize the tracker. The response is returned as a tuple of objects and elapsed time.
+        
+        Args:
+            images (list of Image): List of images to be sent to the tracker.
+            objects (list of Region): List of objects to be sent to the tracker.
+            properties (dict): Dictionary of properties to be sent to the tracker.
+        """
+
+        timage = wrap_images(images)
+        tobjects = wrap_objects(objects)
+        tproperties = Properties(properties)
+
+        status = TraxStatus.decode(trax_client_initialize(self._handle.reference, timage.reference, tobjects.reference, tproperties.reference))
+
+        if self._logger and self._logger.interrupted:
+            raise KeyboardInterrupt("Interrupted by user in log callback")
+
+        if status == TraxStatus.ERROR:
+            message = trax_get_error(self._handle.reference)
+            message = message.decode('utf-8') if not message is None else "Unknown"
+            raise TraxException("Exception when initializing tracker: {}".format(message))
+
+        tobjects = trax_object_list_p()
+        properties = Properties()
+
+        start = time.time()
+
+        status = TraxStatus.decode(trax_client_wait(self._handle.reference, byref(tobjects), properties.reference))
+
+        elapsed = time.time() - start
+
+        tobjects = ObjectListWrapper(tobjects)
+
+        if self._logger and self._logger.interrupted:
+            raise KeyboardInterrupt("Interrupted by user in log callback")
+
+        if status == TraxStatus.ERROR:
+            raise TraxException("Exception when waiting for response")
+        if status == TraxStatus.QUIT:
+            reason = properties.get("trax.reason", None)
+            if reason is None:
+                raise TraxException("Server terminated the session")
+            else:
+                raise TraxException("Server terminated the session: {}".format(reason))
+
+        if status == TraxStatus.ERROR:
+            message = trax_get_error(self._handle.reference)
+            message = message.decode('utf-8') if not message is None else "Unknown"
+            raise TraxException("Exception when waiting for response: {}".format(message))
+
+        return wrap_object_list(tobjects.reference), elapsed
+
+    def frame(self, images, properties = dict(), objects = None):
+        """ Send a frame to the tracker and wait for the response. The response is returned as a tuple of objects and elapsed time.
+        The objects are returned as a list of tuples of region and property objects.
+        The elapsed time is the time it took for the tracker to process the frame in seconds.
+        
+        Args:
+            images (list of Image): The list of images to send to the tracker.
+            properties (dict, optional): The properties to send to the tracker.
+            objects (list of Region, optional): The list of regions to send to the tracker.
+
+        Returns:
+            list: The tuple of objects and elapsed time.
+        """
+
+        timage = wrap_images(images)
+        tobjects = wrap_objects(objects)
+        tproperties = Properties(properties)
+
+        status = TraxStatus.decode(trax_client_frame(self._handle.reference, timage.reference, tobjects.reference, tproperties.reference))
+
+        if self._logger and self._logger.interrupted:
+            raise KeyboardInterrupt("Interrupted by user in log callback")
+
+        if status == TraxStatus.ERROR:
+            message = trax_get_error(self._handle.reference)
+            message = message.decode('utf-8') if not message is None else "Unknown"
+            raise TraxException("Exception when sending frame to tracker: {}".format(message))
+
+        tobjects = trax_object_list_p()
+        properties = Properties()
+
+        start = time.time()
+
+        status = TraxStatus.decode(trax_client_wait(self._handle.reference, byref(tobjects), properties.reference))
+
+        elapsed = time.time() - start
+
+        tobjects = ObjectListWrapper(tobjects)
+
+        if self._logger and self._logger.interrupted:
+            raise KeyboardInterrupt("Interrupted by user in log callback")
+
+        if status == TraxStatus.ERROR:
+            message = trax_get_error(self._handle.reference)
+            message = message.decode('utf-8') if not message is None else "Unknown"
+            raise TraxException("Exception when waiting for response: {}".format(message))
+        if status == TraxStatus.QUIT:
+            reason = properties.get("trax.reason", None)
+            if reason is None:
+                raise TraxException("Server terminated the session")
+            else:
+                raise TraxException("Server terminated the session: {}".format(reason))
+            
+        return wrap_object_list(tobjects.reference), elapsed
+
+    def quit(self, reason: str = None):
+        """ Sends quit message and end terminates communication.
+        
+        Args:
+            reason (str): Optional reason for quitting.
+        """
+        if not reason is None:
+            trax_terminate(self._handle.reference, reason.encode('utf-8'))
+        else:
+            trax_terminate(self._handle.reference, None)
 
-__all__ = \
-    ['TraxException', 'FileImage', 'URLImage', 'Server',
-    'MemoryImage', 'BufferImage', 'Region', 'Image', 'Polygon',
-    'Rectangle', 'Special', 'Mask', 'TraxStatus', 'Properties']
+        if self._logger and self._logger.interrupted:
+            raise KeyboardInterrupt("Interrupted by user in log callback")
```

### Comparing `vot-trax-4.0.1/trax/_ctypes.py` & `vot-trax-4.0.2/trax/_ctypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 import re
 import sys
 
 
 def _environ_path(name):
     """Split an environment variable into a path-like list elements"""
     if name in os.environ:
-        return os.environ[name].split(":")
+        return os.environ[name].split(os.pathsep)
     return []
 
 
 class LibraryLoader:
     """
     A base class For loading of libraries ;-)
     Subclasses load libraries for specific platforms.
@@ -452,23 +452,36 @@
 
 # Windows
 
 
 class WindowsLibraryLoader(LibraryLoader):
     """Library loader for Microsoft Windows"""
 
-    name_formats = ["%s.dll", "lib%s.dll", "%slib.dll", "%s"]
+    name_formats = ["%s.dll", "%sd.dll", "lib%s.dll", "%slib.dll", "%s"]
 
     class Lookup(LibraryLoader.Lookup):
         """Lookup class for Windows libraries..."""
 
         def __init__(self, path):
             super(WindowsLibraryLoader.Lookup, self).__init__(path)
             self.access["stdcall"] = ctypes.windll.LoadLibrary(path)
 
+    def getplatformpaths(self, libname):
+        if os.path.pathsep in libname:
+            names = [libname]
+        else:
+            names = [fmt % libname for fmt in self.name_formats]
+
+        for directory in self.getdirs():
+            for name in names:
+                yield os.path.join(directory, name)
+
+    @staticmethod
+    def getdirs():
+        return _environ_path("PATH")
 
 # Platform switching
 
 # If your value of sys.platform does not appear in this dict, please contact
 # the Ctypesgen maintainers.
 
 loaderclass = {
@@ -488,23 +501,22 @@
     file's directory
     """
     for path in other_dirs:
         if not os.path.isabs(path):
             path = os.path.abspath(path)
         load_library.other_dirs.append(path)
 
-
 del loaderclass
 
 # End loader
 
 add_library_search_dirs([os.path.dirname(__file__)])
 
 # Begin libraries
-_libs["libtrax"] = load_library("libtrax")
+_libs["trax"] = load_library("trax")
 
 # 1 libraries
 # End libraries
 
 # No modules
 
 __off_t = c_long# /usr/include/x86_64-linux-gnu/bits/types.h: 152
@@ -673,520 +685,520 @@
     ('images', POINTER(trax_image) * int(3)),
 ]
 
 trax_image_list = struct_trax_image_list# /home/lukacu/Checkouts/vot/trax/include/trax.h: 217
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 219
 try:
-    trax_no_log = (trax_logging).in_dll(_libs["libtrax"], "trax_no_log")
+    trax_no_log = (trax_logging).in_dll(_libs["trax"], "trax_no_log")
 except:
     pass
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 221
 try:
-    trax_no_bounds = (trax_bounds).in_dll(_libs["libtrax"], "trax_no_bounds")
+    trax_no_bounds = (trax_bounds).in_dll(_libs["trax"], "trax_no_bounds")
 except:
     pass
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 226
-if _libs["libtrax"].has("trax_version", "cdecl"):
-    trax_version = _libs["libtrax"].get("trax_version", "cdecl")
+if _libs["trax"].has("trax_version", "cdecl"):
+    trax_version = _libs["trax"].get("trax_version", "cdecl")
     trax_version.argtypes = []
     trax_version.restype = ctypes.c_char_p
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 231
-if _libs["libtrax"].has("trax_metadata_create", "cdecl"):
-    trax_metadata_create = _libs["libtrax"].get("trax_metadata_create", "cdecl")
+if _libs["trax"].has("trax_metadata_create", "cdecl"):
+    trax_metadata_create = _libs["trax"].get("trax_metadata_create", "cdecl")
     trax_metadata_create.argtypes = [c_int, c_int, c_int, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, c_int]
     trax_metadata_create.restype = POINTER(trax_metadata)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 237
-if _libs["libtrax"].has("trax_metadata_release", "cdecl"):
-    trax_metadata_release = _libs["libtrax"].get("trax_metadata_release", "cdecl")
+if _libs["trax"].has("trax_metadata_release", "cdecl"):
+    trax_metadata_release = _libs["trax"].get("trax_metadata_release", "cdecl")
     trax_metadata_release.argtypes = [POINTER(POINTER(trax_metadata))]
     trax_metadata_release.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 242
-if _libs["libtrax"].has("trax_logger_setup", "cdecl"):
-    trax_logger_setup = _libs["libtrax"].get("trax_logger_setup", "cdecl")
+if _libs["trax"].has("trax_logger_setup", "cdecl"):
+    trax_logger_setup = _libs["trax"].get("trax_logger_setup", "cdecl")
     trax_logger_setup.argtypes = [trax_logger, ctypes.c_void_p, c_int]
     trax_logger_setup.restype = trax_logging
 
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 252
-if _libs["libtrax"].has("trax_client_setup_file", "cdecl"):
-    trax_client_setup_file = _libs["libtrax"].get("trax_client_setup_file", "cdecl")
+if _libs["trax"].has("trax_client_setup_file", "cdecl"):
+    trax_client_setup_file = _libs["trax"].get("trax_client_setup_file", "cdecl")
     trax_client_setup_file.argtypes = [c_int, c_int, trax_logging]
     trax_client_setup_file.restype = POINTER(trax_handle)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 257
-if _libs["libtrax"].has("trax_client_setup_socket", "cdecl"):
-    trax_client_setup_socket = _libs["libtrax"].get("trax_client_setup_socket", "cdecl")
+if _libs["trax"].has("trax_client_setup_socket", "cdecl"):
+    trax_client_setup_socket = _libs["trax"].get("trax_client_setup_socket", "cdecl")
     trax_client_setup_socket.argtypes = [c_int, c_int, trax_logging]
     trax_client_setup_socket.restype = POINTER(trax_handle)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 262
-if _libs["libtrax"].has("trax_client_wait", "cdecl"):
-    trax_client_wait = _libs["libtrax"].get("trax_client_wait", "cdecl")
+if _libs["trax"].has("trax_client_wait", "cdecl"):
+    trax_client_wait = _libs["trax"].get("trax_client_wait", "cdecl")
     trax_client_wait.argtypes = [POINTER(trax_handle), POINTER(POINTER(trax_object_list)), POINTER(trax_properties)]
     trax_client_wait.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 267
-if _libs["libtrax"].has("trax_client_initialize", "cdecl"):
-    trax_client_initialize = _libs["libtrax"].get("trax_client_initialize", "cdecl")
+if _libs["trax"].has("trax_client_initialize", "cdecl"):
+    trax_client_initialize = _libs["trax"].get("trax_client_initialize", "cdecl")
     trax_client_initialize.argtypes = [POINTER(trax_handle), POINTER(trax_image_list), POINTER(trax_object_list), POINTER(trax_properties)]
     trax_client_initialize.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 272
-if _libs["libtrax"].has("trax_client_frame", "cdecl"):
-    trax_client_frame = _libs["libtrax"].get("trax_client_frame", "cdecl")
+if _libs["trax"].has("trax_client_frame", "cdecl"):
+    trax_client_frame = _libs["trax"].get("trax_client_frame", "cdecl")
     trax_client_frame.argtypes = [POINTER(trax_handle), POINTER(trax_image_list), POINTER(trax_object_list), POINTER(trax_properties)]
     trax_client_frame.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 277
-if _libs["libtrax"].has("trax_server_setup_v", "cdecl"):
-    trax_server_setup_v = _libs["libtrax"].get("trax_server_setup_v", "cdecl")
+if _libs["trax"].has("trax_server_setup_v", "cdecl"):
+    trax_server_setup_v = _libs["trax"].get("trax_server_setup_v", "cdecl")
     trax_server_setup_v.argtypes = [POINTER(trax_metadata), trax_logging, c_int]
     trax_server_setup_v.restype = POINTER(trax_handle)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 282
-if _libs["libtrax"].has("trax_server_setup_file_v", "cdecl"):
-    trax_server_setup_file_v = _libs["libtrax"].get("trax_server_setup_file_v", "cdecl")
+if _libs["trax"].has("trax_server_setup_file_v", "cdecl"):
+    trax_server_setup_file_v = _libs["trax"].get("trax_server_setup_file_v", "cdecl")
     trax_server_setup_file_v.argtypes = [POINTER(trax_metadata), c_int, c_int, trax_logging, c_int]
     trax_server_setup_file_v.restype = POINTER(trax_handle)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 287
-if _libs["libtrax"].has("trax_server_wait_sot", "cdecl"):
-    trax_server_wait_sot = _libs["libtrax"].get("trax_server_wait_sot", "cdecl")
+if _libs["trax"].has("trax_server_wait_sot", "cdecl"):
+    trax_server_wait_sot = _libs["trax"].get("trax_server_wait_sot", "cdecl")
     trax_server_wait_sot.argtypes = [POINTER(trax_handle), POINTER(POINTER(trax_image_list)), POINTER(ctypes.c_void_p), POINTER(trax_properties)]
     trax_server_wait_sot.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 292
-if _libs["libtrax"].has("trax_server_reply_sot", "cdecl"):
-    trax_server_reply_sot = _libs["libtrax"].get("trax_server_reply_sot", "cdecl")
+if _libs["trax"].has("trax_server_reply_sot", "cdecl"):
+    trax_server_reply_sot = _libs["trax"].get("trax_server_reply_sot", "cdecl")
     trax_server_reply_sot.argtypes = [POINTER(trax_handle), ctypes.c_void_p, POINTER(trax_properties)]
     trax_server_reply_sot.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 297
-if _libs["libtrax"].has("trax_server_wait_mot", "cdecl"):
-    trax_server_wait_mot = _libs["libtrax"].get("trax_server_wait_mot", "cdecl")
+if _libs["trax"].has("trax_server_wait_mot", "cdecl"):
+    trax_server_wait_mot = _libs["trax"].get("trax_server_wait_mot", "cdecl")
     trax_server_wait_mot.argtypes = [POINTER(trax_handle), POINTER(POINTER(trax_image_list)), POINTER(POINTER(trax_object_list)), POINTER(trax_properties)]
     trax_server_wait_mot.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 302
-if _libs["libtrax"].has("trax_server_reply_mot", "cdecl"):
-    trax_server_reply_mot = _libs["libtrax"].get("trax_server_reply_mot", "cdecl")
+if _libs["trax"].has("trax_server_reply_mot", "cdecl"):
+    trax_server_reply_mot = _libs["trax"].get("trax_server_reply_mot", "cdecl")
     trax_server_reply_mot.argtypes = [POINTER(trax_handle), POINTER(trax_object_list)]
     trax_server_reply_mot.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 307
-if _libs["libtrax"].has("trax_terminate", "cdecl"):
-    trax_terminate = _libs["libtrax"].get("trax_terminate", "cdecl")
+if _libs["trax"].has("trax_terminate", "cdecl"):
+    trax_terminate = _libs["trax"].get("trax_terminate", "cdecl")
     trax_terminate.argtypes = [POINTER(trax_handle), ctypes.c_char_p]
     trax_terminate.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 312
-if _libs["libtrax"].has("trax_get_error", "cdecl"):
-    trax_get_error = _libs["libtrax"].get("trax_get_error", "cdecl")
+if _libs["trax"].has("trax_get_error", "cdecl"):
+    trax_get_error = _libs["trax"].get("trax_get_error", "cdecl")
     trax_get_error.argtypes = [POINTER(trax_handle)]
     trax_get_error.restype = ctypes.c_char_p
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 318
-if _libs["libtrax"].has("trax_is_alive", "cdecl"):
-    trax_is_alive = _libs["libtrax"].get("trax_is_alive", "cdecl")
+if _libs["trax"].has("trax_is_alive", "cdecl"):
+    trax_is_alive = _libs["trax"].get("trax_is_alive", "cdecl")
     trax_is_alive.argtypes = [POINTER(trax_handle)]
     trax_is_alive.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 324
-if _libs["libtrax"].has("trax_cleanup", "cdecl"):
-    trax_cleanup = _libs["libtrax"].get("trax_cleanup", "cdecl")
+if _libs["trax"].has("trax_cleanup", "cdecl"):
+    trax_cleanup = _libs["trax"].get("trax_cleanup", "cdecl")
     trax_cleanup.argtypes = [POINTER(POINTER(trax_handle))]
     trax_cleanup.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 329
-if _libs["libtrax"].has("trax_set_parameter", "cdecl"):
-    trax_set_parameter = _libs["libtrax"].get("trax_set_parameter", "cdecl")
+if _libs["trax"].has("trax_set_parameter", "cdecl"):
+    trax_set_parameter = _libs["trax"].get("trax_set_parameter", "cdecl")
     trax_set_parameter.argtypes = [POINTER(trax_handle), c_int, c_int]
     trax_set_parameter.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 334
-if _libs["libtrax"].has("trax_get_parameter", "cdecl"):
-    trax_get_parameter = _libs["libtrax"].get("trax_get_parameter", "cdecl")
+if _libs["trax"].has("trax_get_parameter", "cdecl"):
+    trax_get_parameter = _libs["trax"].get("trax_get_parameter", "cdecl")
     trax_get_parameter.argtypes = [POINTER(trax_handle), c_int, POINTER(c_int)]
     trax_get_parameter.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 339
-if _libs["libtrax"].has("trax_image_release", "cdecl"):
-    trax_image_release = _libs["libtrax"].get("trax_image_release", "cdecl")
+if _libs["trax"].has("trax_image_release", "cdecl"):
+    trax_image_release = _libs["trax"].get("trax_image_release", "cdecl")
     trax_image_release.argtypes = [POINTER(POINTER(trax_image))]
     trax_image_release.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 344
-if _libs["libtrax"].has("trax_image_create_path", "cdecl"):
-    trax_image_create_path = _libs["libtrax"].get("trax_image_create_path", "cdecl")
+if _libs["trax"].has("trax_image_create_path", "cdecl"):
+    trax_image_create_path = _libs["trax"].get("trax_image_create_path", "cdecl")
     trax_image_create_path.argtypes = [ctypes.c_char_p]
     trax_image_create_path.restype = POINTER(trax_image)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 349
-if _libs["libtrax"].has("trax_image_create_url", "cdecl"):
-    trax_image_create_url = _libs["libtrax"].get("trax_image_create_url", "cdecl")
+if _libs["trax"].has("trax_image_create_url", "cdecl"):
+    trax_image_create_url = _libs["trax"].get("trax_image_create_url", "cdecl")
     trax_image_create_url.argtypes = [ctypes.c_char_p]
     trax_image_create_url.restype = POINTER(trax_image)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 354
-if _libs["libtrax"].has("trax_image_create_memory", "cdecl"):
-    trax_image_create_memory = _libs["libtrax"].get("trax_image_create_memory", "cdecl")
+if _libs["trax"].has("trax_image_create_memory", "cdecl"):
+    trax_image_create_memory = _libs["trax"].get("trax_image_create_memory", "cdecl")
     trax_image_create_memory.argtypes = [c_int, c_int, c_int]
     trax_image_create_memory.restype = POINTER(trax_image)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 359
-if _libs["libtrax"].has("trax_image_create_buffer", "cdecl"):
-    trax_image_create_buffer = _libs["libtrax"].get("trax_image_create_buffer", "cdecl")
+if _libs["trax"].has("trax_image_create_buffer", "cdecl"):
+    trax_image_create_buffer = _libs["trax"].get("trax_image_create_buffer", "cdecl")
     trax_image_create_buffer.argtypes = [c_int, ctypes.c_char_p]
     trax_image_create_buffer.restype = POINTER(trax_image)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 364
-if _libs["libtrax"].has("trax_image_get_type", "cdecl"):
-    trax_image_get_type = _libs["libtrax"].get("trax_image_get_type", "cdecl")
+if _libs["trax"].has("trax_image_get_type", "cdecl"):
+    trax_image_get_type = _libs["trax"].get("trax_image_get_type", "cdecl")
     trax_image_get_type.argtypes = [POINTER(trax_image)]
     trax_image_get_type.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 370
-if _libs["libtrax"].has("trax_image_get_path", "cdecl"):
-    trax_image_get_path = _libs["libtrax"].get("trax_image_get_path", "cdecl")
+if _libs["trax"].has("trax_image_get_path", "cdecl"):
+    trax_image_get_path = _libs["trax"].get("trax_image_get_path", "cdecl")
     trax_image_get_path.argtypes = [POINTER(trax_image)]
     trax_image_get_path.restype = ctypes.c_char_p
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 376
-if _libs["libtrax"].has("trax_image_get_url", "cdecl"):
-    trax_image_get_url = _libs["libtrax"].get("trax_image_get_url", "cdecl")
+if _libs["trax"].has("trax_image_get_url", "cdecl"):
+    trax_image_get_url = _libs["trax"].get("trax_image_get_url", "cdecl")
     trax_image_get_url.argtypes = [POINTER(trax_image)]
     trax_image_get_url.restype = ctypes.c_char_p
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 381
-if _libs["libtrax"].has("trax_image_get_memory_header", "cdecl"):
-    trax_image_get_memory_header = _libs["libtrax"].get("trax_image_get_memory_header", "cdecl")
+if _libs["trax"].has("trax_image_get_memory_header", "cdecl"):
+    trax_image_get_memory_header = _libs["trax"].get("trax_image_get_memory_header", "cdecl")
     trax_image_get_memory_header.argtypes = [POINTER(trax_image), POINTER(c_int), POINTER(c_int), POINTER(c_int)]
     trax_image_get_memory_header.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 386
-if _libs["libtrax"].has("trax_image_write_memory_row", "cdecl"):
-    trax_image_write_memory_row = _libs["libtrax"].get("trax_image_write_memory_row", "cdecl")
+if _libs["trax"].has("trax_image_write_memory_row", "cdecl"):
+    trax_image_write_memory_row = _libs["trax"].get("trax_image_write_memory_row", "cdecl")
     trax_image_write_memory_row.argtypes = [POINTER(trax_image), c_int]
     trax_image_write_memory_row.restype = POINTER(ctypes.c_char)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 391
-if _libs["libtrax"].has("trax_image_get_memory_row", "cdecl"):
-    trax_image_get_memory_row = _libs["libtrax"].get("trax_image_get_memory_row", "cdecl")
+if _libs["trax"].has("trax_image_get_memory_row", "cdecl"):
+    trax_image_get_memory_row = _libs["trax"].get("trax_image_get_memory_row", "cdecl")
     trax_image_get_memory_row.argtypes = [POINTER(trax_image), c_int]
     trax_image_get_memory_row.restype = POINTER(ctypes.c_char)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 397
-if _libs["libtrax"].has("trax_image_get_buffer", "cdecl"):
-    trax_image_get_buffer = _libs["libtrax"].get("trax_image_get_buffer", "cdecl")
+if _libs["trax"].has("trax_image_get_buffer", "cdecl"):
+    trax_image_get_buffer = _libs["trax"].get("trax_image_get_buffer", "cdecl")
     trax_image_get_buffer.argtypes = [POINTER(trax_image), POINTER(c_int), POINTER(c_int)]
     trax_image_get_buffer.restype = POINTER(ctypes.c_char)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 402
-if _libs["libtrax"].has("trax_region_release", "cdecl"):
-    trax_region_release = _libs["libtrax"].get("trax_region_release", "cdecl")
+if _libs["trax"].has("trax_region_release", "cdecl"):
+    trax_region_release = _libs["trax"].get("trax_region_release", "cdecl")
     trax_region_release.argtypes = [POINTER(ctypes.c_void_p)]
     trax_region_release.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 407
-if _libs["libtrax"].has("trax_region_get_type", "cdecl"):
-    trax_region_get_type = _libs["libtrax"].get("trax_region_get_type", "cdecl")
+if _libs["trax"].has("trax_region_get_type", "cdecl"):
+    trax_region_get_type = _libs["trax"].get("trax_region_get_type", "cdecl")
     trax_region_get_type.argtypes = [ctypes.c_void_p]
     trax_region_get_type.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 412
-if _libs["libtrax"].has("trax_region_create_special", "cdecl"):
-    trax_region_create_special = _libs["libtrax"].get("trax_region_create_special", "cdecl")
+if _libs["trax"].has("trax_region_create_special", "cdecl"):
+    trax_region_create_special = _libs["trax"].get("trax_region_create_special", "cdecl")
     trax_region_create_special.argtypes = [c_int]
     trax_region_create_special.restype = ctypes.c_void_p
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 417
-if _libs["libtrax"].has("trax_region_set_special", "cdecl"):
-    trax_region_set_special = _libs["libtrax"].get("trax_region_set_special", "cdecl")
+if _libs["trax"].has("trax_region_set_special", "cdecl"):
+    trax_region_set_special = _libs["trax"].get("trax_region_set_special", "cdecl")
     trax_region_set_special.argtypes = [ctypes.c_void_p, c_int]
     trax_region_set_special.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 422
-if _libs["libtrax"].has("trax_region_get_special", "cdecl"):
-    trax_region_get_special = _libs["libtrax"].get("trax_region_get_special", "cdecl")
+if _libs["trax"].has("trax_region_get_special", "cdecl"):
+    trax_region_get_special = _libs["trax"].get("trax_region_get_special", "cdecl")
     trax_region_get_special.argtypes = [ctypes.c_void_p]
     trax_region_get_special.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 427
-if _libs["libtrax"].has("trax_region_create_rectangle", "cdecl"):
-    trax_region_create_rectangle = _libs["libtrax"].get("trax_region_create_rectangle", "cdecl")
+if _libs["trax"].has("trax_region_create_rectangle", "cdecl"):
+    trax_region_create_rectangle = _libs["trax"].get("trax_region_create_rectangle", "cdecl")
     trax_region_create_rectangle.argtypes = [c_float, c_float, c_float, c_float]
     trax_region_create_rectangle.restype = ctypes.c_void_p
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 432
-if _libs["libtrax"].has("trax_region_set_rectangle", "cdecl"):
-    trax_region_set_rectangle = _libs["libtrax"].get("trax_region_set_rectangle", "cdecl")
+if _libs["trax"].has("trax_region_set_rectangle", "cdecl"):
+    trax_region_set_rectangle = _libs["trax"].get("trax_region_set_rectangle", "cdecl")
     trax_region_set_rectangle.argtypes = [ctypes.c_void_p, c_float, c_float, c_float, c_float]
     trax_region_set_rectangle.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 437
-if _libs["libtrax"].has("trax_region_get_rectangle", "cdecl"):
-    trax_region_get_rectangle = _libs["libtrax"].get("trax_region_get_rectangle", "cdecl")
+if _libs["trax"].has("trax_region_get_rectangle", "cdecl"):
+    trax_region_get_rectangle = _libs["trax"].get("trax_region_get_rectangle", "cdecl")
     trax_region_get_rectangle.argtypes = [ctypes.c_void_p, POINTER(c_float), POINTER(c_float), POINTER(c_float), POINTER(c_float)]
     trax_region_get_rectangle.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 443
-if _libs["libtrax"].has("trax_region_create_polygon", "cdecl"):
-    trax_region_create_polygon = _libs["libtrax"].get("trax_region_create_polygon", "cdecl")
+if _libs["trax"].has("trax_region_create_polygon", "cdecl"):
+    trax_region_create_polygon = _libs["trax"].get("trax_region_create_polygon", "cdecl")
     trax_region_create_polygon.argtypes = [c_int]
     trax_region_create_polygon.restype = ctypes.c_void_p
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 448
-if _libs["libtrax"].has("trax_region_set_polygon_point", "cdecl"):
-    trax_region_set_polygon_point = _libs["libtrax"].get("trax_region_set_polygon_point", "cdecl")
+if _libs["trax"].has("trax_region_set_polygon_point", "cdecl"):
+    trax_region_set_polygon_point = _libs["trax"].get("trax_region_set_polygon_point", "cdecl")
     trax_region_set_polygon_point.argtypes = [ctypes.c_void_p, c_int, c_float, c_float]
     trax_region_set_polygon_point.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 453
-if _libs["libtrax"].has("trax_region_get_polygon_point", "cdecl"):
-    trax_region_get_polygon_point = _libs["libtrax"].get("trax_region_get_polygon_point", "cdecl")
+if _libs["trax"].has("trax_region_get_polygon_point", "cdecl"):
+    trax_region_get_polygon_point = _libs["trax"].get("trax_region_get_polygon_point", "cdecl")
     trax_region_get_polygon_point.argtypes = [ctypes.c_void_p, c_int, POINTER(c_float), POINTER(c_float)]
     trax_region_get_polygon_point.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 458
-if _libs["libtrax"].has("trax_region_get_polygon_count", "cdecl"):
-    trax_region_get_polygon_count = _libs["libtrax"].get("trax_region_get_polygon_count", "cdecl")
+if _libs["trax"].has("trax_region_get_polygon_count", "cdecl"):
+    trax_region_get_polygon_count = _libs["trax"].get("trax_region_get_polygon_count", "cdecl")
     trax_region_get_polygon_count.argtypes = [ctypes.c_void_p]
     trax_region_get_polygon_count.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 463
-if _libs["libtrax"].has("trax_region_create_mask", "cdecl"):
-    trax_region_create_mask = _libs["libtrax"].get("trax_region_create_mask", "cdecl")
+if _libs["trax"].has("trax_region_create_mask", "cdecl"):
+    trax_region_create_mask = _libs["trax"].get("trax_region_create_mask", "cdecl")
     trax_region_create_mask.argtypes = [c_int, c_int, c_int, c_int]
     trax_region_create_mask.restype = ctypes.c_void_p
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 468
-if _libs["libtrax"].has("trax_region_get_mask_header", "cdecl"):
-    trax_region_get_mask_header = _libs["libtrax"].get("trax_region_get_mask_header", "cdecl")
+if _libs["trax"].has("trax_region_get_mask_header", "cdecl"):
+    trax_region_get_mask_header = _libs["trax"].get("trax_region_get_mask_header", "cdecl")
     trax_region_get_mask_header.argtypes = [ctypes.c_void_p, POINTER(c_int), POINTER(c_int), POINTER(c_int), POINTER(c_int)]
     trax_region_get_mask_header.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 473
-if _libs["libtrax"].has("trax_region_write_mask_row", "cdecl"):
-    trax_region_write_mask_row = _libs["libtrax"].get("trax_region_write_mask_row", "cdecl")
+if _libs["trax"].has("trax_region_write_mask_row", "cdecl"):
+    trax_region_write_mask_row = _libs["trax"].get("trax_region_write_mask_row", "cdecl")
     trax_region_write_mask_row.argtypes = [ctypes.c_void_p, c_int]
     trax_region_write_mask_row.restype = POINTER(ctypes.c_char)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 478
-if _libs["libtrax"].has("trax_region_get_mask_row", "cdecl"):
-    trax_region_get_mask_row = _libs["libtrax"].get("trax_region_get_mask_row", "cdecl")
+if _libs["trax"].has("trax_region_get_mask_row", "cdecl"):
+    trax_region_get_mask_row = _libs["trax"].get("trax_region_get_mask_row", "cdecl")
     trax_region_get_mask_row.argtypes = [ctypes.c_void_p, c_int]
     trax_region_get_mask_row.restype = POINTER(ctypes.c_char)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 483
-if _libs["libtrax"].has("trax_region_bounds", "cdecl"):
-    trax_region_bounds = _libs["libtrax"].get("trax_region_bounds", "cdecl")
+if _libs["trax"].has("trax_region_bounds", "cdecl"):
+    trax_region_bounds = _libs["trax"].get("trax_region_bounds", "cdecl")
     trax_region_bounds.argtypes = [ctypes.c_void_p]
     trax_region_bounds.restype = trax_bounds
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 488
-if _libs["libtrax"].has("trax_region_contains", "cdecl"):
-    trax_region_contains = _libs["libtrax"].get("trax_region_contains", "cdecl")
+if _libs["trax"].has("trax_region_contains", "cdecl"):
+    trax_region_contains = _libs["trax"].get("trax_region_contains", "cdecl")
     trax_region_contains.argtypes = [ctypes.c_void_p, c_float, c_float]
     trax_region_contains.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 493
-if _libs["libtrax"].has("trax_region_clone", "cdecl"):
-    trax_region_clone = _libs["libtrax"].get("trax_region_clone", "cdecl")
+if _libs["trax"].has("trax_region_clone", "cdecl"):
+    trax_region_clone = _libs["trax"].get("trax_region_clone", "cdecl")
     trax_region_clone.argtypes = [ctypes.c_void_p]
     trax_region_clone.restype = ctypes.c_void_p
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 498
-if _libs["libtrax"].has("trax_region_convert", "cdecl"):
-    trax_region_convert = _libs["libtrax"].get("trax_region_convert", "cdecl")
+if _libs["trax"].has("trax_region_convert", "cdecl"):
+    trax_region_convert = _libs["trax"].get("trax_region_convert", "cdecl")
     trax_region_convert.argtypes = [ctypes.c_void_p, c_int]
     trax_region_convert.restype = ctypes.c_void_p
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 503
-if _libs["libtrax"].has("trax_region_overlap", "cdecl"):
-    trax_region_overlap = _libs["libtrax"].get("trax_region_overlap", "cdecl")
+if _libs["trax"].has("trax_region_overlap", "cdecl"):
+    trax_region_overlap = _libs["trax"].get("trax_region_overlap", "cdecl")
     trax_region_overlap.argtypes = [ctypes.c_void_p, ctypes.c_void_p, trax_bounds]
     trax_region_overlap.restype = c_float
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 508
-if _libs["libtrax"].has("trax_region_encode", "cdecl"):
-    trax_region_encode = _libs["libtrax"].get("trax_region_encode", "cdecl")
+if _libs["trax"].has("trax_region_encode", "cdecl"):
+    trax_region_encode = _libs["trax"].get("trax_region_encode", "cdecl")
     trax_region_encode.argtypes = [ctypes.c_void_p]
     trax_region_encode.restype = POINTER(ctypes.c_char)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 513
-if _libs["libtrax"].has("trax_region_decode", "cdecl"):
-    trax_region_decode = _libs["libtrax"].get("trax_region_decode", "cdecl")
+if _libs["trax"].has("trax_region_decode", "cdecl"):
+    trax_region_decode = _libs["trax"].get("trax_region_decode", "cdecl")
     trax_region_decode.argtypes = [ctypes.c_char_p]
     trax_region_decode.restype = ctypes.c_void_p
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 518
-if _libs["libtrax"].has("trax_object_list_create", "cdecl"):
-    trax_object_list_create = _libs["libtrax"].get("trax_object_list_create", "cdecl")
+if _libs["trax"].has("trax_object_list_create", "cdecl"):
+    trax_object_list_create = _libs["trax"].get("trax_object_list_create", "cdecl")
     trax_object_list_create.argtypes = [c_int]
     trax_object_list_create.restype = POINTER(trax_object_list)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 523
-if _libs["libtrax"].has("trax_object_list_release", "cdecl"):
-    trax_object_list_release = _libs["libtrax"].get("trax_object_list_release", "cdecl")
+if _libs["trax"].has("trax_object_list_release", "cdecl"):
+    trax_object_list_release = _libs["trax"].get("trax_object_list_release", "cdecl")
     trax_object_list_release.argtypes = [POINTER(POINTER(trax_object_list))]
     trax_object_list_release.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 528
-if _libs["libtrax"].has("trax_object_list_set", "cdecl"):
-    trax_object_list_set = _libs["libtrax"].get("trax_object_list_set", "cdecl")
+if _libs["trax"].has("trax_object_list_set", "cdecl"):
+    trax_object_list_set = _libs["trax"].get("trax_object_list_set", "cdecl")
     trax_object_list_set.argtypes = [POINTER(trax_object_list), c_int, ctypes.c_void_p]
     trax_object_list_set.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 533
-if _libs["libtrax"].has("trax_object_list_get", "cdecl"):
-    trax_object_list_get = _libs["libtrax"].get("trax_object_list_get", "cdecl")
+if _libs["trax"].has("trax_object_list_get", "cdecl"):
+    trax_object_list_get = _libs["trax"].get("trax_object_list_get", "cdecl")
     trax_object_list_get.argtypes = [POINTER(trax_object_list), c_int]
     trax_object_list_get.restype = ctypes.c_void_p
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 538
-if _libs["libtrax"].has("trax_object_list_properties", "cdecl"):
-    trax_object_list_properties = _libs["libtrax"].get("trax_object_list_properties", "cdecl")
+if _libs["trax"].has("trax_object_list_properties", "cdecl"):
+    trax_object_list_properties = _libs["trax"].get("trax_object_list_properties", "cdecl")
     trax_object_list_properties.argtypes = [POINTER(trax_object_list), c_int]
     trax_object_list_properties.restype = POINTER(trax_properties)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 543
-if _libs["libtrax"].has("trax_object_list_count", "cdecl"):
-    trax_object_list_count = _libs["libtrax"].get("trax_object_list_count", "cdecl")
+if _libs["trax"].has("trax_object_list_count", "cdecl"):
+    trax_object_list_count = _libs["trax"].get("trax_object_list_count", "cdecl")
     trax_object_list_count.argtypes = [POINTER(trax_object_list)]
     trax_object_list_count.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 548
-if _libs["libtrax"].has("trax_object_list_append", "cdecl"):
-    trax_object_list_append = _libs["libtrax"].get("trax_object_list_append", "cdecl")
+if _libs["trax"].has("trax_object_list_append", "cdecl"):
+    trax_object_list_append = _libs["trax"].get("trax_object_list_append", "cdecl")
     trax_object_list_append.argtypes = [POINTER(trax_object_list), POINTER(trax_object_list)]
     trax_object_list_append.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 553
-if _libs["libtrax"].has("trax_properties_release", "cdecl"):
-    trax_properties_release = _libs["libtrax"].get("trax_properties_release", "cdecl")
+if _libs["trax"].has("trax_properties_release", "cdecl"):
+    trax_properties_release = _libs["trax"].get("trax_properties_release", "cdecl")
     trax_properties_release.argtypes = [POINTER(POINTER(trax_properties))]
     trax_properties_release.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 558
-if _libs["libtrax"].has("trax_properties_clear", "cdecl"):
-    trax_properties_clear = _libs["libtrax"].get("trax_properties_clear", "cdecl")
+if _libs["trax"].has("trax_properties_clear", "cdecl"):
+    trax_properties_clear = _libs["trax"].get("trax_properties_clear", "cdecl")
     trax_properties_clear.argtypes = [POINTER(trax_properties)]
     trax_properties_clear.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 563
-if _libs["libtrax"].has("trax_properties_create", "cdecl"):
-    trax_properties_create = _libs["libtrax"].get("trax_properties_create", "cdecl")
+if _libs["trax"].has("trax_properties_create", "cdecl"):
+    trax_properties_create = _libs["trax"].get("trax_properties_create", "cdecl")
     trax_properties_create.argtypes = []
     trax_properties_create.restype = POINTER(trax_properties)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 568
-if _libs["libtrax"].has("trax_properties_copy", "cdecl"):
-    trax_properties_copy = _libs["libtrax"].get("trax_properties_copy", "cdecl")
+if _libs["trax"].has("trax_properties_copy", "cdecl"):
+    trax_properties_copy = _libs["trax"].get("trax_properties_copy", "cdecl")
     trax_properties_copy.argtypes = [POINTER(trax_properties)]
     trax_properties_copy.restype = POINTER(trax_properties)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 573
-if _libs["libtrax"].has("trax_properties_has", "cdecl"):
-    trax_properties_has = _libs["libtrax"].get("trax_properties_has", "cdecl")
+if _libs["trax"].has("trax_properties_has", "cdecl"):
+    trax_properties_has = _libs["trax"].get("trax_properties_has", "cdecl")
     trax_properties_has.argtypes = [POINTER(trax_properties), ctypes.c_char_p]
     trax_properties_has.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 578
-if _libs["libtrax"].has("trax_properties_set", "cdecl"):
-    trax_properties_set = _libs["libtrax"].get("trax_properties_set", "cdecl")
+if _libs["trax"].has("trax_properties_set", "cdecl"):
+    trax_properties_set = _libs["trax"].get("trax_properties_set", "cdecl")
     trax_properties_set.argtypes = [POINTER(trax_properties), ctypes.c_char_p, ctypes.c_char_p]
     trax_properties_set.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 583
-if _libs["libtrax"].has("trax_properties_set_int", "cdecl"):
-    trax_properties_set_int = _libs["libtrax"].get("trax_properties_set_int", "cdecl")
+if _libs["trax"].has("trax_properties_set_int", "cdecl"):
+    trax_properties_set_int = _libs["trax"].get("trax_properties_set_int", "cdecl")
     trax_properties_set_int.argtypes = [POINTER(trax_properties), ctypes.c_char_p, c_int]
     trax_properties_set_int.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 588
-if _libs["libtrax"].has("trax_properties_set_float", "cdecl"):
-    trax_properties_set_float = _libs["libtrax"].get("trax_properties_set_float", "cdecl")
+if _libs["trax"].has("trax_properties_set_float", "cdecl"):
+    trax_properties_set_float = _libs["trax"].get("trax_properties_set_float", "cdecl")
     trax_properties_set_float.argtypes = [POINTER(trax_properties), ctypes.c_char_p, c_float]
     trax_properties_set_float.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 594
-if _libs["libtrax"].has("trax_properties_get", "cdecl"):
-    trax_properties_get = _libs["libtrax"].get("trax_properties_get", "cdecl")
+if _libs["trax"].has("trax_properties_get", "cdecl"):
+    trax_properties_get = _libs["trax"].get("trax_properties_get", "cdecl")
     trax_properties_get.argtypes = [POINTER(trax_properties), ctypes.c_char_p]
     trax_properties_get.restype = ctypes.c_char_p
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 600
-if _libs["libtrax"].has("trax_properties_get_int", "cdecl"):
-    trax_properties_get_int = _libs["libtrax"].get("trax_properties_get_int", "cdecl")
+if _libs["trax"].has("trax_properties_get_int", "cdecl"):
+    trax_properties_get_int = _libs["trax"].get("trax_properties_get_int", "cdecl")
     trax_properties_get_int.argtypes = [POINTER(trax_properties), ctypes.c_char_p, c_int]
     trax_properties_get_int.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 606
-if _libs["libtrax"].has("trax_properties_get_float", "cdecl"):
-    trax_properties_get_float = _libs["libtrax"].get("trax_properties_get_float", "cdecl")
+if _libs["trax"].has("trax_properties_get_float", "cdecl"):
+    trax_properties_get_float = _libs["trax"].get("trax_properties_get_float", "cdecl")
     trax_properties_get_float.argtypes = [POINTER(trax_properties), ctypes.c_char_p, c_float]
     trax_properties_get_float.restype = c_float
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 611
-if _libs["libtrax"].has("trax_properties_count", "cdecl"):
-    trax_properties_count = _libs["libtrax"].get("trax_properties_count", "cdecl")
+if _libs["trax"].has("trax_properties_count", "cdecl"):
+    trax_properties_count = _libs["trax"].get("trax_properties_count", "cdecl")
     trax_properties_count.argtypes = [POINTER(trax_properties)]
     trax_properties_count.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 617
-if _libs["libtrax"].has("trax_properties_enumerate", "cdecl"):
-    trax_properties_enumerate = _libs["libtrax"].get("trax_properties_enumerate", "cdecl")
+if _libs["trax"].has("trax_properties_enumerate", "cdecl"):
+    trax_properties_enumerate = _libs["trax"].get("trax_properties_enumerate", "cdecl")
     trax_properties_enumerate.argtypes = [POINTER(struct_trax_properties), trax_enumerator, ctypes.py_object]
     trax_properties_enumerate.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 622
-if _libs["libtrax"].has("trax_properties_append", "cdecl"):
-    trax_properties_append = _libs["libtrax"].get("trax_properties_append", "cdecl")
+if _libs["trax"].has("trax_properties_append", "cdecl"):
+    trax_properties_append = _libs["trax"].get("trax_properties_append", "cdecl")
     trax_properties_append.argtypes = [POINTER(trax_properties), POINTER(trax_properties), c_int]
     trax_properties_append.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 627
-if _libs["libtrax"].has("trax_image_list_create", "cdecl"):
-    trax_image_list_create = _libs["libtrax"].get("trax_image_list_create", "cdecl")
+if _libs["trax"].has("trax_image_list_create", "cdecl"):
+    trax_image_list_create = _libs["trax"].get("trax_image_list_create", "cdecl")
     trax_image_list_create.argtypes = []
     trax_image_list_create.restype = POINTER(trax_image_list)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 632
-if _libs["libtrax"].has("trax_image_list_release", "cdecl"):
-    trax_image_list_release = _libs["libtrax"].get("trax_image_list_release", "cdecl")
+if _libs["trax"].has("trax_image_list_release", "cdecl"):
+    trax_image_list_release = _libs["trax"].get("trax_image_list_release", "cdecl")
     trax_image_list_release.argtypes = [POINTER(POINTER(trax_image_list))]
     trax_image_list_release.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 637
-if _libs["libtrax"].has("trax_image_list_clear", "cdecl"):
-    trax_image_list_clear = _libs["libtrax"].get("trax_image_list_clear", "cdecl")
+if _libs["trax"].has("trax_image_list_clear", "cdecl"):
+    trax_image_list_clear = _libs["trax"].get("trax_image_list_clear", "cdecl")
     trax_image_list_clear.argtypes = [POINTER(trax_image_list)]
     trax_image_list_clear.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 642
-if _libs["libtrax"].has("trax_image_list_get", "cdecl"):
-    trax_image_list_get = _libs["libtrax"].get("trax_image_list_get", "cdecl")
+if _libs["trax"].has("trax_image_list_get", "cdecl"):
+    trax_image_list_get = _libs["trax"].get("trax_image_list_get", "cdecl")
     trax_image_list_get.argtypes = [POINTER(trax_image_list), c_int]
     trax_image_list_get.restype = POINTER(trax_image)
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 647
-if _libs["libtrax"].has("trax_image_list_set", "cdecl"):
-    trax_image_list_set = _libs["libtrax"].get("trax_image_list_set", "cdecl")
+if _libs["trax"].has("trax_image_list_set", "cdecl"):
+    trax_image_list_set = _libs["trax"].get("trax_image_list_set", "cdecl")
     trax_image_list_set.argtypes = [POINTER(trax_image_list), POINTER(trax_image), c_int]
     trax_image_list_set.restype = None
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 652
-if _libs["libtrax"].has("trax_image_list_count", "cdecl"):
-    trax_image_list_count = _libs["libtrax"].get("trax_image_list_count", "cdecl")
+if _libs["trax"].has("trax_image_list_count", "cdecl"):
+    trax_image_list_count = _libs["trax"].get("trax_image_list_count", "cdecl")
     trax_image_list_count.argtypes = [c_int]
     trax_image_list_count.restype = c_int
 
 # /home/lukacu/Checkouts/vot/trax/include/trax.h: 39
 try:
     TRAX_NO_LOG = (-1)
 except:
```

### Comparing `vot-trax-4.0.1/trax/base64.c` & `vot-trax-4.0.2/trax/base64.c`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.1/trax/buffer.h` & `vot-trax-4.0.2/trax/buffer.h`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.1/trax/client.py` & `vot-trax-4.0.2/trax/server.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,223 +1,174 @@
 """
 Bindings for the TraX sever.
 """
 
-import time
+import traceback
+import collections
 
-from ctypes import byref, c_int
+from ctypes import byref, cast, py_object
 
-from . import TraxException, TraxStatus, Properties, HandleWrapper, \
-    ConsoleLogger, FileLogger, ProxyLogger, trax_object_list_p
-    
-from . import wrap_images, wrap_objects, wrap_object_list, ObjectListWrapper
-
-from ._ctypes import \
-    trax_client_initialize, \
-    trax_client_wait, trax_client_frame, \
-    trax_client_setup_file, trax_client_setup_socket, \
-    trax_logger_setup, trax_logger, trax_get_parameter, \
-    trax_terminate, trax_get_error, trax_is_alive, TRAX_PARAMETER_MULTIOBJECT
+__all__ = \
+    ['Server', 'Rquest']
 
 from .image import ImageChannel, Image
 from .region import Region
 
-class Client(object):
 
-    """ TraX client."""
+from ._ctypes import \
+        trax_metadata_create, trax_server_setup_v, \
+        trax_logger_setup, trax_metadata_release, \
+        trax_server_wait, trax_server_reply, \
+        trax_image_list_release,  \
+        trax_logger, trax_terminate, \
+        trax_is_alive, trax_get_error, trax_object_list_release
 
-    def __init__(self, stream=None, timeout=30, log=False):
 
-        if isinstance(log, bool) and log:
-            self._logger = ConsoleLogger()
-        elif isinstance(log, str):
-            self._logger = FileLogger(log)
-        elif callable(log):
-            self._logger = ProxyLogger(log)
-        else:
-            self._logger = None
+class Request(collections.namedtuple('Request', ['type', 'image', 'objects', 'properties'])):
+    """ A container class for client requests. Contains fileds type, image, objects and parameters.
+    
+    Args:
+        type (TraxStatus): Type of the request.
+        image (List[Image]): List of images.
+        objects (List[Region]): List of regions.
+        properties (dict): Optional arguments as a dictionary.
+    """
 
-        self._clogger = trax_logger(self._logger) if not self._logger is None else None
+def _logger(buf, len, obj):
 
-        logger = trax_logger_setup(self._clogger, 0, 0)
+    self = cast(obj, py_object)
 
-        if isinstance(stream, tuple):
+    #self._log(string)
 
-            assert(len(stream) == 2)
+class Server(object):
 
-            handle = trax_client_setup_file(
-                stream[1],
-                stream[0],
-                logger)
+    """ TraX server."""
 
-        elif isinstance(stream, int):
+    def __init__(self, region_formats, image_formats, image_channels=["color"], tracker_name="", tracker_description="", tracker_family="", metadata=None, log=False, multiobject=False):
 
-            handle = trax_client_setup_socket(
-                stream,
-                timeout,
-                logger)
+        from . import TraxException, ConsoleLogger, FileLogger, Properties, HandleWrapper
+        from ._ctypes import TRAX_METADATA_MULTI_OBJECT
 
+        if isinstance(log, bool) and log:
+            self._logger = trax_logger(ConsoleLogger())
+        elif isinstance(log, str):
+            self._logger = trax_logger(FileLogger(log))
         else:
-            raise TraxException("Invalid parameters")
-
-        if self._logger and self._logger.interrupted:
-            raise KeyboardInterrupt("Interrupted by user in log callback")
-
-        if not handle:
-            raise TraxException("Unable to connect to tracker")
-
-        if trax_is_alive(handle) == 0:
-            message = trax_get_error(handle.reference)
-            message = message.decode('utf-8') if not message is None else "Unknown"
-            raise TraxException("Exception when connecting to tracker: {}".format(message))
-
-        self._handle = HandleWrapper(handle)
-
-        metadata = self._handle.reference.contents.metadata
-
-        self._format_region = Region.decode_list(metadata.contents.format_region)
-        self._format_image = Image.decode_list(metadata.contents.format_image)
-        self._channels = ImageChannel.decode_list(metadata.contents.channels)
-        
-        self._tracker_name = metadata.contents.tracker_name.decode("utf-8") \
-            if not metadata.contents.tracker_name is None else ""
-        self._tracker_family = metadata.contents.tracker_family.decode("utf-8") \
-            if not metadata.contents.tracker_family is None else ""
-        self._tracker_description = metadata.contents.tracker_description.decode("utf-8") \
-            if not metadata.contents.tracker_description is None else ""
-
-        custom = Properties(metadata.contents.custom, False)
-
-        self._custom = custom.dict()
-
-        value = c_int(value=0)   
-        trax_get_parameter(handle, TRAX_PARAMETER_MULTIOBJECT, byref(value))
+            self._logger = trax_logger()
 
-        self._custom["multiobject"] = bool(value.value)
+        flags = 0
 
-    @property
-    def channels(self):
-        return self._channels
+        if multiobject:
+            flags |= TRAX_METADATA_MULTI_OBJECT
 
-    @property
-    def image_formats(self):
-        return self._format_image
+        mdata = trax_metadata_create(Region.encode_list(region_formats),
+            Image.encode_list(image_formats), ImageChannel.encode_list(image_channels),
+            tracker_name.encode('utf-8'), tracker_description.encode('utf-8'), tracker_family.encode('utf-8'), flags)
 
-    @property
-    def region_formats(self):
-        return self._format_region
+        if isinstance(metadata, dict):
+            custom = Properties(mdata.contents.custom, False)
+            for key, value in metadata.items():
+                custom.set(key, value)
 
-    @property
-    def tracker_name(self):
-        return self._tracker_name
+        logger = trax_logger_setup(self._logger, None, 0)
 
-    @property
-    def tracker_family(self):
-        return self._tracker_family
+        handle = trax_server_setup_v(mdata, logger, 0)
 
-    @property
-    def tracker_description(self):
-        return self._tracker_description
+        trax_metadata_release(byref(mdata))
 
-    def get(self, key):
-        if key in self._custom:
-            return self._custom[key]
-        return None
-
-    def initialize(self, images, objects, properties):
+        if not handle:
+            raise TraxException("Exception when setting up.")
 
-        timage = wrap_images(images)
-        tobjects = wrap_objects(objects)
-        tproperties = Properties(properties)
+        if trax_is_alive(handle) == 0:
+            message = trax_get_error(handle.reference)
+            message = message.decode('utf-8') if not message is None else "Unknown"
+            raise TraxException("Exception when setting up: {}".format(message))
 
-        status = TraxStatus.decode(trax_client_initialize(self._handle.reference, timage.reference, tobjects.reference, tproperties.reference))
+        self._handle = HandleWrapper(handle)
 
-        if self._logger and self._logger.interrupted:
-            raise KeyboardInterrupt("Interrupted by user in log callback")
+    def wait(self):
+        """ Wait for client message request. Recognize it and parse them when received .
 
-        if status == TraxStatus.ERROR:
-            message = trax_get_error(self._handle.reference)
-            message = message.decode('utf-8') if not message is None else "Unknown"
-            raise TraxException("Exception when initializing tracker: {}".format(message))
+            :returns: A request structure
+            :rtype: trax.server.Request
+        """
+        from . import TraxException, Properties, TraxStatus, wrap_image_list, wrap_object_list, trax_image_list_p, trax_object_list_p
 
+        timage = trax_image_list_p()
         tobjects = trax_object_list_p()
         properties = Properties()
 
-        start = time.time()
-
-        status = TraxStatus.decode(trax_client_wait(self._handle.reference, byref(tobjects), properties.reference))
+        status = TraxStatus.decode(trax_server_wait(self._handle.reference, byref(timage), byref(tobjects), properties.reference))
 
-        elapsed = time.time() - start
-
-        tobjects = ObjectListWrapper(tobjects)
-
-        if self._logger and self._logger.interrupted:
-            raise KeyboardInterrupt("Interrupted by user in log callback")
-
-        if status == TraxStatus.ERROR:
-            raise TraxException("Exception when waiting for response")
         if status == TraxStatus.QUIT:
-            reason = properties.get("trax.reason", None)
-            if reason is None:
-                raise TraxException("Server terminated the session")
+            return Request(status, None, None, properties)
+
+        if status == TraxStatus.INITIALIZE:
+            image = wrap_image_list(timage)
+            objects = wrap_object_list(tobjects)
+            trax_image_list_release(byref(timage))
+            trax_object_list_release(byref(tobjects))
+            return Request(status, image, objects, properties)
+
+        if status == TraxStatus.FRAME:
+            image = wrap_image_list(timage)
+            trax_image_list_release(byref(timage))
+            if tobjects:
+                objects = wrap_object_list(tobjects)
+                trax_object_list_release(byref(tobjects))
             else:
-                raise TraxException("Server terminated the session: {}".format(reason))
+                objects = None
+            return Request(status, image, objects, properties)
 
-        if status == TraxStatus.ERROR:
+        else:
             message = trax_get_error(self._handle.reference)
             message = message.decode('utf-8') if not message is None else "Unknown"
-            raise TraxException("Exception when waiting for response: {}".format(message))
-
-        return wrap_object_list(tobjects.reference), elapsed
+            raise TraxException("Exception when waiting for command: {}".format(message))
 
-    def frame(self, images, properties = dict(), objects = None):
+    def status(self, objects, properties=None):
+        """ Reply to client with a status region and optional properties.
 
-        timage = wrap_images(images)
-        tobjects = wrap_objects(objects)
-        tproperties = Properties(properties)
 
-        status = TraxStatus.decode(trax_client_frame(self._handle.reference, timage.reference, tobjects.reference, tproperties.reference))
+            :param List[Region, Mapping] objects: Resulting status of tracked objects.
+            :param dict properties: Optional arguments as a dictionary.
+        """
+        from . import TraxException, TraxStatus, Properties, wrap_objects
 
-        if self._logger and self._logger.interrupted:
-            raise KeyboardInterrupt("Interrupted by user in log callback")
+        assert(isinstance(objects, list))
+        tproperties = Properties(properties)
+        tobjects = wrap_objects(objects)
+        status = TraxStatus.decode(trax_server_reply(self._handle.reference, tobjects.reference, tproperties.reference))
 
         if status == TraxStatus.ERROR:
             message = trax_get_error(self._handle.reference)
             message = message.decode('utf-8') if not message is None else "Unknown"
-            raise TraxException("Exception when sending frame to tracker: {}".format(message))
+            raise TraxException("Exception when sending status: {}".format(message))
 
-        tobjects = trax_object_list_p()
-        properties = Properties()
-
-        start = time.time()
-
-        status = TraxStatus.decode(trax_client_wait(self._handle.reference, byref(tobjects), properties.reference))
+        return True
 
-        elapsed = time.time() - start
+    def __enter__(self):
+        """ To support instantiation with 'with' statement. """
+        return self
+
+    def __exit__(self, exc_type, exc_val, tb):
+        """ Session destructor used by 'with' statement. """
+        if exc_val:
+            traceback.print_exception(exc_type, exc_val, tb)
+            self.quit(reason=str(exc_val))
+        else:
+            self.quit()
 
-        tobjects = ObjectListWrapper(tobjects)
+    def quit(self, reason=None):
+        """ Sends quit message and end terminates communication. """
+        from . import TraxException, TraxStatus
 
-        if self._logger and self._logger.interrupted:
-            raise KeyboardInterrupt("Interrupted by user in log callback")
+        if not reason is None:
+            status = TraxStatus.decode(trax_terminate(self._handle.reference, reason.encode('utf-8')))
+        else:
+            status = TraxStatus.decode(trax_terminate(self._handle.reference, None))
 
         if status == TraxStatus.ERROR:
             message = trax_get_error(self._handle.reference)
             message = message.decode('utf-8') if not message is None else "Unknown"
-            raise TraxException("Exception when waiting for response: {}".format(message))
-        if status == TraxStatus.QUIT:
-            reason = properties.get("trax.reason", None)
-            if reason is None:
-                raise TraxException("Server terminated the session")
-            else:
-                raise TraxException("Server terminated the session: {}".format(reason))
-            
-        return wrap_object_list(tobjects.reference), elapsed
-
-    def quit(self, reason=None):
-        """ Sends quit message and end terminates communication. """
-        if not reason is None:
-            trax_terminate(self._handle.reference, reason.encode('utf-8'))
-        else:
-            trax_terminate(self._handle.reference, None)
+            raise TraxException("Exception when terminating: {}".format(message))
 
-        if self._logger and self._logger.interrupted:
-            raise KeyboardInterrupt("Interrupted by user in log callback")
+        self._handle = None
```

### Comparing `vot-trax-4.0.1/trax/debug.c` & `vot-trax-4.0.2/trax/debug.c`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.1/trax/debug.h` & `vot-trax-4.0.2/trax/debug.h`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.1/trax/image.py` & `vot-trax-4.0.2/trax/image.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,121 @@
 """
 Image description classes.
 """
 
 #from __future__ import absolute
 
+__all__ = ['Image', 'FileImage', 'URLImage', 'MemoryImage', 'BufferImage', 'ImageChannel']
+
 from abc import abstractmethod
 from ctypes import memmove, byref, c_int, string_at
 
 from ._ctypes import \
         trax_image_create_path, trax_image_create_memory, \
         trax_image_get_memory_header, trax_image_get_type, \
         trax_image_get_path, trax_image_get_url, \
         trax_image_create_url, trax_image_get_memory_row, \
         trax_image_write_memory_row, trax_image_get_buffer, \
         trax_image_create_buffer
-from trax import TraxException, ImageWrapper
 
 class ImageChannel(object):
+    """ Image channel identifier. """
+
     COLOR = "color"
     DEPTH = "depth"
     IR = "ir"
 
     @staticmethod
-    def decode(intcode):
+    def decode(intcode: int):
+        """ Decode an image channel from an integer code.
+        
+        Args:
+            intcode (int): Integer code.
+        """
         if intcode == 1:
             return ImageChannel.COLOR
         elif intcode == 2:
             return ImageChannel.DEPTH
         elif intcode == 4:
             return ImageChannel.IR
         raise IndexError("Illegal image channel identifier {}".format(intcode))
 
     @staticmethod
-    def decode_list(intcode):
+    def decode_list(intcode: int):
+        """ Decode a list of image channels from an integer code.
+        
+        Args:
+            intcode (int): Integer code.
+        """
         decoded = []
         if intcode & 1:
             decoded.append(ImageChannel.COLOR)
         if intcode & 2:
             decoded.append(ImageChannel.DEPTH)
         if intcode & 4:
             decoded.append(ImageChannel.IR)
         return decoded
 
     @staticmethod
     def encode(strcode):
+        """ Encode an image channel into an integer code."""
         if strcode == ImageChannel.COLOR:
             return 1
         elif strcode == ImageChannel.DEPTH:
             return 2
         elif strcode == ImageChannel.IR:
             return 4
         raise IndexError("Illegal image channel name {}".format(strcode))
 
     @staticmethod
     def encode_list(list):
-
+        """ Encode a list of image channels into an integer code.
+        
+        Args:
+            list (list): List of image channels.
+        
+        Returns:
+            int: Integer code.
+        """
         encoded = 0
 
         for format in list:
             encoded = encoded | ImageChannel.encode(format)
 
         return encoded
 
 class Image(object):
+    """ Image description class. """
 
     PATH = "path"
     URL = "url"
     MEMORY = "memory"
     BUFFER = "buffer"
 
     """ Image saved in memory as a numpy array """
     def __init__(self, internal):
+        from . import ImageWrapper
         self._ref = ImageWrapper(internal)
 
     @property
     def reference(self):
+        """ Get reference to the internal object.
+    
+        Returns:
+            c_void_p: Reference to the internal object.
+        """
         return self._ref.reference
 
     @staticmethod
     def decode_list(intcode):
+        """ Decode a list of image formats from an integer code.
+        
+        Args:
+            intcode (int): Integer code.
+        """
         decoded = []
         if intcode & 1:
             decoded.append(Image.PATH)
         if intcode & 2:
             decoded.append(Image.URL)
         if intcode & 4:
             decoded.append(Image.MEMORY)
@@ -100,14 +133,15 @@
         if type == 4:
             return MemoryImage(internal)
         if type == 8:
             return BufferImage(internal)
 
     @abstractmethod
     def type(self):
+        """ Get image type """
         pass
 
     @staticmethod
     def encode(strcode):
         if strcode == Image.PATH:
             return 1
         elif strcode == Image.URL:
@@ -117,14 +151,22 @@
         elif strcode == Image.BUFFER:
             return 8
         raise IndexError("Illegal image format name {}".format(strcode))
 
 
     @staticmethod
     def encode_list(list):
+        """ Encode a list of image formats into an integer code.
+        
+        Args:
+            list (list): List of image formats.
+        
+        Returns:
+            int: Integer code.
+        """
 
         encoded = 0
 
         for format in list:
             encoded = encoded | Image.encode(format)
 
         return encoded
@@ -145,136 +187,168 @@
     def type(self):
         return Image.PATH
 
     def path(self):
         return trax_image_get_path(self.reference).decode('utf8')
 
 class URLImage(Image):
-    """
-    Image saved in a local or remote resource
+    """Image saved in a local or remote resource
     """
 
     @staticmethod
-    def create(url = None):
+    def create(url: str = None):
+        """ Create a new URL image resource.
+        
+        Args:
+            url (str): URL of the resource.
+        """
         return URLImage(trax_image_create_url(url.encode('utf8')))
 
-    def __str__(self):
-        """ Get description """
+    def __str__(self) -> str:
+        """ Get description 
+        
+        Returns:
+            str: Description of the image
+        """
         return "URL resource at '{}'".format(trax_image_get_url(self.reference))
 
     def type(self):
+        """ Get image type
+        
+        Returns:
+            str: Image type
+        """
         return Image.URL
 
     def url(self):
+        """ Get image URL
+        
+        Returns:
+            str: Image URL
+        """
         return trax_image_get_url(self.reference).decode('utf8')
 
-try:
-    import numpy as np
 
-    IMAGE_MEMORY_GRAY8 = 1
+IMAGE_MEMORY_GRAY8 = 1
+IMAGE_MEMORY_GRAY16 = 2
+IMAGE_MEMORY_RGB = 3
 
-    IMAGE_MEMORY_GRAY16 = 2
+_image_memory_map_string = {IMAGE_MEMORY_RGB : "rgb", IMAGE_MEMORY_GRAY8: "gray8", IMAGE_MEMORY_GRAY16: "gray16" }
+_image_memory_map_ch = {IMAGE_MEMORY_RGB : 3, IMAGE_MEMORY_GRAY8: 1, IMAGE_MEMORY_GRAY16: 1}
 
-    IMAGE_MEMORY_RGB = 3
+class MemoryImage(Image):
+    """ Image saved in memory as a numpy array """
 
-    _image_memory_map_string = {IMAGE_MEMORY_RGB : "rgb", IMAGE_MEMORY_GRAY8: "gray8", IMAGE_MEMORY_GRAY16: "gray16" }
-    _image_memory_map_dtype = {IMAGE_MEMORY_RGB : np.uint8, IMAGE_MEMORY_GRAY8: np.uint8, IMAGE_MEMORY_GRAY16: np.uint16 }
-    _image_memory_map_ch = {IMAGE_MEMORY_RGB : 3, IMAGE_MEMORY_GRAY8: 1, IMAGE_MEMORY_GRAY16: 1}
+    @staticmethod
+    def create(image: "numpy.ndarray"):
+        """ Create a new memory image resource. 
+
+        Args:
+            image (np.ndarray): Image data.
+        """
 
-    class MemoryImage(Image):
+        from . import TraxException
 
-        @staticmethod
-        def create(image: np.ndarray):
+        try:
+            import numpy as np
 
             assert(isinstance(image, np.ndarray))
 
             image = np.ascontiguousarray(image)
 
-            width = image.shape[1]
-            height = image.shape[0]
-            format = 0
-            if len(image.shape) == 3 and image.shape[2] == 3:
-                if image.itemsize == 1:
-                    format = IMAGE_MEMORY_RGB
-            elif len(image.shape) == 2 or image.shape[2] == 1:
-                if image.itemsize == 1:
-                    format = IMAGE_MEMORY_GRAY8
-                elif image.itemsize == 2:
-                    format = IMAGE_MEMORY_GRAY16
-
-            if format == 0:
-                raise TraxException("Image format not supported")
-
-            timage = trax_image_create_memory(width, height, format)
+        except ImportError:
+            from . import TraxException
+            raise TraxException("Numpy is not installed")
+
+        width = image.shape[1]
+        height = image.shape[0]
+        format = 0
+        if len(image.shape) == 3 and image.shape[2] == 3:
+            if image.itemsize == 1:
+                format = IMAGE_MEMORY_RGB
+        elif len(image.shape) == 2 or image.shape[2] == 1:
+            if image.itemsize == 1:
+                format = IMAGE_MEMORY_GRAY8
+            elif image.itemsize == 2:
+                format = IMAGE_MEMORY_GRAY16
+
+        if format == 0:
+            raise TraxException("Image format not supported")
+
+        timage = trax_image_create_memory(width, height, format)
+
+        data = trax_image_write_memory_row(timage, 0)
+        
+        memmove(data, image.ctypes, image.nbytes)
+        return MemoryImage(timage)
 
-            data = trax_image_write_memory_row(timage, 0)
-            
-            memmove(data, image.ctypes, image.nbytes)
-            return MemoryImage(timage)
-
-        def __str__(self):
-            """ Get description """
-            width = c_int()
-            height = c_int()
-            format = c_int()
-            trax_image_get_memory_header(self.reference, byref(width), byref(height), byref(format))
+    def __str__(self):
+        """ Get description """
+        width = c_int()
+        height = c_int()
+        format = c_int()
+        trax_image_get_memory_header(self.reference, byref(width), byref(height), byref(format))
 
-            return "Raw image of size {}x{}, format {}".format(width.value, height.value, _image_memory_map_string[format.value])
+        return "Raw image of size {}x{}, format {}".format(width.value, height.value, _image_memory_map_string[format.value])
 
-        def type(self):
-            return Image.MEMORY
+    def type(self):
+        return Image.MEMORY
 
-        def array(self):
+    def array(self):
+        try:
+            import numpy as np
+            _image_memory_map_dtype = {IMAGE_MEMORY_RGB : np.uint8, IMAGE_MEMORY_GRAY8: np.uint8, IMAGE_MEMORY_GRAY16: np.uint16 }
+            
             width = c_int()
             height = c_int()
             format = c_int()
             trax_image_get_memory_header(self.reference, byref(width), byref(height), byref(format))
             mat = np.ones((height.value, width.value, _image_memory_map_ch[format.value]), dtype=_image_memory_map_dtype[format.value])
 
             data = trax_image_get_memory_row(self.reference, 0)
 
             memmove(mat.ctypes.data, data, mat.nbytes)
 
             return mat
-except ImportError:
+        except ImportError:
+            from . import TraxException
+            raise TraxException("NumPy is not installed")
 
-    class MemoryImage(Image):
-        def __str__(self):
-            """ Get description """
-            width = c_int()
-            height = c_int()
-            format = c_int()
-            trax_image_get_memory_header(self.reference, byref(width), byref(height), byref(format))
-            return "Raw image of size {}x{}, format {}".format(width.value, height.value, _image_memory_map_string[format.value])
-
-        def type(self):
-            return Image.MEMORY
 
 IMAGE_BUFFER_JPEG = 1
-
 IMAGE_BUFFER_PNG = 2
 
 _image_buffer_map_string = {IMAGE_BUFFER_JPEG : "jpeg", IMAGE_BUFFER_PNG: "png"}
 
 class BufferImage(Image):
-
-    """ Image encoded in a memory buffer stored in JPEG or PNG file format """
+    """ Image encoded in a memory buffer stored in JPEG or PNG file format."""
     @staticmethod
-    def create(data):
+    def create(data: bytes):
+        """ Create image from a memory buffer
+        
+        Args:
+            data: A memory buffer containing the encoded image.
+        """
         tbuffer = trax_image_create_buffer(len(data), data)
         return BufferImage(tbuffer)
 
     def __str__(self):
         """ Get description """
         length = c_int()
         format = c_int()
         trax_image_get_buffer(self.reference, byref(length), byref(format))
         return "Encoded image (format: {}, size: {})".format(_image_buffer_map_string[format.value], length.value)
 
     def type(self):
+        """ Get image type"""
         return Image.BUFFER
 
     def buffer(self):
+        """ Get image buffer 
+        
+        Returns:
+            A memory buffer containing the encoded image.
+        """
         length = c_int()
         format = c_int()
         data = trax_image_get_buffer(self.reference, byref(length), byref(format))
         return string_at(data, length.value)
```

### Comparing `vot-trax-4.0.1/trax/message.c` & `vot-trax-4.0.2/trax/message.c`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.1/trax/message.h` & `vot-trax-4.0.2/trax/message.h`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.1/trax/region.c` & `vot-trax-4.0.2/trax/region.c`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.1/trax/region.h` & `vot-trax-4.0.2/trax/region.h`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.1/trax/strmap.c` & `vot-trax-4.0.2/trax/strmap.c`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.1/trax/strmap.h` & `vot-trax-4.0.2/trax/strmap.h`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.1/trax/trax.c` & `vot-trax-4.0.2/trax/trax.c`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1460,21 +1460,21 @@
 
     arguments = list_create(1);
     tmp_properties = trax_properties_create();
 
     if (reason)
         trax_properties_set(tmp_properties, "trax.reason", reason);
 
+    handle->flags |= TRAX_FLAG_TERMINATED;
+
     write_message((message_stream*)handle->stream, &LOGGER(handle), TRAX_QUIT, arguments, tmp_properties);
 
     list_destroy(&arguments);
     trax_properties_release(&tmp_properties);
 
-    handle->flags |= TRAX_FLAG_TERMINATED;
-
     return TRAX_OK;
 
 }
 
 int trax_cleanup(trax_handle** handle) {
 
     if (!*handle) return -1;
```

### Comparing `vot-trax-4.0.1/trax/trax.h` & `vot-trax-4.0.2/trax/trax.h`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.1/trax/traxpp.cpp` & `vot-trax-4.0.2/trax/traxpp.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,14 @@
 
 	return Metadata(handle->metadata);
 
 }
 
 bool Handle::terminate(const std::string reason) {
 	if (!claims()) return -1;
-
 	return trax_terminate(handle, reason.c_str()) == TRAX_OK;
 }
 
 std::string Handle::get_error() {
 	if (!claims()) return std::string();
 
 	const char* error = trax_get_error(handle);
```

