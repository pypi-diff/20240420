# Comparing `tmp/ahk-1.6.1.tar.gz` & `tmp/ahk-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.6.1.tar", last modified: Fri Apr  5 07:16:51 2024, max compression
+gzip compressed data, was "ahk-1.6.2.tar", last modified: Fri Apr 19 18:07:03 2024, max compression
```

## Comparing `ahk-1.6.1.tar` & `ahk-1.6.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:16:51.161323 ahk-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-05 07:16:44.000000 ahk-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-05 07:16:44.000000 ahk-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-04-05 07:16:51.161323 ahk-1.6.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:16:51.157323 ahk-1.6.1/ahk/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:16:51.161323 ahk-1.6.1/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   207815 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    49798 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    30508 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (127)   171011 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17089 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:16:51.161323 ahk-1.6.1/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   201095 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    44850 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    27717 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:16:51.161323 ahk-1.6.1/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    80096 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/templates/daemon-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)    80517 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/templates/hotkeys-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-05 07:16:44.000000 ahk-1.6.1/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:16:51.161323 ahk-1.6.1/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-04-05 07:16:51.000000 ahk-1.6.1/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-05 07:16:51.000000 ahk-1.6.1/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:16:51.000000 ahk-1.6.1/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 07:16:51.000000 ahk-1.6.1/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-05 07:16:51.000000 ahk-1.6.1/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-05 07:16:44.000000 ahk-1.6.1/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:16:51.161323 ahk-1.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    26719 2024-04-05 07:16:44.000000 ahk-1.6.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-05 07:16:44.000000 ahk-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-05 07:16:51.161323 ahk-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 07:16:44.000000 ahk-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:07:03.336205 ahk-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-19 18:06:56.000000 ahk-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 18:06:56.000000 ahk-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-04-19 18:07:03.336205 ahk-1.6.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:07:03.332205 ahk-1.6.2/ahk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:07:03.336205 ahk-1.6.2/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   207858 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49798 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30508 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)   171011 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17089 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:07:03.336205 ahk-1.6.2/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   201138 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44850 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27717 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:07:03.336205 ahk-1.6.2/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    80096 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/templates/daemon-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)    80517 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/templates/hotkeys-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-19 18:06:56.000000 ahk-1.6.2/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:07:03.336205 ahk-1.6.2/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-04-19 18:07:03.000000 ahk-1.6.2/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-19 18:07:03.000000 ahk-1.6.2/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:07:03.000000 ahk-1.6.2/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-19 18:07:03.000000 ahk-1.6.2/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 18:07:03.000000 ahk-1.6.2/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-19 18:06:56.000000 ahk-1.6.2/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:07:03.336205 ahk-1.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26719 2024-04-19 18:06:56.000000 ahk-1.6.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-19 18:06:56.000000 ahk-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-19 18:07:03.340205 ahk-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:06:56.000000 ahk-1.6.2/setup.py
```

### Comparing `ahk-1.6.1/LICENSE` & `ahk-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/PKG-INFO` & `ahk-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.6.1
+Version: 1.6.2
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
```

### Comparing `ahk-1.6.1/ahk/__init__.py` & `ahk-1.6.2/ahk/__init__.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/_async/engine.py` & `ahk-1.6.2/ahk/_async/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -3752,14 +3752,17 @@
             options += MsgBoxOtherOptions.TEXT_RIGHT_JUSTIFIED
         if right_to_left_reading:
             options += MsgBoxOtherOptions.RIGHT_TO_LEFT_READING_ORDER
 
         args = [str(options), title, text]
         if timeout is not None:
             args.append(str(timeout))
+        else:
+            args.append('')
+
         return await self._transport.function_call('AHKMsgBox', args, blocking=blocking)
 
     # fmt: off
     @overload
     async def input_box(self, prompt: str = '', title: str = 'Input', default: str = '', hide: bool = False, width: Optional[int] = None, height: Optional[int] = None, x: Optional[int] = None, y: Optional[int] = None, locale: bool = True, timeout: Optional[int] = None) -> Union[None, str]: ...
     @overload
     async def input_box(self, prompt: str = '', title: str = 'Input', default: str = '', hide: bool = False, width: Optional[int] = None, height: Optional[int] = None, x: Optional[int] = None, y: Optional[int] = None, locale: bool = True, timeout: Optional[int] = None, *, blocking: Literal[False]) -> Union[AsyncFutureResult[str], AsyncFutureResult[None]]: ...
```

### Comparing `ahk-1.6.1/ahk/_async/transport.py` & `ahk-1.6.2/ahk/_async/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/_async/window.py` & `ahk-1.6.2/ahk/_async/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/_constants.py` & `ahk-1.6.2/ahk/_constants.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/_hotkey.py` & `ahk-1.6.2/ahk/_hotkey.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/_sync/engine.py` & `ahk-1.6.2/ahk/_sync/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -3740,14 +3740,17 @@
             options += MsgBoxOtherOptions.TEXT_RIGHT_JUSTIFIED
         if right_to_left_reading:
             options += MsgBoxOtherOptions.RIGHT_TO_LEFT_READING_ORDER
 
         args = [str(options), title, text]
         if timeout is not None:
             args.append(str(timeout))
+        else:
+            args.append('')
+
         return self._transport.function_call('AHKMsgBox', args, blocking=blocking)
 
     # fmt: off
     @overload
     def input_box(self, prompt: str = '', title: str = 'Input', default: str = '', hide: bool = False, width: Optional[int] = None, height: Optional[int] = None, x: Optional[int] = None, y: Optional[int] = None, locale: bool = True, timeout: Optional[int] = None) -> Union[None, str]: ...
     @overload
     def input_box(self, prompt: str = '', title: str = 'Input', default: str = '', hide: bool = False, width: Optional[int] = None, height: Optional[int] = None, x: Optional[int] = None, y: Optional[int] = None, locale: bool = True, timeout: Optional[int] = None, *, blocking: Literal[False]) -> Union[FutureResult[str], FutureResult[None]]: ...
```

### Comparing `ahk-1.6.1/ahk/_sync/transport.py` & `ahk-1.6.2/ahk/_sync/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/_sync/window.py` & `ahk-1.6.2/ahk/_sync/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/_utils.py` & `ahk-1.6.2/ahk/_utils.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/directives.py` & `ahk-1.6.2/ahk/directives.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/extensions.py` & `ahk-1.6.2/ahk/extensions.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/keys.py` & `ahk-1.6.2/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/message.py` & `ahk-1.6.2/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/templates/daemon-v2.ahk` & `ahk-1.6.2/ahk/templates/daemon-v2.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/templates/daemon.ahk` & `ahk-1.6.2/ahk/templates/daemon.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/templates/hotkeys-v2.ahk` & `ahk-1.6.2/ahk/templates/hotkeys-v2.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk/templates/hotkeys.ahk` & `ahk-1.6.2/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/ahk.egg-info/PKG-INFO` & `ahk-1.6.2/ahk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.6.1
+Version: 1.6.2
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
```

### Comparing `ahk-1.6.1/ahk.egg-info/SOURCES.txt` & `ahk-1.6.2/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/buildunasync.py` & `ahk-1.6.2/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/docs/README.md` & `ahk-1.6.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `ahk-1.6.1/setup.cfg` & `ahk-1.6.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.6.1
+version = 1.6.2
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 project_urls =
```

