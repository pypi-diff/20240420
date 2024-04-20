# Comparing `tmp/mpv-1.0.5.tar.gz` & `tmp/mpv-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpv-1.0.5.tar", last modified: Sat Nov 18 11:04:29 2023, max compression
+gzip compressed data, was "mpv-1.0.6.tar", last modified: Sat Apr 20 10:53:07 2024, max compression
```

## Comparing `mpv-1.0.5.tar` & `mpv-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jaseg     (1000) jaseg     (1000)        0 2023-11-18 11:04:29.171728 mpv-1.0.5/
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)    18092 2023-02-26 12:13:42.000000 mpv-1.0.5/LICENSE.GPL
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)    26530 2023-02-26 12:13:42.000000 mpv-1.0.5/LICENSE.LGPL
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)    15505 2023-11-18 11:04:29.171728 mpv-1.0.5/PKG-INFO
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)    14206 2023-11-18 10:53:08.000000 mpv-1.0.5/README.rst
-drwxr-xr-x   0 jaseg     (1000) jaseg     (1000)        0 2023-11-18 11:04:29.168394 mpv-1.0.5/mpv.egg-info/
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)    15505 2023-11-18 11:04:29.000000 mpv-1.0.5/mpv.egg-info/PKG-INFO
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)      209 2023-11-18 11:04:29.000000 mpv-1.0.5/mpv.egg-info/SOURCES.txt
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)        1 2023-11-18 11:04:29.000000 mpv-1.0.5/mpv.egg-info/dependency_links.txt
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)       50 2023-11-18 11:04:29.000000 mpv-1.0.5/mpv.egg-info/requires.txt
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)        4 2023-11-18 11:04:29.000000 mpv-1.0.5/mpv.egg-info/top_level.txt
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)    88157 2023-11-18 10:57:40.000000 mpv-1.0.5/mpv.py
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)     1302 2023-11-18 10:57:40.000000 mpv-1.0.5/pyproject.toml
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)       38 2023-11-18 11:04:29.171728 mpv-1.0.5/setup.cfg
-drwxr-xr-x   0 jaseg     (1000) jaseg     (1000)        0 2023-11-18 11:04:29.168394 mpv-1.0.5/tests/
--rwxr-xr-x   0 jaseg     (1000) jaseg     (1000)    31867 2023-07-22 14:03:02.000000 mpv-1.0.5/tests/test_mpv.py
+drwxr-xr-x   0 jaseg     (1000) jaseg     (1000)        0 2024-04-20 10:53:07.766564 mpv-1.0.6/
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)    18092 2023-02-26 12:13:42.000000 mpv-1.0.6/LICENSE.GPL
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)    26530 2023-02-26 12:13:42.000000 mpv-1.0.6/LICENSE.LGPL
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)    15505 2024-04-20 10:53:07.766564 mpv-1.0.6/PKG-INFO
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)    14206 2023-11-18 10:53:08.000000 mpv-1.0.6/README.rst
+drwxr-xr-x   0 jaseg     (1000) jaseg     (1000)        0 2024-04-20 10:53:07.766564 mpv-1.0.6/mpv.egg-info/
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)    15505 2024-04-20 10:53:07.000000 mpv-1.0.6/mpv.egg-info/PKG-INFO
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)      209 2024-04-20 10:53:07.000000 mpv-1.0.6/mpv.egg-info/SOURCES.txt
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)        1 2024-04-20 10:53:07.000000 mpv-1.0.6/mpv.egg-info/dependency_links.txt
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)       50 2024-04-20 10:53:07.000000 mpv-1.0.6/mpv.egg-info/requires.txt
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)        4 2024-04-20 10:53:07.000000 mpv-1.0.6/mpv.egg-info/top_level.txt
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)    90580 2024-04-20 10:51:15.000000 mpv-1.0.6/mpv.py
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)     1302 2024-04-20 10:51:15.000000 mpv-1.0.6/pyproject.toml
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)       38 2024-04-20 10:53:07.766564 mpv-1.0.6/setup.cfg
+drwxr-xr-x   0 jaseg     (1000) jaseg     (1000)        0 2024-04-20 10:53:07.766564 mpv-1.0.6/tests/
+-rwxr-xr-x   0 jaseg     (1000) jaseg     (1000)    32984 2024-04-20 10:35:01.000000 mpv-1.0.6/tests/test_mpv.py
```

### Comparing `mpv-1.0.5/LICENSE.GPL` & `mpv-1.0.6/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `mpv-1.0.5/LICENSE.LGPL` & `mpv-1.0.6/LICENSE.LGPL`

 * *Files identical despite different names*

### Comparing `mpv-1.0.5/PKG-INFO` & `mpv-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpv
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python interface to the mpv media player
 Author-email: jaseg <mpv@jaseg.de>
 License: GPLv2+ or LGPLv2.1+
 Project-URL: homepage, https://github.com/jaseg/python-mpv
 Keywords: mpv,library,video,audio,player,display,multimedia
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications
```

### Comparing `mpv-1.0.5/README.rst` & `mpv-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `mpv-1.0.5/mpv.egg-info/PKG-INFO` & `mpv-1.0.6/mpv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpv
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python interface to the mpv media player
 Author-email: jaseg <mpv@jaseg.de>
 License: GPLv2+ or LGPLv2.1+
 Project-URL: homepage, https://github.com/jaseg/python-mpv
 Keywords: mpv,library,video,audio,player,display,multimedia
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications
```

### Comparing `mpv-1.0.5/mpv.py` & `mpv-1.0.6/mpv.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 # This library is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
 # warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License and the GNU
 # Lesser General Public License for more details.
 #
 # You can find copies of the GPLv2 and LGPLv2.1 licenses in the project repository's LICENSE.GPL and LICENSE.LGPL files.
 
-__version__ = '1.0.5'
+__version__ = '1.0.6'
 
 from ctypes import *
 import ctypes.util
 import threading
 import queue
 import os
 import sys
@@ -889,14 +889,16 @@
             self.set_loglevel(loglevel or 'terminal-default')
         if start_event_thread:
             self._event_thread = threading.Thread(target=self._loop, name='MPVEventHandlerThread')
             self._event_thread.daemon = True
             self._event_thread.start()
         else:
             self._event_thread = None
+        if (m := re.search(r'(\d+)\.(\d+)\.(\d+)', self.mpv_version)):
+            self.mpv_version_tuple = tuple(map(int, m.groups()))
 
     @contextmanager
     def _enqueue_exceptions(self):
         try:
             yield
         except Exception as e:
             for fut in self._exception_futures:
@@ -1320,17 +1322,24 @@
         """Mapped mpv playlist-play-index command, see man mpv(1)."""
         self.command('playlist-play-index', idx)
 
     @staticmethod
     def _encode_options(options):
         return ','.join('{}={}'.format(_py_to_mpv(str(key)), str(val)) for key, val in options.items())
 
-    def loadfile(self, filename, mode='replace', **options):
+    def loadfile(self, filename, mode='replace', index=None, **options):
         """Mapped mpv loadfile command, see man mpv(1)."""
-        self.command('loadfile', filename.encode(fs_enc), mode, MPV._encode_options(options))
+        if self.mpv_version_tuple >= (0, 38, 0):
+            if index is None:
+                index = -1
+            self.command('loadfile', filename.encode(fs_enc), mode, index, MPV._encode_options(options))
+        else:
+            if index is not None:
+                warn(f'The index argument to the loadfile command is only supported on mpv >= 0.38.0')
+            self.command('loadfile', filename.encode(fs_enc), mode, MPV._encode_options(options))
 
     def loadlist(self, playlist, mode='replace'):
         """Mapped mpv loadlist command, see man mpv(1)."""
         self.command('loadlist', playlist.encode(fs_enc), mode)
 
     def playlist_clear(self):
         """Mapped mpv playlist_clear command, see man mpv(1)."""
@@ -1940,14 +1949,63 @@
                         self._python_streams[name][0] is not cb: # This is just a basic sanity check
                     raise RuntimeError('Python stream has already been unregistered')
                 del self._python_streams[name]
             cb.unregister = unregister
             return cb
         return register
 
+    @contextmanager
+    def play_context(self):
+        """ Context manager for streaming bytes straight into libmpv.
+
+        This is a convenience wrapper around python_stream. play_context returns a write method, which you can use in
+        the body of the context manager to feed libmpv bytes. All bytes you feed in with write() in the body of a single
+        call of this context manager are treated as one single file. A queue is used internally, so this function is
+        thread-safe. The queue is unlimited, so it cannot block and is safe to call from async code. You can use this
+        function to stream chunked data, e.g. from the network.
+
+        Use it like this:
+
+        with m.play_context() as write:
+            with open(TESTVID, 'rb') as f:
+                while (chunk := f.read(65536)): # Get some chunks of bytes
+                    write(chunk)
+        """
+        q = queue.Queue()
+
+        frame = sys._getframe()
+        stream_name = f'__python_mpv_play_generator_{hash(frame)}'
+        EOF = frame # Get some unique object as EOF marker
+        @self.python_stream(stream_name)
+        def reader():
+            while (chunk := q.get()) is not EOF:
+                if chunk:
+                    yield chunk
+            reader.unregister()
+
+        def write(chunk):
+            q.put(chunk)
+
+        # Start playback before yielding, the first call to reader() will block until write is called at least once.
+        self.play(f'python://{stream_name}')
+        yield write
+        q.put(EOF)
+
+    def play_bytes(self, data):
+        """ Play the given bytes object as a single file. """
+        frame = sys._getframe()
+        stream_name = f'__python_mpv_play_generator_{hash(frame)}'
+
+        @self.python_stream(stream_name)
+        def reader():
+            yield data
+            reader.unregister() # unregister itself
+
+        self.play(f'python://{stream_name}')
+
     def python_stream_catchall(self, cb):
         """ Register a catch-all python stream to be called when no name matches can be found. Use this decorator on a
         function that takes a name argument and returns a (generator, size) tuple (with size being None if unknown).
 
         An invalid URI can be signalled to libmpv by raising a ValueError inside the callback.
 
         See also: @mpv.python_stream(name, size)
```

### Comparing `mpv-1.0.5/pyproject.toml` & `mpv-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ['mpv']
 
 [project]
 name = "mpv"
-version = "v1.0.5"
+version = "v1.0.6"
 description = "A python interface to the mpv media player"
 readme = "README.rst"
 authors = [{name = "jaseg", email = "mpv@jaseg.de"}]
 license = {text = "GPLv2+ or LGPLv2.1+"}
 requires-python = ">=3.7"
 keywords = ['mpv', 'library', 'video', 'audio', 'player', 'display', 'multimedia']
 classifiers = [
```

### Comparing `mpv-1.0.5/tests/test_mpv.py` & `mpv-1.0.6/tests/test_mpv.py`

 * *Files 1% similar despite different names*

```diff
@@ -639,14 +639,52 @@
         m.wait_for_playback(catch_errors=False)
         try:
             assert result.result()
         finally:
             m.terminate()
             disp.stop()
 
+    def test_play_context(self):
+        handler = mock.Mock()
+
+        disp = Display()
+        disp.start()
+        m = mpv.MPV(vo=testvo)
+        def cb(evt):
+            handler(evt.as_dict(decoder=mpv.lazy_decoder))
+        m.register_event_callback(cb)
+
+        with m.play_context() as write:
+            with open(TESTVID, 'rb') as f:
+                write(f.read(100))
+                write(f.read(1000))
+                write(f.read())
+
+        m.wait_for_playback()
+        handler.assert_any_call({'event': 'end-file', 'reason': 'eof', 'playlist_entry_id': 1})
+        m.terminate()
+        disp.stop()
+
+    def test_play_bytes(self):
+        handler = mock.Mock()
+
+        disp = Display()
+        disp.start()
+        m = mpv.MPV(vo=testvo)
+        def cb(evt):
+            handler(evt.as_dict(decoder=mpv.lazy_decoder))
+        m.register_event_callback(cb)
+
+        with open(TESTVID, 'rb') as f:
+            m.play_bytes(f.read())
+
+        m.wait_for_playback()
+        handler.assert_any_call({'event': 'end-file', 'reason': 'eof', 'playlist_entry_id': 1})
+        m.terminate()
+        disp.stop()
 
 
 class TestLifecycle(unittest.TestCase):
     def test_create_destroy(self):
         thread_names = lambda: [ t.name for t in threading.enumerate() ]
         self.assertNotIn('MPVEventHandlerThread', thread_names())
         m = mpv.MPV()
```

