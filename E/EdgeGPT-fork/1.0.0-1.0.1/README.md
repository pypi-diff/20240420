# Comparing `tmp/edgegpt_fork-1.0.0.tar.gz` & `tmp/edgegpt_fork-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegpt_fork-1.0.0.tar", last modified: Sun Apr 14 13:51:53 2024, max compression
+gzip compressed data, was "edgegpt_fork-1.0.1.tar", last modified: Sat Apr 20 08:34:54 2024, max compression
```

## Comparing `edgegpt_fork-1.0.0.tar` & `edgegpt_fork-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:53.310997 edgegpt_fork-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-04-14 13:51:53.310997 edgegpt_fork-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11545 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-14 13:51:53.310997 edgegpt_fork-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:53.306996 edgegpt_fork-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:53.310997 edgegpt_fork-1.0.0/src/EdgeGPT/
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/EdgeUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/ImageGen.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/chathub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/conversation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:53.310997 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-04-14 13:51:53.000000 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-14 13:51:53.000000 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:51:53.000000 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-14 13:51:53.000000 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-14 13:51:53.000000 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-14 13:51:53.000000 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:34:54.681898 edgegpt_fork-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-04-20 08:34:54.681898 edgegpt_fork-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11545 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-20 08:34:54.681898 edgegpt_fork-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:34:54.677898 edgegpt_fork-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:34:54.677898 edgegpt_fork-1.0.1/src/EdgeGPT/
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/EdgeUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/ImageGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13359 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/chathub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/conversation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-20 08:34:33.000000 edgegpt_fork-1.0.1/src/EdgeGPT/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:34:54.681898 edgegpt_fork-1.0.1/src/EdgeGPT_fork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-04-20 08:34:54.000000 edgegpt_fork-1.0.1/src/EdgeGPT_fork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-20 08:34:54.000000 edgegpt_fork-1.0.1/src/EdgeGPT_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 08:34:54.000000 edgegpt_fork-1.0.1/src/EdgeGPT_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-20 08:34:54.000000 edgegpt_fork-1.0.1/src/EdgeGPT_fork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-20 08:34:54.000000 edgegpt_fork-1.0.1/src/EdgeGPT_fork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-20 08:34:54.000000 edgegpt_fork-1.0.1/src/EdgeGPT_fork.egg-info/top_level.txt
```

### Comparing `edgegpt_fork-1.0.0/LICENSE` & `edgegpt_fork-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.0/PKG-INFO` & `edgegpt_fork-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT-fork
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/xingty/EdgeGPT
 Author: Antonio Cheong,Bigbyto
 Author-email: acheong@student.dalat.org,bigbyto@gmail.com
 License: The Unlicense
 Project-URL: Bug Report, https://github.com/xingty/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT-fork Version: 1.0.0 Summary: Reverse
+Metadata-Version: 2.1 Name: EdgeGPT-fork Version: 1.0.1 Summary: Reverse
 engineered Edge Chat API Home-page: https://github.com/xingty/EdgeGPT Author:
 Antonio Cheong,Bigbyto Author-email:
 acheong@student.dalat.org,bigbyto@gmail.com License: The Unlicense Project-URL:
 Bug Report, https://github.com/xingty/EdgeGPT/issues/new Classifier: License ::
 OSI Approved :: The Unlicense (Unlicense) Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `edgegpt_fork-1.0.0/README.md` & `edgegpt_fork-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.0/setup.py` & `edgegpt_fork-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT-fork",
-    version="1.0.0",
+    version="1.0.1",
     license="The Unlicense",
     author="Antonio Cheong,Bigbyto",
     author_email="acheong@student.dalat.org,bigbyto@gmail.com",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/xingty/EdgeGPT",
```

### Comparing `edgegpt_fork-1.0.0/src/EdgeGPT/EdgeGPT.py` & `edgegpt_fork-1.0.1/src/EdgeGPT/EdgeGPT.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,42 +3,44 @@
 """
 from __future__ import annotations
 
 from .chathub import *
 from .conversation import *
 from .request import *
 from .utilities import *
+import time
 
 
 class Chatbot:
     """
     Combines everything to make it seamless
     """
 
     def __init__(
-        self,
-        proxy: str | None = None,
-        cookies: list[dict] | None = None,
+            self,
+            proxy: str | None = None,
+            cookies: list[dict] | None = None,
     ) -> None:
         self.proxy: str | None = proxy
         self.chat_hub: ChatHub = ChatHub(
             Conversation(self.proxy, cookies=cookies),
             proxy=self.proxy,
             cookies=cookies,
         )
 
     @staticmethod
     async def create(
-        proxy: str | None = None,
-        cookies: list[dict] | None = None,
+            proxy: str | None = None,
+            cookies: list[dict] | None = None,
+            conversation_id: Union[str, None] = None,
     ) -> Chatbot:
         self = Chatbot.__new__(Chatbot)
         self.proxy = proxy
         self.chat_hub = ChatHub(
-            await Conversation.create(self.proxy, cookies=cookies),
+            await Conversation.create(self.proxy, cookies=cookies, conversation_id=conversation_id),
             proxy=self.proxy,
             cookies=cookies,
         )
         return self
 
     async def save_conversation(self, filename: str) -> None:
         """
@@ -52,56 +54,68 @@
             f.write(
                 json.dumps(
                     {
                         "conversation_id": conversation_id,
                         "conversation_signature": conversation_signature,
                         "client_id": client_id,
                         "invocation_id": invocation_id,
+                        "expires": int(time.time()) + 86400 * 7,
                     },
                 ),
             )
 
     async def load_conversation(self, filename: str) -> None:
         """
         Load the conversation from a file
         """
         with open(filename) as f:
             conversation = json.load(f)
-            self.chat_hub.request = ChatHubRequest(
-                conversation_signature=conversation["conversation_signature"],
-                client_id=conversation["client_id"],
-                conversation_id=conversation["conversation_id"],
-                invocation_id=conversation["invocation_id"],
-            )
+            await self.load_conversation_from_json(conversation)
+
+    async def load_conversation_from_json(self, conversation: dict) -> None:
+        """
+        Load the conversation from a json file
+        """
+
+
+        self.chat_hub.request = ChatHubRequest(
+            conversation_signature=conversation["conversation_signature"],
+            client_id=conversation["client_id"],
+            conversation_id=conversation["conversation_id"],
+            invocation_id=conversation["invocation_id"],
+        )
+        self.chat_hub.sec_access_token = conversation["sec_access_token"]
+
 
     async def get_conversation(self) -> dict:
         """
         Gets the conversation history from conversation_id (requires load_conversation)
         """
         return await self.chat_hub.get_conversation()
 
     async def get_activity(self) -> dict:
         """
         Gets the recent activity (requires cookies)
         """
         return await self.chat_hub.get_activity()
 
     async def ask(
-        self,
-        prompt: str,
-        wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
-        conversation_style: CONVERSATION_STYLE_TYPE = None,
-        webpage_context: str | None = None,
-        search_result: bool = False,
-        locale: str = guess_locale(),
-        simplify_response: bool = False,
-        mode: str = None,
-        no_search: bool = True,
-        persona: Persona = Persona.copilot,
-        plugins: set[Plugin] = {}
+            self,
+            prompt: str,
+            wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
+            conversation_style: CONVERSATION_STYLE_TYPE = None,
+            webpage_context: str | None = None,
+            search_result: bool = False,
+            locale: str = guess_locale(),
+            simplify_response: bool = False,
+            mode: str = None,
+            no_search: bool = True,
+            persona: Persona = Persona.copilot,
+            plugins: set[Plugin] = {},
+            image_url: str = None,
     ) -> dict:
         """
         Ask a question to the bot
         Response:
             {
                 item (dict):
                     messages (list[dict]):
@@ -109,29 +123,30 @@
                             body (list[dict]):
                                 text (str): Response
             }
         To get the response, you can do:
             response["item"]["messages"][1]["adaptiveCards"][0]["body"][0]["text"]
         """
         async for final, response in self.chat_hub.ask_stream(
-            prompt=prompt,
-            conversation_style=conversation_style,
-            wss_link=wss_link,
-            webpage_context=webpage_context,
-            locale=locale,
-            no_search=no_search,
-            persona=persona,
-            plugins=plugins
+                prompt=prompt,
+                conversation_style=conversation_style,
+                wss_link=wss_link,
+                webpage_context=webpage_context,
+                locale=locale,
+                no_search=no_search,
+                persona=persona,
+                plugins=plugins,
+                image_url=image_url,
         ):
             if final:
                 if not simplify_response:
                     return response
                 messages_left = response["item"]["throttling"][
-                    "maxNumUserMessagesInConversation"
-                ] - response["item"]["throttling"].get(
+                                    "maxNumUserMessagesInConversation"
+                                ] - response["item"]["throttling"].get(
                     "numUserMessagesInConversation",
                     0,
                 )
                 if messages_left == 0:
                     raise Exception("Max messages reached")
                 message = ""
                 for msg in reversed(response["item"]["messages"]):
@@ -172,54 +187,56 @@
                     ],
                     "adaptive_text": adaptive_text,
                     "media": media
                 }
         return {}
 
     async def ask_stream(
-        self,
-        prompt: str,
-        wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
-        conversation_style: CONVERSATION_STYLE_TYPE = None,
-        raw: bool = False,
-        webpage_context: str | None = None,
-        search_result: bool = False,
-        locale: str = guess_locale(),
-        mode: str = None,
-        no_search: bool = True,
-        persona: Persona = Persona.copilot,
-        plugins: set[Plugin] = {}
+            self,
+            prompt: str,
+            wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
+            conversation_style: CONVERSATION_STYLE_TYPE = None,
+            raw: bool = False,
+            webpage_context: str | None = None,
+            search_result: bool = False,
+            locale: str = guess_locale(),
+            mode: str = None,
+            no_search: bool = True,
+            persona: Persona = Persona.copilot,
+            plugins: set[Plugin] = {},
+            image_url: str = None,
     ) -> Generator[bool, dict | str, None]:
         """
         Ask a question to the bot
         """
         async for response in self.chat_hub.ask_stream(
-            prompt=prompt,
-            conversation_style=conversation_style,
-            wss_link=wss_link,
-            raw=raw,
-            webpage_context=webpage_context,
-            locale=locale,
-            no_search=no_search,
-            persona=persona,
-            plugins=plugins
+                prompt=prompt,
+                conversation_style=conversation_style,
+                wss_link=wss_link,
+                raw=raw,
+                webpage_context=webpage_context,
+                locale=locale,
+                no_search=no_search,
+                persona=persona,
+                plugins=plugins,
+                image_url=image_url
         ):
             yield response
 
     async def close(self) -> None:
         """
         Close the connection
         """
         await self.chat_hub.close()
 
     async def delete_conversation(
-        self,
-        conversation_id: str = None,
-        conversation_signature: str = None,
-        client_id: str = None,
+            self,
+            conversation_id: str = None,
+            conversation_signature: str = None,
+            client_id: str = None,
     ) -> None:
         """
         Delete the chat in the server
         """
         await self.chat_hub.delete_conversation(
             conversation_id=conversation_id,
             conversation_signature=conversation_signature,
@@ -237,12 +254,20 @@
         await self.close()
         self.chat_hub = ChatHub(
             await Conversation.create(self.proxy, cookies=self.chat_hub.cookies),
             proxy=self.proxy,
             cookies=self.chat_hub.cookies,
         )
 
+    async def upload_image(
+            self,
+            binary_image: bytes,
+            style: CONVERSATION_STYLE_TYPE = "precise",
+            blur: bool = False
+    ) -> dict:
+        return await self.chat_hub.upload_image(binary_image,style,blur)
+
 
 if __name__ == "__main__":
     from .main import main
 
     main()
```

### Comparing `edgegpt_fork-1.0.0/src/EdgeGPT/EdgeUtils.py` & `edgegpt_fork-1.0.1/src/EdgeGPT/EdgeUtils.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.0/src/EdgeGPT/chathub.py` & `edgegpt_fork-1.0.1/src/EdgeGPT/chathub.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import asyncio
+import base64
 import json
 import os
 from time import time
 from typing import Generator, List, Union, Optional, Tuple
 
 from curl_cffi import requests
 from curl_cffi.requests.websockets import WebSocket
 from curl_cffi.const import CurlWsFlag
 from curl_cffi import AsyncCurl
+from curl_cffi.curl import CurlMime
 import urllib
 from BingImageCreator import ImageGenAsync
 
 from .constants import DELIMITER, PERSONATE
 from .constants import HEADERS
 from .constants import HEADERS_INIT_CONVER
 from .conversation import Conversation
@@ -93,17 +95,21 @@
             wss_link: str = None,
             conversation_style: CONVERSATION_STYLE_TYPE = None,
             raw: bool = False,
             webpage_context: Union[str, None] = None,
             locale: str = guess_locale(),
             no_search: bool = True,
             persona: Persona = Persona.copilot,
-            plugins: set[Plugin] = {}
+            plugins: set[Plugin] = {},
+            image_url: str = None,
     ) -> Generator[bool, Union[dict, str], None]:
         """ """
+        if (not prompt) and (not image_url):
+            raise ValueError("prompt or image_url must be provided")
+
         cookies = {}
         if self.cookies is not None:
             for cookie in self.cookies:
                 cookies[cookie["name"]] = cookie["value"]
         # self.aio_session = aiohttp.ClientSession(cookies=cookies)
         self.aio_session = AsyncSession(
             cookies=cookies,
@@ -120,26 +126,23 @@
         self.request.update(
             prompt=prompt,
             conversation_style=conversation_style,
             webpage_context=webpage_context,
             locale=locale,
             no_search=no_search,
             persona=persona,
-            plugins=plugins
+            plugins=plugins,
+            image_url=image_url,
         )
         # Send request
         await wss.asend(append_identifier(self.request.struct).encode("utf-8"))
         resp_txt = ""
         generate = None
-        new_line = "\n"
-        search_hint = "Searching the web for:\n"
         search_refs = []
-        images = []
-        search_keywords = ""
-        offset = 0
+        search_keywords = []
         async for obj in self._receive_messages(wss):
             if int(time()) % 6 == 0:
                 await wss.asend(append_identifier({"type": 6}).encode("utf-8"))
 
             if obj is None or not obj:
                 continue
 
@@ -150,77 +153,80 @@
 
             if raw:
                 done = r_type == 2
                 yield done, response
                 if not done:
                     continue
                 else:
-                    return
+                    break
 
             if r_type == 1 and response["arguments"][0].get(
                     "messages",
             ):
                 message = response["arguments"][0]["messages"][0]
                 msg_type = message.get("messageType")
                 hidden_text = message.get("hiddenText")
                 text = message.get("text")
                 if msg_type == "InternalSearchQuery":
-                    search_keywords = f"{search_keywords}\n{search_hint}{hidden_text}\n"
-                    resp_txt = search_keywords
+                    search_keywords.append(hidden_text)
                 elif msg_type == "InternalSearchResult":
                     search_refs += parse_search_result(message)
                 elif msg_type == "GenerateContentQuery":
                     generate = {
                         "content_type": message.get("contentType"),
                         "prompt": text
                     }
                 elif msg_type is None:
                     if message.get("contentOrigin") == "Apology":
                         print('message has been revoked')
                         print(message)
-                        result = f"{message.get('text')} -end- (message has been revoked)"
-                        resp_txt = f"{resp_txt}\n{result}"
+                        resp_txt = f"{resp_txt}{text} -end- (message has been revoked)"
 
-                    text = new_line + text
-                    resp_txt = f"{resp_txt}{text[offset:]}"
-                    offset = len(text)
-                    new_line = ""
+                    if len(search_keywords) > 0:
+                        keywords = "\n* ".join(search_keywords)
+                        resp_txt = f"{resp_txt}Searching the web for:\n* {keywords}\n\n"
+                        search_keywords = []
 
-                yield False, resp_txt
+                    yield False, f"{resp_txt}{text}"
             elif response.get("type") == 2:
                 if response["item"]["result"].get("error"):
                     raise Exception(
                         f"{response['item']['result']['value']}: {response['item']['result']['message']}",
                     )
 
+                response["media"] = {}
                 message = response["item"]["messages"][-1]
+                text = message.get("text")
                 if generate:
                     if generate["content_type"] == "IMAGE":
                         async with ImageGenAsync(
                                 all_cookies=self.cookies,
                                 proxy=self.proxy
                         ) as image_obj:
                             try:
                                 images = await image_obj.get_images(generate["prompt"])
+                                response["media"] = {
+                                    "prompt": generate["prompt"],
+                                    "images": images
+                                }
                             except Exception as e:
                                 print(str(e))
                                 hint = "Your prompt has been prohibited by third-service. Please modify it."
-                                resp_txt = f"{resp_txt}\n{e}\n{hint}"
+                                resp_txt = f"{resp_txt}{text}\n{e}\n{hint}"
 
                 if len(search_refs) > 0:
                     refs_str = ""
                     for index, item in enumerate(search_refs):
                         refs_str += f'- [^{index}^] [{item["title"]}]({item["url"]})\n'
 
-                    resp_txt = f"{resp_txt}\n{refs_str}"
+                    resp_txt = f"{resp_txt}{text}\n{refs_str}"
 
                 message["text"] = resp_txt
-                response["media"] = {
-                    "images": images
-                }
+                if "media" not in response:
+                    response["media"] = {}
 
                 yield True, response
                 return
 
     async def _initial_handshake(self, wss) -> None:
         proto = append_identifier({"protocol": "json", "version": 1})
         await wss.asend(proto.encode("utf-8"))
@@ -278,14 +284,64 @@
                 "optionsSets": ["autosave"],
             },
         )
 
     async def close(self) -> None:
         await self.session.close()
 
+    async def upload_image(
+            self,
+            binary_image: bytes,
+            style: CONVERSATION_STYLE_TYPE = "precise",
+            blur: bool = False
+    ) -> dict:
+        if not isinstance(style, str):
+            style = style.name
+
+        url = "https://www.bing.com/images/kblob"
+        payload = {
+            "imageInfo": {},
+            "knowledgeRequest": {
+                "invokedSkills": ["ImageById"],
+                "subscriptionId": "Bing.Chat.Multimodal",
+                "invokedSkillsRequestData": {"enableFaceBlur": blur},
+                "convoData": {
+                    "convoid": "",
+                    "convotone": style,
+                }
+            }
+        }
+        encode_data = base64.b64encode(binary_image)
+
+        parts = CurlMime()
+        parts.addpart(
+            name="knowledgeRequest",
+            content_type="application/json",
+            data=json.dumps(payload).encode("utf-8"),
+        )
+        parts.addpart(
+            name="imageBase64",
+            content_type="application/octet-stream",
+            data=encode_data,
+        )
+
+        async with AsyncSession(
+            headers={
+                "Referer": "https://www.bing.com/search?q=Bing+AI&showconv=1&FORM=hpcodx"
+            },
+            proxy=self.proxy,
+            impersonate=PERSONATE,
+            timeout=900,
+        ) as session:
+            resp = await session.post(url, multipart=parts)
+            if not resp.ok:
+                raise Exception(f"Failed to upload image. Status: {resp.status}")
+
+            return resp.json()
+
 
 class AsyncSession(requests.AsyncSession):
     def __init__(
             self,
             *,
             loop=None,
             async_curl: Optional[AsyncCurl] = None,
```

### Comparing `edgegpt_fork-1.0.0/src/EdgeGPT/constants.py` & `edgegpt_fork-1.0.1/src/EdgeGPT/constants.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.0/src/EdgeGPT/conversation.py` & `edgegpt_fork-1.0.1/src/EdgeGPT/conversation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import json
 import os
-from tkinter import NO
 from typing import List
 from typing import Union
 
-# import httpx.AsyncClient/
-from httpx import AsyncClient
 from curl_cffi import requests
 from curl_cffi.requests import AsyncSession
 
 from .constants import HEADERS_INIT_CONVER
 from .exceptions import NotAllowedToAccess
 
 
@@ -60,14 +57,15 @@
         if 'X-Sydney-Encryptedconversationsignature' in response.headers:
             self.struct['secAccessToken'] = response.headers['X-Sydney-Encryptedconversationsignature']
 
     @staticmethod
     async def create(
         proxy: Union[str, None] = None,
         cookies: Union[List[dict], None] = None,
+        conversation_id: Union[str, None] = None,
     ) -> "Conversation":
         self = Conversation(async_mode=True)
         self.struct = {
             "conversationId": None,
             "clientId": None,
             "conversationSignature": None,
             "secAccessToken": None,
@@ -89,14 +87,17 @@
             headers=HEADERS_INIT_CONVER,
             proxy=proxy,
             impersonate="chrome116",
         ) as s:
             for cookie in cookies:
                 s.cookies.set(cookie["name"], cookie["value"])
             url = os.environ.get("BING_PROXY_URL") or "https://www.bing.com/turing/conversation/create"
+            if conversation_id:
+                url += f"?conversationId={conversation_id}"
+
             response = await s.get(url=url)
             if response.status_code != 200:
                 print(f"Status code: {response.status_code}")
                 print(response.text)
                 print(response.url)
                 raise Exception("Authentication failed")
```

### Comparing `edgegpt_fork-1.0.0/src/EdgeGPT/conversation_style.py` & `edgegpt_fork-1.0.1/src/EdgeGPT/conversation_style.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.0/src/EdgeGPT/locale.py` & `edgegpt_fork-1.0.1/src/EdgeGPT/locale.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.0/src/EdgeGPT/main.py` & `edgegpt_fork-1.0.1/src/EdgeGPT/main.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.0/src/EdgeGPT/plugin.py` & `edgegpt_fork-1.0.1/src/EdgeGPT/plugin.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.0/src/EdgeGPT/request.py` & `edgegpt_fork-1.0.1/src/EdgeGPT/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,53 +30,51 @@
             self,
             prompt: str,
             conversation_style: CONVERSATION_STYLE_TYPE,
             webpage_context: Union[str, None] = None,
             locale: str = guess_locale(),
             no_search: bool = True,
             persona: Persona = Persona.copilot,
-            plugins: set[Plugin] = {}
+            plugins: set[Plugin] = {},
+            image_url: str = None,
     ) -> None:
         options = [
             "deepleo",
             "enable_debug_commands",
             "disable_emoji_spoken_text",
             "enablemm",
         ]
         if conversation_style:
             if not isinstance(conversation_style, ConversationStyle):
                 conversation_style = getattr(ConversationStyle, conversation_style)
             options = conversation_style.value.copy()
-        #enable gpt4_turbo deprecated
-        # if mode == 'gpt4-turbo':
-        #     options.append('gpt4tmncnp')
 
         plugin_params = []
-        isSearchNeededforPlugin = False
+        is_search_needed_for_plugin = False
         for plugin in plugins:
             val = plugin.value
-            if (val.id is not None):
+            if val.id is not None:
                 plugin_params.append({
                     "id": val.id,
                     "category": 1
                 })
 
-            if (val.option_set is not None):
+            if val.option_set is not None:
                 options.append(val.option_set)
 
-            if (not isSearchNeededforPlugin) and plugin != Plugin.codeInterpreter:
-                isSearchNeededforPlugin = True
+            if (not is_search_needed_for_plugin) and plugin != Plugin.codeInterpreter:
+                is_search_needed_for_plugin = True
 
-        if isSearchNeededforPlugin and (Plugin.search not in plugins):
+        if is_search_needed_for_plugin and (Plugin.search not in plugins):
             plugin_params.append({
                 "id": Plugin.search.value.id,
                 "category": 1
             })
 
-        if (not isSearchNeededforPlugin) and no_search:
+        if (not is_search_needed_for_plugin) and no_search:
             options.append('nosearchall')
 
         options.append(persona.value)
 
         message_id = str(uuid.uuid4())
         # Get the current local time
         now_local = datetime.now()
@@ -92,14 +90,30 @@
         offset_minutes = int((timezone_offset.total_seconds() % 3600) // 60)
 
         # Format the offset as a string
         offset_string = f"{offset_hours:+03d}:{offset_minutes:02d}"
 
         # Get current time
         timestamp = datetime.now().strftime("%Y-%m-%dT%H:%M:%S") + offset_string
+        message = {
+            "locale": locale,
+            "market": locale,
+            "region": locale[-2:],  # en-US -> US
+            "locationHints": get_location_hint_from_locale(locale),
+            "timestamp": timestamp,
+            "author": "user",
+            "inputMethod": "Keyboard",
+            "text": prompt,
+            "messageType": "Chat",
+            "messageId": message_id,
+            "requestId": message_id,
+        }
+        if image_url is not None:
+            message["imageUrl"] = image_url
+
         self.struct = {
             "arguments": [
                 {
                     "source": "cib",
                     "optionsSets": options,
                     "allowedMessageTypes": [
                         "ActionRequest",
@@ -149,27 +163,15 @@
                     ],
                     "verbosity": "verbose",
                     "scenario": "SERP",
                     "plugins": plugin_params,
                     "traceId": get_ran_hex(32),
                     "gptId": persona.name,
                     "isStartOfSession": self.invocation_id == 3,
-                    "message": {
-                        "locale": locale,
-                        "market": locale,
-                        "region": locale[-2:],  # en-US -> US
-                        "locationHints": get_location_hint_from_locale(locale),
-                        "timestamp": timestamp,
-                        "author": "user",
-                        "inputMethod": "Keyboard",
-                        "text": prompt,
-                        "messageType": "Chat",
-                        "messageId": message_id,
-                        "requestId": message_id,
-                    },
+                    "message": message,
                     "tone": conversation_style.name.capitalize(),  # Make first letter uppercase
                     "requestId": message_id,
                     "conversationSignature": self.conversation_signature,
                     "participant": {
                         "id": self.client_id,
                     },
                     "conversationId": self.conversation_id,
```

### Comparing `edgegpt_fork-1.0.0/src/EdgeGPT/utilities.py` & `edgegpt_fork-1.0.1/src/EdgeGPT/utilities.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/PKG-INFO` & `edgegpt_fork-1.0.1/src/EdgeGPT_fork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT-fork
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/xingty/EdgeGPT
 Author: Antonio Cheong,Bigbyto
 Author-email: acheong@student.dalat.org,bigbyto@gmail.com
 License: The Unlicense
 Project-URL: Bug Report, https://github.com/xingty/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT-fork Version: 1.0.0 Summary: Reverse
+Metadata-Version: 2.1 Name: EdgeGPT-fork Version: 1.0.1 Summary: Reverse
 engineered Edge Chat API Home-page: https://github.com/xingty/EdgeGPT Author:
 Antonio Cheong,Bigbyto Author-email:
 acheong@student.dalat.org,bigbyto@gmail.com License: The Unlicense Project-URL:
 Bug Report, https://github.com/xingty/EdgeGPT/issues/new Classifier: License ::
 OSI Approved :: The Unlicense (Unlicense) Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/SOURCES.txt` & `edgegpt_fork-1.0.1/src/EdgeGPT_fork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

