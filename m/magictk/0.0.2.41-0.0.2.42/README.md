# Comparing `tmp/magictk-0.0.2.41.tar.gz` & `tmp/magictk-0.0.2.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.41.tar", last modified: Fri Apr 19 14:17:08 2024, max compression
+gzip compressed data, was "magictk-0.0.2.42.tar", last modified: Sat Apr 20 10:07:06 2024, max compression
```

## Comparing `magictk-0.0.2.41.tar` & `magictk-0.0.2.42.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:17:08.307055 magictk-0.0.2.41/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-19 14:17:07.000000 magictk-0.0.2.41/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-19 14:17:08.307055 magictk-0.0.2.41/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1376 2024-04-19 14:17:07.000000 magictk-0.0.2.41/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:17:08.307055 magictk-0.0.2.41/magictk/
--rw-r--r--   0 root         (0) root         (0)      323 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9778 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)    13450 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11146 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    11910 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)    15906 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/icon.ico
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     6036 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0)    21933 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/res.pickle
--rw-r--r--   0 root         (0) root         (0)     6077 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10457 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-19 14:17:07.000000 magictk-0.0.2.41/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:17:08.307055 magictk-0.0.2.41/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-19 14:17:08.000000 magictk-0.0.2.41/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2024-04-19 14:17:08.000000 magictk-0.0.2.41/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 14:17:08.000000 magictk-0.0.2.41/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-19 14:17:08.000000 magictk-0.0.2.41/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 14:17:08.307055 magictk-0.0.2.41/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-19 14:17:07.000000 magictk-0.0.2.41/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 10:07:06.067696 magictk-0.0.2.42/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-20 10:07:05.000000 magictk-0.0.2.42/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-20 10:07:06.067696 magictk-0.0.2.42/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-04-20 10:07:05.000000 magictk-0.0.2.42/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 10:07:06.063696 magictk-0.0.2.42/magictk/
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)     3253 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/basicwindow.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11146 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    12040 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     5893 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0)    21933 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     6077 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 10:07:06.067696 magictk-0.0.2.42/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-20 10:07:06.000000 magictk-0.0.2.42/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 10:07:06.067696 magictk-0.0.2.42/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-20 10:07:05.000000 magictk-0.0.2.42/setup.py
```

### Comparing `magictk-0.0.2.41/PKG-INFO` & `magictk-0.0.2.42/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.41
+Version: 0.0.2.42
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.41/README.md` & `magictk-0.0.2.42/README.md`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.41/magictk/_window_ctl.py` & `magictk-0.0.2.42/magictk/_window_ctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 import tkinter
 from tkinter import ttk
-try:
-    import color_tmpl
-except:
-    from magictk import color_tmpl
-try:
-    import photoload
-except:
-    from magictk import photoload
+from magictk import color_tmpl
+from magictk import photoload
 
 
 def exit_btn_set(self, root):
     img_exit = photoload.loadimg("close")
     img_act_exit = photoload.loadimg("close_active")
     self.style.configure(
         'BarExitButton.TFrame', background=self.color["background"])
```

### Comparing `magictk-0.0.2.41/magictk/_window_size.py` & `magictk-0.0.2.42/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.41/magictk/button.py` & `magictk-0.0.2.42/magictk/button.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.41/magictk/checkbox.py` & `magictk-0.0.2.42/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.41/magictk/color_tmpl.py` & `magictk-0.0.2.42/magictk/color_tmpl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.41/magictk/entry.py` & `magictk-0.0.2.42/magictk/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,25 +244,27 @@
             if (anim_magictk not in self.root.anim):
                 self.root.anim.append(anim_magictk)
                 self.__anim_obj_id = self.root.anim[-1]
 
     def __bind_event(self):
         def closecallback(obj):
             if (self.__is_hover == 1):
-                if sys.platform.startswith("linux"):
+                if sys.platform.startswith("linux") and self.root.FRAME_INFO == "Custom":
                     self.top.destroy()
                 self.__is_hover = 0
                 self.canvas.focus_force()
 
         def pressrelease_v(event: tkinter.Event):
             if (self.__is_hover == 1):
-                closecallback(event)
+                pass
+                # closecallback(event)
             else:
                 self.__is_hover = 1
-                if sys.platform.startswith("linux"):  # what's fuck?
+                # what's fuck?
+                if sys.platform.startswith("linux") and self.root.FRAME_INFO == "Custom":
                     self.top = tkinter.Toplevel()
                     self.top.geometry(
                         f"{1}x{1}+{10000}+{10000}")
                     self.__top_entry = ttk.Entry(self.top, width=self.w)
                     self.__top_entry.place(
                         x=0, y=0, width=self.w, height=self.h)
                 self.root.update()
@@ -281,10 +283,11 @@
                     self.show_label.place_forget()
                     self.packed = False
         self.frames.bind("<ButtonRelease-1>", pressrelease_v)
         self.canvas.bind("<ButtonRelease-1>", pressrelease_v)
         self.inputobj.bind("<ButtonRelease-1>", pressrelease_v)
         self.show_label.bind("<ButtonRelease-1>", pressrelease_v)
         self.__input_textvar.trace_add("write", update_text)
-        # self.frames.bind_all("<FocusOut>", closecallback)
         if (sys.platform.startswith("linux")):
             self.frames.bind("<Leave>", closecallback)
+        else:
+            self.inputobj.bind_all("<FocusOut>", closecallback)
```

### Comparing `magictk-0.0.2.41/magictk/fontconfig.py` & `magictk-0.0.2.42/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.41/magictk/icon.ico` & `magictk-0.0.2.42/magictk/icon.ico`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.41/magictk/photoload.py` & `magictk-0.0.2.42/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.41/magictk/progressbar.py` & `magictk-0.0.2.42/magictk/progressbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 import json
 import tkinter
 from tkinter import ttk
-from tkinter import font as tkfont
-try:
-    import color_tmpl
-except ImportError:
-    from magictk import color_tmpl
-try:
-    import photoload
-except ImportError:
-    from magictk import photoload
+from magictk import color_tmpl
+from magictk import photoload
 
 
 class ProgressBar:
     color = color_tmpl.default_color
     __fill_obj = {}
     progress = 0.0
     __progress_pixel = 0
```

### Comparing `magictk-0.0.2.41/magictk/res.pickle` & `magictk-0.0.2.42/magictk/res.pickle`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.41/magictk/select.py` & `magictk-0.0.2.42/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.41/magictk/submenu.py` & `magictk-0.0.2.42/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.41/magictk/window.py` & `magictk-0.0.2.42/magictk/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,16 @@
 import time
 import tkinter
 import os
 from tkinter import ttk
-try:
-    import color_tmpl
-except ImportError:
-    from magictk import color_tmpl
-try:
-    import _window_ctl
-except ImportError:
-    from magictk import _window_ctl
-try:
-    import _window_size
-except ImportError:
-    from magictk import _window_size
-try:
-    import workspace
-except ImportError:
-    from magictk import workspace
-try:
-    import photoload
-except ImportError:
-    from magictk import photoload
+from magictk import color_tmpl
+from magictk import _window_ctl
+from magictk import _window_size
+from magictk import workspace
+from magictk import photoload
 import sys
 
 WIN_INF = -10000
 
 
 class Window(ttk.Frame):
     x = 200
@@ -39,14 +24,15 @@
     fullscreen = False
     minmode = False
     color = color_tmpl.default_color
     anim = []
     disable_move = False
     min_w = 200
     min_h = 100
+    FRAME_INFO = "Custom"
 
     def update_size(self) -> None:
         self.tk_w_without_bar.set(self.w-48*3)
         self.place(x=8, y=self.top_h+1+8, width=self.w-16, height=self.h-1-16)
         self.main_tk.geometry(
             f"{self.w}x{self.h+self.top_h}+{self.x}+{self.y}")
         self.__fake_tk.geometry(
```

### Comparing `magictk-0.0.2.41/magictk/workspace.py` & `magictk-0.0.2.42/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.41/magictk.egg-info/PKG-INFO` & `magictk-0.0.2.42/magictk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.41
+Version: 0.0.2.42
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.41/magictk.egg-info/SOURCES.txt` & `magictk-0.0.2.42/magictk.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 MANIFEST.in
 README.md
 setup.py
 ./magictk/__init__.py
 ./magictk/_window_ctl.py
 ./magictk/_window_size.py
+./magictk/basicwindow.py
 ./magictk/button.py
 ./magictk/checkbox.py
 ./magictk/color_tmpl.py
 ./magictk/entry.py
 ./magictk/fontconfig.py
 ./magictk/frame.py
 ./magictk/icon.ico
```

### Comparing `magictk-0.0.2.41/setup.py` & `magictk-0.0.2.42/setup.py`

 * *Files identical despite different names*

