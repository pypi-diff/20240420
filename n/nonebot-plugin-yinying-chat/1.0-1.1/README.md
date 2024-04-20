# Comparing `tmp/nonebot-plugin-yinying-chat-1.0.tar.gz` & `tmp/nonebot-plugin-yinying-chat-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-yinying-chat-1.0.tar", last modified: Fri Apr 19 09:39:46 2024, max compression
+gzip compressed data, was "nonebot-plugin-yinying-chat-1.1.tar", last modified: Sat Apr 20 14:02:58 2024, max compression
```

## Comparing `nonebot-plugin-yinying-chat-1.0.tar` & `nonebot-plugin-yinying-chat-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-19 09:39:46.367516 nonebot-plugin-yinying-chat-1.0/
--rw-r--r--   0 stafx     (1000) stafx     (1000)      235 2024-04-19 09:39:46.367516 nonebot-plugin-yinying-chat-1.0/PKG-INFO
--rw-r--r--   0 stafx     (1000) stafx     (1000)      968 2024-04-16 04:48:34.000000 nonebot-plugin-yinying-chat-1.0/README.md
-drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-19 09:39:46.367516 nonebot-plugin-yinying-chat-1.0/nonebot_plugin_yinying_chat/
--rw-r--r--   0 stafx     (1000) stafx     (1000)     2413 2024-04-17 15:23:28.000000 nonebot-plugin-yinying-chat-1.0/nonebot_plugin_yinying_chat/ChatSession.py
--rw-r--r--   0 stafx     (1000) stafx     (1000)     4859 2024-04-19 09:35:54.000000 nonebot-plugin-yinying-chat-1.0/nonebot_plugin_yinying_chat/__init__.py
--rw-r--r--   0 stafx     (1000) stafx     (1000)      588 2024-04-18 08:46:46.000000 nonebot-plugin-yinying-chat-1.0/nonebot_plugin_yinying_chat/config.py
-drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-19 09:39:46.367516 nonebot-plugin-yinying-chat-1.0/nonebot_plugin_yinying_chat.egg-info/
--rw-r--r--   0 stafx     (1000) stafx     (1000)      235 2024-04-19 09:39:46.000000 nonebot-plugin-yinying-chat-1.0/nonebot_plugin_yinying_chat.egg-info/PKG-INFO
--rw-r--r--   0 stafx     (1000) stafx     (1000)      408 2024-04-19 09:39:46.000000 nonebot-plugin-yinying-chat-1.0/nonebot_plugin_yinying_chat.egg-info/SOURCES.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)        1 2024-04-19 09:39:46.000000 nonebot-plugin-yinying-chat-1.0/nonebot_plugin_yinying_chat.egg-info/dependency_links.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)       64 2024-04-19 09:39:46.000000 nonebot-plugin-yinying-chat-1.0/nonebot_plugin_yinying_chat.egg-info/requires.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)       28 2024-04-19 09:39:46.000000 nonebot-plugin-yinying-chat-1.0/nonebot_plugin_yinying_chat.egg-info/top_level.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)      548 2024-04-19 09:39:40.000000 nonebot-plugin-yinying-chat-1.0/pyproject.toml
--rw-r--r--   0 stafx     (1000) stafx     (1000)       38 2024-04-19 09:39:46.367516 nonebot-plugin-yinying-chat-1.0/setup.cfg
--rw-r--r--   0 stafx     (1000) stafx     (1000)      397 2024-04-19 09:39:33.000000 nonebot-plugin-yinying-chat-1.0/setup.py
+drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-20 14:02:58.009631 nonebot-plugin-yinying-chat-1.1/
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      235 2024-04-20 14:02:58.009631 nonebot-plugin-yinying-chat-1.1/PKG-INFO
+-rw-r--r--   0 stafx     (1000) stafx     (1000)     1896 2024-04-19 10:33:26.000000 nonebot-plugin-yinying-chat-1.1/README.md
+drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-20 14:02:58.009631 nonebot-plugin-yinying-chat-1.1/nonebot_plugin_yinying_chat/
+-rw-r--r--   0 stafx     (1000) stafx     (1000)     2413 2024-04-19 10:33:26.000000 nonebot-plugin-yinying-chat-1.1/nonebot_plugin_yinying_chat/ChatSession.py
+-rw-r--r--   0 stafx     (1000) stafx     (1000)     4861 2024-04-19 10:33:26.000000 nonebot-plugin-yinying-chat-1.1/nonebot_plugin_yinying_chat/__init__.py
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      561 2024-04-20 14:00:00.000000 nonebot-plugin-yinying-chat-1.1/nonebot_plugin_yinying_chat/config.py
+drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-20 14:02:58.009631 nonebot-plugin-yinying-chat-1.1/nonebot_plugin_yinying_chat.egg-info/
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      235 2024-04-20 14:02:57.000000 nonebot-plugin-yinying-chat-1.1/nonebot_plugin_yinying_chat.egg-info/PKG-INFO
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      408 2024-04-20 14:02:57.000000 nonebot-plugin-yinying-chat-1.1/nonebot_plugin_yinying_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)        1 2024-04-20 14:02:57.000000 nonebot-plugin-yinying-chat-1.1/nonebot_plugin_yinying_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)       64 2024-04-20 14:02:57.000000 nonebot-plugin-yinying-chat-1.1/nonebot_plugin_yinying_chat.egg-info/requires.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)       28 2024-04-20 14:02:57.000000 nonebot-plugin-yinying-chat-1.1/nonebot_plugin_yinying_chat.egg-info/top_level.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      529 2024-04-20 14:02:41.000000 nonebot-plugin-yinying-chat-1.1/pyproject.toml
+-rw-r--r--   0 stafx     (1000) stafx     (1000)       38 2024-04-20 14:02:58.009631 nonebot-plugin-yinying-chat-1.1/setup.cfg
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      397 2024-04-20 14:02:49.000000 nonebot-plugin-yinying-chat-1.1/setup.py
```

### Comparing `nonebot-plugin-yinying-chat-1.0/nonebot_plugin_yinying_chat/ChatSession.py` & `nonebot-plugin-yinying-chat-1.1/nonebot_plugin_yinying_chat/ChatSession.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-yinying-chat-1.0/nonebot_plugin_yinying_chat/__init__.py` & `nonebot-plugin-yinying-chat-1.1/nonebot_plugin_yinying_chat/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -126,8 +126,8 @@
         async with http_session.post(
                 "https://api-yinying-ng.wingmark.cn/v1/chatWithCyberFurry",
                 headers={"Authorization": f"Bearer {custom_api_token}"},
                 json=custom_api_data,
         ) as response:
             response_data = await response.json()
             print(f"Response Data: {response_data}")
-            return response_data["choices"][0]["message"]["content"]
+            return response_data["choices"][0]["message"]["content"]
```

### Comparing `nonebot-plugin-yinying-chat-1.0/nonebot_plugin_yinying_chat/config.py` & `nonebot-plugin-yinying-chat-1.1/nonebot_plugin_yinying_chat/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from pydantic import Extra, BaseModel
+from pydantic import BaseModel
 from typing import Optional
 import nonebot
 
 
 #定义配置文件
-class Config(BaseModel, extra=Extra.ignore):
+class Config(BaseModel):
     yinying_api_key: Optional[str] = "" # 在这里输入银影APIKEY
     yinying_model_name: Optional[str] = "" #在这里输入模型名称
     yinying_app_id: Optional[str] = ""    #在这里输入AppID
     enable_private_chat: bool = True    #是否开启私聊
     yinying_chat_public: bool = False  # 群聊是否开启公共会话
```

### Comparing `nonebot-plugin-yinying-chat-1.0/pyproject.toml` & `nonebot-plugin-yinying-chat-1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "nonebot-plugin-yinying-chat"
-version = "1.0"
+version = "1.1"
 description = "A nonebot plugin for yinying-chat"
 authors = ["Yuanluo <3313512421@qq.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0rc3"
 nonebot-adapter-onebot = "^2.2.1"
-openai = "^0.27.0"
 aiohttp = "^3.8.4"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
 default = true
```

