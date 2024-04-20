# Comparing `tmp/mxbt-0.3.3.tar.gz` & `tmp/mxbt-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxbt-0.3.3.tar", last modified: Sun Mar 10 20:17:28 2024, max compression
+gzip compressed data, was "mxbt-0.3.4.tar", last modified: Sat Apr 20 08:58:13 2024, max compression
```

## Comparing `mxbt-0.3.3.tar` & `mxbt-0.3.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-03-10 20:17:28.394009 mxbt-0.3.3/
--rw-r--r--   0 warlock   (1000) warlock   (1000)    35149 2024-02-22 07:41:55.000000 mxbt-0.3.3/LICENSE
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2722 2024-03-10 20:17:28.394009 mxbt-0.3.3/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1975 2024-03-10 20:16:34.000000 mxbt-0.3.3/README.md
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-03-10 20:17:28.394009 mxbt-0.3.3/mxbt/
--rw-r--r--   0 warlock   (1000) warlock   (1000)      240 2024-03-10 20:15:53.000000 mxbt-0.3.3/mxbt/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)    20522 2024-03-10 20:15:41.000000 mxbt-0.3.3/mxbt/api.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     5291 2024-02-22 07:41:55.000000 mxbt-0.3.3/mxbt/auth.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     5659 2024-03-10 18:52:54.000000 mxbt-0.3.3/mxbt/bot.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     3372 2024-03-10 20:12:26.000000 mxbt-0.3.3/mxbt/callbacks.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     7211 2024-03-10 20:14:57.000000 mxbt-0.3.3/mxbt/context.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     7373 2024-02-22 07:41:55.000000 mxbt-0.3.3/mxbt/filters.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     5682 2024-02-22 07:41:55.000000 mxbt-0.3.3/mxbt/listener.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     3939 2024-02-22 07:41:55.000000 mxbt-0.3.3/mxbt/match.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2425 2024-02-22 07:41:55.000000 mxbt-0.3.3/mxbt/module.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-03-10 20:17:28.394009 mxbt-0.3.3/mxbt/types/
--rw-r--r--   0 warlock   (1000) warlock   (1000)       44 2024-02-22 07:41:55.000000 mxbt-0.3.3/mxbt/types/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      279 2024-02-22 07:41:55.000000 mxbt-0.3.3/mxbt/types/command.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     4669 2024-03-10 15:49:10.000000 mxbt-0.3.3/mxbt/types/file.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      282 2024-02-22 07:41:55.000000 mxbt-0.3.3/mxbt/utils.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-03-10 20:17:28.394009 mxbt-0.3.3/mxbt.egg-info/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2722 2024-03-10 20:17:28.000000 mxbt-0.3.3/mxbt.egg-info/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)      393 2024-03-10 20:17:28.000000 mxbt-0.3.3/mxbt.egg-info/SOURCES.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-03-10 20:17:28.000000 mxbt-0.3.3/mxbt.egg-info/dependency_links.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       80 2024-03-10 20:17:28.000000 mxbt-0.3.3/mxbt.egg-info/requires.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        5 2024-03-10 20:17:28.000000 mxbt-0.3.3/mxbt.egg-info/top_level.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-03-10 20:17:28.394009 mxbt-0.3.3/setup.cfg
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1032 2024-02-22 07:41:55.000000 mxbt-0.3.3/setup.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-20 08:58:13.619880 mxbt-0.3.4/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)    35149 2024-03-11 08:01:52.000000 mxbt-0.3.4/LICENSE
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3034 2024-04-20 08:58:13.619880 mxbt-0.3.4/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2287 2024-04-20 08:57:14.000000 mxbt-0.3.4/README.md
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-20 08:58:13.619880 mxbt-0.3.4/mxbt/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      240 2024-04-20 08:56:19.000000 mxbt-0.3.4/mxbt/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)    20638 2024-04-20 07:22:09.000000 mxbt-0.3.4/mxbt/api.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     5465 2024-04-06 15:56:45.000000 mxbt-0.3.4/mxbt/auth.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     5897 2024-04-11 12:46:01.000000 mxbt-0.3.4/mxbt/bot.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3372 2024-04-11 12:46:01.000000 mxbt-0.3.4/mxbt/callbacks.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     7211 2024-03-11 08:01:52.000000 mxbt-0.3.4/mxbt/context.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     9633 2024-04-06 16:48:20.000000 mxbt-0.3.4/mxbt/filters.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     5682 2024-03-11 08:01:52.000000 mxbt-0.3.4/mxbt/listener.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3938 2024-04-06 16:48:25.000000 mxbt-0.3.4/mxbt/match.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2425 2024-03-11 08:01:52.000000 mxbt-0.3.4/mxbt/module.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-20 08:58:13.619880 mxbt-0.3.4/mxbt/types/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       67 2024-04-06 16:48:53.000000 mxbt-0.3.4/mxbt/types/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      279 2024-03-11 08:01:52.000000 mxbt-0.3.4/mxbt/types/command.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)    10011 2024-04-20 08:55:59.000000 mxbt-0.3.4/mxbt/types/file.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      178 2024-04-06 16:47:24.000000 mxbt-0.3.4/mxbt/types/msgtype.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      281 2024-04-11 12:46:01.000000 mxbt-0.3.4/mxbt/utils.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-20 08:58:13.619880 mxbt-0.3.4/mxbt.egg-info/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3034 2024-04-20 08:58:13.000000 mxbt-0.3.4/mxbt.egg-info/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      415 2024-04-20 08:58:13.000000 mxbt-0.3.4/mxbt.egg-info/SOURCES.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-20 08:58:13.000000 mxbt-0.3.4/mxbt.egg-info/dependency_links.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       80 2024-04-20 08:58:13.000000 mxbt-0.3.4/mxbt.egg-info/requires.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        5 2024-04-20 08:58:13.000000 mxbt-0.3.4/mxbt.egg-info/top_level.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-20 08:58:13.619880 mxbt-0.3.4/setup.cfg
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1032 2024-03-11 08:01:52.000000 mxbt-0.3.4/setup.py
```

### Comparing `mxbt-0.3.3/LICENSE` & `mxbt-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.3/PKG-INFO` & `mxbt-0.3.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxbt
-Version: 0.3.3
+Version: 0.3.4
 Summary: Yet another Matrix bot library.
 Home-page: https://codeberg.org/librehub/mxbt
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,matrix-nio,matrix,bot,api
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -19,25 +19,52 @@
 Requires-Dist: markdown
 Requires-Dist: python-cryptography-fernet-wrapper
 Requires-Dist: filetype
 Requires-Dist: aiofiles
 
 # mxbt 
 
-Yet another Matrix bot library.
+Yet another Matrix bot library, built on [matrix-nio](https://github.com/matrix-nio/matrix-nio).
+
+## Feauters
+
+- [x] Simple and powerfull bots creating
+- [ ] Custom emojis support
+    - [x] Getting
+    - [x] Sending
+    - [ ] Creating
+- [x] Files sending
+    - [x] External files
+    - [x] Internal files
+- [x] Native mentions
+- [x] Access to `matrix-nio` features
+- [x] Event filters
+- [x] Bot modules support
+- [ ] Wait for event system
+- [ ] Full e2ee support
 
 ## Installation
 
+**With pip:**
+
 ```sh
 $ pip install mxbt
 ```
 
+**With git and python:**
+
+```sh
+$ git clone https://codeberg.org/librehub/mxbt
+$ cd mxbt
+$ python -m pip install . 
+```
+
 ## Getting started
 
-More examples [here](examples/). Or in [docs](https://librehub.codeberg.page/mxbt/).
+More examples [here](examples/) or in [docs](https://librehub.codeberg.page/mxbt/).
 
 ```python
 from mxbt import Bot, Context, Creds, Filter
 
 bot = Bot(
     prefix="!",          # Standart command prefix, commands can setup it own prefix
     creds=Creds.from_json_file("credits.json")
@@ -69,16 +96,12 @@
 
 ## Special thanks
 
 * [simplematrixbotlib](https://codeberg.org/imbev/simplematrixbotlib) for base parts of API, Listener and Callbacks code ideas. 
 Code from simplematrixbotlib is included under the terms of the MIT license - Copyright (c) 2021-2023 Isaac Beverly
 * [matrix-nio](https://github.com/poljar/matrix-nio) for cool client library.
 
-## Contacts
+## Support
 
-| Contact                                               | Description       |
-| :---:                                                 | :---              |
-| [`Matrix`](https://matrix.to/#/#librehub:matrix.org)  | Matrix server     |
+Any contacts and crytpocurrency wallets you can find on my [profile page](https://warlock.codeberg.page).
 
-## Donates
-**Monero/XMR:** `47KkgEb3agJJjSpeW1LpVi1M8fsCfREhnBCb1yib5KQgCxwb6j47XBQAamueByrLUceRinJqveZ82UCbrGqrsY9oNuZ97xN`
```

### Comparing `mxbt-0.3.3/mxbt/api.py` & `mxbt-0.3.4/mxbt/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,31 +240,31 @@
                 content=content,
                 ignore_unverified_devices=ignore_unverified_devices)
             if isinstance(res, RoomSendResponse):
                 res = await self.async_client.room_get_event(res.room_id, res.event_id)
                 if isinstance(res, RoomGetEventResponse):
                     return res.event
 
-    async def __send(self, room_id: str, body: str | File,
+    async def __send(self, room_id: str, body: str | File | FileUrl,
                      use_html: bool, reply_to: str="", edit_id: str="",
                      mentions: list[str]=list(), emotes: list[str]=list()):
         if isinstance(body, str):
             if use_html: 
                 return await self.send_markdown(room_id, body,
                                          reply_to=reply_to,
                                          edit_id=edit_id,
                                          mentions=mentions,
                                          emotes=emotes)
             else: 
                 return await self.send_text(room_id, body,
                                      reply_to=reply_to,
                                      edit_id=edit_id,
                                      mentions=mentions)
-        elif isinstance(body, File):
-            return await self.send_file(room_id, body.path, reply_to=reply_to, edit_id=edit_id)
+        elif isinstance(body, (File, FileUrl)):
+            return await self.send_file(room_id, body, reply_to=reply_to, edit_id=edit_id)
 
     def _add_relations(self, content: dict, reply_to: str, edit_id: str) -> dict:
         """
         Add edit or reply info to content dict
         """
         if edit_id != "":
             content['m.new_content'] = content.copy()
@@ -368,15 +368,15 @@
         """
         Kick user from room
         """
         if self.async_client is None:
             raise Exception("AsyncClient is None!")
         return await self.async_client.room_kick(room_id, user_id, reason)
 
-    async def send(self, room_id: str, body: str | File,
+    async def send(self, room_id: str, body: str | File | FileUrl,
                    use_html: bool=False, mentions: list[str]=list(),
                    emotes: list[str]=list()):
         """
         Send text or file to room
 
         Parameters:
         -------------
@@ -489,22 +489,24 @@
                 }
             },
             message_type="m.reaction"
         )
 
     async def send_file(
             self, room_id: str,
-            filepath: str,
+            file: File | FileUrl,
             reply_to: str="",
             edit_id: str="") -> tuple[MatrixRoom, RoomMessageImage | RoomMessageVideo | RoomMessageFile] | None:
         if self.async_client is None:
             raise ValueError("AsyncClient is None!")
 
-        file = File(filepath)
-        content = await file.upload(self.async_client)
+        if isinstance(file, File):
+            content = await file.upload(self.async_client)
+        else:
+            content = await file.to_file(self.async_client)
         if content is None: return
 
         content = self._add_relations(
             content, reply_to, edit_id
         )
 
         try:
```

### Comparing `mxbt-0.3.3/mxbt/auth.py` & `mxbt-0.3.4/mxbt/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
     def __init__(self,
                  homeserver,
                  username=None,
                  password=None,
                  login_token=None,
                  access_token=None,
-                 session_stored_file='session.txt'):
+                 session_stored_file='session.txt',
+                 device_name: str='mxbt') -> None:
         """
         Initializes the simplematrixbotlib.Creds class.
 
         Parameters
         ----------
         homeserver : str
             The homeserver for the bot to connect to. Begins with "https://".
@@ -51,23 +52,25 @@
 
         access_token : str, optional
             The access_token for the bot to connect with. Can be used instead of password. One of the password, login_token, or access_token must be provided.
 
         session_stored_file : str, optional
             Location for the bot to read and write device_id and access_token. The data within this file is encrypted and decrypted with the password parameter using the cryptography package. If set to None, session data will not be saved to file.
 
+        device_name : str, optional
+            Name display in the list of sessions. Useful to identified the device.
         """
 
         self.homeserver = homeserver
         self.username = username
         self.password = password
         self.login_token = login_token
         self.access_token = access_token
         self._session_stored_file = session_stored_file
-        self.device_name = "mxbt"
+        self.device_name = device_name
         self.device_id = ""
 
         if self.password:
             self._key = fw.key_from_pass(self.password)
         elif self.login_token:
             self._key = fw.key_from_pass(self.login_token)
         elif self.access_token:
```

### Comparing `mxbt-0.3.3/mxbt/bot.py` & `mxbt-0.3.4/mxbt/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,16 +138,20 @@
         """
         On reaction event listener
         """
         def wrapper(func) -> None:
            self.listener.on_reaction(func) 
         return wrapper
 
-    async def main(self) -> None:
+    async def connect(self) -> None:
         """
+        Main method of mxbt.Bot. Implements bot login and forever sync.
+
+        Can be runed with mxbt.Bot.run method or with asyncio.run(bot.connect())
+
         Implementation from:
         https://codeberg.org/imbev/simplematrixbotlib/src/branch/master/simplematrixbotlib/bot.py
         """
         try:
             self.creds.session_read_file()
         except cryptography.fernet.InvalidToken:
             print("Invalid Stored Token")
@@ -183,9 +187,12 @@
         for action in self.listener._startup_registry:
             for room_id in self.async_client.rooms:
                 await action(room_id)
 
         await self.async_client.sync_forever(timeout=3000, full_state=True)
 
     def run(self) -> None:
-        asyncio.run(self.main())
+        """
+        Run mxbt.Bot.connect method with asyncio.run
+        """
+        asyncio.run(self.connect())
```

### Comparing `mxbt-0.3.3/mxbt/callbacks.py` & `mxbt-0.3.4/mxbt/callbacks.py`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.3/mxbt/context.py` & `mxbt-0.3.4/mxbt/context.py`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.3/mxbt/filters.py` & `mxbt-0.3.4/mxbt/filters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from enum import Enum
 from nio import MatrixRoom
 
+from .types.msgtype import MsgType
 from .context import Context
 from .match import Match
 
 class Filter:
 
     @staticmethod
     def __find_context(args) -> Context | None:
@@ -14,34 +16,41 @@
     @staticmethod
     def __find_context_body(args) -> tuple | None:
         for index, arg in enumerate(args):
             if isinstance(arg, MatrixRoom):
                 return args[index:]
 
     @staticmethod
-    def msgtype(values: list[str]):
+    def msgtype(values: list[str | MsgType]):
         """
         Filter events with msgtype 
 
         filter params:
         ----------------
-        values: list[str]
+        values: list[str | mxbt.enums.MsgType]
             list of accepted msgtypes
         """
+        new_values = list()
+        for value in values:
+            if isinstance(value, Enum):
+                new_values.append(value.value)
+            else:
+                new_values.append(value)
+
         def wrapper(func):
             async def command_func(*args) -> None:
                 ctx = Filter.__find_context(args)
                 if not ctx is None:
-                    if ctx.event.source['content']['msgtype'] in values:
+                    if ctx.event.source['content']['msgtype'] in new_values:
                         await func(*args)
                 else:
                     body = Filter.__find_context_body(args)
                     if body is None: return
                     _, event = body
-                    if event.source['content']['msgtype'] in values:
+                    if event.source['content']['msgtype'] in new_values:
                         await func(*args)
             return command_func
         return wrapper
 
     @staticmethod
     def has_text(values: list[str]):
         """
@@ -71,15 +80,15 @@
     def from_rooms(rooms: list):
         """
         from_rooms event filter
 
         filter params:
         ----------------
         rooms: list[str] 
-            list of user_id, who is accepted to send event
+            list of room_id, who is accepted to send event
 
         func params:
         --------------
         room: MatrixRoom,
         event: Event
 
         or 
@@ -98,14 +107,48 @@
                     room, _ = body
                     if Match.is_from_rooms(room.room_id, rooms):
                         await func(*args)
             return command_func
         return wrapper
 
     @staticmethod
+    def not_from_rooms(rooms: list):
+        """
+        not_from_rooms event filter
+
+        filter params:
+        ----------------
+        rooms: list[str] 
+            list of room_id, who is denied to send event
+
+        func params:
+        --------------
+        room: MatrixRoom,
+        event: Event
+
+        or 
+
+        ctx: Context
+        """
+        def wrapper(func):
+            async def command_func(*args) -> None:
+                ctx = Filter.__find_context(args)
+                if not ctx is None:
+                    if not Match.is_from_rooms(ctx.room.room_id, rooms):
+                        await func(*args)
+                else:
+                    body = Filter.__find_context_body(args)
+                    if body is None: return
+                    room, _ = body
+                    if not Match.is_from_rooms(room.room_id, rooms):
+                        await func(*args)
+            return command_func
+        return wrapper
+
+    @staticmethod
     def from_users(users: list):
         """
         from_users event filter
 
         filter params:
         ----------------
         users: list[str]
@@ -132,14 +175,48 @@
                     _, message = body
                     if Match.is_from_users(message.sender, users):
                         await func(*args)
             return command_func
         return wrapper
 
     @staticmethod
+    def not_from_users(users: list):
+        """
+        not_from_users event filter
+
+        filter params:
+        ----------------
+        users: list[str]
+            list of user_id, who is denied to send event
+
+        func params:
+        --------------
+        room: MatrixRoom,
+        event: Event
+
+        or 
+
+        ctx: Context
+        """
+        def wrapper(func):
+            async def command_func(*args) -> None:
+                ctx = Filter.__find_context(args)
+                if not ctx is None:
+                    if not Match.is_from_users(ctx.sender, users):
+                        await func(*args)
+                else:
+                    body = Filter.__find_context_body(args)
+                    if body is None: return
+                    _, message = body
+                    if not Match.is_from_users(message.sender, users):
+                        await func(*args)
+            return command_func
+        return wrapper
+
+    @staticmethod
     def sender_can_ban():
         """
         sender_can_ban event filter
 
         func params:
         --------------
         room: MatrixRoom,
```

### Comparing `mxbt-0.3.3/mxbt/listener.py` & `mxbt-0.3.4/mxbt/listener.py`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.3/mxbt/match.py` & `mxbt-0.3.4/mxbt/match.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from nio import MatrixRoom
 
-
 class Match:
     """
     Class with methods to filter events
 
     ...
 
     """
```

### Comparing `mxbt-0.3.3/mxbt/module.py` & `mxbt-0.3.4/mxbt/module.py`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.3/mxbt.egg-info/PKG-INFO` & `mxbt-0.3.4/mxbt.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxbt
-Version: 0.3.3
+Version: 0.3.4
 Summary: Yet another Matrix bot library.
 Home-page: https://codeberg.org/librehub/mxbt
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,matrix-nio,matrix,bot,api
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -19,25 +19,52 @@
 Requires-Dist: markdown
 Requires-Dist: python-cryptography-fernet-wrapper
 Requires-Dist: filetype
 Requires-Dist: aiofiles
 
 # mxbt 
 
-Yet another Matrix bot library.
+Yet another Matrix bot library, built on [matrix-nio](https://github.com/matrix-nio/matrix-nio).
+
+## Feauters
+
+- [x] Simple and powerfull bots creating
+- [ ] Custom emojis support
+    - [x] Getting
+    - [x] Sending
+    - [ ] Creating
+- [x] Files sending
+    - [x] External files
+    - [x] Internal files
+- [x] Native mentions
+- [x] Access to `matrix-nio` features
+- [x] Event filters
+- [x] Bot modules support
+- [ ] Wait for event system
+- [ ] Full e2ee support
 
 ## Installation
 
+**With pip:**
+
 ```sh
 $ pip install mxbt
 ```
 
+**With git and python:**
+
+```sh
+$ git clone https://codeberg.org/librehub/mxbt
+$ cd mxbt
+$ python -m pip install . 
+```
+
 ## Getting started
 
-More examples [here](examples/). Or in [docs](https://librehub.codeberg.page/mxbt/).
+More examples [here](examples/) or in [docs](https://librehub.codeberg.page/mxbt/).
 
 ```python
 from mxbt import Bot, Context, Creds, Filter
 
 bot = Bot(
     prefix="!",          # Standart command prefix, commands can setup it own prefix
     creds=Creds.from_json_file("credits.json")
@@ -69,16 +96,12 @@
 
 ## Special thanks
 
 * [simplematrixbotlib](https://codeberg.org/imbev/simplematrixbotlib) for base parts of API, Listener and Callbacks code ideas. 
 Code from simplematrixbotlib is included under the terms of the MIT license - Copyright (c) 2021-2023 Isaac Beverly
 * [matrix-nio](https://github.com/poljar/matrix-nio) for cool client library.
 
-## Contacts
+## Support
 
-| Contact                                               | Description       |
-| :---:                                                 | :---              |
-| [`Matrix`](https://matrix.to/#/#librehub:matrix.org)  | Matrix server     |
+Any contacts and crytpocurrency wallets you can find on my [profile page](https://warlock.codeberg.page).
 
-## Donates
-**Monero/XMR:** `47KkgEb3agJJjSpeW1LpVi1M8fsCfREhnBCb1yib5KQgCxwb6j47XBQAamueByrLUceRinJqveZ82UCbrGqrsY9oNuZ97xN`
```

### Comparing `mxbt-0.3.3/setup.py` & `mxbt-0.3.4/setup.py`

 * *Files identical despite different names*

