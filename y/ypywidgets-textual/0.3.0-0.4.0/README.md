# Comparing `tmp/ypywidgets_textual-0.3.0.tar.gz` & `tmp/ypywidgets_textual-0.4.0.tar.gz`

## Comparing `ypywidgets_textual-0.3.0.tar` & `ypywidgets_textual-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/ypywidgets_textual/__init__.py
--rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/ypywidgets_textual/_driver.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/ypywidgets_textual/button.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/ypywidgets_textual/plotext.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/ypywidgets_textual/switch.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/ypywidgets_textual/widget.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/ypywidgets_textual/txl/button.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/ypywidgets_textual/txl/plotext.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/ypywidgets_textual/txl/switch.py
--rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/ypywidgets_textual/txl/widget.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/.gitignore
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/README.md
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 ypywidgets_textual-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/ypywidgets_textual/__init__.py
+-rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/ypywidgets_textual/_driver.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/ypywidgets_textual/button.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/ypywidgets_textual/plotext.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/ypywidgets_textual/switch.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/ypywidgets_textual/widget.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/ypywidgets_textual/txl/button.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/ypywidgets_textual/txl/plotext.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/ypywidgets_textual/txl/switch.py
+-rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/ypywidgets_textual/txl/widget.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/.gitignore
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/README.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 ypywidgets_textual-0.4.0/PKG-INFO
```

### Comparing `ypywidgets_textual-0.3.0/ypywidgets_textual/_driver.py` & `ypywidgets_textual-0.4.0/ypywidgets_textual/_driver.py`

 * *Files identical despite different names*

### Comparing `ypywidgets_textual-0.3.0/ypywidgets_textual/button.py` & `ypywidgets_textual-0.4.0/ypywidgets_textual/button.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from typing import Callable
 
-from ypywidgets import Widget, reactive
+from ypywidgets import Declare, Widget
 from ypywidgets.comm import CommWidget
 
 
 class ButtonModel(Widget):
 
-    label = reactive("")
-    variant = reactive("default")
-    disabled = reactive(False)
-    _press = reactive(False)
-    _pressed = reactive(False)
+    label = Declare[str]("")
+    variant = Declare[str]("default")
+    disabled = Declare[bool](False)
+    _press = Declare[bool](False)
+    _pressed = Declare[bool](False)
 
     def __init__(
         self,
         label: str | None = None,
         variant: str | None = None,
         disabled: bool | None = None,
         on_button_pressed: Callable[[], None] | None = None,
@@ -43,15 +43,16 @@
     @on_button_pressed.setter
     def on_button_pressed(self, value: Callable[[], None]) -> None:
         self._on_button_pressed = value
 
     def action_press(self):
         self._press = not self._press
 
-    def watch__pressed(self):
+    @_pressed.watch
+    def _watch__pressed(self, old: bool, new: bool):
         self._on_button_pressed()
 
 
 class Button(CommWidget, ButtonModel):
 
     def __init__(
         self,
```

### Comparing `ypywidgets_textual-0.3.0/ypywidgets_textual/plotext.py` & `ypywidgets_textual-0.4.0/ypywidgets_textual/plotext.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
-from ypywidgets import Widget, reactive
+from ypywidgets import Declare, Widget
 from ypywidgets.comm import CommWidget
 
 
 class PlotextModel(Widget):
 
-    _clear_data = reactive(False)
-    _args = reactive([])
-    _scatter = reactive(False)
-    _plot = reactive(False)
-    _title = reactive("")
+    _clear_data = Declare[bool](False)
+    _args = Declare[list]([])
+    _scatter = Declare[bool](False)
+    _plot = Declare[bool](False)
+    _title = Declare[str]("")
 
     def __init__(self, ydoc=None) -> None:
         super().__init__(ydoc)
 
     def clear_data(self) -> None:
         self._clear_data = False
         self._clear_data = True
```

### Comparing `ypywidgets_textual-0.3.0/ypywidgets_textual/switch.py` & `ypywidgets_textual-0.4.0/ypywidgets_textual/switch.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
-from ypywidgets import Widget, reactive
+from ypywidgets import Declare, Widget
 from ypywidgets.comm import CommWidget
 
 
 class SwitchModel(Widget):
-    value = reactive(False)
+    value = Declare[bool](False)
 
     def __init__(
         self,
         value: bool | None = None,
         ydoc=None,
     ) -> None:
         super().__init__(ydoc)
```

### Comparing `ypywidgets_textual-0.3.0/ypywidgets_textual/widget.py` & `ypywidgets_textual-0.4.0/ypywidgets_textual/widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import asyncio
 import json
 from typing import Type
 
 from textual import events
 from textual.app import App
 from textual.geometry import Size
-from ypywidgets import Widget as _Widget, reactive
+from ypywidgets import Declare, Widget as _Widget
 from ypywidgets.comm import CommWidget
 
 from ._driver import Driver
 
 
 class WidgetModel(_Widget):
-    _data_from_app = reactive("")
-    _data_to_app = reactive("")
-    _cols = reactive(0)
-    _rows = reactive(0)
-    _ready = reactive(False)
+    _data_from_app = Declare[str]("")
+    _data_to_app = Declare[str]("")
+    _cols = Declare[int](0)
+    _rows = Declare[int](0)
+    _ready = Declare[bool](False)
 
     def __init__(
         self,
         ydoc=None,
     ) -> None:
         super().__init__(ydoc)
 
@@ -39,27 +39,29 @@
         self._data_to_app_queue = asyncio.Queue()
         self._tasks = [
             asyncio.create_task(self._run()),
             asyncio.create_task(self._send_data()),
             asyncio.create_task(self._recv_data()),
         ]
 
-    def watch__ready(self, value: bool):
-        if value:
-            size = Size(int(self._cols), int(self._rows))
-            loop = asyncio.get_running_loop()
-            event = events.Resize(size, size)
-            asyncio.run_coroutine_threadsafe(
-                self._app._post_message(event),
-                loop=loop,
-            )
-
-    def watch__data_to_app(self, data: str):
-        if data:
-            self._data_to_app_queue.put_nowait(data)
+        @WidgetModel._ready.watch
+        def _watch__ready(obj, old: bool, value: bool):
+            if value:
+                size = Size(int(obj._cols), int(obj._rows))
+                loop = asyncio.get_running_loop()
+                event = events.Resize(size, size)
+                asyncio.run_coroutine_threadsafe(
+                    self._app._post_message(event),
+                    loop=loop,
+                )
+
+        @WidgetModel._data_to_app.watch
+        def _watch__data_to_app(obj, old:str, data: str):
+            if data:
+                obj._data_to_app_queue.put_nowait(data)
 
     async def _send_data(self):
         while True:
             data = await self._data_from_app_queue.get()
             self._data_from_app = ""
             self._data_from_app = data.decode()
```

### Comparing `ypywidgets_textual-0.3.0/ypywidgets_textual/txl/button.py` & `ypywidgets_textual-0.4.0/ypywidgets_textual/txl/button.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,31 @@
 
 
 class Button(TextualButton):
 
     def __init__(self, model: ButtonModel) -> None:
         super().__init__()
         self.ymodel = model
-        model.watch__press = self.action_press
-        model.watch_label = self._set_label
-        model.watch_variant = self._set_variant
-        model.watch_disabled = self._set_disabled
+
+        @ButtonModel._press.watch
+        def _watch__press(obj, old, new):
+            self.action_press()
+
+        @ButtonModel.label.watch
+        def _watch_label(obj, old: str, new: str):
+            self._set_label(new)
+
+        @ButtonModel.variant.watch
+        def _watch_variant(obj, old: str, new: str):
+            self._set_variant(new)
+
+        @ButtonModel.disabled.watch
+        def _watch_disabled(obj, old: bool, new: bool):
+            self._set_disabled(new)
+
         self._set_label(model.label)
         self._set_variant(model.variant)
         self._set_disabled(model.disabled)
 
     def on_button_pressed(self, event) -> None:
         self.ymodel._pressed = not self.ymodel._pressed
```

### Comparing `ypywidgets_textual-0.3.0/ypywidgets_textual/txl/plotext.py` & `ypywidgets_textual-0.4.0/ypywidgets_textual/txl/plotext.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,31 @@
 
 
 class Plotext(PlotextPlot):
 
     def __init__(self, model: PlotextModel) -> None:
         super().__init__()
         self.ymodel = model
-        model.watch__clear_data = self.clear_data
-        model.watch__scatter = self.scatter
-        model.watch__plot = self.plot
-        model.watch__title = self.title
+
+        @PlotextModel._clear_data.watch
+        def _watch__clear_data(obj, old, new):
+            self.clear_data()
+
+        @PlotextModel._scatter.watch
+        def _watch__scatter(obj, old, new):
+            self.scatter()
+
+        @PlotextModel._plot.watch
+        def _watch__plot(obj, old, new):
+            self.plot()
+
+        @PlotextModel._title.watch
+        def _watch__title(obj, old: str, new: str):
+            self.title(new)
+
         self.clear_data()
         self.scatter()
         self.plot()
         self.title(model._title)
 
     def clear_data(self) -> None:
         if self.ymodel._clear_data:
```

### Comparing `ypywidgets_textual-0.3.0/ypywidgets_textual/txl/widget.py` & `ypywidgets_textual-0.4.0/ypywidgets_textual/txl/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,19 @@
 class Widget(Terminal):
 
     def __init__(self, model: WidgetModel) -> None:
         self.ymodel = model
         self._data_from_app_queue = asyncio.Queue()
         self._data_to_app_queue = asyncio.Queue()
         super().__init__(self._data_to_app_queue, self._data_from_app_queue)
-        model.watch__data_from_app = self._to_terminal
+
+        @WidgetModel._data_from_app.watch
+        def _watch__data_from_app(obj, old: str, new: str):
+            self._to_terminal(new)
+
         self._tasks = [asyncio.create_task(self._from_terminal())]
 
     def _to_terminal(self, data: str) -> None:
         self._data_from_app_queue.put_nowait(data)
 
     async def _from_terminal(self):
         while True:
```

### Comparing `ypywidgets_textual-0.3.0/pyproject.toml` & `ypywidgets_textual-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 [project]
 name = "ypywidgets-textual"
 dynamic = ["version"]
 description = "Textual widgets for ypywidgets"
 readme = "README.md"
 license = "MIT"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
     { name = "David Brochart", email = "david.brochart@gmail.com" },
 ]
 keywords = [
     "widgets",
     "jupyter",
     "ypy",
     "textual",
 ]
 dependencies = [
-    "ypywidgets >=0.6.3",
+    "ypywidgets >=0.7.0,<0.8.0",
     "textual >=0.41.0",
     "textual-plotext",
     "pyte",
 ]
 
 [project.urls]
 Homepage = "https://github.com/davidbrochart/ypywidgets-textual"
```

### Comparing `ypywidgets_textual-0.3.0/PKG-INFO` & `ypywidgets_textual-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ypywidgets-textual
-Version: 0.3.0
+Version: 0.4.0
 Summary: Textual widgets for ypywidgets
 Project-URL: Homepage, https://github.com/davidbrochart/ypywidgets-textual
 Author-email: David Brochart <david.brochart@gmail.com>
 License-Expression: MIT
 Keywords: jupyter,textual,widgets,ypy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: pyte
 Requires-Dist: textual-plotext
 Requires-Dist: textual>=0.41.0
-Requires-Dist: ypywidgets>=0.6.3
+Requires-Dist: ypywidgets<0.8.0,>=0.7.0
 Description-Content-Type: text/markdown
 
 # ypywidgets-textual
 
 Textual widgets for ypywidgets
```

