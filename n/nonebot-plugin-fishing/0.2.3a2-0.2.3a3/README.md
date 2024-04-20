# Comparing `tmp/nonebot-plugin-fishing-0.2.3a2.tar.gz` & `tmp/nonebot_plugin_fishing-0.2.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-fishing-0.2.3a2.tar", last modified: Sat Apr 13 01:33:13 2024, max compression
+gzip compressed data, was "nonebot_plugin_fishing-0.2.3a3.tar", last modified: Sat Apr 20 13:51:47 2024, max compression
```

## Comparing `nonebot-plugin-fishing-0.2.3a2.tar` & `nonebot_plugin_fishing-0.2.3a3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:33:13.770884 nonebot-plugin-fishing-0.2.3a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-13 01:33:13.770884 nonebot-plugin-fishing-0.2.3a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:33:13.766884 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:33:13.770884 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/migrations/68463f3e5f33_update_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/migrations/7609e6d106dd_init_db.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:33:13.770884 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-13 01:33:13.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-13 01:33:13.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:33:13.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-13 01:33:13.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 01:33:13.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 01:33:13.770884 nonebot-plugin-fishing-0.2.3a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:51:47.664023 nonebot_plugin_fishing-0.2.3a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-20 13:51:39.000000 nonebot_plugin_fishing-0.2.3a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-20 13:51:47.664023 nonebot_plugin_fishing-0.2.3a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-20 13:51:39.000000 nonebot_plugin_fishing-0.2.3a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:51:47.664023 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-20 13:51:39.000000 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-20 13:51:39.000000 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-20 13:51:39.000000 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:51:47.664023 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-20 13:51:39.000000 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing/migrations/68463f3e5f33_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-20 13:51:39.000000 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing/migrations/7609e6d106dd_init_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-20 13:51:39.000000 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing/migrations/e9015df43907_add_special_fishes_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-20 13:51:39.000000 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing/migrations/f70bdeaec7a4_add_specialfishes_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-20 13:51:39.000000 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:51:47.664023 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-20 13:51:47.000000 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-20 13:51:47.000000 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:51:47.000000 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-20 13:51:47.000000 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 13:51:47.000000 nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-20 13:51:39.000000 nonebot_plugin_fishing-0.2.3a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:51:47.664023 nonebot_plugin_fishing-0.2.3a3/setup.cfg
```

### Comparing `nonebot-plugin-fishing-0.2.3a2/LICENSE` & `nonebot_plugin_fishing-0.2.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fishing-0.2.3a2/PKG-INFO` & `nonebot_plugin_fishing-0.2.3a3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fishing
-Version: 0.2.3a2
+Version: 0.2.3a3
 Summary: 你甚至可以电子钓鱼
 Author-email: C14H22O <160833462+C14H22O@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2>=2.2.1
@@ -96,26 +96,34 @@
     "name": "小鱼", # 鱼的名称
     "frequency": 2, # 鱼上钩的时间
     "weight": 100, # 权重
     "price": 2 # 价格
 }
 ```
 
+## 🔨 更新
 
+每一次更新后，需执行 `nb orm upgrade`。
+
+由于此前版本数据库迁移存在问题，故插件无法对 [v0.2.1](https://pypi.org/project/nonebot-plugin-fishing/0.2.1/) 版本及以前的数据进行迁移。
 
 ## 🎉 使用
 
 ### 指令表
 | 指令 | 范围 | 说明 |
 |:-----:|:----:|:----:|
 | 钓鱼 | 所有 | 放下鱼竿 |
 | 统计信息 | 所有 | 查看钓鱼次数 |
 | 背包 | 所有 | 查看背包 |
 | 卖鱼 | 所有 | 卖鱼 |
 
+## 🔨 更新
+
+每一次升级后，都需执行 `nb orm upgrade`。
+
 ## 📝 Todo
 
 - [x] 重写数据库逻辑（改为使用 [nonebot/plugin-orm](https://github.com/nonebot/plugin-orm)）
 - [x] 增加系统商店，卖出钓到的鱼们
 - [ ] 赛博放生 [#4](https://github.com/C14H22O/nonebot-plugin-fishing/issues/4)
 - [ ] 为鱼竿增加耐久度，耐久度为0时需重新购买鱼竿
 - [ ] 为钓鱼背包添加排序
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.3a2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.3a3 Summary:
 ä½ çè³å¯ä»¥çµå­éé±¼ Author-email: C14H22O
 <160833462+C14H22O@users.noreply.github.com> License: MIT Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: nonebot2>=2.2.1 Requires-Dist: pydantic>=1.10 Requires-Dist: nonebot-
 plugin-localstore>=0.6.0 Requires-Dist: sqlalchemy>=2.0.27 Requires-Dist:
 aiosqlite>=0.20.0 Requires-Dist: nonebot-plugin-orm>=0.7.1
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
@@ -22,16 +22,20 @@
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 è¯´æ | |:-----:|:----:|:----:| | fishes | å¦ |
 éç½®é±¼å¡åé±¼ä»¬çåç§°ãæéãç­å¾æ¶é´åä»·æ ¼ | |
 fishing_limit | å¦ | å¡«å¥æ¯æ¬¡éé±¼åï¼éå¶éé±¼çç§æ° | |
 fishing_coin_name | å¦ | å¡«å¥åé±¼è·åçè´§å¸åç§° | å¶ä¸­ `fishes`
 éç½®é¡¹è¯´æå¦ä¸ï¼ ```dotenv { "name": "å°é±¼", # é±¼çåç§°
 "frequency": 2, # é±¼ä¸é©çæ¶é´ "weight": 100, # æé "price": 2 #
-ä»·æ ¼ } ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:
-|:----:|:----:| | éé±¼ | ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ |
-æ¥çéé±¼æ¬¡æ° | | èå | ææ | æ¥çèå | | åé±¼ | ææ |
-åé±¼ | ## ð Todo - [x] éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨ [nonebot/
-plugin-orm](https://github.com/nonebot/plugin-orm)ï¼ - [x]
+ä»·æ ¼ } ``` ## ð¨ æ´æ° æ¯ä¸æ¬¡æ´æ°åï¼éæ§è¡ `nb orm upgrade`ã
+ç±äºæ­¤åçæ¬æ°æ®åºè¿ç§»å­å¨é®é¢ï¼ææä»¶æ æ³å¯¹ [v0.2.1]
+(https://pypi.org/project/nonebot-plugin-fishing/0.2.1/
+) çæ¬åä»¥åçæ°æ®è¿è¡è¿ç§»ã ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤
+| èå´ | è¯´æ | |:-----:|:----:|:----:| | éé±¼ | ææ | æ¾ä¸é±¼ç«¿ |
+| ç»è®¡ä¿¡æ¯ | ææ | æ¥çéé±¼æ¬¡æ° | | èå | ææ | æ¥çèå
+| | åé±¼ | ææ | åé±¼ | ## ð¨ æ´æ° æ¯ä¸æ¬¡åçº§åï¼é½éæ§è¡
+`nb orm upgrade`ã ## ð Todo - [x] éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨
+[nonebot/plugin-orm](https://github.com/nonebot/plugin-orm)ï¼ - [x]
 å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ] èµåæ¾ç [#4](https://
 github.com/C14H22O/nonebot-plugin-fishing/issues/4) - [ ]
 ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
 ä¸ºéé±¼èåæ·»å æåº - [ ] æ·»å æå°±ç³»ç»
```

### Comparing `nonebot-plugin-fishing-0.2.3a2/README.md` & `nonebot_plugin_fishing-0.2.3a3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -80,26 +80,34 @@
     "name": "小鱼", # 鱼的名称
     "frequency": 2, # 鱼上钩的时间
     "weight": 100, # 权重
     "price": 2 # 价格
 }
 ```
 
+## 🔨 更新
 
+每一次更新后，需执行 `nb orm upgrade`。
+
+由于此前版本数据库迁移存在问题，故插件无法对 [v0.2.1](https://pypi.org/project/nonebot-plugin-fishing/0.2.1/) 版本及以前的数据进行迁移。
 
 ## 🎉 使用
 
 ### 指令表
 | 指令 | 范围 | 说明 |
 |:-----:|:----:|:----:|
 | 钓鱼 | 所有 | 放下鱼竿 |
 | 统计信息 | 所有 | 查看钓鱼次数 |
 | 背包 | 所有 | 查看背包 |
 | 卖鱼 | 所有 | 卖鱼 |
 
+## 🔨 更新
+
+每一次升级后，都需执行 `nb orm upgrade`。
+
 ## 📝 Todo
 
 - [x] 重写数据库逻辑（改为使用 [nonebot/plugin-orm](https://github.com/nonebot/plugin-orm)）
 - [x] 增加系统商店，卖出钓到的鱼们
 - [ ] 赛博放生 [#4](https://github.com/C14H22O/nonebot-plugin-fishing/issues/4)
 - [ ] 为鱼竿增加耐久度，耐久度为0时需重新购买鱼竿
 - [ ] 为钓鱼背包添加排序
```

#### html2text {}

```diff
@@ -15,16 +15,20 @@
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 è¯´æ | |:-----:|:----:|:----:| | fishes | å¦ |
 éç½®é±¼å¡åé±¼ä»¬çåç§°ãæéãç­å¾æ¶é´åä»·æ ¼ | |
 fishing_limit | å¦ | å¡«å¥æ¯æ¬¡éé±¼åï¼éå¶éé±¼çç§æ° | |
 fishing_coin_name | å¦ | å¡«å¥åé±¼è·åçè´§å¸åç§° | å¶ä¸­ `fishes`
 éç½®é¡¹è¯´æå¦ä¸ï¼ ```dotenv { "name": "å°é±¼", # é±¼çåç§°
 "frequency": 2, # é±¼ä¸é©çæ¶é´ "weight": 100, # æé "price": 2 #
-ä»·æ ¼ } ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:
-|:----:|:----:| | éé±¼ | ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ |
-æ¥çéé±¼æ¬¡æ° | | èå | ææ | æ¥çèå | | åé±¼ | ææ |
-åé±¼ | ## ð Todo - [x] éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨ [nonebot/
-plugin-orm](https://github.com/nonebot/plugin-orm)ï¼ - [x]
+ä»·æ ¼ } ``` ## ð¨ æ´æ° æ¯ä¸æ¬¡æ´æ°åï¼éæ§è¡ `nb orm upgrade`ã
+ç±äºæ­¤åçæ¬æ°æ®åºè¿ç§»å­å¨é®é¢ï¼ææä»¶æ æ³å¯¹ [v0.2.1]
+(https://pypi.org/project/nonebot-plugin-fishing/0.2.1/
+) çæ¬åä»¥åçæ°æ®è¿è¡è¿ç§»ã ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤
+| èå´ | è¯´æ | |:-----:|:----:|:----:| | éé±¼ | ææ | æ¾ä¸é±¼ç«¿ |
+| ç»è®¡ä¿¡æ¯ | ææ | æ¥çéé±¼æ¬¡æ° | | èå | ææ | æ¥çèå
+| | åé±¼ | ææ | åé±¼ | ## ð¨ æ´æ° æ¯ä¸æ¬¡åçº§åï¼é½éæ§è¡
+`nb orm upgrade`ã ## ð Todo - [x] éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨
+[nonebot/plugin-orm](https://github.com/nonebot/plugin-orm)ï¼ - [x]
 å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ] èµåæ¾ç [#4](https://
 github.com/C14H22O/nonebot-plugin-fishing/issues/4) - [ ]
 ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
 ä¸ºéé±¼èåæ·»å æåº - [ ] æ·»å æå°±ç³»ç»
```

### Comparing `nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/__init__.py` & `nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,73 +3,97 @@
 require("nonebot_plugin_orm")  # noqa
 from nonebot.plugin import PluginMetadata
 from nonebot.adapters import Event, Message
 from nonebot.params import CommandArg
 
 import asyncio
 
-from .config import Config
-from .data_source import (choice,
-                          is_fishing,
-                          get_stats,
-                          save_fish,
-                          get_backpack,
-                          sell_fish,
-                          get_balance)
+from .config import Config, config
+from .data_source import (
+    choice,
+    can_fishing,
+    can_catch_special_fish,
+    can_free_fish,
+    get_stats,
+    save_fish,
+    save_special_fish,
+    get_backpack,
+    sell_fish,
+    get_balance,
+    free_fish,
+    random_get_a_special_fish
+)
 
 __plugin_meta__ = PluginMetadata(
     name="赛博钓鱼",
     description="你甚至可以电子钓鱼",
     usage="发送“钓鱼”，放下鱼竿。",
     type="application",
     homepage="https://github.com/C14H22O/nonebot-plugin-fishing",
     config=Config,
     supported_adapters=None
 )
 
 fishing = on_command("fishing", aliases={"钓鱼"}, priority=5)
-stats = on_command("stats", aliases={"统计信息"}, priority=5)
-backpack = on_command("backpack", aliases={"背包"}, priority=5)
+stats = on_command("stats", aliases={"统计信息", "钓鱼统计信息"}, priority=5)
+backpack = on_command("backpack", aliases={"背包", "钓鱼背包"}, priority=5)
 sell = on_command("sell", aliases={"卖鱼"}, priority=5)
-balance = on_command("balance", aliases={"余额"}, priority=5)
+balance = on_command("balance", aliases={"余额", "钓鱼余额"}, priority=5)
+free_fish_cmd = on_command("free_fish", aliases={"放生", "钓鱼放生"}, priority=5)
 
 
 @fishing.handle()
-async def _fishing(event: Event):
+async def _(event: Event):
     user_id = event.get_user_id()
-    if not await is_fishing(user_id):
+    if not await can_fishing(user_id):
         await fishing.finish("河累了, 休息一下吧")
     await fishing.send("正在钓鱼…")
+    if await can_catch_special_fish():
+        special_fish_name = await random_get_a_special_fish()
+        result = f"你钓到了别人放生的 {special_fish_name}"
+        await save_special_fish(user_id, special_fish_name)
+        await fishing.finish(result)
     choice_result = choice()
     fish = choice_result[0]
     sleep_time = choice_result[1]
     result = f"钓到了一条{fish}, 你把它收进了背包里"
     await save_fish(user_id, fish)
     await asyncio.sleep(sleep_time)
     await fishing.finish(result)
 
 
 @stats.handle()
-async def _stats(event: Event):
+async def _(event: Event):
     user_id = event.get_user_id()
     await stats.finish(await get_stats(user_id))
 
 
 @backpack.handle()
-async def _backpack(event: Event):
+async def _(event: Event):
     user_id = event.get_user_id()
     await backpack.finish(await get_backpack(user_id))
 
 
 @sell.handle()
-async def _sell(event: Event, arg: Message = CommandArg()):
+async def _(event: Event, arg: Message = CommandArg()):
     fish_name = arg.extract_plain_text()
     if fish_name == "":
         await sell.finish("请输入要卖出的鱼的名字, 如 /卖鱼 小鱼")
     user_id = event.get_user_id()
     await sell.finish(await sell_fish(user_id, fish_name))
 
 
 @balance.handle()
-async def _balance(event: Event):
+async def _(event: Event):
     user_id = event.get_user_id()
     await balance.finish(await get_balance(user_id))
+
+
+@free_fish_cmd.handle()
+async def _(event: Event, arg: Message = CommandArg()):
+    if not can_free_fish():
+        await free_fish_cmd.finish("未开启此功能, 请联系机器人管理员")
+    fish_name = arg.extract_plain_text()
+    if fish_name == "":
+        await free_fish_cmd.finish("请输入要放生的鱼的名字, 如 /放生 测试鱼")
+    user_id = event.get_user_id()
+    await free_fish_cmd.finish(await free_fish(user_id, fish_name))
```

### Comparing `nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/migrations/68463f3e5f33_update_version.py` & `nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing/migrations/68463f3e5f33_.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 
 
 def downgrade(name: str = "") -> None:
     if name:
         return
     # ### commands auto generated by Alembic - please adjust! ###
     pass
-    # ### end Alembic commands ###
+    # ### end Alembic commands ###
```

### Comparing `nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/migrations/7609e6d106dd_init_db.py` & `nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing/migrations/7609e6d106dd_init_db.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-"""init db
-
-迁移 ID: 7609e6d106dd
-父迁移: 
-创建时间: 2024-04-05 19:08:58.835014
-
-"""
-from __future__ import annotations
-
-from collections.abc import Sequence
-
-from alembic import op
-import sqlalchemy as sa
-
-
-revision: str = '7609e6d106dd'
-down_revision: str | Sequence[str] | None = None
-branch_labels: str | Sequence[str] | None = ('nonebot_plugin_fishing',)
-depends_on: str | Sequence[str] | None = None
-
-
-def upgrade(name: str = "") -> None:
-    if name:
-        return
-    # ### commands auto generated by Alembic - please adjust! ###
-    op.create_table('nonebot_plugin_fishing_fishingrecord',
-    sa.Column('id', sa.Integer(), nullable=False),
-    sa.Column('user_id', sa.String(length=32), nullable=False),
-    sa.Column('time', sa.Integer(), nullable=False),
-    sa.Column('frequency', sa.Integer(), nullable=False),
-    sa.Column('fishes', sa.TEXT(), nullable=False),
-    sa.Column('coin', sa.Integer(), nullable=False),
-    sa.PrimaryKeyConstraint('id', name=op.f('pk_nonebot_plugin_fishing_fishingrecord')),
-    info={'bind_key': 'nonebot_plugin_fishing'}
-    )
-    # ### end Alembic commands ###
-
-
-def downgrade(name: str = "") -> None:
-    if name:
-        return
-    # ### commands auto generated by Alembic - please adjust! ###
-    op.drop_table('nonebot_plugin_fishing_fishingrecord')
+"""init db
+
+迁移 ID: 7609e6d106dd
+父迁移:
+创建时间: 2024-04-05 19:08:58.835014
+
+"""
+from __future__ import annotations
+
+from collections.abc import Sequence
+
+from alembic import op
+import sqlalchemy as sa
+
+
+revision: str = '7609e6d106dd'
+down_revision: str | Sequence[str] | None = None
+branch_labels: str | Sequence[str] | None = ('nonebot_plugin_fishing',)
+depends_on: str | Sequence[str] | None = None
+
+
+def upgrade(name: str = "") -> None:
+    if name:
+        return
+    # ### commands auto generated by Alembic - please adjust! ###
+    op.create_table('nonebot_plugin_fishing_fishingrecord',
+    sa.Column('id', sa.Integer(), nullable=False),
+    sa.Column('user_id', sa.String(length=32), nullable=False),
+    sa.Column('time', sa.Integer(), nullable=False),
+    sa.Column('frequency', sa.Integer(), nullable=False),
+    sa.Column('fishes', sa.TEXT(), nullable=False),
+    sa.Column('coin', sa.Integer(), nullable=False),
+    sa.PrimaryKeyConstraint('id', name=op.f('pk_nonebot_plugin_fishing_fishingrecord')),
+    info={'bind_key': 'nonebot_plugin_fishing'}
+    )
+    # ### end Alembic commands ###
+
+
+def downgrade(name: str = "") -> None:
+    if name:
+        return
+    # ### commands auto generated by Alembic - please adjust! ###
+    op.drop_table('nonebot_plugin_fishing_fishingrecord')
     # ### end Alembic commands ###
```

### Comparing `nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/PKG-INFO` & `nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fishing
-Version: 0.2.3a2
+Version: 0.2.3a3
 Summary: 你甚至可以电子钓鱼
 Author-email: C14H22O <160833462+C14H22O@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2>=2.2.1
@@ -96,26 +96,34 @@
     "name": "小鱼", # 鱼的名称
     "frequency": 2, # 鱼上钩的时间
     "weight": 100, # 权重
     "price": 2 # 价格
 }
 ```
 
+## 🔨 更新
 
+每一次更新后，需执行 `nb orm upgrade`。
+
+由于此前版本数据库迁移存在问题，故插件无法对 [v0.2.1](https://pypi.org/project/nonebot-plugin-fishing/0.2.1/) 版本及以前的数据进行迁移。
 
 ## 🎉 使用
 
 ### 指令表
 | 指令 | 范围 | 说明 |
 |:-----:|:----:|:----:|
 | 钓鱼 | 所有 | 放下鱼竿 |
 | 统计信息 | 所有 | 查看钓鱼次数 |
 | 背包 | 所有 | 查看背包 |
 | 卖鱼 | 所有 | 卖鱼 |
 
+## 🔨 更新
+
+每一次升级后，都需执行 `nb orm upgrade`。
+
 ## 📝 Todo
 
 - [x] 重写数据库逻辑（改为使用 [nonebot/plugin-orm](https://github.com/nonebot/plugin-orm)）
 - [x] 增加系统商店，卖出钓到的鱼们
 - [ ] 赛博放生 [#4](https://github.com/C14H22O/nonebot-plugin-fishing/issues/4)
 - [ ] 为鱼竿增加耐久度，耐久度为0时需重新购买鱼竿
 - [ ] 为钓鱼背包添加排序
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.3a2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.3a3 Summary:
 ä½ çè³å¯ä»¥çµå­éé±¼ Author-email: C14H22O
 <160833462+C14H22O@users.noreply.github.com> License: MIT Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: nonebot2>=2.2.1 Requires-Dist: pydantic>=1.10 Requires-Dist: nonebot-
 plugin-localstore>=0.6.0 Requires-Dist: sqlalchemy>=2.0.27 Requires-Dist:
 aiosqlite>=0.20.0 Requires-Dist: nonebot-plugin-orm>=0.7.1
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
@@ -22,16 +22,20 @@
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 è¯´æ | |:-----:|:----:|:----:| | fishes | å¦ |
 éç½®é±¼å¡åé±¼ä»¬çåç§°ãæéãç­å¾æ¶é´åä»·æ ¼ | |
 fishing_limit | å¦ | å¡«å¥æ¯æ¬¡éé±¼åï¼éå¶éé±¼çç§æ° | |
 fishing_coin_name | å¦ | å¡«å¥åé±¼è·åçè´§å¸åç§° | å¶ä¸­ `fishes`
 éç½®é¡¹è¯´æå¦ä¸ï¼ ```dotenv { "name": "å°é±¼", # é±¼çåç§°
 "frequency": 2, # é±¼ä¸é©çæ¶é´ "weight": 100, # æé "price": 2 #
-ä»·æ ¼ } ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:
-|:----:|:----:| | éé±¼ | ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ |
-æ¥çéé±¼æ¬¡æ° | | èå | ææ | æ¥çèå | | åé±¼ | ææ |
-åé±¼ | ## ð Todo - [x] éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨ [nonebot/
-plugin-orm](https://github.com/nonebot/plugin-orm)ï¼ - [x]
+ä»·æ ¼ } ``` ## ð¨ æ´æ° æ¯ä¸æ¬¡æ´æ°åï¼éæ§è¡ `nb orm upgrade`ã
+ç±äºæ­¤åçæ¬æ°æ®åºè¿ç§»å­å¨é®é¢ï¼ææä»¶æ æ³å¯¹ [v0.2.1]
+(https://pypi.org/project/nonebot-plugin-fishing/0.2.1/
+) çæ¬åä»¥åçæ°æ®è¿è¡è¿ç§»ã ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤
+| èå´ | è¯´æ | |:-----:|:----:|:----:| | éé±¼ | ææ | æ¾ä¸é±¼ç«¿ |
+| ç»è®¡ä¿¡æ¯ | ææ | æ¥çéé±¼æ¬¡æ° | | èå | ææ | æ¥çèå
+| | åé±¼ | ææ | åé±¼ | ## ð¨ æ´æ° æ¯ä¸æ¬¡åçº§åï¼é½éæ§è¡
+`nb orm upgrade`ã ## ð Todo - [x] éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨
+[nonebot/plugin-orm](https://github.com/nonebot/plugin-orm)ï¼ - [x]
 å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ] èµåæ¾ç [#4](https://
 github.com/C14H22O/nonebot-plugin-fishing/issues/4) - [ ]
 ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
 ä¸ºéé±¼èåæ·»å æåº - [ ] æ·»å æå°±ç³»ç»
```

### Comparing `nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/SOURCES.txt` & `nonebot_plugin_fishing-0.2.3a3/nonebot_plugin_fishing.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -6,9 +6,11 @@
 nonebot_plugin_fishing/data_source.py
 nonebot_plugin_fishing/model.py
 nonebot_plugin_fishing.egg-info/PKG-INFO
 nonebot_plugin_fishing.egg-info/SOURCES.txt
 nonebot_plugin_fishing.egg-info/dependency_links.txt
 nonebot_plugin_fishing.egg-info/requires.txt
 nonebot_plugin_fishing.egg-info/top_level.txt
-nonebot_plugin_fishing/migrations/68463f3e5f33_update_version.py
-nonebot_plugin_fishing/migrations/7609e6d106dd_init_db.py
+nonebot_plugin_fishing/migrations/68463f3e5f33_.py
+nonebot_plugin_fishing/migrations/7609e6d106dd_init_db.py
+nonebot_plugin_fishing/migrations/e9015df43907_add_special_fishes_field.py
+nonebot_plugin_fishing/migrations/f70bdeaec7a4_add_specialfishes_table.py
```

