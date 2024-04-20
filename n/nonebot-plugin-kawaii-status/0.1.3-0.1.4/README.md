# Comparing `tmp/nonebot_plugin_kawaii_status-0.1.3.tar.gz` & `tmp/nonebot_plugin_kawaii_status-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_kawaii_status-0.1.3.tar", last modified: Fri Mar  8 11:20:23 2024, max compression
+gzip compressed data, was "nonebot_plugin_kawaii_status-0.1.4.tar", last modified: Sat Apr 20 08:43:36 2024, max compression
```

## Comparing `nonebot_plugin_kawaii_status-0.1.3.tar` & `nonebot_plugin_kawaii_status-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1065 2024-03-08 11:20:00.661526 nonebot_plugin_kawaii_status-0.1.3/LICENSE
--rw-r--r--   0        0        0     2223 2024-03-08 11:20:00.661526 nonebot_plugin_kawaii_status-0.1.3/README.md
--rw-r--r--   0        0        0     1495 2024-03-08 11:20:00.665526 nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/__init__.py
--rw-r--r--   0        0        0      669 2024-03-08 11:20:00.665526 nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/color.py
--rw-r--r--   0        0        0      369 2024-03-08 11:20:00.665526 nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/config.py
--rw-r--r--   0        0        0     3935 2024-03-08 11:20:00.665526 nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/drawer.py
--rw-r--r--   0        0        0     2029 2024-03-08 11:20:00.665526 nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/model.py
--rw-r--r--   0        0        0      427 2024-03-08 11:20:00.665526 nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/path.py
--rw-r--r--   0        0        0    96904 2024-03-08 11:20:00.665526 nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/resources/fonts/ADLaMDisplay-Regular.ttf
--rw-r--r--   0        0        0    65816 2024-03-08 11:20:00.665526 nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/resources/fonts/SpicyRice-Regular.ttf
--rw-r--r--   0        0        0  6227568 2024-03-08 11:20:00.697526 nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/resources/fonts/baotu.ttf
--rw-r--r--   0        0        0   603174 2024-03-08 11:20:00.705526 nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/resources/images/background.png
--rw-r--r--   0        0        0     4863 2024-03-08 11:20:00.705526 nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/resources/images/marker.png
--rw-r--r--   0        0        0      385 2024-03-08 11:20:00.705526 nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/utils.py
--rw-r--r--   0        0        0     1431 2024-03-08 11:20:23.781550 nonebot_plugin_kawaii_status-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 nonebot_plugin_kawaii_status-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2326 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/README.md
+-rw-r--r--   0        0        0     1511 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/__init__.py
+-rw-r--r--   0        0        0      669 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/color.py
+-rw-r--r--   0        0        0      369 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/config.py
+-rw-r--r--   0        0        0     3965 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/drawer.py
+-rw-r--r--   0        0        0     2029 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/model.py
+-rw-r--r--   0        0        0      427 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/path.py
+-rw-r--r--   0        0        0    96904 2024-04-20 08:43:11.722305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/fonts/ADLaMDisplay-Regular.ttf
+-rw-r--r--   0        0        0    65816 2024-04-20 08:43:11.722305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/fonts/SpicyRice-Regular.ttf
+-rw-r--r--   0        0        0  6227568 2024-04-20 08:43:11.758305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/fonts/baotu.ttf
+-rw-r--r--   0        0        0   603174 2024-04-20 08:43:11.762305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/images/background.png
+-rw-r--r--   0        0        0     4863 2024-04-20 08:43:11.762305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/images/marker.png
+-rw-r--r--   0        0        0      385 2024-04-20 08:43:11.762305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/utils.py
+-rw-r--r--   0        0        0     1456 2024-04-20 08:43:36.594742 nonebot_plugin_kawaii_status-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 nonebot_plugin_kawaii_status-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_kawaii_status-0.1.3/LICENSE` & `nonebot_plugin_kawaii_status-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.3/README.md` & `nonebot_plugin_kawaii_status-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -52,25 +52,26 @@
 | 配置项 | 必填 | 默认值 |
 | :---: | :---: | :---: |
 | status__to_me | 否 | False |
 | status__only_superuser | 否 | False |
 
 ## 🎉 使用
 
-```bash
-/status
-```
+> [!note]
+> 请注意你的 `COMMAND_START` 以及上述配置项。
+
+指令名：`status` `状态` `运行状态`
 
 ### 效果图
 
 <img src="./docs/renderings.jpg" height="500" alt="renderings"/>
 
 ## 鸣谢
 
-- [`SoraBot`](github.com/netsora/SoraBot)：基于 Nonebot2 开发，互通多平台，超可爱的林汐酱 ~~（自产自销）~~
+- [`SoraBot`](https://github.com/netsora/SoraBot)：基于 Nonebot2 开发，互通多平台，超可爱的林汐酱 ~~（自产自销）~~
 
 ## 许可证
 
 本项目使用 [MIT](./LICENSE) 许可证开源
 
 ```txt
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
```

#### html2text {}

```diff
@@ -5,17 +5,18 @@
 ## ð ä»ç» NoneBot2 æå¡å¨ç¶ææ¥çæä»¶ ## ð¿ å®è£ ```bash pip
 install nonebot-plugin-kawaii-status # or, use poetry poetry add nonebot-
 plugin-kawaii-status # or, use pdm pdm add nonebot-plugin-kawaii-status ```
 æå¼ NoneBot é¡¹ç®æ ¹ç®å½ä¸çéç½®æä»¶, å¨ `[plugin]`
 é¨åè¿½å åå¥ ```toml plugins = ["nonebot_plugin_kawaii_status"] ``` ##
 âï¸ éç½® å¨é¡¹ç®çéç½®æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¯ééç½® |
 éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | | :---: | :---: | :---: | | status__to_me |
-å¦ | False | | status__only_superuser | å¦ | False | ## ð ä½¿ç¨ ```bash /
-status ``` ### ææå¾ [renderings]## é¸£è°¢ - [`SoraBot`](github.com/
-netsora/SoraBot)ï¼åºäº Nonebot2
+å¦ | False | | status__only_superuser | å¦ | False | ## ð ä½¿ç¨ > [!note]
+> è¯·æ³¨æä½ ç `COMMAND_START` ä»¥åä¸è¿°éç½®é¡¹ã æä»¤åï¼`status`
+`ç¶æ` `è¿è¡ç¶æ` ### ææå¾ [renderings]## é¸£è°¢ - [`SoraBot`]
+(https://github.com/netsora/SoraBot)ï¼åºäº Nonebot2
 å¼åï¼äºéå¤å¹³å°ï¼è¶å¯ç±çææ±é± ~~ï¼èªäº§èªéï¼~~ ##
 è®¸å¯è¯ æ¬é¡¹ç®ä½¿ç¨ [MIT](./LICENSE) è®¸å¯è¯å¼æº ```txt THE SOFTWARE
 IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
 INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
 PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
```

### Comparing `nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/__init__.py` & `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 require("nonebot_plugin_alconna")
 from nonebot_plugin_alconna import Command
 from nonebot_plugin_alconna.uniseg import UniMessage
 
 from .config import Config, ScopedConfig
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __plugin_meta__ = PluginMetadata(
     name="运行状态",
     description="NoneBot2 服务器状态查看插件",
     usage="/status",
     type="application",
     homepage="https://github.com/KomoriDev/nonebot-plugin-kawaii-status",
     config=Config,
@@ -47,12 +47,12 @@
 
 status = (
     Command("status", help_text="查看林汐运行状态")
     .usage("/status\n/状态")
     .action(lambda: UniMessage.image(raw=draw()))
     .build(
         rule=to_me(),
-        aliases={"状态"},
+        aliases={"状态", "运行状态"},
         use_cmd_start=True,
         permission=SUPERUSER if config.only_superuser else None,
     )
 )
```

### Comparing `nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/color.py` & `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/color.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/drawer.py` & `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/drawer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import platform
 from io import BytesIO
 
+import cpuinfo
 import nonebot
 from nonebot import get_plugin_config
 from PIL import Image, ImageDraw, ImageFont
 from nonebot.config import Config as BotConfig
 from nonebot import __version__ as __nb_version__
 
 from .model import get_status_info
@@ -92,15 +93,15 @@
         content.ellipse((108, 729, 212, 833), width=105, fill=transparent_color)
         content.ellipse((108, 883, 212, 987), width=105, fill=transparent_color)
         content.ellipse((108, 1037, 212, 1141), width=105, fill=transparent_color)
         content.ellipse((108, 1192, 212, 1295), width=105, fill=transparent_color)
 
         content.text(
             (352, 1378),
-            f"{truncate_string(platform.processor())}",
+            f"{truncate_string(cpuinfo.get_cpu_info()['brand_raw'])}",
             font=adlam_fnt,
             fill=details_color,
         )
         content.text(
             (352, 1431),
             f"{system.system} {system.release}",
             font=adlam_fnt,
```

### Comparing `nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/model.py` & `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/resources/fonts/ADLaMDisplay-Regular.ttf` & `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/fonts/ADLaMDisplay-Regular.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/resources/fonts/SpicyRice-Regular.ttf` & `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/fonts/SpicyRice-Regular.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/resources/fonts/baotu.ttf` & `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/fonts/baotu.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/resources/images/background.png` & `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/images/background.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.3/nonebot_plugin_kawaii_status/resources/images/marker.png` & `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/images/marker.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.3/pyproject.toml` & `nonebot_plugin_kawaii_status-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "nonebot-plugin-kawaii-status"
-version = "0.1.3"
+version = "0.1.4"
 description = "NoneBot2 服务器状态查看插件 / View server status for NoneBot2"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
     { name = "KomoriDev", email = "mute231010@gmail.com" },
 ]
 dependencies = [
     "nonebot-plugin-alconna>=0.37.0",
     "psutil>=5.9.8",
     "pillow>=10.2.0",
     "nonebot2[fastapi]>=2.2.0",
+    "py-cpuinfo>=9.0.0",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/KomoriDev/nonebot-plugin-kawaii-status"
```

### Comparing `nonebot_plugin_kawaii_status-0.1.3/PKG-INFO` & `nonebot_plugin_kawaii_status-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-kawaii-status
-Version: 0.1.3
+Version: 0.1.4
 Summary: NoneBot2 服务器状态查看插件 / View server status for NoneBot2
 Home-page: https://github.com/KomoriDev/nonebot-plugin-kawaii-status
 Author-Email: KomoriDev <mute231010@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/KomoriDev/nonebot-plugin-kawaii-status
 Project-URL: Repository, https://github.com/KomoriDev/nonebot-plugin-kawaii-status
 Requires-Python: >=3.8
 Requires-Dist: nonebot-plugin-alconna>=0.37.0
 Requires-Dist: psutil>=5.9.8
 Requires-Dist: pillow>=10.2.0
 Requires-Dist: nonebot2[fastapi]>=2.2.0
+Requires-Dist: py-cpuinfo>=9.0.0
 Requires-Dist: nonebot-adapter-onebot>=2.4.1; extra == "adapters"
 Provides-Extra: adapters
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 MD045 -->
 <div align="center">
   <a href="https://v2.nonebot.dev/store">
@@ -70,25 +71,26 @@
 | 配置项 | 必填 | 默认值 |
 | :---: | :---: | :---: |
 | status__to_me | 否 | False |
 | status__only_superuser | 否 | False |
 
 ## 🎉 使用
 
-```bash
-/status
-```
+> [!note]
+> 请注意你的 `COMMAND_START` 以及上述配置项。
+
+指令名：`status` `状态` `运行状态`
 
 ### 效果图
 
 <img src="./docs/renderings.jpg" height="500" alt="renderings"/>
 
 ## 鸣谢
 
-- [`SoraBot`](github.com/netsora/SoraBot)：基于 Nonebot2 开发，互通多平台，超可爱的林汐酱 ~~（自产自销）~~
+- [`SoraBot`](https://github.com/netsora/SoraBot)：基于 Nonebot2 开发，互通多平台，超可爱的林汐酱 ~~（自产自销）~~
 
 ## 许可证
 
 本项目使用 [MIT](./LICENSE) 许可证开源
 
 ```txt
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-kawaii-status Version: 0.1.3
+Metadata-Version: 2.1 Name: nonebot-plugin-kawaii-status Version: 0.1.4
 Summary: NoneBot2 æå¡å¨ç¶ææ¥çæä»¶ / View server status for NoneBot2
 Home-page: https://github.com/KomoriDev/nonebot-plugin-kawaii-status Author-
 Email: KomoriDev
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/KomoriDev/
 nonebot-plugin-kawaii-status Project-URL: Repository, https://github.com/
 KomoriDev/nonebot-plugin-kawaii-status Requires-Python: >=3.8 Requires-Dist:
 nonebot-plugin-alconna>=0.37.0 Requires-Dist: psutil>=5.9.8 Requires-Dist:
-pillow>=10.2.0 Requires-Dist: nonebot2[fastapi]>=2.2.0 Requires-Dist: nonebot-
-adapter-onebot>=2.4.1; extra == "adapters" Provides-Extra: adapters
-Description-Content-Type: text/markdown
+pillow>=10.2.0 Requires-Dist: nonebot2[fastapi]>=2.2.0 Requires-Dist: py-
+cpuinfo>=9.0.0 Requires-Dist: nonebot-adapter-onebot>=2.4.1; extra ==
+"adapters" Provides-Extra: adapters Description-Content-Type: text/markdown
                                     _[_l_o_g_o_]
                                     [logo]
 # NoneBot-Plugin-Kawaii-Status _â¨ NoneBot2 æå¡å¨ç¶ææ¥çæä»¶ â¨_
                            /a>[python]_[_p_d_m_-_m_a_n_a_g_e_d_]
 ## ð ä»ç» NoneBot2 æå¡å¨ç¶ææ¥çæä»¶ ## ð¿ å®è£ ```bash pip
 install nonebot-plugin-kawaii-status # or, use poetry poetry add nonebot-
 plugin-kawaii-status # or, use pdm pdm add nonebot-plugin-kawaii-status ```
 æå¼ NoneBot é¡¹ç®æ ¹ç®å½ä¸çéç½®æä»¶, å¨ `[plugin]`
 é¨åè¿½å åå¥ ```toml plugins = ["nonebot_plugin_kawaii_status"] ``` ##
 âï¸ éç½® å¨é¡¹ç®çéç½®æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¯ééç½® |
 éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | | :---: | :---: | :---: | | status__to_me |
-å¦ | False | | status__only_superuser | å¦ | False | ## ð ä½¿ç¨ ```bash /
-status ``` ### ææå¾ [renderings]## é¸£è°¢ - [`SoraBot`](github.com/
-netsora/SoraBot)ï¼åºäº Nonebot2
+å¦ | False | | status__only_superuser | å¦ | False | ## ð ä½¿ç¨ > [!note]
+> è¯·æ³¨æä½ ç `COMMAND_START` ä»¥åä¸è¿°éç½®é¡¹ã æä»¤åï¼`status`
+`ç¶æ` `è¿è¡ç¶æ` ### ææå¾ [renderings]## é¸£è°¢ - [`SoraBot`]
+(https://github.com/netsora/SoraBot)ï¼åºäº Nonebot2
 å¼åï¼äºéå¤å¹³å°ï¼è¶å¯ç±çææ±é± ~~ï¼èªäº§èªéï¼~~ ##
 è®¸å¯è¯ æ¬é¡¹ç®ä½¿ç¨ [MIT](./LICENSE) è®¸å¯è¯å¼æº ```txt THE SOFTWARE
 IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
 INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
 PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
```

