# Comparing `tmp/pymud-0.19.3.post2.tar.gz` & `tmp/pymud-0.19.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymud-0.19.3.post2.tar", last modified: Fri Apr  5 05:02:47 2024, max compression
+gzip compressed data, was "pymud-0.19.4.tar", last modified: Sat Apr 20 00:46:05 2024, max compression
```

## Comparing `pymud-0.19.3.post2.tar` & `pymud-0.19.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 05:02:47.190618 pymud-0.19.3.post2/
--rw-rw-rw-   0        0        0    35823 2024-03-10 00:23:03.000000 pymud-0.19.3.post2/LICENSE.txt
--rw-rw-rw-   0        0        0    67271 2024-04-05 05:02:47.187091 pymud-0.19.3.post2/PKG-INFO
--rw-rw-rw-   0        0        0    24743 2024-04-05 05:02:08.000000 pymud-0.19.3.post2/README.md
--rw-rw-rw-   0        0        0     2075 2024-04-05 05:02:15.000000 pymud-0.19.3.post2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 05:02:47.190618 pymud-0.19.3.post2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 05:02:47.057567 pymud-0.19.3.post2/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 05:02:47.118685 pymud-0.19.3.post2/src/pymud/
--rw-rw-rw-   0        0        0      422 2024-04-03 05:54:50.000000 pymud-0.19.3.post2/src/pymud/__init__.py
--rw-rw-rw-   0        0        0     4636 2024-03-25 06:44:52.000000 pymud-0.19.3.post2/src/pymud/__main__.py
--rw-rw-rw-   0        0        0     5596 2024-03-10 00:23:03.000000 pymud-0.19.3.post2/src/pymud/dialogs.py
--rw-rw-rw-   0        0        0    42400 2024-04-03 08:16:37.000000 pymud-0.19.3.post2/src/pymud/extras.py
--rw-rw-rw-   0        0        0    38063 2024-04-03 07:08:32.000000 pymud-0.19.3.post2/src/pymud/objects.py
--rw-rw-rw-   0        0        0    11496 2024-03-10 00:23:03.000000 pymud-0.19.3.post2/src/pymud/pkuxkx.py
--rw-rw-rw-   0        0        0    49106 2024-04-03 03:07:55.000000 pymud-0.19.3.post2/src/pymud/protocol.py
--rw-rw-rw-   0        0        0    42928 2024-04-05 05:00:36.000000 pymud-0.19.3.post2/src/pymud/pymud.py
--rw-rw-rw-   0        0        0   114021 2024-04-02 10:44:13.000000 pymud-0.19.3.post2/src/pymud/session.py
--rw-rw-rw-   0        0        0     7092 2024-04-05 05:02:27.000000 pymud-0.19.3.post2/src/pymud/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-05 05:02:47.173761 pymud-0.19.3.post2/src/pymud.egg-info/
--rw-rw-rw-   0        0        0    67271 2024-04-05 05:02:47.000000 pymud-0.19.3.post2/src/pymud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-04-05 05:02:47.000000 pymud-0.19.3.post2/src/pymud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 05:02:47.000000 pymud-0.19.3.post2/src/pymud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-05 05:02:47.000000 pymud-0.19.3.post2/src/pymud.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 05:02:47.000000 pymud-0.19.3.post2/src/pymud.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-05 05:02:47.000000 pymud-0.19.3.post2/src/pymud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 00:46:05.842018 pymud-0.19.4/
+-rw-rw-rw-   0        0        0    35823 2024-03-10 00:23:03.000000 pymud-0.19.4/LICENSE.txt
+-rw-rw-rw-   0        0        0    67859 2024-04-20 00:46:05.838024 pymud-0.19.4/PKG-INFO
+-rw-rw-rw-   0        0        0    25335 2024-04-20 00:43:35.000000 pymud-0.19.4/README.md
+-rw-rw-rw-   0        0        0     2070 2024-04-20 00:43:14.000000 pymud-0.19.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-20 00:46:05.843021 pymud-0.19.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 00:46:05.616880 pymud-0.19.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-20 00:46:05.751461 pymud-0.19.4/src/pymud/
+-rw-rw-rw-   0        0        0      422 2024-04-03 05:54:50.000000 pymud-0.19.4/src/pymud/__init__.py
+-rw-rw-rw-   0        0        0     4636 2024-03-25 06:44:52.000000 pymud-0.19.4/src/pymud/__main__.py
+-rw-rw-rw-   0        0        0     5596 2024-03-10 00:23:03.000000 pymud-0.19.4/src/pymud/dialogs.py
+-rw-rw-rw-   0        0        0    42400 2024-04-03 08:16:37.000000 pymud-0.19.4/src/pymud/extras.py
+-rw-rw-rw-   0        0        0    38088 2024-04-13 03:24:07.000000 pymud-0.19.4/src/pymud/objects.py
+-rw-rw-rw-   0        0        0    11496 2024-03-10 00:23:03.000000 pymud-0.19.4/src/pymud/pkuxkx.py
+-rw-rw-rw-   0        0        0    49106 2024-04-03 03:07:55.000000 pymud-0.19.4/src/pymud/protocol.py
+-rw-rw-rw-   0        0        0    43230 2024-04-20 00:38:50.000000 pymud-0.19.4/src/pymud/pymud.py
+-rw-rw-rw-   0        0        0   114503 2024-04-13 03:31:20.000000 pymud-0.19.4/src/pymud/session.py
+-rw-rw-rw-   0        0        0     7092 2024-04-20 00:43:49.000000 pymud-0.19.4/src/pymud/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-20 00:46:05.832024 pymud-0.19.4/src/pymud.egg-info/
+-rw-rw-rw-   0        0        0    67859 2024-04-20 00:46:05.000000 pymud-0.19.4/src/pymud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2024-04-20 00:46:05.000000 pymud-0.19.4/src/pymud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 00:46:05.000000 pymud-0.19.4/src/pymud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-20 00:46:05.000000 pymud-0.19.4/src/pymud.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 00:46:05.000000 pymud-0.19.4/src/pymud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-20 00:46:05.000000 pymud-0.19.4/src/pymud.egg-info/top_level.txt
```

### Comparing `pymud-0.19.3.post2/LICENSE.txt` & `pymud-0.19.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post2/PKG-INFO` & `pymud-0.19.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymud
-Version: 0.19.3.post2
+Version: 0.19.4
 Summary: a MUD Client written in Python
 Author-email: "newstart@pkuxkx" <crapex@crapex.cc>
 Maintainer-email: "newstart@pkuxkx" <crapex@crapex.cc>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -959,7 +959,14 @@
 ### 0.19.3post1 (2024-04-03)
 + 功能增加: 新增一个exec_async函数，是exec函数的异步形式。可以在其他会话中异步执行一段代码
 + 帮助完善: 帮助文档逻辑完善，已完成整个包的内置文档的编写和修改
 + 注: 由于我没弄太明白 readthedocs.io 网站对于读取github源代码的逻辑，目前只能通过新发布正式版本的形式来使 readthedocs.io 网站的文档中的类参考自动更新。
 
 ### 0.19.3post2 （2024-04-05）
 + 问题修复: 修复退出程序时的小bug
+
+### 0.19.4 (2024-04-20)
++ 功能调整: info 现在 msg 恢复为可接受任何类型参数，不一定是 str
++ 功能调整: #var, #global 指令中，现在可以使用参数扩展了，例如 #var max_qi @qi
++ 功能调整: #var, #global 指令中，现在对字符串会先使用 eval 转换类型，转换失败时使用 str 类型。例如， #var myvar 1 时，myvar类型将为int
++ 功能调整: 变量替代时，会自动实现类型转化，当被替代变量值为非 str 类型时不会再报错
++ 问题修复: 修复之前从后向前选择时，无法复制的问题
```

### Comparing `pymud-0.19.3.post2/README.md` & `pymud-0.19.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -254,7 +254,14 @@
 ### 0.19.3post1 (2024-04-03)
 + 功能增加: 新增一个exec_async函数，是exec函数的异步形式。可以在其他会话中异步执行一段代码
 + 帮助完善: 帮助文档逻辑完善，已完成整个包的内置文档的编写和修改
 + 注: 由于我没弄太明白 readthedocs.io 网站对于读取github源代码的逻辑，目前只能通过新发布正式版本的形式来使 readthedocs.io 网站的文档中的类参考自动更新。
 
 ### 0.19.3post2 （2024-04-05）
 + 问题修复: 修复退出程序时的小bug
+
+### 0.19.4 (2024-04-20)
++ 功能调整: info 现在 msg 恢复为可接受任何类型参数，不一定是 str
++ 功能调整: #var, #global 指令中，现在可以使用参数扩展了，例如 #var max_qi @qi
++ 功能调整: #var, #global 指令中，现在对字符串会先使用 eval 转换类型，转换失败时使用 str 类型。例如， #var myvar 1 时，myvar类型将为int
++ 功能调整: 变量替代时，会自动实现类型转化，当被替代变量值为非 str 类型时不会再报错
++ 问题修复: 修复之前从后向前选择时，无法复制的问题
```

### Comparing `pymud-0.19.3.post2/pyproject.toml` & `pymud-0.19.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "pymud"  # Required
-version = "0.19.3post2"  # Required
+version = "0.19.4"  # Required
 description = "a MUD Client written in Python"  # Optional
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["MUD", "multi-user dungeon", "client"]  # Optional
 authors = [
   {name = "newstart@pkuxkx", email = "crapex@crapex.cc" } # Optional
```

### Comparing `pymud-0.19.3.post2/src/pymud/__main__.py` & `pymud-0.19.4/src/pymud/__main__.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post2/src/pymud/dialogs.py` & `pymud-0.19.4/src/pymud/dialogs.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post2/src/pymud/extras.py` & `pymud-0.19.4/src/pymud/extras.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post2/src/pymud/objects.py` & `pymud-0.19.4/src/pymud/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,35 +116,35 @@
             if item in (f"%{i}" for i in range(1, 10)):
                 idx = int(item[1:])
                 if idx <= len(wildcards):
                     item_val = wildcards[idx-1]
                 else:
                     item_val = "None"
                 new_code.append(item_val)
-                new_code_str = new_code_str.replace(item, item_val, 1)
+                new_code_str = new_code_str.replace(item, f"{item_val}", 1)
 
             # 系统变量，%开头
             elif item == "%line":
                 new_code.append(line)
-                new_code_str = new_code_str.replace(item, line, 1)
+                new_code_str = new_code_str.replace(item, f"{line}", 1)
 
             elif item == "%raw":
                 new_code.append(raw)
-                new_code_str = new_code_str.replace(item, raw, 1)
+                new_code_str = new_code_str.replace(item, f"{raw}", 1)
 
             elif item[0] == "%":
                 item_val = session.getVariable(item, "")
                 new_code.append(item_val)
-                new_code_str = new_code_str.replace(item, item_val, 1)
+                new_code_str = new_code_str.replace(item, f"{item_val}", 1)
 
             # 非系统变量，@开头，在变量明前加@引用
             elif item[0] == "@":
                 item_val = session.getVariable(item[1:], "")
                 new_code.append(item_val)
-                new_code_str = new_code_str.replace(item, item_val, 1)
+                new_code_str = new_code_str.replace(item, f"{item_val}", 1)
 
             else:
                 new_code.append(item)
 
         return new_code_str, new_code
 
     async def async_execute(self, session, *args, **kwargs):
```

### Comparing `pymud-0.19.3.post2/src/pymud/pkuxkx.py` & `pymud-0.19.4/src/pymud/pkuxkx.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post2/src/pymud/protocol.py` & `pymud-0.19.4/src/pymud/protocol.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post2/src/pymud/pymud.py` & `pymud-0.19.4/src/pymud/pymud.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,16 +458,20 @@
 
         :param raw: 指定采取文本模式还是ANSI格式模式
 
         ``注意: 复制的内容仅存在于运行环境的剪贴板中。若使用ssh远程，该复制命令不能访问本地剪贴板。``
         """
         b = self.consoleView.buffer
         if b.selection_state:
-            srow, scol = b.document.translate_index_to_position(b.selection_state.original_cursor_position)
-            erow, ecol = b.document.translate_index_to_position(b.document.cursor_position)
+            cur1, cur2 = b.selection_state.original_cursor_position, b.document.cursor_position
+            start, end = min(cur1, cur2), max(cur1, cur2)
+            srow, scol = b.document.translate_index_to_position(start)
+            erow, ecol = b.document.translate_index_to_position(end)
+            # srow, scol = b.document.translate_index_to_position(b.selection_state.original_cursor_position)
+            # erow, ecol = b.document.translate_index_to_position(b.document.cursor_position)
 
             if not raw:
                 # Control-C 复制纯文本
                 if srow == erow:
                     # 单行情况
                     #line = b.document.current_line
                     line = self.mudFormatProc.line_correction(b.document.current_line)
```

### Comparing `pymud-0.19.3.post2/src/pymud/session.py` & `pymud-0.19.4/src/pymud/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1673,15 +1673,18 @@
             :name: 变量名称
             :value: 变量值。注意: 该值赋值后为str类型!
 
         相关命令:
             - #global
         '''
 
-        args = code.code[2:]
+        new_cmd_text, new_code = code.expand(self, *args, **kwargs)
+        args = new_code[2:]
+
+        #args = code.code[2:]
 
         if len(args) == 0:
             vars = self._variables
             vars_simple = {}
             vars_complex = {}
             for k, v in vars.items():
                 # 不显示line, raw两个系统变量
@@ -1731,15 +1734,21 @@
             if args[0] in self._variables.keys():
                 obj = self.getVariable(args[0])
                 self.info(f"变量{args[0]}值为:{obj}")
             else:
                 self.warning(f"当前session中不存在名称为 {args[0]} 的变量")
             
         elif len(args) == 2:
-            self.setVariable(args[0], args[1])
+            val = None
+            try:
+                val = eval(args[1])
+            except:
+                val = args[1]
+
+            self.setVariable(args[0], val)
 
     def handle_global(self, code: CodeLine = None, *args, **kwargs):
         '''
         嵌入命令 #global 的执行函数，操作全局变量（跨会话共享）。
         该命令可以不带参数、带一个参数、两个参数。
         该函数不应该在代码中直接调用。
 
@@ -1752,15 +1761,17 @@
             :name: 变量名称
             :value: 变量值。注意: 该值赋值后为str类型! 
 
         相关命令:
             - #variable
         '''
 
-        args = code.code[2:]
+        new_cmd_text, new_code = code.expand(self, *args, **kwargs)
+        args = new_code[2:]
+        #args = code.code[2:]
 
         if len(args) == 0:
             vars = self.application.globals
             vars_simple = {}
             vars_complex = {}
             for k, v in vars.items():
                 if isinstance(v, Iterable) and not isinstance(v, str):
@@ -1806,15 +1817,20 @@
             var = args[0]
             if var in self.application.globals.keys():
                 self.info("{0:>18} = {1:<19}".format(var, self.application.get_globals(var).__repr__()), "全局变量")
             else:
                 self.info("全局空间不存在名称为 {} 的变量".format(var), "全局变量")
             
         elif len(args) == 2:
-            self.application.set_globals(args[0], args[1])
+            val = None
+            try:
+                val = eval(args[1])
+            except:
+                val = args[1]
+            self.application.set_globals(args[0], val)
 
     def _handle_objs(self, name: str, objs: dict, *args):
         if len(args) == 0:
             width = self.application.get_width()
             
             title = f"  {name.upper()} LIST IN SESSION {self.name}  "
             left = (width - len(title)) // 2
@@ -2771,14 +2787,16 @@
             - #warning
         '''
         
         new_text, new_code = code.expand(self, *args, **kwargs)
         self.error(new_text[6:])
 
     def info2(self, msg, title = "PYMUD INFO", style = Settings.INFO_STYLE):
+        msg = f"{msg}"
+
         if Settings.client["newline"] in msg:
             new_lines = list()
             msg_lines = msg.split(Settings.client["newline"])
             for line in msg_lines:
                 new_lines.append("{}{}".format(style, line))
 
             msg = Settings.client["newline"].join(new_lines)
```

### Comparing `pymud-0.19.3.post2/src/pymud/settings.py` & `pymud-0.19.4/src/pymud/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     "保存PyMUD配置的全局对象"
 
     # 下列内容为APP的常量定义，请勿修改
     __appname__   = "PYMUD"
     "APP 名称, 默认PYMUD"
     __appdesc__   = "a MUD client written in Python"
     "APP 简要描述"
-    __version__   = "0.19.3"
+    __version__   = "0.19.4"
     "APP 当前版本"
-    __release__   = "2024-04-05"
+    __release__   = "2024-04-20"
     "APP 当前版本发布日期"
     __author__    = "本牛(newstart)@北侠"
     "APP 作者"
     __email__     = "crapex@crapex.cc"
     "APP 作者邮箱"
     __website__     = "https://pymud.readthedocs.org/"
     "帮助文档发布网址"
```

### Comparing `pymud-0.19.3.post2/src/pymud.egg-info/PKG-INFO` & `pymud-0.19.4/src/pymud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymud
-Version: 0.19.3.post2
+Version: 0.19.4
 Summary: a MUD Client written in Python
 Author-email: "newstart@pkuxkx" <crapex@crapex.cc>
 Maintainer-email: "newstart@pkuxkx" <crapex@crapex.cc>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -959,7 +959,14 @@
 ### 0.19.3post1 (2024-04-03)
 + 功能增加: 新增一个exec_async函数，是exec函数的异步形式。可以在其他会话中异步执行一段代码
 + 帮助完善: 帮助文档逻辑完善，已完成整个包的内置文档的编写和修改
 + 注: 由于我没弄太明白 readthedocs.io 网站对于读取github源代码的逻辑，目前只能通过新发布正式版本的形式来使 readthedocs.io 网站的文档中的类参考自动更新。
 
 ### 0.19.3post2 （2024-04-05）
 + 问题修复: 修复退出程序时的小bug
+
+### 0.19.4 (2024-04-20)
++ 功能调整: info 现在 msg 恢复为可接受任何类型参数，不一定是 str
++ 功能调整: #var, #global 指令中，现在可以使用参数扩展了，例如 #var max_qi @qi
++ 功能调整: #var, #global 指令中，现在对字符串会先使用 eval 转换类型，转换失败时使用 str 类型。例如， #var myvar 1 时，myvar类型将为int
++ 功能调整: 变量替代时，会自动实现类型转化，当被替代变量值为非 str 类型时不会再报错
++ 问题修复: 修复之前从后向前选择时，无法复制的问题
```

