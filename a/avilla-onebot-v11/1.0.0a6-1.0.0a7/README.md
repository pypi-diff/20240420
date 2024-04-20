# Comparing `tmp/avilla_onebot_v11-1.0.0a6.tar.gz` & `tmp/avilla_onebot_v11-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avilla_onebot_v11-1.0.0a6.tar", last modified: Sun Aug  6 15:15:27 2023, max compression
+gzip compressed data, was "avilla_onebot_v11-1.0.0a7.tar", last modified: Sat Sep  2 13:54:12 2023, max compression
```

## Comparing `avilla_onebot_v11-1.0.0a6.tar` & `avilla_onebot_v11-1.0.0a7.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     1070 2023-08-06 15:15:11.646896 avilla_onebot_v11-1.0.0a6/LICENSE
--rw-r--r--   0        0        0     8089 2023-08-06 15:15:11.646896 avilla_onebot_v11-1.0.0a6/README.md
--rw-r--r--   0        0        0        0 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/__init__.py
--rw-r--r--   0        0        0     2153 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/account.py
--rw-r--r--   0        0        0        0 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/collector/__init__.py
--rw-r--r--   0        0        0      971 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/collector/connection.py
--rw-r--r--   0        0        0      159 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/element.py
--rw-r--r--   0        0        0        0 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/net/__init__.py
--rw-r--r--   0        0        0     2749 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/net/base.py
--rw-r--r--   0        0        0     5333 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/net/ws_client.py
--rw-r--r--   0        0        0     4158 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/net/ws_server.py
--rw-r--r--   0        0        0        0 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/action/__init__.py
--rw-r--r--   0        0        0     1354 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/action/admin.py
--rw-r--r--   0        0        0      995 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/action/ban.py
--rw-r--r--   0        0        0     1112 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/action/leave.py
--rw-r--r--   0        0        0     2260 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/action/message.py
--rw-r--r--   0        0        0     2557 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/action/mute.py
--rw-r--r--   0        0        0        0 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/event/__init__.py
--rw-r--r--   0        0        0     3457 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/event/lifespan.py
--rw-r--r--   0        0        0     9386 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/event/message.py
--rw-r--r--   0        0        0    11222 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/event/notice.py
--rw-r--r--   0        0        0     2235 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/event/request.py
--rw-r--r--   0        0        0     2989 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/message/deserialize.py
--rw-r--r--   0        0        0     4145 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/message/serialize.py
--rw-r--r--   0        0        0        0 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/query/__init__.py
--rw-r--r--   0        0        0     1515 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/query/group.py
--rw-r--r--   0        0        0     1042 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/resource_fetch.py
--rw-r--r--   0        0        0     1424 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/protocol.py
--rw-r--r--   0        0        0      828 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/resource.py
--rw-r--r--   0        0        0     1213 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/service.py
--rw-r--r--   0        0        0      285 2023-08-06 15:15:11.650896 avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/utilles.py
--rw-r--r--   0        0        0     5988 2023-08-06 15:15:27.635166 avilla_onebot_v11-1.0.0a6/pyproject.toml
--rw-r--r--   0        0        0     8548 1970-01-01 00:00:00.000000 avilla_onebot_v11-1.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0      551 2023-09-02 13:53:57.108123 avilla_onebot_v11-1.0.0a7/.mina/onebot-v11.toml
+-rw-r--r--   0        0        0     1070 2023-09-02 13:53:57.108123 avilla_onebot_v11-1.0.0a7/LICENSE
+-rw-r--r--   0        0        0     8360 2023-09-02 13:53:57.108123 avilla_onebot_v11-1.0.0a7/README.md
+-rw-r--r--   0        0        0      197 2023-09-02 13:53:57.112123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/__init__.py
+-rw-r--r--   0        0        0     2154 2023-09-02 13:53:57.112123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/account.py
+-rw-r--r--   0        0        0        0 2023-09-02 13:53:57.112123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/collector/__init__.py
+-rw-r--r--   0        0        0      939 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/collector/connection.py
+-rw-r--r--   0        0        0      159 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/element.py
+-rw-r--r--   0        0        0        0 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/net/__init__.py
+-rw-r--r--   0        0        0     2753 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/net/base.py
+-rw-r--r--   0        0        0     5202 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/net/ws_client.py
+-rw-r--r--   0        0        0     4049 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/net/ws_server.py
+-rw-r--r--   0        0        0        0 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/action/__init__.py
+-rw-r--r--   0        0        0     1354 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/action/admin.py
+-rw-r--r--   0        0        0      995 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/action/ban.py
+-rw-r--r--   0        0        0     1112 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/action/leave.py
+-rw-r--r--   0        0        0     4953 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/action/message.py
+-rw-r--r--   0        0        0     2557 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/action/mute.py
+-rw-r--r--   0        0        0     1882 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/context.py
+-rw-r--r--   0        0        0        0 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/event/__init__.py
+-rw-r--r--   0        0        0     3457 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/event/lifespan.py
+-rw-r--r--   0        0        0     9398 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/event/message.py
+-rw-r--r--   0        0        0    11561 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/event/notice.py
+-rw-r--r--   0        0        0     2235 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/event/request.py
+-rw-r--r--   0        0        0     4056 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/message/deserialize.py
+-rw-r--r--   0        0        0     4145 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/message/serialize.py
+-rw-r--r--   0        0        0        0 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/query/__init__.py
+-rw-r--r--   0        0        0     1515 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/query/group.py
+-rw-r--r--   0        0        0     1042 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/resource_fetch.py
+-rw-r--r--   0        0        0     2474 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/protocol.py
+-rw-r--r--   0        0        0      828 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/resource.py
+-rw-r--r--   0        0        0     1214 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/service.py
+-rw-r--r--   0        0        0      285 2023-09-02 13:53:57.116123 avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/utilles.py
+-rw-r--r--   0        0        0     1006 2023-09-02 13:54:12.708493 avilla_onebot_v11-1.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0     8819 1970-01-01 00:00:00.000000 avilla_onebot_v11-1.0.0a7/PKG-INFO
```

### Comparing `avilla_onebot_v11-1.0.0a6/LICENSE` & `avilla_onebot_v11-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `avilla_onebot_v11-1.0.0a6/README.md` & `avilla_onebot_v11-1.0.0a7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,48 +34,44 @@
   > 担心可用性? 我们同样提供了一些核心的非平台依赖实现, 例如 `TextCommand`, 这些组件仅要求平台实现最基本的交互实现, 剩下的一切交给 Avilla 处理!
  - **现有基建兼容**: 得益于 `Amnesia`, `Commander`, `Twilight`, `Alconna` 或是基于 `Launart` 编写的各式扩展, 可以直接与 Avilla 协同而无需任何迁移成本.
  - **高可伸缩性**: Avilla 既支持单文件使用, 亦支持基于 Graia Saya 驱动的模块系统编写应用.
 
 ## Quick Start
 
 ```py
-from creart import create
-from launart import Launart
-from graia.broadcast import Broadcast
-
 from avilla.core import Avilla, Context, MessageReceived
 from avilla.console.protocol import ConsoleProtocol
 
-broadcast = create(Broadcast)
-launart = Launart()
-avilla = Avilla(broadcast, launart, [ConsoleProtocol()])
+avilla = Avilla()
+avilla.apply_protocols(ConsoleProtocol())
 
 
-@broadcast.receiver(MessageReceived)
+@avilla.listen(MessageReceived)
 async def on_message_received(cx: Context, event: MessageReceived):
     await cx.scene.send_message("Hello, Avilla!")
 
 
-launart.launch_blocking(loop=broadcast.loop)
+avilla.launch()
 ```
 
 ## 部件发布情况
 
-|                    代号                     |           协议           |   开发进度    |                                                  PyPI                                                   |   维护者    |  开源协议  |
-|:-----------------------------------------:|:----------------------:|:---------:|:-------------------------------------------------------------------------------------------------------:|:--------:|:------:|
-|            [Core](avilla/core)            |           -            | **Alpha** |       [![image](https://img.shields.io/pypi/v/avilla-core)](https://pypi.org/project/avilla-core)       | Official |  MIT   |
-|       [Elizabeth](avilla/elizabeth)       |    `mirai-api-http`    |  **WIP**  |  [![image](https://img.shields.io/pypi/v/avilla-elizabeth)](https://pypi.org/project/avilla-elizabeth)  | Official | AGPLv3 |
-|      [Onebot 11](avilla/onebot/v11)       |      `OneBot v11`      |  **WIP**  | [![image](https://img.shields.io/pypi/v/avilla-onebot-v11)](https://pypi.org/project/avilla-onebot-v11) | Official |   -    |
-|          [-](avilla/onebot/v12)           |      `OneBot v12`      | **Draft** | [![image](https://img.shields.io/pypi/v/avilla-onebot-v12)](https://pypi.org/project/avilla-onebot-v12) |    -     |   -    |
-|        [Telegram](avilla/telegram)        |       `Telegram`       | **Draft** |   [![image](https://img.shields.io/pypi/v/avilla-telegram)](https://pypi.org/project/avilla-telegram)   |    -     |   -    |
-|       [Nightcord](avilla/nightcord)       |     `Discord Bots`     | **Draft** |  [![image](https://img.shields.io/pypi/v/avilla-nightcord)](https://pypi.org/project/avilla-nightcord)  |    -     |   -    |
-|         [Console](avilla/console)         |       `Console`        | **Alpha** |    [![image](https://img.shields.io/pypi/v/avilla-console)](https://pypi.org/project/avilla-console)    | Official |  MIT   |
-| [QQGuild Tencent](avilla/qqguild/tencent) | `QQGuild Official API` |  **WIP**  |    [![image](https://img.shields.io/pypi/v/avilla-qqguild)](https://pypi.org/project/avilla-qqguild)    | Official |  MIT   |
-|             [Red](avilla/red)             |     `red-protocol`     |  **WIP**  |        [![image](https://img.shields.io/pypi/v/avilla-red)](https://pypi.org/project/avilla-red)        | Official |  MIT   |
-|            [Kook](avilla/kook)            |  `Kook Official API`   | **Draft** |       [![image](https://img.shields.io/pypi/v/avilla-kook)](https://pypi.org/project/avilla-kook)       |    -     |   -    |
+|                      代号                      |       对接平台       |           协议           |    开发进度     |                                                       PyPI                                                        |   维护者    |  开源协议  |
+|:--------------------------------------------:|:----------------:|:----------------------:|:-----------:|:-----------------------------------------------------------------------------------------------------------------:|:--------:|:------:|
+|             [Core](avilla/core)              |        -         |           -            |  **Alpha**  |            [![image](https://img.shields.io/pypi/v/avilla-core)](https://pypi.org/project/avilla-core)            | Official |  MIT   |
+|          [Console](avilla/console)           |       终端环境       |       `Console`        |  **Alpha**  |         [![image](https://img.shields.io/pypi/v/avilla-console)](https://pypi.org/project/avilla-console)         | Official |  MIT   |
+|        [Elizabeth](avilla/elizabeth)         |    Tencent QQ    |    `mirai-api-http`    |  **Alpha**  |       [![image](https://img.shields.io/pypi/v/avilla-elizabeth)](https://pypi.org/project/avilla-elizabeth)       | Official | AGPLv3 |
+|        [Onebot 11](avilla/onebot/v11)        |     *多平台支持*      |      `OneBot v11`      |   **WIP**   |      [![image](https://img.shields.io/pypi/v/avilla-onebot-v11)](https://pypi.org/project/avilla-onebot-v11)      | Official |   -    |
+| [QQ Guild (Tencent)](avilla/qqguild/tencent) | Tencent QQ Guild | `QQGuild Official API` |   **WIP**   | [![image](https://img.shields.io/pypi/v/avilla-qqguild-tencent)](https://pypi.org/project/avilla-qqguild-tencent) | Official |  MIT   |
+|              [Red](avilla/red)               |   Tencent QQNT   |     `Red Protocol`     |   **WIP**   |             [![image](https://img.shields.io/pypi/v/avilla-red)](https://pypi.org/project/avilla-red)             | Official |  MIT   |
+|         [Telegram](avilla/telegram)          |     Telegram     |       `Telegram`       |  **Draft**  |        [![image](https://img.shields.io/pypi/v/avilla-telegram)](https://pypi.org/project/avilla-telegram)        |    -     |   -    |
+|        [Nightcord](avilla/nightcord)         |     Discord      |     `Discord Bots`     |  **Draft**  |       [![image](https://img.shields.io/pypi/v/avilla-nightcord)](https://pypi.org/project/avilla-nightcord)       |    -     |   -    |
+|             [Kook](avilla/kook)              |       Kook       |         `Kook`         |  **Draft**  |            [![image](https://img.shields.io/pypi/v/avilla-kook)](https://pypi.org/project/avilla-kook)            |    -     |   -    |
+|        [OneBot 12](avilla/onebot/v12)        |     *多平台支持*      |      `OneBot v12`      | **Planned** |                                                         -                                                         |    -     |   -    |
+
 ## 我们的愿景
 
 创造出比这之前还要更加具有潜力和创造性的作品, 借此有力促进社区的发展,
 助力社区的艺术家们 (Developers & Artists) 以更高的效率, 基于更完善的底层, 创作出更加精彩的作品.
 
 ## 相关项目
```

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/account.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
 from typing import TYPE_CHECKING
 
+from launart.utilles import any_completed
+
 from avilla.core.account import AccountStatus, BaseAccount
 from avilla.core.selector import Selector
 from avilla.onebot.v11.net.ws_server import OneBot11WsServerConnection
 from avilla.standard.core.account import AccountAvailable, AccountUnavailable
-from launart.utilles import any_completed
 
 if TYPE_CHECKING:
     from .net.ws_client import OneBot11WsClientNetworking
     from .protocol import OneBot11Protocol
 
 
 class OneBot11Account(BaseAccount):
```

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/collector/connection.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/collector/connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, ClassVar, TypeVar
 
-from avilla.core.ryanvk.collector.base import BaseCollector, PerformTemplate
-from avilla.core.ryanvk.endpoint import Access
+from avilla.core.ryanvk.collector.base import AvillaBaseCollector, BasePerform
+from graia.ryanvk import Access
 
 if TYPE_CHECKING:
     from avilla.onebot.v11.net.ws_client import OneBot11WsClientNetworking
     from avilla.onebot.v11.protocol import OneBot11Protocol
 
 
 T = TypeVar("T")
 T1 = TypeVar("T1")
 
 
-class ConnectionBasedPerformTemplate(PerformTemplate, native=True):
+class ConnectionBasedPerformTemplate(BasePerform, native=True):
     __collector__: ClassVar[ConnectionCollector]
 
     protocol: Access[OneBot11Protocol] = Access()
     connection: Access[OneBot11WsClientNetworking] = Access()
 
 
-class ConnectionCollector(BaseCollector):
+class ConnectionCollector(AvillaBaseCollector):
     post_applying: bool = False
 
     @property
     def _(self):
-        upper = super().get_collect_template()
+        upper = super()._
 
         class PerformTemplate(
             ConnectionBasedPerformTemplate,
             upper,
             native=True,
         ):
             ...
```

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/net/base.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/net/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,8 +79,8 @@
             result = await future
         finally:
             del self.response_waiters[echo]
 
         if result["status"] != "ok":
             raise ActionFailed(f"{result['retcode']}: {result}")
 
-        return result["data"]
+        return result.get("data")
```

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/net/ws_client.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/net/ws_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 from __future__ import annotations
 
 import asyncio
 import json
-from collections import ChainMap
-from dataclasses import dataclass
 from typing import TYPE_CHECKING, cast
 
 import aiohttp
+from launart import Service
+from launart.manager import Launart
+from launart.utilles import any_completed
 from loguru import logger
-from yarl import URL
 
 from avilla.onebot.v11.account import OneBot11Account
 from avilla.onebot.v11.net.base import OneBot11Networking
 from avilla.standard.core.account import AccountUnregistered
-from launart import Service
-from launart.manager import Launart
-from launart.utilles import any_completed
 
 if TYPE_CHECKING:
-    from avilla.onebot.v11.protocol import OneBot11Protocol
-
-
-@dataclass
-class OneBot11WsClientConfig:
-    endpoint: URL
-    access_token: str | None = None
+    from avilla.onebot.v11.protocol import OneBot11Protocol, OneBot11ForwardConfig
 
 
 class OneBot11WsClientNetworking(OneBot11Networking["OneBot11WsClientNetworking"], Service):
-    id = "onebot/v11/connection/websocket/client"
-
     required: set[str] = set()
     stages: set[str] = {"preparing", "blocking", "cleanup"}
 
-    config: OneBot11WsClientConfig
+    config: OneBot11ForwardConfig
     connection: aiohttp.ClientWebSocketResponse | None = None
 
-    def __init__(self, protocol: OneBot11Protocol, config: OneBot11WsClientConfig) -> None:
+    def __init__(self, protocol: OneBot11Protocol, config: OneBot11ForwardConfig) -> None:
         super().__init__(protocol)
         self.config = config
 
+    @property
+    def id(self):
+        return f"onebot/v11/connection/websocket/client#{id(self)}"
+
     async def message_receive(self):
         if self.connection is None:
             raise RuntimeError("connection is not established")
 
         async for msg in self.connection:
             if msg.type in {aiohttp.WSMsgType.CLOSE, aiohttp.WSMsgType.ERROR, aiohttp.WSMsgType.CLOSED}:
                 self.close_signal.set()
@@ -66,15 +59,15 @@
     def get_staff_components(self):
         return {"connection": self, "protocol": self.protocol, "avilla": self.protocol.avilla}
 
     def __staff_generic__(self, element_type: dict, event_type: dict):
         ...
 
     def get_staff_artifacts(self):
-        return ChainMap(self.protocol.isolate.artifacts, self.protocol.avilla.isolate.artifacts)
+        return [self.protocol.artifacts, self.protocol.avilla.global_artifacts]
 
     @property
     def alive(self):
         return self.connection is not None and not self.connection.closed
 
     async def connection_daemon(self, manager: Launart, session: aiohttp.ClientSession):
         avilla = self.protocol.avilla
```

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/net/ws_server.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/net/ws_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 from __future__ import annotations
 
-from collections import ChainMap
 from contextlib import suppress
-from dataclasses import dataclass
 from typing import TYPE_CHECKING, cast
 
+from launart import Service
+from launart.manager import Launart
+from launart.utilles import any_completed
 from starlette.applications import Starlette
 from starlette.routing import WebSocketRoute
 from starlette.websockets import WebSocket
 
 from avilla.onebot.v11.net.base import OneBot11Networking
 from avilla.standard.core.account import AccountUnregistered
 from graia.amnesia.builtins.asgi import UvicornASGIService
-from launart import Service
-from launart.manager import Launart
-from launart.utilles import any_completed
 
 if TYPE_CHECKING:
     from avilla.onebot.v11.account import OneBot11Account
-    from avilla.onebot.v11.protocol import OneBot11Protocol
-
-
-@dataclass
-class OneBot11WsServerConfig:
-    endpoint: str
-    access_token: str | None = None
+    from avilla.onebot.v11.protocol import OneBot11Protocol, OneBot11ReverseConfig
 
 
 class OneBot11WsServerConnection(OneBot11Networking["OneBot11WsServerConnection"]):
     connection: WebSocket
 
     def __init__(self, connection: WebSocket, protocol: OneBot11Protocol):
         self.connection = connection
@@ -54,15 +46,15 @@
     def get_staff_components(self):
         return {"connection": self, "protocol": self.protocol, "avilla": self.protocol.avilla}
 
     def __staff_generic__(self, element_type: dict, event_type: dict):
         ...
 
     def get_staff_artifacts(self):
-        return ChainMap(self.protocol.isolate.artifacts, self.protocol.avilla.isolate.artifacts)
+        return [self.protocol.artifacts, self.protocol.avilla.global_artifacts]
 
     async def send(self, payload: dict) -> None:
         return await self.connection.send_json(payload)
 
     async def unregister_account(self):
         avilla = self.protocol.avilla
         for n in list(avilla.accounts.keys()):
@@ -70,29 +62,32 @@
             account.status.enabled = False
             await avilla.broadcast.postEvent(AccountUnregistered(avilla, avilla.accounts[n].account))
             if n.follows("land(qq).account") and int(n["account"]) in self.accounts:
                 del avilla.accounts[n]
 
 
 class OneBot11WsServerNetworking(Service):
-    id = "onebot/v11/connection/websocket/server"
     required: set[str] = {"asgi.service/uvicorn"}
     stages: set[str] = {"preparing", "blocking", "cleanup"}
 
     protocol: OneBot11Protocol
-    config: OneBot11WsServerConfig
+    config: OneBot11ReverseConfig
 
     connections: dict[str, OneBot11WsServerConnection]
 
-    def __init__(self, protocol: OneBot11Protocol, config: OneBot11WsServerConfig) -> None:
+    def __init__(self, protocol: OneBot11Protocol, config: OneBot11ReverseConfig) -> None:
         self.protocol = protocol
         self.config = config
         self.connections = {}
         super().__init__()
 
+    @property
+    def id(self):
+        return f"onebot/v11/connection/websocket/server#{id(self)}"
+
     async def websocket_server_handler(self, ws: WebSocket):
         if ws.headers["Authorization"][6:] != self.config.access_token:
             return await ws.close()
 
         account_id = ws.headers["X-Self-ID"]
 
         await ws.accept()
```

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/action/admin.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/action/admin.py`

 * *Files identical despite different names*

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/action/ban.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/action/ban.py`

 * *Files identical despite different names*

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/action/leave.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/action/leave.py`

 * *Files identical despite different names*

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/action/mute.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/action/mute.py`

 * *Files identical despite different names*

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/event/lifespan.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/event/lifespan.py`

 * *Files identical despite different names*

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/event/message.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/event/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         context = Context(
             account,
             friend,
             friend,
             friend,
             Selector().land(account.route["land"]).account(str(raw_event["self_id"])),
         )
-        message = await account.staff.x({"context": context}).deserialize_message(raw_event["message"])
+        message = await account.staff.ext({"context": context}).deserialize_message(raw_event["message"])
         reply = None
         if i := message.get(Reply):
             reply = friend.message(i[0].id)
             message = message.exclude(Reply)
 
         return MessageReceived(
             context,
@@ -62,15 +62,15 @@
         context = Context(
             account,
             member,
             member,
             member,
             group.member(str(raw_event["self_id"])),
         )
-        message = await account.staff.x({"context": context}).deserialize_message(raw_event["message"])
+        message = await account.staff.ext({"context": context}).deserialize_message(raw_event["message"])
         reply = None
         if i := message.get(Reply):
             reply = member.message(i[0].id)
             message = message.exclude(Reply)
         return MessageReceived(
             context,
             Message(
@@ -96,15 +96,15 @@
         context = Context(
             account,
             member,
             group,
             group,
             group.member(str(raw_event["self_id"])),
         )
-        message = await account.staff.x({"context": context}).deserialize_message(raw_event["message"])
+        message = await account.staff.ext({"context": context}).deserialize_message(raw_event["message"])
         reply = None
         if i := message.get(Reply):
             reply = group.message(i[0].id)
             message = message.exclude(Reply)
         return MessageReceived(
             context,
             Message(
@@ -128,15 +128,15 @@
         context = Context(
             account,
             stranger,
             stranger,
             stranger,
             Selector().land(account.route["land"]).account(str(raw_event["self_id"])),
         )
-        message = await account.staff.x({"context": context}).deserialize_message(raw_event["message"])
+        message = await account.staff.ext({"context": context}).deserialize_message(raw_event["message"])
         reply = None
         if i := message.get(Reply):
             reply = stranger.message(i[0].id)
             message = message.exclude(Reply)
         return MessageReceived(
             context,
             Message(
@@ -161,15 +161,15 @@
         context = Context(
             account,
             people,
             group,
             group,
             group.member(str(raw_event["self_id"])),
         )
-        message = await account.staff.x({"context": context}).deserialize_message(raw_event["message"])
+        message = await account.staff.ext({"context": context}).deserialize_message(raw_event["message"])
         reply = None
         if i := message.get(Reply):
             reply = group.message(i[0].id)
             message = message.exclude(Reply)
         return MessageReceived(
             context,
             Message(
@@ -189,15 +189,15 @@
         if account is None:
             logger.warning(f"Unknown account {self_id} sent message {raw_event}")
             return
 
         group = Selector().land(account.route["land"]).group(str(raw_event["group_id"]))
         member = group.member(str(raw_event["user_id"]))
         context = Context(account, member, group, group, member)
-        message = await account.staff.x({"context": context}).deserialize_message(raw_event["message"])
+        message = await account.staff.ext({"context": context}).deserialize_message(raw_event["message"])
         reply = None
         if i := message.get(Reply):
             reply = member.message(i[0].id)
             message = message.exclude(Reply)
         return MessageSent(
             context,
             Message(
```

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/event/notice.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/event/notice.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,20 +218,25 @@
     @EventParse.collect(m, "notice.notify.poke")
     async def nudge_received(self, raw_event: dict):
         self_id = raw_event["self_id"]
         account = self.connection.accounts.get(self_id)
         if account is None:
             logger.warning(f"Unknown account {self_id} sent message {raw_event}")
             return
-
-        group = Selector().land(account.route["land"]).group(str(raw_event["group_id"]))
-        target = group.member(str(raw_event["target_id"]))
-        operator = group.message(str(raw_event["user_id"]))
-        context = Context(account, operator, target, group, group.member(str(self_id)))
-        return ActivityTrigged(context, target.activity("nudge"), target.nudge("_"), operator, group)
+        if "group_id" in raw_event:
+            group = Selector().land(account.route["land"]).group(str(raw_event["group_id"]))
+            target = group.member(str(raw_event["target_id"]))
+            operator = group.message(str(raw_event["user_id"]))
+            context = Context(account, operator, target, group, group.member(str(self_id)))
+            return ActivityTrigged(context, "nudge", group, target.nudge("_"), operator)
+        else:
+            friend = Selector().land(account.route["land"]).friend(str(raw_event["sender_id"]))
+            selft = account.route
+            context = Context(account, friend, selft, friend, selft)
+            return ActivityTrigged(context, "nudge", friend, friend.nudge("_"), friend)
 
     @EventParse.collect(m, "notice.notify.lucky_king")
     async def lucky_king_received(self, raw_event: dict):
         self_id = raw_event["self_id"]
         account = self.connection.accounts.get(self_id)
         if account is None:
             logger.warning(f"Unknown account {self_id} sent message {raw_event}")
```

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/event/request.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/event/request.py`

 * *Files identical despite different names*

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/message/deserialize.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/message/deserialize.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from __future__ import annotations
 
+from datetime import datetime
 from typing import TYPE_CHECKING
 
 from avilla.core.elements import Notice, NoticeAll, Picture, Text
 from avilla.core.ryanvk.collector.application import ApplicationCollector
 from avilla.core.ryanvk.descriptor.message.deserialize import MessageDeserialize
-from avilla.core.ryanvk.endpoint import OptionalAccess
 from avilla.core.selector import Selector
 from avilla.onebot.v11.element import Reply
 from avilla.onebot.v11.resource import OneBot11ImageResource
-from avilla.standard.qq.elements import Dice, Face, FlashImage, Json, Poke, Share, Xml
+from avilla.standard.qq.elements import Dice, Face, FlashImage, Json, Poke, Share, Xml, Forward, Node
+from graia.ryanvk import OptionalAccess
 
 if TYPE_CHECKING:
     from avilla.core.context import Context
+    from avilla.onebot.v11.account import OneBot11Account
 
 OneBot11MessageDeserialize = MessageDeserialize[dict]
 
 
 class OneBot11MessageDeserializePerform((m := ApplicationCollector())._):
     m.post_applying = True
 
     context: OptionalAccess[Context] = OptionalAccess()
+    account: OptionalAccess[OneBot11Account] = OptionalAccess()
     # LINK: https://github.com/microsoft/pyright/issues/5409
 
     @OneBot11MessageDeserialize.collect(m, "text")
     async def text(self, raw_element: dict) -> Text:
         return Text(raw_element["data"]["text"])
 
     @OneBot11MessageDeserialize.collect(m, "face")
@@ -70,8 +73,35 @@
         return Share(
             raw_element["data"]["url"],
             raw_element["data"]["title"],
             raw_element["data"].get("content", None),
             raw_element["data"].get("image", None),
         )
 
+    @OneBot11MessageDeserialize.collect(m, "forward")
+    async def forward(self, raw_element: dict):
+        elem = Forward(raw_element["data"]["id"])
+        if not self.account:
+            return elem
+        result = await self.account.call(
+            "get_forward_msg",
+            {
+                "message_id": raw_element["data"]["id"],
+            },
+        )
+        if result is None:
+            return elem
+        for msg in result["messages"]:
+            node = Node(
+                name=msg["sender"]["nickname"],
+                uid=str(msg["sender"]["user_id"]),
+                time=datetime.fromtimestamp(msg["time"]),
+                content=(
+                    await self.account.staff
+                    .ext({"context": self.context})
+                    .deserialize_message(msg["content"])
+                )
+            )
+            elem.nodes.append(node)
+        return elem
+
     # TODO
```

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/message/serialize.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/message/serialize.py`

 * *Files identical despite different names*

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/query/group.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/query/group.py`

 * *Files identical despite different names*

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/perform/resource_fetch.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/perform/resource_fetch.py`

 * *Files identical despite different names*

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/resource.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/resource.py`

 * *Files identical despite different names*

### Comparing `avilla_onebot_v11-1.0.0a6/avilla/onebot/v11/service.py` & `avilla_onebot_v11-1.0.0a7/avilla/onebot/v11/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+from launart import Launart, Service, any_completed
+
 from avilla.onebot.v11.net.ws_client import OneBot11WsClientNetworking
 from avilla.onebot.v11.net.ws_server import OneBot11WsServerNetworking
-from launart import Launart, Service, any_completed
 
 if TYPE_CHECKING:
     from .protocol import OneBot11Protocol
 
 
 class OneBot11Service(Service):
     id = "onebot11.service"
```

### Comparing `avilla_onebot_v11-1.0.0a6/PKG-INFO` & `avilla_onebot_v11-1.0.0a7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avilla-onebot-v11
-Version: 1.0.0a6
+Version: 1.0.0a7
 Home-page: https://github.com/GraiaProject/Avilla
 Author-Email: GreyElaina <GreyElaina@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/GraiaProject/Avilla
 Project-URL: Repository, https://github.com/GraiaProject/Avilla
 Requires-Python: >=3.9
 Requires-Dist: aiohttp>=3.8.1
@@ -48,48 +48,44 @@
   > 担心可用性? 我们同样提供了一些核心的非平台依赖实现, 例如 `TextCommand`, 这些组件仅要求平台实现最基本的交互实现, 剩下的一切交给 Avilla 处理!
  - **现有基建兼容**: 得益于 `Amnesia`, `Commander`, `Twilight`, `Alconna` 或是基于 `Launart` 编写的各式扩展, 可以直接与 Avilla 协同而无需任何迁移成本.
  - **高可伸缩性**: Avilla 既支持单文件使用, 亦支持基于 Graia Saya 驱动的模块系统编写应用.
 
 ## Quick Start
 
 ```py
-from creart import create
-from launart import Launart
-from graia.broadcast import Broadcast
-
 from avilla.core import Avilla, Context, MessageReceived
 from avilla.console.protocol import ConsoleProtocol
 
-broadcast = create(Broadcast)
-launart = Launart()
-avilla = Avilla(broadcast, launart, [ConsoleProtocol()])
+avilla = Avilla()
+avilla.apply_protocols(ConsoleProtocol())
 
 
-@broadcast.receiver(MessageReceived)
+@avilla.listen(MessageReceived)
 async def on_message_received(cx: Context, event: MessageReceived):
     await cx.scene.send_message("Hello, Avilla!")
 
 
-launart.launch_blocking(loop=broadcast.loop)
+avilla.launch()
 ```
 
 ## 部件发布情况
 
-|                    代号                     |           协议           |   开发进度    |                                                  PyPI                                                   |   维护者    |  开源协议  |
-|:-----------------------------------------:|:----------------------:|:---------:|:-------------------------------------------------------------------------------------------------------:|:--------:|:------:|
-|            [Core](avilla/core)            |           -            | **Alpha** |       [![image](https://img.shields.io/pypi/v/avilla-core)](https://pypi.org/project/avilla-core)       | Official |  MIT   |
-|       [Elizabeth](avilla/elizabeth)       |    `mirai-api-http`    |  **WIP**  |  [![image](https://img.shields.io/pypi/v/avilla-elizabeth)](https://pypi.org/project/avilla-elizabeth)  | Official | AGPLv3 |
-|      [Onebot 11](avilla/onebot/v11)       |      `OneBot v11`      |  **WIP**  | [![image](https://img.shields.io/pypi/v/avilla-onebot-v11)](https://pypi.org/project/avilla-onebot-v11) | Official |   -    |
-|          [-](avilla/onebot/v12)           |      `OneBot v12`      | **Draft** | [![image](https://img.shields.io/pypi/v/avilla-onebot-v12)](https://pypi.org/project/avilla-onebot-v12) |    -     |   -    |
-|        [Telegram](avilla/telegram)        |       `Telegram`       | **Draft** |   [![image](https://img.shields.io/pypi/v/avilla-telegram)](https://pypi.org/project/avilla-telegram)   |    -     |   -    |
-|       [Nightcord](avilla/nightcord)       |     `Discord Bots`     | **Draft** |  [![image](https://img.shields.io/pypi/v/avilla-nightcord)](https://pypi.org/project/avilla-nightcord)  |    -     |   -    |
-|         [Console](avilla/console)         |       `Console`        | **Alpha** |    [![image](https://img.shields.io/pypi/v/avilla-console)](https://pypi.org/project/avilla-console)    | Official |  MIT   |
-| [QQGuild Tencent](avilla/qqguild/tencent) | `QQGuild Official API` |  **WIP**  |    [![image](https://img.shields.io/pypi/v/avilla-qqguild)](https://pypi.org/project/avilla-qqguild)    | Official |  MIT   |
-|             [Red](avilla/red)             |     `red-protocol`     |  **WIP**  |        [![image](https://img.shields.io/pypi/v/avilla-red)](https://pypi.org/project/avilla-red)        | Official |  MIT   |
-|            [Kook](avilla/kook)            |  `Kook Official API`   | **Draft** |       [![image](https://img.shields.io/pypi/v/avilla-kook)](https://pypi.org/project/avilla-kook)       |    -     |   -    |
+|                      代号                      |       对接平台       |           协议           |    开发进度     |                                                       PyPI                                                        |   维护者    |  开源协议  |
+|:--------------------------------------------:|:----------------:|:----------------------:|:-----------:|:-----------------------------------------------------------------------------------------------------------------:|:--------:|:------:|
+|             [Core](avilla/core)              |        -         |           -            |  **Alpha**  |            [![image](https://img.shields.io/pypi/v/avilla-core)](https://pypi.org/project/avilla-core)            | Official |  MIT   |
+|          [Console](avilla/console)           |       终端环境       |       `Console`        |  **Alpha**  |         [![image](https://img.shields.io/pypi/v/avilla-console)](https://pypi.org/project/avilla-console)         | Official |  MIT   |
+|        [Elizabeth](avilla/elizabeth)         |    Tencent QQ    |    `mirai-api-http`    |  **Alpha**  |       [![image](https://img.shields.io/pypi/v/avilla-elizabeth)](https://pypi.org/project/avilla-elizabeth)       | Official | AGPLv3 |
+|        [Onebot 11](avilla/onebot/v11)        |     *多平台支持*      |      `OneBot v11`      |   **WIP**   |      [![image](https://img.shields.io/pypi/v/avilla-onebot-v11)](https://pypi.org/project/avilla-onebot-v11)      | Official |   -    |
+| [QQ Guild (Tencent)](avilla/qqguild/tencent) | Tencent QQ Guild | `QQGuild Official API` |   **WIP**   | [![image](https://img.shields.io/pypi/v/avilla-qqguild-tencent)](https://pypi.org/project/avilla-qqguild-tencent) | Official |  MIT   |
+|              [Red](avilla/red)               |   Tencent QQNT   |     `Red Protocol`     |   **WIP**   |             [![image](https://img.shields.io/pypi/v/avilla-red)](https://pypi.org/project/avilla-red)             | Official |  MIT   |
+|         [Telegram](avilla/telegram)          |     Telegram     |       `Telegram`       |  **Draft**  |        [![image](https://img.shields.io/pypi/v/avilla-telegram)](https://pypi.org/project/avilla-telegram)        |    -     |   -    |
+|        [Nightcord](avilla/nightcord)         |     Discord      |     `Discord Bots`     |  **Draft**  |       [![image](https://img.shields.io/pypi/v/avilla-nightcord)](https://pypi.org/project/avilla-nightcord)       |    -     |   -    |
+|             [Kook](avilla/kook)              |       Kook       |         `Kook`         |  **Draft**  |            [![image](https://img.shields.io/pypi/v/avilla-kook)](https://pypi.org/project/avilla-kook)            |    -     |   -    |
+|        [OneBot 12](avilla/onebot/v12)        |     *多平台支持*      |      `OneBot v12`      | **Planned** |                                                         -                                                         |    -     |   -    |
+
 ## 我们的愿景
 
 创造出比这之前还要更加具有潜力和创造性的作品, 借此有力促进社区的发展,
 助力社区的艺术家们 (Developers & Artists) 以更高的效率, 基于更完善的底层, 创作出更加精彩的作品.
 
 ## 相关项目
```

