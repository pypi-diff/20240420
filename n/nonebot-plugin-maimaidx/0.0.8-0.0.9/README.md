# Comparing `tmp/nonebot-plugin-maimaidx-0.0.8.tar.gz` & `tmp/nonebot-plugin-maimaidx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-maimaidx-0.0.8.tar", last modified: Sun Nov 26 08:23:43 2023, max compression
+gzip compressed data, was "nonebot-plugin-maimaidx-0.0.9.tar", last modified: Thu Dec  7 17:36:34 2023, max compression
```

## Comparing `nonebot-plugin-maimaidx-0.0.8.tar` & `nonebot-plugin-maimaidx-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-11-26 08:23:43.806126 nonebot-plugin-maimaidx-0.0.8/
--rw-rw-rw-   0        0        0     1084 2023-10-14 08:49:02.000000 nonebot-plugin-maimaidx-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3180 2023-11-26 08:23:43.805152 nonebot-plugin-maimaidx-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2216 2023-10-15 05:59:41.000000 nonebot-plugin-maimaidx-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-11-26 08:23:43.791689 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/
--rw-rw-rw-   0        0        0    40303 2023-11-26 08:16:02.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/__init__.py
--rw-rw-rw-   0        0        0     3937 2023-10-15 08:12:20.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/config.py
-drwxrwxrwx   0        0        0        0 2023-11-26 08:23:43.802753 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/
--rw-rw-rw-   0        0        0     3039 2023-10-14 12:41:43.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/image.py
--rw-rw-rw-   0        0        0     5357 2023-10-14 12:43:25.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/maimaidx_api_data.py
--rw-rw-rw-   0        0        0    12569 2023-10-14 12:43:48.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/maimaidx_best_50.py
--rw-rw-rw-   0        0        0      740 2023-10-13 07:07:11.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/maimaidx_error.py
--rw-rw-rw-   0        0        0    19502 2023-10-14 13:03:21.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/maimaidx_music.py
--rw-rw-rw-   0        0        0    16951 2023-10-15 08:55:11.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/maimaidx_music_info.py
--rw-rw-rw-   0        0        0    28005 2023-10-14 13:03:37.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/maimaidx_player_score.py
--rw-rw-rw-   0        0        0      570 2023-10-13 07:07:11.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/tool.py
--rw-rw-rw-   0        0        0   388410 2023-08-08 18:28:02.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/maimaidxhelp.png
-drwxrwxrwx   0        0        0        0 2023-11-26 08:23:43.804172 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx.egg-info/
--rw-rw-rw-   0        0        0     3180 2023-11-26 08:23:43.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      791 2023-11-26 08:23:43.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-26 08:23:43.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      252 2023-11-26 08:23:43.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-11-26 08:23:43.000000 nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      962 2023-11-26 08:23:27.000000 nonebot-plugin-maimaidx-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-26 08:23:43.806126 nonebot-plugin-maimaidx-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-12-07 17:36:34.019554 nonebot-plugin-maimaidx-0.0.9/
+-rw-rw-rw-   0        0        0     1084 2023-10-14 08:49:02.000000 nonebot-plugin-maimaidx-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3172 2023-12-07 17:36:34.017554 nonebot-plugin-maimaidx-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2208 2023-12-07 17:31:47.000000 nonebot-plugin-maimaidx-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-12-07 17:36:33.963041 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/
+-rw-rw-rw-   0        0        0    40352 2023-12-07 17:29:25.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/__init__.py
+-rw-rw-rw-   0        0        0     3937 2023-10-15 08:12:20.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/config.py
+drwxrwxrwx   0        0        0        0 2023-12-07 17:36:34.008553 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/
+-rw-rw-rw-   0        0        0     3039 2023-10-14 12:41:43.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/image.py
+-rw-rw-rw-   0        0        0     5357 2023-10-14 12:43:25.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/maimaidx_api_data.py
+-rw-rw-rw-   0        0        0    12569 2023-10-14 12:43:48.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/maimaidx_best_50.py
+-rw-rw-rw-   0        0        0      740 2023-10-13 07:07:11.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/maimaidx_error.py
+-rw-rw-rw-   0        0        0    19502 2023-10-14 13:03:21.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/maimaidx_music.py
+-rw-rw-rw-   0        0        0    16951 2023-10-15 08:55:11.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/maimaidx_music_info.py
+-rw-rw-rw-   0        0        0    28005 2023-10-14 13:03:37.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/maimaidx_player_score.py
+-rw-rw-rw-   0        0        0      570 2023-10-13 07:07:11.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/tool.py
+-rw-rw-rw-   0        0        0   388410 2023-08-08 18:28:02.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/maimaidxhelp.png
+drwxrwxrwx   0        0        0        0 2023-12-07 17:36:34.015553 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx.egg-info/
+-rw-rw-rw-   0        0        0     3172 2023-12-07 17:36:33.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2023-12-07 17:36:33.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-07 17:36:33.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      252 2023-12-07 17:36:33.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-12-07 17:36:33.000000 nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      962 2023-12-07 17:30:12.000000 nonebot-plugin-maimaidx-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-12-07 17:36:34.019554 nonebot-plugin-maimaidx-0.0.9/setup.cfg
```

### Comparing `nonebot-plugin-maimaidx-0.0.8/LICENSE` & `nonebot-plugin-maimaidx-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-maimaidx-0.0.8/PKG-INFO` & `nonebot-plugin-maimaidx-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-maimaidx
-Version: 0.0.8
+Version: 0.0.9
 Summary: maimaidx plugin for nonebot2
 Author-email: Yuri-YuzuChaN <806235364@qq.com>
 Project-URL: Homepage, https://github.com/Yuri-YuzuChaN/nonebot-plugin-maimaidx
 Project-URL: Bug Tracker, https://github.com/Yuri-YuzuChaN/nonebot-plugin-maimaidx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -54,16 +54,16 @@
     - 使用源代码（不推荐） **需自行安装额外依赖**
         ``` git
         git clone https://github.com/Yuri-YuzuChaN/nonebot-plugin-maimaidx
         ```
     
 2. 安装 `PhantomJS`，前往 https://phantomjs.org/download.html 下载对应平台支持
 
-    > [!WARNING]
-    > 未配置 `PhantomJS` 支持的Bot，在使用 `ginfo` 指令时会被强制关闭 Bot 进程
+> [!WARNING]
+> 未配置 `PhantomJS` 支持的Bot，在使用 `ginfo` 指令时会被强制关闭 Bot 进程
 
 ## 配置
    
 1. 下载静态资源文件，将该压缩文件解压，且解压完为文件夹 `static` 。[下载链接](https://vote.yuzuai.xyz/download/static.zip) /  [下载节点2](https://share.yuzuai.xyz/d/aria/static.zip?sign=R9J9HEdOqoRwTpjkHBTsVIwJbmWqolxI5p-JQd1rvJ4=:0)
 2. 在 `.env` 文件中配置静态文件绝对路径 `MAIMAIDXPATH`
 
    ``` dotenv
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-maimaidx Version: 0.0.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-maimaidx Version: 0.0.9 Summary:
 maimaidx plugin for nonebot2 Author-email: Yuri-YuzuChaN <806235364@qq.com>
 Project-URL: Homepage, https://github.com/Yuri-YuzuChaN/nonebot-plugin-maimaidx
 Project-URL: Bug Tracker, https://github.com/Yuri-YuzuChaN/nonebot-plugin-
 maimaidx/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: nonebot2<3.0.0,>=2.0.0 Requires-Dist:
```

### Comparing `nonebot-plugin-maimaidx-0.0.8/README.md` & `nonebot-plugin-maimaidx-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     - 使用源代码（不推荐） **需自行安装额外依赖**
         ``` git
         git clone https://github.com/Yuri-YuzuChaN/nonebot-plugin-maimaidx
         ```
     
 2. 安装 `PhantomJS`，前往 https://phantomjs.org/download.html 下载对应平台支持
 
-    > [!WARNING]
-    > 未配置 `PhantomJS` 支持的Bot，在使用 `ginfo` 指令时会被强制关闭 Bot 进程
+> [!WARNING]
+> 未配置 `PhantomJS` 支持的Bot，在使用 `ginfo` 指令时会被强制关闭 Bot 进程
 
 ## 配置
    
 1. 下载静态资源文件，将该压缩文件解压，且解压完为文件夹 `static` 。[下载链接](https://vote.yuzuai.xyz/download/static.zip) /  [下载节点2](https://share.yuzuai.xyz/d/aria/static.zip?sign=R9J9HEdOqoRwTpjkHBTsVIwJbmWqolxI5p-JQd1rvJ4=:0)
 2. 在 `.env` 文件中配置静态文件绝对路径 `MAIMAIDXPATH`
 
    ``` dotenv
```

### Comparing `nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/__init__.py` & `nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
 import re
 from pathlib import Path
 from random import sample
-from re import Match
 from string import ascii_uppercase, digits
 from textwrap import dedent
 from typing import Optional, Tuple
 
+import aiofiles
 import nonebot
 from nonebot import get_bot, on_command, on_endswith, on_message, on_regex, require
 from nonebot.adapters.onebot.v11 import (
     GROUP_ADMIN,
     GROUP_OWNER,
     Bot,
     GroupMessageEvent,
@@ -141,15 +141,17 @@
     await mai.get_music()
     await mai.get_music_alias()
     await data_update.send('maimai数据更新完成')
 
 
 @manual.handle()
 async def _():
-    await manual.finish(MessageSegment.image(f'file:///{Root / "maimaidxhelp.png"}'), reply_message=True)
+    async with aiofiles.open(Root / 'maimaidxhelp.png', 'rb') as f:
+        help_image = await f.read()
+    await manual.finish(MessageSegment.image(help_image), reply_message=True)
 
 
 @repo.handle()
 async def _():
     await repo.finish('项目地址：https://github.com/Yuri-YuzuChaN/nonebot-plugin-maimaidx\n求star，求宣传~', reply_message=True)
 
 
@@ -317,15 +319,15 @@
             search_result += f'{music.id}. {music.title}\n'
         await search.finish(MessageSegment.image(to_bytes_io(search_result)), reply_message=True)
     else:
         await search.finish(f'结果过多（{len(result)} 条），请缩小查询范围。', reply_message=True)
 
 
 @query_chart.handle()
-async def _(match: Match[str] = RegexMatched()):
+async def _(match = RegexMatched()):
     id = match.group(1)
     music = mai.total_list.by_id(id)
     if not music:
         msg = f'未找到ID为[{id}]的乐曲'
     else:
         msg = await new_draw_music_info(music)
     await query_chart.send(msg)
@@ -367,15 +369,15 @@
         await what_song.finish(msg.strip(), reply_message=True)
 
     music = mai.total_list.by_id(str(data[0].ID))
     await what_song.finish('您要找的是不是：' + await new_draw_music_info(music), reply_message=True)
 
 
 @alias_song.handle()
-async def _(match: Match[str] = RegexMatched()):
+async def _(match = RegexMatched()):
     findid = bool(match.group(1))
     name = match.group(2)
     if findid and name.isdigit():
         alias_id = mai.total_alias_list.by_id(name)
         if not alias_id:
             await alias_song.finish('未找到此歌曲\n可以使用 添加别名 指令给该乐曲添加别名', reply_message=True)
         else:
```

### Comparing `nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/config.py` & `nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/image.py` & `nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/image.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/maimaidx_api_data.py` & `nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/maimaidx_api_data.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/maimaidx_best_50.py` & `nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/maimaidx_best_50.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/maimaidx_error.py` & `nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/maimaidx_error.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/maimaidx_music.py` & `nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/maimaidx_music.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/maimaidx_music_info.py` & `nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/maimaidx_music_info.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/maimaidx_player_score.py` & `nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/maimaidx_player_score.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/libraries/tool.py` & `nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/libraries/tool.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx/maimaidxhelp.png` & `nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx/maimaidxhelp.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx.egg-info/PKG-INFO` & `nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-maimaidx
-Version: 0.0.8
+Version: 0.0.9
 Summary: maimaidx plugin for nonebot2
 Author-email: Yuri-YuzuChaN <806235364@qq.com>
 Project-URL: Homepage, https://github.com/Yuri-YuzuChaN/nonebot-plugin-maimaidx
 Project-URL: Bug Tracker, https://github.com/Yuri-YuzuChaN/nonebot-plugin-maimaidx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -54,16 +54,16 @@
     - 使用源代码（不推荐） **需自行安装额外依赖**
         ``` git
         git clone https://github.com/Yuri-YuzuChaN/nonebot-plugin-maimaidx
         ```
     
 2. 安装 `PhantomJS`，前往 https://phantomjs.org/download.html 下载对应平台支持
 
-    > [!WARNING]
-    > 未配置 `PhantomJS` 支持的Bot，在使用 `ginfo` 指令时会被强制关闭 Bot 进程
+> [!WARNING]
+> 未配置 `PhantomJS` 支持的Bot，在使用 `ginfo` 指令时会被强制关闭 Bot 进程
 
 ## 配置
    
 1. 下载静态资源文件，将该压缩文件解压，且解压完为文件夹 `static` 。[下载链接](https://vote.yuzuai.xyz/download/static.zip) /  [下载节点2](https://share.yuzuai.xyz/d/aria/static.zip?sign=R9J9HEdOqoRwTpjkHBTsVIwJbmWqolxI5p-JQd1rvJ4=:0)
 2. 在 `.env` 文件中配置静态文件绝对路径 `MAIMAIDXPATH`
 
    ``` dotenv
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-maimaidx Version: 0.0.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-maimaidx Version: 0.0.9 Summary:
 maimaidx plugin for nonebot2 Author-email: Yuri-YuzuChaN <806235364@qq.com>
 Project-URL: Homepage, https://github.com/Yuri-YuzuChaN/nonebot-plugin-maimaidx
 Project-URL: Bug Tracker, https://github.com/Yuri-YuzuChaN/nonebot-plugin-
 maimaidx/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: nonebot2<3.0.0,>=2.0.0 Requires-Dist:
```

### Comparing `nonebot-plugin-maimaidx-0.0.8/nonebot_plugin_maimaidx.egg-info/SOURCES.txt` & `nonebot-plugin-maimaidx-0.0.9/nonebot_plugin_maimaidx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-maimaidx-0.0.8/pyproject.toml` & `nonebot-plugin-maimaidx-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-maimaidx"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Yuri-YuzuChaN", email="806235364@qq.com" },
 ]
 description = "maimaidx plugin for nonebot2"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

