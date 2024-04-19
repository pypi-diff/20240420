# Comparing `tmp/grpcio-testing-1.62.2.tar.gz` & `tmp/grpcio-testing-1.63.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grpcio-testing-1.62.2.tar", last modified: Wed Apr 17 17:51:51 2024, max compression
+gzip compressed data, was "grpcio-testing-1.63.0rc1.tar", last modified: Fri Apr 12 06:40:43 2024, max compression
```

## Comparing `grpcio-testing-1.62.2.tar` & `grpcio-testing-1.63.0rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:51:51.000000 grpcio-testing-1.62.2/
--rw-r--r--   0 root         (0) root         (0)    29687 2024-04-17 17:51:51.000000 grpcio-testing-1.62.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      510 2024-04-17 17:51:51.000000 grpcio-testing-1.62.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      266 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:51:51.000000 grpcio-testing-1.62.2/grpc_testing/
--rw-r--r--   0 root         (0) root         (0)    22799 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:51:51.000000 grpcio-testing-1.62.2/grpc_testing/_channel/
--rw-r--r--   0 root         (0) root         (0)      887 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_channel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2671 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_channel/_channel.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_channel/_channel_rpc.py
--rw-r--r--   0 root         (0) root         (0)     1782 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_channel/_channel_state.py
--rw-r--r--   0 root         (0) root         (0)     8036 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_channel/_invocation.py
--rw-r--r--   0 root         (0) root         (0)     4933 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_channel/_multi_callable.py
--rw-r--r--   0 root         (0) root         (0)     7246 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_channel/_rpc_state.py
--rw-r--r--   0 root         (0) root         (0)     4406 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:51:51.000000 grpcio-testing-1.62.2/grpc_testing/_server/
--rw-r--r--   0 root         (0) root         (0)      782 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7428 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_server/_handler.py
--rw-r--r--   0 root         (0) root         (0)     5273 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_server/_rpc.py
--rw-r--r--   0 root         (0) root         (0)     6096 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_server/_server.py
--rw-r--r--   0 root         (0) root         (0)     2460 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_server/_server_rpc.py
--rw-r--r--   0 root         (0) root         (0)     2846 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_server/_service.py
--rw-r--r--   0 root         (0) root         (0)     2631 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_server/_servicer_context.py
--rw-r--r--   0 root         (0) root         (0)     7256 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_testing/_time.py
--rw-r--r--   0 root         (0) root         (0)      697 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:51:51.000000 grpcio-testing-1.62.2/grpcio_testing.egg-info/
--rw-r--r--   0 root         (0) root         (0)      510 2024-04-17 17:51:51.000000 grpcio-testing-1.62.2/grpcio_testing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1416 2024-04-17 17:51:51.000000 grpcio-testing-1.62.2/grpcio_testing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:51:51.000000 grpcio-testing-1.62.2/grpcio_testing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-04-17 17:51:51.000000 grpcio-testing-1.62.2/grpcio_testing.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-17 17:51:51.000000 grpcio-testing-1.62.2/grpcio_testing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 17:51:51.000000 grpcio-testing-1.62.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2320 2024-04-17 17:04:28.000000 grpcio-testing-1.62.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.014548 grpcio-testing-1.63.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    29687 2024-04-12 06:40:42.000000 grpcio-testing-1.63.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-12 06:40:43.014548 grpcio-testing-1.63.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      266 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.006547 grpcio-testing-1.63.0rc1/grpc_testing/
+-rw-r--r--   0 root         (0) root         (0)    22799 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.010548 grpcio-testing-1.63.0rc1/grpc_testing/_channel/
+-rw-r--r--   0 root         (0) root         (0)      887 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/_channel.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/_channel_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/_channel_state.py
+-rw-r--r--   0 root         (0) root         (0)     8036 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     4933 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/_multi_callable.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/_rpc_state.py
+-rw-r--r--   0 root         (0) root         (0)     4406 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.010548 grpcio-testing-1.63.0rc1/grpc_testing/_server/
+-rw-r--r--   0 root         (0) root         (0)      782 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7428 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5273 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     6096 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/_server.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/_server_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/_service.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/_servicer_context.py
+-rw-r--r--   0 root         (0) root         (0)     7256 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_time.py
+-rw-r--r--   0 root         (0) root         (0)      700 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.014548 grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-12 06:40:42.000000 grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1416 2024-04-12 06:40:42.000000 grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 06:40:42.000000 grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-12 06:40:42.000000 grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-12 06:40:42.000000 grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 06:40:43.014548 grpcio-testing-1.63.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2320 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grpcio-testing-1.62.2/LICENSE` & `grpcio-testing-1.63.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/__init__.py` & `grpcio-testing-1.63.0rc1/grpc_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_channel/__init__.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_channel/_channel.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_channel/_channel.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,31 +27,50 @@
 
     def subscribe(self, callback, try_to_connect=False):
         raise NotImplementedError()
 
     def unsubscribe(self, callback):
         raise NotImplementedError()
 
+    def _get_registered_call_handle(self, method: str) -> int:
+        pass
+
     def unary_unary(
-        self, method, request_serializer=None, response_deserializer=None
+        self,
+        method,
+        request_serializer=None,
+        response_deserializer=None,
+        _registered_method=False,
     ):
         return _multi_callable.UnaryUnary(method, self._state)
 
     def unary_stream(
-        self, method, request_serializer=None, response_deserializer=None
+        self,
+        method,
+        request_serializer=None,
+        response_deserializer=None,
+        _registered_method=False,
     ):
         return _multi_callable.UnaryStream(method, self._state)
 
     def stream_unary(
-        self, method, request_serializer=None, response_deserializer=None
+        self,
+        method,
+        request_serializer=None,
+        response_deserializer=None,
+        _registered_method=False,
     ):
         return _multi_callable.StreamUnary(method, self._state)
 
     def stream_stream(
-        self, method, request_serializer=None, response_deserializer=None
+        self,
+        method,
+        request_serializer=None,
+        response_deserializer=None,
+        _registered_method=False,
     ):
         return _multi_callable.StreamStream(method, self._state)
 
     def _close(self):
         # TODO(https://github.com/grpc/grpc/issues/12531): Decide what
         # action to take here, if any?
         pass
```

### Comparing `grpcio-testing-1.62.2/grpc_testing/_channel/_channel_rpc.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_channel/_channel_rpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_channel/_channel_state.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_channel/_channel_state.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_channel/_invocation.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_channel/_invocation.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_channel/_multi_callable.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_channel/_multi_callable.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_channel/_rpc_state.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_channel/_rpc_state.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_common.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_common.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_server/__init__.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_server/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_server/_handler.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_server/_handler.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_server/_rpc.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_server/_rpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_server/_server.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_server/_server.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_server/_server_rpc.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_server/_server_rpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_server/_service.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_server/_service.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_server/_servicer_context.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_server/_servicer_context.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_testing/_time.py` & `grpcio-testing-1.63.0rc1/grpc_testing/_time.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/grpc_version.py` & `grpcio-testing-1.63.0rc1/grpc_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_testing/grpc_version.py.template`!!!
 
-VERSION = '1.62.2'
+VERSION = '1.63.0rc1'
```

### Comparing `grpcio-testing-1.62.2/grpcio_testing.egg-info/SOURCES.txt` & `grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.62.2/setup.py` & `grpcio-testing-1.63.0rc1/setup.py`

 * *Files identical despite different names*

