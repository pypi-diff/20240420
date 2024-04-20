# Comparing `tmp/pywebio_battery-0.5.1.tar.gz` & `tmp/pywebio_battery-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywebio_battery-0.5.1.tar", last modified: Fri Nov  3 09:33:45 2023, max compression
+gzip compressed data, was "pywebio_battery-0.6.0.tar", last modified: Sat Apr 20 15:26:03 2024, max compression
```

## Comparing `pywebio_battery-0.5.1.tar` & `pywebio_battery-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:33:45.408239 pywebio_battery-0.5.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2023-11-03 09:33:32.000000 pywebio_battery-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-11-03 09:33:45.408239 pywebio_battery-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-11-03 09:33:32.000000 pywebio_battery-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:33:45.404238 pywebio_battery-0.5.1/pywebio_battery/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-11-03 09:33:32.000000 pywebio_battery-0.5.1/pywebio_battery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-11-03 09:33:32.000000 pywebio_battery-0.5.1/pywebio_battery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2023-11-03 09:33:32.000000 pywebio_battery-0.5.1/pywebio_battery/file_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    14554 2023-11-03 09:33:32.000000 pywebio_battery-0.5.1/pywebio_battery/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7466 2023-11-03 09:33:32.000000 pywebio_battery-0.5.1/pywebio_battery/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:33:45.404238 pywebio_battery-0.5.1/pywebio_battery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-11-03 09:33:45.000000 pywebio_battery-0.5.1/pywebio_battery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-11-03 09:33:45.000000 pywebio_battery-0.5.1/pywebio_battery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 09:33:45.000000 pywebio_battery-0.5.1/pywebio_battery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-03 09:33:45.000000 pywebio_battery-0.5.1/pywebio_battery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-03 09:33:45.000000 pywebio_battery-0.5.1/pywebio_battery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 09:33:45.408239 pywebio_battery-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-11-03 09:33:32.000000 pywebio_battery-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:26:03.327672 pywebio_battery-0.6.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-20 15:26:03.327672 pywebio_battery-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:26:03.327672 pywebio_battery-0.6.0/pywebio_battery/
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/pywebio_battery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/pywebio_battery/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/pywebio_battery/file_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14717 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/pywebio_battery/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/pywebio_battery/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:26:03.327672 pywebio_battery-0.6.0/pywebio_battery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-20 15:26:03.000000 pywebio_battery-0.6.0/pywebio_battery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-20 15:26:03.000000 pywebio_battery-0.6.0/pywebio_battery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 15:26:03.000000 pywebio_battery-0.6.0/pywebio_battery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 15:26:03.000000 pywebio_battery-0.6.0/pywebio_battery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 15:26:03.000000 pywebio_battery-0.6.0/pywebio_battery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 15:26:03.327672 pywebio_battery-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/setup.py
```

### Comparing `pywebio_battery-0.5.1/LICENSE` & `pywebio_battery-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywebio_battery-0.5.1/PKG-INFO` & `pywebio_battery-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebio_battery
-Version: 0.5.1
+Version: 0.6.0
 Summary: Utilities that help write PyWebIO apps quickly and easily.
 Home-page: https://pywebio.readthedocs.io/en/latest/battery.html
 Author: WeiminWang
 Author-email: wang0.618@qq.com
 License: MIT
 Project-URL: Documentation, https://pywebio.readthedocs.io/en/latest/battery.html
 Project-URL: Source, https://github.com/wang0618/pywebio-battery
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pywebio_battery Version: 0.5.1 Summary: Utilities
+Metadata-Version: 2.1 Name: pywebio_battery Version: 0.6.0 Summary: Utilities
 that help write PyWebIO apps quickly and easily. Home-page: https://
 pywebio.readthedocs.io/en/latest/battery.html Author: WeiminWang Author-email:
 wang0.618@qq.com License: MIT Project-URL: Documentation, https://
 pywebio.readthedocs.io/en/latest/battery.html Project-URL: Source, https://
 github.com/wang0618/pywebio-battery Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
```

### Comparing `pywebio_battery-0.5.1/README.md` & `pywebio_battery-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pywebio_battery-0.5.1/pywebio_battery/__init__.py` & `pywebio_battery-0.6.0/pywebio_battery/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
    * - `redirect_stdout <pywebio_battery.redirect_stdout>`
      - redirecting stdout to pywebio
 
    * - `run_shell <pywebio_battery.run_shell>`
      - Run command in shell
 
-   * - `put_logbox <pywebio_battery.put_logbox>`, `logbox_append <pywebio_battery.logbox_append>`
+   * - `put_logbox <pywebio_battery.put_logbox>`, `logbox_append <pywebio_battery.logbox_append>`, `logbox_clear <pywebio_battery.logbox_clear>`
      - Logbox widget
 
    * - `put_video <pywebio_battery.put_video>`
      - Output video
 
    * - `put_audio <pywebio_battery.put_audio>`
      - Output audio
```

### Comparing `pywebio_battery-0.5.1/pywebio_battery/file_picker.py` & `pywebio_battery-0.6.0/pywebio_battery/file_picker.py`

 * *Files identical despite different names*

### Comparing `pywebio_battery-0.5.1/pywebio_battery/interaction.py` & `pywebio_battery-0.6.0/pywebio_battery/interaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from pywebio.output import *
 from pywebio.output import Output
 from pywebio.output import OutputPosition
 from pywebio.pin import *
 from pywebio.session import *
 from pywebio.utils import random_str
 
-__all__ = ['confirm', 'popup_input', 'redirect_stdout', 'run_shell', 'put_logbox', 'logbox_append', 'put_video',
-           'put_audio', 'wait_scroll_to_bottom']
+__all__ = ['confirm', 'popup_input', 'redirect_stdout', 'run_shell', 'put_logbox', 'logbox_append', 'logbox_clear', 
+           'put_video', 'put_audio', 'wait_scroll_to_bottom']
 
 
 def confirm(
         title: str,
         content: Union[str, Output, Sequence[Union[str, Output]]] = None,
         *,
         timeout: int = None
@@ -236,14 +236,19 @@
 
 
 def logbox_append(name: str, text: str):
     """Append text to a logbox widget"""
     run_js('$("#webio-logbox-%s").append(document.createTextNode(text))' % name, text=str(text))
 
 
+def logbox_clear(name: str):
+    """Clear all contents of a logbox widget"""
+    pywebio.session.run_js('$("#webio-logbox-%s").empty()' % name)
+
+
 def put_video(src: Union[str, bytes], autoplay: bool = False, loop: bool = False,
               height: int = None, width: int = None, muted: bool = False, poster: str = None,
               scope: str = None, position: int = OutputPosition.BOTTOM) -> Output:
     """Output video
 
     :param str/bytes src: Source of video. It can be a string specifying video URL, a bytes-like object specifying
         the binary content of the video.
```

### Comparing `pywebio_battery-0.5.1/pywebio_battery/web.py` & `pywebio_battery-0.6.0/pywebio_battery/web.py`

 * *Files identical despite different names*

### Comparing `pywebio_battery-0.5.1/pywebio_battery.egg-info/PKG-INFO` & `pywebio_battery-0.6.0/pywebio_battery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebio-battery
-Version: 0.5.1
+Version: 0.6.0
 Summary: Utilities that help write PyWebIO apps quickly and easily.
 Home-page: https://pywebio.readthedocs.io/en/latest/battery.html
 Author: WeiminWang
 Author-email: wang0.618@qq.com
 License: MIT
 Project-URL: Documentation, https://pywebio.readthedocs.io/en/latest/battery.html
 Project-URL: Source, https://github.com/wang0618/pywebio-battery
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pywebio-battery Version: 0.5.1 Summary: Utilities
+Metadata-Version: 2.1 Name: pywebio-battery Version: 0.6.0 Summary: Utilities
 that help write PyWebIO apps quickly and easily. Home-page: https://
 pywebio.readthedocs.io/en/latest/battery.html Author: WeiminWang Author-email:
 wang0.618@qq.com License: MIT Project-URL: Documentation, https://
 pywebio.readthedocs.io/en/latest/battery.html Project-URL: Source, https://
 github.com/wang0618/pywebio-battery Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
```

### Comparing `pywebio_battery-0.5.1/setup.py` & `pywebio_battery-0.6.0/setup.py`

 * *Files identical despite different names*

